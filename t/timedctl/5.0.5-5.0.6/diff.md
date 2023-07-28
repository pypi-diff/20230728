# Comparing `tmp/timedctl-5.0.5.tar.gz` & `tmp/timedctl-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timedctl-5.0.5.tar", max compression
+gzip compressed data, was "timedctl-5.0.6.tar", max compression
```

## Comparing `timedctl-5.0.5.tar` & `timedctl-5.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34454 2023-07-27 17:46:25.159686 timedctl-5.0.5/LICENSE
--rw-r--r--   0        0        0      774 2023-07-27 17:46:25.159686 timedctl-5.0.5/README.md
--rw-r--r--   0        0        0      858 2023-07-27 17:46:59.416067 timedctl-5.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-27 17:46:25.159686 timedctl-5.0.5/timedctl/__init__.py
--rw-r--r--   0        0        0     1831 2023-07-27 17:46:25.159686 timedctl-5.0.5/timedctl/helpers.py
--rwxr-xr-x   0        0        0    17124 2023-07-27 17:46:25.159686 timedctl-5.0.5/timedctl/timedctl.py
--rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 timedctl-5.0.5/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-28 14:19:52.199210 timedctl-5.0.6/LICENSE
+-rw-r--r--   0        0        0      774 2023-07-28 14:19:52.199210 timedctl-5.0.6/README.md
+-rw-r--r--   0        0        0      858 2023-07-28 14:20:17.111347 timedctl-5.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-28 14:19:52.199210 timedctl-5.0.6/timedctl/__init__.py
+-rw-r--r--   0        0        0     1831 2023-07-28 14:19:52.199210 timedctl-5.0.6/timedctl/helpers.py
+-rwxr-xr-x   0        0        0    19859 2023-07-28 14:19:52.199210 timedctl-5.0.6/timedctl/timedctl.py
+-rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 timedctl-5.0.6/PKG-INFO
```

### Comparing `timedctl-5.0.5/LICENSE` & `timedctl-5.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `timedctl-5.0.5/README.md` & `timedctl-5.0.6/README.md`

 * *Files identical despite different names*

### Comparing `timedctl-5.0.5/pyproject.toml` & `timedctl-5.0.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timedctl"
-version = "5.0.5"
+version = "5.0.6"
 description = "CLI for timed"
 authors = ["Arthur Deierlein <arthur.deierlein@adfinis.com>", "Gian Klug <gian.klug@adfinis.com>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `timedctl-5.0.5/timedctl/helpers.py` & `timedctl-5.0.6/timedctl/helpers.py`

 * *Files identical despite different names*

### Comparing `timedctl-5.0.5/timedctl/timedctl.py` & `timedctl-5.0.6/timedctl/timedctl.py`

 * *Files 14% similar despite different names*

```diff
@@ -105,14 +105,58 @@
             [" | ".join([row[0], row[1], row[2]]), row[1], row[2], row[3], row[4]]
         )
 
     report = fzf_wrapper(fzf_obj, [0], "Select a report: ")
     return report
 
 
+def select_activity(date):
+    """FZF prompt to select an activity."""
+    activities = timed.activities.get(filters={"date": date})
+    activity_view = []
+    # loop through all activities
+    for activity in activities:
+        # check if there is an actual task, else use an unknown task
+        task_data = activity["relationships"]["task"]["data"]
+        if task_data:
+            task = timed.tasks.get(id=task_data["id"], cached=True)
+        else:
+            task = {"attributes": {"name": "Unknown task"}, "id": None}
+        activity_view.append(
+            [
+                task["attributes"]["name"],
+                activity["attributes"]["comment"],
+                activity["attributes"]["from-time"].strftime("%H:%M:%S")
+                + " - "
+                + activity["attributes"]["to-time"].strftime("%H:%M:%S"),
+                task["id"],
+                activity["id"],
+            ]
+        )
+    # get longest key per value
+    max_key_lengths = [max(map(len, col)) for col in zip(*activity_view)]
+    # pad all the values
+    activity_view = [
+        [
+            activity_view[i][j].ljust(max_key_lengths[j])
+            for j in range(len(activity_view[i]))
+        ]
+        for i in range(len(activity_view))
+    ]
+    # create a list for fzf
+    fzf_obj = []
+    for row in activity_view:
+        fzf_obj.append(
+            [" | ".join([row[0], row[1], row[2]]), row[1], row[2], row[3], row[4]]
+        )
+
+    activity = fzf_wrapper(fzf_obj, [0], "Select an activity: ")
+    return activity
+
+
 timed = client_setup()
 
 
 @click.group(cls=ClickAliasedGroup)
 def timedctl():
     """Use timedctl."""
     pass  # pylint: disable=W0107
@@ -381,21 +425,21 @@
 
 @timedctl.group(cls=ClickAliasedGroup, aliases=["ac"])
 def activity():
     """Do stuff with activities."""
     pass  # pylint: disable=W0107
 
 
-@activity.command(aliases=["add", "a"])
+@activity.command("start", aliases=["add", "a"])
 @click.argument("comment")
 @click.option("--customer", default=None)
 @click.option("--project", default=None)
 @click.option("--task", default=None)
 @click.option("--show-archived", default=False, is_flag=True)
-def start(comment, customer, project, task, show_archived):
+def start_activity(comment, customer, project, task, show_archived):
     """Start recording activity."""
     customers = timed.customers.get(filters={"archived": show_archived}, cached=True)
     # ask the user to select a customer
     msg("Select a customer")
     # select a customer
     if customer:
         customer = [c for c in customers if c["attributes"]["name"] == customer]
@@ -436,39 +480,74 @@
     if res.status_code == 201:
         msg(f"Activity {comment} started successfully.")
         return
     # handle exception
     error_handler("ERR_ACTIVITY_START_FAILED")
 
 
-@activity.command(aliases=["end", "finish"])
-def stop():
+@activity.command("stop", aliases=["end", "finish"])
+def stop_activity():
     """Stop current activity."""
     if not timed.activities.current:
         error_handler("ERR_NO_CURRENT_ACTIVITY")
     else:
         timed.activities.stop()
     msg("Activity stopped successfully.")
 
 
-@activity.command(aliases=["s", "get", "info"])
-def show():
+@activity.command("show", aliases=["s", "get", "info"])
+def show_activity():
     """Show current activity."""
     current_activity = timed.activities.current
     if current_activity:
         msg(
             f"Current activity: {current_activity['attributes']['comment']} (Since "
             + f"{current_activity['attributes']['from-time'].strftime('%H:%M:%S')})"
         )
     else:
         error_handler("ERR_NO_CURRENT_ACTIVITY")
 
 
-@activity.command(aliases=["gts", "ts"])
-def generate_timesheet():
+@activity.command("restart", aliases=["r", "continue", "resume"])
+@click.option("--date", default=None)
+def restart_activity(date):
+    """Restart an activity."""
+    # stop current activity first
+    if timed.activities.current:
+        timed.activities.stop()
+        msg("Stopped current activity.")
+    # select an activity
+    activity = select_activity(date)
+    # grab attributes
+    comment = activity[1]
+    task_id = activity[3]
+    res = timed.activities.start(
+        attributes={"comment": comment}, relationships={"task": task_id}
+    )
+    if res.status_code == 201:
+        msg(f'Activity "{comment}" restarted successfully.')
+        return
+    # handle exception
+    error_handler("ERR_ACTIVITY_START_FAILED")
+
+
+@activity.command("delete", aliases=["d", "rm", "remove"])
+@click.option("--date", default=None)
+def delete_activity(date):
+    """Delete an activity."""
+    # select an activity
+    activity = select_activity(date)
+    if timed.activities.delete(activity[-1]):
+        msg(f"Activity {activity[1]} deleted successfully.")
+        return
+    error_handler("ERR_ACTIVITY_DELETE_FAILED")
+
+
+@activity.command("generate-timesheet", aliases=["gts", "ts"])
+def activity_generate_timesheet():
     """Generate the timesheet of the current activities."""
     activities = timed.activities.get()
     reports = timed.reports.get()
     if activities:
         for activity_obj in activities:
             attr = activity_obj["attributes"]
             if not attr["transferred"]:
```

### Comparing `timedctl-5.0.5/PKG-INFO` & `timedctl-5.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timedctl
-Version: 5.0.5
+Version: 5.0.6
 Summary: CLI for timed
 License: AGPL-3.0-only
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```


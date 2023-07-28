# Comparing `tmp/garth-0.3.0.tar.gz` & `tmp/garth-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.3.0.tar", last modified: Fri Jul 28 15:00:28 2023, max compression
+gzip compressed data, was "garth-0.3.1.tar", last modified: Fri Jul 28 15:03:11 2023, max compression
```

## Comparing `garth-0.3.0.tar` & `garth-0.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.3.0/LICENSE
--rw-r--r--   0        0        0     9447 2023-07-28 14:59:28.391093 garth-0.3.0/README.md
--rw-r--r--   0        0        0      448 2023-07-28 02:46:53.365386 garth-0.3.0/garth/__init__.py
--rw-r--r--   0        0        0      931 2023-07-28 12:08:41.094670 garth-0.3.0/garth/auth_token.py
--rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.3.0/garth/exc.py
--rw-r--r--   0        0        0     4673 2023-07-28 12:13:51.131928 garth-0.3.0/garth/http.py
--rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.3.0/garth/py.typed
--rw-r--r--   0        0        0      157 2023-07-28 02:46:53.365687 garth-0.3.0/garth/resources/__init__.py
--rw-r--r--   0        0        0     3508 2023-07-28 12:23:42.498445 garth-0.3.0/garth/resources/sleep.py
--rw-r--r--   0        0        0      616 2023-07-27 13:31:20.421792 garth-0.3.0/garth/resources/stress.py
--rw-r--r--   0        0        0     3767 2023-07-28 12:13:50.747670 garth-0.3.0/garth/sso.py
--rw-r--r--   0        0        0     1610 2023-07-27 13:31:20.421985 garth-0.3.0/garth/stats.py
--rw-r--r--   0        0        0     1294 2023-07-28 02:46:53.372554 garth-0.3.0/garth/utils.py
--rw-r--r--   0        0        0       22 2023-07-28 15:00:07.780635 garth-0.3.0/garth/version.py
--rw-r--r--   0        0        0     1069 2023-07-28 15:00:28.312703 garth-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.3.0/tests/cassettes/test_client_get.yaml
--rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.3.0/tests/cassettes/test_client_post.yaml
--rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.3.0/tests/cassettes/test_client_request.yaml
--rw-r--r--   0        0        0     2331 2023-07-28 03:35:21.644342 garth-0.3.0/tests/cassettes/test_connectapi.yaml
--rw-r--r--   0        0        0     4564 2023-07-28 03:35:21.644997 garth-0.3.0/tests/cassettes/test_connectapi_refresh.yaml
--rw-r--r--   0        0        0     3231 2023-07-28 03:35:21.645581 garth-0.3.0/tests/cassettes/test_exchange.yaml
--rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.3.0/tests/cassettes/test_get_username.yaml
--rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.3.0/tests/cassettes/test_login_email_password_fail.yaml
--rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.3.0/tests/cassettes/test_login_success.yaml
--rw-r--r--   0        0        0     2270 2023-07-28 03:35:21.646057 garth-0.3.0/tests/cassettes/test_refresh.yaml
--rw-r--r--   0        0        0     2963 2023-07-28 03:35:21.646600 garth-0.3.0/tests/cassettes/test_refresh_expired.yaml
--rw-r--r--   0        0        0     3080 2023-07-28 12:57:32.501754 garth-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     3098 2023-07-28 03:35:40.317256 garth-0.3.0/tests/resources/cassettes/test_daily_sleep.yaml
--rw-r--r--   0        0        0     6252 2023-07-28 03:35:40.317752 garth-0.3.0/tests/resources/cassettes/test_daily_stress.yaml
--rw-r--r--   0        0        0    44427 2023-07-28 03:35:40.318411 garth-0.3.0/tests/resources/cassettes/test_daily_stress_pagination.yaml
--rw-r--r--   0        0        0     3652 2023-07-28 12:21:13.363000 garth-0.3.0/tests/resources/cassettes/test_sleep_data_get.yaml
--rw-r--r--   0        0        0    77468 2023-07-28 12:22:31.103002 garth-0.3.0/tests/resources/cassettes/test_sleep_data_list.yaml
--rw-r--r--   0        0        0     4717 2023-07-28 03:35:40.318832 garth-0.3.0/tests/resources/cassettes/test_weekly_stress.yaml
--rw-r--r--   0        0        0    16221 2023-07-28 03:35:40.319518 garth-0.3.0/tests/resources/cassettes/test_weekly_stress_beyond_data.yaml
--rw-r--r--   0        0        0     7522 2023-07-28 03:35:40.320026 garth-0.3.0/tests/resources/cassettes/test_weekly_stress_pagination.yaml
--rw-r--r--   0        0        0      849 2023-07-28 12:22:22.098284 garth-0.3.0/tests/resources/test_sleep.py
--rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.3.0/tests/resources/test_stress.py
--rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.3.0/tests/test_auth_token.py
--rw-r--r--   0        0        0     4097 2023-07-28 12:02:46.585315 garth-0.3.0/tests/test_http.py
--rw-r--r--   0        0        0     2570 2023-07-28 12:10:36.895963 garth-0.3.0/tests/test_sso.py
--rw-r--r--   0        0        0      531 2023-07-27 13:16:10.645234 garth-0.3.0/tests/test_utils.py
--rw-r--r--   0        0        0     9859 1970-01-01 00:00:00.000000 garth-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.3.1/LICENSE
+-rw-r--r--   0        0        0     9446 2023-07-28 15:02:39.347778 garth-0.3.1/README.md
+-rw-r--r--   0        0        0      448 2023-07-28 02:46:53.365386 garth-0.3.1/garth/__init__.py
+-rw-r--r--   0        0        0      931 2023-07-28 12:08:41.094670 garth-0.3.1/garth/auth_token.py
+-rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.3.1/garth/exc.py
+-rw-r--r--   0        0        0     4673 2023-07-28 12:13:51.131928 garth-0.3.1/garth/http.py
+-rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.3.1/garth/py.typed
+-rw-r--r--   0        0        0      157 2023-07-28 02:46:53.365687 garth-0.3.1/garth/resources/__init__.py
+-rw-r--r--   0        0        0     3508 2023-07-28 12:23:42.498445 garth-0.3.1/garth/resources/sleep.py
+-rw-r--r--   0        0        0      616 2023-07-27 13:31:20.421792 garth-0.3.1/garth/resources/stress.py
+-rw-r--r--   0        0        0     3767 2023-07-28 12:13:50.747670 garth-0.3.1/garth/sso.py
+-rw-r--r--   0        0        0     1610 2023-07-27 13:31:20.421985 garth-0.3.1/garth/stats.py
+-rw-r--r--   0        0        0     1294 2023-07-28 02:46:53.372554 garth-0.3.1/garth/utils.py
+-rw-r--r--   0        0        0       22 2023-07-28 15:02:55.210356 garth-0.3.1/garth/version.py
+-rw-r--r--   0        0        0     1069 2023-07-28 15:03:11.356228 garth-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2386 2023-07-22 11:39:14.617674 garth-0.3.1/tests/cassettes/test_client_get.yaml
+-rw-r--r--   0        0        0     2425 2023-07-22 11:39:14.746057 garth-0.3.1/tests/cassettes/test_client_post.yaml
+-rw-r--r--   0        0        0   100962 2023-07-22 11:22:15.428262 garth-0.3.1/tests/cassettes/test_client_request.yaml
+-rw-r--r--   0        0        0     2331 2023-07-28 03:35:21.644342 garth-0.3.1/tests/cassettes/test_connectapi.yaml
+-rw-r--r--   0        0        0     4564 2023-07-28 03:35:21.644997 garth-0.3.1/tests/cassettes/test_connectapi_refresh.yaml
+-rw-r--r--   0        0        0     3231 2023-07-28 03:35:21.645581 garth-0.3.1/tests/cassettes/test_exchange.yaml
+-rw-r--r--   0        0        0    10962 2023-07-23 13:53:16.232082 garth-0.3.1/tests/cassettes/test_get_username.yaml
+-rw-r--r--   0        0        0    50551 2023-07-22 15:27:42.274531 garth-0.3.1/tests/cassettes/test_login_email_password_fail.yaml
+-rw-r--r--   0        0        0    91847 2023-07-23 13:50:32.012417 garth-0.3.1/tests/cassettes/test_login_success.yaml
+-rw-r--r--   0        0        0     2270 2023-07-28 03:35:21.646057 garth-0.3.1/tests/cassettes/test_refresh.yaml
+-rw-r--r--   0        0        0     2963 2023-07-28 03:35:21.646600 garth-0.3.1/tests/cassettes/test_refresh_expired.yaml
+-rw-r--r--   0        0        0     3080 2023-07-28 12:57:32.501754 garth-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     3098 2023-07-28 03:35:40.317256 garth-0.3.1/tests/resources/cassettes/test_daily_sleep.yaml
+-rw-r--r--   0        0        0     6252 2023-07-28 03:35:40.317752 garth-0.3.1/tests/resources/cassettes/test_daily_stress.yaml
+-rw-r--r--   0        0        0    44427 2023-07-28 03:35:40.318411 garth-0.3.1/tests/resources/cassettes/test_daily_stress_pagination.yaml
+-rw-r--r--   0        0        0     3652 2023-07-28 12:21:13.363000 garth-0.3.1/tests/resources/cassettes/test_sleep_data_get.yaml
+-rw-r--r--   0        0        0    77468 2023-07-28 12:22:31.103002 garth-0.3.1/tests/resources/cassettes/test_sleep_data_list.yaml
+-rw-r--r--   0        0        0     4717 2023-07-28 03:35:40.318832 garth-0.3.1/tests/resources/cassettes/test_weekly_stress.yaml
+-rw-r--r--   0        0        0    16221 2023-07-28 03:35:40.319518 garth-0.3.1/tests/resources/cassettes/test_weekly_stress_beyond_data.yaml
+-rw-r--r--   0        0        0     7522 2023-07-28 03:35:40.320026 garth-0.3.1/tests/resources/cassettes/test_weekly_stress_pagination.yaml
+-rw-r--r--   0        0        0      849 2023-07-28 12:22:22.098284 garth-0.3.1/tests/resources/test_sleep.py
+-rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.3.1/tests/resources/test_stress.py
+-rw-r--r--   0        0        0     1808 2023-07-23 13:40:52.098938 garth-0.3.1/tests/test_auth_token.py
+-rw-r--r--   0        0        0     4097 2023-07-28 12:02:46.585315 garth-0.3.1/tests/test_http.py
+-rw-r--r--   0        0        0     2570 2023-07-28 12:10:36.895963 garth-0.3.1/tests/test_sso.py
+-rw-r--r--   0        0        0      531 2023-07-27 13:16:10.645234 garth-0.3.1/tests/test_utils.py
+-rw-r--r--   0        0        0     9858 1970-01-01 00:00:00.000000 garth-0.3.1/PKG-INFO
```

### Comparing `garth-0.3.0/LICENSE` & `garth-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/README.md` & `garth-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 Garmin SSO auth + Connect client
 
 ## Google Colabs
 
 [Graph 28-day rolling average of daily stress](https://colab.research.google.com/github/matin/garth/blob/main/colabs/stress.ipynb)
 
-
 ## Background
 
 Garth is meant for personal use and follows the philosiphy that your data is
 your data. You should be able to download it and analyze it in the way that
 you'd like. In my case, that means processing with Google Colab, Pandas,
 Matplotlib, etc.
 
@@ -200,15 +199,14 @@
 ```python
 [
     DailySleep(calendar_date=datetime.date(2023, 7, 22), value=69),
     DailySleep(calendar_date=datetime.date(2023, 7, 23), value=73)
 ]
 ```
 
-
 Detailed sleep data
 
 ```python
 garth.SleepData.get("2023-07-20")
 ```
 
 ```python
@@ -334,12 +332,12 @@
             end_gmt=datetime.datetime(2023, 7, 20, 13, 11),
             activity_level=7.088729101943337
         )
     ]
 )
 ```
 
-leep data over several nights
+sleep data over several nights
 
 ```python
 garth.SleepData.get(end="2023-07-20", days=30)
 ```
```

### Comparing `garth-0.3.0/garth/auth_token.py` & `garth-0.3.1/garth/auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/garth/http.py` & `garth-0.3.1/garth/http.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/garth/resources/sleep.py` & `garth-0.3.1/garth/resources/sleep.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/garth/resources/stress.py` & `garth-0.3.1/garth/resources/stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/garth/sso.py` & `garth-0.3.1/garth/sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/garth/stats.py` & `garth-0.3.1/garth/stats.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/garth/utils.py` & `garth-0.3.1/garth/utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/pyproject.toml` & `garth-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
 ]
-version = "0.3.0"
+version = "0.3.1"
 
 [project.license]
 text = "MIT"
 
 [project.packages]
 include = [
     { from = ".", include = "garth" },
```

### Comparing `garth-0.3.0/tests/cassettes/test_client_get.yaml` & `garth-0.3.1/tests/cassettes/test_client_get.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/cassettes/test_client_post.yaml` & `garth-0.3.1/tests/cassettes/test_client_post.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/cassettes/test_client_request.yaml` & `garth-0.3.1/tests/cassettes/test_client_request.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/cassettes/test_connectapi.yaml` & `garth-0.3.1/tests/cassettes/test_connectapi.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/cassettes/test_connectapi_refresh.yaml` & `garth-0.3.1/tests/cassettes/test_connectapi_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/cassettes/test_exchange.yaml` & `garth-0.3.1/tests/cassettes/test_exchange.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/cassettes/test_get_username.yaml` & `garth-0.3.1/tests/cassettes/test_get_username.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/cassettes/test_login_email_password_fail.yaml` & `garth-0.3.1/tests/cassettes/test_login_email_password_fail.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/cassettes/test_login_success.yaml` & `garth-0.3.1/tests/cassettes/test_login_success.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/cassettes/test_refresh.yaml` & `garth-0.3.1/tests/cassettes/test_refresh.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/cassettes/test_refresh_expired.yaml` & `garth-0.3.1/tests/cassettes/test_refresh_expired.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/conftest.py` & `garth-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/resources/cassettes/test_daily_sleep.yaml` & `garth-0.3.1/tests/resources/cassettes/test_daily_sleep.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/resources/cassettes/test_daily_stress.yaml` & `garth-0.3.1/tests/resources/cassettes/test_daily_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/resources/cassettes/test_daily_stress_pagination.yaml` & `garth-0.3.1/tests/resources/cassettes/test_daily_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/resources/cassettes/test_sleep_data_get.yaml` & `garth-0.3.1/tests/resources/cassettes/test_sleep_data_get.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/resources/cassettes/test_sleep_data_list.yaml` & `garth-0.3.1/tests/resources/cassettes/test_sleep_data_list.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/resources/cassettes/test_weekly_stress.yaml` & `garth-0.3.1/tests/resources/cassettes/test_weekly_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/resources/cassettes/test_weekly_stress_beyond_data.yaml` & `garth-0.3.1/tests/resources/cassettes/test_weekly_stress_beyond_data.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/resources/cassettes/test_weekly_stress_pagination.yaml` & `garth-0.3.1/tests/resources/cassettes/test_weekly_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/resources/test_sleep.py` & `garth-0.3.1/tests/resources/test_sleep.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/resources/test_stress.py` & `garth-0.3.1/tests/resources/test_stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/test_auth_token.py` & `garth-0.3.1/tests/test_auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/test_http.py` & `garth-0.3.1/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/test_sso.py` & `garth-0.3.1/tests/test_sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/tests/test_utils.py` & `garth-0.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.3.0/PKG-INFO` & `garth-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garth
-Version: 0.3.0
+Version: 0.3.1
 Summary: Garmin SSO auth + Connect client
 Author-Email: Matin Tamizi <mtamizi@duck.com>
 License: MIT
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
@@ -19,15 +19,14 @@
 
 Garmin SSO auth + Connect client
 
 ## Google Colabs
 
 [Graph 28-day rolling average of daily stress](https://colab.research.google.com/github/matin/garth/blob/main/colabs/stress.ipynb)
 
-
 ## Background
 
 Garth is meant for personal use and follows the philosiphy that your data is
 your data. You should be able to download it and analyze it in the way that
 you'd like. In my case, that means processing with Google Colab, Pandas,
 Matplotlib, etc.
 
@@ -214,15 +213,14 @@
 ```python
 [
     DailySleep(calendar_date=datetime.date(2023, 7, 22), value=69),
     DailySleep(calendar_date=datetime.date(2023, 7, 23), value=73)
 ]
 ```
 
-
 Detailed sleep data
 
 ```python
 garth.SleepData.get("2023-07-20")
 ```
 
 ```python
@@ -348,12 +346,12 @@
             end_gmt=datetime.datetime(2023, 7, 20, 13, 11),
             activity_level=7.088729101943337
         )
     ]
 )
 ```
 
-leep data over several nights
+sleep data over several nights
 
 ```python
 garth.SleepData.get(end="2023-07-20", days=30)
 ```
```


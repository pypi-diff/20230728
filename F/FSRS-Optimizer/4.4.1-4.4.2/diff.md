# Comparing `tmp/FSRS-Optimizer-4.4.1.tar.gz` & `tmp/FSRS-Optimizer-4.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FSRS-Optimizer-4.4.1.tar", last modified: Fri Jul 28 08:41:26 2023, max compression
+gzip compressed data, was "FSRS-Optimizer-4.4.2.tar", last modified: Fri Jul 28 18:00:40 2023, max compression
```

## Comparing `FSRS-Optimizer-4.4.1.tar` & `FSRS-Optimizer-4.4.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:41:26.233910 FSRS-Optimizer-4.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-28 08:41:26.233910 FSRS-Optimizer-4.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-28 08:41:15.000000 FSRS-Optimizer-4.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 08:41:26.233910 FSRS-Optimizer-4.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 08:41:15.000000 FSRS-Optimizer-4.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:41:26.229910 FSRS-Optimizer-4.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:41:26.229910 FSRS-Optimizer-4.4.1/src/FSRS_Optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-28 08:41:26.000000 FSRS-Optimizer-4.4.1/src/FSRS_Optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-28 08:41:26.000000 FSRS-Optimizer-4.4.1/src/FSRS_Optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:41:26.000000 FSRS-Optimizer-4.4.1/src/FSRS_Optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-28 08:41:26.000000 FSRS-Optimizer-4.4.1/src/FSRS_Optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 08:41:26.000000 FSRS-Optimizer-4.4.1/src/FSRS_Optimizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:41:26.229910 FSRS-Optimizer-4.4.1/src/fsrs_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 08:41:15.000000 FSRS-Optimizer-4.4.1/src/fsrs_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-28 08:41:15.000000 FSRS-Optimizer-4.4.1/src/fsrs_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51382 2023-07-28 08:41:15.000000 FSRS-Optimizer-4.4.1/src/fsrs_optimizer/fsrs_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:00:40.152486 FSRS-Optimizer-4.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-28 18:00:40.152486 FSRS-Optimizer-4.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-28 18:00:29.000000 FSRS-Optimizer-4.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-28 18:00:29.000000 FSRS-Optimizer-4.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:00:40.152486 FSRS-Optimizer-4.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 18:00:29.000000 FSRS-Optimizer-4.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:00:40.148486 FSRS-Optimizer-4.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:00:40.152486 FSRS-Optimizer-4.4.2/src/FSRS_Optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-28 18:00:40.000000 FSRS-Optimizer-4.4.2/src/FSRS_Optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-28 18:00:40.000000 FSRS-Optimizer-4.4.2/src/FSRS_Optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:00:40.000000 FSRS-Optimizer-4.4.2/src/FSRS_Optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-28 18:00:40.000000 FSRS-Optimizer-4.4.2/src/FSRS_Optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 18:00:40.000000 FSRS-Optimizer-4.4.2/src/FSRS_Optimizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:00:40.152486 FSRS-Optimizer-4.4.2/src/fsrs_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 18:00:29.000000 FSRS-Optimizer-4.4.2/src/fsrs_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-28 18:00:29.000000 FSRS-Optimizer-4.4.2/src/fsrs_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51419 2023-07-28 18:00:29.000000 FSRS-Optimizer-4.4.2/src/fsrs_optimizer/fsrs_optimizer.py
```

### Comparing `FSRS-Optimizer-4.4.1/src/fsrs_optimizer/__main__.py` & `FSRS-Optimizer-4.4.2/src/fsrs_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `FSRS-Optimizer-4.4.1/src/fsrs_optimizer/fsrs_optimizer.py` & `FSRS-Optimizer-4.4.2/src/fsrs_optimizer/fsrs_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,14 +394,15 @@
             return list(accumulate(x))
 
         t_history = df.groupby('cid', group_keys=False)['delta_t'].apply(lambda x: cum_concat([[int(i)] for i in x]))
         df['t_history']=[','.join(map(str, item[:-1])) for sublist in t_history for item in sublist]
         r_history = df.groupby('cid', group_keys=False)['r'].apply(lambda x: cum_concat([[i] for i in x]))
         df['r_history']=[','.join(map(str, item[:-1])) for sublist in r_history for item in sublist]
         df = df.groupby('cid').filter(lambda group: group['id'].min() > time.mktime(datetime.strptime(revlog_start_date, "%Y-%m-%d").timetuple()) * 1000)
+        df = df[df['r'] != 0].copy()
         df['y'] = df['r'].map(lambda x: {1: 0, 2: 1, 3: 1, 4: 1}[x])
 
         def remove_outliers(group: pd.DataFrame) -> pd.DataFrame:
             # threshold = np.mean(group['delta_t']) * 1.5
             # threshold = group['delta_t'].quantile(0.95)
             Q1 = group['delta_t'].quantile(0.25)
             Q3 = group['delta_t'].quantile(0.75)
```


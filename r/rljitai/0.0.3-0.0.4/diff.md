# Comparing `tmp/rljitai-0.0.3.tar.gz` & `tmp/rljitai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rljitai-0.0.3.tar", last modified: Wed Jul 26 00:01:49 2023, max compression
+gzip compressed data, was "rljitai-0.0.4.tar", last modified: Fri Jul 28 17:58:52 2023, max compression
```

## Comparing `rljitai-0.0.3.tar` & `rljitai-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 00:01:49.807497 rljitai-0.0.3/
--rw-rw-rw-   0        0        0     1134 2023-07-25 23:40:45.000000 rljitai-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      831 2023-07-26 00:01:49.807497 rljitai-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1699 2023-07-25 23:40:45.000000 rljitai-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 00:01:49.807497 rljitai-0.0.3/rljitai.egg-info/
--rw-rw-rw-   0        0        0      831 2023-07-26 00:01:49.000000 rljitai-0.0.3/rljitai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-07-26 00:01:49.000000 rljitai-0.0.3/rljitai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 00:01:49.000000 rljitai-0.0.3/rljitai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-26 00:01:49.000000 rljitai-0.0.3/rljitai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2023-07-26 00:01:49.000000 rljitai-0.0.3/rljitai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 00:01:49.000000 rljitai-0.0.3/rljitai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 00:01:49.807497 rljitai-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1895 2023-07-26 00:01:30.000000 rljitai-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:58:52.186053 rljitai-0.0.4/
+-rw-rw-rw-   0        0        0     1134 2023-07-28 17:41:50.000000 rljitai-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      831 2023-07-28 17:58:52.182877 rljitai-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1808 2023-07-28 17:52:24.000000 rljitai-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 17:58:52.106601 rljitai-0.0.4/rl_jitai_simulation/
+-rw-rw-rw-   0        0        0        0 2023-07-28 17:42:34.000000 rljitai-0.0.4/rl_jitai_simulation/__init__.py
+-rw-rw-rw-   0        0        0     8051 2023-07-28 17:41:50.000000 rljitai-0.0.4/rl_jitai_simulation/agents.py
+-rw-rw-rw-   0        0        0    11529 2023-07-28 17:41:50.000000 rljitai-0.0.4/rl_jitai_simulation/envs.py
+-rw-rw-rw-   0        0        0     2631 2023-07-28 17:48:05.000000 rljitai-0.0.4/rl_jitai_simulation/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 17:58:52.180837 rljitai-0.0.4/rljitai.egg-info/
+-rw-rw-rw-   0        0        0      831 2023-07-28 17:58:51.000000 rljitai-0.0.4/rljitai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-07-28 17:58:51.000000 rljitai-0.0.4/rljitai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 17:58:51.000000 rljitai-0.0.4/rljitai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-28 17:58:51.000000 rljitai-0.0.4/rljitai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2023-07-28 17:58:51.000000 rljitai-0.0.4/rljitai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-28 17:58:51.000000 rljitai-0.0.4/rljitai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 17:58:52.187105 rljitai-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1895 2023-07-28 17:57:29.000000 rljitai-0.0.4/setup.py
```

### Comparing `rljitai-0.0.3/LICENSE` & `rljitai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rljitai-0.0.3/PKG-INFO` & `rljitai-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rljitai
-Version: 0.0.3
+Version: 0.0.4
 Summary: rljitai
 Home-page: https://github.com/reml-lab/rl_jitai_simulation/
 Author: REML Lab developer
 Author-email: remllabdeveloper@gmail.com
 License: MIT
 Keywords: mHealth machine-learning reinforcement-learning jitai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rljitai-0.0.3/README.md` & `rljitai-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 This paper was accepted at the Conference on Uncertainty in Artificial Intelligence, UAI 2023.
 
 + arXiv link: https://arxiv.org/abs/2305.09913
 
 + UAI 2023 link: https://proceedings.mlr.press/v216/karine23a.html
 
++ UAI 2023 poster: https://github.com/reml-lab/rl_jitai_simulation/tree/main/rl_jitai_simulation_poster.pdf
 
 ## Examples
 
 See the [Examples](https://github.com/reml-lab/rl_jitai_simulation/tree/main/examples) directory for a list of examples that can be run locally or launched in Google Colab.
 
 For example:
```

### Comparing `rljitai-0.0.3/rljitai.egg-info/PKG-INFO` & `rljitai-0.0.4/rljitai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rljitai
-Version: 0.0.3
+Version: 0.0.4
 Summary: rljitai
 Home-page: https://github.com/reml-lab/rl_jitai_simulation/
 Author: REML Lab developer
 Author-email: remllabdeveloper@gmail.com
 License: MIT
 Keywords: mHealth machine-learning reinforcement-learning jitai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rljitai-0.0.3/setup.py` & `rljitai-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 long_description = "RL for JITAI optimization using simulated environments"
 
 if __name__ == '__main__':
     setup(
         name="rljitai",
 
-        version='0.0.3',
+        version='0.0.4',
 
         package_data={'': ['default.yml']},
 
         description="rljitai",
         long_description_content_type='text/markdown',
         long_description=long_description,
```


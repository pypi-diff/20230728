# Comparing `tmp/fsrs-0.2.2.tar.gz` & `tmp/fsrs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs-0.2.2.tar", last modified: Tue Jun 20 08:33:55 2023, max compression
+gzip compressed data, was "fsrs-1.0.0.tar", last modified: Fri Jul 28 05:49:26 2023, max compression
```

## Comparing `fsrs-0.2.2.tar` & `fsrs-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:33:55.552683 fsrs-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-20 08:33:38.000000 fsrs-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-20 08:33:55.552683 fsrs-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-20 08:33:38.000000 fsrs-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-20 08:33:38.000000 fsrs-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 08:33:55.552683 fsrs-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 08:33:38.000000 fsrs-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:33:55.548683 fsrs-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:33:55.552683 fsrs-0.2.2/src/fsrs/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 08:33:38.000000 fsrs-0.2.2/src/fsrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-06-20 08:33:38.000000 fsrs-0.2.2/src/fsrs/fsrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-06-20 08:33:38.000000 fsrs-0.2.2/src/fsrs/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:33:55.552683 fsrs-0.2.2/src/fsrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-20 08:33:55.000000 fsrs-0.2.2/src/fsrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-20 08:33:55.000000 fsrs-0.2.2/src/fsrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:33:55.000000 fsrs-0.2.2/src/fsrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 08:33:55.000000 fsrs-0.2.2/src/fsrs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:33:55.552683 fsrs-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-20 08:33:38.000000 fsrs-0.2.2/tests/test_fsrs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:49:26.831310 fsrs-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-28 05:49:15.000000 fsrs-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-28 05:49:26.827310 fsrs-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-28 05:49:15.000000 fsrs-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-28 05:49:15.000000 fsrs-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 05:49:26.831310 fsrs-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 05:49:15.000000 fsrs-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:49:26.827310 fsrs-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:49:26.827310 fsrs-1.0.0/src/fsrs/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-28 05:49:15.000000 fsrs-1.0.0/src/fsrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-28 05:49:15.000000 fsrs-1.0.0/src/fsrs/fsrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-28 05:49:15.000000 fsrs-1.0.0/src/fsrs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:49:26.827310 fsrs-1.0.0/src/fsrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-28 05:49:26.000000 fsrs-1.0.0/src/fsrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-28 05:49:26.000000 fsrs-1.0.0/src/fsrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 05:49:26.000000 fsrs-1.0.0/src/fsrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 05:49:26.000000 fsrs-1.0.0/src/fsrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:49:26.827310 fsrs-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-28 05:49:15.000000 fsrs-1.0.0/tests/test_fsrs.py
```

### Comparing `fsrs-0.2.2/LICENSE` & `fsrs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fsrs-0.2.2/PKG-INFO` & `fsrs-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsrs
-Version: 0.2.2
+Version: 1.0.0
 Summary: Free Spaced Repetition Scheduler
 Author-email: Jarrett Ye <jarrett.ye@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Open Spaced Repetition
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fsrs-0.2.2/README.md` & `fsrs-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fsrs-0.2.2/pyproject.toml` & `fsrs-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fsrs"
-version = "0.2.2"
+version = "1.0.0"
 description = "Free Spaced Repetition Scheduler"
 readme = "README.md"
 authors = [{ name = "Jarrett Ye", email = "jarrett.ye@outlook.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `fsrs-0.2.2/src/fsrs/fsrs.py` & `fsrs-1.0.0/src/fsrs/fsrs.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,35 +21,35 @@
 
         if card.state == State.New:
             self.init_ds(s)
 
             s.again.due = now + timedelta(minutes=1)
             s.hard.due = now + timedelta(minutes=5)
             s.good.due = now + timedelta(minutes=10)
-            easy_interval = self.next_interval(s.easy.stability * self.p.easy_bonus)
+            easy_interval = self.next_interval(s.easy.stability)
             s.easy.scheduled_days = easy_interval
             s.easy.due = now + timedelta(days=easy_interval)
         elif card.state == State.Learning or card.state == State.Relearning:
             hard_interval = 0
             good_interval = self.next_interval(s.good.stability)
-            easy_interval = max(self.next_interval(s.easy.stability * self.p.easy_bonus), good_interval + 1)
+            easy_interval = max(self.next_interval(s.easy.stability), good_interval + 1)
 
             s.schedule(now, hard_interval, good_interval, easy_interval)
         elif card.state == State.Review:
             interval = card.elapsed_days
             last_d = card.difficulty
             last_s = card.stability
-            retrievability = math.exp(math.log(0.9) * interval / last_s)
+            retrievability = (1 + interval / (9 * last_s)) ** -1
             self.next_ds(s, last_d, last_s, retrievability)
 
-            hard_interval = self.next_interval(last_s * self.p.hard_factor)
+            hard_interval = self.next_interval(s.hard.stability)
             good_interval = self.next_interval(s.good.stability)
             hard_interval = min(hard_interval, good_interval)
             good_interval = max(good_interval, hard_interval + 1)
-            easy_interval = max(self.next_interval(s.easy.stability * self.p.easy_bonus), good_interval + 1)
+            easy_interval = max(self.next_interval(s.easy.stability), good_interval + 1)
             s.schedule(now, hard_interval, good_interval, easy_interval)
         return s.record_log(card, now)
 
     def init_ds(self, s: SchedulingCards) -> None:
         s.again.difficulty = self.init_difficulty(Rating.Again)
         s.again.stability = self.init_stability(Rating.Again)
         s.hard.difficulty = self.init_difficulty(Rating.Hard)
@@ -59,38 +59,45 @@
         s.easy.difficulty = self.init_difficulty(Rating.Easy)
         s.easy.stability = self.init_stability(Rating.Easy)
 
     def next_ds(self, s: SchedulingCards, last_d: float, last_s: float, retrievability: float):
         s.again.difficulty = self.next_difficulty(last_d, Rating.Again)
         s.again.stability = self.next_forget_stability(s.again.difficulty, last_s, retrievability)
         s.hard.difficulty = self.next_difficulty(last_d, Rating.Hard)
-        s.hard.stability = self.next_recall_stability(s.hard.difficulty, last_s, retrievability)
+        s.hard.stability = self.next_recall_stability(s.hard.difficulty, last_s, retrievability, Rating.Hard)
         s.good.difficulty = self.next_difficulty(last_d, Rating.Good)
-        s.good.stability = self.next_recall_stability(s.good.difficulty, last_s, retrievability)
+        s.good.stability = self.next_recall_stability(s.good.difficulty, last_s, retrievability, Rating.Good)
         s.easy.difficulty = self.next_difficulty(last_d, Rating.Easy)
-        s.easy.stability = self.next_recall_stability(s.easy.difficulty, last_s, retrievability)
+        s.easy.stability = self.next_recall_stability(s.easy.difficulty, last_s, retrievability, Rating.Easy)
 
     def init_stability(self, r: int) -> float:
-        return max(self.p.w[0] + self.p.w[1] * r, 0.1)
+        return max(self.p.w[r-1], 0.1)
 
     def init_difficulty(self, r: int) -> float:
-        return min(max(self.p.w[2] + self.p.w[3] * (r - 2), 1), 10)
+        return min(max(self.p.w[4] - self.p.w[5] * (r - 3), 1), 10)
 
     def next_interval(self, s: float) -> int:
-        new_interval = s * math.log(self.p.request_retention) / math.log(0.9)
+        new_interval = s * 9 * (1 / self.p.request_retention - 1)
         return min(max(round(new_interval), 1), self.p.maximum_interval)
 
     def next_difficulty(self, d: float, r: int) -> float:
-        next_d = d + self.p.w[4] * (r - 2)
-        return min(max(self.mean_reversion(self.p.w[2], next_d), 1), 10)
+        next_d = d - self.p.w[6] * (r - 3)
+        return min(max(self.mean_reversion(self.p.w[4], next_d), 1), 10)
 
     def mean_reversion(self, init: float, current: float) -> float:
-        return self.p.w[5] * init + (1 - self.p.w[5]) * current
+        return self.p.w[7] * init + (1 - self.p.w[7]) * current
 
-    def next_recall_stability(self, d: float, s: float, r: float) -> float:
-        return s * (1 + math.exp(self.p.w[6]) *
+    def next_recall_stability(self, d: float, s: float, r: float, rating: int) -> float:
+        hard_penalty = self.p.w[15] if rating == Rating.Hard else 1
+        easy_bonus = self.p.w[16] if rating == Rating.Easy else 1
+        return s * (1 + math.exp(self.p.w[8]) *
                     (11 - d) *
-                    math.pow(s, self.p.w[7]) *
-                    (math.exp((1 - r) * self.p.w[8]) - 1))
+                    math.pow(s, -self.p.w[9]) *
+                    (math.exp((1 - r) * self.p.w[10]) - 1) *
+                    hard_penalty *
+                    easy_bonus)
 
     def next_forget_stability(self, d: float, s: float, r: float) -> float:
-        return self.p.w[9] * math.pow(d, self.p.w[10]) * math.pow(s, self.p.w[11]) * math.exp((1 - r) * self.p.w[12])
+        return self.p.w[11] * \
+            math.pow(d, -self.p.w[12]) * \
+            (math.pow(s + 1, self.p.w[13]) - 1) * \
+            math.exp((1 - r) * self.p.w[14])
```

### Comparing `fsrs-0.2.2/src/fsrs/models.py` & `fsrs-1.0.0/src/fsrs/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from datetime import datetime, timedelta
 import copy
-import math
 from typing import Tuple, Optional
 from enum import IntEnum
 
 
 class State(IntEnum):
     New = 0
     Learning = 1
     Review = 2
     Relearning = 3
 
 
 class Rating(IntEnum):
-    Again = 0
-    Hard = 1
-    Good = 2
-    Easy = 3
+    Again = 1
+    Hard = 2
+    Good = 3
+    Easy = 4
 
 
 class ReviewLog:
     rating: int
     elapsed_days: int
     scheduled_days: int
     Review: datetime
@@ -55,15 +54,15 @@
         self.lapses = 0
         self.state = State.New
 
     
     def get_retrievability(self, now: datetime) -> Optional[float]:
         if self.state == State.Review:
             elapsed_days = max(0, (now - self.last_review).days)
-            return math.exp(math.log(0.9) * elapsed_days / self.stability)
+            return (1 + elapsed_days / (9 * self.stability)) ** -1
         else:
             return None
 
 
 class SchedulingInfo:
     card: Card
     Review_log: ReviewLog
@@ -133,17 +132,13 @@
                                                   card.state)),
         }
 
 
 class Parameters:
     request_retention: float
     maximum_interval: int
-    easy_bonus: float
-    hard_factor: float
     w: Tuple[float, ...]
 
     def __init__(self) -> None:
         self.request_retention = 0.9
         self.maximum_interval = 36500
-        self.easy_bonus = 1.3
-        self.hard_factor = 1.2
-        self.w = (1., 1., 5., -0.5, -0.5, 0.2, 1.4, -0.12, 0.8, 2., -0.2, 0.2, 1.)
+        self.w = (0.4, 0.6, 2.4, 5.8, 4.93, 0.94, 0.86, 0.01, 1.49, 0.14, 0.94, 2.18, 0.05, 0.34, 1.26, 0.29, 2.61)
```

### Comparing `fsrs-0.2.2/src/fsrs.egg-info/PKG-INFO` & `fsrs-1.0.0/src/fsrs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsrs
-Version: 0.2.2
+Version: 1.0.0
 Summary: Free Spaced Repetition Scheduler
 Author-email: Jarrett Ye <jarrett.ye@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Open Spaced Repetition
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```


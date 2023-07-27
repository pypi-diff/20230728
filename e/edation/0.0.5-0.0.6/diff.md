# Comparing `tmp/edation-0.0.5.tar.gz` & `tmp/edation-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edation-0.0.5.tar", max compression
+gzip compressed data, was "edation-0.0.6.tar", max compression
```

## Comparing `edation-0.0.5.tar` & `edation-0.0.6.tar`

### file list

```diff
@@ -1,52 +1,44 @@
--rw-r--r--   0        0        0     2485 2023-07-27 12:57:53.566113 edation-0.0.5/README.md
--rw-r--r--   0        0        0     2275 2023-07-27 12:50:52.326113 edation-0.0.5/edation/__init__.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/adapter/__init__.py
--rw-r--r--   0        0        0     4929 2023-07-27 12:48:18.706113 edation-0.0.5/edation/adapter/identity.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/adapter/repo/__init__.py
--rw-r--r--   0        0        0     2480 2023-07-27 12:48:17.736113 edation-0.0.5/edation/adapter/repo/file_visual.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/adapter/repo/odb_dataset.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/adapter/repo/odb_tests.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/adapter/repo/odb_visual.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/adapter/stats/__init__.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/adapter/visual/__init__.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/application/__init__.py
--rw-r--r--   0        0        0     2004 2023-07-27 12:50:52.326113 edation-0.0.5/edation/application/ports/driven/identity.py
--rw-r--r--   0        0        0     2504 2023-07-27 12:50:52.326113 edation-0.0.5/edation/application/ports/driven/repo.py
--rw-r--r--   0        0        0     1707 2023-07-27 12:50:52.326113 edation-0.0.5/edation/application/ports/driven/stats.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/application/ports/driven/visual.py
--rw-r--r--   0        0        0     2897 2023-07-27 12:48:16.846113 edation-0.0.5/edation/application/ports/driver/base.py
--rw-r--r--   0        0        0     3572 2023-07-27 12:51:36.096113 edation-0.0.5/edation/application/ports/driver/data.py
--rw-r--r--   0        0        0     1835 2023-07-27 12:48:14.866114 edation-0.0.5/edation/application/visual/base.py
--rw-r--r--   0        0        0     3672 2023-07-27 12:51:36.096113 edation-0.0.5/edation/container.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/domain/__init__.py
--rw-r--r--   0        0        0     9426 2023-07-27 12:51:36.106114 edation-0.0.5/edation/domain/base.py
--rw-r--r--   0        0        0     4321 2023-07-27 12:50:52.326113 edation-0.0.5/edation/domain/data.py
--rw-r--r--   0        0        0     1971 2023-07-27 12:51:56.966113 edation-0.0.5/edation/edation.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/service/__init__.py
--rw-r--r--   0        0        0    13721 2023-07-27 12:50:52.326113 edation-0.0.5/edation/service/io.py
--rw-r--r--   0        0        0     2835 2023-07-27 12:48:19.596113 edation-0.0.5/edation/setup.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/stats/__init__.py
--rw-r--r--   0        0        0     9276 2023-07-27 17:05:13.106114 edation-0.0.5/edation/stats/base.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/stats/centrality/__init__.py
--rw-r--r--   0        0        0     7237 2023-07-27 17:03:51.146113 edation-0.0.5/edation/stats/centrality/ttest.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/stats/correlation/__init__.py
--rw-r--r--   0        0        0     5791 2023-07-27 12:48:08.966113 edation-0.0.5/edation/stats/correlation/pearson.py
--rw-r--r--   0        0        0     5808 2023-07-27 12:48:07.986113 edation-0.0.5/edation/stats/correlation/spearman.py
--rw-r--r--   0        0        0     3657 2023-07-27 12:50:52.326113 edation-0.0.5/edation/stats/descriptive.py
--rw-r--r--   0        0        0    29599 2023-07-27 12:48:11.946113 edation-0.0.5/edation/stats/distribution.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/stats/goodness_of_fit/__init__.py
--rw-r--r--   0        0        0     6728 2023-07-27 12:48:07.056113 edation-0.0.5/edation/stats/goodness_of_fit/chisquare.py
--rw-r--r--   0        0        0     8435 2023-07-27 12:48:06.046113 edation-0.0.5/edation/stats/goodness_of_fit/ksone.py
--rw-r--r--   0        0        0     7403 2023-07-27 12:48:04.936113 edation-0.0.5/edation/stats/goodness_of_fit/kstwo.py
--rw-r--r--   0        0        0     5862 2023-07-27 12:48:03.846113 edation-0.0.5/edation/stats/goodness_of_fit/shapiro.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/stats/independence/__init__.py
--rw-r--r--   0        0        0     9210 2023-07-27 12:48:02.586113 edation-0.0.5/edation/stats/independence/chisquare.py
--rw-r--r--   0        0        0     2212 2023-07-27 12:48:10.986113 edation-0.0.5/edation/stats/profile.py
--rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.5/edation/visual/__init__.py
--rw-r--r--   0        0        0     9944 2023-07-27 12:50:52.326113 edation-0.0.5/edation/visual/association.py
--rw-r--r--   0        0        0     4883 2023-07-27 18:21:38.446113 edation-0.0.5/edation/visual/base.py
--rw-r--r--   0        0        0    12712 2023-07-27 15:26:02.746113 edation-0.0.5/edation/visual/config.py
--rw-r--r--   0        0        0    12022 2023-07-27 14:26:55.666113 edation-0.0.5/edation/visual/distribution.py
--rw-r--r--   0        0        0     2281 2023-07-27 18:22:07.636114 edation-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3575 2023-07-27 18:22:46.615177 edation-0.0.5/setup.py
--rw-r--r--   0        0        0     3493 2023-07-27 18:22:46.615676 edation-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2485 2023-07-27 12:57:53.566113 edation-0.0.6/README.md
+-rw-r--r--   0        0        0     2275 2023-07-27 12:50:52.326113 edation-0.0.6/edation/__init__.py
+-rw-r--r--   0        0        0     2811 2023-07-27 20:10:30.876114 edation-0.0.6/edation/container.py
+-rw-r--r--   0        0        0     1971 2023-07-27 12:51:56.966113 edation-0.0.6/edation/edation.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.6/edation/service/__init__.py
+-rw-r--r--   0        0        0    13721 2023-07-27 12:50:52.326113 edation-0.0.6/edation/service/io.py
+-rw-r--r--   0        0        0     2835 2023-07-27 12:48:19.596113 edation-0.0.6/edation/setup.py
+-rw-r--r--   0        0        0     1662 2023-07-27 20:02:40.738276 edation-0.0.6/edation/stats/__init__.py
+-rw-r--r--   0        0        0     9276 2023-07-27 20:02:41.503271 edation-0.0.6/edation/stats/base.py
+-rw-r--r--   0        0        0     1662 2023-07-27 20:02:40.950291 edation-0.0.6/edation/stats/centrality/__init__.py
+-rw-r--r--   0        0        0      108 2023-07-27 20:02:40.950291 edation-0.0.6/edation/stats/centrality/__init__.py:Zone.Identifier
+-rw-r--r--   0        0        0     7237 2023-07-27 20:02:41.006222 edation-0.0.6/edation/stats/centrality/ttest.py
+-rw-r--r--   0        0        0      108 2023-07-27 20:02:41.006222 edation-0.0.6/edation/stats/centrality/ttest.py:Zone.Identifier
+-rw-r--r--   0        0        0     1662 2023-07-27 20:02:40.843249 edation-0.0.6/edation/stats/correlation/__init__.py
+-rw-r--r--   0        0        0      108 2023-07-27 20:02:40.843249 edation-0.0.6/edation/stats/correlation/__init__.py:Zone.Identifier
+-rw-r--r--   0        0        0     5791 2023-07-27 20:02:40.807221 edation-0.0.6/edation/stats/correlation/pearson.py
+-rw-r--r--   0        0        0      108 2023-07-27 20:02:40.807221 edation-0.0.6/edation/stats/correlation/pearson.py:Zone.Identifier
+-rw-r--r--   0        0        0     5808 2023-07-27 20:02:40.892222 edation-0.0.6/edation/stats/correlation/spearman.py
+-rw-r--r--   0        0        0      108 2023-07-27 20:02:40.892222 edation-0.0.6/edation/stats/correlation/spearman.py:Zone.Identifier
+-rw-r--r--   0        0        0     3657 2023-07-27 20:02:41.456220 edation-0.0.6/edation/stats/descriptive.py
+-rw-r--r--   0        0        0    29599 2023-07-27 20:02:41.305274 edation-0.0.6/edation/stats/distribution.py
+-rw-r--r--   0        0        0     1662 2023-07-27 20:02:41.157273 edation-0.0.6/edation/stats/goodness_of_fit/__init__.py
+-rw-r--r--   0        0        0      108 2023-07-27 20:02:41.157273 edation-0.0.6/edation/stats/goodness_of_fit/__init__.py:Zone.Identifier
+-rw-r--r--   0        0        0     6728 2023-07-27 20:02:41.254275 edation-0.0.6/edation/stats/goodness_of_fit/chisquare.py
+-rw-r--r--   0        0        0      108 2023-07-27 20:02:41.254275 edation-0.0.6/edation/stats/goodness_of_fit/chisquare.py:Zone.Identifier
+-rw-r--r--   0        0        0     8435 2023-07-27 20:02:41.205221 edation-0.0.6/edation/stats/goodness_of_fit/ksone.py
+-rw-r--r--   0        0        0      108 2023-07-27 20:02:41.205221 edation-0.0.6/edation/stats/goodness_of_fit/ksone.py:Zone.Identifier
+-rw-r--r--   0        0        0     7403 2023-07-27 20:02:41.110223 edation-0.0.6/edation/stats/goodness_of_fit/kstwo.py
+-rw-r--r--   0        0        0      108 2023-07-27 20:02:41.110223 edation-0.0.6/edation/stats/goodness_of_fit/kstwo.py:Zone.Identifier
+-rw-r--r--   0        0        0     5862 2023-07-27 20:02:41.062220 edation-0.0.6/edation/stats/goodness_of_fit/shapiro.py
+-rw-r--r--   0        0        0      108 2023-07-27 20:02:41.062220 edation-0.0.6/edation/stats/goodness_of_fit/shapiro.py:Zone.Identifier
+-rw-r--r--   0        0        0     1662 2023-07-27 20:02:41.407218 edation-0.0.6/edation/stats/independence/__init__.py
+-rw-r--r--   0        0        0      108 2023-07-27 20:02:41.407218 edation-0.0.6/edation/stats/independence/__init__.py:Zone.Identifier
+-rw-r--r--   0        0        0     9210 2023-07-27 20:02:41.361223 edation-0.0.6/edation/stats/independence/chisquare.py
+-rw-r--r--   0        0        0      108 2023-07-27 20:02:41.361223 edation-0.0.6/edation/stats/independence/chisquare.py:Zone.Identifier
+-rw-r--r--   0        0        0     2212 2023-07-27 20:02:41.549277 edation-0.0.6/edation/stats/profile.py
+-rw-r--r--   0        0        0     1662 2023-07-27 12:50:52.326113 edation-0.0.6/edation/visual/__init__.py
+-rw-r--r--   0        0        0     9445 2023-07-27 19:44:42.506113 edation-0.0.6/edation/visual/association.py
+-rw-r--r--   0        0        0     2947 2023-07-27 19:39:36.696113 edation-0.0.6/edation/visual/base.py
+-rw-r--r--   0        0        0    11496 2023-07-27 19:36:09.946113 edation-0.0.6/edation/visual/config.py
+-rw-r--r--   0        0        0    11337 2023-07-27 20:12:10.566113 edation-0.0.6/edation/visual/distribution.py
+-rw-r--r--   0        0        0     2281 2023-07-27 20:08:37.626114 edation-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3329 2023-07-27 23:12:09.113452 edation-0.0.6/setup.py
+-rw-r--r--   0        0        0     3493 2023-07-27 23:12:09.113829 edation-0.0.6/PKG-INFO
```

### Comparing `edation-0.0.5/README.md` & `edation-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `edation-0.0.5/edation/__init__.py` & `edation-0.0.6/edation/__init__.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.5/edation/adapter/__init__.py` & `edation-0.0.6/edation/service/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Enter Project Name in Workspace Settings                                            #
 # Version    : 0.1.19                                                                              #
-# Python     : 3.10.11                                                                             #
-# Filename   : /edation/adapter/__init__.py                                                        #
+# Python     : 3.10.10                                                                             #
+# Filename   : /edation/service/__init__.py                                                        #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
-# Created    : Wednesday June 21st 2023 04:52:50 am                                                #
+# Created    : Friday May 26th 2023 11:59:46 pm                                                    #
 # Modified   : Thursday July 27th 2023 08:50:52 am                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
```

### Comparing `edation-0.0.5/edation/adapter/repo/__init__.py` & `edation-0.0.6/edation/visual/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Enter Project Name in Workspace Settings                                            #
 # Version    : 0.1.19                                                                              #
 # Python     : 3.10.11                                                                             #
-# Filename   : /edation/adapter/repo/__init__.py                                                   #
+# Filename   : /edation/visual/__init__.py                                                         #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
-# Created    : Wednesday June 21st 2023 04:52:50 am                                                #
+# Created    : Sunday May 28th 2023 01:20:57 pm                                                    #
 # Modified   : Thursday July 27th 2023 08:50:52 am                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
```

### Comparing `edation-0.0.5/edation/adapter/repo/file_visual.py` & `edation-0.0.6/edation/edation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,27 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Enter Project Name in Workspace Settings                                            #
 # Version    : 0.1.19                                                                              #
 # Python     : 3.10.11                                                                             #
-# Filename   : /edation/adapter/repo/file_visual.py                                                #
+# Filename   : /edation/explorer.py                                                                #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
-# Created    : Friday June 23rd 2023 03:10:02 am                                                   #
-# Modified   : Thursday July 27th 2023 08:48:17 am                                                 #
+# Created    : Wednesday June 21st 2023 03:41:39 am                                                #
+# Modified   : Thursday July 27th 2023 08:51:56 am                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
-import os
-
-from edation.application.ports.driven.repo import RepoPort
 
+from edation.container import EdationContainer
 
 # ------------------------------------------------------------------------------------------------ #
-class FileVisualRepo(RepoPort):
-    """File repository for storing visualizations in image format."""
-
-    def __init__(self, location: str) -> None:
-        super().__init__()
-        self._location = location
-        os.makedirs(self._location, exist_ok=True)
-
-    def add(self, *args, **kwargs) -> None:
-        """Adds an entity to the repository"""
-
-    def get(self, id: str) -> Any:
-        """Retrieves an entity from the repository."""
-
-    def remove(self, id: str) -> None:
-        """Removes an entity from the repository"""
 
-    def registry(self) -> pd.DataFrame:
-        """Returns the registry of entities from the repository"""
+if __name__ == "__main__":
+    container = EdationContainer()
+    container.init_resources()
+    container.wire(modules=["edation.application.ports.driver"])
```

### Comparing `edation-0.0.5/edation/adapter/repo/odb_dataset.py` & `edation-0.0.6/edation/stats/correlation/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Enter Project Name in Workspace Settings                                            #
 # Version    : 0.1.19                                                                              #
 # Python     : 3.10.11                                                                             #
-# Filename   : /edation/adapter/repo/odb_dataset.py                                                #
+# Filename   : /edation/stats/correlation/__init__.py                                              #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
-# Created    : Friday June 23rd 2023 03:06:18 am                                                   #
+# Created    : Sunday May 28th 2023 01:21:49 pm                                                    #
 # Modified   : Thursday July 27th 2023 08:50:52 am                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
```

### Comparing `edation-0.0.5/edation/adapter/repo/odb_tests.py` & `edation-0.0.6/edation/stats/goodness_of_fit/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Enter Project Name in Workspace Settings                                            #
 # Version    : 0.1.19                                                                              #
 # Python     : 3.10.11                                                                             #
-# Filename   : /edation/adapter/repo/odb_tests.py                                                  #
+# Filename   : /edation/stats/goodness_of_fit/__init__.py                                          #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
-# Created    : Friday June 23rd 2023 03:03:22 am                                                   #
+# Created    : Sunday May 28th 2023 01:21:49 pm                                                    #
 # Modified   : Thursday July 27th 2023 08:50:52 am                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
```

### Comparing `edation-0.0.5/edation/adapter/repo/odb_visual.py` & `edation-0.0.6/edation/stats/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Enter Project Name in Workspace Settings                                            #
 # Version    : 0.1.19                                                                              #
 # Python     : 3.10.11                                                                             #
-# Filename   : /edation/adapter/repo/odb_visual.py                                                 #
+# Filename   : /edation/stats/__init__.py                                                          #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
-# Created    : Friday June 23rd 2023 03:09:45 am                                                   #
+# Created    : Sunday May 28th 2023 01:21:49 pm                                                    #
 # Modified   : Thursday July 27th 2023 08:50:52 am                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
```

### Comparing `edation-0.0.5/edation/adapter/stats/__init__.py` & `edation-0.0.6/edation/stats/independence/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Enter Project Name in Workspace Settings                                            #
 # Version    : 0.1.19                                                                              #
 # Python     : 3.10.11                                                                             #
-# Filename   : /edation/adapter/stats/__init__.py                                                  #
+# Filename   : /edation/stats/independence/__init__.py                                             #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
-# Created    : Wednesday June 21st 2023 04:52:50 am                                                #
+# Created    : Sunday May 28th 2023 01:21:49 pm                                                    #
 # Modified   : Thursday July 27th 2023 08:50:52 am                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
```

### Comparing `edation-0.0.5/edation/application/__init__.py` & `edation-0.0.6/edation/stats/centrality/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Enter Project Name in Workspace Settings                                            #
 # Version    : 0.1.19                                                                              #
 # Python     : 3.10.11                                                                             #
-# Filename   : /edation/application/__init__.py                                                    #
+# Filename   : /edation/stats/centrality/__init__.py                                               #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
-# Created    : Wednesday June 21st 2023 04:52:50 am                                                #
+# Created    : Sunday May 28th 2023 01:21:49 pm                                                    #
 # Modified   : Thursday July 27th 2023 08:50:52 am                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
```

### Comparing `edation-0.0.5/edation/application/ports/driver/base.py` & `edation-0.0.6/edation/stats/profile.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,34 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Enter Project Name in Workspace Settings                                            #
 # Version    : 0.1.19                                                                              #
 # Python     : 3.10.11                                                                             #
-# Filename   : /edation/application/ports/driver/base.py                                           #
+# Filename   : /edation/stats/profile.py                                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
-# Created    : Friday June 23rd 2023 07:55:16 am                                                   #
-# Modified   : Thursday July 27th 2023 08:48:16 am                                                 #
+# Created    : Sunday May 28th 2023 06:24:28 pm                                                    #
+# Modified   : Thursday July 27th 2023 08:48:10 am                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
-from abc import ABC
+"""Profile Module for the Statistical Analytics Package"""
 from dataclasses import dataclass
-from datetime import datetime
+from edation.stats.base import StatTestProfile
 
-from edation import IMMUTABLE_TYPES, SEQUENCE_TYPES
 
-
-# ------------------------------------------------------------------------------------------------ #
-#                                 ABSTRACT DTO                                                     #
 # ------------------------------------------------------------------------------------------------ #
 @dataclass
-class DTO(ABC):
-    """Abstract base class for Configuration data classes."""
+class StatTestProfileOne(StatTestProfile):
+    X_variable_type: str = None
 
-    def as_dict(self) -> dict:
-        """Returns a dictionary representation of the the Legend object."""
-        return {k: self._export_config(v) for k, v in self.__dict__.items()}
 
-    @classmethod
-    def _export_config(cls, v):  # pragma: no cover
-        """Returns v with Configs converted to dicts, recursively."""
-        if isinstance(v, IMMUTABLE_TYPES):
-            return v
-        elif isinstance(v, SEQUENCE_TYPES):
-            return type(v)(map(cls._export_config, v))
-        elif isinstance(v, datetime):
-            return v
-        elif isinstance(v, dict):
-            return v
-        elif hasattr(v, "as_dict"):
-            return v.as_dict()
-        else:
-            return v
+# ------------------------------------------------------------------------------------------------ #
+@dataclass
+class StatTestProfileTwo(StatTestProfile):
+    X_variable_type: str = None
+    Y_variable_type: str = None
```

### Comparing `edation-0.0.5/edation/container.py` & `edation-0.0.6/edation/container.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,56 +7,37 @@
 # Filename   : /edation/container.py                                                               #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Monday March 27th 2023 07:02:56 pm                                                  #
-# Modified   : Thursday July 27th 2023 08:51:35 am                                                 #
+# Modified   : Thursday July 27th 2023 04:10:30 pm                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 """Framework Dependency Container"""
 import logging.config  # pragma: no cover
 
 from dependency_injector import containers, providers
 
-from edation.adapter.identity import IDGenerator, FakeIDGenerator
-
 
 # ------------------------------------------------------------------------------------------------ #
 #                                        LOGGING                                                   #
 # ------------------------------------------------------------------------------------------------ #
 class LoggingContainer(containers.DeclarativeContainer):
     config = providers.Configuration()
 
     logging = providers.Resource(
         logging.config.dictConfig,
         config=config,
     )
 
 
 # ------------------------------------------------------------------------------------------------ #
-#                                          ADAPTER                                                 #
-# ------------------------------------------------------------------------------------------------ #
-class AdapterContainer(containers.DeclarativeContainer):
-    config = providers.Configuration()
-
-    idgen = providers.Singleton(IDGenerator, filepath=config.idgen.filepath, size=config.idgen.size)
-
-    fake_idgen = providers.Singleton(FakeIDGenerator)
-
-
-# ------------------------------------------------------------------------------------------------ #
 #                                          FRAMEWORK                                               #
 # ------------------------------------------------------------------------------------------------ #
 class EdationContainer(containers.DeclarativeContainer):
     log_config = providers.Configuration(yaml_files=["config/logging.yml"])
 
-    stats_config = providers.Configuration(yaml_files=["config/stats.yml"])
-
-    adapter_config = providers.Configuration(yaml_files=["config/adapters.yml"])
-
     logs = providers.Container(LoggingContainer, config=log_config.logging)
-
-    adapters = providers.Container(AdapterContainer, config=adapter_config)
```

### Comparing `edation-0.0.5/edation/domain/base.py` & `edation-0.0.6/edation/stats/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,159 +1,82 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Enter Project Name in Workspace Settings                                            #
 # Version    : 0.1.19                                                                              #
-# Python     : 3.10.11                                                                             #
-# Filename   : /edation/domain/base.py                                                             #
+# Python     : 3.10.10                                                                             #
+# Filename   : /edation/stats/base.py                                                              #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
-# Created    : Wednesday June 21st 2023 07:45:48 pm                                                #
-# Modified   : Thursday July 27th 2023 08:51:36 am                                                 #
+# Created    : Monday June 5th 2023 12:13:09 am                                                    #
+# Modified   : Thursday July 27th 2023 01:05:12 pm                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
-"""Base Module for the Analysis Package"""
 from __future__ import annotations
 from abc import ABC, abstractmethod
-from dataclasses import dataclass, fields
-from datetime import datetime
 import logging
+from dataclasses import dataclass, fields
+from typing import Union
 
-from dependency_injector.wiring import inject, Provide
 import pandas as pd
+import matplotlib.pyplot as plt
+import numpy as np
+import seaborn as sns
+from scipy import stats
+
+from edation.service.io import IOService
+from edation import IMMUTABLE_TYPES, SEQUENCE_TYPES
+from edation.visual.config import Canvas
+
+# ------------------------------------------------------------------------------------------------ #
+sns.set_style(Canvas.style)
+# ------------------------------------------------------------------------------------------------ #
+ANALYSIS_TYPES = {
+    "univariate": "Univariate",
+    "bivariate": "Bivariate",
+    "multivariate": "Multivariate",
+}
+STAT_CONFIG = "config/stats.yml"
 
 
-from edation.container import EdationContainer
-
-
-# ------------------------------------------------------------------------------------------------ #
-#                                        DATA                                                      #
-# ------------------------------------------------------------------------------------------------ #
-class Data(ABC):
-    """Encapsulates the data used in an analysis"""
-
-    @property
-    @abstractmethod
-    def metadata(self) -> dict:
-        """Returns metadata that identifies and distinguishes the dataset."""
-
-    @property
-    @abstractmethod
-    def summary(self) -> pd.DataFrame:
-        """Provides summary metrics at the dataset level."""
-
-    @property
-    @abstractmethod
-    def info(self) -> pd.DataFrame:
-        """Immulates the pandas DataFrame info method"""
-
-    @abstractmethod
-    def describe(self, include: list = None, exclude: list = None) -> pd.DataFrame:
-        """Reports descriptive statistics for the DataFrame.
-
-        Args:
-            include (list) Optional list of dtypes to include in the analysis.
-            exclude (list) Optional list of dtypes to exclude from the analysis.
-        """
-
-    @abstractmethod
-    def head(self, n: int = 5) -> pd.DataFrame:
-        """Returns the top n rows from the DataFrame."""
-
-
-# ------------------------------------------------------------------------------------------------ #
-#                                        PLOT                                                      #
-# ------------------------------------------------------------------------------------------------ #
-class Plot(ABC):
-    """Abstraction for classes that encapsulate plots."""
-
-    @abstractmethod
-    def fit(
-        self,
-        dataset: pd.DataFrame,
-        x: str,
-        y: str = None,
-        z: str = None,
-        *args,
-        **kwargs,
-    ) -> Plot:
-        """Fits the data to the plot
-
-        Args:
-            dataset (pd.DataFrame): DataFrame containing the data to be plotted.
-            x: (str): Name of the column in the dataset to be plotted along the x-axis.
-            y: (str): Optional name of the column in the dataset to be plotted along the y-axis.
-            z: (str): Optional name of the column to be used as a third dimension.
-            canvas (Canvas): Optional Canvas object upon which the plot will be rendered.
-                If a Canvas is not provided, one will be created.
-            *args, **kwargs: Positional and keyword arguments of subclasses.
-
-        """
-
-    @abstractmethod
-    def show(self) -> None:
-        """Renders the plot."""
-
-    @abstractmethod
-    def export(self, filepath: str) -> None:
-        """Saves plot as an image to file."""
-
-
-# ------------------------------------------------------------------------------------------------ #
-#                                       VISUAL                                                     #
 # ------------------------------------------------------------------------------------------------ #
-class Visual(ABC):
-    """Specifies a visualization object."""
-
-    def __init__(self, data: Data, config: Config) -> None:
-        self._data = data
-        self._config = config
-        self._logger = logging.getLogger(f"{self.__class__.__name__}")
-
-    @abstractmethod
-    def add_plot(self, name: str, plot: Plot) -> None:
-        """Adds a Plot object to the Visual
-        Args:
-            name (str): Unique name for plot in the visual
-            plot (Plot): A Plot object.
-        """
+@dataclass
+class Description(ABC):
+    """Descriptive statistics for distributions"""
 
-    @abstractmethod
-    def show(self) -> None:
-        """Renders the visualization"""
+    count: int  # Non-Nulls only
+    length: int  # Total length of iterable.
+    size: int
 
 
 # ------------------------------------------------------------------------------------------------ #
-#                          STATISTICAL TEST PROFILE                                                #
-# ------------------------------------------------------------------------------------------------ #
-@inject
 @dataclass
 class StatTestProfile(ABC):
-    """Abstract base class specifying the parameters for the statistical test."""
+    """Abstract base class defining the interface for statistical tests.
+
+    Interface inspired by: https://doc.dataiku.com/dss/latest/statistics/tests.html
+    """
 
     id: str
     name: str = None
     description: str = None
     statistic: str = None
     analysis: str = None  # one of ANALYSIS_TYPES
     hypothesis: str = None  # One of HYPOTHESIS_TYPES
     H0: str = None
     parametric: bool = None
     min_sample_size: int = None
     assumptions: str = None
     use_when: str = None
 
-    def __post_init__(self, stats_config=Provide[EdationContainer.stats_config]) -> None:
-        self._stats_config = stats_config
-
     def __repr__(self) -> str:
         return "{}({})".format(
             self.__class__.__name__,
             ", ".join("{}={!r}".format(k, v) for k, v in self.__dict__.items()),
         )
 
     def __str__(self) -> str:
@@ -162,28 +85,101 @@
         for k, v in self.__dict__.items():
             s += f"\t{k.rjust(width,' ')} | {v}\n"
         return s
 
     @classmethod
     def create(cls, id) -> None:
         """Loads the values from the statistical tests file"""
-
-        profile = cls._stats_config[id]
+        profiles = IOService.read(STAT_CONFIG)
+        profile = profiles[id]
         fieldlist = {f.name for f in fields(cls) if f.init}
         filtered_dict = {k: v for k, v in profile.items() if k in fieldlist}
         filtered_dict["id"] = id
         return cls(**filtered_dict)
 
 
 # ------------------------------------------------------------------------------------------------ #
-#                              STATISTICAL TEST ABC                                                #
+@dataclass
+class StatTestResult(ABC):
+    test: str
+    hypothesis: str
+    H0: str
+    statistic: str
+    value: float
+    pvalue: float
+    inference: str
+    alpha: float = 0.05
+    result: str = None
+    interpretation: str = None
+
+    def __repr__(self) -> str:
+        return "{}({})".format(
+            self.__class__.__name__,
+            ", ".join(
+                "{}={!r}".format(k, v)
+                for k, v in self.__dict__.items()
+                if type(v) in IMMUTABLE_TYPES
+            ),
+        )
+
+    def __str__(self) -> str:
+        s = ""
+        width = 32
+        for k, v in self.__dict__.items():
+            if type(v) in IMMUTABLE_TYPES:
+                s += f"\t{k.rjust(width,' ')} | {v}\n"
+        return s
+
+    def _fill_reject_region(
+        self,
+        ax: plt.Axes,
+        lower: float,
+        upper: float,
+        lower_critical: float,
+        upper_critical: float,
+        dof: int,
+    ) -> plt.Axes:
+        """Fills the area under the curve at the value of the hypothesis test statistic."""
+
+        # Fill lower tail
+        xlower = np.arange(lower, lower_critical, 0.001)
+        ax.fill_between(x=xlower, y1=0, y2=stats.t.pdf(xlower, dof), color=Canvas.colors.orange)
+
+        # Fill Upper Tail
+        xupper = np.arange(upper_critical, upper, 0.001)
+        ax.fill_between(x=xupper, y1=0, y2=stats.t.pdf(xupper, dof), color=Canvas.colors.orange)
+
+        # Plot the statistic
+        line = ax.lines[0]
+        xdata = line.get_xydata()[:, 0]
+        ydata = line.get_xydata()[:, 1]
+        try:
+            idx = np.where(xdata > self.value)[0][0]
+            x = xdata[idx]
+            y = ydata[idx]
+            ax = sns.regplot(
+                x=np.array([x]),
+                y=np.array([y]),
+                scatter=True,
+                fit_reg=False,
+                marker="o",
+                scatter_kws={"s": 100},
+                ax=ax,
+                color=Canvas.colors.dark_blue,
+            )
+        except IndexError:
+            pass
+
+        return ax
+
+
 # ------------------------------------------------------------------------------------------------ #
-@inject
 class StatisticalTest(ABC):
-    def __init__(self) -> None:
+    def __init__(self, io: IOService = IOService) -> None:
+        self._io = io
         self._logger = logging.getLogger(f"{self.__class__.__name__}")
 
     @property
     @abstractmethod
     def profile(self) -> StatTestProfile:
         """Returns the statistical test profile."""
 
@@ -205,39 +201,53 @@
 
     def _report_alpha(self) -> str:
         a = int(self._alpha * 100)
         return f"significant at {a}%."
 
 
 # ------------------------------------------------------------------------------------------------ #
-#                               STATISTICAL TEST RESULT                                            #
-# ------------------------------------------------------------------------------------------------ #
-@dataclass
-class StatTestResult(ABC):
-    test: str
-    hypothesis: str
-    H0: str
-    statistic: str
-    value: float
-    pvalue: float
-    inference: str
-    alpha: float = 0.05
-    result: str = None
-    interpretation: str = None
+class StatisticalTestTwo(StatisticalTest):
+    """Abstract base class for bivariate statistial tests."""
 
-    def __repr__(self) -> str:
-        return "{}({})".format(
-            self.__class__.__name__,
-            ", ".join(
-                "{}={!r}".format(k, v)
-                for k, v in self.__dict__.items()
-                if type(v) in IMMUTABLE_TYPES
-            ),
-        )
+    def _parse_arguments(
+        self, data: pd.DataFrame, x: Union[np.ndarray, str], y: Union[np.ndarray, str]
+    ) -> None:
+        """Parses arguments into a 2 column DataFrame and x,y column names"""
+        msg = ""
+        if isinstance(data, pd.DataFrame):
+            if data.shape[1] == 2:
+                x, y = data.columns
+                return data, x, y
+            elif data.shape[1] > 2:
+                if self._is_column(data, x) and self._is_column(data, y) and x != y:
+                    return data, x, y
+                else:
+                    msg += "Arguments are ambiguous. If data contains more than two columns, x and y must reference columns in data."
+
+        elif data is None:
+            if self._is_iterable(x) and self._is_iterable(y):
+                return self._make_df(x, y)
+            else:
+                msg += "Arguments are ambiguous. Data must be a dataframe and x,y column names, or x and y must be array-like."
+        else:
+            msg += "Arguments are ambiguous. Data must be a dataframe and x,y column names, or x and y must be array-like."
 
-    def __str__(self) -> str:
-        s = ""
-        width = 32
-        for k, v in self.__dict__.items():
-            if type(v) in IMMUTABLE_TYPES:
-                s += f"\t{k.rjust(width,' ')} | {v}\n"
-        return s
+        if len(msg) > 0:
+            self._logger.error(msg)
+            raise ValueError(msg)
+
+    def _make_df(self, x: np.ndarray, y: np.ndarray) -> pd.DataFrame:
+        """Converts two arrays to a DataFrame"""
+        d = {"Sample 1": x, "Sample 2": y}
+        df = pd.DataFrame(data=d)
+        x = "Sample 1"
+        y = "Sample 2"
+        return df, x, y
+
+    def _is_iterable(self, a) -> bool:
+        return type(a) in SEQUENCE_TYPES or isinstance(a, pd.Series)
+
+    def _is_column(self, data: pd.DataFrame, a: str) -> bool:
+        if not isinstance(a, str):
+            return False
+        else:
+            return a in data.columns
```

### Comparing `edation-0.0.5/edation/service/io.py` & `edation-0.0.6/edation/service/io.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.5/edation/setup.py` & `edation-0.0.6/edation/setup.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.5/edation/stats/base.py` & `edation-0.0.6/edation/stats/goodness_of_fit/ksone.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,253 +1,183 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Enter Project Name in Workspace Settings                                            #
 # Version    : 0.1.19                                                                              #
 # Python     : 3.10.10                                                                             #
-# Filename   : /edation/stats/base.py                                                              #
+# Filename   : /edation/stats/goodness_of_fit/ksone.py                                             #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
-# Created    : Monday June 5th 2023 12:13:09 am                                                    #
-# Modified   : Thursday July 27th 2023 01:05:12 pm                                                 #
+# Created    : Tuesday June 6th 2023 01:45:05 am                                                   #
+# Modified   : Thursday July 27th 2023 08:48:05 am                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
-from __future__ import annotations
-from abc import ABC, abstractmethod
-import logging
-from dataclasses import dataclass, fields
-from typing import Union
+from dataclasses import dataclass
+from typing import Union, Tuple
 
+import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
-import numpy as np
 import seaborn as sns
 from scipy import stats
 
-from edation.service.io import IOService
-from edation import IMMUTABLE_TYPES, SEQUENCE_TYPES
+from edation.stats.profile import StatTestProfileOne
+from edation.stats.base import StatTestResult, StatisticalTest, StatTestProfile
 from edation.visual.config import Canvas
+from edation.stats.distribution import DISTRIBUTIONS
+from edation.stats.distribution import RVSDistribution
 
 # ------------------------------------------------------------------------------------------------ #
-sns.set_style(Canvas.style)
+MC_SAMPLES = 100
 # ------------------------------------------------------------------------------------------------ #
-ANALYSIS_TYPES = {
-    "univariate": "Univariate",
-    "bivariate": "Bivariate",
-    "multivariate": "Multivariate",
-}
-STAT_CONFIG = "config/stats.yml"
+sns.set_style(Canvas.style)
 
 
 # ------------------------------------------------------------------------------------------------ #
-@dataclass
-class Description(ABC):
-    """Descriptive statistics for distributions"""
-
-    count: int  # Non-Nulls only
-    length: int  # Total length of iterable.
-    size: int
-
-
+#                                     TEST RESULT                                                  #
 # ------------------------------------------------------------------------------------------------ #
 @dataclass
-class StatTestProfile(ABC):
-    """Abstract base class defining the interface for statistical tests.
-
-    Interface inspired by: https://doc.dataiku.com/dss/latest/statistics/tests.html
-    """
-
-    id: str
-    name: str = None
-    description: str = None
-    statistic: str = None
-    analysis: str = None  # one of ANALYSIS_TYPES
-    hypothesis: str = None  # One of HYPOTHESIS_TYPES
-    H0: str = None
-    parametric: bool = None
-    min_sample_size: int = None
-    assumptions: str = None
-    use_when: str = None
-
-    def __repr__(self) -> str:
-        return "{}({})".format(
-            self.__class__.__name__,
-            ", ".join("{}={!r}".format(k, v) for k, v in self.__dict__.items()),
+class KSOneTestResult(StatTestResult):
+    reference_distribution: str = None
+    data: Union[pd.DataFrame, np.ndarray, pd.Series] = None
+
+    def plot(self, ax: plt.Axes = None) -> plt.Axes:  # pragma: no cover
+        """Plots the critical values and shades the area on the KS distribution
+
+        Args:
+            ax (plt.Axes): A matplotlib Axes object. Optional
+        """
+        canvas = Canvas()
+        ax = ax or canvas.ax
+
+        # Get the callable for the statistic.
+        n = len(self.data)
+
+        x = np.linspace(stats.ksone.ppf(0.01, n), stats.ksone.ppf(0.999, n), 500)
+        y = stats.ksone.pdf(x, n)
+        ax = sns.lineplot(
+            x=x, y=y, markers=False, dashes=False, sort=True, ax=ax, color=canvas.colors.dark_blue
         )
 
-    def __str__(self) -> str:
-        s = ""
-        width = 20
-        for k, v in self.__dict__.items():
-            s += f"\t{k.rjust(width,' ')} | {v}\n"
-        return s
-
-    @classmethod
-    def create(cls, id) -> None:
-        """Loads the values from the statistical tests file"""
-        profiles = IOService.read(STAT_CONFIG)
-        profile = profiles[id]
-        fieldlist = {f.name for f in fields(cls) if f.init}
-        filtered_dict = {k: v for k, v in profile.items() if k in fieldlist}
-        filtered_dict["id"] = id
-        return cls(**filtered_dict)
-
-
-# ------------------------------------------------------------------------------------------------ #
-@dataclass
-class StatTestResult(ABC):
-    test: str
-    hypothesis: str
-    H0: str
-    statistic: str
-    value: float
-    pvalue: float
-    inference: str
-    alpha: float = 0.05
-    result: str = None
-    interpretation: str = None
-
-    def __repr__(self) -> str:
-        return "{}({})".format(
-            self.__class__.__name__,
-            ", ".join(
-                "{}={!r}".format(k, v)
-                for k, v in self.__dict__.items()
-                if type(v) in IMMUTABLE_TYPES
-            ),
+        # Compute reject region
+        upper_alpha = 1 - (self.alpha)
+        upper = stats.ksone.ppf(upper_alpha, n)
+
+        # Fill reject region at critical points
+        self._fill_curve(ax, upper=upper)
+
+        ax.set_title(
+            f"Goodness of Fit\n{self.reference_distribution.capitalize()} Distribution\n{self.result}",
+            fontsize=canvas.fontsize_title,
         )
 
-    def __str__(self) -> str:
-        s = ""
-        width = 32
-        for k, v in self.__dict__.items():
-            if type(v) in IMMUTABLE_TYPES:
-                s += f"\t{k.rjust(width,' ')} | {v}\n"
-        return s
-
-    def _fill_reject_region(
-        self,
-        ax: plt.Axes,
-        lower: float,
-        upper: float,
-        lower_critical: float,
-        upper_critical: float,
-        dof: int,
-    ) -> plt.Axes:
-        """Fills the area under the curve at the value of the hypothesis test statistic."""
-
-        # Fill lower tail
-        xlower = np.arange(lower, lower_critical, 0.001)
-        ax.fill_between(x=xlower, y1=0, y2=stats.t.pdf(xlower, dof), color=Canvas.colors.orange)
-
-        # Fill Upper Tail
-        xupper = np.arange(upper_critical, upper, 0.001)
-        ax.fill_between(x=xupper, y1=0, y2=stats.t.pdf(xupper, dof), color=Canvas.colors.orange)
-
-        # Plot the statistic
-        line = ax.lines[0]
-        xdata = line.get_xydata()[:, 0]
-        ydata = line.get_xydata()[:, 1]
-        try:
-            idx = np.where(xdata > self.value)[0][0]
-            x = xdata[idx]
-            y = ydata[idx]
-            ax = sns.regplot(
-                x=np.array([x]),
-                y=np.array([y]),
-                scatter=True,
-                fit_reg=False,
-                marker="o",
-                scatter_kws={"s": 100},
-                ax=ax,
-                color=Canvas.colors.dark_blue,
-            )
-        except IndexError:
-            pass
-
+        ax.set_xlabel("Value")
+        ax.set_ylabel("Probability Density")
         return ax
 
+    def plotpdf(self, ax: plt.Axes = None) -> plt.Axes:  # pragma: no cover)
+        """Plots the data against the theoretical probability distribution function.
+
+        Args:
+            ax (plt.Axes): A matplotlib Axes object. Optional
+        """
+        dist = RVSDistribution()
+        dist(data=self.data, distribution=self.reference_distribution)
+        return dist.histpdfplot()
+
+    def plotcdf(self, ax: plt.Axes = None) -> plt.Axes:  # pragma: no cover)
+        """Plots the data against the theoretical cumulative distribution function.
+
+        Args:
+            ax (plt.Axes): A matplotlib Axes object. Optional
+        """
+        dist = RVSDistribution()
+        dist(data=self.data, distribution=self.reference_distribution)
+        return dist.ecdfplot()
+
 
 # ------------------------------------------------------------------------------------------------ #
-class StatisticalTest(ABC):
-    def __init__(self, io: IOService = IOService) -> None:
-        self._io = io
-        self._logger = logging.getLogger(f"{self.__class__.__name__}")
+#                                          TEST                                                    #
+# ------------------------------------------------------------------------------------------------ #
+class KSOneTest(StatisticalTest):
+    __id = "ks1"
+
+    def __init__(self, alpha: float = 0.05) -> None:
+        super().__init__()
+        self._alpha = alpha
+        self._profile = StatTestProfileOne.create(self.__id)
+        self._result = None
 
     @property
-    @abstractmethod
     def profile(self) -> StatTestProfile:
         """Returns the statistical test profile."""
+        return self._profile
+
+    @property
+    def data(self) -> Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]:
+        """Returns the data tested"""
+        return self._data
 
     @property
-    @abstractmethod
     def result(self) -> StatTestResult:
         """Returns a Statistical Test Result object."""
+        return self._result
 
-    @abstractmethod
-    def __call__(self, *args, **kwargs) -> None:
-        """Performs the statistical test and creates a result object."""
-
-    def _report_pvalue(self, pvalue: float) -> str:
-        """Rounds the pvalue in accordance with the APA Style Guide 7th Edition"""
-        if pvalue < 0.001:
-            return "p<.001"
-        else:
-            return "P=" + str(round(pvalue, 3))
+    def __call__(self, data: np.ndarray, reference_distribution: str) -> None:
+        """Performs the statistical test and creates a result object.
 
-    def _report_alpha(self) -> str:
-        a = int(self._alpha * 100)
-        return f"significant at {a}%."
+        Args:
+            data (np.ndarray): 1D Numpy array of data to be tested.
+            reference_distribution (str): A reference distribution from the scipy list
+                of Continuous Distributions at https://docs.scipy.org/doc/scipy/reference/stats.html
 
+        """
+        self._data = data
 
-# ------------------------------------------------------------------------------------------------ #
-class StatisticalTestTwo(StatisticalTest):
-    """Abstract base class for bivariate statistial tests."""
-
-    def _parse_arguments(
-        self, data: pd.DataFrame, x: Union[np.ndarray, str], y: Union[np.ndarray, str]
-    ) -> None:
-        """Parses arguments into a 2 column DataFrame and x,y column names"""
-        msg = ""
-        if isinstance(data, pd.DataFrame):
-            if data.shape[1] == 2:
-                x, y = data.columns
-                return data, x, y
-            elif data.shape[1] > 2:
-                if self._is_column(data, x) and self._is_column(data, y) and x != y:
-                    return data, x, y
-                else:
-                    msg += "Arguments are ambiguous. If data contains more than two columns, x and y must reference columns in data."
-
-        elif data is None:
-            if self._is_iterable(x) and self._is_iterable(y):
-                return self._make_df(x, y)
-            else:
-                msg += "Arguments are ambiguous. Data must be a dataframe and x,y column names, or x and y must be array-like."
-        else:
-            msg += "Arguments are ambiguous. Data must be a dataframe and x,y column names, or x and y must be array-like."
-
-        if len(msg) > 0:
+        # Conduct the two-sided ks test
+        try:
+            result = stats.goodness_of_fit(
+                dist=DISTRIBUTIONS[reference_distribution],
+                data=data,
+                statistic="ks",
+                n_mc_samples=MC_SAMPLES,
+            )
+        except KeyError as e:
+            msg = f"Distribution {reference_distribution} is not supported.\n{e}"
             self._logger.error(msg)
-            raise ValueError(msg)
+            raise
 
-    def _make_df(self, x: np.ndarray, y: np.ndarray) -> pd.DataFrame:
-        """Converts two arrays to a DataFrame"""
-        d = {"Sample 1": x, "Sample 2": y}
-        df = pd.DataFrame(data=d)
-        x = "Sample 1"
-        y = "Sample 2"
-        return df, x, y
-
-    def _is_iterable(self, a) -> bool:
-        return type(a) in SEQUENCE_TYPES or isinstance(a, pd.Series)
-
-    def _is_column(self, data: pd.DataFrame, a: str) -> bool:
-        if not isinstance(a, str):
-            return False
+        self._logger.debug(
+            f"\n\nType Pvalue: {type(result.pvalue)}\nType Statistic{type(result.statistic)}"
+        )
+
+        if result.pvalue > self._alpha:
+            inference = f"The pvalue {round(result.pvalue,2)} is greater than level of significance {int(self._alpha*100)}%; therefore, the null hypothesis is not rejected. The evidence against the data being drawn from the {reference_distribution} distribution is not significant."
         else:
-            return a in data.columns
+            inference = f"The pvalue {round(result.pvalue,2)} is less than level of significance {int(self._alpha*100)}%; therefore, the null hypothesis is rejected. The evidence against the data being drawn from the {reference_distribution} distribution is significant."
+
+        interpretation = None
+        if len(data) < 50:
+            interpretation = "Note: The Kolmogorov-Smirnov Test requires a sample size N > 50. For smaller sample sizes, the Shapiro-Wilk test should be considered."
+        if len(data) > 1000:
+            interpretation = "Note: The Kolmogorov-Smirnov Test on large sample sizes may lead to rejections of the null hypothesis that are statistically significant, yet practically insignificant."
+
+        # Create the result object.
+        self._result = KSOneTestResult(
+            test=self._profile.name,
+            H0=self._profile.H0,
+            statistic=self._profile.statistic,
+            hypothesis=self._profile.hypothesis,
+            value=result.statistic,
+            pvalue=result.pvalue,
+            result=f"(N={len(data)})={round(result.statistic,2)}, {self._report_pvalue(result.pvalue)} {self._report_alpha()}",
+            data=data,
+            reference_distribution=reference_distribution,
+            inference=inference,
+            interpretation=interpretation,
+            alpha=self._alpha,
+        )
```

### Comparing `edation-0.0.5/edation/stats/centrality/ttest.py` & `edation-0.0.6/edation/stats/centrality/ttest.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.5/edation/stats/correlation/pearson.py` & `edation-0.0.6/edation/stats/correlation/pearson.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.5/edation/stats/correlation/spearman.py` & `edation-0.0.6/edation/stats/correlation/spearman.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.5/edation/stats/descriptive.py` & `edation-0.0.6/edation/stats/descriptive.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.5/edation/stats/distribution.py` & `edation-0.0.6/edation/stats/distribution.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.5/edation/stats/goodness_of_fit/chisquare.py` & `edation-0.0.6/edation/stats/goodness_of_fit/chisquare.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.5/edation/stats/goodness_of_fit/kstwo.py` & `edation-0.0.6/edation/stats/goodness_of_fit/kstwo.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.5/edation/stats/goodness_of_fit/shapiro.py` & `edation-0.0.6/edation/stats/goodness_of_fit/shapiro.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.5/edation/stats/independence/chisquare.py` & `edation-0.0.6/edation/stats/independence/chisquare.py`

 * *Files identical despite different names*

### Comparing `edation-0.0.5/edation/visual/association.py` & `edation-0.0.6/edation/visual/association.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,38 +7,36 @@
 # Filename   : /edation/visual/association.py                                                      #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Tuesday June 20th 2023 07:57:56 pm                                                  #
-# Modified   : Thursday July 27th 2023 08:50:52 am                                                 #
+# Modified   : Thursday July 27th 2023 03:44:42 pm                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 """Visualizations that Reveal Associations between Variables."""
 import pandas as pd
 
 import seaborn as sns
 import matplotlib.pyplot as plt
 
 from .base import Visual
+from .config import Canvas
 
 # ------------------------------------------------------------------------------------------------ #
 #                                        SCATTERPLOT                                               #
 # ------------------------------------------------------------------------------------------------ #
 
 
 class ScatterPlot(Visual):  # pragma: no cover
     """Draw a scatter plot with possibility of several semantic groupings."""
 
-    def __init__(self) -> None:
-        super().__init__()
-
     def __call__(
         self,
         data: pd.DataFrame,
         x: str,
         y: str = None,
         hue: str = None,
         ax: plt.Axes = None,
@@ -60,16 +58,15 @@
             palette (str): A string indicating one of the supported palettes. See docstring for
                 Palette class in config module. Defaults to 'winter_blue'.
             args and kwargs passed to the underlying seaborn histplot method.
                 See https://seaborn.pydata.org/generated/seaborn.histplot.html for a
                 complete list of parameters.
         """
 
-        ax = self.get_or_create_ax(ax)
-        style = self.get_set_styling(style=style, palette=palette)
+        ax = ax or Canvas().ax
 
         ax = sns.scatterplot(
             data=data,
             x=x,
             y=y,
             hue=hue,
             ax=ax,
@@ -84,17 +81,14 @@
 #                                        LINE PLOT                                                 #
 # ------------------------------------------------------------------------------------------------ #
 
 
 class LinePlot(Visual):  # pragma: no cover
     """Draw a scatter plot with possibility of several semantic groupings."""
 
-    def __init__(self) -> None:
-        super().__init__()
-
     def __call__(
         self,
         data: pd.DataFrame,
         x: str,
         y: str = None,
         hue: str = None,
         ax: plt.Axes = None,
@@ -116,16 +110,15 @@
             palette (str): A string indicating one of the supported palettes. See docstring for
                 Palette class in config module. Defaults to 'winter_blue'.
             args and kwargs passed to the underlying seaborn histplot method.
                 See https://seaborn.pydata.org/generated/seaborn.histplot.html for a
                 complete list of parameters.
         """
 
-        ax = self.get_or_create_ax(ax)
-        style = self.get_set_styling(style=style, palette=palette)
+        ax = ax or Canvas().ax
 
         ax = sns.lineplot(
             data=data,
             x=x,
             y=y,
             hue=hue,
             ax=ax,
@@ -140,17 +133,14 @@
 #                                        PAIR PLOT                                                 #
 # ------------------------------------------------------------------------------------------------ #
 
 
 class PairPlot(Visual):  # pragma: no cover
     """Plot pairwise relationships in a dataset. This is a figure level plot showing a grid of axes."""
 
-    def __init__(self) -> None:
-        super().__init__()
-
     def __call__(
         self,
         data: pd.DataFrame,
         hue: str = None,
         vars: list = None,
         x_vars: list = None,
         y_vars: list = None,
@@ -172,16 +162,14 @@
             palette (str): A string indicating one of the supported palettes. See docstring for
                 Palette class in config module. Defaults to 'winter_blue'.
             args and kwargs passed to the underlying seaborn histplot method.
                 See https://seaborn.pydata.org/generated/seaborn.histplot.html for a
                 complete list of parameters.
         """
 
-        style = self.get_set_styling(style=style, palette=palette)
-
         g = sns.pairplot(
             data=data,
             hue=hue,
             vars=vars,
             x_vars=x_vars,
             y_vars=y_vars,
             *args,
@@ -196,17 +184,14 @@
 #                                       JOINT PLOT                                                 #
 # ------------------------------------------------------------------------------------------------ #
 
 
 class JointPlot(Visual):  # pragma: no cover
     """Draw a plot of two variables with bivariate and univariate graphs."""
 
-    def __init__(self) -> None:
-        super().__init__()
-
     def __call__(
         self,
         data: pd.DataFrame,
         x: str,
         y: str = None,
         hue: str = None,
         ax: plt.Axes = None,
@@ -228,16 +213,14 @@
             palette (str): A string indicating one of the supported palettes. See docstring for
                 Palette class in config module. Defaults to 'winter_blue'.
             args and kwargs passed to the underlying seaborn histplot method.
                 See https://seaborn.pydata.org/generated/seaborn.histplot.html for a
                 complete list of parameters.
         """
 
-        style = self.get_set_styling(style=style, palette=palette)
-
         g = sns.jointplot(
             data=data,
             x=x,
             y=y,
             hue=hue,
             ax=ax,
             *args,
```

### Comparing `edation-0.0.5/edation/visual/config.py` & `edation-0.0.6/edation/visual/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 # Filename   : /edation/visual/config.py                                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Wednesday May 24th 2023 04:11:27 pm                                                 #
-# Modified   : Thursday July 27th 2023 11:26:02 am                                                 #
+# Modified   : Thursday July 27th 2023 03:36:09 pm                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 from __future__ import annotations
 from abc import ABC
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import List
-import logging
 
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 from edation import IMMUTABLE_TYPES, SEQUENCE_TYPES
 
 # ------------------------------------------------------------------------------------------------ #
@@ -101,14 +100,15 @@
     ),
     "blue_orange": sns.color_palette(
         [Colors.russian_violet, Colors.dark_cornflower_blue, Colors.meat_brown, Colors.peach],
         as_cmap=True,
     ),
 }
 
+
 # ------------------------------------------------------------------------------------------------ #
 #                                            CANVAS                                                #
 # ------------------------------------------------------------------------------------------------ #
 
 
 @dataclass
 class Canvas(PlotConfig):
@@ -120,62 +120,29 @@
     ncols: int = 1
     saturation: float = 0.5
     fontsize: int = 10
     fontsize_title: int = 10
     fig: plt.figure = None
     ax: plt.axes = None
     axs: List = field(default_factory=lambda: [plt.axes])
-    colors: Colors = Colors()
-
-    # def __post_init__(self) -> None:
-    #     width = int(self.figsize[0] / self.nrows)
-    #     height = int(self.figsize[1] / self.ncols)
-    #     figsize = []
-    #     figsize.append(width * self.ncols)
-    #     figsize.append(height * self.nrows)
-    #     self.fig, self.axs = plt.subplots(nrows=self.nrows, ncols=self.ncols, figsize=figsize)
+    palette: str = "Blues_r"
 
     def __post_init__(self) -> None:
         if self.nrows > 1 or self.ncols > 1:
             figsize = []
             figsize.append(self.figsize[0] * self.ncols)
             figsize.append(self.figsize[1] * self.nrows)
             self.fig, self.axs = plt.subplots(nrows=self.nrows, ncols=self.ncols, figsize=figsize)
         else:
             self.fig, self.ax = plt.subplots(
                 nrows=self.nrows, ncols=self.ncols, figsize=self.figsize
             )
 
 
 # ------------------------------------------------------------------------------------------------ #
-#                                            STYLE                                                 #
-# ------------------------------------------------------------------------------------------------ #
-@dataclass
-class Styling(PlotConfig):
-    """Style configuration"""
-
-    style: str = "whitegrid"
-    saturation: float = 1
-    fontsize: int = 8
-    title_fontsize: int = 10
-    palette: str = "blues_r"
-
-    def __post_init__(self) -> None:
-        """Sets the palette."""
-
-        try:
-            sns.set_palette(palette=PALETTES[self.palette])
-            return PALETTES[self.palette]
-        except Exception as e:
-            msg = f"{self.palette} is not a supported palette name"
-            logging.error(msg)
-            raise e
-
-
-# ------------------------------------------------------------------------------------------------ #
 #                                            LEGEND                                                #
 # ------------------------------------------------------------------------------------------------ #
 @dataclass
 class LegendConfig(PlotConfig):
     loc: str = "best"
     ncols: int = 1
     fontsize: int = 8
```

### Comparing `edation-0.0.5/edation/visual/distribution.py` & `edation-0.0.6/edation/visual/distribution.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,38 +7,36 @@
 # Filename   : /edation/visual/distribution.py                                                     #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : Enter URL in Workspace Settings                                                     #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Sunday June 18th 2023 01:41:15 am                                                   #
-# Modified   : Thursday July 27th 2023 10:26:55 am                                                 #
+# Modified   : Thursday July 27th 2023 04:12:10 pm                                                 #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 """Visualizations Revealing the Distribution of Data"""
 import pandas as pd
 
 import seaborn as sns
 import matplotlib.pyplot as plt
 
 from .base import Visual
+from .config import Canvas
 
 # ------------------------------------------------------------------------------------------------ #
 #                                       HISTOGRAM                                                  #
 # ------------------------------------------------------------------------------------------------ #
 
 
 class Histogram(Visual):  # pragma: no cover
     """Plot univariate or bivariate histograms to show distributions of datasets."""
 
-    def __init__(self) -> None:
-        super().__init__()
-
     def __call__(
         self,
         data: pd.DataFrame,
         x: str,
         y: str = None,
         hue: str = None,
         kde: bool = True,
@@ -61,44 +59,39 @@
             style (str): A string representing a seaborn style. Optional. Defaults to 'whitegrid'
             palette (str): A string indicating one of the supported palettes. See docstring for
                 Palette class in config module. Defaults to 'winter_blue'.
             args and kwargs passed to the underlying seaborn histplot method.
                 See https://seaborn.pydata.org/generated/seaborn.histplot.html for a
                 complete list of parameters.
         """
-
-        ax = self.get_or_create_ax(ax)
-        style = self.get_set_styling(style=style, palette=palette)
+        ax = ax or Canvas().ax
 
         ax = sns.histplot(
             data=data,
             x=x,
             y=y,
             hue=hue,
             kde=kde,
             ax=ax,
             legend=True,
-            pmax=style.saturation,
             *args,
             **kwargs,
         )
         if title:
             ax.set_title(title)
 
+
 # ------------------------------------------------------------------------------------------------ #
 #                                       KDE PLOT                                                   #
 # ------------------------------------------------------------------------------------------------ #
 
 
 class KDEPlot(Visual):  # pragma: no cover
     """Plot univariate or bivariate histograms to show distributions of datasets."""
 
-    def __init__(self) -> None:
-        super().__init__()
-
     def __call__(
         self,
         data: pd.DataFrame,
         x: str,
         y: str = None,
         hue: str = None,
         ax: plt.Axes = None,
@@ -122,17 +115,15 @@
             style (str): A string representing a seaborn style. Optional. Defaults to 'whitegrid'
             palette (str): A string indicating one of the supported palettes. See docstring for
                 Palette class in config module. Defaults to 'winter_blue'.
             args and kwargs passed to the underlying seaborn histplot method.
                 See https://seaborn.pydata.org/generated/seaborn.histplot.html for a
                 complete list of parameters.
         """
-
-        ax = self.get_or_create_ax(ax)
-        style = self.get_set_styling(style=style, palette=palette)
+        ax = ax or Canvas().ax
 
         ax = sns.kdeplot(
             data=data,
             x=x,
             y=y,
             hue=hue,
             legend=legend,
@@ -148,17 +139,14 @@
 #                                        BOX PLOT                                                  #
 # ------------------------------------------------------------------------------------------------ #
 
 
 class BoxPlot(Visual):  # pragma: no cover
     """Draw a box plot to show distributions with respect to categories or groups."""
 
-    def __init__(self) -> None:
-        super().__init__()
-
     def __call__(
         self,
         data: pd.DataFrame,
         x: str,
         y: str = None,
         ax: plt.Axes = None,
         title: str = None,
@@ -178,16 +166,15 @@
             palette (str): A string indicating one of the supported palettes. See docstring for
                 Palette class in config module. Defaults to 'winter_blue'.
             args and kwargs passed to the underlying seaborn histplot method.
                 See https://seaborn.pydata.org/generated/seaborn.histplot.html for a
                 complete list of parameters.
         """
 
-        ax = self.get_or_create_ax(ax)
-        style = self.get_set_styling(style=style, palette=palette)
+        ax = ax or Canvas().ax
 
         ax = sns.boxplot(
             data=data,
             x=x,
             y=y,
             ax=ax,
             *args,
@@ -201,17 +188,14 @@
 #                                     VIOLIN PLOT                                                  #
 # ------------------------------------------------------------------------------------------------ #
 
 
 class ViolinPlot(Visual):  # pragma: no cover
     """Draw a combination of boxplot and kernel density estimate."""
 
-    def __init__(self) -> None:
-        super().__init__()
-
     def __call__(
         self,
         data: pd.DataFrame,
         x: str,
         y: str = None,
         hue: str = None,
         ax: plt.Axes = None,
@@ -232,17 +216,15 @@
             style (str): A string representing a seaborn style. Optional. Defaults to 'whitegrid'
             palette (str): A string indicating one of the supported palettes. See docstring for
                 Palette class in config module. Defaults to 'winter_blue'.
             args and kwargs passed to the underlying seaborn histplot method.
                 See https://seaborn.pydata.org/generated/seaborn.histplot.html for a
                 complete list of parameters.
         """
-
-        ax = self.get_or_create_ax(ax)
-        style = self.get_set_styling(style=style, palette=palette)
+        ax = ax or Canvas().ax
 
         ax = sns.violinplot(
             data=data,
             x=x,
             y=y,
             hue=hue,
             ax=ax,
@@ -257,17 +239,14 @@
 #                           EMPIRICAL CUMULATIVE DISTRIBUTION PLOT                                 #
 # ------------------------------------------------------------------------------------------------ #
 
 
 class ECDFPlot(Visual):  # pragma: no cover
     """Draw a combination of boxplot and kernel density estimate."""
 
-    def __init__(self) -> None:
-        super().__init__()
-
     def __call__(
         self,
         data: pd.DataFrame,
         x: str,
         y: str = None,
         hue: str = None,
         ax: plt.Axes = None,
@@ -289,16 +268,15 @@
             palette (str): A string indicating one of the supported palettes. See docstring for
                 Palette class in config module. Defaults to 'winter_blue'.
             args and kwargs passed to the underlying seaborn histplot method.
                 See https://seaborn.pydata.org/generated/seaborn.histplot.html for a
                 complete list of parameters.
         """
 
-        ax = self.get_or_create_ax(ax)
-        style = self.get_set_styling(style=style, palette=palette)
+        ax = ax or Canvas().ax
 
         ax = sns.ecdfplot(
             data=data,
             x=x,
             y=y,
             hue=hue,
             ax=ax,
```

### Comparing `edation-0.0.5/pyproject.toml` & `edation-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edation"
-version = "0.0.5"
+version = "0.0.6"
 description = "Exploratory Data Analysis Framework"
 authors = [
     "John James <john.james.ai.studio@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `edation-0.0.5/setup.py` & `edation-0.0.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,26 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['edation',
- 'edation.adapter',
- 'edation.adapter.repo',
- 'edation.adapter.stats',
- 'edation.adapter.visual',
- 'edation.application',
- 'edation.application.ports.driven',
- 'edation.application.ports.driver',
- 'edation.application.visual',
- 'edation.domain',
  'edation.service',
  'edation.stats',
  'edation.stats.centrality',
  'edation.stats.correlation',
  'edation.stats.goodness_of_fit',
  'edation.stats.independence',
  'edation.visual']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'edation',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': 'Exploratory Data Analysis Framework',
     'long_description': "# EDAtion - An Exploratory Data Analysis Framework\n\n[![PyPI](https://img.shields.io/pypi/v/edation?style=flat-square)](https://pypi.python.org/pypi/edation/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edation?style=flat-square)](https://pypi.python.org/pypi/edation/)\n[![PyPI - License](https://img.shields.io/pypi/l/edation?style=flat-square)](https://pypi.python.org/pypi/edation/)\n\n---\n\n**Documentation**: [https://john-james-ai.github.io/edation](https://john-james-ai.github.io/edation)\n\n**Source Code**: [https://github.com/john-james-ai/edation](https://github.com/john-james-ai/edation)\n\n**PyPI**: [https://pypi.org/project/edation/](https://pypi.org/project/edation/)\n\n---\n\nExploratory Data Analysis Framework\n\n## Installation\n\n```sh\npip install edation\n```\n\n## Development\n\n* Clone this repository\n* Requirements:\n  * [Poetry](https://python-poetry.org/)\n  * Python 3.7+\n* Create a virtual environment and install the dependencies\n\n```sh\npoetry install\n```\n\n* Activate the virtual environment\n\n```sh\npoetry shell\n```\n\n### Testing\n\n```sh\npytest\n```\n\n### Documentation\n\nThe documentation is automatically generated from the content of the [docs directory](./docs) and from the docstrings\n of the public signatures of the source code. The documentation is updated and published as a [Github project page\n ](https://pages.github.com/) automatically as part each release.\n\n### Releasing\n\nTrigger the [Draft release workflow](https://github.com/john-james-ai/edation/actions/workflows/draft_release.yml)\n(press _Run workflow_). This will update the changelog & version and create a GitHub release which is in _Draft_ state.\n\nFind the draft release from the\n[GitHub releases](https://github.com/john-james-ai/edation/releases) and publish it. When\n a release is published, it'll trigger [release](https://github.com/john-james-ai/edation/blob/master/.github/workflows/release.yml) workflow which creates PyPI\n release and deploys updated documentation.\n\n### Pre-commit\n\nPre-commit hooks run all the auto-formatters (e.g. `black`, `isort`), linters (e.g. `mypy`, `flake8`), and other quality\n checks to make sure the changeset is in good shape before a commit/push happens.\n\nYou can install the hooks with (runs for each commit):\n\n```sh\npre-commit install\n```\n\nOr if you want them to run only for each push:\n\n```sh\npre-commit install -t pre-push\n```\n\nOr if you want e.g. want to run all checks manually for all files:\n\n```sh\npre-commit run --all-files\n```\n\n---\n",
     'author': 'John James',
     'author_email': 'john.james.ai.studio@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://john-james-ai.github.io/edation',
```

### Comparing `edation-0.0.5/PKG-INFO` & `edation-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edation
-Version: 0.0.5
+Version: 0.0.6
 Summary: Exploratory Data Analysis Framework
 Home-page: https://john-james-ai.github.io/edation
 License: MIT
 Author: John James
 Author-email: john.james.ai.studio@gmail.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: Development Status :: 4 - Beta
```


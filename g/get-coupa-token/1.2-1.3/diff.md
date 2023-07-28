# Comparing `tmp/get_coupa_token-1.2.tar.gz` & `tmp/get_coupa_token-1.3.tar.gz`

## Comparing `get_coupa_token-1.2.tar` & `get_coupa_token-1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 get_coupa_token-1.2/__init__.py
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 get_coupa_token-1.2/get_coupa_token.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 get_coupa_token-1.2/LICENSE
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 get_coupa_token-1.2/README.md
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 get_coupa_token-1.2/pyproject.toml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 get_coupa_token-1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 get_coupa_token-1.3/__init__.py
+-rw-r--r--   0        0        0     5224 2020-02-02 00:00:00.000000 get_coupa_token-1.3/get_coupa_token.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 get_coupa_token-1.3/LICENSE
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 get_coupa_token-1.3/README.md
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 get_coupa_token-1.3/pyproject.toml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 get_coupa_token-1.3/PKG-INFO
```

### Comparing `get_coupa_token-1.2/get_coupa_token.py` & `get_coupa_token-1.3/get_coupa_token.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 import api_secrets as api_secrets
 import requests
 import time
 import json
 from pathlib import Path
 import datetime
 from selenium import webdriver
+from selenium.webdriver.chrome.service import Service as ChromeService
 from webdriver_manager.chrome import ChromeDriverManager
+from selenium.webdriver.chrome.service import Service as ChromiumService
+from webdriver_manager.chrome import ChromeDriverManager
+from webdriver_manager.core.utils import ChromeType
+from webdriver_manager.firefox import GeckoDriverManager
 from selenium.webdriver.support import ui
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 from selenium.common.exceptions import TimeoutException
 from selenium.common.exceptions import ElementClickInterceptedException
 from selenium.webdriver.support.ui import WebDriverWait # available since 2.4.0
@@ -19,15 +24,26 @@
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.by import By
 
 
   
 def initiate_driver():
-    driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()))
+    try:
+        driver = webdriver.Chrome(service=ChromeService(ChromeDriverManager().install()))
+    except ValueError as e:
+        print(f"Caught ValueError: {e}")
+        print("Reverting to chromium")
+        
+        try:
+            driver = webdriver.Chrome(ChromeDriverManager(chrome_type=ChromeType.CHROMIUM).install())
+        except ValueError as e:
+            print(f"Caught ValueError: {e}")
+            print("Reverting to firefox")
+            driver = webdriver.Firefox(service=FirefoxService(GeckoDriverManager().install()))
     return driver
 
 def get_token(system, grant_type, token_user, client_id, user, scope):
     def refresh_token():
         
         secret = api_secrets.get_secret(system, user)
         if not secret:
```

### Comparing `get_coupa_token-1.2/LICENSE` & `get_coupa_token-1.3/LICENSE`

 * *Files identical despite different names*


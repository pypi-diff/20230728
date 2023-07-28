# Comparing `tmp/st-login-form-0.2.1.tar.gz` & `tmp/st-login-form-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-login-form-0.2.1.tar", last modified: Fri Jul 28 09:45:48 2023, max compression
+gzip compressed data, was "st-login-form-0.3.0.tar", last modified: Fri Jul 21 15:56:51 2023, max compression
```

## Comparing `st-login-form-0.2.1.tar` & `st-login-form-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:45:48.337193 st-login-form-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-28 09:45:36.000000 st-login-form-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-28 09:45:36.000000 st-login-form-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-28 09:45:48.333193 st-login-form-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-28 09:45:36.000000 st-login-form-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:45:48.333193 st-login-form-0.2.1/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    24479 2023-07-28 09:45:36.000000 st-login-form-0.2.1/assets/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 09:45:48.337193 st-login-form-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-28 09:45:36.000000 st-login-form-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:45:48.333193 st-login-form-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:45:48.333193 st-login-form-0.2.1/src/st_login_form/
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-07-28 09:45:36.000000 st-login-form-0.2.1/src/st_login_form/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 09:45:48.333193 st-login-form-0.2.1/src/st_login_form.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-28 09:45:48.000000 st-login-form-0.2.1/src/st_login_form.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-28 09:45:48.000000 st-login-form-0.2.1/src/st_login_form.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 09:45:48.000000 st-login-form-0.2.1/src/st_login_form.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 09:45:48.000000 st-login-form-0.2.1/src/st_login_form.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 09:45:48.000000 st-login-form-0.2.1/src/st_login_form.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:56:51.754086 st-login-form-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-21 15:56:42.000000 st-login-form-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 15:56:42.000000 st-login-form-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-21 15:56:51.754086 st-login-form-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-21 15:56:42.000000 st-login-form-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:56:51.754086 st-login-form-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-21 15:56:42.000000 st-login-form-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:56:51.750085 st-login-form-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:56:51.750085 st-login-form-0.3.0/src/st_login_form/
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-21 15:56:42.000000 st-login-form-0.3.0/src/st_login_form/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:56:51.754086 st-login-form-0.3.0/src/st_login_form.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-21 15:56:51.000000 st-login-form-0.3.0/src/st_login_form.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-21 15:56:51.000000 st-login-form-0.3.0/src/st_login_form.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:56:51.000000 st-login-form-0.3.0/src/st_login_form.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-21 15:56:51.000000 st-login-form-0.3.0/src/st_login_form.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-21 15:56:51.000000 st-login-form-0.3.0/src/st_login_form.egg-info/top_level.txt
```

### Comparing `st-login-form-0.2.1/LICENSE` & `st-login-form-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `st-login-form-0.2.1/PKG-INFO` & `st-login-form-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: st-login-form
-Version: 0.2.1
+Version: 0.3.0
 Summary: A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.
 Home-page: https://github.com/SiddhantSadangi/st_login_form
 Author: Siddhant Sadangi
 Author-email: siddhant.sadangi@gmail.com
 Project-URL: Documentation, https://github.com/SiddhantSadangi/st_login_form/blob/main/README.md
-Project-URL: Funding, https://www.buymeacoffee.com/siddhantsadangi
+Project-URL: Support, https://www.buymeacoffee.com/siddhantsadangi
 Keywords: streamlit,login
 Classifier: Environment :: Plugins
-Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.8
@@ -28,17 +27,17 @@
 ![Form screenshot](assets/screenshot.png)
 
 The login form collapses after login to free screen-space.
 
 ## :computer: Demo app
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://st-lgn-form.streamlit.app/)
 
-## :construction: Installation
+## :construction: Installation 
 
-1. Install `st-login-form`
+1. Install `st-login-form` 
 ```sh
 pip install st-login-form
 ```
 2. Create a Supabase project as mentioned [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/supabase#sign-in-to-supabase-and-create-a-project)
 3. Create a table to store the usernames and passwords. The table name and column names can be as per your choice.
 ```sql
 CREATE TABLE users (
@@ -78,15 +77,15 @@
 `login_form()` sets `session_state["authenticated"]` to `True` if the login is successful, `session_state["username"]` to the `username` or new or existing user, and to `None` for guest login.
 
 Returns the initialized `supabase.Client` instance to let you interact with the databse downstream in the script.
 
 ```python
 import streamlit as st
 
-from st_login_form import login_form
+from streamlit_login import login_form
 
 client = login_form()
 
 if st.session_state["authenticated"]:
     if st.session_state["username"]:
         st.success(f"Welcome {st.session_state['username']}")
     else:
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: st-login-form Version: 0.2.1 Summary: A streamlit
+Metadata-Version: 2.1 Name: st-login-form Version: 0.3.0 Summary: A streamlit
 component that creates a user login form connected to a Supabase DB. It lets
 users create a new username and password, login to an existing account, or
 login as an anonymous guest. Home-page: https://github.com/SiddhantSadangi/
 st_login_form Author: Siddhant Sadangi Author-email: siddhant.sadangi@gmail.com
 Project-URL: Documentation, https://github.com/SiddhantSadangi/st_login_form/
-blob/main/README.md Project-URL: Funding, https://www.buymeacoffee.com/
+blob/main/README.md Project-URL: Support, https://www.buymeacoffee.com/
 siddhantsadangi Keywords: streamlit,login Classifier: Environment :: Plugins
-Classifier: Environment :: Web Environment Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: GNU General Public License v3
-(GPLv3) Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python Classifier: Topic :: Software Development :: Libraries ::
-Python Modules Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE # :lock: st-login-form [![Downloads](https://static.pepy.tech/
-personalized-badge/st-login-
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: GNU General Public License v3 (GPLv3) Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Topic ::
+Software Development :: User Interfaces Requires-Python: >=3.8 Description-
+Content-Type: text/markdown License-File: LICENSE # :lock: st-login-form [!
+[Downloads](https://static.pepy.tech/personalized-badge/st-login-
 form?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=Downloads)]
 (https://pepy.tech/project/st-login-form) A streamlit component that creates a
 user login form connected to a Supabase DB. It lets users create a new username
 and password, login to an existing account, or login as an anonymous guest. !
 [Form screenshot](assets/screenshot.png) The login form collapses after login
 to free screen-space. ## :computer: Demo app [![Open in Streamlit](https://
 static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://st-lgn-
@@ -34,15 +33,15 @@
 > 1 ) ) ) tablespace pg_default; ``` 4. Follow the rest of the steps from
 [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/
 supabase#copy-your-app-secrets-to-the-cloud) to connect your Streamlit app to
 Supabase ## :pen: Usage `login_form()` sets `session_state["authenticated"]` to
 `True` if the login is successful, `session_state["username"]` to the
 `username` or new or existing user, and to `None` for guest login. Returns the
 initialized `supabase.Client` instance to let you interact with the databse
-downstream in the script. ```python import streamlit as st from st_login_form
+downstream in the script. ```python import streamlit as st from streamlit_login
 import login_form client = login_form() if st.session_state["authenticated"]:
 if st.session_state["username"]: st.success(f"Welcome {st.session_state
 ['username']}") else: st.success("Welcome guest") else: st.error("Not
 authenticated") ``` [![See demo in Streamlit](https://static.streamlit.io/
 badges/streamlit_badge_black_white.svg)](https://st-lgn-form.streamlit.app/) ##
 ð¤ Want to support my work?
                                [Buy_Me_A_Coffee]
```

### Comparing `st-login-form-0.2.1/README.md` & `st-login-form-0.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 ![Form screenshot](assets/screenshot.png)
 
 The login form collapses after login to free screen-space.
 
 ## :computer: Demo app
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://st-lgn-form.streamlit.app/)
 
-## :construction: Installation
+## :construction: Installation 
 
-1. Install `st-login-form`
+1. Install `st-login-form` 
 ```sh
 pip install st-login-form
 ```
 2. Create a Supabase project as mentioned [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/supabase#sign-in-to-supabase-and-create-a-project)
 3. Create a table to store the usernames and passwords. The table name and column names can be as per your choice.
 ```sql
 CREATE TABLE users (
@@ -56,15 +56,15 @@
 `login_form()` sets `session_state["authenticated"]` to `True` if the login is successful, `session_state["username"]` to the `username` or new or existing user, and to `None` for guest login.
 
 Returns the initialized `supabase.Client` instance to let you interact with the databse downstream in the script.
 
 ```python
 import streamlit as st
 
-from st_login_form import login_form
+from streamlit_login import login_form
 
 client = login_form()
 
 if st.session_state["authenticated"]:
     if st.session_state["username"]:
         st.success(f"Welcome {st.session_state['username']}")
     else:
```

#### html2text {}

```diff
@@ -20,15 +20,15 @@
 > 1 ) ) ) tablespace pg_default; ``` 4. Follow the rest of the steps from
 [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/
 supabase#copy-your-app-secrets-to-the-cloud) to connect your Streamlit app to
 Supabase ## :pen: Usage `login_form()` sets `session_state["authenticated"]` to
 `True` if the login is successful, `session_state["username"]` to the
 `username` or new or existing user, and to `None` for guest login. Returns the
 initialized `supabase.Client` instance to let you interact with the databse
-downstream in the script. ```python import streamlit as st from st_login_form
+downstream in the script. ```python import streamlit as st from streamlit_login
 import login_form client = login_form() if st.session_state["authenticated"]:
 if st.session_state["username"]: st.success(f"Welcome {st.session_state
 ['username']}") else: st.success("Welcome guest") else: st.error("Not
 authenticated") ``` [![See demo in Streamlit](https://static.streamlit.io/
 badges/streamlit_badge_black_white.svg)](https://st-lgn-form.streamlit.app/) ##
 ð¤ Want to support my work?
                                [Buy_Me_A_Coffee]
```

### Comparing `st-login-form-0.2.1/src/st_login_form/__init__.py` & `st-login-form-0.3.0/src/st_login_form/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import streamlit as st
-from supabase import Client, create_client
-
-__version__ = "0.2.1"
+from supabase import create_client, Client
 
 
 @st.cache_resource
 def init_connection() -> Client:
     return create_client(st.secrets["SUPABASE_URL"], st.secrets["SUPABASE_KEY"])
 
 
@@ -26,15 +24,15 @@
     allow_guest: bool = True,
     guest_title: str = "Guest login :ninja: ",
     create_username_label: str = "Create a unique username",
     create_username_placeholder: str = None,
     create_username_help: str = None,
     create_password_label: str = "Create a password",
     create_password_placeholder: str = None,
-    create_password_help: str = "⚠️ Password will be stored as plain text. Do not reuse from other websites. Password cannot be recovered.",
+    create_password_help: str = "⚠️ Remember your password. You won't be able to recover it if forgotten.",
     create_submit_label: str = "Create account",
     create_success_message: str = "Account created :tada:",
     login_username_label: str = "Enter your unique username",
     login_username_placeholder: str = None,
     login_username_help: str = None,
     login_password_label: str = "Enter your password",
     login_password_placeholder: str = None,
@@ -103,15 +101,17 @@
                     label=create_submit_label,
                     type="primary",
                     disabled=st.session_state["authenticated"],
                 ):
                     try:
                         data, _ = (
                             client.table(user_tablename)
-                            .insert({username_col: username, password_col: password})
+                            .insert(
+                                {username_col: username, password_col: hash(password)}
+                            )
                             .execute()
                         )
                     except Exception as e:
                         st.error(e.message)
                     else:
                         login_success(create_success_message, username)
 
@@ -138,15 +138,15 @@
                     disabled=st.session_state["authenticated"],
                     type="primary",
                 ):
                     data, _ = (
                         client.table(user_tablename)
                         .select(f"{username_col}, {password_col}")
                         .eq(username_col, username)
-                        .eq(password_col, password)
+                        .eq(password_col, hash(password))
                         .execute()
                     )
 
                     if len(data[-1]) > 0:
                         login_success(login_success_message, username)
                     else:
                         st.error(login_error_message)
@@ -163,14 +163,14 @@
 
         return client
 
 
 def main() -> None:
     login_form(
         create_username_placeholder="Username will be visible in the global leaderboard.",
-        create_password_placeholder="⚠️ Password will be stored as plain text. You won't be able to recover it if you forget.",
+        create_password_placeholder="⚠️ Remember your password. You won't be able to recover it if you forget.",
         guest_submit_label="Play as a guest ⚠️ Scores won't be saved",
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `st-login-form-0.2.1/src/st_login_form.egg-info/PKG-INFO` & `st-login-form-0.3.0/src/st_login_form.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: st-login-form
-Version: 0.2.1
+Version: 0.3.0
 Summary: A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.
 Home-page: https://github.com/SiddhantSadangi/st_login_form
 Author: Siddhant Sadangi
 Author-email: siddhant.sadangi@gmail.com
 Project-URL: Documentation, https://github.com/SiddhantSadangi/st_login_form/blob/main/README.md
-Project-URL: Funding, https://www.buymeacoffee.com/siddhantsadangi
+Project-URL: Support, https://www.buymeacoffee.com/siddhantsadangi
 Keywords: streamlit,login
 Classifier: Environment :: Plugins
-Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.8
@@ -28,17 +27,17 @@
 ![Form screenshot](assets/screenshot.png)
 
 The login form collapses after login to free screen-space.
 
 ## :computer: Demo app
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://st-lgn-form.streamlit.app/)
 
-## :construction: Installation
+## :construction: Installation 
 
-1. Install `st-login-form`
+1. Install `st-login-form` 
 ```sh
 pip install st-login-form
 ```
 2. Create a Supabase project as mentioned [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/supabase#sign-in-to-supabase-and-create-a-project)
 3. Create a table to store the usernames and passwords. The table name and column names can be as per your choice.
 ```sql
 CREATE TABLE users (
@@ -78,15 +77,15 @@
 `login_form()` sets `session_state["authenticated"]` to `True` if the login is successful, `session_state["username"]` to the `username` or new or existing user, and to `None` for guest login.
 
 Returns the initialized `supabase.Client` instance to let you interact with the databse downstream in the script.
 
 ```python
 import streamlit as st
 
-from st_login_form import login_form
+from streamlit_login import login_form
 
 client = login_form()
 
 if st.session_state["authenticated"]:
     if st.session_state["username"]:
         st.success(f"Welcome {st.session_state['username']}")
     else:
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: st-login-form Version: 0.2.1 Summary: A streamlit
+Metadata-Version: 2.1 Name: st-login-form Version: 0.3.0 Summary: A streamlit
 component that creates a user login form connected to a Supabase DB. It lets
 users create a new username and password, login to an existing account, or
 login as an anonymous guest. Home-page: https://github.com/SiddhantSadangi/
 st_login_form Author: Siddhant Sadangi Author-email: siddhant.sadangi@gmail.com
 Project-URL: Documentation, https://github.com/SiddhantSadangi/st_login_form/
-blob/main/README.md Project-URL: Funding, https://www.buymeacoffee.com/
+blob/main/README.md Project-URL: Support, https://www.buymeacoffee.com/
 siddhantsadangi Keywords: streamlit,login Classifier: Environment :: Plugins
-Classifier: Environment :: Web Environment Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: GNU General Public License v3
-(GPLv3) Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python Classifier: Topic :: Software Development :: Libraries ::
-Python Modules Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE # :lock: st-login-form [![Downloads](https://static.pepy.tech/
-personalized-badge/st-login-
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: GNU General Public License v3 (GPLv3) Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Topic ::
+Software Development :: User Interfaces Requires-Python: >=3.8 Description-
+Content-Type: text/markdown License-File: LICENSE # :lock: st-login-form [!
+[Downloads](https://static.pepy.tech/personalized-badge/st-login-
 form?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=Downloads)]
 (https://pepy.tech/project/st-login-form) A streamlit component that creates a
 user login form connected to a Supabase DB. It lets users create a new username
 and password, login to an existing account, or login as an anonymous guest. !
 [Form screenshot](assets/screenshot.png) The login form collapses after login
 to free screen-space. ## :computer: Demo app [![Open in Streamlit](https://
 static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://st-lgn-
@@ -34,15 +33,15 @@
 > 1 ) ) ) tablespace pg_default; ``` 4. Follow the rest of the steps from
 [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/
 supabase#copy-your-app-secrets-to-the-cloud) to connect your Streamlit app to
 Supabase ## :pen: Usage `login_form()` sets `session_state["authenticated"]` to
 `True` if the login is successful, `session_state["username"]` to the
 `username` or new or existing user, and to `None` for guest login. Returns the
 initialized `supabase.Client` instance to let you interact with the databse
-downstream in the script. ```python import streamlit as st from st_login_form
+downstream in the script. ```python import streamlit as st from streamlit_login
 import login_form client = login_form() if st.session_state["authenticated"]:
 if st.session_state["username"]: st.success(f"Welcome {st.session_state
 ['username']}") else: st.success("Welcome guest") else: st.error("Not
 authenticated") ``` [![See demo in Streamlit](https://static.streamlit.io/
 badges/streamlit_badge_black_white.svg)](https://st-lgn-form.streamlit.app/) ##
 ð¤ Want to support my work?
                                [Buy_Me_A_Coffee]
```


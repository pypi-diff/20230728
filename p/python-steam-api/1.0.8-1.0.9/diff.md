# Comparing `tmp/python-steam-api-1.0.8.tar.gz` & `tmp/python-steam-api-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-steam-api-1.0.8.tar", last modified: Sun Jan 22 16:56:11 2023, max compression
+gzip compressed data, was "python-steam-api-1.0.9.tar", last modified: Fri Jul 28 21:25:01 2023, max compression
```

## Comparing `python-steam-api-1.0.8.tar` & `python-steam-api-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-01-22 16:56:11.610751 python-steam-api-1.0.8/
--rw-rw-rw-   0        0        0     1101 2022-08-08 11:46:12.000000 python-steam-api-1.0.8/LICENCE
--rw-rw-rw-   0        0        0       48 2022-08-08 12:05:46.000000 python-steam-api-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0    32230 2023-01-22 16:56:11.610751 python-steam-api-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    31412 2022-12-30 15:22:32.000000 python-steam-api-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-22 16:56:11.595238 python-steam-api-1.0.8/python_steam_api.egg-info/
--rw-rw-rw-   0        0        0    32230 2023-01-22 16:56:11.000000 python-steam-api-1.0.8/python_steam_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-01-22 16:56:11.000000 python-steam-api-1.0.8/python_steam_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-22 16:56:11.000000 python-steam-api-1.0.8/python_steam_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-01-22 16:56:11.000000 python-steam-api-1.0.8/python_steam_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-01-22 16:56:11.000000 python-steam-api-1.0.8/python_steam_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       77 2023-01-22 16:56:11.615266 python-steam-api-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1184 2023-01-22 16:54:34.000000 python-steam-api-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-22 16:56:11.609751 python-steam-api-1.0.8/steam/
--rw-rw-rw-   0        0        0      127 2022-12-30 14:15:58.000000 python-steam-api-1.0.8/steam/__init__.py
--rw-rw-rw-   0        0        0     3228 2023-01-22 16:53:54.000000 python-steam-api-1.0.8/steam/apps.py
--rw-rw-rw-   0        0        0     1821 2023-01-22 16:40:27.000000 python-steam-api-1.0.8/steam/client.py
--rw-rw-rw-   0        0        0      188 2022-08-08 01:42:59.000000 python-steam-api-1.0.8/steam/constants.py
--rw-rw-rw-   0        0        0      479 2023-01-22 16:43:58.000000 python-steam-api-1.0.8/steam/steam.py
--rw-rw-rw-   0        0        0     5218 2022-08-14 23:05:26.000000 python-steam-api-1.0.8/steam/users.py
--rw-rw-rw-   0        0        0     2180 2023-01-22 16:39:39.000000 python-steam-api-1.0.8/steam/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-28 21:25:01.570465 python-steam-api-1.0.9/
+-rw-rw-rw-   0        0        0     1101 2022-08-08 11:46:12.000000 python-steam-api-1.0.9/LICENCE
+-rw-rw-rw-   0        0        0       48 2022-08-08 12:05:46.000000 python-steam-api-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    32230 2023-07-28 21:25:01.574475 python-steam-api-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    31412 2022-12-30 15:22:32.000000 python-steam-api-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 21:25:01.474542 python-steam-api-1.0.9/python_steam_api.egg-info/
+-rw-rw-rw-   0        0        0    32230 2023-07-28 21:25:01.000000 python-steam-api-1.0.9/python_steam_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-07-28 21:25:01.000000 python-steam-api-1.0.9/python_steam_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 21:25:01.000000 python-steam-api-1.0.9/python_steam_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-28 21:25:01.000000 python-steam-api-1.0.9/python_steam_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-28 21:25:01.000000 python-steam-api-1.0.9/python_steam_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       77 2023-07-28 21:25:01.574475 python-steam-api-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1184 2023-07-28 21:17:15.000000 python-steam-api-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 21:25:01.570465 python-steam-api-1.0.9/steam/
+-rw-rw-rw-   0        0        0      127 2022-12-30 14:15:58.000000 python-steam-api-1.0.9/steam/__init__.py
+-rw-rw-rw-   0        0        0     4381 2023-07-28 21:16:50.000000 python-steam-api-1.0.9/steam/apps.py
+-rw-rw-rw-   0        0        0     1821 2023-01-22 16:40:27.000000 python-steam-api-1.0.9/steam/client.py
+-rw-rw-rw-   0        0        0      188 2022-08-08 01:42:59.000000 python-steam-api-1.0.9/steam/constants.py
+-rw-rw-rw-   0        0        0      479 2023-01-22 16:43:58.000000 python-steam-api-1.0.9/steam/steam.py
+-rw-rw-rw-   0        0        0     5243 2023-07-28 21:16:50.000000 python-steam-api-1.0.9/steam/users.py
+-rw-rw-rw-   0        0        0     2180 2023-01-22 16:39:39.000000 python-steam-api-1.0.9/steam/utils.py
```

### Comparing `python-steam-api-1.0.8/LICENCE` & `python-steam-api-1.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `python-steam-api-1.0.8/PKG-INFO` & `python-steam-api-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-steam-api
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python Client wrapper for Steam API
 Home-page: https://github.com/deivit24/steam-python-sdk
 Author: David Salazar
 Author-email: david.asal@hotmail.com
 License: MIT
 Keywords: steam,steamapi,steam community,api
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-steam-api-1.0.8/README.md` & `python-steam-api-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `python-steam-api-1.0.8/python_steam_api.egg-info/PKG-INFO` & `python-steam-api-1.0.9/python_steam_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-steam-api
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python Client wrapper for Steam API
 Home-page: https://github.com/deivit24/steam-python-sdk
 Author: David Salazar
 Author-email: david.asal@hotmail.com
 License: MIT
 Keywords: steam,steamapi,steam community,api
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python-steam-api-1.0.8/setup.py` & `python-steam-api-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as fp:
     long_description = fp.read()
 
 setup(
     name="python-steam-api",
-    version="1.0.8",
+    version="1.0.9",
     description="Python Client wrapper for Steam API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=[
         "steam",
         "steamapi",
         "steam community",
```

### Comparing `python-steam-api-1.0.8/steam/client.py` & `python-steam-api-1.0.9/steam/client.py`

 * *Files identical despite different names*

### Comparing `python-steam-api-1.0.8/steam/users.py` & `python-steam-api-1.0.9/steam/users.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,58 +26,58 @@
         steam_id = search_response["steamid"]
         return self.get_user_details(steam_id)
 
     def get_user_details(self, steam_id: str, single=True) -> dict:
         """Gets user/player details by steam ID
 
         Args:
-            steam_id (str): Steam ID
-            single (bool, optional): Gets on player. Defaults to True. When false, steam_id can be a string of steamids and delimited by a ','
+            steam_id (str): Steam 64 ID
+            single (bool, optional): Gets one player. Defaults to True. When false, steam_id can be a string of steamids and delimited by a ','
 
         """
         user_response = self.__client.request(
             "get", "/ISteamUser/GetPlayerSummaries/v2/", params={"steamids": steam_id}
         )["response"]
         if single:
             return {"player": user_response["players"][0]}
         else:
             return {"players": user_response["players"]}
 
     def get_user_friends_list(self, steam_id: str) -> dict:
         """Gets friend list of a user
 
         Args:
-            steam_id (str): Steam ID
+            steam_id (str): Steam 64 ID
         """
         friends_list_response = self.__client.request(
             "get", "/ISteamUser/GetFriendList/v1/", params={"steamid": steam_id}
         )["friendslist"]
         transform_friends = self._transform_friends(friends_list_response)
         return {"friends": transform_friends}
 
     def get_user_recently_played_games(self, steam_id: str) -> dict:
         """Gets recently played games
 
         Args:
-            steam_id (str): Steam ID
+            steam_id (str): Steam 64 ID
         """
         response = self.__client.request(
             "get",
             "/IPlayerService/GetRecentlyPlayedGames/v1/",
             params={"steamid": steam_id},
         )["response"]
         return response
 
     def get_owned_games(
         self, steam_id: str, include_appinfo=True, includ_free_games=True
     ) -> dict:
         """Gets all owned games of a user by steam id
 
         Args:
-            steam_id (str): Steam ID
+            steam_id (str): Steam 64 ID
             include_appinfo (bool, optional): Includes app/game info. Defaults to True.
             includ_free_games (bool, optional): Includes free games. Defaults to True.
         """
         params = {
             "steamid": steam_id,
             "include_appinfo": include_appinfo,
             "include_played_free_games": includ_free_games,
@@ -89,55 +89,55 @@
         )["response"]
         return response
 
     def get_user_steam_level(self, steam_id: str) -> dict:
         """Gets user steam level
 
         Args:
-            steam_id (str): Steam ID
+            steam_id (str): Steam 64 ID
         """
         response = self.__client.request(
             "get",
             "/IPlayerService/GetSteamLevel/v1/",
             params={"steamid": steam_id},
         )["response"]
         return response
 
     def get_user_badges(self, steam_id: str) -> dict:
         """Gets user steam badges
 
         Args:
-            steam_id (str): Steam ID
+            steam_id (str): Steam 64 ID
         """
         response = self.__client.request(
             "get",
             "/IPlayerService/GetBadges/v1/",
             params={"steamid": steam_id},
         )["response"]
         return response
 
     def get_community_badge_progress(self, steam_id: str, badge_id: int) -> dict:
         """Gets user community badge progress
 
         Args:
-            steam_id (str): Steam ID
+            steam_id (str): Steam 64 ID
             badge_id (int): Badge ID
         """
         response = self.__client.request(
             "get",
             "/IPlayerService/GetCommunityBadgeProgress/v1",
             params={"steamid": steam_id, "badgeid": badge_id},
         )["response"]
         return response
 
     def get_account_public_info(self, steam_id: str) -> dict:
         """Gets account public info
 
         Args:
-            steam_id (str): Steam ID
+            steam_id (str): Steam 64 ID
         """
         response = self.__client.request(
             "get",
             "/IGameServersService/GetAccountPublicInfo/v1",
             params={"steamid": steam_id},
         )
         return response
```

### Comparing `python-steam-api-1.0.8/steam/utils.py` & `python-steam-api-1.0.9/steam/utils.py`

 * *Files identical despite different names*


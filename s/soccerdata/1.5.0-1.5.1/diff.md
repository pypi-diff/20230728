# Comparing `tmp/soccerdata-1.5.0.tar.gz` & `tmp/soccerdata-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soccerdata-1.5.0.tar", max compression
+gzip compressed data, was "soccerdata-1.5.1.tar", max compression
```

## Comparing `soccerdata-1.5.0.tar` & `soccerdata-1.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1384 2023-07-23 22:15:29.151558 soccerdata-1.5.0/LICENSE.rst
--rw-r--r--   0        0        0     3130 2023-07-23 22:15:29.151558 soccerdata-1.5.0/README.rst
--rw-r--r--   0        0        0     2328 2023-07-23 22:15:49.399722 soccerdata-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      457 2023-07-23 22:15:49.399722 soccerdata-1.5.0/soccerdata/__init__.py
--rw-r--r--   0        0        0    20702 2023-07-23 22:15:29.159558 soccerdata-1.5.0/soccerdata/_common.py
--rw-r--r--   0        0        0     5207 2023-07-23 22:15:29.159558 soccerdata-1.5.0/soccerdata/_config.py
--rw-r--r--   0        0        0     6382 2023-07-23 22:15:29.159558 soccerdata-1.5.0/soccerdata/clubelo.py
--rw-r--r--   0        0        0    12890 2023-07-23 22:15:29.159558 soccerdata-1.5.0/soccerdata/espn.py
--rw-r--r--   0        0        0    44941 2023-07-23 22:15:29.159558 soccerdata-1.5.0/soccerdata/fbref.py
--rw-r--r--   0        0        0     8536 2023-07-23 22:15:29.159558 soccerdata-1.5.0/soccerdata/fivethirtyeight.py
--rw-r--r--   0        0        0     4657 2023-07-23 22:15:29.159558 soccerdata-1.5.0/soccerdata/match_history.py
--rw-r--r--   0        0        0    16744 2023-07-23 22:15:29.163558 soccerdata-1.5.0/soccerdata/sofifa.py
--rw-r--r--   0        0        0    32695 2023-07-23 22:15:29.163558 soccerdata-1.5.0/soccerdata/whoscored.py
--rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 soccerdata-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1384 2023-07-28 10:54:36.163195 soccerdata-1.5.1/LICENSE.rst
+-rw-r--r--   0        0        0     3130 2023-07-28 10:54:36.163195 soccerdata-1.5.1/README.rst
+-rw-r--r--   0        0        0     2308 2023-07-28 10:54:53.703246 soccerdata-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      457 2023-07-28 10:54:53.703246 soccerdata-1.5.1/soccerdata/__init__.py
+-rw-r--r--   0        0        0    20702 2023-07-28 10:54:36.171195 soccerdata-1.5.1/soccerdata/_common.py
+-rw-r--r--   0        0        0     5207 2023-07-28 10:54:36.171195 soccerdata-1.5.1/soccerdata/_config.py
+-rw-r--r--   0        0        0     6382 2023-07-28 10:54:36.171195 soccerdata-1.5.1/soccerdata/clubelo.py
+-rw-r--r--   0        0        0    12890 2023-07-28 10:54:36.175195 soccerdata-1.5.1/soccerdata/espn.py
+-rw-r--r--   0        0        0    46359 2023-07-28 10:54:36.175195 soccerdata-1.5.1/soccerdata/fbref.py
+-rw-r--r--   0        0        0     8536 2023-07-28 10:54:36.175195 soccerdata-1.5.1/soccerdata/fivethirtyeight.py
+-rw-r--r--   0        0        0     4657 2023-07-28 10:54:36.175195 soccerdata-1.5.1/soccerdata/match_history.py
+-rw-r--r--   0        0        0    16744 2023-07-28 10:54:36.175195 soccerdata-1.5.1/soccerdata/sofifa.py
+-rw-r--r--   0        0        0    32695 2023-07-28 10:54:36.175195 soccerdata-1.5.1/soccerdata/whoscored.py
+-rw-r--r--   0        0        0     4339 1970-01-01 00:00:00.000000 soccerdata-1.5.1/PKG-INFO
```

### Comparing `soccerdata-1.5.0/LICENSE.rst` & `soccerdata-1.5.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `soccerdata-1.5.0/README.rst` & `soccerdata-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `soccerdata-1.5.0/pyproject.toml` & `soccerdata-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "soccerdata"
-version = "1.5.0"
+version = "1.5.1"
 description = "A collection of wrappers over soccer data from various websites / APIs."
 authors = ["Pieter Robberechts <pieter.robberechts@kuleuven.be>"]
 license = "Apache-2.0"
 readme = 'README.rst'
 homepage = "https://github.com/probberechts/soccerdata"
 repository = "https://github.com/probberechts/soccerdata"
 keywords = ["soccer", "football", "soccer data", "web scraping", "soccer analytics"]
@@ -16,20 +16,19 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 pandas = "^2.0.0"
 requests = "^2.23"
 unicode = "^2.7"
 lxml = "^4.6"
-selenium = "^4.0.0"
 Unidecode = "^1.2.0"
 rich = "^13.0.0"
 PySocks = "^1.7.1"
 html5lib = "^1.1"
-undetected-chromedriver = "^3.1.3"
+undetected-chromedriver = "^3.5.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 mypy = "^1.0"
 pylint = "^2.15.5"
 pytest-deadfixtures = "^2.2.1"
 unify = "^0.5"
```

### Comparing `soccerdata-1.5.0/soccerdata/_common.py` & `soccerdata-1.5.1/soccerdata/_common.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.5.0/soccerdata/_config.py` & `soccerdata-1.5.1/soccerdata/_config.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.5.0/soccerdata/clubelo.py` & `soccerdata-1.5.1/soccerdata/clubelo.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.5.0/soccerdata/espn.py` & `soccerdata-1.5.1/soccerdata/espn.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.5.0/soccerdata/fbref.py` & `soccerdata-1.5.1/soccerdata/fbref.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Scraper for http://fbref.com."""
-import itertools
 import warnings
 from datetime import date, datetime
 from functools import reduce
 from pathlib import Path
 from typing import Callable, Dict, List, Optional, Union
 
 import pandas as pd
@@ -86,29 +85,29 @@
             no_cache=no_cache,
             no_store=no_store,
             data_dir=data_dir,
         )
         self.rate_limit = 3
         self.seasons = seasons  # type: ignore
         # check if all top 5 leagues are selected
-        if set(BIG_FIVE_DICT.values()).issubset(self.leagues):
+        if (
+            set(BIG_FIVE_DICT.values()).issubset(self.leagues)
+            and "Big 5 European Leagues Combined" not in self.leagues
+        ):
             warnings.warn(
                 "You are trying to scrape data for all of the Big 5 European leagues. "
                 "This can be done more efficiently by setting "
                 "leagues='Big 5 European Leagues Combined'.",
                 stacklevel=1,
             )
 
     @property
     def leagues(self) -> List[str]:
         """Return a list of selected leagues."""
-        selected_leagues = set(self._leagues_dict.keys())
-        if "Big 5 European Leagues Combined" in selected_leagues:
-            selected_leagues -= set(BIG_FIVE_DICT.values())
-        return list(selected_leagues)
+        return list(self._leagues_dict.keys())
 
     @classmethod
     def _all_leagues(cls) -> Dict[str, str]:
         """Return a dict mapping all canonical league IDs to source league IDs."""
         res = super()._all_leagues()
         res.update({"Big 5 European Leagues Combined": "Big 5 European Leagues Combined"})
         return res
@@ -116,54 +115,73 @@
     def _is_complete(self, league: str, season: str) -> bool:
         """Check if a season is complete."""
         if league == "Big 5 European Leagues Combined":
             season_ends = date(datetime.strptime(season[-2:], "%y").year, 7, 1)
             return date.today() >= season_ends
         return super()._is_complete(league, season)
 
-    def read_leagues(self) -> pd.DataFrame:
+    def read_leagues(self, split_up_big5: bool = False) -> pd.DataFrame:
         """Retrieve selected leagues from the datasource.
 
+        Parameters
+        ----------
+        split_up_big5: bool
+            If True, it will load the "Big 5 European Leagues Combined" instead of
+            each league individually.
+
         Returns
         -------
         pd.DataFrame
         """
         url = f"{FBREF_API}/en/comps/"
         filepath = self.data_dir / "leagues.html"
         reader = self.get(url, filepath)
 
         # extract league links
-        leagues = []
+        dfs = []
         tree = html.parse(reader)
         for html_table in tree.xpath("//table[contains(@id, 'comps')]"):
             df_table = _parse_table(html_table)
             df_table["url"] = html_table.xpath(".//th[@data-stat='league_name']/a/@href")
-            leagues.append(df_table)
+            dfs.append(df_table)
         df = (
-            pd.concat(leagues)
+            pd.concat(dfs)
             .pipe(standardize_colnames)
             .rename(columns={"competition_name": "league"})
             .pipe(self._translate_league)
             .drop_duplicates(subset="league")
             .set_index("league")
             .sort_index()
         )
         df["first_season"] = df["first_season"].apply(season_code)
         df["last_season"] = df["last_season"].apply(season_code)
-        return df[df.index.isin(self.leagues)]
 
-    def read_seasons(self) -> pd.DataFrame:
+        leagues = self.leagues
+        if "Big 5 European Leagues Combined" in self.leagues and split_up_big5:
+            leagues = list(
+                (set(self.leagues) - {"Big 5 European Leagues Combined"})
+                | set(BIG_FIVE_DICT.values())
+            )
+        return df[df.index.isin(leagues)]
+
+    def read_seasons(self, split_up_big5: bool = False) -> pd.DataFrame:
         """Retrieve the selected seasons for the selected leagues.
 
+        Parameters
+        ----------
+        split_up_big5: bool
+            If True, it will load the "Big 5 European Leagues Combined" instead of
+            each league individually.
+
         Returns
         -------
         pd.DataFrame
         """
         filemask = "seasons_{}.html"
-        df_leagues = self.read_leagues()
+        df_leagues = self.read_leagues(split_up_big5)
 
         seasons = []
         for lkey, league in df_leagues.iterrows():
             url = FBREF_API + league.url
             filepath = self.data_dir / filemask.format(lkey)
             reader = self.get(url, filepath)
 
@@ -188,17 +206,15 @@
 
         df = pd.concat(seasons).pipe(standardize_colnames)
         df = df.rename(columns={"competition_name": "league"})
         df["season"] = df["season"].apply(season_code)
         # if both a 20xx and 19xx season are available, drop the 19xx season
         df.drop_duplicates(subset=["league", "season"], keep="first", inplace=True)
         df = df.set_index(["league", "season"]).sort_index()
-        return df.loc[
-            df.index.isin(list(itertools.product(self.leagues, self.seasons))), ["format", "url"]
-        ]
+        return df.loc[(slice(None), self.seasons), ["format", "url"]]
 
     def read_team_season_stats(  # noqa: C901
         self, stat_type: str = "standard", opponent_stats: bool = False
     ) -> pd.DataFrame:
         """Retrieve aggregated season stats for all teams in the selected leagues and seasons.
 
         The following stat types are available:
@@ -601,15 +617,15 @@
              If True, will force the use of cached data anyway.
 
         Returns
         -------
         pd.DataFrame
         """
         # get league IDs
-        seasons = self.read_seasons()
+        seasons = self.read_seasons(split_up_big5=True)
 
         # collect teams
         schedule = []
         for (lkey, skey), season in seasons.iterrows():
             # read html page (league overview)
             url_stats = FBREF_API + season.url
             filepath_stats = self.data_dir / f"teams_{lkey}_{skey}.html"
@@ -863,17 +879,23 @@
                     df_table["game"] = game["game"]
                     df_table.drop(bench_idx, inplace=True)
                 # augment with stats
                 html_stats_table = tree.find(
                     "//table[@id='" + "stats_{}_summary".format(teams[i]["id"]) + "']"
                 )
                 df_stats_table = _parse_table(html_stats_table)
-                df_stats_table = df_stats_table.droplevel(0, axis=1)[["Player", "Pos", "Min"]]
-                df_stats_table.columns = ["player", "position", "minutes_played"]
-                lineups.append(pd.merge(df_table, df_stats_table, on="player", how="left"))
+                df_stats_table = df_stats_table.droplevel(0, axis=1)[["Player", "#", "Pos", "Min"]]
+                df_stats_table.columns = ["player", "jersey_number", "position", "minutes_played"]
+                df_stats_table["jersey_number"] = df_stats_table["jersey_number"].astype("Int64")
+                df_table["jersey_number"] = df_table["jersey_number"].astype("Int64")
+                df_table = pd.merge(
+                    df_table, df_stats_table, on=["player", "jersey_number"], how="left"
+                )
+                df_table["minutes_played"] = df_table["minutes_played"].fillna(0)
+                lineups.append(df_table)
         df = pd.concat(lineups).set_index(["league", "season", "game"])
         return df
 
     def read_events(
         self, match_id: Optional[Union[str, List[str]]] = None, force_cache: bool = False
     ) -> pd.DataFrame:
         """Retrieve match events for the selected seasons or selected matches.
@@ -1076,67 +1098,69 @@
 
 def _concat(dfs: List[pd.DataFrame], key: List[str]) -> pd.DataFrame:
     """Merge matching tables scraped from different pages.
 
     The level 0 headers are not consistent across seasons and leagues, this
     function tries to determine uniform column names.
 
+    If there are dataframes with different columns, we will use the ones from
+    the dataframe with the most columns.
+
     Parameters
     ----------
     dfs : list(pd.DataFrame)
         Input dataframes.
     key : list(str)
         List of columns that uniquely identify each df.
 
-    Raises
-    ------
-    RuntimeError
-        If the dfs cannot be merged due to the columns not matching each other.
-
     Returns
     -------
     pd.DataFrame
         Concatenated dataframe with uniform column names.
     """
     all_columns = []
 
+    # Step 0: Sort dfs by the number of columns
+    dfs = sorted(dfs, key=lambda x: len(x.columns), reverse=True)
+
     # Step 1: Clean up the columns of each dataframe that should be merged
     for df in dfs:
         columns = pd.DataFrame(df.columns.tolist())
         # Set "Unnamed: ..." column names to None
         columns.replace(to_replace=r"^Unnamed:.*", value=None, regex=True, inplace=True)
         if columns.shape[1] == 2:
             # Set "" column names to None
             columns.replace(to_replace="", value=None, inplace=True)
             # Move None column names to level 0
             mask = pd.isnull(columns[1])
             columns.loc[mask, [0, 1]] = columns.loc[mask, [1, 0]].values
+
             # We'll try to replace some the None values in step 2
             all_columns.append(columns.copy())
             # But for now, we assume that we cannot replace them and move all
             # missing columns to level 1 and replace them with the empty string
             mask = pd.isnull(columns[0])
             columns.loc[mask, [0, 1]] = columns.loc[mask, [1, 0]].values
             columns.loc[mask, 1] = ""
             df.columns = pd.MultiIndex.from_tuples(columns.to_records(index=False).tolist())
 
-    # all dataframes should now have the same length and level 1 columns
+    # throw a warning if not all dataframes have the same length and level 1 columns
     if len(all_columns) and all_columns[0].shape[1] == 2:
         for i, columns in enumerate(all_columns):
             if not columns[1].equals(all_columns[0][1]):
                 res = all_columns[0].merge(columns, indicator=True, how='outer')
-                raise RuntimeError(
+                warnings.warn(
                     (
-                        "Cannot merge the data for {first} and {cur}.\n\n"
+                        "Different columns found for {first} and {cur}.\n\n"
                         + "The following columns are missing in {first}: {extra_cols}.\n\n"
                         + "The following columns are missing in {cur}: {missing_cols}.\n\n"
-                        + "Please try to scrape the data again with caching disabled."
+                        + "The columns of the dataframe with the most columns will be used."
                     ).format(
-                        first=dfs[0].loc[0, key].values,
-                        cur=dfs[i].loc[0, key].values,
+                        first=dfs[0].iloc[:1][key].values,
+                        cur=dfs[i].iloc[:1][key].values,
                         extra_cols=", ".join(
                             map(
                                 str,
                                 res.loc[res['_merge'] == "left_only", [0, 1]]
                                 .to_records(index=False)
                                 .tolist(),
                             )
@@ -1146,34 +1170,40 @@
                                 str,
                                 res.loc[res['_merge'] == "right_only", [0, 1]]
                                 .to_records(index=False)
                                 .tolist(),
                             )
                         ),
                     ),
+                    stacklevel=1,
                 )
 
+    if len(all_columns) and all_columns[0].shape[1] == 2:
         # Step 2: Look for the most complete level 0 columns
         columns = reduce(lambda left, right: left.combine_first(right), all_columns)
 
         # Step 3: Make sure columns are consistent
         mask = pd.isnull(columns[0])
         columns.loc[mask, [0, 1]] = columns.loc[mask, [1, 0]].values
         columns.loc[mask, 1] = ""
         column_idx = pd.MultiIndex.from_tuples(columns.to_records(index=False).tolist())
 
-        for df in dfs:
+        for i, df in enumerate(dfs):
             if df.columns.equals(column_idx):
                 # This dataframe already has the uniform column index
                 pass
-            elif len(df.columns) == len(column_idx):
+            if len(df.columns) == len(column_idx):
                 # This dataframe has the same number of columns and the same
                 # level 1 columns, we assume that the level 0 columns can be
                 # replaced
                 df.columns = column_idx
+            else:
+                # This dataframe has a different number of columns, so we want
+                # to make sure its columns match with column_idx
+                dfs[i] = df.reindex(columns=column_idx, fill_value=None)
 
     return pd.concat(dfs)
 
 
 def _fix_nation_col(df_table: pd.DataFrame) -> pd.DataFrame:
     """Fix the "Nation" column.
```

### Comparing `soccerdata-1.5.0/soccerdata/fivethirtyeight.py` & `soccerdata-1.5.1/soccerdata/fivethirtyeight.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.5.0/soccerdata/match_history.py` & `soccerdata-1.5.1/soccerdata/match_history.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.5.0/soccerdata/sofifa.py` & `soccerdata-1.5.1/soccerdata/sofifa.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.5.0/soccerdata/whoscored.py` & `soccerdata-1.5.1/soccerdata/whoscored.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.5.0/PKG-INFO` & `soccerdata-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soccerdata
-Version: 1.5.0
+Version: 1.5.1
 Summary: A collection of wrappers over soccer data from various websites / APIs.
 Home-page: https://github.com/probberechts/soccerdata
 License: Apache-2.0
 Keywords: soccer,football,soccer data,web scraping,soccer analytics
 Author: Pieter Robberechts
 Author-email: pieter.robberechts@kuleuven.be
 Requires-Python: >=3.8.1,<4.0.0
@@ -18,16 +18,15 @@
 Requires-Dist: PySocks (>=1.7.1,<2.0.0)
 Requires-Dist: Unidecode (>=1.2.0,<2.0.0)
 Requires-Dist: html5lib (>=1.1,<2.0)
 Requires-Dist: lxml (>=4.6,<5.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: requests (>=2.23,<3.0)
 Requires-Dist: rich (>=13.0.0,<14.0.0)
-Requires-Dist: selenium (>=4.0.0,<5.0.0)
-Requires-Dist: undetected-chromedriver (>=3.1.3,<4.0.0)
+Requires-Dist: undetected-chromedriver (>=3.5.0,<4.0.0)
 Requires-Dist: unicode (>=2.7,<3.0)
 Project-URL: Repository, https://github.com/probberechts/soccerdata
 Description-Content-Type: text/x-rst
 
 .. image:: https://raw.githubusercontent.com/probberechts/soccerdata/master/docs/_static/logo2.png
    :align: center
    :alt: SoccerData
```


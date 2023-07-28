# Comparing `tmp/psychoanalyze-0.7.0.tar.gz` & `tmp/psychoanalyze-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoanalyze-0.7.0.tar", max compression
+gzip compressed data, was "psychoanalyze-0.8.0.tar", max compression
```

## Comparing `psychoanalyze-0.7.0.tar` & `psychoanalyze-0.8.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0    35149 2022-10-04 02:36:06.350931 psychoanalyze-0.7.0/LICENSE
--rw-r--r--   0        0        0     1105 2023-07-10 23:11:08.910130 psychoanalyze-0.7.0/README.md
--rw-r--r--   0        0        0     1357 2023-07-10 06:32:31.020291 psychoanalyze-0.7.0/psychoanalyze/__init__.py
--rw-r--r--   0        0        0      756 2023-07-10 06:35:55.935533 psychoanalyze-0.7.0/psychoanalyze/analysis/__init__.py
--rw-r--r--   0        0        0     1288 2023-07-10 06:35:48.275360 psychoanalyze-0.7.0/psychoanalyze/analysis/bayes.py
--rw-r--r--   0        0        0     1120 2023-07-10 06:35:38.831225 psychoanalyze-0.7.0/psychoanalyze/analysis/ecdf.py
--rw-r--r--   0        0        0     2302 2023-07-10 23:10:13.757714 psychoanalyze-0.7.0/psychoanalyze/analysis/strength_duration.py
--rw-r--r--   0        0        0     2373 2023-07-10 06:35:32.351775 psychoanalyze-0.7.0/psychoanalyze/analysis/weber.py
--rw-r--r--   0        0        0     1070 2023-07-10 06:31:40.686289 psychoanalyze-0.7.0/psychoanalyze/dashboard/__init__.py
--rw-r--r--   0        0        0    12406 2023-07-20 06:38:26.196273 psychoanalyze-0.7.0/psychoanalyze/dashboard/app.py
--rw-r--r--   0        0        0    10618 2023-07-11 07:34:32.872491 psychoanalyze-0.7.0/psychoanalyze/dashboard/assets/PsychoAnalyze.svg
--rw-r--r--   0        0        0    33510 2023-07-11 07:34:42.444787 psychoanalyze-0.7.0/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png
--rw-r--r--   0        0        0     6575 2023-07-20 04:43:03.897369 psychoanalyze-0.7.0/psychoanalyze/dashboard/assets/favicon.ico
--rw-r--r--   0        0        0     6575 2023-07-20 04:41:06.090118 psychoanalyze-0.7.0/psychoanalyze/dashboard/assets/logo_bgwhite.png
--rw-r--r--   0        0        0     5350 2023-07-11 09:34:15.577086 psychoanalyze-0.7.0/psychoanalyze/dashboard/assets/logo_transparent_100x100.png
--rw-r--r--   0        0        0      551 2023-07-15 02:24:50.772266 psychoanalyze-0.7.0/psychoanalyze/dashboard/assets/styles.css
--rw-r--r--   0        0        0    11423 2023-07-20 05:46:31.875938 psychoanalyze-0.7.0/psychoanalyze/dashboard/components.py
--rw-r--r--   0        0        0     8514 2023-07-20 06:38:02.146351 psychoanalyze-0.7.0/psychoanalyze/dashboard/layout.py
--rw-r--r--   0        0        0     1153 2023-07-15 09:38:33.343476 psychoanalyze-0.7.0/psychoanalyze/data/__init__.py
--rw-r--r--   0        0        0     5715 2023-07-19 06:34:50.450027 psychoanalyze-0.7.0/psychoanalyze/data/blocks.py
--rw-r--r--   0        0        0     7245 2023-07-19 04:42:14.885318 psychoanalyze-0.7.0/psychoanalyze/data/points.py
--rw-r--r--   0        0        0     2868 2023-07-10 06:35:10.993442 psychoanalyze-0.7.0/psychoanalyze/data/sessions.py
--rw-r--r--   0        0        0      841 2023-07-10 06:35:04.783422 psychoanalyze-0.7.0/psychoanalyze/data/stimulus.py
--rw-r--r--   0        0        0     1678 2023-07-10 06:34:48.603492 psychoanalyze-0.7.0/psychoanalyze/data/subjects.py
--rw-r--r--   0        0        0     5206 2023-07-14 06:02:28.786486 psychoanalyze-0.7.0/psychoanalyze/data/trials.py
--rw-r--r--   0        0        0     3002 2023-07-16 02:29:21.297443 psychoanalyze-0.7.0/psychoanalyze/data/types.py
--rw-r--r--   0        0        0     1589 2023-07-10 06:34:59.633459 psychoanalyze-0.7.0/psychoanalyze/plot.py
--rw-r--r--   0        0        0     1518 2023-07-10 06:34:24.801696 psychoanalyze-0.7.0/psychoanalyze/sigmoids.py
--rw-r--r--   0        0        0     1954 2023-07-20 07:51:59.410195 psychoanalyze-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 psychoanalyze-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-04 02:36:06.350931 psychoanalyze-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1274 2023-07-26 11:57:00.456909 psychoanalyze-0.8.0/README.md
+-rw-r--r--   0        0        0     1357 2023-07-10 06:32:31.020291 psychoanalyze-0.8.0/psychoanalyze/__init__.py
+-rw-r--r--   0        0        0      756 2023-07-10 06:35:55.935533 psychoanalyze-0.8.0/psychoanalyze/analysis/__init__.py
+-rw-r--r--   0        0        0     1288 2023-07-10 06:35:48.275360 psychoanalyze-0.8.0/psychoanalyze/analysis/bayes.py
+-rw-r--r--   0        0        0     1120 2023-07-10 06:35:38.831225 psychoanalyze-0.8.0/psychoanalyze/analysis/ecdf.py
+-rw-r--r--   0        0        0     2302 2023-07-10 23:10:13.757714 psychoanalyze-0.8.0/psychoanalyze/analysis/strength_duration.py
+-rw-r--r--   0        0        0     2373 2023-07-10 06:35:32.351775 psychoanalyze-0.8.0/psychoanalyze/analysis/weber.py
+-rw-r--r--   0        0        0     1070 2023-07-10 06:31:40.686289 psychoanalyze-0.8.0/psychoanalyze/dashboard/__init__.py
+-rw-r--r--   0        0        0    12468 2023-07-28 02:10:21.380217 psychoanalyze-0.8.0/psychoanalyze/dashboard/app.py
+-rw-r--r--   0        0        0    10618 2023-07-11 07:34:32.872491 psychoanalyze-0.8.0/psychoanalyze/dashboard/assets/PsychoAnalyze.svg
+-rw-r--r--   0        0        0    33510 2023-07-11 07:34:42.444787 psychoanalyze-0.8.0/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png
+-rw-r--r--   0        0        0     6575 2023-07-20 04:43:03.897369 psychoanalyze-0.8.0/psychoanalyze/dashboard/assets/favicon.ico
+-rw-r--r--   0        0        0     6575 2023-07-20 04:41:06.090118 psychoanalyze-0.8.0/psychoanalyze/dashboard/assets/logo_bgwhite.png
+-rw-r--r--   0        0        0     5350 2023-07-11 09:34:15.577086 psychoanalyze-0.8.0/psychoanalyze/dashboard/assets/logo_transparent_100x100.png
+-rw-r--r--   0        0        0      551 2023-07-15 02:24:50.772266 psychoanalyze-0.8.0/psychoanalyze/dashboard/assets/styles.css
+-rw-r--r--   0        0        0     8915 2023-07-28 00:17:06.312544 psychoanalyze-0.8.0/psychoanalyze/dashboard/components.py
+-rw-r--r--   0        0        0     8514 2023-07-20 06:38:02.146351 psychoanalyze-0.8.0/psychoanalyze/dashboard/layout.py
+-rw-r--r--   0        0        0     1153 2023-07-20 09:25:55.060489 psychoanalyze-0.8.0/psychoanalyze/data/__init__.py
+-rw-r--r--   0        0        0     6031 2023-07-28 00:17:06.312544 psychoanalyze-0.8.0/psychoanalyze/data/blocks.py
+-rw-r--r--   0        0        0     6787 2023-07-28 00:17:06.312544 psychoanalyze-0.8.0/psychoanalyze/data/points.py
+-rw-r--r--   0        0        0     2868 2023-07-10 06:35:10.993442 psychoanalyze-0.8.0/psychoanalyze/data/sessions.py
+-rw-r--r--   0        0        0      841 2023-07-10 06:35:04.783422 psychoanalyze-0.8.0/psychoanalyze/data/stimulus.py
+-rw-r--r--   0        0        0     1678 2023-07-10 06:34:48.603492 psychoanalyze-0.8.0/psychoanalyze/data/subjects.py
+-rw-r--r--   0        0        0     5225 2023-07-20 09:41:06.475106 psychoanalyze-0.8.0/psychoanalyze/data/trials.py
+-rw-r--r--   0        0        0     3002 2023-07-16 02:29:21.297443 psychoanalyze-0.8.0/psychoanalyze/data/types.py
+-rw-r--r--   0        0        0     1135 2023-07-28 02:10:21.380217 psychoanalyze-0.8.0/psychoanalyze/main.py
+-rw-r--r--   0        0        0     1239 2023-07-21 04:57:55.937376 psychoanalyze-0.8.0/psychoanalyze/params.py
+-rw-r--r--   0        0        0     2116 2023-07-21 02:42:52.381174 psychoanalyze-0.8.0/psychoanalyze/plot.py
+-rw-r--r--   0        0        0     1518 2023-07-10 06:34:24.801696 psychoanalyze-0.8.0/psychoanalyze/sigmoids.py
+-rw-r--r--   0        0        0     3176 2023-07-28 06:17:26.754486 psychoanalyze-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3827 1970-01-01 00:00:00.000000 psychoanalyze-0.8.0/PKG-INFO
```

### Comparing `psychoanalyze-0.7.0/LICENSE` & `psychoanalyze-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/__init__.py` & `psychoanalyze-0.8.0/psychoanalyze/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/analysis/__init__.py` & `psychoanalyze-0.8.0/psychoanalyze/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/analysis/bayes.py` & `psychoanalyze-0.8.0/psychoanalyze/analysis/bayes.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/analysis/ecdf.py` & `psychoanalyze-0.8.0/psychoanalyze/analysis/ecdf.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/analysis/strength_duration.py` & `psychoanalyze-0.8.0/psychoanalyze/analysis/strength_duration.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/analysis/weber.py` & `psychoanalyze-0.8.0/psychoanalyze/analysis/weber.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/dashboard/__init__.py` & `psychoanalyze-0.8.0/psychoanalyze/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/dashboard/app.py` & `psychoanalyze-0.8.0/psychoanalyze/dashboard/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     """Update points table."""
     n_param_values = [
         "n_levels",
         "n_trials",
         "n_blocks",
     ]
     n_params = pd.Series(n_param, index=n_param_values)
+    param = [*param, 0.0, 0.0]
     params = pd.Series(param, index=["x_0", "k", "gamma", "lambda"])
     params["intercept"] = -params["x_0"] / params["k"]
     params["slope"] = 1 / params["k"]
     min_x = (logit(0.01) - params["intercept"]) / params["slope"]
     max_x = (logit(0.99) - params["intercept"]) / params["slope"]
     if callback_context.triggered_id == "upload":
         _, content_string = contents.split(",")
@@ -185,14 +186,15 @@
     points: Records,
     blocks: Records,
     selected_rows: list[int],
     min_x: float,
     max_x: float,
 ) -> go.Figure:
     """Update plot and tables based on data store and selected view."""
+    param = [*param, 0.0, 0.0]
     params = pd.Series(param, index=["x_0", "k", "gamma", "lambda"])
     params["intercept"] = -params["x_0"] / params["k"]
     params["slope"] = 1 / params["k"]
     blocks = [blocks[i] for i in selected_rows] + [
         {"Block": "Model"} | params.to_dict(),
     ]
     x = pd.Index(
```

### Comparing `psychoanalyze-0.7.0/psychoanalyze/dashboard/assets/PsychoAnalyze.svg` & `psychoanalyze-0.8.0/psychoanalyze/dashboard/assets/PsychoAnalyze.svg`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png` & `psychoanalyze-0.8.0/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/dashboard/assets/favicon.ico` & `psychoanalyze-0.8.0/psychoanalyze/dashboard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/dashboard/assets/logo_bgwhite.png` & `psychoanalyze-0.8.0/psychoanalyze/dashboard/assets/logo_bgwhite.png`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/dashboard/assets/logo_transparent_100x100.png` & `psychoanalyze-0.8.0/psychoanalyze/dashboard/assets/logo_transparent_100x100.png`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/dashboard/assets/styles.css` & `psychoanalyze-0.8.0/psychoanalyze/dashboard/assets/styles.css`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/dashboard/components.py` & `psychoanalyze-0.8.0/psychoanalyze/dashboard/components.py`

 * *Files 19% similar despite different names*

```diff
@@ -80,81 +80,14 @@
                 ),
             ],
             class_name="g-0 mb-0",
         ),
         dbc.Row(
             [
                 dbc.Col(
-                    dcc.Markdown("$\\gamma$", mathjax=True),
-                    width=2,
-                    align="center",
-                    style={"text-align": "center"},
-                ),
-                dbc.Col(
-                    dbc.InputGroup(
-                        [
-                            dbc.InputGroupText(
-                                dbc.Checkbox(
-                                    id={"type": "free", "name": "gamma"},
-                                    value=True,
-                                ),
-                            ),
-                            dbc.Input(
-                                id={"type": "param", "name": "gamma"},
-                                type="number",
-                                value=0.0,
-                                step=0.1,
-                                min=0.0,
-                                max=1.0,
-                            ),
-                        ],
-                        size="sm",
-                        class_name="p-0",
-                    ),
-                    width=4,
-                    align="center",
-                    style={"text-align": "center"},
-                ),
-                dbc.Col(
-                    dcc.Markdown("$\\lambda$", mathjax=True),
-                    width=2,
-                    align="center",
-                    style={"text-align": "center"},
-                ),
-                dbc.Col(
-                    dbc.InputGroup(
-                        [
-                            dbc.InputGroupText(
-                                dbc.Checkbox(
-                                    value=True,
-                                    id={"type": "free", "name": "lambda"},
-                                ),
-                            ),
-                            dbc.Input(
-                                id={"type": "param", "name": "lambda"},
-                                type="number",
-                                value=0.0,
-                                step=0.1,
-                                min=0.0,
-                                max=1.0,
-                            ),
-                        ],
-                        size="sm",
-                        class_name="p-0",
-                    ),
-                    width=4,
-                    align="center",
-                    style={"text-align": "center"},
-                ),
-            ],
-            class_name="g-0",
-        ),
-        dbc.Row(
-            [
-                dbc.Col(
                     dcc.Dropdown(
                         id="preset",
                         placeholder="Presets",
                         options=[
                             {
                                 "label": "Standard",
                                 "value": "standard",
```

### Comparing `psychoanalyze-0.7.0/psychoanalyze/dashboard/layout.py` & `psychoanalyze-0.8.0/psychoanalyze/dashboard/layout.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/data/__init__.py` & `psychoanalyze-0.8.0/psychoanalyze/data/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/data/blocks.py` & `psychoanalyze-0.8.0/psychoanalyze/data/blocks.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 import plotly.express as px
 import plotly.graph_objects as go
 from scipy.special import expit
 from scipy.stats import logistic as scipy_logistic
 from sklearn.linear_model import LogisticRegression
 
 from psychoanalyze.data import (
-    points,
     sessions,
     stimulus,
     subjects,
     trials,
 )
 from psychoanalyze.plot import template
 
@@ -53,21 +52,14 @@
     p = scipy_logistic.cdf(index)
     return pd.DataFrame(
         {"n": n, "Hits": np.random.default_rng().binomial(n, p)},
         index=index,
     )
 
 
-def dimensions(_points: pd.DataFrame, dims: list[str]) -> pd.Series:
-    """Calculate dimensions for multiple blocks."""
-    return _points.groupby(
-        [dim for dim in list(_points.index.names) if dim not in dims],
-    ).apply(points.dimension)
-
-
 def plot_fits(blocks: pd.DataFrame) -> go.Figure:
     """Plot fits."""
     x = np.linspace(-3, 3, 100)
     y = expit(x)
     return px.line(blocks.reset_index(), x=x, y=y)
 
 
@@ -172,7 +164,23 @@
         rows,  # row eg 'p[1]:p[8]'
         ["5%", "50%", "95%"],  # col
     ]
     param_fits = transform_errors(param_fits)
     param_fits = param_fits.rename(columns={"50%": y})
     param_fits.index = x
     return param_fits
+
+
+def standard_logistic() -> pd.Series:
+    """Generate points for a line trace of a standard logistic function."""
+    x = pd.Index(np.linspace(-3, 3, 100), name="x")
+    y = expit(x)
+    return pd.Series(y, index=x, name="f(x)")
+
+
+def logistic(location: float, scale: float) -> pd.Series:
+    """Generate points for a line trace of a logistic function."""
+    x_min = (location - 4) * scale
+    x_max = (location + 4) * scale
+    x = pd.Index(np.linspace(x_min, x_max, 100), name="Intensity")
+    y = expit((x - location) / scale)
+    return pd.Series(y, index=x, name="Ψ(x)")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `psychoanalyze-0.7.0/psychoanalyze/data/points.py` & `psychoanalyze-0.8.0/psychoanalyze/data/points.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,28 +49,14 @@
 @check_output(types.points)
 def load(data_path: Path) -> pd.DataFrame:
     """Load points data from csv."""
     trials = pa_trials.load(data_path)
     return from_trials(trials)
 
 
-def dimension(points: pd.DataFrame) -> str:
-    """Determine modulated dimension from point-level data."""
-    amp1, width1 = (
-        points.index.get_level_values(param) for param in ["Amp1", "Width1"]
-    )
-    if amp1.nunique() > 1 and width1.nunique() == 1:
-        return "Amp"
-    if width1.nunique() > 1 and amp1.nunique() == 1:
-        return "Width"
-    if width1.nunique() > 1 and amp1.nunique() > 1:
-        return "Both"
-    return "Neither"
-
-
 def prep_fit(points: pd.DataFrame, dimension: str = "Amp1") -> dict:
     """Transform points data for numpy-related fitting procedures."""
     points = points.reset_index()
     return {
         "X": len(points),
         "x": points[f"{dimension}"].to_numpy(),
         "N": points["n"].to_numpy(),
```

### Comparing `psychoanalyze-0.7.0/psychoanalyze/data/sessions.py` & `psychoanalyze-0.8.0/psychoanalyze/data/sessions.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/data/stimulus.py` & `psychoanalyze-0.8.0/psychoanalyze/data/stimulus.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/data/subjects.py` & `psychoanalyze-0.8.0/psychoanalyze/data/subjects.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/data/trials.py` & `psychoanalyze-0.8.0/psychoanalyze/data/trials.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,21 +55,24 @@
         {
             "Result": [int(random.random() <= psi(x_val, params)) for x_val in x],
             "Intensity": x,
         },
     )
 
 
-def load(data_path: Path = Path("data")) -> pd.DataFrame:
+def load(data_path: Path) -> pd.DataFrame:
     """Load trials data from csv."""
     return types.trials.validate(
         pd.read_csv(
-            data_path / "trials.csv",
-            index_col=types.points_index_levels,
-            parse_dates=["Date"],
+            data_path,
+            dtype={
+                "Result": int,
+                "Intensity": float,
+                "Block": int,
+            },
         ),
     )
 
 
 def from_store(store_data: str) -> pd.DataFrame:
     """Convert JSON-formatted string to DataFrame."""
     df_dict = json.loads(store_data)
```

### Comparing `psychoanalyze-0.7.0/psychoanalyze/data/types.py` & `psychoanalyze-0.8.0/psychoanalyze/data/types.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/psychoanalyze/plot.py` & `psychoanalyze-0.8.0/psychoanalyze/plot.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License along with
 # PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Global plot settings and generic plot utilities."""
-from plotly import graph_objects as go
+
+import plotly.express as px
+import plotly.graph_objects as go
+
+from psychoanalyze.data import blocks
 
 axis_settings = {
     "ticks": "outside",
     "showgrid": False,
     "showline": True,
     "zeroline": False,
     "title": {"font": {"size": 12, "family": "Arial"}},
@@ -43,7 +47,26 @@
         "y": "Threshold Amplitude (μA)",
     },
     "Width": {
         "x": "Fixed Amplitude (μA)",
         "y": "Threshold Pulse Width (μs)",
     },
 }
+
+
+def standard_logistic() -> go.Scatter:
+    """Plot a standard logistic function."""
+    return px.line(
+        blocks.standard_logistic(),
+        y="f(x)",
+        template="plotly_white",
+        title="$f(x) = \\frac{1}{1 + e^{-x}}$",
+    )
+
+
+def logistic(location: float, scale: float) -> go.Scatter:
+    """Plot a logistic function."""
+    return px.line(
+        blocks.logistic(location, scale),
+        y="Ψ(x)",
+        template="plotly_white",
+    )
```

### Comparing `psychoanalyze-0.7.0/psychoanalyze/sigmoids.py` & `psychoanalyze-0.8.0/psychoanalyze/sigmoids.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.7.0/pyproject.toml` & `psychoanalyze-0.8.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,98 @@
 [tool.poetry]
 name = "psychoanalyze"
-version = "0.7.0"
-description = "A Pythonic analysis package for psychophysics data"
+version = "0.8.0"
+description = "Interactive analysis and simulation of psychophysical data."
 authors = ["Ty Schlichenmeyer <t.schlic@wustl.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
+packages = [{ include = "psychoanalyze" }]
+homepage = "https://psychoanalyze.io"
+repository = "https://github.com/psychoanalyze/psychoanalyze"
+documentation = "https://docs.psychoanalyze.io"
+keywords = ["psychophysics", "neuroscience", "psychology", "bayes"]
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Environment :: Web Environment",
+    "Framework :: Dash",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+    "Natural Language :: English",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Scientific/Engineering :: Visualization",
+    "Topic :: Scientific/Engineering :: Information Analysis",
+    "Topic :: Scientific/Engineering :: Medical Science Apps.",
+]
+urls = { JupyterHub = "https://nb.psychoanalyze.io" }
 
 [tool.poetry.dependencies]
 python = "3.11.4"
 pandas = "^2.0.2"
 scipy = "^1.10.1"
 numpy = "^1.25.0"
 dash-bootstrap-components = "^1.4.1"
 statsmodels = "^0.14.0"
 dash-daq = "^0.5.0"
 dash = "^2.11.1"
-dbt-duckdb = "^1.5.1"
+dbt-duckdb = "^1.5.2"
 scikit-learn = "^1.2.2"
 bambi = "^0.11.0"
 cmdstanpy = "^1.1.0"
 pandas-stubs = "^2.0.2.230605"
-pandera = {extras = ["mypy"], version = "^0.15.1"}
+pandera = { extras = ["mypy"], version = "^0.15.1" }
 pytest = "^7.3.2"
 hypothesis = "^6.79.0"
 datatest = "^0.11.1"
 pytest-mock = "^3.11.1"
 gunicorn = "^20.1.0"
 mypy = "^1.4.1"
 click = "^8.1.3"
-typer = {extras = ["all"], version = "^0.9.0"}
+typer = { extras = ["all"], version = "^0.9.0" }
 tuna = "^0.5.11"
-ruff = "^0.0.276"
+ruff = "^0.0.280"
 black = "^23.3.0"
 ipykernel = "^6.24.0"
 ipywidgets = "^8.0.7"
 kaleido = "0.2.1"
 pyarrow = "^12.0.1"
 types-pytz = "^2023.3.0.0"
 python-semantic-release = "^8.0.2"
+jupyter = "^1.0.0"
+types-setuptools = "^68.0.0.3"
 
 [tool.poetry.scripts]
-psychoanalyze = "psychoanalyze.__main__:main"
+psychoanalyze = "psychoanalyze.main:app"
 
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry.extras]
+docs = ["mkdocs", "mkdocs-materal", "mkdocstrings-python"]
 
 [tool.semantic_release]
-version_variable = [
-    "psychoanalyze/__init__.py:__version__",
-    "pyproject.toml:version"
-]
-branch = "main"
+version_toml = ["pyproject.toml:tool.poetry.version"]
 build_command = "poetry build"
-major_on_zero = true
+commit_message = "chore(release): release {version}"
+
+[tool.semantic_release.branches.main]
+match = "^release"
+
+[tool.semantic_release.commit_parser_options]
+allowed_tags = [
+    "feat",
+    "fix",
+    "ci",
+    "docs",
+    "test",
+    "dash",
+    "dev",
+    "deps",
+    "style",
+    "refactor",
+    "perf",
+    "chore",
+    "notebook",
+]
 
 [tool.bandit]
 targets = ["psychoanalyze/"]
 skips = ["B311", "B104"]
 
 [tool.mypy]
 exclude = ['target']
@@ -73,21 +107,25 @@
     'scipy.special',
     'sklearn.linear_model',
     'dash_daq',
     'datatest',
     'bambi',
     'hypothesis',
     'statsmodels.*',
-    'pytz'
+    'pytz',
 ]
 ignore_missing_imports = true
 
 [tool.ruff]
 fix = true
 select = ["ALL", "CPY001"]
 ignore = ["S101", "S311", "D211", "D213"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.per-file-ignores]
 "tests/*.py" = ["D100", "D103", "ANN201"]
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `psychoanalyze-0.7.0/PKG-INFO` & `psychoanalyze-0.8.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,84 @@
 Metadata-Version: 2.1
 Name: psychoanalyze
-Version: 0.7.0
-Summary: A Pythonic analysis package for psychophysics data
+Version: 0.8.0
+Summary: Interactive analysis and simulation of psychophysical data.
+Home-page: https://psychoanalyze.io
 License: GPL-3.0-or-later
+Keywords: psychophysics,neuroscience,psychology,bayes
 Author: Ty Schlichenmeyer
 Author-email: t.schlic@wustl.edu
 Requires-Python: ==3.11.4
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Dash
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Provides-Extra: docs
 Requires-Dist: bambi (>=0.11.0,<0.12.0)
 Requires-Dist: black (>=23.3.0,<24.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cmdstanpy (>=1.1.0,<2.0.0)
 Requires-Dist: dash (>=2.11.1,<3.0.0)
 Requires-Dist: dash-bootstrap-components (>=1.4.1,<2.0.0)
 Requires-Dist: dash-daq (>=0.5.0,<0.6.0)
 Requires-Dist: datatest (>=0.11.1,<0.12.0)
-Requires-Dist: dbt-duckdb (>=1.5.1,<2.0.0)
+Requires-Dist: dbt-duckdb (>=1.5.2,<2.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: hypothesis (>=6.79.0,<7.0.0)
 Requires-Dist: ipykernel (>=6.24.0,<7.0.0)
 Requires-Dist: ipywidgets (>=8.0.7,<9.0.0)
+Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: kaleido (==0.2.1)
 Requires-Dist: mypy (>=1.4.1,<2.0.0)
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pandas-stubs (>=2.0.2.230605,<3.0.0.0)
 Requires-Dist: pandera[mypy] (>=0.15.1,<0.16.0)
 Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
 Requires-Dist: pytest (>=7.3.2,<8.0.0)
 Requires-Dist: pytest-mock (>=3.11.1,<4.0.0)
 Requires-Dist: python-semantic-release (>=8.0.2,<9.0.0)
-Requires-Dist: ruff (>=0.0.276,<0.0.277)
+Requires-Dist: ruff (>=0.0.280,<0.0.281)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Requires-Dist: tuna (>=0.5.11,<0.6.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: types-pytz (>=2023.3.0.0,<2024.0.0.0)
+Requires-Dist: types-setuptools (>=68.0.0.3,<69.0.0.0)
+Project-URL: Documentation, https://docs.psychoanalyze.io
+Project-URL: JupyterHub, https://nb.psychoanalyze.io
+Project-URL: Repository, https://github.com/psychoanalyze/psychoanalyze
 Description-Content-Type: text/markdown
 
 # PsychoAnalyze
 
-Psychophysics analysis in Python.
+Interactive data simulation and analysis for psychophysics.
+
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/psychoanalyze)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![Open in Remote - Containers](https://img.shields.io/static/v1?label=Remote%20-%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/psychoanalyze/psychoanalyze)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/psychoanalyze/psychoanalyze/main.svg)](https://results.pre-commit.ci/latest/github/psychoanalyze/psychoanalyze/main)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/psychoanalyze/psychoanalyze/main?labpath=docs%2Fnotebooks%2Ftutorial.ipynb)
 
 
+## Dashboard
+See what `psychoanalyze` can do by [viewing our dashboard](https://psychoanalyze.io/).
 
-## Installation
-poetry (preferred):
-```console
-poetry add psychoanalyze
-```
-pip:
+## Install with Python
 ```console
 pip install psychoanalyze
-```
-
-## Dashboard
-See what `psychoanalyze` can do by [viewing our dashboard](https://psychoanalyze.io/).
 
+psychoanalyze --help
+```
 ## Documentation
-View the full documentation [here](https://docs.psychoanalyze.io).
+View the full documentation at [https://docs.psychoanalyze.io](https://docs.psychoanalyze.io).
```


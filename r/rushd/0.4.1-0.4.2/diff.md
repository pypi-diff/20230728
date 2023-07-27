# Comparing `tmp/rushd-0.4.1.tar.gz` & `tmp/rushd-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rushd-0.4.1.tar", last modified: Tue Jun 27 16:28:16 2023, max compression
+gzip compressed data, was "rushd-0.4.2.tar", last modified: Thu Jul 27 22:21:58 2023, max compression
```

## Comparing `rushd-0.4.1.tar` & `rushd-0.4.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-06-27 16:28:16.027449 rushd-0.4.1/
--rw-r--r--   0 christopher  (1000) christopher  (1000)     1069 2022-08-30 19:04:22.000000 rushd-0.4.1/LICENSE
--rw-r--r--   0 christopher  (1000) christopher  (1000)     3950 2023-06-27 16:28:16.027449 rushd-0.4.1/PKG-INFO
--rw-r--r--   0 christopher  (1000) christopher  (1000)     2982 2023-06-27 16:26:42.000000 rushd-0.4.1/README.md
--rw-r--r--   0 christopher  (1000) christopher  (1000)      527 2023-02-02 22:08:57.000000 rushd-0.4.1/pyproject.toml
--rw-r--r--   0 christopher  (1000) christopher  (1000)       38 2023-06-27 16:28:16.027449 rushd-0.4.1/setup.cfg
--rw-r--r--   0 christopher  (1000) christopher  (1000)     1885 2023-06-27 16:26:11.000000 rushd-0.4.1/setup.py
-drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-06-27 16:28:16.020782 rushd-0.4.1/src/
-drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-06-27 16:28:16.024116 rushd-0.4.1/src/rushd/
--rw-r--r--   0 christopher  (1000) christopher  (1000)      651 2023-04-19 21:24:37.000000 rushd-0.4.1/src/rushd/__init__.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)    15035 2023-06-08 19:55:56.000000 rushd-0.4.1/src/rushd/flow.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)    11323 2023-06-08 19:55:36.000000 rushd-0.4.1/src/rushd/io.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)     6548 2023-06-08 19:54:47.000000 rushd-0.4.1/src/rushd/plot.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)     6268 2023-06-08 19:55:12.000000 rushd-0.4.1/src/rushd/well_mapper.py
-drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-06-27 16:28:16.024116 rushd-0.4.1/src/rushd.egg-info/
--rw-r--r--   0 christopher  (1000) christopher  (1000)     3950 2023-06-27 16:28:16.000000 rushd-0.4.1/src/rushd.egg-info/PKG-INFO
--rw-r--r--   0 christopher  (1000) christopher  (1000)      440 2023-06-27 16:28:16.000000 rushd-0.4.1/src/rushd.egg-info/SOURCES.txt
--rw-r--r--   0 christopher  (1000) christopher  (1000)        1 2023-06-27 16:28:16.000000 rushd-0.4.1/src/rushd.egg-info/dependency_links.txt
--rw-r--r--   0 christopher  (1000) christopher  (1000)      210 2023-06-27 16:28:16.000000 rushd-0.4.1/src/rushd.egg-info/requires.txt
--rw-r--r--   0 christopher  (1000) christopher  (1000)        6 2023-06-27 16:28:16.000000 rushd-0.4.1/src/rushd.egg-info/top_level.txt
-drwxr-xr-x   0 christopher  (1000) christopher  (1000)        0 2023-06-27 16:28:16.027449 rushd-0.4.1/tests/
--rw-r--r--   0 christopher  (1000) christopher  (1000)    11898 2023-02-02 22:12:16.000000 rushd-0.4.1/tests/test_file_io.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)     3607 2023-02-02 22:12:16.000000 rushd-0.4.1/tests/test_file_moi.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)    18337 2023-03-24 17:26:34.000000 rushd-0.4.1/tests/test_flow.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)      891 2023-02-02 22:12:16.000000 rushd-0.4.1/tests/test_pandas_cache.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)     4845 2023-06-02 21:07:49.000000 rushd-0.4.1/tests/test_plot.py
--rw-r--r--   0 christopher  (1000) christopher  (1000)     3274 2023-02-02 22:12:16.000000 rushd-0.4.1/tests/test_well_mapper.py
+drwxr-xr-x   0 kaseylove   (501) staff       (20)        0 2023-07-27 22:21:58.528868 rushd-0.4.2/
+-rw-r--r--   0 kaseylove   (501) staff       (20)     1069 2022-01-21 15:10:03.000000 rushd-0.4.2/LICENSE
+-rw-r--r--   0 kaseylove   (501) staff       (20)     3962 2023-07-27 22:21:58.528437 rushd-0.4.2/PKG-INFO
+-rw-r--r--   0 kaseylove   (501) staff       (20)     2994 2023-07-27 21:59:34.000000 rushd-0.4.2/README.md
+-rw-r--r--   0 kaseylove   (501) staff       (20)      527 2023-03-01 18:01:20.000000 rushd-0.4.2/pyproject.toml
+-rw-r--r--   0 kaseylove   (501) staff       (20)       38 2023-07-27 22:21:58.528993 rushd-0.4.2/setup.cfg
+-rw-r--r--   0 kaseylove   (501) staff       (20)     1885 2023-07-27 22:21:23.000000 rushd-0.4.2/setup.py
+drwxr-xr-x   0 kaseylove   (501) staff       (20)        0 2023-07-27 22:21:58.510642 rushd-0.4.2/src/
+drwxr-xr-x   0 kaseylove   (501) staff       (20)        0 2023-07-27 22:21:58.517656 rushd-0.4.2/src/rushd/
+-rw-r--r--   0 kaseylove   (501) staff       (20)      651 2023-07-26 21:44:53.000000 rushd-0.4.2/src/rushd/__init__.py
+-rw-r--r--   0 kaseylove   (501) staff       (20)    15035 2023-07-26 21:44:53.000000 rushd-0.4.2/src/rushd/flow.py
+-rw-r--r--   0 kaseylove   (501) staff       (20)    11323 2023-07-26 21:44:53.000000 rushd-0.4.2/src/rushd/io.py
+-rw-r--r--   0 kaseylove   (501) staff       (20)     9791 2023-07-27 21:47:05.000000 rushd-0.4.2/src/rushd/plot.py
+-rw-r--r--   0 kaseylove   (501) staff       (20)     6268 2023-07-26 21:44:53.000000 rushd-0.4.2/src/rushd/well_mapper.py
+drwxr-xr-x   0 kaseylove   (501) staff       (20)        0 2023-07-27 22:21:58.522591 rushd-0.4.2/src/rushd.egg-info/
+-rw-r--r--   0 kaseylove   (501) staff       (20)     3962 2023-07-27 22:21:58.000000 rushd-0.4.2/src/rushd.egg-info/PKG-INFO
+-rw-r--r--   0 kaseylove   (501) staff       (20)      440 2023-07-27 22:21:58.000000 rushd-0.4.2/src/rushd.egg-info/SOURCES.txt
+-rw-r--r--   0 kaseylove   (501) staff       (20)        1 2023-07-27 22:21:58.000000 rushd-0.4.2/src/rushd.egg-info/dependency_links.txt
+-rw-r--r--   0 kaseylove   (501) staff       (20)      210 2023-07-27 22:21:58.000000 rushd-0.4.2/src/rushd.egg-info/requires.txt
+-rw-r--r--   0 kaseylove   (501) staff       (20)        6 2023-07-27 22:21:58.000000 rushd-0.4.2/src/rushd.egg-info/top_level.txt
+drwxr-xr-x   0 kaseylove   (501) staff       (20)        0 2023-07-27 22:21:58.527781 rushd-0.4.2/tests/
+-rw-r--r--   0 kaseylove   (501) staff       (20)    11898 2023-03-01 18:01:20.000000 rushd-0.4.2/tests/test_file_io.py
+-rw-r--r--   0 kaseylove   (501) staff       (20)     3607 2023-03-01 18:01:20.000000 rushd-0.4.2/tests/test_file_moi.py
+-rw-r--r--   0 kaseylove   (501) staff       (20)    18337 2023-03-01 18:03:58.000000 rushd-0.4.2/tests/test_flow.py
+-rw-r--r--   0 kaseylove   (501) staff       (20)      891 2023-03-01 18:01:20.000000 rushd-0.4.2/tests/test_pandas_cache.py
+-rw-r--r--   0 kaseylove   (501) staff       (20)     5431 2023-07-27 17:35:52.000000 rushd-0.4.2/tests/test_plot.py
+-rw-r--r--   0 kaseylove   (501) staff       (20)     3274 2023-03-01 18:01:20.000000 rushd-0.4.2/tests/test_well_mapper.py
```

### Comparing `rushd-0.4.1/LICENSE` & `rushd-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rushd-0.4.1/PKG-INFO` & `rushd-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rushd
-Version: 0.4.1
+Version: 0.4.2
 Summary: Package for maintaining robust, reproducible data management.
 Home-page: https://github.com/GallowayLabMIT/rushd
 Author: Christopher Johnstone, Kasey Love, Conrad Oakes
 Author-email: meson800@gmail.com
 Project-URL: Bug Tracker, https://github.com/GallowayLabMIT/rushd/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -68,20 +68,20 @@
 ```
 After this 'local install', you can use and import `rushd` freely without
 having to re-install after each update.
 
 ## Changelog
 See the [CHANGELOG](CHANGELOG.md) for detailed changes.
 ```
+## [0.4.2] - 2023-07-27
+### Added
+- `rd.plot.generate_xticklabels` replaces a plot's existing xticklabels with specified metadata in a table-like format
 ## [0.4.1] - 2023-06-27
 ### Modified
 - Updated the `rd.plot.plot_mapping` command to properly handle the single-numeric case.
-## [0.4.0] - 2023-04-21
-### Added
-- `rd.plot.plot_well_metadata` to make nice plots corresponding to well metadata specified as a YAML file.
 ```
 
 ## License
 This is licensed by the MIT license. Use freely!
 
 ## What does the name mean?
 The name is a reference to [Ibn Rushd](https://en.wikipedia.org/wiki/Averroes), a Muslim scholar born in Córdoba who was responsible for translating and adding scholastic commentary to ancient Greek works, especially Aristotle. His translations spurred further translations into Latin and Hebrew, reigniting interest in ancient Greek works for the first time since the fall of the Roman empire.
```

### Comparing `rushd-0.4.1/README.md` & `rushd-0.4.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -44,20 +44,20 @@
 ```
 After this 'local install', you can use and import `rushd` freely without
 having to re-install after each update.
 
 ## Changelog
 See the [CHANGELOG](CHANGELOG.md) for detailed changes.
 ```
+## [0.4.2] - 2023-07-27
+### Added
+- `rd.plot.generate_xticklabels` replaces a plot's existing xticklabels with specified metadata in a table-like format
 ## [0.4.1] - 2023-06-27
 ### Modified
 - Updated the `rd.plot.plot_mapping` command to properly handle the single-numeric case.
-## [0.4.0] - 2023-04-21
-### Added
-- `rd.plot.plot_well_metadata` to make nice plots corresponding to well metadata specified as a YAML file.
 ```
 
 ## License
 This is licensed by the MIT license. Use freely!
 
 ## What does the name mean?
 The name is a reference to [Ibn Rushd](https://en.wikipedia.org/wiki/Averroes), a Muslim scholar born in Córdoba who was responsible for translating and adding scholastic commentary to ancient Greek works, especially Aristotle. His translations spurred further translations into Latin and Hebrew, reigniting interest in ancient Greek works for the first time since the fall of the Roman empire.
```

### Comparing `rushd-0.4.1/pyproject.toml` & `rushd-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rushd-0.4.1/setup.py` & `rushd-0.4.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rushd",
-    version="0.4.1",
+    version="0.4.2",
     author="Christopher Johnstone, Kasey Love, Conrad Oakes",
     author_email="meson800@gmail.com",
     description="Package for maintaining robust, reproducible data management.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GallowayLabMIT/rushd",
     project_urls={
```

### Comparing `rushd-0.4.1/src/rushd/__init__.py` & `rushd-0.4.2/src/rushd/__init__.py`

 * *Files identical despite different names*

### Comparing `rushd-0.4.1/src/rushd/flow.py` & `rushd-0.4.2/src/rushd/flow.py`

 * *Files identical despite different names*

### Comparing `rushd-0.4.1/src/rushd/io.py` & `rushd-0.4.2/src/rushd/io.py`

 * *Files identical despite different names*

### Comparing `rushd-0.4.1/src/rushd/plot.py` & `rushd-0.4.2/src/rushd/plot.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 except ImportError:
     from typing_extensions import Literal
 
 import matplotlib
 import matplotlib.figure
 import matplotlib.pyplot as plt
 import numpy as np
+import pandas as pd
 
 from . import flow
 
 WellMappingStyle = Union[Literal["category"], Literal["linear"], Literal["log"], Dict[str, Any]]
 
 
 def plot_mapping(
@@ -118,15 +119,15 @@
         well = row_str[row] + str(col + 1)
 
         ax.add_patch(
             plt.Circle(
                 (col, -row),
                 0.45,
                 ec="k",
-                fc=mapping_colors[mapping[well]] if well in mapping else None,
+                fc=mapping_colors[mapping[well]] if well in mapping else "#00000000",
             )
         )
     # Create the legend
     legend_entries = [
         plt.Circle((0, 0), 0.45, ec="k", fc=color) for color in mapping_colors.values()
     ]
     ax.legend(legend_entries, mapping_colors.keys(), loc="center left", bbox_to_anchor=(1, 0.5))
@@ -175,7 +176,91 @@
         if output_dir is None:
             plt.show()
         else:
             plt.savefig(output_dir / f"{column}.png", bbox_inches="tight")
             plt.savefig(output_dir / f"{column}.svg", bbox_inches="tight")
             plt.savefig(output_dir / f"{column}.pdf", bbox_inches="tight")
         plt.close()
+
+
+def generate_xticklabels(
+    df_labels: pd.DataFrame,
+    ax_col,
+    label_cols: List,
+    *,
+    ax: Optional[matplotlib.axes.Axes] = None,
+    align_ticklabels: Optional[
+        Union[Literal["left"], Literal["center"], Literal["right"]]
+    ] = "center",
+    align_annotation: Optional[
+        Union[Literal["left"], Literal["center"], Literal["right"]]
+    ] = "right",
+):
+    """
+    Create table-like x-axis tick labels based on provided metadata.
+
+    Parameters
+    ----------
+    df_labels: Pandas DataFrame
+        DataFrame of metadata related to original xticklabels. Columns are metadata values,
+        including the x-axis value.
+    ax_col:
+        Column of 'df_labels' that contains the original xticklabels. For seaborn plots, this
+        should be equivalent to the column passed to the x variable.
+    label_cols:
+        List of columns of 'df_labels' to use to replace the xticklabels.
+    ax: Optional Matplotlib axes
+        Axes to edit, uses current axes if none specified.
+    align_ticklabels: 'left', 'center', or 'right'
+        Text alignment for multi-line xticklabels.
+    align_annotation: 'left', 'center', or 'right'
+        Text alignment for multi-line annotations comprising the columns of 'df_labels' used to
+        replace the xticklabels. These appear to the bottom left of the plot, with the bounding
+        box right-aligned with the right of the yticklabels and aligned vertically center with
+        the vertical center of the xticklabels.
+
+    Returns
+    -------
+    None; modifies the axes in place.
+
+    """
+    # Draw plotting canvas to generate original xticklabels
+    if ax is None:
+        ax = plt.gca()
+    ax.figure.canvas.draw()
+
+    # Create dictionary from DataFrame, where keys are original xticklabels
+    #  and values are dictionaries of (metadata_key, metadata_value) pairs
+    dict_labels_by_xticklabel = df_labels.set_index(ax_col).to_dict(orient="index")
+
+    # Loop over xticklabels and set new values
+    ax_labels = []
+    for item in ax.get_xticklabels():
+        dict_labels = dict_labels_by_xticklabel[item.get_text()]
+
+        # For each specified metadata key (label_cols), get the metadata value
+        #  and concatenate all values into separate lines of a single string
+        new_xticklabel = "\n".join([str(dict_labels[i]) for i in label_cols])
+        ax_labels.append(new_xticklabel)
+
+    ax.set_xticks(ax.get_xticks(), ax_labels, multialignment=align_ticklabels)
+
+    # Get Artists for first axes labels
+    xlabel_bbox = ax.get_xticklabels()[0]
+    ylabel_bbox = ax.get_yticklabels()[0]
+
+    font_size = plt.rcParams["xtick.labelsize"]
+
+    # Annotate plot with metadata keys
+    #   x value: align the right of the annotation bbox (ha='right')
+    #       with the right (x=1) of the ylabel bbox (xcoord=ylabel_bbox)
+    #   y value: align the vertical center of the annotation bbox (va='center')
+    #       with the vertical center (y=0.5) of the xlabel bbox (ycoord=xlabel_bbox)
+    ax.annotate(
+        text="\n".join(label_cols),
+        xy=(1, 0.5),
+        xycoords=(ylabel_bbox, xlabel_bbox),
+        ha="right",
+        va="center",
+        multialignment=align_annotation,
+        fontsize=font_size,
+    )
```

### Comparing `rushd-0.4.1/src/rushd/well_mapper.py` & `rushd-0.4.2/src/rushd/well_mapper.py`

 * *Files identical despite different names*

### Comparing `rushd-0.4.1/src/rushd.egg-info/PKG-INFO` & `rushd-0.4.2/src/rushd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rushd
-Version: 0.4.1
+Version: 0.4.2
 Summary: Package for maintaining robust, reproducible data management.
 Home-page: https://github.com/GallowayLabMIT/rushd
 Author: Christopher Johnstone, Kasey Love, Conrad Oakes
 Author-email: meson800@gmail.com
 Project-URL: Bug Tracker, https://github.com/GallowayLabMIT/rushd/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -68,20 +68,20 @@
 ```
 After this 'local install', you can use and import `rushd` freely without
 having to re-install after each update.
 
 ## Changelog
 See the [CHANGELOG](CHANGELOG.md) for detailed changes.
 ```
+## [0.4.2] - 2023-07-27
+### Added
+- `rd.plot.generate_xticklabels` replaces a plot's existing xticklabels with specified metadata in a table-like format
 ## [0.4.1] - 2023-06-27
 ### Modified
 - Updated the `rd.plot.plot_mapping` command to properly handle the single-numeric case.
-## [0.4.0] - 2023-04-21
-### Added
-- `rd.plot.plot_well_metadata` to make nice plots corresponding to well metadata specified as a YAML file.
 ```
 
 ## License
 This is licensed by the MIT license. Use freely!
 
 ## What does the name mean?
 The name is a reference to [Ibn Rushd](https://en.wikipedia.org/wiki/Averroes), a Muslim scholar born in Córdoba who was responsible for translating and adding scholastic commentary to ancient Greek works, especially Aristotle. His translations spurred further translations into Latin and Hebrew, reigniting interest in ancient Greek works for the first time since the fall of the Roman empire.
```

### Comparing `rushd-0.4.1/tests/test_file_io.py` & `rushd-0.4.2/tests/test_file_io.py`

 * *Files identical despite different names*

### Comparing `rushd-0.4.1/tests/test_file_moi.py` & `rushd-0.4.2/tests/test_file_moi.py`

 * *Files identical despite different names*

### Comparing `rushd-0.4.1/tests/test_flow.py` & `rushd-0.4.2/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `rushd-0.4.1/tests/test_pandas_cache.py` & `rushd-0.4.2/tests/test_pandas_cache.py`

 * *Files identical despite different names*

### Comparing `rushd-0.4.1/tests/test_plot.py` & `rushd-0.4.2/tests/test_plot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
 
 import matplotlib.pyplot as plt
+import pandas as pd
 import rushd.plot
 from pytest_mock import MockerFixture
 
 TEST_METADATA = """
 metadata:
     inducible_fluorophore:
         - TagBFP: A1-H9
@@ -15,14 +16,16 @@
     test_negative_linear:
         - -1: A1-H9
         - 2: A10-H12
     orientation:
         - tandem: A1-H3, A10-H12
         - convergent: A4-H6
         - divergent: A7-H9
+    test_empty:
+        - wells: A1-C4
     dox:
         - 0: A1-A12
         - 0.0000820: B1-B12
         - 0.0003248: C1-C12
         - 0.0012864: D1-D12
         - 0.0050940: E1-E12
         - 0.0201723: F1-F12
@@ -44,15 +47,15 @@
     show_mock.assert_called_once()
     show_mock.reset_mock()
     rushd.plot.plot_well_metadata(tmp_path / "metadata.yaml")
     show_mock.assert_called()
     out_path = tmp_path / "output"
     out_path.mkdir()
     rushd.plot.plot_well_metadata(tmp_path / "metadata.yaml", output_dir=out_path)
-    assert len(list(out_path.glob("*"))) == 5 * 3
+    assert len(list(out_path.glob("*"))) == 6 * 3
 
 
 def test_column_autodetection(tmp_path: Path):
     """
     Tests the autodetection of numerical and categorical columns, by comparing legend colors
     """
     with (tmp_path / "metadata.yaml").open("w") as meta_file:
@@ -128,7 +131,20 @@
 def test_single_entry_zero(tmp_path: Path):
     """Tests that single entries where max=min do not crash the plotter"""
     with (tmp_path / "metadata.yaml").open("w") as meta_file:
         meta_file.write("metadata:\n  foo:\n    - 0: A1-H6")
     mapping = rushd.flow.load_well_metadata(tmp_path / "metadata.yaml")
     rushd.plot.plot_mapping(mapping["foo"])
     plt.close()
+
+
+def test_generate_xticklabels():
+    """Tests that xticklabels are replaced as expected"""
+    df_labels = pd.DataFrame(
+        {"category": ["cat_A", "cat_B"], "metadata1": ["foo", "bar"], "metadata2": ["-", "+"]}
+    )
+    plt.plot(["cat_A", "cat_B"], [0, 1])
+    rushd.plot.generate_xticklabels(df_labels, "category", ["metadata1", "metadata2"])
+    new_labels = [item.get_text() for item in plt.gca().get_xticklabels()]
+    expected_labels = ["foo\n-", "bar\n+"]
+    plt.close()
+    assert new_labels == expected_labels
```

### Comparing `rushd-0.4.1/tests/test_well_mapper.py` & `rushd-0.4.2/tests/test_well_mapper.py`

 * *Files identical despite different names*


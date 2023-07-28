# Comparing `tmp/caloutils-0.0.1.tar.gz` & `tmp/caloutils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caloutils-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "caloutils-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `caloutils-0.0.1.tar` & `caloutils-0.0.3.tar`

### file list

```diff
@@ -1,44 +1,49 @@
--rw-r--r--   0        0        0      292 2023-07-26 11:57:30.963154 caloutils-0.0.1/.editorconfig
--rw-r--r--   0        0        0      320 2023-07-26 11:57:31.032914 caloutils-0.0.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0     1204 2023-07-26 11:57:30.993792 caloutils-0.0.1/.gitignore
--rw-r--r--   0        0        0      685 2023-07-26 12:06:00.272840 caloutils-0.0.1/.travis.yml
--rw-r--r--   0        0        0     3508 2023-07-28 08:12:56.174479 caloutils-0.0.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0       89 2023-07-26 11:57:30.972970 caloutils-0.0.1/HISTORY.rst
--rw-r--r--   0        0        0     1063 2023-07-26 11:59:58.844814 caloutils-0.0.1/LICENSE
--rw-r--r--   0        0        0      262 2023-07-26 11:57:30.991734 caloutils-0.0.1/MANIFEST.in
--rw-r--r--   0        0        0     2394 2023-07-26 11:59:58.845293 caloutils-0.0.1/Makefile
--rw-r--r--   0        0        0      931 2023-07-26 11:59:58.845720 caloutils-0.0.1/README.rst
--rw-r--r--   0        0        0      130 2023-07-26 11:59:58.846169 caloutils-0.0.1/caloutils/__init__.py
--rw-r--r--   0        0        0       19 2023-07-26 11:57:31.041876 caloutils-0.0.1/caloutils/caloutils.py
--rw-r--r--   0        0        0     1645 2023-07-13 15:22:58.683044 caloutils-0.0.1/caloutils/metrics/pca.py
--rw-r--r--   0        0        0     1288 2023-07-27 09:34:25.075862 caloutils-0.0.1/caloutils/metrics/postprocess.py
--rw-r--r--   0        0        0     4830 2023-07-26 16:01:01.161651 caloutils-0.0.1/caloutils/metrics/shower.py
--rw-r--r--   0        0        0      182 2023-07-11 09:44:02.111276 caloutils-0.0.1/caloutils/plotting/__init__.py
--rw-r--r--   0        0        0     1502 2023-07-12 12:02:07.227507 caloutils-0.0.1/caloutils/plotting/binborders.py
--rw-r--r--   0        0        0     1287 2023-07-18 14:11:03.118006 caloutils-0.0.1/caloutils/plotting/hist1d.py
--rw-r--r--   0        0        0     3409 2023-07-18 17:04:43.626171 caloutils-0.0.1/caloutils/plotting/hist2d.py
--rw-r--r--   0        0        0     1546 2023-07-13 09:37:50.325838 caloutils-0.0.1/caloutils/plotting/infolut.py
--rw-r--r--   0        0        0     3098 2023-07-18 13:55:31.201586 caloutils-0.0.1/caloutils/plotting/ratioplot.py
--rw-r--r--   0        0        0     1361 2023-07-19 16:10:01.233027 caloutils-0.0.1/caloutils/processing/alpharot.py
--rw-r--r--   0        0        0      945 2023-07-13 20:31:17.248962 caloutils-0.0.1/caloutils/processing/convcoord.py
--rw-r--r--   0        0        0     1758 2023-07-25 11:29:09.808698 caloutils-0.0.1/caloutils/processing/dequantscaler.py
--rw-r--r--   0        0        0     2148 2023-07-17 07:58:56.085446 caloutils-0.0.1/caloutils/processing/idxscale.py
--rw-r--r--   0        0        0     3185 2023-07-19 13:11:32.819398 caloutils-0.0.1/caloutils/processing/objcol.py
--rw-r--r--   0        0        0     1565 2023-07-03 15:49:45.719972 caloutils-0.0.1/caloutils/processing/seq.py
--rw-r--r--   0        0        0     7377 2023-07-25 12:16:19.196884 caloutils-0.0.1/caloutils/processing/voxelize.py
--rw-r--r--   0        0        0      610 2023-07-26 11:57:31.012714 caloutils-0.0.1/docs/Makefile
--rw-r--r--   0        0        0       28 2023-07-26 11:57:31.023907 caloutils-0.0.1/docs/authors.rst
--rwxr-xr-x   0        0        0     4780 2023-07-26 11:59:58.846724 caloutils-0.0.1/docs/conf.py
--rw-r--r--   0        0        0       33 2023-07-26 11:57:31.025132 caloutils-0.0.1/docs/contributing.rst
--rw-r--r--   0        0        0       28 2023-07-26 11:57:31.021451 caloutils-0.0.1/docs/history.rst
--rw-r--r--   0        0        0      306 2023-07-26 11:57:31.010408 caloutils-0.0.1/docs/index.rst
--rw-r--r--   0        0        0     1114 2023-07-26 11:59:58.847191 caloutils-0.0.1/docs/installation.rst
--rw-r--r--   0        0        0      807 2023-07-26 11:57:31.027205 caloutils-0.0.1/docs/make.bat
--rw-r--r--   0        0        0       27 2023-07-26 11:57:31.022677 caloutils-0.0.1/docs/readme.rst
--rw-r--r--   0        0        0       73 2023-07-26 11:57:31.019832 caloutils-0.0.1/docs/usage.rst
--rw-r--r--   0        0        0     2762 2023-07-28 08:56:57.521233 caloutils-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       39 2023-07-26 11:57:31.007880 caloutils-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      397 2023-07-26 11:59:58.848546 caloutils-0.0.1/tests/test_caloutils.py
--rw-r--r--   0        0        0     5386 2023-07-25 11:39:08.539980 caloutils-0.0.1/tests/voxelize.py
--rw-r--r--   0        0        0      230 2023-07-28 08:16:45.615705 caloutils-0.0.1/tox.ini
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 caloutils-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      305 2023-07-28 14:47:00.347636 caloutils-0.0.3/.bumpversion.cfg
+-rw-r--r--   0        0        0      292 2023-07-28 14:47:00.347636 caloutils-0.0.3/.editorconfig
+-rw-r--r--   0        0        0      320 2023-07-28 14:47:00.347636 caloutils-0.0.3/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0     1036 2023-07-28 14:47:00.347636 caloutils-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     3078 2023-07-28 14:47:00.347636 caloutils-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1122 2023-07-28 14:47:00.347636 caloutils-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      728 2023-07-28 14:47:00.347636 caloutils-0.0.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      685 2023-07-28 14:47:00.347636 caloutils-0.0.3/.travis.yml
+-rw-r--r--   0        0        0     3517 2023-07-28 14:47:00.347636 caloutils-0.0.3/CONTRIBUTING.rst
+-rw-r--r--   0        0        0       89 2023-07-28 14:47:00.347636 caloutils-0.0.3/HISTORY.rst
+-rw-r--r--   0        0        0     1062 2023-07-28 14:47:00.347636 caloutils-0.0.3/LICENSE
+-rw-r--r--   0        0        0      262 2023-07-28 14:47:00.347636 caloutils-0.0.3/MANIFEST.in
+-rw-r--r--   0        0        0      928 2023-07-28 14:47:00.347636 caloutils-0.0.3/Makefile
+-rw-r--r--   0        0        0      937 2023-07-28 14:47:00.347636 caloutils-0.0.3/README.rst
+-rw-r--r--   0        0        0      610 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/Makefile
+-rw-r--r--   0        0        0       28 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/authors.rst
+-rwxr-xr-x   0        0        0     4787 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/conf.py
+-rw-r--r--   0        0        0       33 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/contributing.rst
+-rw-r--r--   0        0        0       28 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/history.rst
+-rw-r--r--   0        0        0      306 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/index.rst
+-rw-r--r--   0        0        0     1126 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/installation.rst
+-rw-r--r--   0        0        0      807 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/make.bat
+-rw-r--r--   0        0        0       27 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/readme.rst
+-rw-r--r--   0        0        0       73 2023-07-28 14:47:00.347636 caloutils-0.0.3/docs/usage.rst
+-rw-r--r--   0        0        0     2431 2023-07-28 14:47:00.347636 caloutils-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      143 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/caloutils.py
+-rw-r--r--   0        0        0     1644 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/metrics/pca.py
+-rw-r--r--   0        0        0     1287 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/metrics/postprocess.py
+-rw-r--r--   0        0        0     4829 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/metrics/shower.py
+-rw-r--r--   0        0        0      182 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/plotting/__init__.py
+-rw-r--r--   0        0        0     1501 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/plotting/binborders.py
+-rw-r--r--   0        0        0     1286 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/plotting/hist1d.py
+-rw-r--r--   0        0        0     3408 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/plotting/hist2d.py
+-rw-r--r--   0        0        0     1545 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/plotting/infolut.py
+-rw-r--r--   0        0        0     3097 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/plotting/ratioplot.py
+-rw-r--r--   0        0        0     1360 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/processing/alpharot.py
+-rw-r--r--   0        0        0      945 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/processing/convcoord.py
+-rw-r--r--   0        0        0     1758 2023-07-28 14:47:00.347636 caloutils-0.0.3/src/processing/dequantscaler.py
+-rw-r--r--   0        0        0     2148 2023-07-28 14:47:00.351636 caloutils-0.0.3/src/processing/idxscale.py
+-rw-r--r--   0        0        0     3184 2023-07-28 14:47:00.351636 caloutils-0.0.3/src/processing/objcol.py
+-rw-r--r--   0        0        0     1564 2023-07-28 14:47:00.351636 caloutils-0.0.3/src/processing/seq.py
+-rw-r--r--   0        0        0     7376 2023-07-28 14:47:00.351636 caloutils-0.0.3/src/processing/voxelize.py
+-rw-r--r--   0        0        0       39 2023-07-28 14:47:00.351636 caloutils-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      364 2023-07-28 14:47:00.351636 caloutils-0.0.3/tests/test_caloutils.py
+-rw-r--r--   0        0        0     5385 2023-07-28 14:47:00.351636 caloutils-0.0.3/tests/voxelize.py
+-rw-r--r--   0        0        0      230 2023-07-28 14:47:00.351636 caloutils-0.0.3/tox.ini
+-rwxr-xr-x   0        0        0      318 2023-07-28 14:47:00.351636 caloutils-0.0.3/venv_setup.sh
+-rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 caloutils-0.0.3/PKG-INFO
```

### Comparing `caloutils-0.0.1/.travis.yml` & `caloutils-0.0.3/.travis.yml`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.1/CONTRIBUTING.rst` & `caloutils-0.0.3/CONTRIBUTING.rst`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Types of Contributions
 ----------------------
 
 Report Bugs
 ~~~~~~~~~~~
 
-Report bugs at https://github.com/mova/caloutils/issues.
+Report bugs at https://github.com/DeGeSim/caloutils/issues.
 
 If you are reporting a bug, please include:
 
 * Your operating system name and version.
 * Any details about your local setup that might be helpful in troubleshooting.
 * Detailed steps to reproduce the bug.
 
@@ -41,15 +41,15 @@
 caloutils could always use more documentation, whether as part of the
 official caloutils docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 Submit Feedback
 ~~~~~~~~~~~~~~~
 
-The best way to send feedback is to file an issue at https://github.com/mova/caloutils/issues.
+The best way to send feedback is to file an issue at https://github.com/DeGeSim/caloutils/issues.
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
 * Keep the scope as narrow as possible, to make it easier to implement.
 * Remember that this is a volunteer-driven project, and that contributions
   are welcome :)
@@ -99,15 +99,15 @@
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
 3. The pull request should work for Python >= 3.10. Check
-   https://travis-ci.com/mova/caloutils/pull_requests
+   https://travis-ci.com/DeGeSim/caloutils/pull_requests
    and make sure that the tests pass for all supported Python versions.
 
 Tips
 ----
 
 To run a subset of tests::
```

### Comparing `caloutils-0.0.1/LICENSE` & `caloutils-0.0.3/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
```

### Comparing `caloutils-0.0.1/README.rst` & `caloutils-0.0.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 caloutils
 =========
 
 
 .. image:: https://img.shields.io/pypi/v/caloutils.svg
         :target: https://pypi.python.org/pypi/caloutils
 
-.. image:: https://img.shields.io/travis/mova/caloutils.svg
-        :target: https://travis-ci.com/mova/caloutils
+.. image:: https://img.shields.io/travis/DeGeSim/caloutils.svg
+        :target: https://travis-ci.com/DeGeSim/caloutils
 
 .. image:: https://readthedocs.org/projects/caloutils/badge/?version=latest
         :target: https://caloutils.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
```

### Comparing `caloutils-0.0.1/caloutils/metrics/pca.py` & `caloutils-0.0.3/src/metrics/pca.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import torch
+from fgsim.models.pool.std_pool import global_std_pool
 from torch_geometric.data import Batch
 from torch_geometric.nn.pool import global_mean_pool
 
-from fgsim.models.pool.std_pool import global_std_pool
-
 
 def fpc_from_batch(batch: Batch) -> dict[str, torch.Tensor]:
     """Get the first principal component from a PC"""
     batchidx = batch.batch
     xyz = batch.xyz.double()
     means = global_mean_pool(xyz, batchidx)
     stds = global_std_pool(xyz, batchidx)
```

### Comparing `caloutils-0.0.1/caloutils/metrics/postprocess.py` & `caloutils-0.0.3/src/metrics/postprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import torch
-from torch_geometric.data import Batch
-
 from fgsim.config import conf
+from torch_geometric.data import Batch
 
 from .convcoord import batch_to_Exyz
 from .pca import fpc_from_batch
 from .shower import analyze_layers, cyratio, response, sphereratio
 from .voxelize import sum_dublicate_hits
 
 alphapos = conf.loader.x_features.index("alpha")
```

### Comparing `caloutils-0.0.1/caloutils/metrics/shower.py` & `caloutils-0.0.3/src/metrics/shower.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import torch
+from fgsim.config import conf
 from torch_geometric.data import Batch
 from torch_geometric.nn.pool import (
     global_add_pool,
     global_max_pool,
     global_mean_pool,
 )
 from torch_scatter import scatter_std
 
-from fgsim.config import conf
-
 n_layers = 45
 
 
 def analyze_layers(batch: Batch) -> dict[str, torch.Tensor]:
     """Get the ratio between half-turnon and
     half turnoff to peak center from a PC"""
     batchidx = batch.batch
```

### Comparing `caloutils-0.0.1/caloutils/plotting/binborders.py` & `caloutils-0.0.3/src/plotting/binborders.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-
 from fgsim.utils.torchtonp import wrap_torch_to_np
 
 
 @wrap_torch_to_np
 def binborders_wo_outliers(points: np.ndarray, bins=50) -> np.ndarray:
     assert len(points.shape) == 1
     if len(np.unique(points[:500])) < 50:
```

### Comparing `caloutils-0.0.1/caloutils/plotting/hist1d.py` & `caloutils-0.0.3/src/plotting/hist1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Dict
 
-from matplotlib.figure import Figure
-
 from fgsim.config import conf
 from fgsim.plot.infolut import var_to_label
+from matplotlib.figure import Figure
 
 from .ratioplot import ratioplot
 
 
 def hist1d(
     sim, gen, ftxname: str, bins=None, energy_weighted=False
 ) -> Dict[str, Figure]:
```

### Comparing `caloutils-0.0.1/caloutils/plotting/hist2d.py` & `caloutils-0.0.3/src/plotting/hist2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from typing import Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
+from fgsim.plot.binborders import binborders_wo_outliers, chip_to_binborders
+from fgsim.utils.torchtonp import wrap_torch_to_np
 from matplotlib.axes import Axes
 from matplotlib.colors import LogNorm, Normalize
 from matplotlib.figure import Figure
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
-from fgsim.plot.binborders import binborders_wo_outliers, chip_to_binborders
-from fgsim.utils.torchtonp import wrap_torch_to_np
-
 np.set_printoptions(formatter={"float_kind": "{:.3g}".format})
 
 
 @wrap_torch_to_np
 def hist2d(
     sim: np.ndarray,
     gen: np.ndarray,
```

### Comparing `caloutils-0.0.1/caloutils/plotting/infolut.py` & `caloutils-0.0.3/src/plotting/infolut.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Dict, Optional, Union
 
 import numpy as np
-
 from fgsim.config import conf
 
 labels_dict: Dict[str, str] = {
     "etarel": "$\\eta_\\mathrm{rel}$",
     "phirel": "$\\phi_\\mathrm{rel}$",
     "ptrel": "$p^\\mathrm{T}_\\mathrm{rel}$",
     "mass": "$m_{rel}$",
```

### Comparing `caloutils-0.0.1/caloutils/plotting/ratioplot.py` & `caloutils-0.0.3/src/plotting/ratioplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from typing import Optional
 
 import matplotlib.pyplot as plt
 import mplhep
 import numpy as np
+from fgsim.utils.torchtonp import wrap_torch_to_np
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 
-from fgsim.utils.torchtonp import wrap_torch_to_np
-
 from .binborders import binborders_wo_outliers, bincenters
 
 
 @wrap_torch_to_np
 def ratioplot(
     sim: np.ndarray,
     gen: np.ndarray,
```

### Comparing `caloutils-0.0.1/caloutils/processing/alpharot.py` & `caloutils-0.0.3/src/processing/alpharot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import torch
-from torch_scatter import scatter_mean
-
 from fgsim.config import conf
 from fgsim.utils import check_tensor
+from torch_scatter import scatter_mean
 
 from .objcol import scaler
 
 
 def rotate_alpha(alphas, batchidx, fake=False, center=False):
     batch_size = int(batchidx[-1] + 1)
     alphapos = conf.loader.x_features.index("alpha")
```

### Comparing `caloutils-0.0.1/caloutils/processing/convcoord.py` & `caloutils-0.0.3/src/processing/convcoord.py`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.1/caloutils/processing/dequantscaler.py` & `caloutils-0.0.3/src/processing/dequantscaler.py`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.1/caloutils/processing/idxscale.py` & `caloutils-0.0.3/src/processing/idxscale.py`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.1/caloutils/processing/objcol.py` & `caloutils-0.0.3/src/processing/objcol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from pathlib import Path
 from typing import List, Tuple
 
 import h5py
 import numpy as np
 import torch
+from fgsim.config import conf
+from fgsim.io import FileManager, ScalerBase
+from fgsim.io.dequantscaler import dequant_stdscale
 from sklearn.pipeline import make_pipeline
 from sklearn.preprocessing import (
     FunctionTransformer,
     PowerTransformer,
     QuantileTransformer,
     StandardScaler,
 )
 from torch_geometric.data import Data
 
-from fgsim.config import conf
-from fgsim.io import FileManager, ScalerBase
-from fgsim.io.dequantscaler import dequant_stdscale
-
 
 def path_to_len(fn: Path) -> int:
     return len(h5py.File(fn, "r")["incident_energies"])
 
 
 file_manager = FileManager(
     path_to_len,
```

### Comparing `caloutils-0.0.1/caloutils/processing/seq.py` & `caloutils-0.0.3/src/processing/seq.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import List, Union
 
 import queueflow as qf
+from fgsim.config import conf
 from torch.multiprocessing import Queue, Value
 from torch_geometric.data import Batch, Data
 
-from fgsim.config import conf
-
 from .objcol import contruct_graph_from_row, read_chunks, scaler
 
 # Sharded switch for the postprocessing
 shared_postprocess_switch = Value("i", 0)
 shared_batch_size = Value("i", int(conf.loader.batch_size))
```

### Comparing `caloutils-0.0.1/caloutils/processing/voxelize.py` & `caloutils-0.0.3/src/processing/voxelize.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from math import prod
 
 import torch
-from torch_scatter import scatter_add
-
 from fgsim.config import conf, device
 from fgsim.io.batch_tools import fix_slice_dict_nodeattr
 from fgsim.utils.batch import ptr_from_batchidx
+from torch_scatter import scatter_add
 
 from .objcol import scaler
 
 num_z = 45
 num_alpha = 16
 num_r = 9
 dims = [num_z, num_alpha, num_r]
```

### Comparing `caloutils-0.0.1/docs/Makefile` & `caloutils-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.1/docs/conf.py` & `caloutils-0.0.3/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,42 +15,43 @@
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 import os
 import sys
-sys.path.insert(0, os.path.abspath('..'))
+
+sys.path.insert(0, os.path.abspath(".."))
 
 import caloutils
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
+extensions = ["sphinx.ext.autodoc", "sphinx.ext.viewcode"]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = 'caloutils'
+project = "caloutils"
 copyright = "2023, mova"
 author = "mova"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
@@ -65,98 +66,89 @@
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 
 # -- Options for HTMLHelp output ---------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'caloutilsdoc'
+htmlhelp_basename = "caloutilsdoc"
 
 
 # -- Options for LaTeX output ------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'caloutils.tex',
-     'caloutils Documentation',
-     'mova', 'manual'),
+    (master_doc, "caloutils.tex", "caloutils Documentation", "mova", "manual"),
 ]
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'caloutils',
-     'caloutils Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "caloutils", "caloutils Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'caloutils',
-     'caloutils Documentation',
-     author,
-     'caloutils',
-     'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "caloutils",
+        "caloutils Documentation",
+        author,
+        "caloutils",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
-
-
-
```

### Comparing `caloutils-0.0.1/docs/installation.rst` & `caloutils-0.0.3/docs/installation.rst`

 * *Files 10% similar despite different names*

```diff
@@ -28,24 +28,24 @@
 
 The sources for caloutils can be downloaded from the `Github repo`_.
 
 You can either clone the public repository:
 
 .. code-block:: console
 
-    $ git clone git://github.com/mova/caloutils
+    $ git clone git://github.com/DeGeSim/caloutils
 
 Or download the `tarball`_:
 
 .. code-block:: console
 
-    $ curl -OJL https://github.com/mova/caloutils/tarball/master
+    $ curl -OJL https://github.com/DeGeSim/caloutils/tarball/master
 
 Once you have a copy of the source, you can install it with:
 
 .. code-block:: console
 
     $ python setup.py install
 
 
-.. _Github repo: https://github.com/mova/caloutils
-.. _tarball: https://github.com/mova/caloutils/tarball/master
+.. _Github repo: https://github.com/DeGeSim/caloutils
+.. _tarball: https://github.com/DeGeSim/caloutils/tarball/master
```

### Comparing `caloutils-0.0.1/docs/make.bat` & `caloutils-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `caloutils-0.0.1/pyproject.toml` & `caloutils-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 [project]
 name = "caloutils"
-version = "0.0.1"
+version = '0.0.3'
 authors = [
   { name="mova", email="mova@users.noreply.github.com" },
   { name="kaechb", email="kaechb@users.noreply.github.com" },
 ]
 description = "Metrics and tools for evaluation generative models for calorimeter shower based on pytorch_geometric."
 requires-python = ">=3.8"
 readme="README.rst"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
+    "torch>=2.0.0",
     "torch_geometric>=2.3.0",
-    "torch-scatter>=2.1.1"
+    "torch-scatter>=2.1.1",
 ]
 [project.optional-dependencies]
-test = [
-    "pytest >=2.7.3",
-    "pytest-cov",
+dev = [
+  "pytest >=2.7.3",
+  "pytest-cov",
+  "bump2version",
+  "black",
+  "pre-commit",
+  "ruff",
 ]
 doc = ["sphinx"]
 
 
 [project.urls]
 "Homepage" = "https://github.com/DeGeSim/caloutils"
 "Bug Tracker" = "https://github.com/DeGeSim/caloutils/issues"
@@ -34,37 +39,16 @@
 
 
 
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = [
   "flit_core >=3.2,<4",
-  "ruff>=0.0.280",
-  "black==21.7b0",
 ]
 
-[tool.bdist_wheel]
-universal = 1
-
-
-# [tool.bumpversion]
-# current_version = 0.1.0
-# commit = True
-# tag = True
-
-# [tool.bumpversion:file:setup.py]
-# search = version='{current_version}'
-# replace = version='{new_version}'
-
-# [tool.bumpversion:file:caloutils/__init__.py]
-# search = __version__ = '{current_version}'
-# replace = __version__ = '{new_version}'
-
-
-
 
 [tool.pytest.ini_options]
 python_files = "*.py"
 testpaths = [
   "tests",
 ]
 #--ignore=E203,E302
@@ -146,10 +130,7 @@
     "node_modules",
     "venv",
 ]
 target-version = "py310"
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402","F401"]
-
-
-
```

### Comparing `caloutils-0.0.1/tests/voxelize.py` & `caloutils-0.0.3/tests/voxelize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # %%
 import numpy as np
 import torch
+from fgsim.config import compute_conf, conf
 from torch_geometric.data import Batch
 from tqdm import tqdm
 
-from fgsim.config import compute_conf, conf
-
 compute_conf(conf, {"dataset_name": "calochallange", "command": "test"})
 step = 1_000
 conf.loader.scaling_fit_size //= 10
 conf.loader.batch_size = step
 
 from fgsim.io.dequantscaler import (  # noqa: E402
     FunctionTransformer,
```

### Comparing `caloutils-0.0.1/PKG-INFO` & `caloutils-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 Metadata-Version: 2.1
 Name: caloutils
-Version: 0.0.1
+Version: 0.0.3
 Summary: Metrics and tools for evaluation generative models for calorimeter shower based on pytorch_geometric.
 Author-email: mova <mova@users.noreply.github.com>, kaechb <kaechb@users.noreply.github.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Dist: torch>=2.0.0
 Requires-Dist: torch_geometric>=2.3.0
 Requires-Dist: torch-scatter>=2.1.1
+Requires-Dist: pytest >=2.7.3 ; extra == "dev"
+Requires-Dist: pytest-cov ; extra == "dev"
+Requires-Dist: bump2version ; extra == "dev"
+Requires-Dist: black ; extra == "dev"
+Requires-Dist: pre-commit ; extra == "dev"
+Requires-Dist: ruff ; extra == "dev"
 Requires-Dist: sphinx ; extra == "doc"
-Requires-Dist: pytest >=2.7.3 ; extra == "test"
-Requires-Dist: pytest-cov ; extra == "test"
 Project-URL: Bug Tracker, https://github.com/DeGeSim/caloutils/issues
 Project-URL: Homepage, https://github.com/DeGeSim/caloutils
+Provides-Extra: dev
 Provides-Extra: doc
-Provides-Extra: test
 
 =========
 caloutils
 =========
 
 
 .. image:: https://img.shields.io/pypi/v/caloutils.svg
         :target: https://pypi.python.org/pypi/caloutils
 
-.. image:: https://img.shields.io/travis/mova/caloutils.svg
-        :target: https://travis-ci.com/mova/caloutils
+.. image:: https://img.shields.io/travis/DeGeSim/caloutils.svg
+        :target: https://travis-ci.com/DeGeSim/caloutils
 
 .. image:: https://readthedocs.org/projects/caloutils/badge/?version=latest
         :target: https://caloutils.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
```


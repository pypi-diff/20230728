# Comparing `tmp/sympy_plot_backends-2.4.2.tar.gz` & `tmp/sympy_plot_backends-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sympy_plot_backends-2.4.2.tar", last modified: Sun Jul  9 14:14:03 2023, max compression
+gzip compressed data, was "sympy_plot_backends-2.4.3.tar", last modified: Fri Jul 28 10:02:02 2023, max compression
```

## Comparing `sympy_plot_backends-2.4.2.tar` & `sympy_plot_backends-2.4.3.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.649411 sympy_plot_backends-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-09 14:14:03.649411 sympy_plot_backends-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 14:14:03.649411 sympy_plot_backends-2.4.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2004 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.637410 sympy_plot_backends-2.4.2/spb/
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.637410 sympy_plot_backends-2.4.2/spb/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25407 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/base_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/base_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.637410 sympy_plot_backends-2.4.2/spb/backends/bokeh/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/bokeh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.637410 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/hvline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/line2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/vector2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.637410 sympy_plot_backends-2.4.2/spb/backends/k3d/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/k3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.637410 sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/complex.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/implicit3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/line3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/vector3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.641410 sympy_plot_backends-2.4.2/spb/backends/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24461 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/matplotlib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.641410 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/hvline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/implicit2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/line2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/line3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/nichols.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/nyquist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/vector2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/vector3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.641410 sympy_plot_backends-2.4.2/spb/backends/mayavi/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/mayavi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/mayavi/mayavi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.641410 sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/implicit3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/line3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/vector3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.641410 sympy_plot_backends-2.4.2/spb/backends/plotly/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19219 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.645411 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/hvline.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/implicit3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/line2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/line3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/vector2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/vector3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    21845 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.645411 sympy_plot_backends-2.4.2/spb/ccomplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/ccomplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78700 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/ccomplex/complex.py
--rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/ccomplex/wegert.py
--rw-r--r--   0 runner    (1001) docker     (123)    41127 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   179849 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.645411 sympy_plot_backends-2.4.2/spb/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/interactive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.645411 sympy_plot_backends-2.4.2/spb/interactive/bootstrap_spb/
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/interactive/bootstrap_spb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/interactive/bootstrap_spb/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/interactive/bootstrap_spb/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/interactive/ipywidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    39194 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/interactive/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/plotgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)   142578 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/series.py
--rw-r--r--   0 runner    (1001) docker     (123)    21641 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31071 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/vectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.645411 sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-09 14:14:03.000000 sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-09 14:14:03.000000 sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:14:03.000000 sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:14:03.000000 sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-09 14:14:03.000000 sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-09 14:14:03.000000 sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.645411 sympy_plot_backends-2.4.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.649411 sympy_plot_backends-2.4.2/tests/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23665 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/backends/make_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/backends/test_base_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    37300 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/backends/test_bokeh.py
--rw-r--r--   0 runner    (1001) docker     (123)    25876 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/backends/test_k3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    62918 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/backends/test_matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    55450 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/backends/test_plotly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_color_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    72837 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_complex.py
--rw-r--r--   0 runner    (1001) docker     (123)    34886 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    75888 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23636 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_plotgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)   117233 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    46627 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.517692 sympy_plot_backends-2.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-28 10:02:02.517692 sympy_plot_backends-2.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:02:02.517692 sympy_plot_backends-2.4.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2004 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.505692 sympy_plot_backends-2.4.3/spb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.505692 sympy_plot_backends-2.4.3/spb/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25395 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/base_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.505692 sympy_plot_backends-2.4.3/spb/backends/bokeh/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/bokeh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17883 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/bokeh/bokeh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.505692 sympy_plot_backends-2.4.3/spb/backends/bokeh/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/bokeh/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/bokeh/renderers/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/bokeh/renderers/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/bokeh/renderers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/bokeh/renderers/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/bokeh/renderers/hvline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/bokeh/renderers/line2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/bokeh/renderers/vector2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.505692 sympy_plot_backends-2.4.3/spb/backends/k3d/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/k3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/k3d/k3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.505692 sympy_plot_backends-2.4.3/spb/backends/k3d/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/k3d/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/k3d/renderers/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/k3d/renderers/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/k3d/renderers/implicit3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/k3d/renderers/line3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/k3d/renderers/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/k3d/renderers/vector3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.509692 sympy_plot_backends-2.4.3/spb/backends/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24461 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/matplotlib/matplotlib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.509692 sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/hvline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/implicit2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/line2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/line3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/nichols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/nyquist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/vector2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/vector3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.509692 sympy_plot_backends-2.4.3/spb/backends/mayavi/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/mayavi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/mayavi/mayavi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.509692 sympy_plot_backends-2.4.3/spb/backends/mayavi/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/mayavi/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/mayavi/renderers/implicit3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/mayavi/renderers/line3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/mayavi/renderers/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/mayavi/renderers/vector3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.509692 sympy_plot_backends-2.4.3/spb/backends/plotly/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19219 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/plotly/plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.513692 sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/hvline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/implicit3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/line2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/line3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/vector2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/vector3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21845 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/backends/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.513692 sympy_plot_backends-2.4.3/spb/ccomplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/ccomplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80690 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/ccomplex/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/ccomplex/wegert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41766 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/doc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179849 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.513692 sympy_plot_backends-2.4.3/spb/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/interactive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.513692 sympy_plot_backends-2.4.3/spb/interactive/bootstrap_spb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/interactive/bootstrap_spb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/interactive/bootstrap_spb/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/interactive/bootstrap_spb/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/interactive/ipywidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39202 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/interactive/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/plotgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143078 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21641 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31071 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/spb/vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.513692 sympy_plot_backends-2.4.3/sympy_plot_backends.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-28 10:02:02.000000 sympy_plot_backends-2.4.3/sympy_plot_backends.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-28 10:02:02.000000 sympy_plot_backends-2.4.3/sympy_plot_backends.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:02:02.000000 sympy_plot_backends-2.4.3/sympy_plot_backends.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:02:02.000000 sympy_plot_backends-2.4.3/sympy_plot_backends.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-28 10:02:02.000000 sympy_plot_backends-2.4.3/sympy_plot_backends.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 10:02:02.000000 sympy_plot_backends-2.4.3/sympy_plot_backends.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.517692 sympy_plot_backends-2.4.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:02.517692 sympy_plot_backends-2.4.3/tests/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/tests/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23665 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/tests/backends/make_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/tests/backends/test_base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37300 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/tests/backends/test_bokeh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25876 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/tests/backends/test_k3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62918 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/tests/backends/test_matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55450 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/tests/backends/test_plotly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/tests/test_color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72837 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/tests/test_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34886 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/tests/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/tests/test_doc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75888 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23636 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/tests/test_plotgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118098 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/tests/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46627 2023-07-28 10:01:53.000000 sympy_plot_backends-2.4.3/tests/test_vectors.py
```

### Comparing `sympy_plot_backends-2.4.2/LICENSE` & `sympy_plot_backends-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/PKG-INFO` & `sympy_plot_backends-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sympy_plot_backends
-Version: 2.4.2
+Version: 2.4.3
 Summary: Backends for plotting with SymPy
 Home-page: https://github.com/Davide-sd/sympy-plot-backends
 Author: Davide Sandona
 Author-email: sandona.davide@gmail.com
 License: BSD License
 Keywords: sympy plot plotting backend plotly bokeh mayavi k3d panel
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sympy_plot_backends-2.4.2/README.md` & `sympy_plot_backends-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/setup.py` & `sympy_plot_backends-2.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/__init__.py` & `sympy_plot_backends-2.4.3/spb/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/base_backend.py` & `sympy_plot_backends-2.4.3/spb/backends/base_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,17 +279,17 @@
         self.xlabel = kwargs.get("xlabel", None)
         self.ylabel = kwargs.get("ylabel", None)
         self.zlabel = kwargs.get("zlabel", None)
         self.aspect = kwargs.get("aspect", kwargs.get("aspect_ratio", "auto"))
         self.axis_center = kwargs.get("axis_center", None)
         self.camera = kwargs.get("camera", None)
         self.grid = kwargs.get("grid", True)
-        self.xscale = kwargs.get("xscale", "linear")
-        self.yscale = kwargs.get("yscale", "linear")
-        self.zscale = kwargs.get("zscale", "linear")
+        self.xscale = kwargs.get("xscale", None)
+        self.yscale = kwargs.get("yscale", None)
+        self.zscale = kwargs.get("zscale", None)
         self.polar_axis = kwargs.get("polar_axis", None)
         # NOTE: it would be nice to have detect_poles=True by default.
         # However, the correct detection also depends on the number of points
         # and the value of `eps`. Getting the detection right is likely to
         # be a trial-by-error procedure. Hence, keep this parameter to False.
         self.detect_poles = kwargs.get("detect_poles", False)
         # NOTE: matplotlib is not designed to be interactive, therefore it
```

### Comparing `sympy_plot_backends-2.4.2/spb/backends/base_renderer.py` & `sympy_plot_backends-2.4.3/spb/backends/base_renderer.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,22 +24,23 @@
         stored in ``handle`` with new numerical ``data``.
 
       Multiple key/value pairs can be added, all of which will receive the
       same numerical data. This allows to add different graphical elements
       to the same data series, in order to create more complex plots, promoting
       code reusability at the same time.
 
-    A renderer must implement these methods:
+    A renderer implements these methods:
 
     * `draw`: it will be called by ``plot`` when the figure is empty. This
       method extracts the numerical data from the ``series``, and sends it to
-      ``draw_method``.
+      each ``draw_method`` contained in ``draw_update_map``.
     * ``update``: it will be called by ``plot`` when the widgets change state.
       This method extracts the numerical data from the ``series``, and sends it
-      to ``update_method`` together with the appropriate ``handle``.
+      to each ``update_method`` contained in ``draw_update_map``, together
+      with the appropriate ``handle``.
     """
     draw_update_map = {}
 
     def __init__(self, plot, series):
         self.plot = plot if isinstance(plot, Plot) else plot.backend
         self.series = series
         self.handles = []
```

### Comparing `sympy_plot_backends-2.4.2/spb/backends/bokeh/bokeh.py` & `sympy_plot_backends-2.4.3/spb/backends/bokeh/bokeh.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,24 +189,26 @@
         kw = dict(
             title=title,
             x_axis_label=xlabel if xlabel else "x",
             y_axis_label=ylabel if ylabel else "y",
             sizing_mode="fixed" if self.size else sizing_mode,
             width=int(self.size[0]) if self.size else cfg["bokeh"]["width"],
             height=int(self.size[1]) if self.size else cfg["bokeh"]["height"],
-            x_axis_type=self.xscale,
-            y_axis_type=self.yscale,
             tools="pan,wheel_zoom,box_zoom,reset,hover,save",
             tooltips=TOOLTIPS,
             match_aspect=True if self.aspect == "equal" else False,
         )
         if self.xlim:
             kw["x_range"] = self.xlim
         if self.ylim:
             kw["y_range"] = self.ylim
+        if self.xscale:
+            kw["x_axis_type"] = self.xscale
+        if self.yscale:
+            kw["y_axis_type"] = self.yscale
         self._fig = self.bokeh.plotting.figure(**kw)
         self._fig.axis.visible = self.axis
         self.grid = kwargs.get("grid", cfg["bokeh"]["grid"])
         self._fig.grid.visible = self.grid
         if cfg["bokeh"]["show_minor_grid"]:
             self._fig.grid.minor_grid_line_alpha = cfg["bokeh"]["minor_grid_line_alpha"]
             self._fig.grid.minor_grid_line_color = self._fig.grid.grid_line_color[0]
```

### Comparing `sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/complex.py` & `sympy_plot_backends-2.4.3/spb/backends/bokeh/renderers/complex.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/contour.py` & `sympy_plot_backends-2.4.3/spb/backends/bokeh/renderers/contour.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/generic.py` & `sympy_plot_backends-2.4.3/spb/backends/bokeh/renderers/generic.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/geometry.py` & `sympy_plot_backends-2.4.3/spb/backends/bokeh/renderers/geometry.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/hvline.py` & `sympy_plot_backends-2.4.3/spb/backends/bokeh/renderers/hvline.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/line2d.py` & `sympy_plot_backends-2.4.3/spb/backends/bokeh/renderers/line2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/vector2d.py` & `sympy_plot_backends-2.4.3/spb/backends/bokeh/renderers/vector2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/k3d/k3d.py` & `sympy_plot_backends-2.4.3/spb/backends/k3d/k3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/complex.py` & `sympy_plot_backends-2.4.3/spb/backends/k3d/renderers/complex.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/implicit3d.py` & `sympy_plot_backends-2.4.3/spb/backends/k3d/renderers/implicit3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/line3d.py` & `sympy_plot_backends-2.4.3/spb/backends/k3d/renderers/line3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/surface.py` & `sympy_plot_backends-2.4.3/spb/backends/k3d/renderers/surface.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/vector3d.py` & `sympy_plot_backends-2.4.3/spb/backends/k3d/renderers/vector3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/matplotlib/matplotlib.py` & `sympy_plot_backends-2.4.3/spb/backends/matplotlib/matplotlib.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/__init__.py` & `sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/complex.py` & `sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/complex.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/contour.py` & `sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/contour.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/generic.py` & `sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/generic.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/geometry.py` & `sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/geometry.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/hvline.py` & `sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/hvline.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/implicit2d.py` & `sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/implicit2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/line2d.py` & `sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/line2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/line3d.py` & `sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/line3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/nichols.py` & `sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/nichols.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/nyquist.py` & `sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/nyquist.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/renderer.py` & `sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/renderer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from spb.backends.base_renderer import Renderer
 
 
 class MatplotlibRenderer(Renderer):
+    """A base class for renderers related to Matplotlib.
+    
+    Matplotlib is not really great at keeping track of axis limits when
+    Collections (LineCollection, PolyCollection, ...). This base class
+    implements the code to compute them.
+    """
     draw_update_map = {}
 
     # NOTE: matplotlib 3d plots (and also 2D plots containing LineCollection)
     # suffer from this problem:
     # https://github.com/matplotlib/matplotlib/issues/17130
     # Renderers that deals with Matplotlib's `*Collection` objects should
     # set this attribute to True, which is going to compute axis limits
```

### Comparing `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/surface.py` & `sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/surface.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/vector2d.py` & `sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/vector2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/vector3d.py` & `sympy_plot_backends-2.4.3/spb/backends/matplotlib/renderers/vector3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/mayavi/mayavi.py` & `sympy_plot_backends-2.4.3/spb/backends/mayavi/mayavi.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/implicit3d.py` & `sympy_plot_backends-2.4.3/spb/backends/mayavi/renderers/implicit3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/line3d.py` & `sympy_plot_backends-2.4.3/spb/backends/mayavi/renderers/line3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/surface.py` & `sympy_plot_backends-2.4.3/spb/backends/mayavi/renderers/surface.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/vector3d.py` & `sympy_plot_backends-2.4.3/spb/backends/mayavi/renderers/vector3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/plotly/plotly.py` & `sympy_plot_backends-2.4.3/spb/backends/plotly/plotly.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/__init__.py` & `sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/complex.py` & `sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/complex.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/contour.py` & `sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/contour.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/generic.py` & `sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/generic.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/geometry.py` & `sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/geometry.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/hvline.py` & `sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/hvline.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/implicit3d.py` & `sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/implicit3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/line2d.py` & `sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/line2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/line3d.py` & `sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/line3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/surface.py` & `sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/surface.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/vector2d.py` & `sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/vector2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/vector3d.py` & `sympy_plot_backends-2.4.3/spb/backends/plotly/renderers/vector3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/backends/utils.py` & `sympy_plot_backends-2.4.3/spb/backends/utils.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/ccomplex/complex.py` & `sympy_plot_backends-2.4.3/spb/ccomplex/complex.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,14 +523,70 @@
         Sets the scaling of the x-axis or y-axis, respectively.
         Default to ``'linear'``.
 
     xlim, ylim, zlim : (float, float), optional
         Denotes the x-axis limits, y-axis limits or z-axis limits,
         respectively, ``(min, max)``. ``zlim`` is only available for 3D plots.
 
+    Notes
+    =====
+
+    Given a symbolic expression, there are two possible way to create a
+    real/imag plot:
+
+    1. Apply Sympy's ``re`` or ``im`` to the symbolic expression, then
+       evaluates it.
+    2. Evaluates the symbolic expression over the provided range in order to
+       get complex values, then extract the real/imaginary parts with Numpy.
+
+    For performance reasons, ``plot_real_imag`` implements the second approach.
+    In fact, SymPy's ``re`` and ``im`` functions evaluate their arguments,
+    potentially creating unecessarely long symbolic expressions that requires
+    a lot of time to be evaluated.
+
+    Another thing to be aware of is branch cuts of complex-valued functions.
+    The plotting module attempt to evaluate a symbolic expression using complex
+    numbers. Depending on the evaluation module being used, we might get
+    different results. For example, the following two expressions should be
+    equal only when ``x > 0``. Instead, the plotting module gives us an
+    incorrect result:
+
+    .. plot::
+       :context: reset
+       :format: doctest
+       :include-source: True
+
+       >>> from sympy import symbols, im, Rational
+       >>> from spb import plot_real_imag, plot
+       >>> x = symbols('x')
+       >>> e1 = (1 / x)**(Rational(6, 5))
+       >>> e2 = x**(-Rational(6, 5))
+       >>> plot_real_imag((e1, "e1"), (e2, "e2"), real=False, ylim=(-5, 5))
+
+    We can force the evaluation to use only real numbers:
+
+    .. plot::
+       :context: close-figs
+       :format: doctest
+       :include-source: True
+
+       >>> plot_real_imag((e1, "e1"), (e2, "e2"), real=False, ylim=(-5, 5),
+       ...     force_real_eval=True)
+
+    This produced the correct visualization. Alternatively, we can evaluate
+    the expressions with mpmath:
+
+    .. plot::
+       :context: close-figs
+       :format: doctest
+       :include-source: True
+
+       >>> plot_real_imag((e1, "e1"), (e2, "e2"), real=False, ylim=(-5, 5),
+       ...     modules="mpmath")
+
 
     Examples
     ========
 
     .. plot::
        :context: reset
        :format: doctest
```

### Comparing `sympy_plot_backends-2.4.2/spb/ccomplex/wegert.py` & `sympy_plot_backends-2.4.3/spb/ccomplex/wegert.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/control.py` & `sympy_plot_backends-2.4.3/spb/control.py`

 * *Files 0% similar despite different names*

```diff
@@ -739,32 +739,48 @@
         If ``True``, the coordinate axes will be shown. Defaults to False.
     freq_unit : string, optional
         User can choose between ``'rad/sec'`` (radians/second) and ``'Hz'``
         (Hertz) as frequency units.
     phase_unit : string, optional
         User can choose between ``'rad'`` (radians) and ``'deg'`` (degree)
         as phase units.
+    unwrap : bool, optional
+        Depending on the transfer function, there could be discontinuities in
+        the phase plot. Set ``unwrap=True`` to get a continuous phase.
+        Default to False.
     **kwargs :
         See ``plot`` for a list of keyword arguments to further customize
         the resulting figure.
 
     Examples
     ========
 
     .. plot::
         :context: close-figs
         :format: doctest
         :include-source: True
 
         >>> from sympy.abc import s
         >>> from sympy.physics.control.lti import TransferFunction
-        >>> from spb import plot_bode
+        >>> from spb import plot_bode, plot_bode_phase, plotgrid
         >>> tf1 = TransferFunction(1*s**2 + 0.1*s + 7.5, 1*s**4 + 0.12*s**3 + 9*s**2, s)
         >>> plot_bode(tf1, initial_exp=0.2, final_exp=0.7)   # doctest: +SKIP
 
+    In this example it is necessary to unwrap the phase:
+
+    .. plot::
+        :context: close-figs
+        :format: doctest
+        :include-source: True
+
+        >>> TransferFunction(1, s**3 + 2*s**2 + s, s)
+        >>> p1 = plot_bode_phase(tf, unwrap=False, show=False, title="unwrap=False")
+        >>> p2 = plot_bode_phase(tf, unwrap=True, show=False, title="unwrap=True")
+        >>> plotgrid(p1, p2)
+
     Interactive-widget plot:
 
     .. panel-screenshot::
        :small-size: 800, 675
 
        from sympy.abc import a, b, c, d, e, f, s
        from sympy.physics.control.lti import TransferFunction
```

### Comparing `sympy_plot_backends-2.4.2/spb/defaults.py` & `sympy_plot_backends-2.4.3/spb/defaults.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/doc_utils.py` & `sympy_plot_backends-2.4.3/spb/doc_utils.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/functions.py` & `sympy_plot_backends-2.4.3/spb/functions.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/interactive/__init__.py` & `sympy_plot_backends-2.4.3/spb/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/interactive/bootstrap_spb/__init__.py` & `sympy_plot_backends-2.4.3/spb/interactive/bootstrap_spb/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/interactive/bootstrap_spb/bootstrap.css` & `sympy_plot_backends-2.4.3/spb/interactive/bootstrap_spb/bootstrap.css`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/interactive/bootstrap_spb/bootstrap.html` & `sympy_plot_backends-2.4.3/spb/interactive/bootstrap_spb/bootstrap.html`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/interactive/ipywidgets.py` & `sympy_plot_backends-2.4.3/spb/interactive/ipywidgets.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/interactive/panel.py` & `sympy_plot_backends-2.4.3/spb/interactive/panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -733,17 +733,17 @@
     showing the value in degrees on its label:
 
     .. panel-screenshot::
        :small-size: 800, 570
 
        from sympy import sin, pi, symbols
        from spb import *
-       from bokeh.models.formatters import FuncTickFormatter
+       from bokeh.models.formatters import CustomJSTickFormatter
        # Javascript code is passed to `code=`
-       formatter = FuncTickFormatter(code="return (180./3.1415926 * tick).toFixed(2)")
+       formatter = CustomJSTickFormatter(code="return (180./3.1415926 * tick).toFixed(2)")
        x, t = symbols("x, t")
 
        plot(
            (1 + x * sin(t), (x, -5, 5)),
            params = {
                t: (1, -2 * pi, 2 * pi, 100, formatter, "theta [deg]")
            },
```

### Comparing `sympy_plot_backends-2.4.2/spb/plotgrid.py` & `sympy_plot_backends-2.4.3/spb/plotgrid.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/series.py` & `sympy_plot_backends-2.4.3/spb/series.py`

 * *Files 1% similar despite different names*

```diff
@@ -1076,14 +1076,15 @@
         self.loss_fn = kwargs.get("loss_fn", None)
         self.use_cm = kwargs.get("use_cm", False)
         self.color_func = kwargs.get("color_func", None)
         self.line_color = kwargs.get("line_color", None)
         self.detect_poles = kwargs.get("detect_poles", False)
         self.eps = kwargs.get("eps", 0.01)
         self.is_polar = kwargs.get("is_polar", False)
+        self.unwrap = kwargs.get("unwrap", False)
         # when detect_poles="symbolic", stores the location of poles so that
         # they can be appropriately rendered
         self.poles_locations = []
         exclude = kwargs.get("exclude", [])
         if isinstance(exclude, Set):
             exclude = list(extract_solution(exclude, n=100))
         if not hasattr(exclude, "__iter__"):
@@ -1133,14 +1134,28 @@
                     x, y, self.eps)
                 points = (x, y)
             else:
                 x, y, p = points
                 x, y = _detect_poles_numerical_helper(x, y, self.eps)
                 points = (x, y, p)
 
+        if self.unwrap:
+            kw = {}
+            if self.unwrap is not True:
+                kw = self.unwrap
+            if self.is_2Dline:
+                if len(points) == 2:
+                    x, y = points
+                    y = np.unwrap(y, **kw)
+                    points = (x, y)
+                else:
+                    x, y, p = points
+                    y = np.unwrap(y, **kw)
+                    points = (x, y, p)
+
         if self.steps is True:
             if self.is_2Dline:
                 x, y = points[0], points[1]
                 x = np.array((x, x)).T.flatten()[1:]
                 y = np.array((y, y)).T.flatten()[:-1]
                 if self.is_parametric:
                     points = (x, y, points[2])
@@ -1349,15 +1364,15 @@
 class LineOver1DRangeSeries(Line2DBaseSeries):
     """Representation for a line consisting of a SymPy expression over a
     real range."""
 
     _allowed_keys = ["absarg", "adaptive", "adaptive_goal", "color_func",
     "detect_poles", "eps","is_complex", "is_filled", "is_point", "line_color",
     "loss_fn", "modules", "n", "only_integers", "rendering_kw", "steps",
-    "use_cm", "xscale", "tx", "ty", "tz", "is_polar", "exclude"]
+    "use_cm", "xscale", "tx", "ty", "tz", "is_polar", "exclude", "unwrap"]
 
     def __new__(cls, *args, **kwargs):
         if kwargs.get("absarg", False):
             return super().__new__(AbsArgLineSeries)
         cf = kwargs.get("color_func", None)
         if (callable(cf) or  callable(kwargs.get("line_color", None)) or
             isinstance(cf, Expr)):
```

### Comparing `sympy_plot_backends-2.4.2/spb/utils.py` & `sympy_plot_backends-2.4.3/spb/utils.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/spb/vectors.py` & `sympy_plot_backends-2.4.3/spb/vectors.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/PKG-INFO` & `sympy_plot_backends-2.4.3/sympy_plot_backends.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sympy-plot-backends
-Version: 2.4.2
+Version: 2.4.3
 Summary: Backends for plotting with SymPy
 Home-page: https://github.com/Davide-sd/sympy-plot-backends
 Author: Davide Sandona
 Author-email: sandona.davide@gmail.com
 License: BSD License
 Keywords: sympy plot plotting backend plotly bokeh mayavi k3d panel
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/SOURCES.txt` & `sympy_plot_backends-2.4.3/sympy_plot_backends.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/tests/backends/__init__.py` & `sympy_plot_backends-2.4.3/tests/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/tests/backends/make_tests.py` & `sympy_plot_backends-2.4.3/tests/backends/make_tests.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/tests/backends/test_base_backend.py` & `sympy_plot_backends-2.4.3/tests/backends/test_base_backend.py`

 * *Files 14% similar despite different names*

```diff
@@ -194,11 +194,32 @@
         assert len(p.series) == len(p.renderers) == 1
 
         p.extend([hor, ver1])
         assert len(p.series) == len(p.renderers) == 3
 
         p.append(ver2)
         assert len(p.series) == len(p.renderers) == 4
-    
+
     do_test(MB)
     do_test(PB)
     do_test(BB)
+
+
+def test_axis_scales():
+    # by default, axis scales should be set to None: this allows users to
+    # extend plot capabilities to create plots with categoricals axis.
+    # See: https://github.com/Davide-sd/sympy-plot-backends/issues/29
+    x = symbols("x")
+    p = plot(sin(x), backend=MB, show=False, n=5)
+    assert all(t is None for t in [p.xscale, p.yscale, p.zscale])
+
+    p = plot(sin(x), backend=MB, show=False, n=5, xscale="linear")
+    assert p.xscale == "linear"
+    assert all(t is None for t in [p.yscale, p.zscale])
+
+    p = plot(sin(x), backend=MB, show=False, n=5, yscale="linear")
+    assert p.yscale == "linear"
+    assert all(t is None for t in [p.xscale, p.zscale])
+
+    p = plot(sin(x), backend=MB, show=False, n=5, zscale="linear")
+    assert p.zscale == "linear"
+    assert all(t is None for t in [p.xscale, p.yscale])
```

### Comparing `sympy_plot_backends-2.4.2/tests/backends/test_bokeh.py` & `sympy_plot_backends-2.4.3/tests/backends/test_bokeh.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/tests/backends/test_k3d.py` & `sympy_plot_backends-2.4.3/tests/backends/test_k3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/tests/backends/test_matplotlib.py` & `sympy_plot_backends-2.4.3/tests/backends/test_matplotlib.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/tests/backends/test_plotly.py` & `sympy_plot_backends-2.4.3/tests/backends/test_plotly.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/tests/test_color_utils.py` & `sympy_plot_backends-2.4.3/tests/test_color_utils.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/tests/test_complex.py` & `sympy_plot_backends-2.4.3/tests/test_complex.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/tests/test_control.py` & `sympy_plot_backends-2.4.3/tests/test_control.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/tests/test_defaults.py` & `sympy_plot_backends-2.4.3/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/tests/test_doc_utils.py` & `sympy_plot_backends-2.4.3/tests/test_doc_utils.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/tests/test_functions.py` & `sympy_plot_backends-2.4.3/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/tests/test_plotgrid.py` & `sympy_plot_backends-2.4.3/tests/test_plotgrid.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/tests/test_series.py` & `sympy_plot_backends-2.4.3/tests/test_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -3039,7 +3039,31 @@
     s = Parametric2DLineSeries(e1, e2, (x, 1, 12), adaptive=False, n=100,
         exclude=list(range(1, 13)))
     xx, yy, pp = s.get_data()
     assert not np.isnan(pp).any()
     assert np.count_nonzero(np.isnan(xx)) == 11
     assert np.count_nonzero(np.isnan(yy)) == 11
     assert len(xx) > 100
+
+
+def test_unwrap():
+    # verify that unwrap works as expected
+
+    x, y = symbols("x, y")
+    expr = 1 / (x**3 + 2*x**2 + x)
+    expr = arg(expr.subs(x, I*y*2*pi))
+    s1 = LineOver1DRangeSeries(expr, (y, 1e-05, 1e05), xscale="log",
+        adaptive=False, n=10, unwrap=False)
+    s2 = LineOver1DRangeSeries(expr, (y, 1e-05, 1e05), xscale="log",
+        adaptive=False, n=10, unwrap=True)
+    s3 = LineOver1DRangeSeries(expr, (y, 1e-05, 1e05), xscale="log",
+        adaptive=False, n=10, unwrap={"period": 4})
+    x1, y1 = s1.get_data()
+    x2, y2 = s2.get_data()
+    x3, y3 = s3.get_data()
+    assert np.allclose(x1, x2)
+    # there must not be nan values in the results of these evaluations
+    assert all(not np.isnan(t).any() for t in [y1, y2, y3])
+    assert not np.allclose(y1, y2)
+    assert not np.allclose(y1, y3)
+    assert not np.allclose(y2, y3)
+
```

### Comparing `sympy_plot_backends-2.4.2/tests/test_utils.py` & `sympy_plot_backends-2.4.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.2/tests/test_vectors.py` & `sympy_plot_backends-2.4.3/tests/test_vectors.py`

 * *Files identical despite different names*


# Comparing `tmp/nrv-py-0.9.9.tar.gz` & `tmp/nrv-py-0.9.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrv-py-0.9.9.tar", last modified: Thu Jul 27 11:36:12 2023, max compression
+gzip compressed data, was "nrv-py-0.9.9a0.tar", last modified: Fri Jul 28 09:33:13 2023, max compression
```

## Comparing `nrv-py-0.9.9.tar` & `nrv-py-0.9.9a0.tar`

### file list

```diff
@@ -1,14 +1,243 @@
-drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-27 11:36:12.112702 nrv-py-0.9.9/
--rw-r--r--   0 fkolbl     (501) staff       (20)      234 2023-07-25 23:18:42.000000 nrv-py-0.9.9/MANIFEST.in
--rw-r--r--   0 fkolbl     (501) staff       (20)     1300 2023-07-27 11:36:12.112193 nrv-py-0.9.9/PKG-INFO
-drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-27 11:36:12.108558 nrv-py-0.9.9/nrv/
--rw-r--r--   0 fkolbl     (501) staff       (20)     3111 2023-07-27 11:19:09.000000 nrv-py-0.9.9/nrv/__init__.py
-drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-27 11:36:12.111195 nrv-py-0.9.9/nrv_py.egg-info/
--rw-r--r--   0 fkolbl     (501) staff       (20)     1300 2023-07-27 11:36:12.000000 nrv-py-0.9.9/nrv_py.egg-info/PKG-INFO
--rw-r--r--   0 fkolbl     (501) staff       (20)      200 2023-07-27 11:36:12.000000 nrv-py-0.9.9/nrv_py.egg-info/SOURCES.txt
--rw-r--r--   0 fkolbl     (501) staff       (20)        1 2023-07-27 11:36:12.000000 nrv-py-0.9.9/nrv_py.egg-info/dependency_links.txt
--rw-r--r--   0 fkolbl     (501) staff       (20)       88 2023-07-27 11:36:12.000000 nrv-py-0.9.9/nrv_py.egg-info/requires.txt
--rw-r--r--   0 fkolbl     (501) staff       (20)        4 2023-07-27 11:36:12.000000 nrv-py-0.9.9/nrv_py.egg-info/top_level.txt
--rw-r--r--   0 fkolbl     (501) staff       (20)     1424 2023-07-27 11:35:12.000000 nrv-py-0.9.9/pyproject.toml
--rw-r--r--   0 fkolbl     (501) staff       (20)       38 2023-07-27 11:36:12.112799 nrv-py-0.9.9/setup.cfg
--rw-r--r--   0 fkolbl     (501) staff       (20)     1335 2023-07-26 08:32:23.000000 nrv-py-0.9.9/setup.py
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:13.047511 nrv-py-0.9.9a0/
+-rw-r--r--   0 fkolbl     (501) staff       (20)      234 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/MANIFEST.in
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1302 2023-07-28 09:33:13.047119 nrv-py-0.9.9a0/PKG-INFO
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:12.912127 nrv-py-0.9.9a0/nrv/
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3117 2023-07-28 09:32:59.000000 nrv-py-0.9.9a0/nrv/__init__.py
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:12.912630 nrv-py-0.9.9a0/nrv/_misc/
+-rw-r--r--   0 fkolbl     (501) staff       (20)      601 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/NRV.ini
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:12.915264 nrv-py-0.9.9a0/nrv/_misc/OTF_PP/
+-rw-r--r--   0 fkolbl     (501) staff       (20)      216 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/OTF_PP/default.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1145 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/OTF_PP/is_blocked.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1074 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/OTF_PP/is_excited.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1150 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/OTF_PP/is_onset.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)      569 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/OTF_PP/raster_plot.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)      411 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/OTF_PP/rmv_keys.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)      715 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/OTF_PP/vmem_plot.py
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:12.918102 nrv-py-0.9.9a0/nrv/_misc/comsol_templates/
+-rw-r--r--   0 fkolbl     (501) staff       (20)   972710 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/comsol_templates/Nerve_1_Fascicle_1_CUFF.mph
+-rw-r--r--   0 fkolbl     (501) staff       (20)   442553 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/comsol_templates/Nerve_1_Fascicle_1_LIFE.mph
+-rw-r--r--   0 fkolbl     (501) staff       (20)   460556 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/comsol_templates/Nerve_1_Fascicle_2_LIFE.mph
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:12.922470 nrv-py-0.9.9a0/nrv/_misc/geom/
+-rw-r--r--   0 fkolbl     (501) staff       (20)  1736930 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/geom/smoothed_edges_white.dxf
+-rw-r--r--   0 fkolbl     (501) staff       (20)    81236 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/geom/smoothed_edges_white.png
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:12.923183 nrv-py-0.9.9a0/nrv/_misc/log/
+-rw-r--r--   0 fkolbl     (501) staff       (20)   165485 2023-07-28 09:33:12.000000 nrv-py-0.9.9a0/nrv/_misc/log/NRV.log
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:12.930241 nrv-py-0.9.9a0/nrv/_misc/materials/
+-rw-r--r--   0 fkolbl     (501) staff       (20)       49 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/materials/bone.mat
+-rw-r--r--   0 fkolbl     (501) staff       (20)       61 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/materials/cerebrospinal_fluid.mat
+-rw-r--r--   0 fkolbl     (501) staff       (20)       47 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/materials/dura.mat
+-rw-r--r--   0 fkolbl     (501) staff       (20)       46 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/materials/endoneurium_bhadra.mat
+-rw-r--r--   0 fkolbl     (501) staff       (20)       80 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/materials/endoneurium_ranck.mat
+-rw-r--r--   0 fkolbl     (501) staff       (20)       55 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/materials/epidural_space.mat
+-rw-r--r--   0 fkolbl     (501) staff       (20)       45 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/materials/epineurium.mat
+-rw-r--r--   0 fkolbl     (501) staff       (20)       29 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/materials/material_1.mat
+-rw-r--r--   0 fkolbl     (501) staff       (20)       58 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/materials/material_2.mat
+-rw-r--r--   0 fkolbl     (501) staff       (20)       47 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/materials/muscle.mat
+-rw-r--r--   0 fkolbl     (501) staff       (20)       47 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/materials/perineurium.mat
+-rw-r--r--   0 fkolbl     (501) staff       (20)       46 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/materials/platinum.mat
+-rw-r--r--   0 fkolbl     (501) staff       (20)       45 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/materials/saline.mat
+-rw-r--r--   0 fkolbl     (501) staff       (20)       44 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/materials/silicone.mat
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:12.958588 nrv-py-0.9.9a0/nrv/_misc/mods/
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3787 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/AXNODE.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1806 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/CaPump.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2056 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/DNav18.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3043 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/KCa.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2475 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/NaCaPump.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1505 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/Nakpump.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2225 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/NakpumpSchild.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2773 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/Nav11_a.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2762 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/Nav16_a.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2747 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/RattayAberham.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2574 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/caextscale.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2607 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/caintscale.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     4234 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/can.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3606 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/cat.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)      502 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/extrapump.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3707 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/flut_motor.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3562 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/flut_sensory.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2102 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/h.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)      994 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/k_ion_dynamics.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3226 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/ka.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1739 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/kaslow.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3228 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/kd.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1647 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/kdr.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1010 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/kdr_Tiger.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3132 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/kds.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1498 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/kf.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1123 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/kmtype.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)      719 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/kna.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1493 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/ks.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)      765 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/leak.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1715 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/leakSchild.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3569 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/mysa_motor.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3560 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/mysa_sensory.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2665 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/na3.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1014 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/na_ion_dynamics.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3825 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/naf.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3072 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/naf97.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3183 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/naf97mean.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1517 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/nahh.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3252 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/nas.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3128 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/nas97.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3240 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/nas97mean.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2671 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/nattxs.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3232 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/nav1p9.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1838 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/nax.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     5217 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/node_motor.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     5330 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/node_sensory.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3569 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/stin_motor.mod
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3566 2023-07-16 23:12:28.000000 nrv-py-0.9.9a0/nrv/_misc/mods/stin_sensory.mod
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:12.982255 nrv-py-0.9.9a0/nrv/_misc/pops/
+-rw-r--r--   0 fkolbl     (501) staff       (20)    23459 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_1000_axons_A.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    23450 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_1000_axons_B.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    23429 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_1000_axons_C.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    23441 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_1000_axons_D.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    23456 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_1000_axons_E.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    23474 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_1000_axons_F.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2348 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_100_axons_A.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2346 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_100_axons_B.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2355 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_100_axons_C.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2349 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_100_axons_D.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2352 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_100_axons_E.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2346 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_100_axons_F.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    46916 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_2000_axons_A.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    46879 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_2000_axons_B.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    46946 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_2000_axons_C.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    46882 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_2000_axons_D.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    46948 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_2000_axons_E.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    46923 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_2000_axons_F.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     4694 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_200_axons_A.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     4681 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_200_axons_B.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     4702 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_200_axons_C.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     4699 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_200_axons_D.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     4685 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_200_axons_E.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     4673 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_200_axons_F.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   117300 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_5000_axons_A.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   117318 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_5000_axons_B.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   117303 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_5000_axons_C.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   117297 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_5000_axons_D.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   117184 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_5000_axons_E.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   117231 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_5000_axons_F.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    11725 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_500_axons_A.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    11730 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_500_axons_B.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    11732 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_500_axons_C.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    11720 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_500_axons_D.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    11705 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_500_axons_E.pop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    11710 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/pops/Population_of_500_axons_F.pop
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:13.009215 nrv-py-0.9.9a0/nrv/_misc/ppops/
+-rw-r--r--   0 fkolbl     (501) staff       (20)    63162 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_1000_axons_A.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    63158 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_1000_axons_B.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    63156 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_1000_axons_C.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    63146 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_1000_axons_D.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    63224 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_1000_axons_E.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    63118 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_1000_axons_F.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     6335 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_100_axons_A.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     6345 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_100_axons_B.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     6367 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_100_axons_C.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     6337 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_100_axons_D.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     6350 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_100_axons_E.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)     6346 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_100_axons_F.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   125839 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_2000_axons_A.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   125735 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_2000_axons_B.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   125872 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_2000_axons_C.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   125804 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_2000_axons_D.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   125951 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_2000_axons_E.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   125835 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_2000_axons_F.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    12703 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_200_axons_A.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    12674 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_200_axons_B.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    12705 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_200_axons_C.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    12695 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_200_axons_D.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    12671 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_200_axons_E.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    12677 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_200_axons_F.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   316552 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_5000_axons_A.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   316575 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_5000_axons_B.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   316397 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_5000_axons_C.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   316442 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_5000_axons_D.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   316314 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_5000_axons_E.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)   316431 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_5000_axons_F.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    31672 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_500_axons_A.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    31680 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_500_axons_B.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    31643 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_500_axons_C.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    31664 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_500_axons_D.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    31663 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_500_axons_E.ppop
+-rw-r--r--   0 fkolbl     (501) staff       (20)    31668 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/ppops/Placed_population_of_500_axons_F.ppop
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:13.015966 nrv-py-0.9.9a0/nrv/_misc/stats/
+-rw-r--r--   0 fkolbl     (501) staff       (20)      219 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/stats/Jacobs_11_A.csv
+-rw-r--r--   0 fkolbl     (501) staff       (20)      159 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/stats/Jacobs_11_B.csv
+-rw-r--r--   0 fkolbl     (501) staff       (20)      249 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/stats/Jacobs_11_C.csv
+-rw-r--r--   0 fkolbl     (501) staff       (20)      270 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/stats/Jacobs_11_D.csv
+-rw-r--r--   0 fkolbl     (501) staff       (20)      169 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/stats/Jacobs_9_A.csv
+-rw-r--r--   0 fkolbl     (501) staff       (20)      209 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/stats/Jacobs_9_B.csv
+-rw-r--r--   0 fkolbl     (501) staff       (20)      269 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/stats/Jacobs_9_C.csv
+-rw-r--r--   0 fkolbl     (501) staff       (20)      278 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/stats/Jacobs_9_D.csv
+-rw-r--r--   0 fkolbl     (501) staff       (20)      319 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/stats/Ochoa_M.csv
+-rw-r--r--   0 fkolbl     (501) staff       (20)      401 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/stats/Ochoa_U.csv
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1415 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/stats/Schellens_1.csv
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1117 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/_misc/stats/Schellens_2.csv
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:13.020386 nrv-py-0.9.9a0/nrv/backend/
+-rw-r--r--   0 fkolbl     (501) staff       (20)     8213 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/backend/MCore.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3166 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/backend/NRV_Class.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)      134 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/backend/__init__.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1216 2023-07-26 14:34:26.000000 nrv-py-0.9.9a0/nrv/backend/compileMods.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3599 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/backend/file_handler.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)      372 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/backend/inouts.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)     5584 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/backend/log_interface.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2072 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/backend/parameters.py
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:13.023766 nrv-py-0.9.9a0/nrv/fmod/
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:13.025925 nrv-py-0.9.9a0/nrv/fmod/FEM/
+-rw-r--r--   0 fkolbl     (501) staff       (20)     6835 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/FEM/COMSOL_model.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1785 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/FEM/FEM.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)    16166 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/FEM/FENICS_model.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)      134 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/FEM/__init__.py
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:13.028676 nrv-py-0.9.9a0/nrv/fmod/FEM/fenics_utils/
+-rw-r--r--   0 fkolbl     (501) staff       (20)    21654 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/FEM/fenics_utils/FEMSimulation.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)    14870 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/FEM/fenics_utils/SimParameters.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)    12079 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/FEM/fenics_utils/SimResult.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)      134 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/FEM/fenics_utils/__init__.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)     9124 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/FEM/fenics_utils/fenics_materials.py
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:13.031494 nrv-py-0.9.9a0/nrv/fmod/FEM/mesh_creator/
+-rw-r--r--   0 fkolbl     (501) staff       (20)    20865 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/FEM/mesh_creator/MshCreator.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2710 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/FEM/mesh_creator/NRV_Msh.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)    36968 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/FEM/mesh_creator/NerveMshCreator.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)      134 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/FEM/mesh_creator/__init__.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)      148 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/__init__.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)    14600 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/electrodes.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)    25773 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/extracellular.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)     4910 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/materials.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)    23394 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/recording.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)    16167 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/fmod/stimulus.py
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:13.036614 nrv-py-0.9.9a0/nrv/nmod/
+-rw-r--r--   0 fkolbl     (501) staff       (20)      149 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/nmod/__init__.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)    42779 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/nmod/axons.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)    33313 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/nmod/fascicle_generator.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)    64218 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/nmod/fascicles.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)    60832 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/nmod/myelinated.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)     6269 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/nmod/nerve.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)    48791 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/nmod/thin_myelinated.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)    49019 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/nmod/unmyelinated.py
+-rwxr--r--   0 fkolbl     (501) staff       (20)     4497 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/nrv2calm
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:13.038940 nrv-py-0.9.9a0/nrv/optim/
+-rw-r--r--   0 fkolbl     (501) staff       (20)     3750 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/optim/CostFunctions.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)      457 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/optim/Optimizers.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2258 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/optim/Problems.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)      132 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/optim/__init__.py
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:13.041188 nrv-py-0.9.9a0/nrv/utils/
+-rw-r--r--   0 fkolbl     (501) staff       (20)      132 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/utils/__init__.py
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:13.043027 nrv-py-0.9.9a0/nrv/utils/cell/
+-rw-r--r--   0 fkolbl     (501) staff       (20)    11323 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/utils/cell/CL_discretization.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)    34620 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/utils/cell/CL_postprocessing.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)    32335 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/utils/cell/CL_simulations.py
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:13.043743 nrv-py-0.9.9a0/nrv/utils/fascicle/
+-rw-r--r--   0 fkolbl     (501) staff       (20)     6396 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/utils/fascicle/FL_postprocessing.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)    13713 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/utils/nrv_function.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2565 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/utils/saving_handler.py
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1704 2023-07-25 23:18:42.000000 nrv-py-0.9.9a0/nrv/utils/units.py
+drwxr-xr-x   0 fkolbl     (501) staff       (20)        0 2023-07-28 09:33:13.046512 nrv-py-0.9.9a0/nrv_py.egg-info/
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1302 2023-07-28 09:33:12.000000 nrv-py-0.9.9a0/nrv_py.egg-info/PKG-INFO
+-rw-r--r--   0 fkolbl     (501) staff       (20)     7822 2023-07-28 09:33:12.000000 nrv-py-0.9.9a0/nrv_py.egg-info/SOURCES.txt
+-rw-r--r--   0 fkolbl     (501) staff       (20)        1 2023-07-28 09:33:12.000000 nrv-py-0.9.9a0/nrv_py.egg-info/dependency_links.txt
+-rw-r--r--   0 fkolbl     (501) staff       (20)       88 2023-07-28 09:33:12.000000 nrv-py-0.9.9a0/nrv_py.egg-info/requires.txt
+-rw-r--r--   0 fkolbl     (501) staff       (20)        4 2023-07-28 09:33:12.000000 nrv-py-0.9.9a0/nrv_py.egg-info/top_level.txt
+-rw-r--r--   0 fkolbl     (501) staff       (20)     1528 2023-07-28 08:53:44.000000 nrv-py-0.9.9a0/pyproject.toml
+-rw-r--r--   0 fkolbl     (501) staff       (20)       38 2023-07-28 09:33:13.047644 nrv-py-0.9.9a0/setup.cfg
+-rw-r--r--   0 fkolbl     (501) staff       (20)     2468 2023-07-28 09:29:29.000000 nrv-py-0.9.9a0/setup.py
```

### Comparing `nrv-py-0.9.9/PKG-INFO` & `nrv-py-0.9.9a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrv-py
-Version: 0.9.9
+Version: 0.9.9a0
 Summary: NeuRon Virtualizer (NRV)
 Home-page: https://github.com/fkolbl/NRV
 Author: Florian Kolbl - Roland Giraud - Louis Regnacq - Thomas Couppey
 Project-URL: Documentation, https://nrv.readthedocs.io
 Project-URL: Source, https://github.com/fkolbl/NRV
 Keywords: neuronal simulation,computer simulation,neurosciences,multiphysics,Neuron,Comsol
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
```

### Comparing `nrv-py-0.9.9/nrv/__init__.py` & `nrv-py-0.9.9a0/nrv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ NeuRon Virtualizer, large scale modeling of Peripheral Nervous System with random stimulation waveforms"""
 
 # Meta information
 __title__           = 'NRV'
 __project__         = 'NeuRon Virtualizer (NRV)'
-__version__         = '0.9.9'
+__version__         = '0.9.9.alpha'
 __date__            = '2023–07–23'
 __author__          = 'Florian Kolbl'
 __contributors__    = 'Florian Kolbl, Roland Giraud, Louis Regnacq, Thomas Couppey'
 __copyright__       = '2023, Florian Kolbl'
 __license__         = 'CeCILL'
 
 #################################
```

### Comparing `nrv-py-0.9.9/nrv_py.egg-info/PKG-INFO` & `nrv-py-0.9.9a0/nrv_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrv-py
-Version: 0.9.9
+Version: 0.9.9a0
 Summary: NeuRon Virtualizer (NRV)
 Home-page: https://github.com/fkolbl/NRV
 Author: Florian Kolbl - Roland Giraud - Louis Regnacq - Thomas Couppey
 Project-URL: Documentation, https://nrv.readthedocs.io
 Project-URL: Source, https://github.com/fkolbl/NRV
 Keywords: neuronal simulation,computer simulation,neurosciences,multiphysics,Neuron,Comsol
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
```

### Comparing `nrv-py-0.9.9/pyproject.toml` & `nrv-py-0.9.9a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 # Meta information: PyPI and Pip
+[build-system]
+requires = [
+    "setuptools>=42",
+    "wheel"
+]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = 'nrv-py'
 authors = [{name='Florian Kolbl - Roland Giraud - Louis Regnacq - Thomas Couppey'}]
 license = {file='License.txt'}
 keywords = ['neuronal simulation', 'computer simulation', 'neurosciences',
             'multiphysics', 'Neuron', 'Comsol']
```


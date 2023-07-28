# Comparing `tmp/femagtools-1.3.1.tar.gz` & `tmp/femagtools-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femagtools-1.3.1.tar", last modified: Fri Jul  7 06:15:30 2023, max compression
+gzip compressed data, was "femagtools-1.3.2.tar", last modified: Fri Jul 28 12:08:24 2023, max compression
```

## Comparing `femagtools-1.3.1.tar` & `femagtools-1.3.2.tar`

### file list

```diff
@@ -1,190 +1,195 @@
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-07 06:15:30.359389 femagtools-1.3.1/
--rw-r--r--   0 tar        (210) tar        (210)     1316 2023-02-15 20:03:56.000000 femagtools-1.3.1/LICENSE
--rw-r--r--   0 tar        (210) tar        (210)       35 2023-02-15 20:03:56.000000 femagtools-1.3.1/MANIFEST.in
--rw-r--r--   0 tar        (210) tar        (210)     5262 2023-07-07 06:15:30.359389 femagtools-1.3.1/PKG-INFO
--rw-r--r--   0 tar        (210) tar        (210)     3072 2023-02-14 18:11:00.000000 femagtools-1.3.1/README.md
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-07 06:15:30.344389 femagtools-1.3.1/femagtools/
--rw-r--r--   0 tar        (210) tar        (210)     1630 2023-07-07 06:14:03.000000 femagtools-1.3.1/femagtools/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     2250 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/airgap.py
--rw-r--r--   0 tar        (210) tar        (210)    12122 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/amazon.py
--rw-r--r--   0 tar        (210) tar        (210)    14001 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/amela.py
--rw-r--r--   0 tar        (210) tar        (210)     7706 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/asm.py
--rwxr-xr-x   0 tar        (210) tar        (210)    68745 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/bch.py
--rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/bchxml.py
--rw-r--r--   0 tar        (210) tar        (210)    10766 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/condor.py
--rw-r--r--   0 tar        (210) tar        (210)     1076 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/conductor.py
--rw-r--r--   0 tar        (210) tar        (210)     3087 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/config.py
--rw-r--r--   0 tar        (210) tar        (210)    23706 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/convert.py
--rw-r--r--   0 tar        (210) tar        (210)     7017 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/dakota.py
--rwxr-xr-x   0 tar        (210) tar        (210)     4064 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/dakota_femag.py
--rw-r--r--   0 tar        (210) tar        (210)     5573 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/dakotaout.py
--rw-r--r--   0 tar        (210) tar        (210)     7460 2023-03-24 14:45:00.000000 femagtools-1.3.1/femagtools/docker.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-07 06:15:30.345389 femagtools-1.3.1/femagtools/dxfsl/
--rw-r--r--   0 tar        (210) tar        (210)        0 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/dxfsl/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)    52804 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/dxfsl/area.py
--rw-r--r--   0 tar        (210) tar        (210)     8990 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/dxfsl/conv.py
--rw-r--r--   0 tar        (210) tar        (210)    19131 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/dxfsl/converter.py
--rw-r--r--   0 tar        (210) tar        (210)     1266 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/dxfsl/corner.py
--rw-r--r--   0 tar        (210) tar        (210)     1861 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/dxfsl/dumprenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    23372 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/dxfsl/fslrenderer.py
--rw-r--r--   0 tar        (210) tar        (210)     9835 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/dxfsl/functions.py
--rw-r--r--   0 tar        (210) tar        (210)   141862 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/dxfsl/geom.py
--rw-r--r--   0 tar        (210) tar        (210)    28135 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/dxfsl/machine.py
--rw-r--r--   0 tar        (210) tar        (210)    12311 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/dxfsl/plotrenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    44863 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/dxfsl/shape.py
--rw-r--r--   0 tar        (210) tar        (210)    13156 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/ecloss.py
--rw-r--r--   0 tar        (210) tar        (210)     1224 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/erg.py
--rw-r--r--   0 tar        (210) tar        (210)    42176 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/femag.py
--rw-r--r--   0 tar        (210) tar        (210)     7415 2023-05-17 15:12:10.000000 femagtools-1.3.1/femagtools/forcedens.py
--rw-r--r--   0 tar        (210) tar        (210)    30989 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/fsl.py
--rw-r--r--   0 tar        (210) tar        (210)     3017 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/getset.py
--rw-r--r--   0 tar        (210) tar        (210)     3903 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/gmsh.py
--rw-r--r--   0 tar        (210) tar        (210)    17166 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/google.py
--rw-r--r--   0 tar        (210) tar        (210)     1561 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/grid.py
--rw-r--r--   0 tar        (210) tar        (210)     3738 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/hxy.py
--rw-r--r--   0 tar        (210) tar        (210)    41578 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/isa7.py
--rw-r--r--   0 tar        (210) tar        (210)     2790 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/jcf2msh.py
--rw-r--r--   0 tar        (210) tar        (210)     1779 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/jhb.py
--rw-r--r--   0 tar        (210) tar        (210)    11320 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/job.py
--rw-r--r--   0 tar        (210) tar        (210)     2261 2022-08-24 07:36:25.000000 femagtools-1.3.1/femagtools/losscoeffs.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-07 06:15:30.346389 femagtools-1.3.1/femagtools/machine/
--rw-r--r--   0 tar        (210) tar        (210)     7413 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/machine/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)    11371 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/machine/effloss.py
--rw-r--r--   0 tar        (210) tar        (210)    38093 2023-07-03 13:37:05.000000 femagtools-1.3.1/femagtools/machine/im.py
--rwxr-xr-x   0 tar        (210) tar        (210)    51280 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/machine/pm.py
--rw-r--r--   0 tar        (210) tar        (210)    21743 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/machine/sizing.py
--rw-r--r--   0 tar        (210) tar        (210)    32810 2023-07-03 13:37:05.000000 femagtools-1.3.1/femagtools/machine/sm.py
--rw-r--r--   0 tar        (210) tar        (210)    16617 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/machine/utils.py
--rw-r--r--   0 tar        (210) tar        (210)     1093 2023-02-15 20:03:56.000000 femagtools-1.3.1/femagtools/magnet.py
--rw-r--r--   0 tar        (210) tar        (210)    39696 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/mcv.py
--rw-r--r--   0 tar        (210) tar        (210)     1833 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/me.py
--rw-r--r--   0 tar        (210) tar        (210)    14068 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/model.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-07 06:15:30.346389 femagtools-1.3.1/femagtools/moo/
--rw-r--r--   0 tar        (210) tar        (210)      175 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/moo/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     5493 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/moo/algorithm.py
--rw-r--r--   0 tar        (210) tar        (210)    10100 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/moo/population.py
--rw-r--r--   0 tar        (210) tar        (210)     2391 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/moo/problem.py
--rw-r--r--   0 tar        (210) tar        (210)     2825 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/moproblem.py
--rw-r--r--   0 tar        (210) tar        (210)     8506 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/multiproc.py
--rw-r--r--   0 tar        (210) tar        (210)     1841 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/mxw2msh.py
--rw-r--r--   0 tar        (210) tar        (210)    12781 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/nc.py
--rw-r--r--   0 tar        (210) tar        (210)     2052 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/netlist.py
--rw-r--r--   0 tar        (210) tar        (210)     3099 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/ntib.py
--rw-r--r--   0 tar        (210) tar        (210)     8685 2023-02-21 19:53:03.000000 femagtools-1.3.1/femagtools/opt.py
--rw-r--r--   0 tar        (210) tar        (210)    18717 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/parstudy.py
--rw-r--r--   0 tar        (210) tar        (210)    61312 2023-07-07 06:13:48.000000 femagtools-1.3.1/femagtools/plot.py
--rw-r--r--   0 tar        (210) tar        (210)     6536 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/poc.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-07 06:15:30.357389 femagtools-1.3.1/femagtools/templates/
--rw-r--r--   0 tar        (210) tar        (210)      874 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/FE-losses.mako
--rw-r--r--   0 tar        (210) tar        (210)      246 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/templates/airgapinduc.mako
--rw-r--r--   0 tar        (210) tar        (210)     2879 2022-09-28 06:51:55.000000 femagtools-1.3.1/femagtools/templates/asyn_motor.mako
--rw-r--r--   0 tar        (210) tar        (210)     2483 2022-09-28 06:51:55.000000 femagtools-1.3.1/femagtools/templates/basic_modpar.mako
--rw-r--r--   0 tar        (210) tar        (210)     1911 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/calc_field_ts.mako
--rw-r--r--   0 tar        (210) tar        (210)     1600 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/templates/calc_therm_field.mako
--rw-r--r--   0 tar        (210) tar        (210)      997 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/cogg_calc.mako
--rw-r--r--   0 tar        (210) tar        (210)      400 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/colorgrad.mako
--rw-r--r--   0 tar        (210) tar        (210)     1264 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/com_motor_sim.mako
--rw-r--r--   0 tar        (210) tar        (210)      472 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/conduct-data.mako
--rw-r--r--   0 tar        (210) tar        (210)      663 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/templates/connect_models.mako
--rw-r--r--   0 tar        (210) tar        (210)     1350 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/cu_losses.mako
--rw-r--r--   0 tar        (210) tar        (210)     1672 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/ec-rotorbar.mako
--rw-r--r--   0 tar        (210) tar        (210)     1983 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/fe-contr.mako
--rw-r--r--   0 tar        (210) tar        (210)     4820 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/templates/gen_winding.mako
--rw-r--r--   0 tar        (210) tar        (210)      560 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/inductances.mako
--rw-r--r--   0 tar        (210) tar        (210)     1270 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/ld_lq_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      600 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/leak_dist_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)      770 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/leak_evol_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)      431 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/leak_tooth_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)     1271 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnet-data.mako
--rw-r--r--   0 tar        (210) tar        (210)      788 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetFC2.mako
--rw-r--r--   0 tar        (210) tar        (210)     2268 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/templates/magnetIron.mako
--rw-r--r--   0 tar        (210) tar        (210)     1426 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetIron2.mako
--rw-r--r--   0 tar        (210) tar        (210)     2315 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetIron3.mako
--rw-r--r--   0 tar        (210) tar        (210)     1413 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetIron4.mako
--rw-r--r--   0 tar        (210) tar        (210)     1376 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetIron5.mako
--rw-r--r--   0 tar        (210) tar        (210)     3960 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/templates/magnetIronV.mako
--rw-r--r--   0 tar        (210) tar        (210)     2010 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetSector.mako
--rw-r--r--   0 tar        (210) tar        (210)      727 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetSectorLinear.mako
--rw-r--r--   0 tar        (210) tar        (210)     1295 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetShell.mako
--rw-r--r--   0 tar        (210) tar        (210)     4080 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/magnetShell2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1094 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/mesh-airgap.mako
--rw-r--r--   0 tar        (210) tar        (210)     2298 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/modal_analysis.mako
--rw-r--r--   0 tar        (210) tar        (210)     1202 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/mult_cal_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      345 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/new_model.mako
--rw-r--r--   0 tar        (210) tar        (210)     3209 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/noloadflux-rot.mako
--rw-r--r--   0 tar        (210) tar        (210)     4661 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/noloadflux.mako
--rw-r--r--   0 tar        (210) tar        (210)     3146 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/noloadfluxdc.mako
--rw-r--r--   0 tar        (210) tar        (210)      313 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/open.mako
--rw-r--r--   0 tar        (210) tar        (210)      630 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/plots.mako
--rw-r--r--   0 tar        (210) tar        (210)     1373 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/pm_sym_f_cur.mako
--rw-r--r--   0 tar        (210) tar        (210)     2319 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/pm_sym_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      925 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/pm_sym_loss.mako
--rw-r--r--   0 tar        (210) tar        (210)     1251 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/psd_psq_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      643 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/ring.mako
--rw-r--r--   0 tar        (210) tar        (210)      973 2022-09-28 06:51:55.000000 femagtools-1.3.1/femagtools/templates/rot_hsm.mako
--rw-r--r--   0 tar        (210) tar        (210)     2280 2022-09-28 06:51:55.000000 femagtools-1.3.1/femagtools/templates/rotorAsyn.mako
--rw-r--r--   0 tar        (210) tar        (210)     1908 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/rotorKs2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1910 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/rotor_msh.mako
--rw-r--r--   0 tar        (210) tar        (210)      753 2022-09-28 06:51:55.000000 femagtools-1.3.1/femagtools/templates/rotor_winding.mako
--rw-r--r--   0 tar        (210) tar        (210)     1981 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/shortcircuit.mako
--rw-r--r--   0 tar        (210) tar        (210)     2077 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/srm.mako
--rw-r--r--   0 tar        (210) tar        (210)      761 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/stator1.mako
--rw-r--r--   0 tar        (210) tar        (210)      599 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/stator2.mako
--rw-r--r--   0 tar        (210) tar        (210)      724 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/stator3Linear.mako
--rw-r--r--   0 tar        (210) tar        (210)     1179 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/stator4.mako
--rw-r--r--   0 tar        (210) tar        (210)      893 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/statorBG.mako
--rw-r--r--   0 tar        (210) tar        (210)     2071 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/templates/statorRing.mako
--rw-r--r--   0 tar        (210) tar        (210)     4942 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/templates/statorRotor3.mako
--rw-r--r--   0 tar        (210) tar        (210)     1799 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/templates/stator_msh.mako
--rw-r--r--   0 tar        (210) tar        (210)     3142 2023-07-03 13:26:45.000000 femagtools-1.3.1/femagtools/templates/therm-dynamic.mako
--rw-r--r--   0 tar        (210) tar        (210)     1002 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/templates/therm-static.mako
--rw-r--r--   0 tar        (210) tar        (210)     1782 2023-06-23 19:15:43.000000 femagtools-1.3.1/femagtools/templates/torq_calc.mako
--rw-r--r--   0 tar        (210) tar        (210)     5791 2022-08-24 07:36:25.000000 femagtools-1.3.1/femagtools/tks.py
--rw-r--r--   0 tar        (210) tar        (210)    47280 2023-02-14 18:11:00.000000 femagtools-1.3.1/femagtools/ts.py
--rw-r--r--   0 tar        (210) tar        (210)     2444 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/vbf.py
--rw-r--r--   0 tar        (210) tar        (210)     8595 2022-08-07 12:24:45.000000 femagtools-1.3.1/femagtools/vtu.py
--rw-r--r--   0 tar        (210) tar        (210)    22279 2023-03-24 14:45:00.000000 femagtools-1.3.1/femagtools/windings.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-07 06:15:30.344389 femagtools-1.3.1/femagtools.egg-info/
--rw-r--r--   0 tar        (210) tar        (210)     5262 2023-07-07 06:15:30.000000 femagtools-1.3.1/femagtools.egg-info/PKG-INFO
--rw-r--r--   0 tar        (210) tar        (210)     5022 2023-07-07 06:15:30.000000 femagtools-1.3.1/femagtools.egg-info/SOURCES.txt
--rw-r--r--   0 tar        (210) tar        (210)        1 2023-07-07 06:15:30.000000 femagtools-1.3.1/femagtools.egg-info/dependency_links.txt
--rw-r--r--   0 tar        (210) tar        (210)      191 2023-07-07 06:15:30.000000 femagtools-1.3.1/femagtools.egg-info/entry_points.txt
--rw-r--r--   0 tar        (210) tar        (210)      144 2023-07-07 06:15:30.000000 femagtools-1.3.1/femagtools.egg-info/requires.txt
--rw-r--r--   0 tar        (210) tar        (210)       11 2023-07-07 06:15:30.000000 femagtools-1.3.1/femagtools.egg-info/top_level.txt
--rw-r--r--   0 tar        (210) tar        (210)     1369 2023-02-15 20:03:56.000000 femagtools-1.3.1/pyproject.toml
--rw-r--r--   0 tar        (210) tar        (210)       38 2023-07-07 06:15:30.359389 femagtools-1.3.1/setup.cfg
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-07 06:15:30.359389 femagtools-1.3.1/tests/
--rw-r--r--   0 tar        (210) tar        (210)     1065 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_airgap_induction.py
--rw-r--r--   0 tar        (210) tar        (210)      646 2023-02-14 18:11:00.000000 femagtools-1.3.1/tests/test_amela.py
--rw-r--r--   0 tar        (210) tar        (210)     1398 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_asm.py
--rwxr-xr-x   0 tar        (210) tar        (210)    14755 2023-02-14 18:11:00.000000 femagtools-1.3.1/tests/test_bchreader.py
--rw-r--r--   0 tar        (210) tar        (210)      332 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_conductor.py
--rw-r--r--   0 tar        (210) tar        (210)     6171 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_convert.py
--rw-r--r--   0 tar        (210) tar        (210)     1142 2023-07-03 13:36:57.000000 femagtools-1.3.1/tests/test_effloss.py
--rw-r--r--   0 tar        (210) tar        (210)      523 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_erg.py
--rw-r--r--   0 tar        (210) tar        (210)     1934 2023-02-16 09:09:33.000000 femagtools-1.3.1/tests/test_femag.py
--rw-r--r--   0 tar        (210) tar        (210)      533 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_forcedens.py
--rwxr-xr-x   0 tar        (210) tar        (210)    16099 2023-06-23 19:15:43.000000 femagtools-1.3.1/tests/test_fsl.py
--rw-r--r--   0 tar        (210) tar        (210)      662 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_im.py
--rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_isa7.py
--rw-r--r--   0 tar        (210) tar        (210)      824 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_jhb.py
--rw-r--r--   0 tar        (210) tar        (210)      981 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_job.py
--rw-r--r--   0 tar        (210) tar        (210)     2012 2022-08-24 07:36:25.000000 femagtools-1.3.1/tests/test_losscoeffs.py
--rwxr-xr-x   0 tar        (210) tar        (210)    12881 2023-07-03 13:26:45.000000 femagtools-1.3.1/tests/test_machine.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2608 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_magncurv.py
--rw-r--r--   0 tar        (210) tar        (210)      276 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_magnet.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2118 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_mcvreader.py
--rwxr-xr-x   0 tar        (210) tar        (210)     3986 2023-06-23 19:15:43.000000 femagtools-1.3.1/tests/test_mcvwriter.py
--rw-r--r--   0 tar        (210) tar        (210)      192 2023-02-14 18:11:00.000000 femagtools-1.3.1/tests/test_me.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2372 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_model.py
--rw-r--r--   0 tar        (210) tar        (210)     3116 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_nc.py
--rw-r--r--   0 tar        (210) tar        (210)     1340 2023-07-03 13:26:45.000000 femagtools-1.3.1/tests/test_parident.py
--rw-r--r--   0 tar        (210) tar        (210)     3200 2023-03-02 15:44:17.000000 femagtools-1.3.1/tests/test_parstudy.py
--rwxr-xr-x   0 tar        (210) tar        (210)     5816 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_pocfile.py
--rw-r--r--   0 tar        (210) tar        (210)     1109 2023-02-14 18:11:00.000000 femagtools-1.3.1/tests/test_sizing.py
--rw-r--r--   0 tar        (210) tar        (210)    83524 2023-06-23 19:15:43.000000 femagtools-1.3.1/tests/test_sm.py
--rwxr-xr-x   0 tar        (210) tar        (210)      766 2022-08-24 07:36:25.000000 femagtools-1.3.1/tests/test_tksreader.py
--rw-r--r--   0 tar        (210) tar        (210)     1825 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_ts.py
--rwxr-xr-x   0 tar        (210) tar        (210)      832 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_vbfreader.py
--rw-r--r--   0 tar        (210) tar        (210)      868 2022-08-07 12:24:45.000000 femagtools-1.3.1/tests/test_vtu.py
--rw-r--r--   0 tar        (210) tar        (210)     4912 2023-03-24 14:45:00.000000 femagtools-1.3.1/tests/test_windings.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-28 12:08:24.171510 femagtools-1.3.2/
+-rw-r--r--   0 tar        (210) tar        (210)     1316 2023-02-15 20:03:56.000000 femagtools-1.3.2/LICENSE
+-rw-r--r--   0 tar        (210) tar        (210)       35 2023-02-15 20:03:56.000000 femagtools-1.3.2/MANIFEST.in
+-rw-r--r--   0 tar        (210) tar        (210)     5262 2023-07-28 12:08:24.171510 femagtools-1.3.2/PKG-INFO
+-rw-r--r--   0 tar        (210) tar        (210)     3072 2023-02-14 18:11:00.000000 femagtools-1.3.2/README.md
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-28 12:08:24.153510 femagtools-1.3.2/femagtools/
+-rw-r--r--   0 tar        (210) tar        (210)     1630 2023-07-28 12:07:16.000000 femagtools-1.3.2/femagtools/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     1550 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/airgap.py
+-rw-r--r--   0 tar        (210) tar        (210)    12122 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/amazon.py
+-rw-r--r--   0 tar        (210) tar        (210)    14056 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/amela.py
+-rw-r--r--   0 tar        (210) tar        (210)     7706 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/asm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    69488 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/bch.py
+-rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/bchxml.py
+-rw-r--r--   0 tar        (210) tar        (210)    10766 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/condor.py
+-rw-r--r--   0 tar        (210) tar        (210)     1076 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/conductor.py
+-rw-r--r--   0 tar        (210) tar        (210)     3087 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/config.py
+-rw-r--r--   0 tar        (210) tar        (210)    23706 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/convert.py
+-rw-r--r--   0 tar        (210) tar        (210)     7017 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/dakota.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     4064 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/dakota_femag.py
+-rw-r--r--   0 tar        (210) tar        (210)     5573 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/dakotaout.py
+-rw-r--r--   0 tar        (210) tar        (210)     7460 2023-03-24 14:45:00.000000 femagtools-1.3.2/femagtools/docker.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-28 12:08:24.154510 femagtools-1.3.2/femagtools/dxfsl/
+-rw-r--r--   0 tar        (210) tar        (210)        0 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/dxfsl/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)    54793 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/dxfsl/area.py
+-rw-r--r--   0 tar        (210) tar        (210)     8990 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/dxfsl/conv.py
+-rw-r--r--   0 tar        (210) tar        (210)    19237 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/dxfsl/converter.py
+-rw-r--r--   0 tar        (210) tar        (210)     1266 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/dxfsl/corner.py
+-rw-r--r--   0 tar        (210) tar        (210)     1861 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/dxfsl/dumprenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    23372 2023-07-03 13:26:45.000000 femagtools-1.3.2/femagtools/dxfsl/fslrenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)     9835 2023-07-03 13:26:45.000000 femagtools-1.3.2/femagtools/dxfsl/functions.py
+-rw-r--r--   0 tar        (210) tar        (210)   146625 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/dxfsl/geom.py
+-rw-r--r--   0 tar        (210) tar        (210)    31058 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/dxfsl/machine.py
+-rw-r--r--   0 tar        (210) tar        (210)    12311 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/dxfsl/plotrenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    44863 2023-07-07 06:13:48.000000 femagtools-1.3.2/femagtools/dxfsl/shape.py
+-rw-r--r--   0 tar        (210) tar        (210)    13239 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/ecloss.py
+-rw-r--r--   0 tar        (210) tar        (210)     1224 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/erg.py
+-rw-r--r--   0 tar        (210) tar        (210)    42422 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/femag.py
+-rw-r--r--   0 tar        (210) tar        (210)     7415 2023-05-17 15:12:10.000000 femagtools-1.3.2/femagtools/forcedens.py
+-rw-r--r--   0 tar        (210) tar        (210)    30989 2023-07-07 06:13:48.000000 femagtools-1.3.2/femagtools/fsl.py
+-rw-r--r--   0 tar        (210) tar        (210)     3017 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/getset.py
+-rw-r--r--   0 tar        (210) tar        (210)     3903 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/gmsh.py
+-rw-r--r--   0 tar        (210) tar        (210)    17166 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/google.py
+-rw-r--r--   0 tar        (210) tar        (210)     1561 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/grid.py
+-rw-r--r--   0 tar        (210) tar        (210)     3738 2023-07-03 13:26:45.000000 femagtools-1.3.2/femagtools/hxy.py
+-rw-r--r--   0 tar        (210) tar        (210)    42052 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/isa7.py
+-rw-r--r--   0 tar        (210) tar        (210)     2790 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/jcf2msh.py
+-rw-r--r--   0 tar        (210) tar        (210)     1779 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/jhb.py
+-rw-r--r--   0 tar        (210) tar        (210)    11320 2023-02-14 18:11:00.000000 femagtools-1.3.2/femagtools/job.py
+-rw-r--r--   0 tar        (210) tar        (210)     2261 2022-08-24 07:36:25.000000 femagtools-1.3.2/femagtools/losscoeffs.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-28 12:08:24.156510 femagtools-1.3.2/femagtools/machine/
+-rw-r--r--   0 tar        (210) tar        (210)     7413 2023-07-03 13:26:45.000000 femagtools-1.3.2/femagtools/machine/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)    11467 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/machine/effloss.py
+-rw-r--r--   0 tar        (210) tar        (210)    38093 2023-07-03 13:37:05.000000 femagtools-1.3.2/femagtools/machine/im.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    51280 2023-07-07 06:13:48.000000 femagtools-1.3.2/femagtools/machine/pm.py
+-rw-r--r--   0 tar        (210) tar        (210)    21743 2023-02-14 18:11:00.000000 femagtools-1.3.2/femagtools/machine/sizing.py
+-rw-r--r--   0 tar        (210) tar        (210)    32810 2023-07-03 13:37:05.000000 femagtools-1.3.2/femagtools/machine/sm.py
+-rw-r--r--   0 tar        (210) tar        (210)    16747 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/machine/utils.py
+-rw-r--r--   0 tar        (210) tar        (210)     1093 2023-02-15 20:03:56.000000 femagtools-1.3.2/femagtools/magnet.py
+-rw-r--r--   0 tar        (210) tar        (210)    39696 2023-07-03 13:26:45.000000 femagtools-1.3.2/femagtools/mcv.py
+-rw-r--r--   0 tar        (210) tar        (210)     1833 2023-02-14 18:11:00.000000 femagtools-1.3.2/femagtools/me.py
+-rw-r--r--   0 tar        (210) tar        (210)    14696 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/model.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-28 12:08:24.157510 femagtools-1.3.2/femagtools/moo/
+-rw-r--r--   0 tar        (210) tar        (210)      175 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/moo/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     5493 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/moo/algorithm.py
+-rw-r--r--   0 tar        (210) tar        (210)    10100 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/moo/population.py
+-rw-r--r--   0 tar        (210) tar        (210)     2391 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/moo/problem.py
+-rw-r--r--   0 tar        (210) tar        (210)     2825 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/moproblem.py
+-rw-r--r--   0 tar        (210) tar        (210)     8506 2023-06-23 19:15:43.000000 femagtools-1.3.2/femagtools/multiproc.py
+-rw-r--r--   0 tar        (210) tar        (210)     1841 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/mxw2msh.py
+-rw-r--r--   0 tar        (210) tar        (210)    12781 2023-02-14 18:11:00.000000 femagtools-1.3.2/femagtools/nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     2052 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/netlist.py
+-rw-r--r--   0 tar        (210) tar        (210)     3099 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/ntib.py
+-rw-r--r--   0 tar        (210) tar        (210)     8685 2023-02-21 19:53:03.000000 femagtools-1.3.2/femagtools/opt.py
+-rw-r--r--   0 tar        (210) tar        (210)    18717 2023-07-03 13:26:45.000000 femagtools-1.3.2/femagtools/parstudy.py
+-rw-r--r--   0 tar        (210) tar        (210)    62239 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/plot.py
+-rw-r--r--   0 tar        (210) tar        (210)     6536 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/poc.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-28 12:08:24.165510 femagtools-1.3.2/femagtools/templates/
+-rw-r--r--   0 tar        (210) tar        (210)      874 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/FE-losses.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3062 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/templates/afm_rotor.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4618 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/templates/afm_stator.mako
+-rw-r--r--   0 tar        (210) tar        (210)      246 2023-07-03 13:26:45.000000 femagtools-1.3.2/femagtools/templates/airgapinduc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2879 2022-09-28 06:51:55.000000 femagtools-1.3.2/femagtools/templates/asyn_motor.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3036 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/templates/basic_modpar.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1911 2023-02-14 18:11:00.000000 femagtools-1.3.2/femagtools/templates/calc_field_ts.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1600 2023-06-23 19:15:43.000000 femagtools-1.3.2/femagtools/templates/calc_therm_field.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1746 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/templates/cogg_calc.mako
+-rw-r--r--   0 tar        (210) tar        (210)      400 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/colorgrad.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1264 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/com_motor_sim.mako
+-rw-r--r--   0 tar        (210) tar        (210)      472 2023-02-14 18:11:00.000000 femagtools-1.3.2/femagtools/templates/conduct-data.mako
+-rw-r--r--   0 tar        (210) tar        (210)      663 2023-06-23 19:15:43.000000 femagtools-1.3.2/femagtools/templates/connect_models.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1339 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/templates/cu_losses.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1672 2023-02-14 18:11:00.000000 femagtools-1.3.2/femagtools/templates/ec-rotorbar.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1983 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/fe-contr.mako
+-rw-r--r--   0 tar        (210) tar        (210)      905 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/templates/fieldcalc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4983 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/templates/gen_winding.mako
+-rw-r--r--   0 tar        (210) tar        (210)      560 2023-02-14 18:11:00.000000 femagtools-1.3.2/femagtools/templates/inductances.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1270 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/ld_lq_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      600 2023-02-14 18:11:00.000000 femagtools-1.3.2/femagtools/templates/leak_dist_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)      770 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/leak_evol_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)      431 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/leak_tooth_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1271 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/magnet-data.mako
+-rw-r--r--   0 tar        (210) tar        (210)      788 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/magnetFC2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2268 2023-06-23 19:15:43.000000 femagtools-1.3.2/femagtools/templates/magnetIron.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1426 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/magnetIron2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2315 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/magnetIron3.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1413 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/magnetIron4.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1376 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/magnetIron5.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3960 2023-06-23 19:15:43.000000 femagtools-1.3.2/femagtools/templates/magnetIronV.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2010 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/magnetSector.mako
+-rw-r--r--   0 tar        (210) tar        (210)      727 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/magnetSectorLinear.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1295 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/magnetShell.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4080 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/magnetShell2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2250 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/templates/mesh-airgap.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2298 2023-02-14 18:11:00.000000 femagtools-1.3.2/femagtools/templates/modal_analysis.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1202 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/mult_cal_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      345 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/new_model.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3209 2023-02-14 18:11:00.000000 femagtools-1.3.2/femagtools/templates/noloadflux-rot.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4661 2023-02-14 18:11:00.000000 femagtools-1.3.2/femagtools/templates/noloadflux.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3146 2023-02-14 18:11:00.000000 femagtools-1.3.2/femagtools/templates/noloadfluxdc.mako
+-rw-r--r--   0 tar        (210) tar        (210)      313 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/open.mako
+-rw-r--r--   0 tar        (210) tar        (210)      630 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/plots.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1373 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/pm_sym_f_cur.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2319 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/pm_sym_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      925 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/pm_sym_loss.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1251 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/psd_psq_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      643 2023-02-14 18:11:00.000000 femagtools-1.3.2/femagtools/templates/ring.mako
+-rw-r--r--   0 tar        (210) tar        (210)      973 2022-09-28 06:51:55.000000 femagtools-1.3.2/femagtools/templates/rot_hsm.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2280 2022-09-28 06:51:55.000000 femagtools-1.3.2/femagtools/templates/rotorAsyn.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1908 2023-02-14 18:11:00.000000 femagtools-1.3.2/femagtools/templates/rotorKs2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1910 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/rotor_msh.mako
+-rw-r--r--   0 tar        (210) tar        (210)      753 2022-09-28 06:51:55.000000 femagtools-1.3.2/femagtools/templates/rotor_winding.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1981 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/shortcircuit.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2077 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/srm.mako
+-rw-r--r--   0 tar        (210) tar        (210)      761 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/stator1.mako
+-rw-r--r--   0 tar        (210) tar        (210)      599 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/stator2.mako
+-rw-r--r--   0 tar        (210) tar        (210)      760 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/templates/stator3Linear.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1179 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/stator4.mako
+-rw-r--r--   0 tar        (210) tar        (210)      893 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/statorBG.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2071 2023-02-14 18:11:00.000000 femagtools-1.3.2/femagtools/templates/statorRing.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4942 2023-06-23 19:15:43.000000 femagtools-1.3.2/femagtools/templates/statorRotor3.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1799 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/templates/stator_msh.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3142 2023-07-03 13:26:45.000000 femagtools-1.3.2/femagtools/templates/therm-dynamic.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1348 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/templates/therm-static.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1729 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/templates/torq_calc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     5791 2022-08-24 07:36:25.000000 femagtools-1.3.2/femagtools/tks.py
+-rw-r--r--   0 tar        (210) tar        (210)    47280 2023-02-14 18:11:00.000000 femagtools-1.3.2/femagtools/ts.py
+-rw-r--r--   0 tar        (210) tar        (210)     1265 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/utils.py
+-rw-r--r--   0 tar        (210) tar        (210)     2444 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/vbf.py
+-rw-r--r--   0 tar        (210) tar        (210)     8595 2022-08-07 12:24:45.000000 femagtools-1.3.2/femagtools/vtu.py
+-rw-r--r--   0 tar        (210) tar        (210)    22310 2023-07-28 12:07:00.000000 femagtools-1.3.2/femagtools/windings.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-28 12:08:24.153510 femagtools-1.3.2/femagtools.egg-info/
+-rw-r--r--   0 tar        (210) tar        (210)     5262 2023-07-28 12:08:24.000000 femagtools-1.3.2/femagtools.egg-info/PKG-INFO
+-rw-r--r--   0 tar        (210) tar        (210)     5170 2023-07-28 12:08:24.000000 femagtools-1.3.2/femagtools.egg-info/SOURCES.txt
+-rw-r--r--   0 tar        (210) tar        (210)        1 2023-07-28 12:08:24.000000 femagtools-1.3.2/femagtools.egg-info/dependency_links.txt
+-rw-r--r--   0 tar        (210) tar        (210)      191 2023-07-28 12:08:24.000000 femagtools-1.3.2/femagtools.egg-info/entry_points.txt
+-rw-r--r--   0 tar        (210) tar        (210)      144 2023-07-28 12:08:24.000000 femagtools-1.3.2/femagtools.egg-info/requires.txt
+-rw-r--r--   0 tar        (210) tar        (210)       11 2023-07-28 12:08:24.000000 femagtools-1.3.2/femagtools.egg-info/top_level.txt
+-rw-r--r--   0 tar        (210) tar        (210)     1369 2023-02-15 20:03:56.000000 femagtools-1.3.2/pyproject.toml
+-rw-r--r--   0 tar        (210) tar        (210)       38 2023-07-28 12:08:24.171510 femagtools-1.3.2/setup.cfg
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-07-28 12:08:24.171510 femagtools-1.3.2/tests/
+-rw-r--r--   0 tar        (210) tar        (210)    10668 2023-07-28 12:07:00.000000 femagtools-1.3.2/tests/test_afpm.py
+-rw-r--r--   0 tar        (210) tar        (210)     1065 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_airgap_induction.py
+-rw-r--r--   0 tar        (210) tar        (210)      646 2023-02-14 18:11:00.000000 femagtools-1.3.2/tests/test_amela.py
+-rw-r--r--   0 tar        (210) tar        (210)     1398 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_asm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    14755 2023-02-14 18:11:00.000000 femagtools-1.3.2/tests/test_bchreader.py
+-rw-r--r--   0 tar        (210) tar        (210)      332 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_conductor.py
+-rw-r--r--   0 tar        (210) tar        (210)     6171 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_convert.py
+-rw-r--r--   0 tar        (210) tar        (210)     1142 2023-07-03 13:36:57.000000 femagtools-1.3.2/tests/test_effloss.py
+-rw-r--r--   0 tar        (210) tar        (210)      523 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_erg.py
+-rw-r--r--   0 tar        (210) tar        (210)     1934 2023-02-16 09:09:33.000000 femagtools-1.3.2/tests/test_femag.py
+-rw-r--r--   0 tar        (210) tar        (210)      533 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_forcedens.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    16099 2023-06-23 19:15:43.000000 femagtools-1.3.2/tests/test_fsl.py
+-rw-r--r--   0 tar        (210) tar        (210)      662 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_im.py
+-rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_isa7.py
+-rw-r--r--   0 tar        (210) tar        (210)      824 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_jhb.py
+-rw-r--r--   0 tar        (210) tar        (210)      981 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_job.py
+-rw-r--r--   0 tar        (210) tar        (210)     2012 2022-08-24 07:36:25.000000 femagtools-1.3.2/tests/test_losscoeffs.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    12881 2023-07-03 13:26:45.000000 femagtools-1.3.2/tests/test_machine.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2608 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_magncurv.py
+-rw-r--r--   0 tar        (210) tar        (210)      276 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_magnet.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2118 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_mcvreader.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     3986 2023-06-23 19:15:43.000000 femagtools-1.3.2/tests/test_mcvwriter.py
+-rw-r--r--   0 tar        (210) tar        (210)      192 2023-02-14 18:11:00.000000 femagtools-1.3.2/tests/test_me.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2372 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_model.py
+-rw-r--r--   0 tar        (210) tar        (210)     3116 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     1340 2023-07-03 13:26:45.000000 femagtools-1.3.2/tests/test_parident.py
+-rw-r--r--   0 tar        (210) tar        (210)     3200 2023-03-02 15:44:17.000000 femagtools-1.3.2/tests/test_parstudy.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     5816 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_pocfile.py
+-rw-r--r--   0 tar        (210) tar        (210)     1109 2023-02-14 18:11:00.000000 femagtools-1.3.2/tests/test_sizing.py
+-rw-r--r--   0 tar        (210) tar        (210)    83524 2023-06-23 19:15:43.000000 femagtools-1.3.2/tests/test_sm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      766 2022-08-24 07:36:25.000000 femagtools-1.3.2/tests/test_tksreader.py
+-rw-r--r--   0 tar        (210) tar        (210)     1825 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_ts.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      832 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_vbfreader.py
+-rw-r--r--   0 tar        (210) tar        (210)      868 2022-08-07 12:24:45.000000 femagtools-1.3.2/tests/test_vtu.py
+-rw-r--r--   0 tar        (210) tar        (210)     4912 2023-03-24 14:45:00.000000 femagtools-1.3.2/tests/test_windings.py
```

### Comparing `femagtools-1.3.1/LICENSE` & `femagtools-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/PKG-INFO` & `femagtools-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femagtools
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python API for FEMAG
 Author-email: Ronald Tanner <tar@semafor.ch>, Dapu Zhang <d.zhan@gtisoft.com>, Beat Holm <hob@semafor.ch>, Günther Amsler <amg@semafor.ch>, Nicolas Mauchle <mau@semafor.ch>
 License: Copyright (c) 2016-2023, Semafor Informatik & Energie AG, Basel
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
```

### Comparing `femagtools-1.3.1/README.md` & `femagtools-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/__init__.py` & `femagtools-1.3.2/femagtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     Python bindings for FEMAG
 
 
 
 """
 __title__ = 'femagtools'
-__version__ = '1.3.1'
+__version__ = '1.3.2'
 __author__ = 'Ronald Tanner'
 __license__ = 'BSD'
 __copyright__ = 'Copyright 2016-2022 SEMAFOR Informatik & Energie AG'
 
 from .asm import read
 from .bch import Reader
 from .model import MachineModel
```

### Comparing `femagtools-1.3.1/femagtools/airgap.py` & `femagtools-1.3.2/femagtools/airgap.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,70 +5,44 @@
 
     Read airgap dat file
 
 
 """
 import numpy as np
 import logging
+from . import utils
 
 logger = logging.getLogger(__name__)
 
 
 def fft(pos, b, pmod=0):
     """calculate fft spectrum of flux density and return samples,
     values, amplitude and phase of base harmonic
 
     Arguments:
       pos: (list of floats) sample positions
       b: (list of floats) flux density values
       pmod: number of poles in model (ignored if 0)
     """
-    model_angle = pos[-1] - pos[0]
-    ntiles = int(round(360/model_angle))
-
-    if pmod:
-        negative_periodic = pmod % 2
-    else:
-        negative_periodic = np.abs(b[0] - b[-1])/np.max(b) > 1
-
-    if negative_periodic:
-        bx = np.append(
-            np.concatenate(
-                [n*b[:-1]
-                 for n in [m % 2 or -1
-                           for m in range(1, ntiles+1)]]),
-            b[0])
-    else:
-        bx = np.append(
-            np.tile(b[:-1], ntiles),
-            b[0])
-
-    N = len(bx)
-    # compute DFT from induction
-    Y = np.fft.fft(bx)
-
-    # find the peak (amplitude of base harmonic)
-    i = np.argmax(np.abs(Y[:N//2]))
-    a = 2*np.abs(Y[i])/N
-    freq = np.fft.fftfreq(N, d=pos[1]-pos[0])
-    T0 = np.abs(1/freq[i])
+    r = utils.fft(pos, b, pmod)
+    Bamp = r['a']
+    alfa0 = r['alfa0']
+    T0 = r['T0']
     npoles = 2*int(np.ceil(360/T0))
     logger.info("flux density: %s poles B amp %f ",
-                npoles, a)
-
-    alfa0 = np.angle(Y[i])
-    return dict(Bamp=a, npoles=npoles,
+                npoles, r['a'])
+    return dict(Bamp=Bamp, npoles=npoles,
                 phi0=alfa0,
                 pos=pos.tolist(),
                 B=b.tolist(),
                 nue=np.arange(0, 9*npoles).tolist(),
-                B_nue=(2*np.abs(Y[:9*npoles])/N).tolist(),
-                B_fft=(a*np.cos(2*np.pi*pos/T0+alfa0)).tolist(),
-                Bi=bx.tolist(),
-                phi=np.linspace(pos[0], 360+pos[0], len(bx)).tolist())
+                B_nue=r['nue'],
+                B_fft=(Bamp*np.cos(2*np.pi*pos/T0+alfa0)).tolist(),
+                Bi=r['yi'],
+                phi=np.linspace(pos[0], 360+pos[0], len(r['yi'])).tolist())
 
 
 def read(filename, pmod=0):
     """read dat file with columns (phi, Br, Bphi)
     returns samples, values, amplitude and phase of base harmonic
 
     Args:
```

### Comparing `femagtools-1.3.1/femagtools/amazon.py` & `femagtools-1.3.2/femagtools/amazon.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/amela.py` & `femagtools-1.3.2/femagtools/amela.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,15 +310,16 @@
                                 nodes=dict(),
                                 elements=dict(),
                                 bndkeys=bndkey[i],
                                 bndx=[float(c) for c in bndx[i]],
                                 bndy=[float(c) for c in bndy[i]],
                                 bl=bl[i],
                                 elcp=elcp[i],
-                                area=spel_area[i]))
+                                area=spel_area[i], 
+                                spel_key=spel_key[i]))
             pm_data[i].update(pos)
 
         for k in range(len(pm_node_key)):
             for i, j in enumerate(pm_node_key[k]):
                 pm_data[k]['nodes'][str(j + 1)] = dict(
                     key=int(j + 1),
                     x=float(r.nodes[j].x*1e3),
```

### Comparing `femagtools-1.3.1/femagtools/asm.py` & `femagtools-1.3.2/femagtools/asm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/bch.py` & `femagtools-1.3.2/femagtools/bch.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,14 +166,15 @@
         self.linearForce = []
         self.linearForce_fft = []
         self.powerSituation = {}
         self.scData = {}
         self.dqPar = {}
         self.ldq = {}
         self.losses = []
+        self.magnet_loss_th = []
         self.demag = []
         self.weights = []
         self.weight = {}
         self.characteristics = []
         self.areas = []
         self.current_angles = []
         self.dispatch = {
@@ -1493,26 +1494,41 @@
                     losses['total'] += rotfe
                 i += 3
                 continue
 
             if l.find('Fe-Losses-Rotor') > -1:
                 rec = self.__findNums(content[i+3])
                 if len(rec) == 2:
-                    if content[i+1].find('Iron') > -1 and content[i+1].find('StJo') > 0:
+                    if (content[i+1].find('Iron') > -1 and content[i+1].find('StJo') > 0 or
+                        content[i+1].split() == ['RoZa', 'RoJo']):
                         self.external_rotor = True
                         # TODO: there might be better places to check this
-                        losses['stajo'] = floatnan(rec[0])
-                        losses['staza'] = floatnan(rec[1])
+                        losses['staza'] = floatnan(rec[0])
+                        losses['stajo'] = floatnan(rec[1])
                         losses['total'] += losses['staza']+losses['stajo']
                     else:
                         losses['rotfe'] = floatnan(rec[1])
                         losses['total'] += losses['rotfe']
                 i += 4
                 continue
 
+            if l.find('Fe-Losses-Stator') > -1:
+                rec = self.__findNums(content[i+3])
+                if len(rec) == 2:
+                    if content[i+1].split() == ['StJo', 'StZa']:
+                        losses['stajo'] = floatnan(rec[0])
+                        losses['staza'] = floatnan(rec[1])
+                        losses['total'] += losses['staza']+losses['stajo']
+
+                    if content[i+1].split() == ['rotf', '----']:
+                        losses['rotfe'] = sum([floatnan(x) for x in rec])
+                        losses['total'] += losses['rotfe']
+                i += 4
+                continue
+
             if l.find('Magnet-Losses') > -1:
                 rec = self.__findNums(content[i+1])
                 if len(rec) == 1:
                     losses['magnetJ'] = float(rec[0])
                     # losses['magnetB'] = float(Nan)
                 if len(rec) == 2:
                     losses['magnetJ'] = float(rec[0])
```

### Comparing `femagtools-1.3.1/femagtools/bchxml.py` & `femagtools-1.3.2/femagtools/bchxml.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/condor.py` & `femagtools-1.3.2/femagtools/condor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/conductor.py` & `femagtools-1.3.2/femagtools/conductor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/config.py` & `femagtools-1.3.2/femagtools/config.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/convert.py` & `femagtools-1.3.2/femagtools/convert.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/dakota.py` & `femagtools-1.3.2/femagtools/dakota.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/dakota_femag.py` & `femagtools-1.3.2/femagtools/dakota_femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/dakotaout.py` & `femagtools-1.3.2/femagtools/dakotaout.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/docker.py` & `femagtools-1.3.2/femagtools/docker.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/dxfsl/area.py` & `femagtools-1.3.2/femagtools/dxfsl/area.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,16 @@
         self.type = 0  # material
         self.phi = 0.0
         self.min_angle = 0.0
         self.max_angle = 0.0
         self.min_air_angle = 0.0
         self.max_air_angle = 0.0
         self.close_to_ag = False
+        self.close_to_ag_startcorner = False
+        self.close_to_ag_endcorner = False
         self.close_to_startangle = False
         self.close_to_endangle = False
         self.mag_rectangle = False
         self.min_dist = 99999.0
         self.max_dist = 0.0
         self.height = 0.0
         self.alpha = 0.0
@@ -1052,14 +1054,20 @@
                 if not self.is_identical(a):
                     if self.is_inside(a):
                         return True
                     elif self.is_touching(a):
                         return True
         return False
 
+    def is_touching_areas(self, areas):
+        for a in areas:
+            if self.is_touching(a):
+                return True
+        return False
+
     def mark_stator_subregions(self,
                                is_inner,
                                stator_size,
                                mirrored,
                                alpha,
                                center,
                                r_in,
@@ -1151,39 +1159,58 @@
 
         if self.close_to_endangle:
             if self.is_half_circle(center, self.max_angle):
                 self.type = 0  # air
                 logger.debug("***** air (part of a circle)\n")
                 return self.type
 
+        def bad_winding_position():
+            if is_inner:
+                radius_third = airgap_radius - (airgap_radius - opposite_radius) * 0.33
+                if self.max_dist < radius_third:
+                    return True
+            else:  # outer
+                radius_third = airgap_radius + (opposite_radius - airgap_radius) * 0.33
+                if self.min_dist > radius_third:
+                    return True
+            return False
+
         if self.min_angle > 0.001:
             if self.max_angle < alpha - 0.001:
-                self.type = 2  # windings
-                logger.debug("***** windings #1\n")
+                if bad_winding_position():
+                    self.type = 12  # windings or air
+                    logger.debug("***** windings or air #1\n")
+                else:
+                    self.type = 2  # windings
+                    logger.debug("***** windings #1\n")
                 return self.type
             if mirrored:
-                self.type = 2  # windings
-                logger.debug("***** windings #2\n")
+                if bad_winding_position():
+                    self.type = 12  # windings or air
+                    logger.debug("***** windings or air #2\n")
+                else:
+                    self.type = 2  # windings
+                    logger.debug("***** windings #2\n")
                 return self.type
 
             self.type = 0  # air
-            logger.debug("***** air #2")
+            logger.debug("***** air #3")
 
         if self.close_to_startangle or self.close_to_endangle:
             f = self.surface / stator_size
             if f < 0.02:  # area_size less then 2 percent of stator size
                 # Luftloch
                 self.type = 0  # air
                 logger.debug("***** small area => air\n")
             else:
                 self.type = 9  # air or iron near windings and near airgap?
                 logger.debug("***** air or iron close to border\n")
             return self.type
 
-        logger.debug("***** air #3\n")
+        logger.debug("***** air #4\n")
         return 0
 
     def mark_rotor_subregions(self, is_inner, mirrored, alpha,
                               center, r_in, r_out):
         logger.debug("mark_rotor_subregions")
 
         alpha = round(alpha, 6)
@@ -1327,14 +1354,23 @@
             logger.debug(">>> iron close to start- and end-angle")
             return self.type
 
         self.type = 0  # air
         logger.debug(">>> air remains")
         return self.type
 
+    def mark_airgap_corners(self, start_cp, end_cp):
+        for n in self.list_of_nodes():
+            if self.close_to_startangle:
+                if points_are_close(n, start_cp):
+                    self.close_to_ag_startcorner = True
+            if self.close_to_endangle:
+                if points_are_close(n, end_cp):
+                    self.close_to_ag_endcorner = True
+
     def area_size(self):
         nodes = [n for n in self.list_of_nodes()]
         return area_size(nodes)
 
     def set_surface(self, mirrored):
         self.surface = self.area_size()
         if self.close_to_endangle and mirrored:
@@ -1463,18 +1499,23 @@
 
             n1_prev = n1
             e_prev = e
         return c
 
     def __str__(self):
         return "Area {}\n".format(self.id) + \
-            "distance: from {} to {}\n".\
+            "distance...............: from {} to {}\n".\
             format(round(self.min_dist, 4), round(self.max_dist, 4)) + \
-            "height..: {}\n".format(self.height) + \
-            "alpha...: {}\n".format(self.alpha) + \
-            "angle...: from {} to {}\n".\
+            "height.................: {}\n".format(self.height) + \
+            "alpha..................: {}\n".format(self.alpha) + \
+            "angle..................: from {} to {}\n".\
             format(round(self.min_angle, 6), round(self.max_angle, 6)) + \
-            "delta...: {}\n".format(self.delta) + \
-            "number..: {}\n".format(self.count) + \
-            "equal...: {}\n".format(len(self.equal_areas)) + \
-            "symmetry: {}\n".format(self.symmetry) + \
-            "sym_type: {}".format(self.sym_type)
+            "delta..................: {}\n".format(self.delta) + \
+            "number.................: {}\n".format(self.count) + \
+            "equal areas............: {}\n".format(len(self.equal_areas)) + \
+            "symmetry...............: {}\n".format(self.symmetry) + \
+            "symmetry type..........: {}\n".format(self.sym_type) + \
+            "close to airgap........: {}\n".format(self.close_to_ag) + \
+            "close to startangle....: {}\n".format(self.close_to_startangle) + \
+            "close to endangle......: {}\n".format(self.close_to_endangle) + \
+            "close to ag startcorner: {}\n".format(self.close_to_ag_startcorner) + \
+            "close to ag endcorner..: {}\n".format(self.close_to_ag_endcorner)
```

### Comparing `femagtools-1.3.1/femagtools/dxfsl/conv.py` & `femagtools-1.3.2/femagtools/dxfsl/conv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/dxfsl/converter.py` & `femagtools-1.3.2/femagtools/dxfsl/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,21 +395,23 @@
                 machine.geom.search_stator_subregions(part[1])
 
                 if machine.has_mirrored_windings():
                     logger.info("undo mirror of stator")
                     machine = machine.undo_mirror()
                     machine.geom.set_stator()
                     machine.geom.search_stator_subregions(part[1])
+                    machine.geom.looking_for_corners()
                     machine.create_mirror_lines_outside_windings()
 
                 params = create_femag_parameters_stator(machine,
                                                         part[1])
             else:
                 machine.geom.set_rotor()
                 machine.geom.search_rotor_subregions(part[1])
+                machine.geom.looking_for_corners()
                 params = create_femag_parameters_rotor(machine,
                                                        part[1])
         else:
             machine.geom.search_subregions()
 
         machine.delete_tiny_elements(mindist)
         machine.geom.create_corner_areas()
```

### Comparing `femagtools-1.3.1/femagtools/dxfsl/corner.py` & `femagtools-1.3.2/femagtools/dxfsl/corner.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/dxfsl/dumprenderer.py` & `femagtools-1.3.2/femagtools/dxfsl/dumprenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/dxfsl/fslrenderer.py` & `femagtools-1.3.2/femagtools/dxfsl/fslrenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/dxfsl/functions.py` & `femagtools-1.3.2/femagtools/dxfsl/functions.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/dxfsl/geom.py` & `femagtools-1.3.2/femagtools/dxfsl/geom.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,14 +272,40 @@
                        rotation=rotation)
             p1 = p2
     if entity.is_closed:
         yield Line(Element(start=p1, end=points[0]), lf,
                    xoff=xoff, yoff=yoff,
                    rotation=rotation)
 
+def ellipse(entity, lf, xoff=0.0, yoff=0.0, rotation=0.0):
+    w = np.linalg.norm(entity.major_axis) * 2
+    h = entity.ratio * w
+    theta = np.arctan2(entity.major_axis[1], entity.major_axis[0])
+    start_angle = entity.start_param
+    end_angle = entity.end_param
+    if end_angle < start_angle:
+        end_angle += 2*np.pi
+    alfa = np.linspace(start_angle, end_angle, 20)
+    x = 0.5 * w * np.cos(alfa)
+    y = 0.5 * h * np.sin(alfa)
+    R = np.array([
+        [np.cos(theta), -np.sin(theta)],
+        [np.sin(theta),  np.cos(theta)]
+    ])
+    x, y = np.dot(R, [x, y])
+    x += entity.center[0]
+    y += entity.center[1]
+    points = np.array((x,y)).T
+    p1 = points[0]
+    for p2 in points[1:]:
+        yield Line(Element(start=p1, end=p2), lf,
+                   xoff=xoff, yoff=yoff,
+                   rotation=rotation)
+        p1 = p2
+
 
 def spline(entity, lf, min_dist=0.001, xoff=0.0, yoff=0.0, rotation=0.0):
     if False:
         yield Line(Element(start=entity.control_points[0],
                            end=entity.control_points[-1]), lf,
                    xoff=xoff, yoff=yoff,
                    rotation=rotation)
@@ -489,30 +515,34 @@
                     yield l
             elif e.dxftype == 'INSERT':
                 logger.debug("Insert of Block %s", e.name)
                 block = dwg.blocks[e.name]
                 for l in insert_block(dwg, e, lf, rf, block, min_dist=mindist):
                     yield l
             elif e.dxftype == 'ELLIPSE':
-                w = np.linalg.norm(e.major_axis) * 2
-                h = e.ratio * w
-                rtheta = np.arctan2(e.major_axis[1], e.major_axis[0])
-                angle = rtheta*180/np.pi
-                start_angle = e.start_param*180/np.pi + angle
-                end_angle = e.end_param*180/np.pi + angle
-                arc = Arc(Element(center=e.center,
-                                  radius=w/2,
-                                  start_angle=start_angle,
-                                  end_angle=end_angle,
-                                  width=w,
-                                  height=h,
-                                  rtheta=rtheta,
-                                  start_param=e.start_param,
-                                  end_param=e.end_param))
-                yield arc
+                for l in ellipse(e, lf):
+                    yield l
+                #w = np.linalg.norm(e.major_axis) * 2
+                #h = e.ratio * w
+                #rtheta = np.arctan2(e.major_axis[1], e.major_axis[0])
+                #angle = rtheta*180/np.pi
+                #start_angle = e.start_param*180/np.pi + angle
+                #end_angle = e.end_param*180/np.pi + angle
+                #if end_angle < start_angle:
+                #    end_angle += 360
+                #arc = Arc(Element(center=e.center,
+                #                  radius=w/2,
+                #                  start_angle=start_angle,
+                #                  end_angle=end_angle,
+                #                  width=w,
+                #                  height=h,
+                #                  rtheta=rtheta,
+                #                  start_param=e.start_param,
+                #                  end_param=e.end_param))
+                #yield arc
 
             elif e.dxftype == 'POINT':
                 logger.debug("Id %d4: type %s ignored", id, e.dxftype)
             elif e.dxftype == '3DFACE':
                 logger.warning(
                     "Id %d4: type %s not implemented", id, e.dxftype)
                 # for l in face3d(e, lf):
@@ -990,20 +1020,36 @@
     def remove_edges(self, edges):
         for e in edges:
             self.remove_edge(e)
 
     def add_line(self, n1, n2, color=None):
         line = Line(Element(start=n1, end=n2), color=color)
         add_or_join(self,
-                    line.node1(ndec),
-                    line.node2(ndec),
+                    n1,
+                    n2,
                     line,
                     self.rtol,
                     self.atol)
 
+    def add_arc(self, n1, n2, center, radius, color=None):
+        angle_n1 = alpha_line(center, n1)
+        angle_n2 = alpha_line(center, n2)
+        arc = Arc(Element(center=center,
+                          radius=radius,
+                          start_angle=angle_n1*180/np.pi,
+                          end_angle=angle_n2*180/np.pi),
+                  color=color)
+        add_or_join(self,
+                    n1,
+                    n2,
+                    arc,
+                    self.rtol,
+                    self.atol)
+
+
     def elements(self, type):
         """return lists of objects"""
         return [e[2]['object'] for e in self.g.edges(data=True)
                 if isinstance(e[2]['object'], type)]
 
     def arcs(self):
         """return lists of arcs"""
@@ -2627,15 +2673,15 @@
         dist_max = 0.0
         for g in gaplist:
             if not less_equal(g[0], dist_max):
                 airgaps.append((dist_max, g[0]))
             dist_max = max(dist_max, g[1])
         return airgaps
 
-    def detect_airgaps(self, center, startangle, endangle, atol):
+    def detect_airgaps(self, center, startangle, endangle, atol=0.1, with_end=False):
         """ Die Funktion sucht Luftspalt-Kandidaten und liefert eine Liste
             von Möglichkeiten mit jeweils einem minimalen und einem maximalen
             Radius als Begrenzung des Luftspalts.
         """
 
         gaplist = []
         for e in self.elements(Shape):
@@ -2647,14 +2693,16 @@
         self.min_radius = gaplist[0][0]
         self.max_radius = gaplist[-1][1]
 
         airgaps = []
         min_radius = self.min_radius + 1.0
         cur_radius = gaplist[0][1]
         max_radius = self.max_radius - 1.0
+        if with_end:
+            max_radius = self.max_radius + 1.0
 
         for g in gaplist:
             if greater(g[0], cur_radius) and \
                greater(cur_radius, min_radius) and \
                less(g[0], max_radius):
                 airgaps.append((cur_radius, g[0]))
 
@@ -3020,21 +3068,39 @@
                     elist = [e for e in a.list_of_equal_edges(w)]
                     logger.debug(" --> %s equal egdes", len(elist))
                     for e in elist:
                         e.init_attributes('lightblue', 'no_fsl')
 
     def search_subregions(self):
         if self.is_stator():
-            return self.search_stator_subregions()
-
-        if self.is_rotor():
-            return self.search_rotor_subregions()
+            self.search_stator_subregions()
+        elif self.is_rotor():
+            self.search_rotor_subregions()
+        else:
+            logger.warning("no stator or rotor assigned")
+            self.search_unknown_subregions()
+        self.looking_for_corners()
+
+    def collect_windings(self):
+        found = True
+        while found:
+            windings = [a for a in self.list_of_areas()
+                        if a.type == 2]
+            bad_windings = [a for a in self.list_of_areas()
+                            if a.type == 12]
+            if not bad_windings:
+                return windings
+
+            found = False
+            for a in bad_windings:
+                if a.is_touching_areas(windings):
+                    a.type = 2
+                    found = True
 
-        logger.warning("no stator or rotor assigned")
-        return self.search_unknown_subregions()
+        return [a for a in self.list_of_areas() if a.type == 2]
 
     def search_stator_subregions(self, place=''):
         logger.debug("Begin of search_stator_subregions")
 
         if place == 'in':
             self.is_inner = True
         elif place == 'out':
@@ -3049,25 +3115,25 @@
                                         stator_size,
                                         self.is_mirrored(),
                                         self.alfa,
                                         self.center,
                                         self.min_radius,
                                         self.max_radius)
 
-        windings = [a for a in self.list_of_areas()
-                    if a.type == 2]
+        windings = self.collect_windings()
+        [a.set_type(0) for a in self.list_of_areas() if a.type == 12]
         windings_found = len(windings)
         logger.info("%d windings found", windings_found)
 
         if windings_found > 1:
             windings_surface = [[w.surface, w] for w in windings]
             windings_surface.sort(reverse=True)
             max_size = windings_surface[0][0]
             for sz, w in windings_surface:
-                logger.info("winding size = %s", sz)
+                logger.debug("winding size = %s", sz)
                 if sz / max_size < 0.95:
                     w.set_type(0)
                     if sz / max_size < 0.2:
                         windings_found -= 1
             windings = [a for a in self.list_of_areas()
                         if a.is_winding()]
             if windings_found > 2 and len(windings) == 1:
@@ -3324,15 +3390,29 @@
                 for a in emb_mag_areas:
                     max_surface = max(max_surface, a.surface)
 
                 for a in emb_mag_areas:
                     if a.surface < max_surface * 0.20:  # too small
                         a.set_type(0)  # air
 
-        logger.debug("begin of search_unknown_subregions")
+        logger.debug("end of search_unknown_subregions")
+
+    def looking_for_corners(self):
+        if self.is_inner:
+            logger.debug("looking_for_corners: inner")
+            start_cp = self.start_corners[-1]
+            end_cp = self.end_corners[-1]
+        else:
+            logger.debug("looking_for_corners: outer")
+            start_cp = self.start_corners[0]
+            end_cp = self.end_corners[0]
+        logger.debug("looking_for_corners: start=%s, end=%s",
+                     start_cp, end_cp)
+        for area in self.list_of_areas():
+            area.mark_airgap_corners(start_cp, end_cp)
         return
 
     def num_areas_of_type(self, type):
         return len([area for area in self.list_of_areas()
                     if area.type == type])
 
     def num_of_windings(self):
@@ -3577,42 +3657,39 @@
         self._remove_edge(n1, n2)
         c = 1
         nbrs = [nbr for nbr in self.g.neighbors(n2)]
         if len(nbrs) == 1:
             c += self.remove_appendix(n2, nbrs[0], incr_text + '.')
         return c
 
-    def split_and_get_intersect_points(self, center, outer_radius, angle):
+    def split_and_get_intersect_points(self, el, aktion=True):
         logger.debug("begin of split_and_get_intersect_points")
         rtol = 1e-03
         atol = 1e-03
-        line = Line(
-            Element(start=center,
-                    end=point(center, outer_radius+1, angle)))
         points = []
         for e in self.elements(Shape):
-            pts = e.intersect_line(line,
-                                   rtol=rtol,
-                                   atol=atol,
-                                   include_end=True)
+            pts = e.intersect_shape(el,
+                                    rtol=rtol,
+                                    atol=atol,
+                                    include_end=True)
             if pts:
                 pts_inside = []
                 pts_real = []
                 for p in pts:
                     if not e.is_point_inside(p, rtol, atol, False):
                         # get the real point
                         if e.get_point_number(p) == 1:
                             pts_real.append(e.p1)
                         else:
                             pts_real.append(e.p2)
                     else:
                         pts_real.append(p)
                         pts_inside.append(p)
 
-                if pts_inside:
+                if pts_inside and aktion:
                     self.remove_edge(e)
                     elements = e.split(pts_inside, rtol, atol)
                     for e in elements:
                         n = self.find_nodes(e.start(), e.end())
                         if distance(n[0], n[1]) == 0.0:
                             logger.debug(
                                 "=== OMIT ELEMENT WITH SAME NODES ===")
@@ -3627,14 +3704,39 @@
         for area in self.list_of_areas():
             if area.is_winding():
                 if area.is_point_inside(p1):
                     if area.is_point_inside(p2):
                         return True
         return False
 
+    def inside_area_list(self, p):
+        for area in self.list_of_areas():
+            if area.is_point_inside(p):
+                yield area
+
+    def critical_touch_point(self, points):
+        logger.debug("looking for critical touch-point")
+        winding_touched = False
+        for p in points[1:]:
+            d = distance(self.center, p)
+            logger.debug("-- p = %s, dist = %s", p, d)
+            for a in self.inside_area_list(p):
+                logger.debug("-- Area type = %s", a.type)
+                logger.debug("        min=%s,  max= %s", a.min_dist, a.max_dist)
+                logger.debug("        close to start = %s", a.close_to_startangle)
+                logger.debug("        close to end   = %s", a.close_to_endangle)
+                if a.is_winding():
+                    winding_touched = True
+                else:
+                    if winding_touched and greater(a.max_dist, d, atol=0.001):
+                        if not (a.close_to_startangle and a.close_to_endangle):
+                            logger.debug("-- return %s", p)
+                            return p
+        return None
+
     def create_lines_outside_windings(self, points):
         if not points:
             return False
         created = False
 
         p1 = points[0]
         for p2 in points[1:]:
@@ -3657,50 +3759,59 @@
     def has_areas_touching_both_sides(self):
         for a in self.area_list:
             if a.is_touching_both_sides():
                 return True
         return False
 
     def get_inner_airgap_line(self):
+        logger.debug("begin of get_inner_airgap_line")
+
         if not self.is_inner:
+            logger.debug("end of get_inner_airgap_line: not inner")
             return []
-        area = [a for a in self.area_list if a.close_to_endangle and a.close_to_ag]
+        for a in self.area_list:
+            logger.debug("%s", a)
+        area = [a for a in self.area_list if a.close_to_ag_endcorner]
         if len(area) != 1:
+            logger.debug("end of get_inner_airgap_line: %s areas found", len(area))
             return []
 
         end_corner = self.end_corners[-1]
         logger.debug("END CORNER %s", end_corner)
         nodes = [n for n in area[0].list_of_nodes()]
         if not nodes:
+            logger.debug("end of get_inner_airgap_line: no nodes found")
             return []
         n1 = nodes[0]
         if points_are_close(end_corner, n1):
             n2 = nodes[-1]
         else:
             n2 = n1
             for n1 in nodes[1:]:
                 if points_are_close(end_corner, n1):
                     break
                 n2 = n1
 
         if not points_are_close(end_corner, n1):
+            logger.debug("end of get_inner_airgap_line: not close to endcorner")
             return []
 
         start_corner = self.start_corners[-1]
 
         logger.debug("EDGE FOUND: %s - %s", n1, n2)
         nodes = [n1, n2]
         info = self.get_edge_info(n1, n2)
         while not points_are_close(start_corner, n2):
             info = self.next_edge_lefthand_side(info)
             if not info:
                 return []
             n2 = info['n2']
             nodes.append(n2)
 
+        logger.debug("end of get_inner_airgap_line #%s", len(nodes))
         return nodes
 
     def create_corner_areas(self):
         self.set_edge_attributes()
         self.create_inner_corner_areas()
 
     def create_and_append_area(self, n1, n2):
@@ -3739,15 +3850,19 @@
             start_cp = start_line.node2(ndec)
             i = 0
             for n in airgap_nodes:
                 i += 1
                 if not self.search_intersection(i, self.max_radius,
                                                 n, start_cp,
                                                 airgap_nodes):
-                    self.add_line(start_cp, n, color='red')
+                    d = distance(self.center, n)
+                    if np.isclose(d, self.max_radius):
+                        self.add_arc(start_cp, n, self.center, self.max_radius, color='red')
+                    else:
+                        self.add_line(start_cp, n, color='red')
                     self.add_edge(cp, start_cp, start_line)
                     self.create_and_append_area(start_cp, n)
                     self.start_corners = self.get_corner_nodes(self.center,
                                                                0.0)
                     break
 
         if not end_exists:
@@ -3758,15 +3873,19 @@
             airgap_nodes.reverse()
             i = 0
             for n in airgap_nodes:
                 i += 1
                 if not self.search_intersection(i, self.max_radius,
                                                 n, end_cp,
                                                 airgap_nodes):
-                    self.add_line(end_cp, n, color='red')
+                    d = distance(self.center, n)
+                    if np.isclose(d, self.max_radius):
+                        self.add_arc(n, end_cp, self.center, self.max_radius, color='red')
+                    else:
+                        self.add_line(end_cp, n, color='red')
                     self.add_edge(cp, end_cp, end_line)
                     self.create_and_append_area(n, end_cp)
                     self.end_corners = self.get_corner_nodes(self.center,
                                                              self.alfa)
                     break
 
     def search_intersection(self, start_i, r, n1, n2, airgap_nodes):
@@ -3784,15 +3903,15 @@
                 # no intersection
                 return  # ok
             if len(pts) != 1:
                 logger.error("-- no intersection found ?!? %s", pts)
                 logger.debug("end of search_intersection: bad")
                 return True  # fatal
             dist_p = distance(self.center, pts[0])
-            logger.info("-- check point %s[%s] -- %s[%s]", n, dist_n, pts[0], dist_p)
+            logger.debug("-- check point %s[%s] -- %s[%s]", n, dist_n, pts[0], dist_p)
             if not less(dist_n, dist_p):
                 logger.debug("end of search_intersection: found")
                 return True  # intersection
             logger.debug("-- dist %s <= %s", dist_n, dist_p)
         logger.debug("end of search_intersection: ok")
         return False  # ok
```

### Comparing `femagtools-1.3.1/femagtools/dxfsl/machine.py` & `femagtools-1.3.2/femagtools/dxfsl/machine.py`

 * *Files 6% similar despite different names*

```diff
@@ -709,29 +709,106 @@
 
     def search_subregions(self):
         self.geom.search_subregions()
 
     def delete_tiny_elements(self, mindist):
         self.geom.delete_tiny_elements(mindist)
 
+    def create_arc(self, radius):
+        arc = Arc(Element(center=self.center,
+                          radius=radius,
+                          start_angle=(self.startangle-0.1)*180/np.pi,
+                          end_angle=(self.endangle+0.1)*180/np.pi),
+                  color='red')
+        pts = self.geom.split_and_get_intersect_points(arc)
+        if len(pts) != 2:
+            logger.warning("create_arc(): Bad Points: %s", pts)
+            # self.geom.add_edge(arc.node1(4), arc.node2(4), arc)
+            return False
+
+        arc = Arc(Element(center=self.center,
+                          radius=radius,
+                          start_angle=self.startangle*180/np.pi,
+                          end_angle=self.endangle*180/np.pi))
+        n = self.geom.find_nodes(pts[0], pts[1])
+        self.geom.add_edge(n[0], n[1], arc)
+        return True
+
+    def get_iron_separator(self, radius_list):
+        if len(radius_list) < 2:
+            return 0.0
+
+        r_min = radius_list[0][0]
+        for r in radius_list[1:]:
+            if np.isclose(r[2], r_min, atol=0.001):
+                return r[2]
+            r_min = r[0]
+
+        return 0.0
+
     def create_mirror_lines_outside_windings(self):
+        logger.debug("create_mirror_lines_outside_windings")
+
         if not self.geom.has_areas_touching_both_sides():
+            logger.debug("end create_mirror_lines_outside_windings: not done")
             return
 
+        radius = self.radius+10
+        ag_list = self.geom.detect_airgaps(self.center,
+                                           self.startangle, self.endangle,
+                                           atol=0.001,
+                                           with_end=True)
+        radius_list = [(ag[0], (ag[0] + ag[1]) / 2, ag[1]) for ag in ag_list]
+        radius_list.sort(reverse=True)
+
         midangle = middle_angle(self.startangle, self.endangle)
-        pts = self.geom.split_and_get_intersect_points(self.center,
-                                                       self.radius+10,
-                                                       midangle)
+        line = Line(
+            Element(start=self.center,
+                    end=point(self.center, radius, midangle)))
+
+        pts = self.geom.split_and_get_intersect_points(line, aktion=False)
         pts.sort()
+
+        p_critical = self.geom.critical_touch_point(pts)
+        if p_critical:
+            d_critical = distance(self.center, p_critical)
+            logger.info("Critical Point: %s, len=%s", p_critical, d_critical)
+            sep_radius = self.get_iron_separator(radius_list)
+            logger.debug("Iron Separator found: %s", sep_radius)
+            if sep_radius > 0.0 and sep_radius < d_critical:
+                radius = sep_radius
+            else:
+                for r in radius_list:
+                    logger.debug("Gap Radius = %s", r[1])
+                    if r[1] < d_critical:
+                        if self.create_arc(r[1]):
+                            radius = r[1]
+                        break
+#        else:
+#            sep_radius = self.get_iron_separator(radius_list)
+#            if sep_radius > 0.0:
+#                logger.debug("Iron Separator found: %s", sep_radius)
+#                radius = sep_radius
+
+        # install line
+        line = Line(
+            Element(start=self.center,
+                    end=point(self.center, radius, midangle)))
+
+        pts = self.geom.split_and_get_intersect_points(line)
+        pts.sort()
+
         if self.geom.create_lines_outside_windings(pts):
             self.geom.area_list = []
             logger.debug("create subregions again")
             self.geom.create_list_of_areas()
             self.geom.search_subregions()
 
+        logger.debug("end create_mirror_lines_outside_windings")
+
     def check_and_correct_geom(self, what):
         geom = self.geom.check_geom(what)
         if geom:
             logger.warning("=== Angle correction (%s) ===", what)
             self.geom = geom
             self.startangle = 0.0
             self.endangle = self.geom.alfa
```

### Comparing `femagtools-1.3.1/femagtools/dxfsl/plotrenderer.py` & `femagtools-1.3.2/femagtools/dxfsl/plotrenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/dxfsl/shape.py` & `femagtools-1.3.2/femagtools/dxfsl/shape.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/ecloss.py` & `femagtools-1.3.2/femagtools/ecloss.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         super().__init__(workdir, magnet_data=dict(name=modelname))
         self.pm = self.get_magnet_data_all(ibeta)
         self.theta = self.pm[-1][-1]['phi'] # rotor pos
         self.speed = kwargs.get('speed', self.pm[-1][-1]['speed'])
         self.tgrid = 60/self.speed*(self.theta[-1] - self.theta[0])/360
         self.lt = len(self.theta)
         self.ls = self.pm[-1][-1]['ls']
-
+        self.th_loss = []
         try:
             self.numpoles = self.pm[-1][-1]['numpoles']
         except KeyError: 
             self.numpoles = 1
 
         try:
             self.mur = kwargs.get('mur', self.pm[-1][-1]['mur'])
@@ -347,15 +347,15 @@
                 for c in range(lfft):
                     for iy in range(ny):
                         for ix in range(nx):
                             if self.is_x and nu[ix] < 2:
                                 with warnings.catch_warnings():
                                     warnings.simplefilter('ignore')
                                     px_se[iy,ix,c] = self.calc_pvpm(bx_fft[iy,ix,c], max(c/self.tgrid, 1e-6),
-                                                                    mu[iy], wm/self.segx[jj], hm, 0)
+                                                                    mu[iy], hm, wm/self.segx[jj], 0)
                                 
                             if mu[iy] < 2:
                                 with warnings.catch_warnings():
                                     warnings.simplefilter('ignore')
                                     py_se[iy,ix,c] = self.calc_pvpm(by_fft[iy,ix,c], max(c/self.tgrid, 1e-6),
                                                                     nu[ix], wm/self.segx[jj], hm, 0)
                 py_sum = np.sum(py_se)
@@ -370,22 +370,24 @@
         Returns 
         --------------
         all_load_cases: list of losses for all load cases
         '''
         all_load_cases = []
         for k in self.pm:
             ialh_loss = 0
+            loss_detail = []
             for i in k: 
                 logger.info(f'magnet width and height: {i["wm"]:.2f}mm {i["hm"]:.2f}mm')
                 [nt, bx_fft, by_fft] = self.periodicity_id(i['bl'])
                 [nx, ny] = ngrid(i['wm'], i['hm'], i['elcp'])
                 keyset = ('wm', 'hm')
                 for j in keyset: 
                     i[j]*=1e-3
                 self.consider_bx(i['wm'], i['hm'], bx_fft, by_fft)
                 bfft = self.bpm_fft(nx, ny, nt, i['elcp'], i['bl'])
-                #loss = self.loss(bfft[0], bfft[1], bfft[2], bfft[3], i['wm'], i['hm'])
                 loss = self.loss(*bfft, i['wm'], i['hm'])
                 ialh_loss += loss
+                loss_detail.append([i['spel_key'], loss/self.numpoles])
+            self.th_loss.append(loss_detail)
             all_load_cases.append(ialh_loss)
 
         return all_load_cases
```

### Comparing `femagtools-1.3.1/femagtools/erg.py` & `femagtools-1.3.2/femagtools/erg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/femag.py` & `femagtools-1.3.2/femagtools/femag.py`

 * *Files 1% similar despite different names*

```diff
@@ -488,15 +488,16 @@
             if simulation['calculationMode'] == 'therm-dynamic':
                 temp = [[float(n) for n in l.split()]
                         for l in (pathlib.Path(self.workdir) / 'temperature.dat').read_text().split('\n') if l]
                 ttemp = list(zip(*temp))
                 return {'t': ttemp[0], 'temperature': ttemp[1]}
 
             bch = self.read_bch(self.modelname)
-            if simulation['calculationMode'] == 'pm_sym_fast':
+            if simulation['calculationMode'] == 'pm_sym_fast' or \
+                simulation['calculationMode'] == 'torq_calc':
                 if simulation.get('shortCircuit', False):
                     logger.info("short circuit simulation")
                     simulation.update(
                         get_shortCircuit_parameters(bch,
                                                     simulation.get('initial', 2)))
 
                     builder = femagtools.fsl.Builder(self.templatedirs)
@@ -546,14 +547,19 @@
                 if len(ops) != len(bch.losses): 
                     magn_losses.insert(0, magn_losses[0])
                 try:
                     for i in range(len(bch.losses)): 
                         bch.losses[i].update({"magnetH": magn_losses[i]})
                 except: 
                     pass
+                # pass losses to bch object for th usage
+                try: 
+                    bch.magnet_loss_th = m.th_loss
+                except: 
+                    pass
             return bch
         return dict(status='ok', message=self.modelname)
 
 
 class FemagTask(threading.Thread):
     def __init__(self, port, args, workdir, logdir):
         threading.Thread.__init__(self)
```

### Comparing `femagtools-1.3.1/femagtools/forcedens.py` & `femagtools-1.3.2/femagtools/forcedens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/fsl.py` & `femagtools-1.3.2/femagtools/fsl.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/getset.py` & `femagtools-1.3.2/femagtools/getset.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/gmsh.py` & `femagtools-1.3.2/femagtools/gmsh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/google.py` & `femagtools-1.3.2/femagtools/google.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/grid.py` & `femagtools-1.3.2/femagtools/grid.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/hxy.py` & `femagtools-1.3.2/femagtools/hxy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/isa7.py` & `femagtools-1.3.2/femagtools/isa7.py`

 * *Files 4% similar despite different names*

```diff
@@ -192,15 +192,17 @@
         self.pos_el_fe_induction = []
 
         if NUM_FE_EVAL_MOVE_STEP > 1:
             self.pos_el_fe_induction = self.next_block("f")
             self.el_fe_induction_1.append([[]])
             self.el_fe_induction_2.append([[]])
             for i in range(NUM_FE_EVAL_MOVE_STEP + 1):
-                self.el_fe_induction_1[0][0].append(self.next_block("h"))
+                b = self.next_block("h")
+                logger.debug("el_fe_induction move step %d: %d", i, len(b))
+                self.el_fe_induction_1[0][0].append(b)
                 self.el_fe_induction_2[0][0].append(self.next_block("h"))
 
         FC_NUM_MOVE_CALC_LOAD_PMS, FC_NUM_FLX = self.next_block("i")[0:2]
 
         if FC_NUM_MOVE_CALC_LOAD_PMS > 1:
             self.skip_block(4)
             self.skip_block(3 * FC_NUM_FLX)
@@ -266,15 +268,17 @@
         FC_NUM_MOVE_LOSSES = self.next_block("i")[0]
 
         if FC_NUM_MOVE_LOSSES > 1 and NUM_FE_EVAL_MOVE_STEP > 1:
             self.el_fe_induction_1.append([[]])
             self.el_fe_induction_2.append([[]])
             self.eddy_cu_vpot.append([[]])
             for i in range(NUM_FE_EVAL_MOVE_STEP + 1):
-                self.el_fe_induction_1[1][0].append(self.next_block("h"))
+                b = self.next_block("h")
+                logger.debug("el_fe_induction move losses step %d: %d", i, len(b))
+                self.el_fe_induction_1[1][0].append(b)
                 self.el_fe_induction_2[1][0].append(self.next_block("h"))
             for i in range(NUM_FE_EVAL_MOVE_STEP + 1):
                 self.eddy_cu_vpot[1][0].append(self.next_block("h"))
 
         # VIRGIN_PM_SYN
         self.skip_block(3)
         # magnet iron 4
@@ -331,15 +335,18 @@
 
         if (FC_NUM_MOVE_LOSSES > 2 and NUM_FE_EVAL_MOVE_STEP > 1
                 and FC_NUM_BETA_ID > 1):
             self.el_fe_induction_1.append([[]])
             self.el_fe_induction_2.append([[]])
             self.eddy_cu_vpot.append([[]])
             for i in range(NUM_FE_EVAL_MOVE_STEP + 1):
-                self.el_fe_induction_1[2][0].append(self.next_block("h"))
+                b = self.next_block("h")
+                logger.debug("el_fe_induction move losses (2) step %d: %d",
+                            i, len(b))
+                self.el_fe_induction_1[2][0].append(b)
                 self.el_fe_induction_2[2][0].append(self.next_block("h"))
             for i in range(NUM_FE_EVAL_MOVE_STEP + 1):
                 self.eddy_cu_vpot[2][0].append(self.next_block("h"))
 
         self.skip_block()
         self.skip_block(2 * 3)  # MAX_LOSS_EVAL_STEPS
         try:
@@ -684,33 +691,39 @@
             pass
         self.pos_el_fe_induction = np.asarray(reader.pos_el_fe_induction)
         try:
             self.beta_loss = np.asarray(reader.beta_loss)
             self.curr_loss = np.array([c/np.sqrt(2) for c in reader.curr_loss])
         except AttributeError:
             pass
-        logger.debug(reader.el_fe_induction_1)
-        if len(np.asarray(reader.el_fe_induction_1).shape) > 2:
-            self.el_fe_induction_1 = np.asarray(
-                reader.el_fe_induction_1).T/1000
-            self.el_fe_induction_2 = np.asarray(
-                reader.el_fe_induction_2).T/1000
-            self.eddy_cu_vpot = np.asarray(reader.eddy_cu_vpot).T/1000
-        else:
-            try:
-                self.el_fe_induction_1 = np.asarray(
-                    [e for e in reader.el_fe_induction_1 if e[0]]).T/1000
-                self.el_fe_induction_2 = np.asarray(
-                    [e for e in reader.el_fe_induction_2 if e[0]]).T/1000
-                self.eddy_cu_vpot = np.asarray(
-                    [e for e in reader.eddy_cu_vpot if e[0]]).T/1000
-                logger.debug('El Fe Induction %s', np.asarray(
-                    reader.el_fe_induction_1).shape)
-            except:
-                pass
+
+        try:
+            el_fe_ind = [np.array(reader.el_fe_induction_1).T/1000,
+                         np.array(reader.el_fe_induction_2).T/1000]
+            eddy_cu_vpot = np.array(reader.eddy_cu_vpot).T/1000
+        except (ValueError, TypeError) as e:
+            # inhomogenous array
+            l = len(reader.el_fe_induction_1[0][0])
+            shape = []
+            for i in reader.el_fe_induction_1:
+                for j in i:
+                    n = 0
+                    for k in j:
+                        if len(k) < l:
+                            break
+                        n += 1
+                    if n > 0:
+                        shape.append(n)
+            el_fe_ind = [np.array([[reader.el_fe_induction_1[0][0][:shape[0]]]]).T/1000,
+                         np.array([[reader.el_fe_induction_2[0][0][:shape[0]]]]).T/1000]
+            eddy_cu_vpot = np.array([[reader.eddy_cu_vpot[0][0][:shape[0]]]]).T/1000
+
+        self.el_fe_induction_1 = el_fe_ind[0]
+        self.el_fe_induction_2 = el_fe_ind[1]
+        self.eddy_cu_vpot = eddy_cu_vpot
 
         self.iron_loss_coefficients = getattr(
             reader, 'iron_loss_coefficients', [])
 
     def get_subregion(self, name):
         """return subregion by name"""
         for s in self.subregions:
```

### Comparing `femagtools-1.3.1/femagtools/jcf2msh.py` & `femagtools-1.3.2/femagtools/jcf2msh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/jhb.py` & `femagtools-1.3.2/femagtools/jhb.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/job.py` & `femagtools-1.3.2/femagtools/job.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/losscoeffs.py` & `femagtools-1.3.2/femagtools/losscoeffs.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/machine/__init__.py` & `femagtools-1.3.2/femagtools/machine/__init__.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/machine/effloss.py` & `femagtools-1.3.2/femagtools/machine/effloss.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,18 @@
         plmag = np.zeros(ntmesh.shape[1])
         plcu1 = np.array(r['plcu1'])
         plcu2 = np.array(r['plcu2'])
         iqd = np.zeros(ntmesh.shape)
         u1 = np.array(r['u1'])
         i1 = np.array(r['i1'])
         try:
-            tfric = eecpars['kfric_b']*eecpars['rotor_mass']*30e-3/np.pi
+            if isinstance(eecpars, dict):
+                tfric = eecpars['kfric_b']*eecpars['rotor_mass']*30e-3/np.pi
+            else:
+                tfric = m.tfric
         except KeyError:
             tfric = 0
 
     plfric = 2*np.pi*ntmesh[0]*tfric
     if not with_tmech:
         ntmesh[1] -= tfric
     pmech = np.array(
```

### Comparing `femagtools-1.3.1/femagtools/machine/im.py` & `femagtools-1.3.2/femagtools/machine/im.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/machine/pm.py` & `femagtools-1.3.2/femagtools/machine/pm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/machine/sizing.py` & `femagtools-1.3.2/femagtools/machine/sizing.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/machine/sm.py` & `femagtools-1.3.2/femagtools/machine/sm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/machine/utils.py` & `femagtools-1.3.2/femagtools/machine/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,14 +342,15 @@
 
     optional arguments:
     num_cur_steps: number of current steps (default 5)
     num_beta_steps: number of current steps (default 7 per quadrant)
     speed: rotor speed in 1/s (default 160/p)
     i1_max: maximum current in A rms (default approx 3*i1nom)
     period_frac: fraction of rotating angle (default 6)
+    cmd: femag executable
     """
     import pathlib
 
     da1 = machine['outer_diam']
     Q1 = machine['stator']['num_slots']
     slotmodel = [k for k in machine['stator'] if isinstance(
         machine['stator'][k], dict)][-1]
@@ -364,21 +365,24 @@
     i1_max = round(0.28*np.pi*hs*(da1+hs)/Q1/N*Jmax*1e5)*10 * \
         machine['windings'].get('num_par_wdgs', 1)
     period_frac = kwargs.get('period_frac', 6)
     if machine.get('external_rotor', False):
         period_frac = 1  # TODO: missing femag support
 
     # winding resistance
-    yd = machine['windings'].get('coil_span', Q1/machine['poles'])
-    wdg = windings.Winding(
-        {'Q': machine['stator']['num_slots'],
-         'm': machine['windings']['num_phases'],
-         'p': machine['poles']//2,
-         'l': machine['windings']['num_layers'],
-         'yd': yd})
+    wpar = {'Q': machine['stator']['num_slots'],
+            'm': machine['windings']['num_phases'],
+            'p': machine['poles']//2}
+
+    if 'coil_span' in machine['windings']:
+        wpar['yd'] = machine['windings']['coil_span']
+    if 'num_layers' in machine['windings']:
+        wpar['l'] = machine['windings']['num_layers']
+
+    wdg = windings.Winding(wpar)
 
     lfe = machine['lfe']
     g = machine['windings'].get('num_par_wdgs', 1)
     if 'wire_gauge' in machine['windings']:
         aw = machine['windings']['wire_gauge']
     elif 'dia_wire' in machine['windings']:
         aw = np.pi*machine['windings'].get('dia_wire', 1e-3)**2/4
@@ -397,15 +401,15 @@
             {"values": n*[-90, -180], "name": "beta_min"}
         ]
     }
 
     parvar = parstudy.List(
         workdir, condMat=condMat,
         magnetizingCurves=magnetizingCurves,
-        magnets=magnetMat)
+        magnets=magnetMat, cmd=kwargs.get('cmd', None))
 
     leakfile = pathlib.Path(workdir) / 'end_wind_leak.dat'
     leakfile.unlink(missing_ok=True)
 
     simulation = dict(
         calculationMode='ld_lq_fast',
         i1_max=kwargs.get('i1_max', i1_max),
```

### Comparing `femagtools-1.3.1/femagtools/magnet.py` & `femagtools-1.3.2/femagtools/magnet.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/mcv.py` & `femagtools-1.3.2/femagtools/mcv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/me.py` & `femagtools-1.3.2/femagtools/me.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/model.py` & `femagtools-1.3.2/femagtools/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 
 
 """
 import logging
 import string
 import numpy as np
+from . import windings
 
 logger = logging.getLogger(__name__)
 #
 # Set of legal model name chars
 # 0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ
 MODELNAME_CHARS = string.printable[:63] + "-_äöüéè"
 # maximum name length
@@ -152,16 +153,25 @@
             self.exit_on_end = 'false'
         if 'magnet' in parameters:
             if 'mcvkey_mshaft' in self.magnet:
                 self.magnet['mcvkey_shaft'] = self.magnet['mcvkey_mshaft']
             for mcv in ('mcvkey_yoke', 'mcvkey_shaft'):
                 if mcv not in self.magnet:
                     self.magnet[mcv] = 'dummy'
-        if 'coord_system' in parameters:
+        if 'coord_system' in parameters or 'afmtype' in parameters:
             self.move_action = 1
+            wdg = windings.Winding({'Q': self.stator['num_slots'],
+                                    'p': self.poles//2,
+                                    'm': self.windings.get('num_phases', 3),
+                                    'l': self.windings.get('num_layers', 1)})
+            self.windings['wdgscheme'] = ''.join([
+                '{'] + [','.join([''.join(['{']+[','.join([''.join([
+                    '{', ','.join(
+                        [str(n) for n in z]), '}']) for z in l])] + ['}'])
+                                  for l in wdg.zoneplan()])] + ['}'])
         else:
             self.coord_system = 0
             self.move_action = 0
 
         try:
             self.set_num_slots_gen()
         except (AttributeError):
```

### Comparing `femagtools-1.3.1/femagtools/moo/algorithm.py` & `femagtools-1.3.2/femagtools/moo/algorithm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/moo/population.py` & `femagtools-1.3.2/femagtools/moo/population.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/moo/problem.py` & `femagtools-1.3.2/femagtools/moo/problem.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/moproblem.py` & `femagtools-1.3.2/femagtools/moproblem.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/multiproc.py` & `femagtools-1.3.2/femagtools/multiproc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/mxw2msh.py` & `femagtools-1.3.2/femagtools/mxw2msh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/nc.py` & `femagtools-1.3.2/femagtools/nc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/netlist.py` & `femagtools-1.3.2/femagtools/netlist.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/ntib.py` & `femagtools-1.3.2/femagtools/ntib.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/opt.py` & `femagtools-1.3.2/femagtools/opt.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/parstudy.py` & `femagtools-1.3.2/femagtools/parstudy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/plot.py` & `femagtools-1.3.2/femagtools/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,28 +225,31 @@
         markerline1, stemlines1, _ = ax.stem(order, fluxdens, '-.', basefmt=" ",
                                              use_line_collection=True)
         ax.set_xticks(order)
     except ValueError:  # empty sequence
         pass
 
 
-def torque(pos, torque, ax=0):
+def torque(pos, torque, title='', ax=0):
     """creates plot from torque vs position"""
     k = 20
     alpha = np.linspace(pos[0], pos[-1],
                         k*len(torque))
     f = ip.interp1d(pos, torque, kind='quadratic')
     unit = 'Nm'
     scale = 1
     if np.min(torque) < -9.9e3 or np.max(torque) > 9.9e3:
         scale = 1e-3
         unit = 'kNm'
     if ax == 0:
         ax = plt.gca()
-    ax.set_title('Torque / {}'.format(unit))
+    if title:
+        ax.set_title(title)
+    else:
+        ax.set_title('Torque / {}'.format(unit))
     ax.grid(True)
     ax.plot(pos, [scale*t for t in torque], 'go')
     ax.plot(alpha, scale*f(alpha))
     if np.min(torque) > 0 and np.max(torque) > 0:
         ax.set_ylim(bottom=0)
     elif np.min(torque) < 0 and np.max(torque) < 0:
         ax.set_ylim(top=0)
@@ -1340,16 +1343,17 @@
       isa: Isa7/NC object
     """
     if subreg:
         if isinstance(subreg, list):
             sr = subreg
         else:
             sr = [subreg]
-        elements = [e for s in sr for sre in isa.get_subregion(s).elements()
-                    for e in sre]
+        elements = [e
+                    for s in sr
+                    for e in isa.get_subregion(s).elements()]
     else:
         elements = [e for e in isa.elements]
 
     lossd = np.array([e.loss_density*1e-3 for e in elements])
     _contour(ax, 'Loss Density kW/m³', elements, lossd)
 
 
@@ -1770,31 +1774,51 @@
             bnd[1].append((n0, t0))
             bnd[0].append((nx, tx))
             n0 = nx
         t0 = tx
     bnd[1].append((nx, tx))
     return np.array(bnd[0] + bnd[1][::-1])
 
-def normalize10(v):
+def normalize10(v, **kwargs):
     """
     Normalizes the input-array using the nearest (ceiling) power of 10.
 
     Arguments:
         v: array to normalize
 
     Returns:
         normalized array
         normalisation factor (power of 10)
     """
-    norm = 10**(np.ceil(np.log10(np.max(np.abs(v)))))
+    n_type = kwargs.get('n_type', 'abs') # 'norm')
+    r_type = kwargs.get('r_type', 'round') # 'floor')
+    if n_type == 'norm':
+        norm = np.log10(np.linalg.norm(v))
+    elif n_type == 'abs':
+        norm = np.log10(np.max(np.abs(v)))
+    else:
+        raise AttributeError('Unknown norm-type. Allowed values are: "norm", "abs".')
+
+    if r_type == 'floor':
+        norm = 10 ** np.floor(norm)
+    elif r_type == 'ceil':
+        norm = 10 ** np.ceil(norm)
+    elif r_type == 'round':
+        norm = 10 ** np.round(norm)
+    else:
+        raise AttributeError('Unknown rounding type. Allowed values are: "floor", "ceil", "round".')
+    # norm = 10**(np.ceil(np.log10(np.max(np.abs(v)))))
+    # norm = 10 ** (np.ceil(np.log10(np.linalg.norm(v))))
+    # norm = 10 ** (np.floor(np.log10(np.max(np.abs(v)))))
+    # norm = 10 ** (np.floor(np.log10(np.linalg.norm(v))))
     return v / norm, norm
 
 
 def plot_contour(speed, torque, z, ax, title='', levels=[],
-                 clabel=True, cmap='YlOrRd', cbar=False):
+                 clabel=True, cmap='YlOrRd', cbar=False, **kwargs):
     """ contour plot of speed, torque, z values
     Arguments:
     levels: (list of floats)
     clabel: contour labels if True
     cmap: colour map
     cbar: (bool) create color bar if True (default False)
 
@@ -1803,16 +1827,16 @@
     returns tricontourf, xscale, yscale
     """
     from matplotlib.path import Path
     from matplotlib.patches import PathPatch
     x = 60*np.asarray(speed)
     y = np.asarray(torque)
 
-    x, xscale = normalize10(x)
-    y, yscale = normalize10(y)
+    x, xscale = normalize10(x, **kwargs)
+    y, yscale = normalize10(y, **kwargs)
 
     if not levels:
         if max(z) <= 1:
             if max(z) > 0.96:
                 levels = [0.5, 0.75, 0.8, 0.84,
                           0.89, 0.92, 0.94, 0.96, 0.97]
             else:
```

### Comparing `femagtools-1.3.1/femagtools/poc.py` & `femagtools-1.3.2/femagtools/poc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/FE-losses.mako` & `femagtools-1.3.2/femagtools/templates/FE-losses.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/asyn_motor.mako` & `femagtools-1.3.2/femagtools/templates/asyn_motor.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/basic_modpar.mako` & `femagtools-1.3.2/femagtools/templates/basic_modpar.mako`

 * *Files 9% similar despite different names*

```diff
@@ -10,43 +10,47 @@
 % endif
 % else:
 ag = 0
 % endif
 % if model.move_action == 0:
 % if model.external_rotor:
 dy2 = ${model.get(['outer_diam'])*1e3}
+% if hasattr(model, 'bore_diam'):
 % if isinstance(model.get(['bore_diam']), list):
 <%
 da2 = '{' + ','.join([str(x*1e3) for x in model.get(['bore_diam'])]) +'}'
 %>
 da2 = ${da2}
 da1 = {}
 for i=1, table.getn(ag) do
   da1[i] = da2[i] - 2*ag[i]
 end
 % else:  # bore_diam is scalar
 da2 = ${model.get(['bore_diam'])*1e3}
 da1 = da2 - 2*ag
 % endif
+% endif # bore_diam dos not exist
 dy1 = ${model.get(['inner_diam'])*1e3}
 % else: # internal rotor
 dy1 = ${model.get(['outer_diam'])*1e3}
+% if hasattr(model, 'bore_diam'):
 % if isinstance(model.get(['bore_diam']), list):
 <%
 da1 = '{' + ','.join([str(x*1e3) for x in model.get(['bore_diam'])]) +'}'
 %>
 da1 = ${da1}
 da2 = {}
 for i=1, table.getn(ag) do
   da2[i] = da1[i] - 2*ag[i]
 end
 % else: # bore_diam is scalar
 da1 = ${model.get(['bore_diam'])*1e3}
 da2 = da1 - 2*ag
 % endif
+% endif
 % if hasattr(model, 'shaft_diam'):
 dy2 = ${model.get(['shaft_diam'])*1e3}
 dsh = ${model.get(['inner_diam'])*1e3}
 % else:
 dy2 = ${model.get(['inner_diam'])*1e3}
 % endif
 % endif
@@ -62,25 +66,42 @@
 m.num_sl_gen      =   ${int(model.get(['rotor','num_slots_gen']))}
 % endif
 m.num_poles       =   ${int(model.get(['poles']))}
 m.num_pol_pair    =   m.num_poles/2
 m.num_slots       =   m.num_sl_gen
 m.npols_gen       =   m.num_poles * m.num_sl_gen / m.tot_num_slot
 m.tot_num_sl      =   m.tot_num_slot
-% if model.move_action == 0:
+% if model.move_action == 0:  # rotating
+% if hasattr(model, 'bore_diam'):
 % if isinstance(model.get(['bore_diam']), list):
 m.fc_radius       =   (da1[2]/2-ag[2]/2) -- Radius airgap (extern)
 m.fc_radius1      =   (da1[1]/2-ag[1]/2) -- Radius airgap (intern?)
 m.fc_radius2 = 	m.fc_radius1
 % else:
 m.fc_radius       =   (da1+da2)/4
 m.fc_radius1      =   m.fc_radius
 m.sl_radius       =   m.fc_radius      -- radius of sliding area
 % endif
 % endif
+% elif hasattr(model, 'pole_width'):  # move action linear
+m.pole_width      = ${model['pole_width']*1e3}
+% endif
+% if hasattr(model, 'lfe'):
 m.arm_length      =   ${model.get(['lfe'])*1e3}
+% endif
 pre_models("basic_modpar")
 % endif
 % if hasattr(model, 'num_agnodes'):
-num_agnodes = ${model.num_agnodes}
+num_agnodes = m.npols_gen*${model.num_agnodes}
+% if hasattr(model, 'bore_diam'):
 agndst = 2*math.pi*m.fc_radius/num_agnodes
+% else:
+if m.pole_width ~= nil then
+  agndst = 2*m.pole_width/num_agnodes
+else
+  agndst = 1 -- last resort
+end
+% endif
 % endif
+% if hasattr(model, 'afmtype'):
+m.model_type      =  "${model['afmtype']}"
+% endif
```

### Comparing `femagtools-1.3.1/femagtools/templates/calc_field_ts.mako` & `femagtools-1.3.2/femagtools/templates/calc_field_ts.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/calc_therm_field.mako` & `femagtools-1.3.2/femagtools/templates/calc_therm_field.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/cogg_calc.mako` & `femagtools-1.3.2/femagtools/templates/pm_sym_loss.mako`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 --
--- Cogging
+-- PM/Rel Losses
 --
 m.move_action     =    0.0 -- rotate
-% if model.get('lfe', 0):
+% if 'lfe' in model:
 m.arm_length      =    ${model.get('lfe')*1e3}
 % endif
-
-m.speed           =    ${model.get('speed')*60}
-m.skew_angle      =    ${model.get('skew_angle', 0)}
-m.nu_skew_steps   =    ${model.get('num_skew_steps', 0)}
+m.speed           =    1000.
+m.skew_angle      =    ${model.get('skew_angle',0)}
+m.nu_skew_steps   =    ${model.get('num_skew_steps',0)}
 m.magn_temp       =    ${model.get('magn_temp')}
 m.fc_mult_move_type =  1.0 --  Type of move path in air gap
 m.fc_force_points   =  0.0 --    number move points in air gap       
 m.phi_start       =    ${model.get('phi_start', 0)}
 m.range_phi       =    ${model.get('range_phi', 0)}
 m.nu_move_steps   =    ${model.get('num_move_steps', 49)}
-
 m.num_par_wdgs    =    ${model.get('num_par_wdgs',1)}
-m.nu_force_pat     =  0.0
 
-m.eval_force1     =    ${model.get('eval_force', 0)}
+m.winding_temp    =    ${model.get('wind_temp')}
+m.current         =    1.0
+m.ntibfilename    =    model..'.ntib'
 m.period_frac     =    ${model.get('period_frac', 1)}
 
 m.pocfilename    = '${model.get('pocfilename', 'sin.poc')}'
-% if model.get('vtu_movie', 0):
-m.movie_type = 'vtu'
-% else:
-m.movie_type = nil
-% endif
-run_models("cogg_calc")
+
+run_models("pm_sym_loss")
```

### Comparing `femagtools-1.3.1/femagtools/templates/com_motor_sim.mako` & `femagtools-1.3.2/femagtools/templates/com_motor_sim.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/connect_models.mako` & `femagtools-1.3.2/femagtools/templates/connect_models.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/cu_losses.mako` & `femagtools-1.3.2/femagtools/templates/cu_losses.mako`

 * *Files 0% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 m.conrelperm      =  ${model.get('relperm', 100)} -- rel permeability
 m.contecoef       =  ${model.get('tempcoef', 0)} -- conduct. temperature coeff 1/K
 m.spconweight     =  ${model.get('spmaweight', 7.6)} -- mass density g/cm³
 m.relconlength    =  ${model.get('rlen', 1)*100} -- rel cond length %
 pre_models('conduct-data')
 pre_models("CU-Losses-2") -- inside
 % else:
-pre_models("CU-Losses-1") -- outside
+pre_models("CU-Losses-1")
 % endif
```

### Comparing `femagtools-1.3.1/femagtools/templates/ec-rotorbar.mako` & `femagtools-1.3.2/femagtools/templates/ec-rotorbar.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/fe-contr.mako` & `femagtools-1.3.2/femagtools/templates/fe-contr.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/gen_winding.mako` & `femagtools-1.3.2/femagtools/templates/gen_winding.mako`

 * *Files 4% similar despite different names*

```diff
@@ -43,43 +43,44 @@
 % if model.get(['stator', 'num_slots_gen']) == 1:
 def_new_wdg(m.xcoil_1, m.ycoil_1, "green", "1", m.num_wires, 0.0, "wi")
 add_to_wdg(m.xcoil_2, m.ycoil_2, "wsamekey", "wo", "wser")
 % else:
 pre_models("Gen_winding")
 pre_models("gen_pocfile")
 % endif
-% else:
+% else:  # move_action > 0
 color={"green", "yellow", "magenta", "lightgrey", "darkred", "skyblue", "violet"}
 wkey={0,0,0,0,0,0}
---
+
 bz = m.width_bz
---
+sw = m.slot_width
 ys = m.slot_height/2
-
-dirl = 1
-for i=1, m.num_phases do
-  wdg = "w"..i
-  for g=1, m.num_sl_gen/m.num_phases/2 do
-    xs = 2*bz*((i-1) + (g-1)*m.num_phases)
-    if g == 1 then
-      wkey[i]=def_new_wdg(xs + bz/3, ys, color[i], wdg, m.num_wires, 0, dirl)
-    else
-      add_to_wdg(xs + bz/3, ys, color[i], wkey[i], dirl, "wser")
-    end
-    if m.num_layers > 1 then
-      add_to_wdg(xs + bz - bz/3, ys, wkey[i], dirl, "wser")
-    end
-    dirl = -dirl
-    if i > 1 or g > 1 then
-      add_to_wdg(xs - bz/3, ys, wkey[i], dirl, "wser")
-    else
-      add_to_wdg(m.num_sl_gen*bz - bz/3, ys, wkey[i], -dirl, "wser")
-    end
-    if m.num_layers > 1 then
-      add_to_wdg(xs + bz + bz/3, ys, wkey[i], dirl, "wser")
+wdgscheme = ${model.windings.get('wdgscheme', '{}')}
+-- TODO: m.middle_line = 1 only
+for l=1, #wdgscheme do
+  for z=1, #wdgscheme[l] do
+    for i=1, #wdgscheme[l][z] do
+      k = wdgscheme[l][z][i]
+      if math.abs(k) < m.num_sl_gen+1 then
+        xs = (2*math.abs(k)-1)*bz/2
+        dir = 1
+        if k < 0 then
+          dir = -1
+        end
+        if wkey[z] == 0 then
+         wdg = "wdg"..z
+         wkey[z]=def_new_wdg(xs + sw/4, ys, color[z], wdg, m.num_wires, 0, dir)
+        else
+          if l == 1 then
+             add_to_wdg(xs + sw/4, ys, wkey[z], dir, "wser")
+          else
+             add_to_wdg(xs - sw/4, ys, wkey[z], dir, "wser")
+          end
+        end
+      end
     end
   end
 end
 
 ----------------------------------------------------------------------
 -- create poc-File
 ----------------------------------------------------------------------
@@ -100,43 +101,47 @@
     end
   end
   if     period<10   then f:write(string.format("   %10.8f\n",period));
   elseif period<100  then f:write(string.format("   %10.7f\n",period));
   elseif period<1000 then f:write(string.format("   %10.6f\n",period));
   end
   f:write("sin\n");
-  f:write("   0.00000000\n");
+  f:write("   0.0\n");
   f:write("          0\n");
 io.close(f);
 
 %endif
 % if 'num_poles' in model.windings:
 m.num_poles       =  ${model.poles}
 % endif
 % endif
 
 % if 'thcap' in model.windings:
 -- Thermal Material properties
-rw = da1/2 +(m.slot_height-m.slot_h1)/2
-dw = 0
-dr = 0
-if m.middle_line == 1 then
-  dw = 1/60
-elseif m.middle_line == 2 then
-  dr = 1
-end
-lamCu = 400
-capCu = 385
-da = 1.0785
-dCu = 1.0
-lam = lamCu*(dCu/(da-dCu)+(da-dCu)/da)
-cap = capCu*da^2/(dCu^2*math.pi/4)
-for i=1,m.num_sl_gen do
-  a = (2*i-1)*math.pi/m.tot_num_sl + m.zeroangl/180*math.pi
-  xwl,ywl = pr2c(rw+dr,a+dw)
-  def_mat_therm(xwl,ywl,'yellow',8920,lam,cap,1)
-  if m.middle_line > 0 then
-    xwr,ywr = pr2c(rw-dr,a-dw)
-    def_mat_therm(xwr,ywr,'yellow',8920,lam,cap,1)
+if m.slot_height ~= nil then
+  -- FEMAG slot model
+  -- TODO: slot model from user
+  rw = da1/2 +(m.slot_height-m.slot_h1)/2
+  dw = 0
+  dr = 0
+  if m.middle_line == 1 then
+    dw = 1/60
+  elseif m.middle_line == 2 then
+    dr = 1
+  end
+  lamCu = 400
+  capCu = 385
+  da = 1.0785
+  dCu = 1.0
+  lam = lamCu*(dCu/(da-dCu)+(da-dCu)/da)
+  cap = capCu*da^2/(dCu^2*math.pi/4)
+  for i=1,m.num_sl_gen do
+    a = (2*i-1)*math.pi/m.tot_num_sl + m.zeroangl/180*math.pi
+    xwl,ywl = pr2c(rw+dr,a+dw)
+    def_mat_therm(xwl,ywl,'yellow',8920,lam,cap,1)
+    if m.middle_line > 0 then
+      xwr,ywr = pr2c(rw-dr,a-dw)
+      def_mat_therm(xwr,ywr,'yellow',8920,lam,cap,1)
+    end
   end
 end
 %endif
```

### Comparing `femagtools-1.3.1/femagtools/templates/inductances.mako` & `femagtools-1.3.2/femagtools/templates/inductances.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/ld_lq_fast.mako` & `femagtools-1.3.2/femagtools/templates/ld_lq_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/leak_dist_wind.mako` & `femagtools-1.3.2/femagtools/templates/leak_dist_wind.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/leak_evol_wind.mako` & `femagtools-1.3.2/femagtools/templates/leak_evol_wind.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/magnet-data.mako` & `femagtools-1.3.2/femagtools/templates/magnet-data.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/magnetFC2.mako` & `femagtools-1.3.2/femagtools/templates/magnetFC2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/magnetIron.mako` & `femagtools-1.3.2/femagtools/templates/magnetIron.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/magnetIron2.mako` & `femagtools-1.3.2/femagtools/templates/magnetIron2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/magnetIron3.mako` & `femagtools-1.3.2/femagtools/templates/magnetIron3.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/magnetIron4.mako` & `femagtools-1.3.2/femagtools/templates/magnetIron4.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/magnetIron5.mako` & `femagtools-1.3.2/femagtools/templates/magnetIron5.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/magnetIronV.mako` & `femagtools-1.3.2/femagtools/templates/magnetIronV.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/magnetSector.mako` & `femagtools-1.3.2/femagtools/templates/magnetSector.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/magnetSectorLinear.mako` & `femagtools-1.3.2/femagtools/templates/magnetSectorLinear.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/magnetShell.mako` & `femagtools-1.3.2/femagtools/templates/magnetShell.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/magnetShell2.mako` & `femagtools-1.3.2/femagtools/templates/magnetShell2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/modal_analysis.mako` & `femagtools-1.3.2/femagtools/templates/modal_analysis.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/mult_cal_fast.mako` & `femagtools-1.3.2/femagtools/templates/mult_cal_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/noloadflux-rot.mako` & `femagtools-1.3.2/femagtools/templates/noloadflux-rot.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/noloadflux.mako` & `femagtools-1.3.2/femagtools/templates/noloadflux.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/noloadfluxdc.mako` & `femagtools-1.3.2/femagtools/templates/noloadfluxdc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/plots.mako` & `femagtools-1.3.2/femagtools/templates/plots.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/pm_sym_f_cur.mako` & `femagtools-1.3.2/femagtools/templates/pm_sym_f_cur.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/pm_sym_fast.mako` & `femagtools-1.3.2/femagtools/templates/pm_sym_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/pm_sym_loss.mako` & `femagtools-1.3.2/femagtools/templates/psd_psq_fast.mako`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 --
--- PM/Rel Losses
+-- Psid-Psiq- Identification
 --
+% if model.get('magn_temp',0):
+set_dev_data("magn_temp", ${model.get('magn_temp')})
+%endif
+	 
 m.move_action     =    0.0 -- rotate
-% if 'lfe' in model:
-m.arm_length      =    ${model.get('lfe')*1e3}
-% endif
-m.speed           =    1000.
+m.speed           =    ${model.get('speed')*60}
 m.skew_angle      =    ${model.get('skew_angle',0)}
 m.nu_skew_steps   =    ${model.get('num_skew_steps',0)}
-m.magn_temp       =    ${model.get('magn_temp')}
 m.fc_mult_move_type =  1.0 --  Type of move path in air gap
-m.fc_force_points   =  0.0 --    number move points in air gap       
 m.phi_start       =    ${model.get('phi_start', 0)}
 m.range_phi       =    ${model.get('range_phi', 0)}
 m.nu_move_steps   =    ${model.get('num_move_steps', 49)}
 m.num_par_wdgs    =    ${model.get('num_par_wdgs',1)}
 
-m.winding_temp    =    ${model.get('wind_temp')}
-m.current         =    1.0
-m.ntibfilename    =    model..'.ntib'
+m.maxid           =    ${model['maxid']}/m.num_par_wdgs
+m.minid           =    ${model['minid']}/m.num_par_wdgs
+m.maxiq           =    ${model['maxiq']}/m.num_par_wdgs
+m.miniq           =    ${model['miniq']}/m.num_par_wdgs
+m.delta_id        =    ${model['delta_id']}/m.num_par_wdgs
+m.delta_iq        =    ${model['delta_iq']}/m.num_par_wdgs
+% if model.get('load_ex_cur',0):
+m.load_ex_cur     =    ${model['load_ex_cur']}
+%endif
+m.pm_eff_aktiv    =    0.0
+m.calc_noload     =    ${model.get('calc_noload', 1)}
 m.period_frac     =    ${model.get('period_frac', 1)}
-
 m.pocfilename    = '${model.get('pocfilename', 'sin.poc')}'
+run_models("psd_psq_fast")
 
-run_models("pm_sym_loss")
```

### Comparing `femagtools-1.3.1/femagtools/templates/ring.mako` & `femagtools-1.3.2/femagtools/templates/ring.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/rot_hsm.mako` & `femagtools-1.3.2/femagtools/templates/rot_hsm.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/rotorAsyn.mako` & `femagtools-1.3.2/femagtools/templates/rotorAsyn.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/rotorKs2.mako` & `femagtools-1.3.2/femagtools/templates/rotorKs2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/rotor_msh.mako` & `femagtools-1.3.2/femagtools/templates/rotor_msh.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/rotor_winding.mako` & `femagtools-1.3.2/femagtools/templates/rotor_winding.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/shortcircuit.mako` & `femagtools-1.3.2/femagtools/templates/shortcircuit.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/srm.mako` & `femagtools-1.3.2/femagtools/templates/srm.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/stator1.mako` & `femagtools-1.3.2/femagtools/templates/stator1.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/stator2.mako` & `femagtools-1.3.2/femagtools/templates/stator2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/stator3Linear.mako` & `femagtools-1.3.2/femagtools/templates/stator3Linear.mako`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 
 
-m.cood_system     = ${model.get('coord_system', 1)} -- 1: x/y or 2: r/z 
+m.cood_system     = ${model.get('coord_system', 1)} -- 1: x/y or 2: r/z
 
 m.l_corner_x0     = 0.0
 m.l_corner_y0     = 0.0
 m.slot_height     = ${model['slot_height']*1e3}
 m.slot_h1         = ${model['slot_h1']*1e3}
 m.slot_h2         = ${model['slot_h2']*1e3}
 m.tip_slot        = ${model['tip_slot']*1e3}
 m.yoke_height     = ${model['yoke_height']*1e3}
 m.slot_r1         = ${model['slot_r1']*1e3}
 m.slot_r2         = ${model['slot_r2']*1e3}
 m.width_bz        = ${model['width_bz']*1e3}
 m.tooth_width     = ${model['tooth_width']*1e3}
+m.slot_width      = m.width_bz - m.tooth_width
 
 m.middle_line     = ${model['middle_line']}
-m.zeroangl        =          0.000 --   Reference angle to x-axis [grad]        
- 
+m.zeroangl        =          0.000 --   Reference angle to x-axis [grad]
+
  m.mcvkey_yoke = mcvkey_yoke
- 
+
  pre_models("STATOR3_Linear");
```

### Comparing `femagtools-1.3.1/femagtools/templates/stator4.mako` & `femagtools-1.3.2/femagtools/templates/stator4.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/statorBG.mako` & `femagtools-1.3.2/femagtools/templates/statorBG.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/statorRing.mako` & `femagtools-1.3.2/femagtools/templates/statorRing.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/statorRotor3.mako` & `femagtools-1.3.2/femagtools/templates/statorRotor3.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/stator_msh.mako` & `femagtools-1.3.2/femagtools/templates/stator_msh.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/therm-dynamic.mako` & `femagtools-1.3.2/femagtools/templates/therm-dynamic.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/templates/torq_calc.mako` & `femagtools-1.3.2/femagtools/templates/torq_calc.mako`

 * *Files 16% similar despite different names*

```diff
@@ -21,26 +21,24 @@
 m.line            =    0
 m.two_pole_wi     =    2*m.pole_width
 m.range_x         =    m.two_pole_wi
 m.range_y         =    0.0
 
 m.fc_force_points =  5
 m.fcpx_mm1        =   m.npols_gen*m.pole_width +1.0
-m.fcpy_mm1        =   -3*ag/4
+m.fcpy_mm1        =   -ag/2
 m.fcpx_mm2        =   -1.0
 m.fcpy_mm2        =   m.fcpy_mm1
 m.fcpx_mm3        =   m.fcpx_mm2
-m.fcpy_mm3        =   -m.magn_height -m.yoke_height -m.gap_ma_yoke -4
+m.fcpy_mm3        =   -m.magn_height -m.yoke_height -m.gap_ma_yoke -ag -1
 m.fcpx_mm4        =   m.fcpx_mm1
 m.fcpy_mm4        =   m.fcpy_mm3
 m.fcpx_mm5        =   m.fcpx_mm1
 m.fcpy_mm5        =   m.fcpy_mm1
 
-m.npols_gen       =  1 -- number of sectors simulated
-
 % endif
 m.nu_force_pat    =    0.0
 m.nu_skew_steps   =    ${model.get('num_skew_steps',0)}
 m.magn_temp       =    ${model.get('magn_temp',20.0)}
 m.winding_temp    =    ${model.get('wind_temp', 20.0)}
 m.fc_mult_move_type =  1.0 --  Type of move path in air gap
 m.nu_move_steps   =    ${model.get('num_move_steps', 49)}
```

### Comparing `femagtools-1.3.1/femagtools/tks.py` & `femagtools-1.3.2/femagtools/tks.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/ts.py` & `femagtools-1.3.2/femagtools/ts.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/vbf.py` & `femagtools-1.3.2/femagtools/vbf.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/vtu.py` & `femagtools-1.3.2/femagtools/vtu.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/femagtools/windings.py` & `femagtools-1.3.2/femagtools/windings.py`

 * *Files 1% similar despite different names*

```diff
@@ -579,9 +579,10 @@
     plt.annotate("", xy=(phi[0], y[0]),
                  xytext=(0, y[0]), arrowprops=dict(arrowstyle="->"))
 
     plt.grid()
     plt.show()
 
     svg = wdgs.diagram()
-    ET.ElementTree(svg).write('wind.svg')
+    tree = ET.ElementTree(ET.fromstring(svg))
+    tree.write('wind.svg')
     print('SVG file "wind.svg" created')
```

### Comparing `femagtools-1.3.1/femagtools.egg-info/PKG-INFO` & `femagtools-1.3.2/femagtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femagtools
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python API for FEMAG
 Author-email: Ronald Tanner <tar@semafor.ch>, Dapu Zhang <d.zhan@gtisoft.com>, Beat Holm <hob@semafor.ch>, Günther Amsler <amg@semafor.ch>, Nicolas Mauchle <mau@semafor.ch>
 License: Copyright (c) 2016-2023, Semafor Informatik & Energie AG, Basel
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
```

### Comparing `femagtools-1.3.1/femagtools.egg-info/SOURCES.txt` & `femagtools-1.3.2/femagtools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 femagtools/ntib.py
 femagtools/opt.py
 femagtools/parstudy.py
 femagtools/plot.py
 femagtools/poc.py
 femagtools/tks.py
 femagtools/ts.py
+femagtools/utils.py
 femagtools/vbf.py
 femagtools/vtu.py
 femagtools/windings.py
 femagtools.egg-info/PKG-INFO
 femagtools.egg-info/SOURCES.txt
 femagtools.egg-info/dependency_links.txt
 femagtools.egg-info/entry_points.txt
@@ -77,27 +78,30 @@
 femagtools/machine/sm.py
 femagtools/machine/utils.py
 femagtools/moo/__init__.py
 femagtools/moo/algorithm.py
 femagtools/moo/population.py
 femagtools/moo/problem.py
 femagtools/templates/FE-losses.mako
+femagtools/templates/afm_rotor.mako
+femagtools/templates/afm_stator.mako
 femagtools/templates/airgapinduc.mako
 femagtools/templates/asyn_motor.mako
 femagtools/templates/basic_modpar.mako
 femagtools/templates/calc_field_ts.mako
 femagtools/templates/calc_therm_field.mako
 femagtools/templates/cogg_calc.mako
 femagtools/templates/colorgrad.mako
 femagtools/templates/com_motor_sim.mako
 femagtools/templates/conduct-data.mako
 femagtools/templates/connect_models.mako
 femagtools/templates/cu_losses.mako
 femagtools/templates/ec-rotorbar.mako
 femagtools/templates/fe-contr.mako
+femagtools/templates/fieldcalc.mako
 femagtools/templates/gen_winding.mako
 femagtools/templates/inductances.mako
 femagtools/templates/ld_lq_fast.mako
 femagtools/templates/leak_dist_wind.mako
 femagtools/templates/leak_evol_wind.mako
 femagtools/templates/leak_tooth_wind.mako
 femagtools/templates/magnet-data.mako
@@ -140,14 +144,15 @@
 femagtools/templates/statorBG.mako
 femagtools/templates/statorRing.mako
 femagtools/templates/statorRotor3.mako
 femagtools/templates/stator_msh.mako
 femagtools/templates/therm-dynamic.mako
 femagtools/templates/therm-static.mako
 femagtools/templates/torq_calc.mako
+tests/test_afpm.py
 tests/test_airgap_induction.py
 tests/test_amela.py
 tests/test_asm.py
 tests/test_bchreader.py
 tests/test_conductor.py
 tests/test_convert.py
 tests/test_effloss.py
```

### Comparing `femagtools-1.3.1/pyproject.toml` & `femagtools-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_airgap_induction.py` & `femagtools-1.3.2/tests/test_airgap_induction.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_amela.py` & `femagtools-1.3.2/tests/test_amela.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_asm.py` & `femagtools-1.3.2/tests/test_asm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_bchreader.py` & `femagtools-1.3.2/tests/test_bchreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_convert.py` & `femagtools-1.3.2/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_effloss.py` & `femagtools-1.3.2/tests/test_effloss.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_erg.py` & `femagtools-1.3.2/tests/test_erg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_femag.py` & `femagtools-1.3.2/tests/test_femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_forcedens.py` & `femagtools-1.3.2/tests/test_forcedens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_fsl.py` & `femagtools-1.3.2/tests/test_fsl.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_im.py` & `femagtools-1.3.2/tests/test_im.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_isa7.py` & `femagtools-1.3.2/tests/test_isa7.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_jhb.py` & `femagtools-1.3.2/tests/test_jhb.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_job.py` & `femagtools-1.3.2/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_losscoeffs.py` & `femagtools-1.3.2/tests/test_losscoeffs.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_machine.py` & `femagtools-1.3.2/tests/test_machine.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_magncurv.py` & `femagtools-1.3.2/tests/test_magncurv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_mcvreader.py` & `femagtools-1.3.2/tests/test_mcvreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_mcvwriter.py` & `femagtools-1.3.2/tests/test_mcvwriter.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_model.py` & `femagtools-1.3.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_nc.py` & `femagtools-1.3.2/tests/test_nc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_parident.py` & `femagtools-1.3.2/tests/test_parident.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_parstudy.py` & `femagtools-1.3.2/tests/test_parstudy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_pocfile.py` & `femagtools-1.3.2/tests/test_pocfile.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_sizing.py` & `femagtools-1.3.2/tests/test_sizing.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_sm.py` & `femagtools-1.3.2/tests/test_sm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_tksreader.py` & `femagtools-1.3.2/tests/test_tksreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_ts.py` & `femagtools-1.3.2/tests/test_ts.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_vbfreader.py` & `femagtools-1.3.2/tests/test_vbfreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_vtu.py` & `femagtools-1.3.2/tests/test_vtu.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.3.1/tests/test_windings.py` & `femagtools-1.3.2/tests/test_windings.py`

 * *Files identical despite different names*


# Comparing `tmp/sdss-coordio-1.7.4a0.tar.gz` & `tmp/sdss-coordio-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss-coordio-1.7.4a0.tar", last modified: Mon Jul 24 17:44:07 2023, max compression
+gzip compressed data, was "sdss-coordio-1.8.1.tar", last modified: Fri Jul 28 15:35:03 2023, max compression
```

## Comparing `sdss-coordio-1.7.4a0.tar` & `sdss-coordio-1.8.1.tar`

### file list

```diff
@@ -1,330 +1,330 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-24 17:44:07.758082 sdss-coordio-1.7.4a0/
--rw-r--r--   0 runner     (501) staff       (20)     1504 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/LICENSE.md
--rw-r--r--   0 runner     (501) staff       (20)       62 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     1739 2023-07-24 17:44:07.758381 sdss-coordio-1.7.4a0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      796 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-24 17:44:07.578914 sdss-coordio-1.7.4a0/cextern/
--rw-r--r--   0 runner     (501) staff       (20)      343 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/README.md
--rw-r--r--   0 runner     (501) staff       (20)    12507 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/conv.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-24 17:44:07.585794 sdss-coordio-1.7.4a0/cextern/dimage/
--rw-r--r--   0 runner     (501) staff       (20)     3150 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/dimage/dallpeaks.c
--rw-r--r--   0 runner     (501) staff       (20)     1295 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/dimage/dcen3x3.c
--rw-r--r--   0 runner     (501) staff       (20)     3239 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/dimage/dfind.c
--rw-r--r--   0 runner     (501) staff       (20)     2553 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/dimage/dfloodfill.c
--rw-r--r--   0 runner     (501) staff       (20)     1407 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/dimage/dimage.h
--rw-r--r--   0 runner     (501) staff       (20)     6057 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/dimage/dmedsmooth.c
--rw-r--r--   0 runner     (501) staff       (20)     1351 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/dimage/dobjects.c
--rw-r--r--   0 runner     (501) staff       (20)     3798 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/dimage/dpeaks.c
--rw-r--r--   0 runner     (501) staff       (20)     2856 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/dimage/drefine.c
--rw-r--r--   0 runner     (501) staff       (20)     1872 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/dimage/dselip.c
--rw-r--r--   0 runner     (501) staff       (20)     1252 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/dimage/dsigma.c
--rw-r--r--   0 runner     (501) staff       (20)     3854 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/dimage/dsmooth.c
--rw-r--r--   0 runner     (501) staff       (20)       58 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/dimage/readme.txt
--rw-r--r--   0 runner     (501) staff       (20)     1984 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/dimage/simplexy.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-24 17:44:07.716720 sdss-coordio-1.7.4a0/cextern/sofa/
--rw-r--r--   0 runner     (501) staff       (20)     6468 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/a2af.c
--rw-r--r--   0 runner     (501) staff       (20)     6374 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/a2tf.c
--rw-r--r--   0 runner     (501) staff       (20)     6611 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ab.c
--rw-r--r--   0 runner     (501) staff       (20)     7187 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ae2hd.c
--rw-r--r--   0 runner     (501) staff       (20)     6087 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/af2a.c
--rw-r--r--   0 runner     (501) staff       (20)     4955 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/anp.c
--rw-r--r--   0 runner     (501) staff       (20)     4983 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/anpm.c
--rw-r--r--   0 runner     (501) staff       (20)     9173 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/apcg.c
--rw-r--r--   0 runner     (501) staff       (20)     9278 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/apcg13.c
--rw-r--r--   0 runner     (501) staff       (20)     9669 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/apci.c
--rw-r--r--   0 runner     (501) staff       (20)     9954 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/apci13.c
--rw-r--r--   0 runner     (501) staff       (20)    12864 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/apco.c
--rw-r--r--   0 runner     (501) staff       (20)    14172 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/apco13.c
--rw-r--r--   0 runner     (501) staff       (20)    11004 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/apcs.c
--rw-r--r--   0 runner     (501) staff       (20)     9686 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/apcs13.c
--rw-r--r--   0 runner     (501) staff       (20)     8285 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/aper.c
--rw-r--r--   0 runner     (501) staff       (20)     9207 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/aper13.c
--rw-r--r--   0 runner     (501) staff       (20)    10588 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/apio.c
--rw-r--r--   0 runner     (501) staff       (20)    12842 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/apio13.c
--rw-r--r--   0 runner     (501) staff       (20)     8257 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/atci13.c
--rw-r--r--   0 runner     (501) staff       (20)     7978 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/atciq.c
--rw-r--r--   0 runner     (501) staff       (20)     9826 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/atciqn.c
--rw-r--r--   0 runner     (501) staff       (20)     7729 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/atciqz.c
--rw-r--r--   0 runner     (501) staff       (20)    12474 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/atco13.c
--rw-r--r--   0 runner     (501) staff       (20)     7919 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/atic13.c
--rw-r--r--   0 runner     (501) staff       (20)     8735 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/aticq.c
--rw-r--r--   0 runner     (501) staff       (20)    10634 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/aticqn.c
--rw-r--r--   0 runner     (501) staff       (20)    11485 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/atio13.c
--rw-r--r--   0 runner     (501) staff       (20)    11389 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/atioq.c
--rw-r--r--   0 runner     (501) staff       (20)    12003 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/atoc13.c
--rw-r--r--   0 runner     (501) staff       (20)    11902 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/atoi13.c
--rw-r--r--   0 runner     (501) staff       (20)    11115 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/atoiq.c
--rw-r--r--   0 runner     (501) staff       (20)     6640 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/bi00.c
--rw-r--r--   0 runner     (501) staff       (20)     8454 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/bp00.c
--rw-r--r--   0 runner     (501) staff       (20)     7280 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/bp06.c
--rw-r--r--   0 runner     (501) staff       (20)     5822 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/bpn2xy.c
--rw-r--r--   0 runner     (501) staff       (20)     7375 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/c2i00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7362 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/c2i00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7165 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/c2i06a.c
--rw-r--r--   0 runner     (501) staff       (20)     7592 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/c2ibpn.c
--rw-r--r--   0 runner     (501) staff       (20)     7162 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/c2ixy.c
--rw-r--r--   0 runner     (501) staff       (20)     6391 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/c2ixys.c
--rw-r--r--   0 runner     (501) staff       (20)     5320 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/c2s.c
--rw-r--r--   0 runner     (501) staff       (20)     8083 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/c2t00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7985 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/c2t00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7970 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/c2t06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6652 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/c2tcio.c
--rw-r--r--   0 runner     (501) staff       (20)     6679 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/c2teqx.c
--rw-r--r--   0 runner     (501) staff       (20)     8786 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/c2tpe.c
--rw-r--r--   0 runner     (501) staff       (20)     8249 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/c2txy.c
--rw-r--r--   0 runner     (501) staff       (20)     6962 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/cal2jd.c
--rw-r--r--   0 runner     (501) staff       (20)     4897 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/cp.c
--rw-r--r--   0 runner     (501) staff       (20)     4990 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/cpv.c
--rw-r--r--   0 runner     (501) staff       (20)     4974 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/cr.c
--rw-r--r--   0 runner     (501) staff       (20)     9794 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/d2dtf.c
--rw-r--r--   0 runner     (501) staff       (20)     7240 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/d2tf.c
--rw-r--r--   0 runner     (501) staff       (20)    13394 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/dat.c
--rw-r--r--   0 runner     (501) staff       (20)    63548 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/dtdb.c
--rw-r--r--   0 runner     (501) staff       (20)     9375 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/dtf2d.c
--rw-r--r--   0 runner     (501) staff       (20)     7237 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/eceq06.c
--rw-r--r--   0 runner     (501) staff       (20)     7251 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ecm06.c
--rw-r--r--   0 runner     (501) staff       (20)     6929 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ee00.c
--rw-r--r--   0 runner     (501) staff       (20)     7105 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ee00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7436 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ee00b.c
--rw-r--r--   0 runner     (501) staff       (20)     6632 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ee06a.c
--rw-r--r--   0 runner     (501) staff       (20)    12358 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/eect00.c
--rw-r--r--   0 runner     (501) staff       (20)     6688 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/eform.c
--rw-r--r--   0 runner     (501) staff       (20)     7000 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/eo06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6082 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/eors.c
--rw-r--r--   0 runner     (501) staff       (20)     5398 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/epb.c
--rw-r--r--   0 runner     (501) staff       (20)     5342 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/epb2jd.c
--rw-r--r--   0 runner     (501) staff       (20)     5327 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/epj.c
--rw-r--r--   0 runner     (501) staff       (20)     5330 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/epj2jd.c
--rw-r--r--   0 runner     (501) staff       (20)   152024 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/epv00.c
--rw-r--r--   0 runner     (501) staff       (20)     7238 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/eqec06.c
--rw-r--r--   0 runner     (501) staff       (20)     6953 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/eqeq94.c
--rw-r--r--   0 runner     (501) staff       (20)     6978 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/era00.c
--rw-r--r--   0 runner     (501) staff       (20)     5789 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fad03.c
--rw-r--r--   0 runner     (501) staff       (20)     5756 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fae03.c
--rw-r--r--   0 runner     (501) staff       (20)     5883 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/faf03.c
--rw-r--r--   0 runner     (501) staff       (20)     5768 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/faju03.c
--rw-r--r--   0 runner     (501) staff       (20)     5758 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fal03.c
--rw-r--r--   0 runner     (501) staff       (20)     5758 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/falp03.c
--rw-r--r--   0 runner     (501) staff       (20)     5760 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fama03.c
--rw-r--r--   0 runner     (501) staff       (20)     5770 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fame03.c
--rw-r--r--   0 runner     (501) staff       (20)     5631 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fane03.c
--rw-r--r--   0 runner     (501) staff       (20)     5826 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/faom03.c
--rw-r--r--   0 runner     (501) staff       (20)     5754 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fapa03.c
--rw-r--r--   0 runner     (501) staff       (20)     5765 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fasa03.c
--rw-r--r--   0 runner     (501) staff       (20)     5629 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/faur03.c
--rw-r--r--   0 runner     (501) staff       (20)     5764 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fave03.c
--rw-r--r--   0 runner     (501) staff       (20)    12333 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fk425.c
--rw-r--r--   0 runner     (501) staff       (20)     9855 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fk45z.c
--rw-r--r--   0 runner     (501) staff       (20)    12391 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fk524.c
--rw-r--r--   0 runner     (501) staff       (20)     7422 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fk52h.c
--rw-r--r--   0 runner     (501) staff       (20)     7286 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fk54z.c
--rw-r--r--   0 runner     (501) staff       (20)     6198 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fk5hip.c
--rw-r--r--   0 runner     (501) staff       (20)     8093 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fk5hz.c
--rw-r--r--   0 runner     (501) staff       (20)     7061 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fw2m.c
--rw-r--r--   0 runner     (501) staff       (20)     6147 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/fw2xy.c
--rw-r--r--   0 runner     (501) staff       (20)     8396 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/g2icrs.c
--rw-r--r--   0 runner     (501) staff       (20)     6710 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/gc2gd.c
--rw-r--r--   0 runner     (501) staff       (20)     8338 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/gc2gde.c
--rw-r--r--   0 runner     (501) staff       (20)     6783 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/gd2gc.c
--rw-r--r--   0 runner     (501) staff       (20)     6968 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/gd2gce.c
--rw-r--r--   0 runner     (501) staff       (20)     7699 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/gmst00.c
--rw-r--r--   0 runner     (501) staff       (20)     7337 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/gmst06.c
--rw-r--r--   0 runner     (501) staff       (20)     7688 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/gmst82.c
--rw-r--r--   0 runner     (501) staff       (20)     7470 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/gst00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7770 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/gst00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7536 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/gst06.c
--rw-r--r--   0 runner     (501) staff       (20)     7174 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/gst06a.c
--rw-r--r--   0 runner     (501) staff       (20)     7099 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/gst94.c
--rw-r--r--   0 runner     (501) staff       (20)     7614 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/h2fk5.c
--rw-r--r--   0 runner     (501) staff       (20)     7382 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/hd2ae.c
--rw-r--r--   0 runner     (501) staff       (20)     6333 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/hd2pa.c
--rw-r--r--   0 runner     (501) staff       (20)     8684 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/hfk5z.c
--rw-r--r--   0 runner     (501) staff       (20)     8382 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/icrs2g.c
--rw-r--r--   0 runner     (501) staff       (20)     4970 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ir.c
--rw-r--r--   0 runner     (501) staff       (20)     8269 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/jd2cal.c
--rw-r--r--   0 runner     (501) staff       (20)     7559 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/jdcalf.c
--rw-r--r--   0 runner     (501) staff       (20)     7662 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ld.c
--rw-r--r--   0 runner     (501) staff       (20)     8829 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ldn.c
--rw-r--r--   0 runner     (501) staff       (20)     5982 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ldsun.c
--rw-r--r--   0 runner     (501) staff       (20)     7014 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/lteceq.c
--rw-r--r--   0 runner     (501) staff       (20)     7567 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ltecm.c
--rw-r--r--   0 runner     (501) staff       (20)     7019 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/lteqec.c
--rw-r--r--   0 runner     (501) staff       (20)     6500 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ltp.c
--rw-r--r--   0 runner     (501) staff       (20)     6581 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ltpb.c
--rw-r--r--   0 runner     (501) staff       (20)     7601 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ltpecl.c
--rw-r--r--   0 runner     (501) staff       (20)     7880 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ltpequ.c
--rw-r--r--   0 runner     (501) staff       (20)    27755 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/makefile
--rw-r--r--   0 runner     (501) staff       (20)     6728 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/num00a.c
--rw-r--r--   0 runner     (501) staff       (20)     6713 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/num00b.c
--rw-r--r--   0 runner     (501) staff       (20)     6660 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/num06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6057 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/numat.c
--rw-r--r--   0 runner     (501) staff       (20)   119801 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/nut00a.c
--rw-r--r--   0 runner     (501) staff       (20)    19020 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/nut00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7823 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/nut06a.c
--rw-r--r--   0 runner     (501) staff       (20)    16295 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/nut80.c
--rw-r--r--   0 runner     (501) staff       (20)     6473 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/nutm80.c
--rw-r--r--   0 runner     (501) staff       (20)     6414 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/obl06.c
--rw-r--r--   0 runner     (501) staff       (20)     6459 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/obl80.c
--rw-r--r--   0 runner     (501) staff       (20)    13793 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/p06e.c
--rw-r--r--   0 runner     (501) staff       (20)     5029 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/p2pv.c
--rw-r--r--   0 runner     (501) staff       (20)     5276 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/p2s.c
--rw-r--r--   0 runner     (501) staff       (20)     6768 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pap.c
--rw-r--r--   0 runner     (501) staff       (20)     5638 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pas.c
--rw-r--r--   0 runner     (501) staff       (20)     7817 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pb06.c
--rw-r--r--   0 runner     (501) staff       (20)     5008 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pdp.c
--rw-r--r--   0 runner     (501) staff       (20)     7964 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pfw06.c
--rw-r--r--   0 runner     (501) staff       (20)    23180 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/plan94.c
--rw-r--r--   0 runner     (501) staff       (20)     4887 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pm.c
--rw-r--r--   0 runner     (501) staff       (20)     6579 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pmat00.c
--rw-r--r--   0 runner     (501) staff       (20)     6683 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pmat06.c
--rw-r--r--   0 runner     (501) staff       (20)     7548 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pmat76.c
--rw-r--r--   0 runner     (501) staff       (20)     5090 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pmp.c
--rw-r--r--   0 runner     (501) staff       (20)     7054 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pmpx.c
--rw-r--r--   0 runner     (501) staff       (20)    10220 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pmsafe.c
--rw-r--r--   0 runner     (501) staff       (20)     5495 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pn.c
--rw-r--r--   0 runner     (501) staff       (20)     9146 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pn00.c
--rw-r--r--   0 runner     (501) staff       (20)     8833 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pn00a.c
--rw-r--r--   0 runner     (501) staff       (20)     8825 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pn00b.c
--rw-r--r--   0 runner     (501) staff       (20)     9253 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pn06.c
--rw-r--r--   0 runner     (501) staff       (20)     8282 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pn06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6802 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pnm00a.c
--rw-r--r--   0 runner     (501) staff       (20)     6797 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pnm00b.c
--rw-r--r--   0 runner     (501) staff       (20)     6835 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pnm06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6778 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pnm80.c
--rw-r--r--   0 runner     (501) staff       (20)     6453 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pom00.c
--rw-r--r--   0 runner     (501) staff       (20)     5087 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ppp.c
--rw-r--r--   0 runner     (501) staff       (20)     5275 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ppsp.c
--rw-r--r--   0 runner     (501) staff       (20)     7813 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pr00.c
--rw-r--r--   0 runner     (501) staff       (20)     8023 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/prec76.c
--rw-r--r--   0 runner     (501) staff       (20)     4958 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pv2p.c
--rw-r--r--   0 runner     (501) staff       (20)     6861 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pv2s.c
--rw-r--r--   0 runner     (501) staff       (20)     5587 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pvdpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5073 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pvm.c
--rw-r--r--   0 runner     (501) staff       (20)     5182 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pvmpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5177 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pvppv.c
--rw-r--r--   0 runner     (501) staff       (20)    10128 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pvstar.c
--rw-r--r--   0 runner     (501) staff       (20)     7712 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pvtob.c
--rw-r--r--   0 runner     (501) staff       (20)     5373 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pvu.c
--rw-r--r--   0 runner     (501) staff       (20)     5280 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pvup.c
--rw-r--r--   0 runner     (501) staff       (20)     5842 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pvxpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5234 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/pxp.c
--rw-r--r--   0 runner     (501) staff       (20)    11663 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/refco.c
--rw-r--r--   0 runner     (501) staff       (20)     5989 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/rm2v.c
--rw-r--r--   0 runner     (501) staff       (20)     5996 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/rv2m.c
--rw-r--r--   0 runner     (501) staff       (20)     5807 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/rx.c
--rw-r--r--   0 runner     (501) staff       (20)     5298 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/rxp.c
--rw-r--r--   0 runner     (501) staff       (20)     5144 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/rxpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5337 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/rxr.c
--rw-r--r--   0 runner     (501) staff       (20)     5848 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ry.c
--rw-r--r--   0 runner     (501) staff       (20)     5817 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/rz.c
--rw-r--r--   0 runner     (501) staff       (20)    15540 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/s00.c
--rw-r--r--   0 runner     (501) staff       (20)     7781 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/s00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7772 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/s00b.c
--rw-r--r--   0 runner     (501) staff       (20)    15442 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/s06.c
--rw-r--r--   0 runner     (501) staff       (20)     7799 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/s06a.c
--rw-r--r--   0 runner     (501) staff       (20)     5073 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/s2c.c
--rw-r--r--   0 runner     (501) staff       (20)     5209 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/s2p.c
--rw-r--r--   0 runner     (501) staff       (20)     5636 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/s2pv.c
--rw-r--r--   0 runner     (501) staff       (20)     5282 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/s2xpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5877 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/sepp.c
--rw-r--r--   0 runner     (501) staff       (20)     5424 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/seps.c
--rw-r--r--   0 runner     (501) staff       (20)    26863 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/sofa.h
--rw-r--r--   0 runner     (501) staff       (20)     8772 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/sofam.h
--rw-r--r--   0 runner     (501) staff       (20)     6557 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/sp00.c
--rw-r--r--   0 runner     (501) staff       (20)    10677 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/starpm.c
--rw-r--r--   0 runner     (501) staff       (20)    11959 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/starpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5038 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/sxp.c
--rw-r--r--   0 runner     (501) staff       (20)     5101 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/sxpv.c
--rw-r--r--   0 runner     (501) staff       (20)   241327 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/t_sofa_c.c
--rw-r--r--   0 runner     (501) staff       (20)     5845 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/taitt.c
--rw-r--r--   0 runner     (501) staff       (20)     5901 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/taiut1.c
--rw-r--r--   0 runner     (501) staff       (20)     7493 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/taiutc.c
--rw-r--r--   0 runner     (501) staff       (20)     6987 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/tcbtdb.c
--rw-r--r--   0 runner     (501) staff       (20)     5845 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/tcgtt.c
--rw-r--r--   0 runner     (501) staff       (20)     7109 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/tdbtcb.c
--rw-r--r--   0 runner     (501) staff       (20)     6353 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/tdbtt.c
--rw-r--r--   0 runner     (501) staff       (20)     6062 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/tf2a.c
--rw-r--r--   0 runner     (501) staff       (20)     6066 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/tf2d.c
--rw-r--r--   0 runner     (501) staff       (20)     8685 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/tpors.c
--rw-r--r--   0 runner     (501) staff       (20)     8649 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/tporv.c
--rw-r--r--   0 runner     (501) staff       (20)     6534 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/tpsts.c
--rw-r--r--   0 runner     (501) staff       (20)     7337 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/tpstv.c
--rw-r--r--   0 runner     (501) staff       (20)     7253 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/tpxes.c
--rw-r--r--   0 runner     (501) staff       (20)     7927 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/tpxev.c
--rw-r--r--   0 runner     (501) staff       (20)     5136 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/tr.c
--rw-r--r--   0 runner     (501) staff       (20)     5263 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/trxp.c
--rw-r--r--   0 runner     (501) staff       (20)     5291 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/trxpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5841 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/tttai.c
--rw-r--r--   0 runner     (501) staff       (20)     5913 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/tttcg.c
--rw-r--r--   0 runner     (501) staff       (20)     6345 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/tttdb.c
--rw-r--r--   0 runner     (501) staff       (20)     5794 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ttut1.c
--rw-r--r--   0 runner     (501) staff       (20)     5898 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ut1tai.c
--rw-r--r--   0 runner     (501) staff       (20)     5798 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ut1tt.c
--rw-r--r--   0 runner     (501) staff       (20)     8782 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/ut1utc.c
--rw-r--r--   0 runner     (501) staff       (20)     8283 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/utctai.c
--rw-r--r--   0 runner     (501) staff       (20)     7458 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/utcut1.c
--rw-r--r--   0 runner     (501) staff       (20)   133674 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/xy06.c
--rw-r--r--   0 runner     (501) staff       (20)     7028 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/xys00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7010 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/xys00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7056 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/xys06a.c
--rw-r--r--   0 runner     (501) staff       (20)     4820 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/zp.c
--rw-r--r--   0 runner     (501) staff       (20)     4874 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/zpv.c
--rw-r--r--   0 runner     (501) staff       (20)     4967 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/cextern/sofa/zr.c
--rw-r--r--   0 runner     (501) staff       (20)     2391 2023-07-24 17:44:07.759745 sdss-coordio-1.7.4a0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     2697 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-24 17:44:07.575170 sdss-coordio-1.7.4a0/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-24 17:44:07.729168 sdss-coordio-1.7.4a0/src/coordio/
--rw-r--r--   0 runner     (501) staff       (20)     1178 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12342 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/astrometry.py
--rw-r--r--   0 runner     (501) staff       (20)     5635 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/calibration.py
--rw-r--r--   0 runner     (501) staff       (20)    51063 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/conv.py
--rw-r--r--   0 runner     (501) staff       (20)     9926 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/coordinate.py
--rw-r--r--   0 runner     (501) staff       (20)     7570 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/defaults.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-24 17:44:07.730363 sdss-coordio-1.7.4a0/src/coordio/etc/
--rw-r--r--   0 runner     (501) staff       (20)       73 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/etc/astrometrynet.cfg
--rw-r--r--   0 runner     (501) staff       (20)      366 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/etc/coordio.yml
--rw-r--r--   0 runner     (501) staff       (20)      722 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)    12748 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/extraction.py
--rwxr-xr-x   0 runner     (501) staff       (20)    13362 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/fitData.py
--rw-r--r--   0 runner     (501) staff       (20)    30968 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/guide.py
--rw-r--r--   0 runner     (501) staff       (20)     5870 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/iers.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-24 17:44:07.730852 sdss-coordio-1.7.4a0/src/coordio/include/
--rw-r--r--   0 runner     (501) staff       (20)     1992 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/include/coordio.h
--rw-r--r--   0 runner     (501) staff       (20)     4013 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/positioner.py
--rw-r--r--   0 runner     (501) staff       (20)     4146 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/site.py
--rw-r--r--   0 runner     (501) staff       (20)    14255 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/sky.py
--rw-r--r--   0 runner     (501) staff       (20)     6440 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/sofa_bindings.py
--rw-r--r--   0 runner     (501) staff       (20)    10661 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/tangent.py
--rw-r--r--   0 runner     (501) staff       (20)    13390 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/telescope.py
--rw-r--r--   0 runner     (501) staff       (20)     6451 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/time.py
--rw-r--r--   0 runner     (501) staff       (20)    51462 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/transforms.py
--rw-r--r--   0 runner     (501) staff       (20)    37978 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     3734 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/wok.py
--rw-r--r--   0 runner     (501) staff       (20)    14872 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/zernike.py
--rw-r--r--   0 runner     (501) staff       (20)    12907 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/src/coordio/zhaoburge.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-24 17:44:07.733776 sdss-coordio-1.7.4a0/src/sdss_coordio.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     1739 2023-07-24 17:44:07.000000 sdss-coordio-1.7.4a0/src/sdss_coordio.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     6867 2023-07-24 17:44:07.000000 sdss-coordio-1.7.4a0/src/sdss_coordio.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-24 17:44:07.000000 sdss-coordio-1.7.4a0/src/sdss_coordio.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-24 17:43:13.000000 sdss-coordio-1.7.4a0/src/sdss_coordio.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)      483 2023-07-24 17:44:07.000000 sdss-coordio-1.7.4a0/src/sdss_coordio.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        8 2023-07-24 17:44:07.000000 sdss-coordio-1.7.4a0/src/sdss_coordio.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-24 17:44:07.757628 sdss-coordio-1.7.4a0/tests/
--rw-r--r--   0 runner     (501) staff       (20)    13006 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_conv.py
--rw-r--r--   0 runner     (501) staff       (20)     7006 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_coordinate.py
--rw-r--r--   0 runner     (501) staff       (20)     1386 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_fpScale.py
--rw-r--r--   0 runner     (501) staff       (20)     4290 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_guide.py
--rw-r--r--   0 runner     (501) staff       (20)     1418 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_iers.py
--rw-r--r--   0 runner     (501) staff       (20)    11447 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_libcoordio.py
--rw-r--r--   0 runner     (501) staff       (20)     9056 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_offset.py
--rw-r--r--   0 runner     (501) staff       (20)     8074 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_plPlug.py
--rw-r--r--   0 runner     (501) staff       (20)     5525 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_positioner.py
--rw-r--r--   0 runner     (501) staff       (20)     1105 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_site.py
--rw-r--r--   0 runner     (501) staff       (20)     5302 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_sky.py
--rw-r--r--   0 runner     (501) staff       (20)     1171 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_sofa.py
--rw-r--r--   0 runner     (501) staff       (20)     3340 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_tangent.py
--rw-r--r--   0 runner     (501) staff       (20)     2738 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_tangentToPositioner2.py
--rw-r--r--   0 runner     (501) staff       (20)    13872 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_telescope.py
--rw-r--r--   0 runner     (501) staff       (20)     1407 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_time.py
--rw-r--r--   0 runner     (501) staff       (20)     2588 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_wok.py
--rw-r--r--   0 runner     (501) staff       (20)     1363 2023-07-24 17:42:44.000000 sdss-coordio-1.7.4a0/tests/test_zern.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-28 15:35:03.921664 sdss-coordio-1.8.1/
+-rw-r--r--   0 runner     (501) staff       (20)     1504 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/LICENSE.md
+-rw-r--r--   0 runner     (501) staff       (20)       62 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     1737 2023-07-28 15:35:03.921878 sdss-coordio-1.8.1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      796 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-28 15:35:03.751560 sdss-coordio-1.8.1/cextern/
+-rw-r--r--   0 runner     (501) staff       (20)      343 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/README.md
+-rw-r--r--   0 runner     (501) staff       (20)    12507 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/conv.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-28 15:35:03.758898 sdss-coordio-1.8.1/cextern/dimage/
+-rw-r--r--   0 runner     (501) staff       (20)     3150 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/dimage/dallpeaks.c
+-rw-r--r--   0 runner     (501) staff       (20)     1295 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/dimage/dcen3x3.c
+-rw-r--r--   0 runner     (501) staff       (20)     3239 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/dimage/dfind.c
+-rw-r--r--   0 runner     (501) staff       (20)     2553 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/dimage/dfloodfill.c
+-rw-r--r--   0 runner     (501) staff       (20)     1407 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/dimage/dimage.h
+-rw-r--r--   0 runner     (501) staff       (20)     6057 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/dimage/dmedsmooth.c
+-rw-r--r--   0 runner     (501) staff       (20)     1351 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/dimage/dobjects.c
+-rw-r--r--   0 runner     (501) staff       (20)     3798 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/dimage/dpeaks.c
+-rw-r--r--   0 runner     (501) staff       (20)     2856 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/dimage/drefine.c
+-rw-r--r--   0 runner     (501) staff       (20)     1872 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/dimage/dselip.c
+-rw-r--r--   0 runner     (501) staff       (20)     1252 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/dimage/dsigma.c
+-rw-r--r--   0 runner     (501) staff       (20)     3854 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/dimage/dsmooth.c
+-rw-r--r--   0 runner     (501) staff       (20)       58 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/dimage/readme.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1984 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/dimage/simplexy.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-28 15:35:03.893280 sdss-coordio-1.8.1/cextern/sofa/
+-rw-r--r--   0 runner     (501) staff       (20)     6468 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/a2af.c
+-rw-r--r--   0 runner     (501) staff       (20)     6374 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/a2tf.c
+-rw-r--r--   0 runner     (501) staff       (20)     6611 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ab.c
+-rw-r--r--   0 runner     (501) staff       (20)     7187 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ae2hd.c
+-rw-r--r--   0 runner     (501) staff       (20)     6087 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/af2a.c
+-rw-r--r--   0 runner     (501) staff       (20)     4955 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/anp.c
+-rw-r--r--   0 runner     (501) staff       (20)     4983 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/anpm.c
+-rw-r--r--   0 runner     (501) staff       (20)     9173 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/apcg.c
+-rw-r--r--   0 runner     (501) staff       (20)     9278 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/apcg13.c
+-rw-r--r--   0 runner     (501) staff       (20)     9669 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/apci.c
+-rw-r--r--   0 runner     (501) staff       (20)     9954 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/apci13.c
+-rw-r--r--   0 runner     (501) staff       (20)    12864 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/apco.c
+-rw-r--r--   0 runner     (501) staff       (20)    14172 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/apco13.c
+-rw-r--r--   0 runner     (501) staff       (20)    11004 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/apcs.c
+-rw-r--r--   0 runner     (501) staff       (20)     9686 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/apcs13.c
+-rw-r--r--   0 runner     (501) staff       (20)     8285 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/aper.c
+-rw-r--r--   0 runner     (501) staff       (20)     9207 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/aper13.c
+-rw-r--r--   0 runner     (501) staff       (20)    10588 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/apio.c
+-rw-r--r--   0 runner     (501) staff       (20)    12842 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/apio13.c
+-rw-r--r--   0 runner     (501) staff       (20)     8257 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/atci13.c
+-rw-r--r--   0 runner     (501) staff       (20)     7978 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/atciq.c
+-rw-r--r--   0 runner     (501) staff       (20)     9826 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/atciqn.c
+-rw-r--r--   0 runner     (501) staff       (20)     7729 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/atciqz.c
+-rw-r--r--   0 runner     (501) staff       (20)    12474 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/atco13.c
+-rw-r--r--   0 runner     (501) staff       (20)     7919 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/atic13.c
+-rw-r--r--   0 runner     (501) staff       (20)     8735 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/aticq.c
+-rw-r--r--   0 runner     (501) staff       (20)    10634 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/aticqn.c
+-rw-r--r--   0 runner     (501) staff       (20)    11485 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/atio13.c
+-rw-r--r--   0 runner     (501) staff       (20)    11389 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/atioq.c
+-rw-r--r--   0 runner     (501) staff       (20)    12003 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/atoc13.c
+-rw-r--r--   0 runner     (501) staff       (20)    11902 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/atoi13.c
+-rw-r--r--   0 runner     (501) staff       (20)    11115 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/atoiq.c
+-rw-r--r--   0 runner     (501) staff       (20)     6640 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/bi00.c
+-rw-r--r--   0 runner     (501) staff       (20)     8454 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/bp00.c
+-rw-r--r--   0 runner     (501) staff       (20)     7280 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/bp06.c
+-rw-r--r--   0 runner     (501) staff       (20)     5822 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/bpn2xy.c
+-rw-r--r--   0 runner     (501) staff       (20)     7375 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/c2i00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7362 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/c2i00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     7165 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/c2i06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7592 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/c2ibpn.c
+-rw-r--r--   0 runner     (501) staff       (20)     7162 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/c2ixy.c
+-rw-r--r--   0 runner     (501) staff       (20)     6391 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/c2ixys.c
+-rw-r--r--   0 runner     (501) staff       (20)     5320 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/c2s.c
+-rw-r--r--   0 runner     (501) staff       (20)     8083 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/c2t00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7985 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/c2t00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     7970 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/c2t06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6652 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/c2tcio.c
+-rw-r--r--   0 runner     (501) staff       (20)     6679 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/c2teqx.c
+-rw-r--r--   0 runner     (501) staff       (20)     8786 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/c2tpe.c
+-rw-r--r--   0 runner     (501) staff       (20)     8249 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/c2txy.c
+-rw-r--r--   0 runner     (501) staff       (20)     6962 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/cal2jd.c
+-rw-r--r--   0 runner     (501) staff       (20)     4897 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/cp.c
+-rw-r--r--   0 runner     (501) staff       (20)     4990 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/cpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     4974 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/cr.c
+-rw-r--r--   0 runner     (501) staff       (20)     9794 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/d2dtf.c
+-rw-r--r--   0 runner     (501) staff       (20)     7240 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/d2tf.c
+-rw-r--r--   0 runner     (501) staff       (20)    13394 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/dat.c
+-rw-r--r--   0 runner     (501) staff       (20)    63548 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/dtdb.c
+-rw-r--r--   0 runner     (501) staff       (20)     9375 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/dtf2d.c
+-rw-r--r--   0 runner     (501) staff       (20)     7237 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/eceq06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7251 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ecm06.c
+-rw-r--r--   0 runner     (501) staff       (20)     6929 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ee00.c
+-rw-r--r--   0 runner     (501) staff       (20)     7105 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ee00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7436 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ee00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     6632 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ee06a.c
+-rw-r--r--   0 runner     (501) staff       (20)    12358 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/eect00.c
+-rw-r--r--   0 runner     (501) staff       (20)     6688 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/eform.c
+-rw-r--r--   0 runner     (501) staff       (20)     7000 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/eo06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6082 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/eors.c
+-rw-r--r--   0 runner     (501) staff       (20)     5398 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/epb.c
+-rw-r--r--   0 runner     (501) staff       (20)     5342 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/epb2jd.c
+-rw-r--r--   0 runner     (501) staff       (20)     5327 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/epj.c
+-rw-r--r--   0 runner     (501) staff       (20)     5330 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/epj2jd.c
+-rw-r--r--   0 runner     (501) staff       (20)   152024 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/epv00.c
+-rw-r--r--   0 runner     (501) staff       (20)     7238 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/eqec06.c
+-rw-r--r--   0 runner     (501) staff       (20)     6953 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/eqeq94.c
+-rw-r--r--   0 runner     (501) staff       (20)     6978 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/era00.c
+-rw-r--r--   0 runner     (501) staff       (20)     5789 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fad03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5756 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fae03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5883 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/faf03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5768 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/faju03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5758 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fal03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5758 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/falp03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5760 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fama03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5770 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fame03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5631 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fane03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5826 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/faom03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5754 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fapa03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5765 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fasa03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5629 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/faur03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5764 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fave03.c
+-rw-r--r--   0 runner     (501) staff       (20)    12333 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fk425.c
+-rw-r--r--   0 runner     (501) staff       (20)     9855 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fk45z.c
+-rw-r--r--   0 runner     (501) staff       (20)    12391 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fk524.c
+-rw-r--r--   0 runner     (501) staff       (20)     7422 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fk52h.c
+-rw-r--r--   0 runner     (501) staff       (20)     7286 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fk54z.c
+-rw-r--r--   0 runner     (501) staff       (20)     6198 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fk5hip.c
+-rw-r--r--   0 runner     (501) staff       (20)     8093 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fk5hz.c
+-rw-r--r--   0 runner     (501) staff       (20)     7061 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fw2m.c
+-rw-r--r--   0 runner     (501) staff       (20)     6147 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/fw2xy.c
+-rw-r--r--   0 runner     (501) staff       (20)     8396 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/g2icrs.c
+-rw-r--r--   0 runner     (501) staff       (20)     6710 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/gc2gd.c
+-rw-r--r--   0 runner     (501) staff       (20)     8338 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/gc2gde.c
+-rw-r--r--   0 runner     (501) staff       (20)     6783 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/gd2gc.c
+-rw-r--r--   0 runner     (501) staff       (20)     6968 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/gd2gce.c
+-rw-r--r--   0 runner     (501) staff       (20)     7699 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/gmst00.c
+-rw-r--r--   0 runner     (501) staff       (20)     7337 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/gmst06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7688 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/gmst82.c
+-rw-r--r--   0 runner     (501) staff       (20)     7470 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/gst00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7770 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/gst00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     7536 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/gst06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7174 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/gst06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7099 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/gst94.c
+-rw-r--r--   0 runner     (501) staff       (20)     7614 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/h2fk5.c
+-rw-r--r--   0 runner     (501) staff       (20)     7382 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/hd2ae.c
+-rw-r--r--   0 runner     (501) staff       (20)     6333 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/hd2pa.c
+-rw-r--r--   0 runner     (501) staff       (20)     8684 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/hfk5z.c
+-rw-r--r--   0 runner     (501) staff       (20)     8382 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/icrs2g.c
+-rw-r--r--   0 runner     (501) staff       (20)     4970 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ir.c
+-rw-r--r--   0 runner     (501) staff       (20)     8269 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/jd2cal.c
+-rw-r--r--   0 runner     (501) staff       (20)     7559 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/jdcalf.c
+-rw-r--r--   0 runner     (501) staff       (20)     7662 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ld.c
+-rw-r--r--   0 runner     (501) staff       (20)     8829 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ldn.c
+-rw-r--r--   0 runner     (501) staff       (20)     5982 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ldsun.c
+-rw-r--r--   0 runner     (501) staff       (20)     7014 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/lteceq.c
+-rw-r--r--   0 runner     (501) staff       (20)     7567 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ltecm.c
+-rw-r--r--   0 runner     (501) staff       (20)     7019 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/lteqec.c
+-rw-r--r--   0 runner     (501) staff       (20)     6500 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ltp.c
+-rw-r--r--   0 runner     (501) staff       (20)     6581 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ltpb.c
+-rw-r--r--   0 runner     (501) staff       (20)     7601 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ltpecl.c
+-rw-r--r--   0 runner     (501) staff       (20)     7880 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ltpequ.c
+-rw-r--r--   0 runner     (501) staff       (20)    27755 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/makefile
+-rw-r--r--   0 runner     (501) staff       (20)     6728 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/num00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6713 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/num00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     6660 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/num06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6057 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/numat.c
+-rw-r--r--   0 runner     (501) staff       (20)   119801 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/nut00a.c
+-rw-r--r--   0 runner     (501) staff       (20)    19020 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/nut00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     7823 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/nut06a.c
+-rw-r--r--   0 runner     (501) staff       (20)    16295 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/nut80.c
+-rw-r--r--   0 runner     (501) staff       (20)     6473 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/nutm80.c
+-rw-r--r--   0 runner     (501) staff       (20)     6414 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/obl06.c
+-rw-r--r--   0 runner     (501) staff       (20)     6459 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/obl80.c
+-rw-r--r--   0 runner     (501) staff       (20)    13793 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/p06e.c
+-rw-r--r--   0 runner     (501) staff       (20)     5029 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/p2pv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5276 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/p2s.c
+-rw-r--r--   0 runner     (501) staff       (20)     6768 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pap.c
+-rw-r--r--   0 runner     (501) staff       (20)     5638 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pas.c
+-rw-r--r--   0 runner     (501) staff       (20)     7817 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pb06.c
+-rw-r--r--   0 runner     (501) staff       (20)     5008 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pdp.c
+-rw-r--r--   0 runner     (501) staff       (20)     7964 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pfw06.c
+-rw-r--r--   0 runner     (501) staff       (20)    23180 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/plan94.c
+-rw-r--r--   0 runner     (501) staff       (20)     4887 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pm.c
+-rw-r--r--   0 runner     (501) staff       (20)     6579 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pmat00.c
+-rw-r--r--   0 runner     (501) staff       (20)     6683 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pmat06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7548 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pmat76.c
+-rw-r--r--   0 runner     (501) staff       (20)     5090 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pmp.c
+-rw-r--r--   0 runner     (501) staff       (20)     7054 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pmpx.c
+-rw-r--r--   0 runner     (501) staff       (20)    10220 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pmsafe.c
+-rw-r--r--   0 runner     (501) staff       (20)     5495 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pn.c
+-rw-r--r--   0 runner     (501) staff       (20)     9146 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pn00.c
+-rw-r--r--   0 runner     (501) staff       (20)     8833 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pn00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     8825 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pn00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     9253 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pn06.c
+-rw-r--r--   0 runner     (501) staff       (20)     8282 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pn06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6802 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pnm00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6797 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pnm00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     6835 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pnm06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6778 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pnm80.c
+-rw-r--r--   0 runner     (501) staff       (20)     6453 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pom00.c
+-rw-r--r--   0 runner     (501) staff       (20)     5087 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ppp.c
+-rw-r--r--   0 runner     (501) staff       (20)     5275 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ppsp.c
+-rw-r--r--   0 runner     (501) staff       (20)     7813 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pr00.c
+-rw-r--r--   0 runner     (501) staff       (20)     8023 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/prec76.c
+-rw-r--r--   0 runner     (501) staff       (20)     4958 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pv2p.c
+-rw-r--r--   0 runner     (501) staff       (20)     6861 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pv2s.c
+-rw-r--r--   0 runner     (501) staff       (20)     5587 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pvdpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5073 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pvm.c
+-rw-r--r--   0 runner     (501) staff       (20)     5182 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pvmpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5177 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pvppv.c
+-rw-r--r--   0 runner     (501) staff       (20)    10128 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pvstar.c
+-rw-r--r--   0 runner     (501) staff       (20)     7712 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pvtob.c
+-rw-r--r--   0 runner     (501) staff       (20)     5373 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pvu.c
+-rw-r--r--   0 runner     (501) staff       (20)     5280 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pvup.c
+-rw-r--r--   0 runner     (501) staff       (20)     5842 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pvxpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5234 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/pxp.c
+-rw-r--r--   0 runner     (501) staff       (20)    11663 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/refco.c
+-rw-r--r--   0 runner     (501) staff       (20)     5989 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/rm2v.c
+-rw-r--r--   0 runner     (501) staff       (20)     5996 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/rv2m.c
+-rw-r--r--   0 runner     (501) staff       (20)     5807 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/rx.c
+-rw-r--r--   0 runner     (501) staff       (20)     5298 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/rxp.c
+-rw-r--r--   0 runner     (501) staff       (20)     5144 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/rxpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5337 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/rxr.c
+-rw-r--r--   0 runner     (501) staff       (20)     5848 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ry.c
+-rw-r--r--   0 runner     (501) staff       (20)     5817 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/rz.c
+-rw-r--r--   0 runner     (501) staff       (20)    15540 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/s00.c
+-rw-r--r--   0 runner     (501) staff       (20)     7781 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/s00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7772 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/s00b.c
+-rw-r--r--   0 runner     (501) staff       (20)    15442 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/s06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7799 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/s06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     5073 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/s2c.c
+-rw-r--r--   0 runner     (501) staff       (20)     5209 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/s2p.c
+-rw-r--r--   0 runner     (501) staff       (20)     5636 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/s2pv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5282 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/s2xpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5877 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/sepp.c
+-rw-r--r--   0 runner     (501) staff       (20)     5424 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/seps.c
+-rw-r--r--   0 runner     (501) staff       (20)    26863 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/sofa.h
+-rw-r--r--   0 runner     (501) staff       (20)     8772 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/sofam.h
+-rw-r--r--   0 runner     (501) staff       (20)     6557 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/sp00.c
+-rw-r--r--   0 runner     (501) staff       (20)    10677 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/starpm.c
+-rw-r--r--   0 runner     (501) staff       (20)    11959 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/starpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5038 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/sxp.c
+-rw-r--r--   0 runner     (501) staff       (20)     5101 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/sxpv.c
+-rw-r--r--   0 runner     (501) staff       (20)   241327 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/t_sofa_c.c
+-rw-r--r--   0 runner     (501) staff       (20)     5845 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/taitt.c
+-rw-r--r--   0 runner     (501) staff       (20)     5901 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/taiut1.c
+-rw-r--r--   0 runner     (501) staff       (20)     7493 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/taiutc.c
+-rw-r--r--   0 runner     (501) staff       (20)     6987 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/tcbtdb.c
+-rw-r--r--   0 runner     (501) staff       (20)     5845 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/tcgtt.c
+-rw-r--r--   0 runner     (501) staff       (20)     7109 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/tdbtcb.c
+-rw-r--r--   0 runner     (501) staff       (20)     6353 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/tdbtt.c
+-rw-r--r--   0 runner     (501) staff       (20)     6062 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/tf2a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6066 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/tf2d.c
+-rw-r--r--   0 runner     (501) staff       (20)     8685 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/tpors.c
+-rw-r--r--   0 runner     (501) staff       (20)     8649 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/tporv.c
+-rw-r--r--   0 runner     (501) staff       (20)     6534 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/tpsts.c
+-rw-r--r--   0 runner     (501) staff       (20)     7337 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/tpstv.c
+-rw-r--r--   0 runner     (501) staff       (20)     7253 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/tpxes.c
+-rw-r--r--   0 runner     (501) staff       (20)     7927 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/tpxev.c
+-rw-r--r--   0 runner     (501) staff       (20)     5136 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/tr.c
+-rw-r--r--   0 runner     (501) staff       (20)     5263 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/trxp.c
+-rw-r--r--   0 runner     (501) staff       (20)     5291 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/trxpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5841 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/tttai.c
+-rw-r--r--   0 runner     (501) staff       (20)     5913 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/tttcg.c
+-rw-r--r--   0 runner     (501) staff       (20)     6345 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/tttdb.c
+-rw-r--r--   0 runner     (501) staff       (20)     5794 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ttut1.c
+-rw-r--r--   0 runner     (501) staff       (20)     5898 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ut1tai.c
+-rw-r--r--   0 runner     (501) staff       (20)     5798 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ut1tt.c
+-rw-r--r--   0 runner     (501) staff       (20)     8782 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/ut1utc.c
+-rw-r--r--   0 runner     (501) staff       (20)     8283 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/utctai.c
+-rw-r--r--   0 runner     (501) staff       (20)     7458 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/utcut1.c
+-rw-r--r--   0 runner     (501) staff       (20)   133674 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/xy06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7028 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/xys00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7010 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/xys00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     7056 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/xys06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     4820 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/zp.c
+-rw-r--r--   0 runner     (501) staff       (20)     4874 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/zpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     4967 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/cextern/sofa/zr.c
+-rw-r--r--   0 runner     (501) staff       (20)     2389 2023-07-28 15:35:03.923222 sdss-coordio-1.8.1/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     2697 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-28 15:35:03.747826 sdss-coordio-1.8.1/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-28 15:35:03.906041 sdss-coordio-1.8.1/src/coordio/
+-rw-r--r--   0 runner     (501) staff       (20)     1178 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    12342 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/astrometry.py
+-rw-r--r--   0 runner     (501) staff       (20)     5635 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/calibration.py
+-rw-r--r--   0 runner     (501) staff       (20)    51063 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/conv.py
+-rw-r--r--   0 runner     (501) staff       (20)     9926 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/coordinate.py
+-rw-r--r--   0 runner     (501) staff       (20)     7570 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/defaults.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-28 15:35:03.907009 sdss-coordio-1.8.1/src/coordio/etc/
+-rw-r--r--   0 runner     (501) staff       (20)       73 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/etc/astrometrynet.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      366 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/etc/coordio.yml
+-rw-r--r--   0 runner     (501) staff       (20)      722 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/exceptions.py
+-rw-r--r--   0 runner     (501) staff       (20)    12748 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/extraction.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    13362 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/fitData.py
+-rw-r--r--   0 runner     (501) staff       (20)    30968 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/guide.py
+-rw-r--r--   0 runner     (501) staff       (20)     5870 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/iers.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-28 15:35:03.907522 sdss-coordio-1.8.1/src/coordio/include/
+-rw-r--r--   0 runner     (501) staff       (20)     1992 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/include/coordio.h
+-rw-r--r--   0 runner     (501) staff       (20)     4013 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/positioner.py
+-rw-r--r--   0 runner     (501) staff       (20)     4146 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/site.py
+-rw-r--r--   0 runner     (501) staff       (20)    14255 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/sky.py
+-rw-r--r--   0 runner     (501) staff       (20)     6440 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/sofa_bindings.py
+-rw-r--r--   0 runner     (501) staff       (20)    10661 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/tangent.py
+-rw-r--r--   0 runner     (501) staff       (20)    13390 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/telescope.py
+-rw-r--r--   0 runner     (501) staff       (20)     6451 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/time.py
+-rw-r--r--   0 runner     (501) staff       (20)    52635 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/transforms.py
+-rw-r--r--   0 runner     (501) staff       (20)    37978 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     3734 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/wok.py
+-rw-r--r--   0 runner     (501) staff       (20)    14872 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/zernike.py
+-rw-r--r--   0 runner     (501) staff       (20)    13102 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/src/coordio/zhaoburge.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-28 15:35:03.910738 sdss-coordio-1.8.1/src/sdss_coordio.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     1737 2023-07-28 15:35:03.000000 sdss-coordio-1.8.1/src/sdss_coordio.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     6867 2023-07-28 15:35:03.000000 sdss-coordio-1.8.1/src/sdss_coordio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-28 15:35:03.000000 sdss-coordio-1.8.1/src/sdss_coordio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-28 15:34:09.000000 sdss-coordio-1.8.1/src/sdss_coordio.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)      483 2023-07-28 15:35:03.000000 sdss-coordio-1.8.1/src/sdss_coordio.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        8 2023-07-28 15:35:03.000000 sdss-coordio-1.8.1/src/sdss_coordio.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-28 15:35:03.921256 sdss-coordio-1.8.1/tests/
+-rw-r--r--   0 runner     (501) staff       (20)    13006 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_conv.py
+-rw-r--r--   0 runner     (501) staff       (20)     7006 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_coordinate.py
+-rw-r--r--   0 runner     (501) staff       (20)     1386 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_fpScale.py
+-rw-r--r--   0 runner     (501) staff       (20)     4290 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_guide.py
+-rw-r--r--   0 runner     (501) staff       (20)     1418 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_iers.py
+-rw-r--r--   0 runner     (501) staff       (20)    11447 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_libcoordio.py
+-rw-r--r--   0 runner     (501) staff       (20)     9056 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_offset.py
+-rw-r--r--   0 runner     (501) staff       (20)     8074 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_plPlug.py
+-rw-r--r--   0 runner     (501) staff       (20)     5525 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_positioner.py
+-rw-r--r--   0 runner     (501) staff       (20)     1105 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_site.py
+-rw-r--r--   0 runner     (501) staff       (20)     5302 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_sky.py
+-rw-r--r--   0 runner     (501) staff       (20)     1171 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_sofa.py
+-rw-r--r--   0 runner     (501) staff       (20)     3340 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_tangent.py
+-rw-r--r--   0 runner     (501) staff       (20)     2738 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_tangentToPositioner2.py
+-rw-r--r--   0 runner     (501) staff       (20)    13872 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_telescope.py
+-rw-r--r--   0 runner     (501) staff       (20)     1407 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_time.py
+-rw-r--r--   0 runner     (501) staff       (20)     2588 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_wok.py
+-rw-r--r--   0 runner     (501) staff       (20)     1363 2023-07-28 15:33:39.000000 sdss-coordio-1.8.1/tests/test_zern.py
```

### Comparing `sdss-coordio-1.7.4a0/LICENSE.md` & `sdss-coordio-1.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/PKG-INFO` & `sdss-coordio-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-coordio
-Version: 1.7.4a0
+Version: 1.8.1
 Summary: Coordinate conversion for SDSS-V
 Home-page: https://github.com/sdss/coordio
 Author: Conor Sayres
 Author-email: csayres@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/coordio
 Project-URL: Documentation, https://sdss-coordio.readthedocs.org
```

### Comparing `sdss-coordio-1.7.4a0/README.md` & `sdss-coordio-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/conv.cpp` & `sdss-coordio-1.8.1/cextern/conv.cpp`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/dimage/dallpeaks.c` & `sdss-coordio-1.8.1/cextern/dimage/dallpeaks.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/dimage/dcen3x3.c` & `sdss-coordio-1.8.1/cextern/dimage/dcen3x3.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/dimage/dfind.c` & `sdss-coordio-1.8.1/cextern/dimage/dfind.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/dimage/dfloodfill.c` & `sdss-coordio-1.8.1/cextern/dimage/dfloodfill.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/dimage/dimage.h` & `sdss-coordio-1.8.1/cextern/dimage/dimage.h`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/dimage/dmedsmooth.c` & `sdss-coordio-1.8.1/cextern/dimage/dmedsmooth.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/dimage/dobjects.c` & `sdss-coordio-1.8.1/cextern/dimage/dobjects.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/dimage/dpeaks.c` & `sdss-coordio-1.8.1/cextern/dimage/dpeaks.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/dimage/drefine.c` & `sdss-coordio-1.8.1/cextern/dimage/drefine.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/dimage/dselip.c` & `sdss-coordio-1.8.1/cextern/dimage/dselip.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/dimage/dsigma.c` & `sdss-coordio-1.8.1/cextern/dimage/dsigma.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/dimage/dsmooth.c` & `sdss-coordio-1.8.1/cextern/dimage/dsmooth.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/dimage/simplexy.c` & `sdss-coordio-1.8.1/cextern/dimage/simplexy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/a2af.c` & `sdss-coordio-1.8.1/cextern/sofa/a2af.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/a2tf.c` & `sdss-coordio-1.8.1/cextern/sofa/a2tf.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ab.c` & `sdss-coordio-1.8.1/cextern/sofa/ab.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ae2hd.c` & `sdss-coordio-1.8.1/cextern/sofa/ae2hd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/af2a.c` & `sdss-coordio-1.8.1/cextern/sofa/af2a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/anp.c` & `sdss-coordio-1.8.1/cextern/sofa/anp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/anpm.c` & `sdss-coordio-1.8.1/cextern/sofa/anpm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/apcg.c` & `sdss-coordio-1.8.1/cextern/sofa/apcg.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/apcg13.c` & `sdss-coordio-1.8.1/cextern/sofa/apcg13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/apci.c` & `sdss-coordio-1.8.1/cextern/sofa/apci.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/apci13.c` & `sdss-coordio-1.8.1/cextern/sofa/apci13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/apco.c` & `sdss-coordio-1.8.1/cextern/sofa/apco.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/apco13.c` & `sdss-coordio-1.8.1/cextern/sofa/apco13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/apcs.c` & `sdss-coordio-1.8.1/cextern/sofa/apcs.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/apcs13.c` & `sdss-coordio-1.8.1/cextern/sofa/apcs13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/aper.c` & `sdss-coordio-1.8.1/cextern/sofa/aper.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/aper13.c` & `sdss-coordio-1.8.1/cextern/sofa/aper13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/apio.c` & `sdss-coordio-1.8.1/cextern/sofa/apio.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/apio13.c` & `sdss-coordio-1.8.1/cextern/sofa/apio13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/atci13.c` & `sdss-coordio-1.8.1/cextern/sofa/atci13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/atciq.c` & `sdss-coordio-1.8.1/cextern/sofa/atciq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/atciqn.c` & `sdss-coordio-1.8.1/cextern/sofa/atciqn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/atciqz.c` & `sdss-coordio-1.8.1/cextern/sofa/atciqz.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/atco13.c` & `sdss-coordio-1.8.1/cextern/sofa/atco13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/atic13.c` & `sdss-coordio-1.8.1/cextern/sofa/atic13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/aticq.c` & `sdss-coordio-1.8.1/cextern/sofa/aticq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/aticqn.c` & `sdss-coordio-1.8.1/cextern/sofa/aticqn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/atio13.c` & `sdss-coordio-1.8.1/cextern/sofa/atio13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/atioq.c` & `sdss-coordio-1.8.1/cextern/sofa/atioq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/atoc13.c` & `sdss-coordio-1.8.1/cextern/sofa/atoc13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/atoi13.c` & `sdss-coordio-1.8.1/cextern/sofa/atoi13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/atoiq.c` & `sdss-coordio-1.8.1/cextern/sofa/atoiq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/bi00.c` & `sdss-coordio-1.8.1/cextern/sofa/bi00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/bp00.c` & `sdss-coordio-1.8.1/cextern/sofa/bp00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/bp06.c` & `sdss-coordio-1.8.1/cextern/sofa/bp06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/bpn2xy.c` & `sdss-coordio-1.8.1/cextern/sofa/bpn2xy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/c2i00a.c` & `sdss-coordio-1.8.1/cextern/sofa/c2i00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/c2i00b.c` & `sdss-coordio-1.8.1/cextern/sofa/c2i00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/c2i06a.c` & `sdss-coordio-1.8.1/cextern/sofa/c2i06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/c2ibpn.c` & `sdss-coordio-1.8.1/cextern/sofa/c2ibpn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/c2ixy.c` & `sdss-coordio-1.8.1/cextern/sofa/c2ixy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/c2ixys.c` & `sdss-coordio-1.8.1/cextern/sofa/c2ixys.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/c2s.c` & `sdss-coordio-1.8.1/cextern/sofa/c2s.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/c2t00a.c` & `sdss-coordio-1.8.1/cextern/sofa/c2t00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/c2t00b.c` & `sdss-coordio-1.8.1/cextern/sofa/c2t00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/c2t06a.c` & `sdss-coordio-1.8.1/cextern/sofa/c2t06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/c2tcio.c` & `sdss-coordio-1.8.1/cextern/sofa/c2tcio.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/c2teqx.c` & `sdss-coordio-1.8.1/cextern/sofa/c2teqx.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/c2tpe.c` & `sdss-coordio-1.8.1/cextern/sofa/c2tpe.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/c2txy.c` & `sdss-coordio-1.8.1/cextern/sofa/c2txy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/cal2jd.c` & `sdss-coordio-1.8.1/cextern/sofa/cal2jd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/cp.c` & `sdss-coordio-1.8.1/cextern/sofa/cp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/cpv.c` & `sdss-coordio-1.8.1/cextern/sofa/cpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/cr.c` & `sdss-coordio-1.8.1/cextern/sofa/cr.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/d2dtf.c` & `sdss-coordio-1.8.1/cextern/sofa/d2dtf.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/d2tf.c` & `sdss-coordio-1.8.1/cextern/sofa/d2tf.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/dat.c` & `sdss-coordio-1.8.1/cextern/sofa/dat.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/dtdb.c` & `sdss-coordio-1.8.1/cextern/sofa/dtdb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/dtf2d.c` & `sdss-coordio-1.8.1/cextern/sofa/dtf2d.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/eceq06.c` & `sdss-coordio-1.8.1/cextern/sofa/eceq06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ecm06.c` & `sdss-coordio-1.8.1/cextern/sofa/ecm06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ee00.c` & `sdss-coordio-1.8.1/cextern/sofa/ee00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ee00a.c` & `sdss-coordio-1.8.1/cextern/sofa/ee00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ee00b.c` & `sdss-coordio-1.8.1/cextern/sofa/ee00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ee06a.c` & `sdss-coordio-1.8.1/cextern/sofa/ee06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/eect00.c` & `sdss-coordio-1.8.1/cextern/sofa/eect00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/eform.c` & `sdss-coordio-1.8.1/cextern/sofa/eform.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/eo06a.c` & `sdss-coordio-1.8.1/cextern/sofa/eo06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/eors.c` & `sdss-coordio-1.8.1/cextern/sofa/eors.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/epb.c` & `sdss-coordio-1.8.1/cextern/sofa/epb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/epb2jd.c` & `sdss-coordio-1.8.1/cextern/sofa/epb2jd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/epj.c` & `sdss-coordio-1.8.1/cextern/sofa/epj.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/epj2jd.c` & `sdss-coordio-1.8.1/cextern/sofa/epj2jd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/epv00.c` & `sdss-coordio-1.8.1/cextern/sofa/epv00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/eqec06.c` & `sdss-coordio-1.8.1/cextern/sofa/eqec06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/eqeq94.c` & `sdss-coordio-1.8.1/cextern/sofa/eqeq94.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/era00.c` & `sdss-coordio-1.8.1/cextern/sofa/era00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fad03.c` & `sdss-coordio-1.8.1/cextern/sofa/fad03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fae03.c` & `sdss-coordio-1.8.1/cextern/sofa/fae03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/faf03.c` & `sdss-coordio-1.8.1/cextern/sofa/faf03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/faju03.c` & `sdss-coordio-1.8.1/cextern/sofa/faju03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fal03.c` & `sdss-coordio-1.8.1/cextern/sofa/fal03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/falp03.c` & `sdss-coordio-1.8.1/cextern/sofa/falp03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fama03.c` & `sdss-coordio-1.8.1/cextern/sofa/fama03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fame03.c` & `sdss-coordio-1.8.1/cextern/sofa/fame03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fane03.c` & `sdss-coordio-1.8.1/cextern/sofa/fane03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/faom03.c` & `sdss-coordio-1.8.1/cextern/sofa/faom03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fapa03.c` & `sdss-coordio-1.8.1/cextern/sofa/fapa03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fasa03.c` & `sdss-coordio-1.8.1/cextern/sofa/fasa03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/faur03.c` & `sdss-coordio-1.8.1/cextern/sofa/faur03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fave03.c` & `sdss-coordio-1.8.1/cextern/sofa/fave03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fk425.c` & `sdss-coordio-1.8.1/cextern/sofa/fk425.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fk45z.c` & `sdss-coordio-1.8.1/cextern/sofa/fk45z.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fk524.c` & `sdss-coordio-1.8.1/cextern/sofa/fk524.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fk52h.c` & `sdss-coordio-1.8.1/cextern/sofa/fk52h.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fk54z.c` & `sdss-coordio-1.8.1/cextern/sofa/fk54z.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fk5hip.c` & `sdss-coordio-1.8.1/cextern/sofa/fk5hip.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fk5hz.c` & `sdss-coordio-1.8.1/cextern/sofa/fk5hz.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fw2m.c` & `sdss-coordio-1.8.1/cextern/sofa/fw2m.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/fw2xy.c` & `sdss-coordio-1.8.1/cextern/sofa/fw2xy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/g2icrs.c` & `sdss-coordio-1.8.1/cextern/sofa/g2icrs.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/gc2gd.c` & `sdss-coordio-1.8.1/cextern/sofa/gc2gd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/gc2gde.c` & `sdss-coordio-1.8.1/cextern/sofa/gc2gde.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/gd2gc.c` & `sdss-coordio-1.8.1/cextern/sofa/gd2gc.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/gd2gce.c` & `sdss-coordio-1.8.1/cextern/sofa/gd2gce.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/gmst00.c` & `sdss-coordio-1.8.1/cextern/sofa/gmst00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/gmst06.c` & `sdss-coordio-1.8.1/cextern/sofa/gmst06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/gmst82.c` & `sdss-coordio-1.8.1/cextern/sofa/gmst82.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/gst00a.c` & `sdss-coordio-1.8.1/cextern/sofa/gst00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/gst00b.c` & `sdss-coordio-1.8.1/cextern/sofa/gst00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/gst06.c` & `sdss-coordio-1.8.1/cextern/sofa/gst06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/gst06a.c` & `sdss-coordio-1.8.1/cextern/sofa/gst06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/gst94.c` & `sdss-coordio-1.8.1/cextern/sofa/gst94.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/h2fk5.c` & `sdss-coordio-1.8.1/cextern/sofa/h2fk5.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/hd2ae.c` & `sdss-coordio-1.8.1/cextern/sofa/hd2ae.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/hd2pa.c` & `sdss-coordio-1.8.1/cextern/sofa/hd2pa.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/hfk5z.c` & `sdss-coordio-1.8.1/cextern/sofa/hfk5z.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/icrs2g.c` & `sdss-coordio-1.8.1/cextern/sofa/icrs2g.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ir.c` & `sdss-coordio-1.8.1/cextern/sofa/ir.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/jd2cal.c` & `sdss-coordio-1.8.1/cextern/sofa/jd2cal.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/jdcalf.c` & `sdss-coordio-1.8.1/cextern/sofa/jdcalf.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ld.c` & `sdss-coordio-1.8.1/cextern/sofa/ld.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ldn.c` & `sdss-coordio-1.8.1/cextern/sofa/ldn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ldsun.c` & `sdss-coordio-1.8.1/cextern/sofa/ldsun.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/lteceq.c` & `sdss-coordio-1.8.1/cextern/sofa/lteceq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ltecm.c` & `sdss-coordio-1.8.1/cextern/sofa/ltecm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/lteqec.c` & `sdss-coordio-1.8.1/cextern/sofa/lteqec.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ltp.c` & `sdss-coordio-1.8.1/cextern/sofa/ltp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ltpb.c` & `sdss-coordio-1.8.1/cextern/sofa/ltpb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ltpecl.c` & `sdss-coordio-1.8.1/cextern/sofa/ltpecl.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ltpequ.c` & `sdss-coordio-1.8.1/cextern/sofa/ltpequ.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/makefile` & `sdss-coordio-1.8.1/cextern/sofa/makefile`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/num00a.c` & `sdss-coordio-1.8.1/cextern/sofa/num00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/num00b.c` & `sdss-coordio-1.8.1/cextern/sofa/num00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/num06a.c` & `sdss-coordio-1.8.1/cextern/sofa/num06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/numat.c` & `sdss-coordio-1.8.1/cextern/sofa/numat.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/nut00a.c` & `sdss-coordio-1.8.1/cextern/sofa/nut00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/nut00b.c` & `sdss-coordio-1.8.1/cextern/sofa/nut00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/nut06a.c` & `sdss-coordio-1.8.1/cextern/sofa/nut06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/nut80.c` & `sdss-coordio-1.8.1/cextern/sofa/nut80.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/nutm80.c` & `sdss-coordio-1.8.1/cextern/sofa/nutm80.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/obl06.c` & `sdss-coordio-1.8.1/cextern/sofa/obl06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/obl80.c` & `sdss-coordio-1.8.1/cextern/sofa/obl80.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/p06e.c` & `sdss-coordio-1.8.1/cextern/sofa/p06e.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/p2pv.c` & `sdss-coordio-1.8.1/cextern/sofa/p2pv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/p2s.c` & `sdss-coordio-1.8.1/cextern/sofa/p2s.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pap.c` & `sdss-coordio-1.8.1/cextern/sofa/pap.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pas.c` & `sdss-coordio-1.8.1/cextern/sofa/pas.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pb06.c` & `sdss-coordio-1.8.1/cextern/sofa/pb06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pdp.c` & `sdss-coordio-1.8.1/cextern/sofa/pdp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pfw06.c` & `sdss-coordio-1.8.1/cextern/sofa/pfw06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/plan94.c` & `sdss-coordio-1.8.1/cextern/sofa/plan94.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pm.c` & `sdss-coordio-1.8.1/cextern/sofa/pm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pmat00.c` & `sdss-coordio-1.8.1/cextern/sofa/pmat00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pmat06.c` & `sdss-coordio-1.8.1/cextern/sofa/pmat06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pmat76.c` & `sdss-coordio-1.8.1/cextern/sofa/pmat76.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pmp.c` & `sdss-coordio-1.8.1/cextern/sofa/pmp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pmpx.c` & `sdss-coordio-1.8.1/cextern/sofa/pmpx.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pmsafe.c` & `sdss-coordio-1.8.1/cextern/sofa/pmsafe.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pn.c` & `sdss-coordio-1.8.1/cextern/sofa/pn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pn00.c` & `sdss-coordio-1.8.1/cextern/sofa/pn00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pn00a.c` & `sdss-coordio-1.8.1/cextern/sofa/pn00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pn00b.c` & `sdss-coordio-1.8.1/cextern/sofa/pn00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pn06.c` & `sdss-coordio-1.8.1/cextern/sofa/pn06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pn06a.c` & `sdss-coordio-1.8.1/cextern/sofa/pn06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pnm00a.c` & `sdss-coordio-1.8.1/cextern/sofa/pnm00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pnm00b.c` & `sdss-coordio-1.8.1/cextern/sofa/pnm00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pnm06a.c` & `sdss-coordio-1.8.1/cextern/sofa/pnm06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pnm80.c` & `sdss-coordio-1.8.1/cextern/sofa/pnm80.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pom00.c` & `sdss-coordio-1.8.1/cextern/sofa/pom00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ppp.c` & `sdss-coordio-1.8.1/cextern/sofa/ppp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ppsp.c` & `sdss-coordio-1.8.1/cextern/sofa/ppsp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pr00.c` & `sdss-coordio-1.8.1/cextern/sofa/pr00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/prec76.c` & `sdss-coordio-1.8.1/cextern/sofa/prec76.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pv2p.c` & `sdss-coordio-1.8.1/cextern/sofa/pv2p.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pv2s.c` & `sdss-coordio-1.8.1/cextern/sofa/pv2s.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pvdpv.c` & `sdss-coordio-1.8.1/cextern/sofa/pvdpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pvm.c` & `sdss-coordio-1.8.1/cextern/sofa/pvm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pvmpv.c` & `sdss-coordio-1.8.1/cextern/sofa/pvmpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pvppv.c` & `sdss-coordio-1.8.1/cextern/sofa/pvppv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pvstar.c` & `sdss-coordio-1.8.1/cextern/sofa/pvstar.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pvtob.c` & `sdss-coordio-1.8.1/cextern/sofa/pvtob.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pvu.c` & `sdss-coordio-1.8.1/cextern/sofa/pvu.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pvup.c` & `sdss-coordio-1.8.1/cextern/sofa/pvup.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pvxpv.c` & `sdss-coordio-1.8.1/cextern/sofa/pvxpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/pxp.c` & `sdss-coordio-1.8.1/cextern/sofa/pxp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/refco.c` & `sdss-coordio-1.8.1/cextern/sofa/refco.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/rm2v.c` & `sdss-coordio-1.8.1/cextern/sofa/rm2v.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/rv2m.c` & `sdss-coordio-1.8.1/cextern/sofa/rv2m.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/rx.c` & `sdss-coordio-1.8.1/cextern/sofa/rx.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/rxp.c` & `sdss-coordio-1.8.1/cextern/sofa/rxp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/rxpv.c` & `sdss-coordio-1.8.1/cextern/sofa/rxpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/rxr.c` & `sdss-coordio-1.8.1/cextern/sofa/rxr.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ry.c` & `sdss-coordio-1.8.1/cextern/sofa/ry.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/rz.c` & `sdss-coordio-1.8.1/cextern/sofa/rz.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/s00.c` & `sdss-coordio-1.8.1/cextern/sofa/s00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/s00a.c` & `sdss-coordio-1.8.1/cextern/sofa/s00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/s00b.c` & `sdss-coordio-1.8.1/cextern/sofa/s00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/s06.c` & `sdss-coordio-1.8.1/cextern/sofa/s06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/s06a.c` & `sdss-coordio-1.8.1/cextern/sofa/s06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/s2c.c` & `sdss-coordio-1.8.1/cextern/sofa/s2c.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/s2p.c` & `sdss-coordio-1.8.1/cextern/sofa/s2p.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/s2pv.c` & `sdss-coordio-1.8.1/cextern/sofa/s2pv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/s2xpv.c` & `sdss-coordio-1.8.1/cextern/sofa/s2xpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/sepp.c` & `sdss-coordio-1.8.1/cextern/sofa/sepp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/seps.c` & `sdss-coordio-1.8.1/cextern/sofa/seps.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/sofa.h` & `sdss-coordio-1.8.1/cextern/sofa/sofa.h`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/sofam.h` & `sdss-coordio-1.8.1/cextern/sofa/sofam.h`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/sp00.c` & `sdss-coordio-1.8.1/cextern/sofa/sp00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/starpm.c` & `sdss-coordio-1.8.1/cextern/sofa/starpm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/starpv.c` & `sdss-coordio-1.8.1/cextern/sofa/starpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/sxp.c` & `sdss-coordio-1.8.1/cextern/sofa/sxp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/sxpv.c` & `sdss-coordio-1.8.1/cextern/sofa/sxpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/t_sofa_c.c` & `sdss-coordio-1.8.1/cextern/sofa/t_sofa_c.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/taitt.c` & `sdss-coordio-1.8.1/cextern/sofa/taitt.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/taiut1.c` & `sdss-coordio-1.8.1/cextern/sofa/taiut1.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/taiutc.c` & `sdss-coordio-1.8.1/cextern/sofa/taiutc.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/tcbtdb.c` & `sdss-coordio-1.8.1/cextern/sofa/tcbtdb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/tcgtt.c` & `sdss-coordio-1.8.1/cextern/sofa/tcgtt.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/tdbtcb.c` & `sdss-coordio-1.8.1/cextern/sofa/tdbtcb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/tdbtt.c` & `sdss-coordio-1.8.1/cextern/sofa/tdbtt.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/tf2a.c` & `sdss-coordio-1.8.1/cextern/sofa/tf2a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/tf2d.c` & `sdss-coordio-1.8.1/cextern/sofa/tf2d.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/tpors.c` & `sdss-coordio-1.8.1/cextern/sofa/tpors.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/tporv.c` & `sdss-coordio-1.8.1/cextern/sofa/tporv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/tpsts.c` & `sdss-coordio-1.8.1/cextern/sofa/tpsts.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/tpstv.c` & `sdss-coordio-1.8.1/cextern/sofa/tpstv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/tpxes.c` & `sdss-coordio-1.8.1/cextern/sofa/tpxes.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/tpxev.c` & `sdss-coordio-1.8.1/cextern/sofa/tpxev.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/tr.c` & `sdss-coordio-1.8.1/cextern/sofa/tr.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/trxp.c` & `sdss-coordio-1.8.1/cextern/sofa/trxp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/trxpv.c` & `sdss-coordio-1.8.1/cextern/sofa/trxpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/tttai.c` & `sdss-coordio-1.8.1/cextern/sofa/tttai.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/tttcg.c` & `sdss-coordio-1.8.1/cextern/sofa/tttcg.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/tttdb.c` & `sdss-coordio-1.8.1/cextern/sofa/tttdb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ttut1.c` & `sdss-coordio-1.8.1/cextern/sofa/ttut1.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ut1tai.c` & `sdss-coordio-1.8.1/cextern/sofa/ut1tai.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ut1tt.c` & `sdss-coordio-1.8.1/cextern/sofa/ut1tt.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/ut1utc.c` & `sdss-coordio-1.8.1/cextern/sofa/ut1utc.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/utctai.c` & `sdss-coordio-1.8.1/cextern/sofa/utctai.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/utcut1.c` & `sdss-coordio-1.8.1/cextern/sofa/utcut1.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/xy06.c` & `sdss-coordio-1.8.1/cextern/sofa/xy06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/xys00a.c` & `sdss-coordio-1.8.1/cextern/sofa/xys00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/xys00b.c` & `sdss-coordio-1.8.1/cextern/sofa/xys00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/xys06a.c` & `sdss-coordio-1.8.1/cextern/sofa/xys06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/zp.c` & `sdss-coordio-1.8.1/cextern/sofa/zp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/zpv.c` & `sdss-coordio-1.8.1/cextern/sofa/zpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/cextern/sofa/zr.c` & `sdss-coordio-1.8.1/cextern/sofa/zr.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/setup.cfg` & `sdss-coordio-1.8.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sdss-coordio
-version = 1.7.4a0
+version = 1.8.1
 author = Conor Sayres
 author_email = csayres@uw.edu
 description = Coordinate conversion for SDSS-V
 url = https://github.com/sdss/coordio
 project_urls = 
 	Repository = https://github.com/sdss/coordio
 	Documentation = https://sdss-coordio.readthedocs.org
```

### Comparing `sdss-coordio-1.7.4a0/setup.py` & `sdss-coordio-1.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/__init__.py` & `sdss-coordio-1.8.1/src/coordio/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/astrometry.py` & `sdss-coordio-1.8.1/src/coordio/astrometry.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/calibration.py` & `sdss-coordio-1.8.1/src/coordio/calibration.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/conv.py` & `sdss-coordio-1.8.1/src/coordio/conv.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/coordinate.py` & `sdss-coordio-1.8.1/src/coordio/coordinate.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/defaults.py` & `sdss-coordio-1.8.1/src/coordio/defaults.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/exceptions.py` & `sdss-coordio-1.8.1/src/coordio/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/extraction.py` & `sdss-coordio-1.8.1/src/coordio/extraction.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/fitData.py` & `sdss-coordio-1.8.1/src/coordio/fitData.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/guide.py` & `sdss-coordio-1.8.1/src/coordio/guide.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/iers.py` & `sdss-coordio-1.8.1/src/coordio/iers.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/include/coordio.h` & `sdss-coordio-1.8.1/src/coordio/include/coordio.h`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/positioner.py` & `sdss-coordio-1.8.1/src/coordio/positioner.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/site.py` & `sdss-coordio-1.8.1/src/coordio/site.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/sky.py` & `sdss-coordio-1.8.1/src/coordio/sky.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/sofa_bindings.py` & `sdss-coordio-1.8.1/src/coordio/sofa_bindings.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/tangent.py` & `sdss-coordio-1.8.1/src/coordio/tangent.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/telescope.py` & `sdss-coordio-1.8.1/src/coordio/telescope.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/time.py` & `sdss-coordio-1.8.1/src/coordio/time.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/transforms.py` & `sdss-coordio-1.8.1/src/coordio/transforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -455,37 +455,44 @@
     """Apply a full Zhao-Burge transformation.
 
 
     Residuals from a similarity tranform are fit with Zhao-Burge
     2D vector polynomials.
     """
 
-    def __init__(self, xyCCD, xyWok, polids=None):
+    def __init__(self, xyCCD, xyWok, polids=None, normFactor=1):
         """ Compute a transformation between xyCCD and xyWok using
         Zhao-Burge polynomials
 
         xyCCD and xyWok need to be a mapping by index
 
         Parameters
         ------------
         xyCCD : numpy.ndarray
             Nx2 array of xy ccd coordinates (pixels)
         xyWok :numpy.ndarray
             Nx2 array of xy wok coordinates (mm)
         polids : numpy.ndarray or None
             Mx1 array of integers specifying the ZB basis vectors to use.
             If not passed a default basis vector set is used.
+        normFactor : float
+            Scale xyWok coordinates by this factor.  Intended
+            use is for moving coordinates to unit circle. 330 is a good
+            choice, but default is 1 to remain backwards compatible
+            (no normalization)
 
         Attributes
         -------------
         polids : numpy.ndarray
             1D integer array containing basis IDs used for ZB transform
         coeffs : numpy.ndarray
             1D float array containing the fit coefficient values for each
             polid in the ZB transform
+        normFactor : float
+            normalization factor used
         simTrans : skimage.transform.SimilarityTransform
             similarity transform fit between xyCCD and xyWok
         unbiasedErrs : numpy.ndarray
             Nx1 array containing zb fit residuals (mm) at each
             jacknife iteration.  At each iter a single point is left out of the
             fit, and that point is used to measure predictive error of the
             model.
@@ -501,14 +508,19 @@
         if polids is None:
             self.polids = numpy.array(
                 [0, 1, 2, 3, 4, 5, 6, 9, 20, 28, 29], dtype=numpy.int16
             )
         else:
             self.polids = numpy.array(polids, dtype=numpy.int16)
 
+        if normFactor < 1:
+            raise CoordIOError("normFactor must >= 1")
+
+        self.normFactor = normFactor
+
         # First fit a transrotscale model
         self.simTrans = SimilarityTransform()
         self.simTrans.estimate(xyCCD, xyWok)
 
         # Apply the model to the data
         xySimTransFit = self.simTrans(xyCCD)
 
@@ -525,17 +537,24 @@
 
             polids, coeffs = fitZhaoBurge(
                 _xySimTransFit[:, 0],
                 _xySimTransFit[:, 1],
                 _xyWok[:, 0],
                 _xyWok[:, 1],
                 polids=self.polids,
+                normFactor=self.normFactor
             )
 
-            dx, dy = getZhaoBurgeXY(polids, coeffs, fitCheck[:, 0], fitCheck[:, 1])
+            dx, dy = getZhaoBurgeXY(
+                polids,
+                coeffs,
+                fitCheck[:, 0],
+                fitCheck[:, 1],
+                normFactor=self.normFactor
+            )
             zxfit = fitCheck[:, 0] + dx
             zyfit = fitCheck[:, 1] + dy
             zxyfit = numpy.array([zxfit, zyfit]).T
             self.unbiasedErrs.append(destCheck.squeeze() - zxyfit.squeeze())
 
         self.unbiasedErrs = numpy.array(self.unbiasedErrs)
         self.unbiasedRMS = numpy.sqrt(numpy.mean(self.unbiasedErrs ** 2))
@@ -544,21 +563,23 @@
 
         polids, self.coeffs = fitZhaoBurge(
             xySimTransFit[:, 0],
             xySimTransFit[:, 1],
             xyWok[:, 0],
             xyWok[:, 1],
             polids=self.polids,
+            normFactor=self.normFactor
         )
 
         dx, dy = getZhaoBurgeXY(
             polids,
             self.coeffs,
             xySimTransFit[:, 0],
             xySimTransFit[:, 1],
+            normFactor=self.normFactor
         )
 
         xWokFit = xySimTransFit[:, 0] + dx
         yWokFit = xySimTransFit[:, 1] + dy
         xyWokFit = numpy.array([xWokFit, yWokFit]).T
 
         self.xyWokIn = xyWok
@@ -588,14 +609,15 @@
 
         if zb:
             dx, dy = getZhaoBurgeXY(
                 self.polids,
                 self.coeffs,
                 xySimTransFit[:, 0],
                 xySimTransFit[:, 1],
+                normFactor=self.normFactor
             )
             xWokFit = xySimTransFit[:, 0] + dx
             yWokFit = xySimTransFit[:, 1] + dy
             xyWokFit = numpy.array([xWokFit, yWokFit]).T
         else:
             xyWokFit = xySimTransFit
 
@@ -853,15 +875,16 @@
         telRotAng,
         plotPathPrefix=None,
         positionerTable=calibration.positionerTable,
         wokCoords=calibration.wokCoords,
         fiducialCoords=calibration.fiducialCoords,
         telRotAngRef=None,
         polids=None,
-        nudgeAdjust=True
+        nudgeAdjust=True,
+        zbNormFactor=330
     ):
         """
         Parameters
         -------------
         fvcImgData : numpy.ndarray
             raw image data from the fvc
         positionerCoords : pandas.DataFrame
@@ -887,16 +910,22 @@
         telRotAngRef : float
             telescope rotator angle in mount coordinate degrees at
             which xyCCD ~= xyWok directions.
             Default is 135.4 (for APO)
         polids : 1D array or None
             list of integers for selecting zhaoburge basis polynomials.
             Default is supplied by class attribute polids
+        nudgeAdjust : boolean
+            if True, apply nudge correction to CCD detections
+        zbNormFactor : float
+            scale wok coordinates by this factor for unit circle
+            normalization when fitting ZhaoBurge transform.
         """
         self.nudgeAdjust = nudgeAdjust
+        self.zbNormFactor = zbNormFactor
 
         self.fvcImgData = numpy.array(fvcImgData, dtype=numpy.float32)
         # apply rough bias/background subtraction
         # rough bias/bg subtract
         imbias = numpy.median(self.fvcImgData, axis=0)
         imbias = numpy.outer(
             numpy.ones(self.fvcImgData.shape[0], dtype=numpy.float32),
@@ -1000,15 +1029,16 @@
             ("FVC_SPLM", self.simpleBoxSize, "box size for simple centroid algorithm (pix)"),
             ("FVC_RMS", self.positionerRMS, "robot rms (mm)"),
             ("FVC_FRMS", self.fiducialRMS, "fiducial rms (mm)"),
             ("FVC_CRMS", self.positionerRMS_clipped, "in-spec (outlier-clipped) robot rms (mm)"),
             ("FVC_SCL", self.fullTransform.simTrans.scale, "FVC model fit scale"),
             ("FVC_TRAX", self.fullTransform.simTrans.translation[0], "FVC model fit X translation"),
             ("FVC_TRAY", self.fullTransform.simTrans.translation[1], "FVC model fit Y translation"),
-            ("FVC_ROT", numpy.degrees(self.fullTransform.simTrans.rotation), "FVC model fit rotation (deg)")
+            ("FVC_ROT", numpy.degrees(self.fullTransform.simTrans.rotation), "FVC model fit rotation (deg)"),
+            ("FVC_ZNRM", self.zbNormFactor, "ZB normilization factor")
         ]
 
         # add in ZB coeffs
         for polid, coeff in zip(self.polids, self.fullTransform.coeffs):
             metaDataList.append(
                 ("FVC_ZB%i"%polid, coeff, "zhao-burge transform coeff for polid %i"%polid)
             )
@@ -1293,15 +1323,16 @@
             )
 
         # finally, do the full ZB transform based on all found FIF locations
         xyCCDFIF = xyCCD[xyWokMeas_idx]
         self.fullTransform = ZhaoBurgeTransform(
             xyCCDFIF,
             _xyWokFIF,
-            polids=self.polids
+            polids=self.polids,
+            normFactor=self.zbNormFactor
         )
 
         xyWokMeas = self.fullTransform.apply(xyCCD)
 
         # update the final measurements for positioners
         # and fiducials based on the fullTransform
         # dont enforce any minimum distance
```

### Comparing `sdss-coordio-1.7.4a0/src/coordio/utils.py` & `sdss-coordio-1.8.1/src/coordio/utils.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/wok.py` & `sdss-coordio-1.8.1/src/coordio/wok.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/zernike.py` & `sdss-coordio-1.8.1/src/coordio/zernike.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/src/coordio/zhaoburge.py` & `sdss-coordio-1.8.1/src/coordio/zhaoburge.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,29 +145,32 @@
 def normalizeArea(noll):
     # converts an edge=1 Zernike to an area=Pi normalized Zernike
     return np.sqrt(squares[noll])
 
 def getZ(noll, x, y):
     return normalizeArea(noll) * getZernFuncXY(convertNolltoBW(noll), x, y)
 
-def getZhaoBurgeXY(polids, coeffs, x, y):
+def getZhaoBurgeXY(polids, coeffs, x, y, normFactor=1):
     """
     Args:
         coeffs: array of coefficients
         x,y : locations at which to evaluate
     returns dx, dy arrays
     """
+    x = x / normFactor
+    y = y / normFactor
+
     dx = np.zeros(len(x))
     dy = np.zeros(len(y))
     for polid, coeff in zip(polids,coeffs):
         zbx, zby, _ = getZhaoBurgeTerm(polid, x, y)
         dx += coeff*zbx
         dy += coeff*zby
 
-    return dx, dy
+    return dx*normFactor, dy*normFactor
 
 def getZhaoBurgeTerm(polid, x, y):
 
     # Cartesian input x,y; cartesian output x, y, and label.
     # Calls getZ() and delivers area normalized ZB terms
     if polid==0:   # case "S2"  r^0, keep; X translate;
         result =  getZ(1,x,y), 0.0,            'S2'   # parm=0/13 translation
@@ -305,15 +308,21 @@
         # for adjustment of shift translation rotation
         xx, yy = transform(x, y, scale, rotation, offset_x, offset_y)
         zbpolids, zbcoeffs = fitZhaoBurge(xx, yy, xp, yp, zbpolids)
         return scale, rotation, offset_x, offset_y, zbpolids, zbcoeffs
     else:
         return scale, rotation, offset_x, offset_y
 
-def fitZhaoBurge(x, y, xp, yp, polids=None):
+
+def fitZhaoBurge(x, y, xp, yp, polids=None, normFactor=1):
+    x = x / normFactor
+    y = y / normFactor
+    xp = xp / normFactor
+    yp = yp / normFactor
+
     dx = xp-x
     dy = yp-y
 
     nx = len(x)
 
     # here we choose the polynomials
     # 0  = S2 = translation along X
```

### Comparing `sdss-coordio-1.7.4a0/src/sdss_coordio.egg-info/PKG-INFO` & `sdss-coordio-1.8.1/src/sdss_coordio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-coordio
-Version: 1.7.4a0
+Version: 1.8.1
 Summary: Coordinate conversion for SDSS-V
 Home-page: https://github.com/sdss/coordio
 Author: Conor Sayres
 Author-email: csayres@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/coordio
 Project-URL: Documentation, https://sdss-coordio.readthedocs.org
```

### Comparing `sdss-coordio-1.7.4a0/src/sdss_coordio.egg-info/SOURCES.txt` & `sdss-coordio-1.8.1/src/sdss_coordio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_conv.py` & `sdss-coordio-1.8.1/tests/test_conv.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_coordinate.py` & `sdss-coordio-1.8.1/tests/test_coordinate.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_fpScale.py` & `sdss-coordio-1.8.1/tests/test_fpScale.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_guide.py` & `sdss-coordio-1.8.1/tests/test_guide.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_iers.py` & `sdss-coordio-1.8.1/tests/test_iers.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_libcoordio.py` & `sdss-coordio-1.8.1/tests/test_libcoordio.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_offset.py` & `sdss-coordio-1.8.1/tests/test_offset.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_plPlug.py` & `sdss-coordio-1.8.1/tests/test_plPlug.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_positioner.py` & `sdss-coordio-1.8.1/tests/test_positioner.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_site.py` & `sdss-coordio-1.8.1/tests/test_site.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_sky.py` & `sdss-coordio-1.8.1/tests/test_sky.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_sofa.py` & `sdss-coordio-1.8.1/tests/test_sofa.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_tangent.py` & `sdss-coordio-1.8.1/tests/test_tangent.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_tangentToPositioner2.py` & `sdss-coordio-1.8.1/tests/test_tangentToPositioner2.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_telescope.py` & `sdss-coordio-1.8.1/tests/test_telescope.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_time.py` & `sdss-coordio-1.8.1/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_wok.py` & `sdss-coordio-1.8.1/tests/test_wok.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.4a0/tests/test_zern.py` & `sdss-coordio-1.8.1/tests/test_zern.py`

 * *Files identical despite different names*


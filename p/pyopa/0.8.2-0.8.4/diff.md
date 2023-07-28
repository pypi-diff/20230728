# Comparing `tmp/pyopa-0.8.2.tar.gz` & `tmp/pyopa-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopa-0.8.2.tar", last modified: Mon Apr 25 09:19:09 2022, max compression
+gzip compressed data, was "pyopa-0.8.4.tar", last modified: Fri Jul 28 12:54:44 2023, max compression
```

## Comparing `pyopa-0.8.2.tar` & `pyopa-0.8.4.tar`

### file list

```diff
@@ -1,412 +1,412 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 09:19:08.998655 pyopa-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (121)    16725 2022-04-25 09:18:50.000000 pyopa-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-04-25 09:18:50.000000 pyopa-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2018 2022-04-25 09:19:08.998655 pyopa-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-04-25 09:18:50.000000 pyopa-0.8.2/README
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-04-25 09:18:50.000000 pyopa-0.8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 09:19:08.946655 pyopa-0.8.2/c_source/
--rw-r--r--   0 runner    (1001) docker     (121)     2581 2022-04-25 09:18:50.000000 pyopa-0.8.2/c_source/DynProgr_scalar.c
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2022-04-25 09:18:50.000000 pyopa-0.8.2/c_source/DynProgr_scalar.h
--rw-r--r--   0 runner    (1001) docker     (121)    13065 2022-04-25 09:18:50.000000 pyopa-0.8.2/c_source/DynProgr_sse_byte.c
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-04-25 09:18:50.000000 pyopa-0.8.2/c_source/DynProgr_sse_byte.h
--rw-r--r--   0 runner    (1001) docker     (121)    10009 2022-04-25 09:18:50.000000 pyopa-0.8.2/c_source/DynProgr_sse_double.c
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-04-25 09:18:50.000000 pyopa-0.8.2/c_source/DynProgr_sse_double.h
--rw-r--r--   0 runner    (1001) docker     (121)    13501 2022-04-25 09:18:50.000000 pyopa-0.8.2/c_source/DynProgr_sse_short.c
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-04-25 09:18:50.000000 pyopa-0.8.2/c_source/DynProgr_sse_short.h
--rw-r--r--   0 runner    (1001) docker     (121)    22982 2022-04-25 09:18:50.000000 pyopa-0.8.2/c_source/EstimatePam.c
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-04-25 09:18:50.000000 pyopa-0.8.2/c_source/EstimatePam.h
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-04-25 09:18:50.000000 pyopa-0.8.2/c_source/Page_size.c
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-04-25 09:18:50.000000 pyopa-0.8.2/c_source/Page_size.h
--rw-r--r--   0 runner    (1001) docker     (121)    11066 2022-04-25 09:18:50.000000 pyopa-0.8.2/c_source/Python_extension.c
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-04-25 09:18:50.000000 pyopa-0.8.2/c_source/Python_extension.h
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-04-25 09:18:50.000000 pyopa-0.8.2/c_source/debug.h
--rw-r--r--   0 runner    (1001) docker     (121)     1652 2022-04-25 09:18:50.000000 pyopa-0.8.2/c_source/matrix.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 09:19:08.950655 pyopa-0.8.2/c_source/simde/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-04-25 09:18:52.000000 pyopa-0.8.2/c_source/simde/.git
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 09:19:08.950655 pyopa-0.8.2/c_source/simde/arm/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 09:19:08.970655 pyopa-0.8.2/c_source/simde/arm/neon/
--rw-r--r--   0 runner    (1001) docker     (121)     6276 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/aba.h
--rw-r--r--   0 runner    (1001) docker     (121)    15460 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/abd.h
--rw-r--r--   0 runner    (1001) docker     (121)     4266 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/abdl.h
--rw-r--r--   0 runner    (1001) docker     (121)    13752 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/abs.h
--rw-r--r--   0 runner    (1001) docker     (121)    21266 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/add.h
--rw-r--r--   0 runner    (1001) docker     (121)     7275 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/addhn.h
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/addl.h
--rw-r--r--   0 runner    (1001) docker     (121)     4141 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/addl_high.h
--rw-r--r--   0 runner    (1001) docker     (121)     8399 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/addlv.h
--rw-r--r--   0 runner    (1001) docker     (121)    10476 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/addv.h
--rw-r--r--   0 runner    (1001) docker     (121)     7501 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/addw.h
--rw-r--r--   0 runner    (1001) docker     (121)     6592 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/addw_high.h
--rw-r--r--   0 runner    (1001) docker     (121)    16286 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/and.h
--rw-r--r--   0 runner    (1001) docker     (121)     5564 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/bcax.h
--rw-r--r--   0 runner    (1001) docker     (121)    14608 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/bic.h
--rw-r--r--   0 runner    (1001) docker     (121)    26650 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/bsl.h
--rw-r--r--   0 runner    (1001) docker     (121)     5902 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/cage.h
--rw-r--r--   0 runner    (1001) docker     (121)     5934 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/cagt.h
--rw-r--r--   0 runner    (1001) docker     (121)    25317 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/ceq.h
--rw-r--r--   0 runner    (1001) docker     (121)    11098 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/ceqz.h
--rw-r--r--   0 runner    (1001) docker     (121)    27527 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/cge.h
--rw-r--r--   0 runner    (1001) docker     (121)    13009 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/cgez.h
--rw-r--r--   0 runner    (1001) docker     (121)    24738 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/cgt.h
--rw-r--r--   0 runner    (1001) docker     (121)    13030 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/cgtz.h
--rw-r--r--   0 runner    (1001) docker     (121)    25850 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/cle.h
--rw-r--r--   0 runner    (1001) docker     (121)    13121 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/clez.h
--rw-r--r--   0 runner    (1001) docker     (121)     4854 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/cls.h
--rw-r--r--   0 runner    (1001) docker     (121)    25069 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/clt.h
--rw-r--r--   0 runner    (1001) docker     (121)     9949 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/cltz.h
--rw-r--r--   0 runner    (1001) docker     (121)    12547 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/clz.h
--rw-r--r--   0 runner    (1001) docker     (121)     4712 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/cmla.h
--rw-r--r--   0 runner    (1001) docker     (121)     5339 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/cmla_rot180.h
--rw-r--r--   0 runner    (1001) docker     (121)     5385 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/cmla_rot270.h
--rw-r--r--   0 runner    (1001) docker     (121)     5367 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/cmla_rot90.h
--rw-r--r--   0 runner    (1001) docker     (121)     5869 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/cnt.h
--rw-r--r--   0 runner    (1001) docker     (121)    11610 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/combine.h
--rw-r--r--   0 runner    (1001) docker     (121)     5174 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/create.h
--rw-r--r--   0 runner    (1001) docker     (121)    39919 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/cvt.h
--rw-r--r--   0 runner    (1001) docker     (121)     6728 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/dot.h
--rw-r--r--   0 runner    (1001) docker     (121)    16404 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/dot_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)    45828 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/dup_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)    19922 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/dup_n.h
--rw-r--r--   0 runner    (1001) docker     (121)    16286 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/eor.h
--rw-r--r--   0 runner    (1001) docker     (121)    37965 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/ext.h
--rw-r--r--   0 runner    (1001) docker     (121)     4189 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/fma.h
--rw-r--r--   0 runner    (1001) docker     (121)     8714 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/fma_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)     3660 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/fma_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     9471 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/get_high.h
--rw-r--r--   0 runner    (1001) docker     (121)    14801 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/get_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)    10181 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/get_low.h
--rw-r--r--   0 runner    (1001) docker     (121)    10597 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/hadd.h
--rw-r--r--   0 runner    (1001) docker     (121)    10597 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/hsub.h
--rw-r--r--   0 runner    (1001) docker     (121)    14926 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/ld1.h
--rw-r--r--   0 runner    (1001) docker     (121)    11068 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/ld1_dup.h
--rw-r--r--   0 runner    (1001) docker     (121)    14058 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/ld1_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)    21392 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/ld2.h
--rw-r--r--   0 runner    (1001) docker     (121)    16637 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/ld3.h
--rw-r--r--   0 runner    (1001) docker     (121)    18030 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/ld4.h
--rw-r--r--   0 runner    (1001) docker     (121)    21587 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/ld4_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)    19557 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/max.h
--rw-r--r--   0 runner    (1001) docker     (121)     7025 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/maxnm.h
--rw-r--r--   0 runner    (1001) docker     (121)     9895 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/maxv.h
--rw-r--r--   0 runner    (1001) docker     (121)    21635 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/min.h
--rw-r--r--   0 runner    (1001) docker     (121)     7249 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/minnm.h
--rw-r--r--   0 runner    (1001) docker     (121)    10751 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/minv.h
--rw-r--r--   0 runner    (1001) docker     (121)     8908 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mla.h
--rw-r--r--   0 runner    (1001) docker     (121)    10388 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mla_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     5025 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mlal.h
--rw-r--r--   0 runner    (1001) docker     (121)     5259 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mlal_high.h
--rw-r--r--   0 runner    (1001) docker     (121)     4299 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mlal_high_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     4826 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mlal_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)     4149 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mlal_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     8654 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mls.h
--rw-r--r--   0 runner    (1001) docker     (121)     5586 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mls_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     3888 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mlsl.h
--rw-r--r--   0 runner    (1001) docker     (121)     4092 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mlsl_high.h
--rw-r--r--   0 runner    (1001) docker     (121)     4299 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mlsl_high_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     4826 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mlsl_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)     3110 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mlsl_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     7490 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/movl.h
--rw-r--r--   0 runner    (1001) docker     (121)     3784 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/movl_high.h
--rw-r--r--   0 runner    (1001) docker     (121)     5749 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/movn.h
--rw-r--r--   0 runner    (1001) docker     (121)     3905 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/movn_high.h
--rw-r--r--   0 runner    (1001) docker     (121)    16404 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mul.h
--rw-r--r--   0 runner    (1001) docker     (121)    23046 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mul_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)     6102 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mul_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     7990 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mull.h
--rw-r--r--   0 runner    (1001) docker     (121)     4044 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mull_high.h
--rw-r--r--   0 runner    (1001) docker     (121)     4634 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mull_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)     5368 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mull_n.h
--rw-r--r--   0 runner    (1001) docker     (121)    12486 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/mvn.h
--rw-r--r--   0 runner    (1001) docker     (121)    11885 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/neg.h
--rw-r--r--   0 runner    (1001) docker     (121)    14783 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/orn.h
--rw-r--r--   0 runner    (1001) docker     (121)    16254 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/orr.h
--rw-r--r--   0 runner    (1001) docker     (121)     6129 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/padal.h
--rw-r--r--   0 runner    (1001) docker     (121)    11574 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/padd.h
--rw-r--r--   0 runner    (1001) docker     (121)    10862 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/paddl.h
--rw-r--r--   0 runner    (1001) docker     (121)     8449 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/pmax.h
--rw-r--r--   0 runner    (1001) docker     (121)     9213 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/pmin.h
--rw-r--r--   0 runner    (1001) docker     (121)     8316 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qabs.h
--rw-r--r--   0 runner    (1001) docker     (121)    25575 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qadd.h
--rw-r--r--   0 runner    (1001) docker     (121)     5129 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qdmulh.h
--rw-r--r--   0 runner    (1001) docker     (121)     6291 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qdmulh_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)     2873 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qdmulh_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     5689 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qdmull.h
--rw-r--r--   0 runner    (1001) docker     (121)     8266 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qmovn.h
--rw-r--r--   0 runner    (1001) docker     (121)     4029 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qmovn_high.h
--rw-r--r--   0 runner    (1001) docker     (121)     5196 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qmovun.h
--rw-r--r--   0 runner    (1001) docker     (121)     8600 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qneg.h
--rw-r--r--   0 runner    (1001) docker     (121)     6167 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qrdmulh.h
--rw-r--r--   0 runner    (1001) docker     (121)     6252 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qrdmulh_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)     4088 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qrdmulh_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     4913 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qrshrn_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     3259 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qrshrun_n.h
--rw-r--r--   0 runner    (1001) docker     (121)    19189 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qshl.h
--rw-r--r--   0 runner    (1001) docker     (121)    17502 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qshlu_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     4888 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qshrn_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     3280 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qshrun_n.h
--rw-r--r--   0 runner    (1001) docker     (121)    22099 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qsub.h
--rw-r--r--   0 runner    (1001) docker     (121)    18234 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qtbl.h
--rw-r--r--   0 runner    (1001) docker     (121)    20301 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/qtbx.h
--rw-r--r--   0 runner    (1001) docker     (121)     6633 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/rbit.h
--rw-r--r--   0 runner    (1001) docker     (121)     7949 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/recpe.h
--rw-r--r--   0 runner    (1001) docker     (121)     3893 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/recps.h
--rw-r--r--   0 runner    (1001) docker     (121)    97470 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/reinterpret.h
--rw-r--r--   0 runner    (1001) docker     (121)     4718 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/rev16.h
--rw-r--r--   0 runner    (1001) docker     (121)     8045 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/rev32.h
--rw-r--r--   0 runner    (1001) docker     (121)    11921 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/rev64.h
--rw-r--r--   0 runner    (1001) docker     (121)    17720 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/rhadd.h
--rw-r--r--   0 runner    (1001) docker     (121)     4379 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/rnd.h
--rw-r--r--   0 runner    (1001) docker     (121)     4190 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/rndi.h
--rw-r--r--   0 runner    (1001) docker     (121)     4408 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/rndm.h
--rw-r--r--   0 runner    (1001) docker     (121)     4602 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/rndn.h
--rw-r--r--   0 runner    (1001) docker     (121)     4400 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/rndp.h
--rw-r--r--   0 runner    (1001) docker     (121)    45188 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/rshl.h
--rw-r--r--   0 runner    (1001) docker     (121)    18114 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/rshr_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     3506 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/rshrn_n.h
--rw-r--r--   0 runner    (1001) docker     (121)    12020 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/rsqrte.h
--rw-r--r--   0 runner    (1001) docker     (121)     4450 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/rsqrts.h
--rw-r--r--   0 runner    (1001) docker     (121)     8089 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/rsra_n.h
--rw-r--r--   0 runner    (1001) docker     (121)    13789 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/set_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)    37056 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/shl.h
--rw-r--r--   0 runner    (1001) docker     (121)    19519 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/shl_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/shll_n.h
--rw-r--r--   0 runner    (1001) docker     (121)    21291 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/shr_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     5227 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/shrn_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     9516 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/sqadd.h
--rw-r--r--   0 runner    (1001) docker     (121)     7798 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/sra_n.h
--rw-r--r--   0 runner    (1001) docker     (121)     9661 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/sri_n.h
--rw-r--r--   0 runner    (1001) docker     (121)    12358 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/st1.h
--rw-r--r--   0 runner    (1001) docker     (121)    12450 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/st1_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)    13088 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/st2.h
--rw-r--r--   0 runner    (1001) docker     (121)    14198 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/st2_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)    35028 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/st3.h
--rw-r--r--   0 runner    (1001) docker     (121)    14199 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/st3_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)    16018 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/st4.h
--rw-r--r--   0 runner    (1001) docker     (121)    14151 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/st4_lane.h
--rw-r--r--   0 runner    (1001) docker     (121)    19685 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/sub.h
--rw-r--r--   0 runner    (1001) docker     (121)     7275 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/subhn.h
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/subl.h
--rw-r--r--   0 runner    (1001) docker     (121)     4068 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/subl_high.h
--rw-r--r--   0 runner    (1001) docker     (121)     7418 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/subw.h
--rw-r--r--   0 runner    (1001) docker     (121)     7930 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/subw_high.h
--rw-r--r--   0 runner    (1001) docker     (121)     8375 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/tbl.h
--rw-r--r--   0 runner    (1001) docker     (121)     9359 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/tbx.h
--rw-r--r--   0 runner    (1001) docker     (121)     7435 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/trn.h
--rw-r--r--   0 runner    (1001) docker     (121)    14460 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/trn1.h
--rw-r--r--   0 runner    (1001) docker     (121)    14595 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/trn2.h
--rw-r--r--   0 runner    (1001) docker     (121)    18580 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/tst.h
--rw-r--r--   0 runner    (1001) docker     (121)    38668 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/types.h
--rw-r--r--   0 runner    (1001) docker     (121)     9983 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/uqadd.h
--rw-r--r--   0 runner    (1001) docker     (121)     7435 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/uzp.h
--rw-r--r--   0 runner    (1001) docker     (121)    21179 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/uzp1.h
--rw-r--r--   0 runner    (1001) docker     (121)    21357 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/uzp2.h
--rw-r--r--   0 runner    (1001) docker     (121)     2270 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/xar.h
--rw-r--r--   0 runner    (1001) docker     (121)     7435 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/zip.h
--rw-r--r--   0 runner    (1001) docker     (121)    22121 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/zip1.h
--rw-r--r--   0 runner    (1001) docker     (121)    20911 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon/zip2.h
--rw-r--r--   0 runner    (1001) docker     (121)     5589 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/neon.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 09:19:08.970655 pyopa-0.8.2/c_source/simde/arm/sve/
--rw-r--r--   0 runner    (1001) docker     (121)    55418 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/sve/add.h
--rw-r--r--   0 runner    (1001) docker     (121)    41067 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/sve/and.h
--rw-r--r--   0 runner    (1001) docker     (121)    24579 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/sve/cmplt.h
--rw-r--r--   0 runner    (1001) docker     (121)     2576 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/sve/cnt.h
--rw-r--r--   0 runner    (1001) docker     (121)    43805 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/sve/dup.h
--rw-r--r--   0 runner    (1001) docker     (121)    12726 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/sve/ld1.h
--rw-r--r--   0 runner    (1001) docker     (121)     2326 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/sve/ptest.h
--rw-r--r--   0 runner    (1001) docker     (121)     4419 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/sve/ptrue.h
--rw-r--r--   0 runner    (1001) docker     (121)    18612 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/sve/qadd.h
--rw-r--r--   0 runner    (1001) docker     (121)    66380 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/sve/reinterpret.h
--rw-r--r--   0 runner    (1001) docker     (121)    27124 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/sve/sel.h
--rw-r--r--   0 runner    (1001) docker     (121)    11772 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/sve/st1.h
--rw-r--r--   0 runner    (1001) docker     (121)    55418 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/sve/sub.h
--rw-r--r--   0 runner    (1001) docker     (121)    34105 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/sve/types.h
--rw-r--r--   0 runner    (1001) docker     (121)    31909 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/sve/whilelt.h
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/arm/sve.h
--rw-r--r--   0 runner    (1001) docker     (121)     9846 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/check.h
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/debug-trap.h
--rw-r--r--   0 runner    (1001) docker     (121)    77513 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/hedley.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 09:19:08.970655 pyopa-0.8.2/c_source/simde/mips/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 09:19:08.970655 pyopa-0.8.2/c_source/simde/mips/msa/
--rw-r--r--   0 runner    (1001) docker     (121)     7730 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/mips/msa/add_a.h
--rw-r--r--   0 runner    (1001) docker     (121)    14942 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/mips/msa/adds.h
--rw-r--r--   0 runner    (1001) docker     (121)     9262 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/mips/msa/adds_a.h
--rw-r--r--   0 runner    (1001) docker     (121)     5700 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/mips/msa/addv.h
--rw-r--r--   0 runner    (1001) docker     (121)     6970 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/mips/msa/addvi.h
--rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/mips/msa/and.h
--rw-r--r--   0 runner    (1001) docker     (121)     2820 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/mips/msa/andi.h
--rw-r--r--   0 runner    (1001) docker     (121)     6448 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/mips/msa/ld.h
--rw-r--r--   0 runner    (1001) docker     (121)     4432 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/mips/msa/madd.h
--rw-r--r--   0 runner    (1001) docker     (121)     3528 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/mips/msa/st.h
--rw-r--r--   0 runner    (1001) docker     (121)     5700 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/mips/msa/subv.h
--rw-r--r--   0 runner    (1001) docker     (121)    12037 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/mips/msa/types.h
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/mips/msa.h
--rw-r--r--   0 runner    (1001) docker     (121)    18009 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/simde-align.h
--rw-r--r--   0 runner    (1001) docker     (121)    17620 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/simde-arch.h
--rw-r--r--   0 runner    (1001) docker     (121)    40938 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/simde-common.h
--rw-r--r--   0 runner    (1001) docker     (121)     5257 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/simde-complex.h
--rw-r--r--   0 runner    (1001) docker     (121)    18585 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/simde-constify.h
--rw-r--r--   0 runner    (1001) docker     (121)     5054 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/simde-detect-clang.h
--rw-r--r--   0 runner    (1001) docker     (121)    20459 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/simde-diagnostic.h
--rw-r--r--   0 runner    (1001) docker     (121)     9088 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/simde-f16.h
--rw-r--r--   0 runner    (1001) docker     (121)    22856 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/simde-features.h
--rw-r--r--   0 runner    (1001) docker     (121)    58922 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/simde-math.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 09:19:08.970655 pyopa-0.8.2/c_source/simde/wasm/
--rw-r--r--   0 runner    (1001) docker     (121)    17450 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/wasm/relaxed-simd.h
--rw-r--r--   0 runner    (1001) docker     (121)   303675 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/wasm/simd128.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 09:19:08.974655 pyopa-0.8.2/c_source/simde/x86/
--rw-r--r--   0 runner    (1001) docker     (121)   196755 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx.h
--rw-r--r--   0 runner    (1001) docker     (121)   197650 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx2.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 09:19:08.986655 pyopa-0.8.2/c_source/simde/x86/avx512/
--rw-r--r--   0 runner    (1001) docker     (121)     8026 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/2intersect.h
--rw-r--r--   0 runner    (1001) docker     (121)     2637 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/4dpwssd.h
--rw-r--r--   0 runner    (1001) docker     (121)     2672 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/4dpwssds.h
--rw-r--r--   0 runner    (1001) docker     (121)    19089 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/abs.h
--rw-r--r--   0 runner    (1001) docker     (121)    21097 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/add.h
--rw-r--r--   0 runner    (1001) docker     (121)    18352 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/adds.h
--rw-r--r--   0 runner    (1001) docker     (121)     9570 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/and.h
--rw-r--r--   0 runner    (1001) docker     (121)     7564 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/andnot.h
--rw-r--r--   0 runner    (1001) docker     (121)     8799 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/avg.h
--rw-r--r--   0 runner    (1001) docker     (121)     7989 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/bitshuffle.h
--rw-r--r--   0 runner    (1001) docker     (121)     9480 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/blend.h
--rw-r--r--   0 runner    (1001) docker     (121)    29208 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/broadcast.h
--rw-r--r--   0 runner    (1001) docker     (121)     9094 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/cast.h
--rw-r--r--   0 runner    (1001) docker     (121)    20945 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/cmp.h
--rw-r--r--   0 runner    (1001) docker     (121)     6448 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/cmpeq.h
--rw-r--r--   0 runner    (1001) docker     (121)    50531 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/cmpge.h
--rw-r--r--   0 runner    (1001) docker     (121)     6266 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/cmpgt.h
--rw-r--r--   0 runner    (1001) docker     (121)    50422 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/cmple.h
--rw-r--r--   0 runner    (1001) docker     (121)     4022 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/cmplt.h
--rw-r--r--   0 runner    (1001) docker     (121)    17516 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/cmpneq.h
--rw-r--r--   0 runner    (1001) docker     (121)    21624 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/compress.h
--rw-r--r--   0 runner    (1001) docker     (121)    11984 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/conflict.h
--rw-r--r--   0 runner    (1001) docker     (121)     3008 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/copysign.h
--rw-r--r--   0 runner    (1001) docker     (121)     8860 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/cvt.h
--rw-r--r--   0 runner    (1001) docker     (121)    23453 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/cvts.h
--rw-r--r--   0 runner    (1001) docker     (121)     3794 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/cvtt.h
--rw-r--r--   0 runner    (1001) docker     (121)    15983 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/dbsad.h
--rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/div.h
--rw-r--r--   0 runner    (1001) docker     (121)     9799 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/dpbf16.h
--rw-r--r--   0 runner    (1001) docker     (121)    10824 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/dpbusd.h
--rw-r--r--   0 runner    (1001) docker     (121)    13835 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/dpbusds.h
--rw-r--r--   0 runner    (1001) docker     (121)     8962 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/dpwssd.h
--rw-r--r--   0 runner    (1001) docker     (121)    11188 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/dpwssds.h
--rw-r--r--   0 runner    (1001) docker     (121)     3115 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/expand.h
--rw-r--r--   0 runner    (1001) docker     (121)     9050 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/extract.h
--rw-r--r--   0 runner    (1001) docker     (121)    28836 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/fixupimm.h
--rw-r--r--   0 runner    (1001) docker     (121)    26373 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/fixupimm_round.h
--rw-r--r--   0 runner    (1001) docker     (121)     2380 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/flushsubnormal.h
--rw-r--r--   0 runner    (1001) docker     (121)     4563 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/fmadd.h
--rw-r--r--   0 runner    (1001) docker     (121)     9231 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/fmsub.h
--rw-r--r--   0 runner    (1001) docker     (121)     3620 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/fnmadd.h
--rw-r--r--   0 runner    (1001) docker     (121)     3620 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/fnmsub.h
--rw-r--r--   0 runner    (1001) docker     (121)    18325 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/insert.h
--rw-r--r--   0 runner    (1001) docker     (121)     6599 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/kshift.h
--rw-r--r--   0 runner    (1001) docker     (121)     2556 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/load.h
--rw-r--r--   0 runner    (1001) docker     (121)     4062 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/loadu.h
--rw-r--r--   0 runner    (1001) docker     (121)     7815 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/lzcnt.h
--rw-r--r--   0 runner    (1001) docker     (121)     5950 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/madd.h
--rw-r--r--   0 runner    (1001) docker     (121)     6126 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/maddubs.h
--rw-r--r--   0 runner    (1001) docker     (121)    18597 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/max.h
--rw-r--r--   0 runner    (1001) docker     (121)    18599 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/min.h
--rw-r--r--   0 runner    (1001) docker     (121)    30273 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/mov.h
--rw-r--r--   0 runner    (1001) docker     (121)    11929 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/mov_mask.h
--rw-r--r--   0 runner    (1001) docker     (121)    15715 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/movm.h
--rw-r--r--   0 runner    (1001) docker     (121)     9151 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/mul.h
--rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/mulhi.h
--rw-r--r--   0 runner    (1001) docker     (121)     2272 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/mulhrs.h
--rw-r--r--   0 runner    (1001) docker     (121)     5509 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/mullo.h
--rw-r--r--   0 runner    (1001) docker     (121)     6519 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/multishift.h
--rw-r--r--   0 runner    (1001) docker     (121)     2639 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/negate.h
--rw-r--r--   0 runner    (1001) docker     (121)     9812 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/or.h
--rw-r--r--   0 runner    (1001) docker     (121)     6819 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/packs.h
--rw-r--r--   0 runner    (1001) docker     (121)     6833 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/packus.h
--rw-r--r--   0 runner    (1001) docker     (121)    69997 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/permutex2var.h
--rw-r--r--   0 runner    (1001) docker     (121)    49807 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/permutexvar.h
--rw-r--r--   0 runner    (1001) docker     (121)    46335 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/popcnt.h
--rw-r--r--   0 runner    (1001) docker     (121)    27800 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/range.h
--rw-r--r--   0 runner    (1001) docker     (121)    25064 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/range_round.h
--rw-r--r--   0 runner    (1001) docker     (121)    14839 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/rol.h
--rw-r--r--   0 runner    (1001) docker     (121)    14812 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/rolv.h
--rw-r--r--   0 runner    (1001) docker     (121)    14869 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/ror.h
--rw-r--r--   0 runner    (1001) docker     (121)    14732 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/rorv.h
--rw-r--r--   0 runner    (1001) docker     (121)    12991 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/round.h
--rw-r--r--   0 runner    (1001) docker     (121)    23118 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/roundscale.h
--rw-r--r--   0 runner    (1001) docker     (121)    26544 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/roundscale_round.h
--rw-r--r--   0 runner    (1001) docker     (121)     2638 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/sad.h
--rw-r--r--   0 runner    (1001) docker     (121)    14266 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/scalef.h
--rw-r--r--   0 runner    (1001) docker     (121)    15717 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/set.h
--rw-r--r--   0 runner    (1001) docker     (121)     9209 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/set1.h
--rw-r--r--   0 runner    (1001) docker     (121)     3705 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/set4.h
--rw-r--r--   0 runner    (1001) docker     (121)     2104 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/setone.h
--rw-r--r--   0 runner    (1001) docker     (121)     4723 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/setr.h
--rw-r--r--   0 runner    (1001) docker     (121)     3735 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/setr4.h
--rw-r--r--   0 runner    (1001) docker     (121)     2924 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/setzero.h
--rw-r--r--   0 runner    (1001) docker     (121)     5050 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/shldv.h
--rw-r--r--   0 runner    (1001) docker     (121)    10711 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/shuffle.h
--rw-r--r--   0 runner    (1001) docker     (121)     8169 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/sll.h
--rw-r--r--   0 runner    (1001) docker     (121)     6854 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/slli.h
--rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/sllv.h
--rw-r--r--   0 runner    (1001) docker     (121)     3977 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/sqrt.h
--rw-r--r--   0 runner    (1001) docker     (121)     2684 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/sra.h
--rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/srai.h
--rw-r--r--   0 runner    (1001) docker     (121)     2271 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/srav.h
--rw-r--r--   0 runner    (1001) docker     (121)     6928 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/srl.h
--rw-r--r--   0 runner    (1001) docker     (121)     6641 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/srli.h
--rw-r--r--   0 runner    (1001) docker     (121)     9485 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/srlv.h
--rw-r--r--   0 runner    (1001) docker     (121)     3507 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/store.h
--rw-r--r--   0 runner    (1001) docker     (121)     3429 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/storeu.h
--rw-r--r--   0 runner    (1001) docker     (121)    10888 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/sub.h
--rw-r--r--   0 runner    (1001) docker     (121)     7107 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/subs.h
--rw-r--r--   0 runner    (1001) docker     (121)   112262 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/ternarylogic.h
--rw-r--r--   0 runner    (1001) docker     (121)     7540 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/test.h
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/testn.h
--rw-r--r--   0 runner    (1001) docker     (121)    31286 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/types.h
--rw-r--r--   0 runner    (1001) docker     (121)    28925 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/unpackhi.h
--rw-r--r--   0 runner    (1001) docker     (121)    28831 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/unpacklo.h
--rw-r--r--   0 runner    (1001) docker     (121)    10505 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/xor.h
--rw-r--r--   0 runner    (1001) docker     (121)     2426 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512/xorsign.h
--rw-r--r--   0 runner    (1001) docker     (121)     4134 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/avx512.h
--rw-r--r--   0 runner    (1001) docker     (121)    16019 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/clmul.h
--rw-r--r--   0 runner    (1001) docker     (121)     5539 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/f16c.h
--rw-r--r--   0 runner    (1001) docker     (121)    22155 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/fma.h
--rw-r--r--   0 runner    (1001) docker     (121)    53191 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/gfni.h
--rw-r--r--   0 runner    (1001) docker     (121)    76704 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/mmx.h
--rw-r--r--   0 runner    (1001) docker     (121)   156055 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/sse.h
--rw-r--r--   0 runner    (1001) docker     (121)   255138 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/sse2.h
--rw-r--r--   0 runner    (1001) docker     (121)    16133 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/sse3.h
--rw-r--r--   0 runner    (1001) docker     (121)    79366 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/sse4.1.h
--rw-r--r--   0 runner    (1001) docker     (121)    13033 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/sse4.2.h
--rw-r--r--   0 runner    (1001) docker     (121)    36284 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/ssse3.h
--rw-r--r--   0 runner    (1001) docker     (121)   398844 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/svml.h
--rw-r--r--   0 runner    (1001) docker     (121)   118352 2022-04-25 09:18:53.000000 pyopa-0.8.2/c_source/simde/x86/xop.h
--rw-r--r--   0 runner    (1001) docker     (121)     2097 2022-04-25 09:18:50.000000 pyopa-0.8.2/c_source/swps3.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 09:19:08.986655 pyopa-0.8.2/pyopa/
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-04-25 09:18:50.000000 pyopa-0.8.2/pyopa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-04-25 09:18:50.000000 pyopa-0.8.2/pyopa/aligner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 09:19:08.990655 pyopa-0.8.2/pyopa/backend/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-25 09:18:50.000000 pyopa-0.8.2/pyopa/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2445 2022-04-25 09:18:50.000000 pyopa-0.8.2/pyopa/backend/cpyopa.pxd
--rw-r--r--   0 runner    (1001) docker     (121)  1007543 2022-04-25 09:19:06.000000 pyopa-0.8.2/pyopa/backend/pyopa.c
--rw-r--r--   0 runner    (1001) docker     (121)    27607 2022-04-25 09:18:50.000000 pyopa-0.8.2/pyopa/backend/pyopa.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 09:19:08.990655 pyopa-0.8.2/pyopa/matrices/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 09:19:08.998655 pyopa-0.8.2/pyopa/matrices/json/
--rw-r--r--   0 runner    (1001) docker     (121) 10824093 2022-04-25 09:18:51.000000 pyopa-0.8.2/pyopa/matrices/json/all_matrices.json
--rw-r--r--   0 runner    (1001) docker     (121)     9510 2022-04-25 09:18:51.000000 pyopa-0.8.2/pyopa/matrices/json/logPAM1.json
--rw-r--r--   0 runner    (1001) docker     (121)     8382 2022-04-25 09:18:51.000000 pyopa-0.8.2/pyopa/matrices/json/logPAM1_unscaled.json
--rw-r--r--   0 runner    (1001) docker     (121)     2960 2022-04-25 09:18:51.000000 pyopa-0.8.2/pyopa/matrices/jtt.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 09:19:08.986655 pyopa-0.8.2/pyopa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2018 2022-04-25 09:19:08.000000 pyopa-0.8.2/pyopa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12336 2022-04-25 09:19:08.000000 pyopa-0.8.2/pyopa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-25 09:19:08.000000 pyopa-0.8.2/pyopa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-25 09:19:08.000000 pyopa-0.8.2/pyopa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-25 09:19:08.000000 pyopa-0.8.2/pyopa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-04-25 09:18:51.000000 pyopa-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-25 09:18:51.000000 pyopa-0.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-25 09:19:08.998655 pyopa-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2155 2022-04-25 09:18:51.000000 pyopa-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-25 09:19:08.998655 pyopa-0.8.2/test/
--rw-r--r--   0 runner    (1001) docker     (121)     9042 2022-04-25 09:18:51.000000 pyopa-0.8.2/test/test_darwin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2022-04-25 09:18:51.000000 pyopa-0.8.2/test/test_env.py
--rw-r--r--   0 runner    (1001) docker     (121)     8987 2022-04-25 09:18:51.000000 pyopa-0.8.2/test/test_input.py
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-04-25 09:18:51.000000 pyopa-0.8.2/test/test_run_time_long_alignment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:44.336959 pyopa-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-28 12:54:28.000000 pyopa-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-28 12:54:28.000000 pyopa-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-28 12:54:44.336959 pyopa-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-28 12:54:28.000000 pyopa-0.8.4/README
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-28 12:54:28.000000 pyopa-0.8.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:44.272959 pyopa-0.8.4/c_source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-28 12:54:28.000000 pyopa-0.8.4/c_source/DynProgr_scalar.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-28 12:54:28.000000 pyopa-0.8.4/c_source/DynProgr_scalar.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-07-28 12:54:28.000000 pyopa-0.8.4/c_source/DynProgr_sse_byte.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-28 12:54:28.000000 pyopa-0.8.4/c_source/DynProgr_sse_byte.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-07-28 12:54:28.000000 pyopa-0.8.4/c_source/DynProgr_sse_double.c
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-28 12:54:28.000000 pyopa-0.8.4/c_source/DynProgr_sse_double.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-28 12:54:28.000000 pyopa-0.8.4/c_source/DynProgr_sse_short.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-28 12:54:28.000000 pyopa-0.8.4/c_source/DynProgr_sse_short.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22982 2023-07-28 12:54:28.000000 pyopa-0.8.4/c_source/EstimatePam.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-28 12:54:28.000000 pyopa-0.8.4/c_source/EstimatePam.h
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-28 12:54:28.000000 pyopa-0.8.4/c_source/Page_size.c
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-28 12:54:28.000000 pyopa-0.8.4/c_source/Page_size.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-07-28 12:54:28.000000 pyopa-0.8.4/c_source/Python_extension.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-28 12:54:28.000000 pyopa-0.8.4/c_source/Python_extension.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-28 12:54:28.000000 pyopa-0.8.4/c_source/debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-28 12:54:28.000000 pyopa-0.8.4/c_source/matrix.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:44.272959 pyopa-0.8.4/c_source/simde/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-28 12:54:29.000000 pyopa-0.8.4/c_source/simde/.git
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:44.276959 pyopa-0.8.4/c_source/simde/arm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:44.296959 pyopa-0.8.4/c_source/simde/arm/neon/
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/aba.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15460 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/abd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/abdl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/abs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21266 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/add.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/addhn.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/addl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/addl_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/addlv.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/addv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/addw.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/addw_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/bcax.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/bic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26650 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/bsl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/cage.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/cagt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25317 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/ceq.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/ceqz.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27527 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/cge.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/cgez.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24738 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/cgt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/cgtz.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25850 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/cle.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/clez.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/cls.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25069 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/clt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/cltz.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/clz.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/cmla.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/cmla_rot180.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/cmla_rot270.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/cmla_rot90.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/cnt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/combine.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/create.h
+-rw-r--r--   0 runner    (1001) docker     (123)    39919 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/cvt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/dot.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16404 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/dot_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45828 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/dup_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19922 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/dup_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/eor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37965 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/ext.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/fma.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/fma_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/fma_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/get_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/get_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/get_low.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/hadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/hsub.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14926 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/ld1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/ld1_dup.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/ld1_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/ld2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16637 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/ld3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18030 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/ld4.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/ld4_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/max.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/maxnm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/maxv.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21635 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/min.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/minnm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/minv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mla.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mla_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mlal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mlal_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mlal_high_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mlal_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mlal_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mls.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mls_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mlsl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mlsl_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mlsl_high_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mlsl_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mlsl_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/movl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/movl_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/movn.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/movn_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16404 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mul.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23046 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mul_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mul_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mull_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mull_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mull_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/mvn.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/neg.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/orn.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16254 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/orr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/padal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11574 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/padd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/paddl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/pmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/pmin.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qabs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25575 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qdmulh.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qdmulh_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qdmulh_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qdmull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qmovn.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qmovn_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qmovun.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qneg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qrdmulh.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qrdmulh_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qrdmulh_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qrshrn_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qrshrun_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qshl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17502 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qshlu_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qshrn_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qshrun_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22099 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qsub.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qtbl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20301 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/qtbx.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/rbit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/recpe.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/recps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    97470 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/reinterpret.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/rev16.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/rev32.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/rev64.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/rhadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/rnd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/rndi.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/rndm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/rndn.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/rndp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45188 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/rshl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18114 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/rshr_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/rshrn_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/rsqrte.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/rsqrts.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/rsra_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/set_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37056 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/shl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19519 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/shl_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/shll_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/shr_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/shrn_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/sqadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/sra_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/sri_n.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/st1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/st1_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/st2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/st2_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35028 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/st3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/st3_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/st4.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14151 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/st4_lane.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/sub.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/subhn.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/subl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/subl_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/subw.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/subw_high.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/tbl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/tbx.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/trn.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14460 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/trn1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/trn2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18580 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/tst.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38668 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/uqadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/uzp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21179 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/uzp1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21357 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/uzp2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/xar.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/zip.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22121 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/zip1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20911 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon/zip2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/neon.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:44.300959 pyopa-0.8.4/c_source/simde/arm/sve/
+-rw-r--r--   0 runner    (1001) docker     (123)    55418 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/sve/add.h
+-rw-r--r--   0 runner    (1001) docker     (123)    41067 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/sve/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24579 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/sve/cmplt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/sve/cnt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    43805 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/sve/dup.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12726 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/sve/ld1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/sve/ptest.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/sve/ptrue.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18612 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/sve/qadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    66380 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/sve/reinterpret.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27124 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/sve/sel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/sve/st1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    55418 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/sve/sub.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34105 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/sve/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31909 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/sve/whilelt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/arm/sve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/check.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/debug-trap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    77513 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/hedley.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:44.300959 pyopa-0.8.4/c_source/simde/mips/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:44.300959 pyopa-0.8.4/c_source/simde/mips/msa/
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/mips/msa/add_a.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/mips/msa/adds.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/mips/msa/adds_a.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/mips/msa/addv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/mips/msa/addvi.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/mips/msa/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/mips/msa/andi.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/mips/msa/ld.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/mips/msa/madd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/mips/msa/st.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/mips/msa/subv.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/mips/msa/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/mips/msa.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18009 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/simde-align.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/simde-arch.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40938 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/simde-common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/simde-complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18585 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/simde-constify.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/simde-detect-clang.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20459 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/simde-diagnostic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/simde-f16.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22856 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/simde-features.h
+-rw-r--r--   0 runner    (1001) docker     (123)    58922 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/simde-math.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:44.300959 pyopa-0.8.4/c_source/simde/wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/wasm/relaxed-simd.h
+-rw-r--r--   0 runner    (1001) docker     (123)   303675 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/wasm/simd128.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:44.304959 pyopa-0.8.4/c_source/simde/x86/
+-rw-r--r--   0 runner    (1001) docker     (123)   196755 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx.h
+-rw-r--r--   0 runner    (1001) docker     (123)   197650 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx2.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:44.320959 pyopa-0.8.4/c_source/simde/x86/avx512/
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/2intersect.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/4dpwssd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/4dpwssds.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19089 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/abs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21097 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/add.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18352 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/adds.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/and.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/andnot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/avg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/bitshuffle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9480 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/blend.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29208 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/broadcast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20945 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/cmp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/cmpeq.h
+-rw-r--r--   0 runner    (1001) docker     (123)    50531 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/cmpge.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/cmpgt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    50422 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/cmple.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/cmplt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17516 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/cmpneq.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21624 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/compress.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/conflict.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/copysign.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/cvt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23453 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/cvts.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/cvtt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15983 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/dbsad.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/div.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/dpbf16.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10824 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/dpbusd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13835 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/dpbusds.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/dpwssd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/dpwssds.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/expand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/extract.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28836 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/fixupimm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26373 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/fixupimm_round.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/flushsubnormal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/fmadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/fmsub.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/fnmadd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/fnmsub.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18325 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/insert.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/kshift.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/load.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/loadu.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/lzcnt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/madd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/maddubs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18597 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/max.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/min.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30273 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/mov.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/mov_mask.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15715 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/movm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/mul.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/mulhi.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/mulhrs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/mullo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/multishift.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/negate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/or.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/packs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/packus.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69997 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/permutex2var.h
+-rw-r--r--   0 runner    (1001) docker     (123)    49807 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/permutexvar.h
+-rw-r--r--   0 runner    (1001) docker     (123)    46335 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/popcnt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27800 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/range.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25064 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/range_round.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/rol.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14812 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/rolv.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14869 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/ror.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/rorv.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/round.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23118 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/roundscale.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/roundscale_round.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/sad.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/scalef.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/set.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/set1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/set4.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/setone.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/setr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/setr4.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/setzero.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/shldv.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/shuffle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/sll.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/slli.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/sllv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/sqrt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/sra.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/srai.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/srav.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/srl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/srli.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/srlv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/store.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/storeu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/sub.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/subs.h
+-rw-r--r--   0 runner    (1001) docker     (123)   112262 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/ternarylogic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/test.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/testn.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31286 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28925 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/unpackhi.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28831 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/unpacklo.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/xor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512/xorsign.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/avx512.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/clmul.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/f16c.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22155 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/fma.h
+-rw-r--r--   0 runner    (1001) docker     (123)    53191 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/gfni.h
+-rw-r--r--   0 runner    (1001) docker     (123)    76704 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/mmx.h
+-rw-r--r--   0 runner    (1001) docker     (123)   156055 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/sse.h
+-rw-r--r--   0 runner    (1001) docker     (123)   255138 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/sse2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16133 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/sse3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    79366 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/sse4.1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/sse4.2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36284 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/ssse3.h
+-rw-r--r--   0 runner    (1001) docker     (123)   398844 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/svml.h
+-rw-r--r--   0 runner    (1001) docker     (123)   118352 2023-07-28 12:54:30.000000 pyopa-0.8.4/c_source/simde/x86/xop.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-28 12:54:28.000000 pyopa-0.8.4/c_source/swps3.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:44.320959 pyopa-0.8.4/pyopa/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-28 12:54:28.000000 pyopa-0.8.4/pyopa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-28 12:54:28.000000 pyopa-0.8.4/pyopa/aligner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:44.324959 pyopa-0.8.4/pyopa/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:28.000000 pyopa-0.8.4/pyopa/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-28 12:54:28.000000 pyopa-0.8.4/pyopa/backend/cpyopa.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)  1015068 2023-07-28 12:54:43.000000 pyopa-0.8.4/pyopa/backend/pyopa.c
+-rw-r--r--   0 runner    (1001) docker     (123)    27607 2023-07-28 12:54:28.000000 pyopa-0.8.4/pyopa/backend/pyopa.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:44.324959 pyopa-0.8.4/pyopa/matrices/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:44.332959 pyopa-0.8.4/pyopa/matrices/json/
+-rw-r--r--   0 runner    (1001) docker     (123) 10824093 2023-07-28 12:54:28.000000 pyopa-0.8.4/pyopa/matrices/json/all_matrices.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-28 12:54:28.000000 pyopa-0.8.4/pyopa/matrices/json/logPAM1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-07-28 12:54:28.000000 pyopa-0.8.4/pyopa/matrices/json/logPAM1_unscaled.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-28 12:54:28.000000 pyopa-0.8.4/pyopa/matrices/jtt.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:44.320959 pyopa-0.8.4/pyopa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-28 12:54:44.000000 pyopa-0.8.4/pyopa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-28 12:54:44.000000 pyopa-0.8.4/pyopa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:54:44.000000 pyopa-0.8.4/pyopa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 12:54:44.000000 pyopa-0.8.4/pyopa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 12:54:44.000000 pyopa-0.8.4/pyopa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-28 12:54:28.000000 pyopa-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 12:54:28.000000 pyopa-0.8.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 12:54:44.336959 pyopa-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-28 12:54:28.000000 pyopa-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:54:44.336959 pyopa-0.8.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-07-28 12:54:28.000000 pyopa-0.8.4/test/test_darwin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-28 12:54:28.000000 pyopa-0.8.4/test/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-07-28 12:54:28.000000 pyopa-0.8.4/test/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-28 12:54:28.000000 pyopa-0.8.4/test/test_run_time_long_alignment.py
```

### Comparing `pyopa-0.8.2/LICENSE` & `pyopa-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/MANIFEST.in` & `pyopa-0.8.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/PKG-INFO` & `pyopa-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyopa
-Version: 0.8.2
+Version: 0.8.4
 Summary: PyOPA - optimal pairwise sequence alignments
 Home-page: http://omabrowser.org/
 Author: OMA Browser
 Author-email: contact@omabrowser.org
 License: MPL 2.0
 Keywords: sequence alignments Smith-Waterman Needleman-Wunsch dynamic programming bioinformatics
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -48,9 +47,7 @@
 
    # super fast check whether the alignment reaches a given min-score
    min_score = 100
    pam250_env = pyopa.generate_env(log_pam1_env, 250, min_score)
    pyopa.align_short(s1, s2, pam250_env)
 
    
-
-
```

### Comparing `pyopa-0.8.2/README` & `pyopa-0.8.4/README`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/README.rst` & `pyopa-0.8.4/README.rst`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/DynProgr_scalar.c` & `pyopa-0.8.4/c_source/DynProgr_scalar.c`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/DynProgr_scalar.h` & `pyopa-0.8.4/c_source/DynProgr_scalar.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/DynProgr_sse_byte.c` & `pyopa-0.8.4/c_source/DynProgr_sse_byte.c`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/DynProgr_sse_byte.h` & `pyopa-0.8.4/c_source/DynProgr_sse_byte.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/DynProgr_sse_double.c` & `pyopa-0.8.4/c_source/DynProgr_sse_double.c`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/DynProgr_sse_double.h` & `pyopa-0.8.4/c_source/DynProgr_sse_double.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/DynProgr_sse_short.c` & `pyopa-0.8.4/c_source/DynProgr_sse_short.c`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/DynProgr_sse_short.h` & `pyopa-0.8.4/c_source/DynProgr_sse_short.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/EstimatePam.c` & `pyopa-0.8.4/c_source/EstimatePam.c`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/EstimatePam.h` & `pyopa-0.8.4/c_source/EstimatePam.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/Python_extension.c` & `pyopa-0.8.4/c_source/Python_extension.c`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/Python_extension.h` & `pyopa-0.8.4/c_source/Python_extension.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/debug.h` & `pyopa-0.8.4/c_source/debug.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/matrix.h` & `pyopa-0.8.4/c_source/matrix.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/COPYING` & `pyopa-0.8.4/c_source/simde/COPYING`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/aba.h` & `pyopa-0.8.4/c_source/simde/arm/neon/aba.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/abd.h` & `pyopa-0.8.4/c_source/simde/arm/neon/abd.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/abdl.h` & `pyopa-0.8.4/c_source/simde/arm/neon/abdl.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/abs.h` & `pyopa-0.8.4/c_source/simde/arm/neon/abs.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/add.h` & `pyopa-0.8.4/c_source/simde/arm/neon/add.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/addhn.h` & `pyopa-0.8.4/c_source/simde/arm/neon/addhn.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/addl.h` & `pyopa-0.8.4/c_source/simde/arm/neon/addl.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/addl_high.h` & `pyopa-0.8.4/c_source/simde/arm/neon/addl_high.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/addlv.h` & `pyopa-0.8.4/c_source/simde/arm/neon/addlv.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/addv.h` & `pyopa-0.8.4/c_source/simde/arm/neon/addv.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/addw.h` & `pyopa-0.8.4/c_source/simde/arm/neon/addw.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/addw_high.h` & `pyopa-0.8.4/c_source/simde/arm/neon/addw_high.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/and.h` & `pyopa-0.8.4/c_source/simde/arm/neon/and.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/bcax.h` & `pyopa-0.8.4/c_source/simde/arm/neon/bcax.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/bic.h` & `pyopa-0.8.4/c_source/simde/arm/neon/bic.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/bsl.h` & `pyopa-0.8.4/c_source/simde/arm/neon/bsl.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/cage.h` & `pyopa-0.8.4/c_source/simde/arm/neon/cage.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/cagt.h` & `pyopa-0.8.4/c_source/simde/arm/neon/cagt.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/ceq.h` & `pyopa-0.8.4/c_source/simde/arm/neon/ceq.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/ceqz.h` & `pyopa-0.8.4/c_source/simde/arm/neon/ceqz.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/cge.h` & `pyopa-0.8.4/c_source/simde/arm/neon/cge.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/cgez.h` & `pyopa-0.8.4/c_source/simde/arm/neon/cgez.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/cgt.h` & `pyopa-0.8.4/c_source/simde/arm/neon/cgt.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/cgtz.h` & `pyopa-0.8.4/c_source/simde/arm/neon/cgtz.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/cle.h` & `pyopa-0.8.4/c_source/simde/arm/neon/cle.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/clez.h` & `pyopa-0.8.4/c_source/simde/arm/neon/clez.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/cls.h` & `pyopa-0.8.4/c_source/simde/arm/neon/cls.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/clt.h` & `pyopa-0.8.4/c_source/simde/arm/neon/clt.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/cltz.h` & `pyopa-0.8.4/c_source/simde/arm/neon/cltz.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/clz.h` & `pyopa-0.8.4/c_source/simde/arm/neon/clz.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/cmla.h` & `pyopa-0.8.4/c_source/simde/arm/neon/cmla.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/cmla_rot180.h` & `pyopa-0.8.4/c_source/simde/arm/neon/cmla_rot180.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/cmla_rot270.h` & `pyopa-0.8.4/c_source/simde/arm/neon/cmla_rot270.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/cmla_rot90.h` & `pyopa-0.8.4/c_source/simde/arm/neon/cmla_rot90.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/cnt.h` & `pyopa-0.8.4/c_source/simde/arm/neon/cnt.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/combine.h` & `pyopa-0.8.4/c_source/simde/arm/neon/combine.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/create.h` & `pyopa-0.8.4/c_source/simde/arm/neon/create.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/cvt.h` & `pyopa-0.8.4/c_source/simde/arm/neon/cvt.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/dot.h` & `pyopa-0.8.4/c_source/simde/arm/neon/dot.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/dot_lane.h` & `pyopa-0.8.4/c_source/simde/arm/neon/dot_lane.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/dup_lane.h` & `pyopa-0.8.4/c_source/simde/arm/neon/dup_lane.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/dup_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/dup_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/eor.h` & `pyopa-0.8.4/c_source/simde/arm/neon/eor.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/ext.h` & `pyopa-0.8.4/c_source/simde/arm/neon/ext.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/fma.h` & `pyopa-0.8.4/c_source/simde/arm/neon/fma.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/fma_lane.h` & `pyopa-0.8.4/c_source/simde/arm/neon/fma_lane.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/fma_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/fma_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/get_high.h` & `pyopa-0.8.4/c_source/simde/arm/neon/get_high.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/get_lane.h` & `pyopa-0.8.4/c_source/simde/arm/neon/get_lane.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/get_low.h` & `pyopa-0.8.4/c_source/simde/arm/neon/get_low.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/hadd.h` & `pyopa-0.8.4/c_source/simde/arm/neon/hadd.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/hsub.h` & `pyopa-0.8.4/c_source/simde/arm/neon/hsub.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/ld1.h` & `pyopa-0.8.4/c_source/simde/arm/neon/ld1.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/ld1_dup.h` & `pyopa-0.8.4/c_source/simde/arm/neon/ld1_dup.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/ld1_lane.h` & `pyopa-0.8.4/c_source/simde/arm/neon/ld1_lane.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/ld2.h` & `pyopa-0.8.4/c_source/simde/arm/neon/ld2.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/ld3.h` & `pyopa-0.8.4/c_source/simde/arm/neon/ld3.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/ld4.h` & `pyopa-0.8.4/c_source/simde/arm/neon/ld4.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/ld4_lane.h` & `pyopa-0.8.4/c_source/simde/arm/neon/ld4_lane.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/max.h` & `pyopa-0.8.4/c_source/simde/arm/neon/max.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/maxnm.h` & `pyopa-0.8.4/c_source/simde/arm/neon/maxnm.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/maxv.h` & `pyopa-0.8.4/c_source/simde/arm/neon/maxv.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/min.h` & `pyopa-0.8.4/c_source/simde/arm/neon/min.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/minnm.h` & `pyopa-0.8.4/c_source/simde/arm/neon/minnm.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/minv.h` & `pyopa-0.8.4/c_source/simde/arm/neon/minv.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mla.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mla.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mla_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mla_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mlal.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mlal.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mlal_high.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mlal_high.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mlal_high_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mlal_high_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mlal_lane.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mlal_lane.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mlal_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mlal_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mls.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mls.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mls_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mls_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mlsl.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mlsl.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mlsl_high.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mlsl_high.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mlsl_high_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mlsl_high_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mlsl_lane.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mlsl_lane.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mlsl_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mlsl_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/movl.h` & `pyopa-0.8.4/c_source/simde/arm/neon/movl.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/movl_high.h` & `pyopa-0.8.4/c_source/simde/arm/neon/movl_high.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/movn.h` & `pyopa-0.8.4/c_source/simde/arm/neon/movn.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/movn_high.h` & `pyopa-0.8.4/c_source/simde/arm/neon/movn_high.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mul.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mul.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mul_lane.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mul_lane.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mul_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mul_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mull.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mull.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mull_high.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mull_high.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mull_lane.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mull_lane.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mull_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mull_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/mvn.h` & `pyopa-0.8.4/c_source/simde/arm/neon/mvn.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/neg.h` & `pyopa-0.8.4/c_source/simde/arm/neon/neg.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/orn.h` & `pyopa-0.8.4/c_source/simde/arm/neon/orn.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/orr.h` & `pyopa-0.8.4/c_source/simde/arm/neon/orr.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/padal.h` & `pyopa-0.8.4/c_source/simde/arm/neon/padal.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/padd.h` & `pyopa-0.8.4/c_source/simde/arm/neon/padd.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/paddl.h` & `pyopa-0.8.4/c_source/simde/arm/neon/paddl.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/pmax.h` & `pyopa-0.8.4/c_source/simde/arm/neon/pmax.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/pmin.h` & `pyopa-0.8.4/c_source/simde/arm/neon/pmin.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qabs.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qabs.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qadd.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qadd.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qdmulh.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qdmulh.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qdmulh_lane.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qdmulh_lane.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qdmulh_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qdmulh_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qdmull.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qdmull.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qmovn.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qmovn.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qmovn_high.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qmovn_high.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qmovun.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qmovun.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qneg.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qneg.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qrdmulh.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qrdmulh.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qrdmulh_lane.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qrdmulh_lane.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qrdmulh_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qrdmulh_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qrshrn_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qrshrn_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qrshrun_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qrshrun_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qshl.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qshl.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qshlu_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qshlu_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qshrn_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qshrn_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qshrun_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qshrun_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qsub.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qsub.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qtbl.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qtbl.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/qtbx.h` & `pyopa-0.8.4/c_source/simde/arm/neon/qtbx.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/rbit.h` & `pyopa-0.8.4/c_source/simde/arm/neon/rbit.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/recpe.h` & `pyopa-0.8.4/c_source/simde/arm/neon/recpe.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/recps.h` & `pyopa-0.8.4/c_source/simde/arm/neon/recps.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/reinterpret.h` & `pyopa-0.8.4/c_source/simde/arm/neon/reinterpret.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/rev16.h` & `pyopa-0.8.4/c_source/simde/arm/neon/rev16.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/rev32.h` & `pyopa-0.8.4/c_source/simde/arm/neon/rev32.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/rev64.h` & `pyopa-0.8.4/c_source/simde/arm/neon/rev64.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/rhadd.h` & `pyopa-0.8.4/c_source/simde/arm/neon/rhadd.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/rnd.h` & `pyopa-0.8.4/c_source/simde/arm/neon/rnd.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/rndi.h` & `pyopa-0.8.4/c_source/simde/arm/neon/rndi.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/rndm.h` & `pyopa-0.8.4/c_source/simde/arm/neon/rndm.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/rndn.h` & `pyopa-0.8.4/c_source/simde/arm/neon/rndn.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/rndp.h` & `pyopa-0.8.4/c_source/simde/arm/neon/rndp.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/rshl.h` & `pyopa-0.8.4/c_source/simde/arm/neon/rshl.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/rshr_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/rshr_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/rshrn_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/rshrn_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/rsqrte.h` & `pyopa-0.8.4/c_source/simde/arm/neon/rsqrte.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/rsqrts.h` & `pyopa-0.8.4/c_source/simde/arm/neon/rsqrts.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/rsra_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/rsra_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/set_lane.h` & `pyopa-0.8.4/c_source/simde/arm/neon/set_lane.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/shl.h` & `pyopa-0.8.4/c_source/simde/arm/neon/shl.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/shl_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/shl_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/shll_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/shll_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/shr_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/shr_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/shrn_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/shrn_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/sqadd.h` & `pyopa-0.8.4/c_source/simde/arm/neon/sqadd.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/sra_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/sra_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/sri_n.h` & `pyopa-0.8.4/c_source/simde/arm/neon/sri_n.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/st1.h` & `pyopa-0.8.4/c_source/simde/arm/neon/st1.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/st1_lane.h` & `pyopa-0.8.4/c_source/simde/arm/neon/st1_lane.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/st2.h` & `pyopa-0.8.4/c_source/simde/arm/neon/st2.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/st2_lane.h` & `pyopa-0.8.4/c_source/simde/arm/neon/st2_lane.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/st3.h` & `pyopa-0.8.4/c_source/simde/arm/neon/st3.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/st3_lane.h` & `pyopa-0.8.4/c_source/simde/arm/neon/st3_lane.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/st4.h` & `pyopa-0.8.4/c_source/simde/arm/neon/st4.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/st4_lane.h` & `pyopa-0.8.4/c_source/simde/arm/neon/st4_lane.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/sub.h` & `pyopa-0.8.4/c_source/simde/arm/neon/sub.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/subhn.h` & `pyopa-0.8.4/c_source/simde/arm/neon/subhn.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/subl.h` & `pyopa-0.8.4/c_source/simde/arm/neon/subl.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/subl_high.h` & `pyopa-0.8.4/c_source/simde/arm/neon/subl_high.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/subw.h` & `pyopa-0.8.4/c_source/simde/arm/neon/subw.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/subw_high.h` & `pyopa-0.8.4/c_source/simde/arm/neon/subw_high.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/tbl.h` & `pyopa-0.8.4/c_source/simde/arm/neon/tbl.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/tbx.h` & `pyopa-0.8.4/c_source/simde/arm/neon/tbx.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/trn.h` & `pyopa-0.8.4/c_source/simde/arm/neon/trn.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/trn1.h` & `pyopa-0.8.4/c_source/simde/arm/neon/trn1.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/trn2.h` & `pyopa-0.8.4/c_source/simde/arm/neon/trn2.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/tst.h` & `pyopa-0.8.4/c_source/simde/arm/neon/tst.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/types.h` & `pyopa-0.8.4/c_source/simde/arm/neon/types.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/uqadd.h` & `pyopa-0.8.4/c_source/simde/arm/neon/uqadd.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/uzp.h` & `pyopa-0.8.4/c_source/simde/arm/neon/uzp.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/uzp1.h` & `pyopa-0.8.4/c_source/simde/arm/neon/uzp1.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/uzp2.h` & `pyopa-0.8.4/c_source/simde/arm/neon/uzp2.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/xar.h` & `pyopa-0.8.4/c_source/simde/arm/neon/xar.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/zip.h` & `pyopa-0.8.4/c_source/simde/arm/neon/zip.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/zip1.h` & `pyopa-0.8.4/c_source/simde/arm/neon/zip1.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon/zip2.h` & `pyopa-0.8.4/c_source/simde/arm/neon/zip2.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/neon.h` & `pyopa-0.8.4/c_source/simde/arm/neon.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/sve/add.h` & `pyopa-0.8.4/c_source/simde/arm/sve/add.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/sve/and.h` & `pyopa-0.8.4/c_source/simde/arm/sve/and.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/sve/cmplt.h` & `pyopa-0.8.4/c_source/simde/arm/sve/cmplt.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/sve/cnt.h` & `pyopa-0.8.4/c_source/simde/arm/sve/cnt.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/sve/dup.h` & `pyopa-0.8.4/c_source/simde/arm/sve/dup.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/sve/ld1.h` & `pyopa-0.8.4/c_source/simde/arm/sve/ld1.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/sve/ptest.h` & `pyopa-0.8.4/c_source/simde/arm/sve/ptest.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/sve/ptrue.h` & `pyopa-0.8.4/c_source/simde/arm/sve/ptrue.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/sve/qadd.h` & `pyopa-0.8.4/c_source/simde/arm/sve/qadd.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/sve/reinterpret.h` & `pyopa-0.8.4/c_source/simde/arm/sve/reinterpret.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/sve/sel.h` & `pyopa-0.8.4/c_source/simde/arm/sve/sel.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/sve/st1.h` & `pyopa-0.8.4/c_source/simde/arm/sve/st1.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/sve/sub.h` & `pyopa-0.8.4/c_source/simde/arm/sve/sub.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/sve/types.h` & `pyopa-0.8.4/c_source/simde/arm/sve/types.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/sve/whilelt.h` & `pyopa-0.8.4/c_source/simde/arm/sve/whilelt.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/arm/sve.h` & `pyopa-0.8.4/c_source/simde/arm/sve.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/check.h` & `pyopa-0.8.4/c_source/simde/check.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/debug-trap.h` & `pyopa-0.8.4/c_source/simde/debug-trap.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/hedley.h` & `pyopa-0.8.4/c_source/simde/hedley.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/mips/msa/add_a.h` & `pyopa-0.8.4/c_source/simde/mips/msa/add_a.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/mips/msa/adds.h` & `pyopa-0.8.4/c_source/simde/mips/msa/adds.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/mips/msa/adds_a.h` & `pyopa-0.8.4/c_source/simde/mips/msa/adds_a.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/mips/msa/addv.h` & `pyopa-0.8.4/c_source/simde/mips/msa/addv.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/mips/msa/addvi.h` & `pyopa-0.8.4/c_source/simde/mips/msa/addvi.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/mips/msa/and.h` & `pyopa-0.8.4/c_source/simde/mips/msa/and.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/mips/msa/andi.h` & `pyopa-0.8.4/c_source/simde/mips/msa/andi.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/mips/msa/ld.h` & `pyopa-0.8.4/c_source/simde/mips/msa/ld.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/mips/msa/madd.h` & `pyopa-0.8.4/c_source/simde/mips/msa/madd.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/mips/msa/st.h` & `pyopa-0.8.4/c_source/simde/mips/msa/st.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/mips/msa/subv.h` & `pyopa-0.8.4/c_source/simde/mips/msa/subv.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/mips/msa/types.h` & `pyopa-0.8.4/c_source/simde/mips/msa/types.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/mips/msa.h` & `pyopa-0.8.4/c_source/simde/mips/msa.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/simde-align.h` & `pyopa-0.8.4/c_source/simde/simde-align.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/simde-arch.h` & `pyopa-0.8.4/c_source/simde/simde-arch.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/simde-common.h` & `pyopa-0.8.4/c_source/simde/simde-common.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/simde-complex.h` & `pyopa-0.8.4/c_source/simde/simde-complex.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/simde-constify.h` & `pyopa-0.8.4/c_source/simde/simde-constify.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/simde-detect-clang.h` & `pyopa-0.8.4/c_source/simde/simde-detect-clang.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/simde-diagnostic.h` & `pyopa-0.8.4/c_source/simde/simde-diagnostic.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/simde-f16.h` & `pyopa-0.8.4/c_source/simde/simde-f16.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/simde-features.h` & `pyopa-0.8.4/c_source/simde/simde-features.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/simde-math.h` & `pyopa-0.8.4/c_source/simde/simde-math.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/wasm/relaxed-simd.h` & `pyopa-0.8.4/c_source/simde/wasm/relaxed-simd.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/wasm/simd128.h` & `pyopa-0.8.4/c_source/simde/wasm/simd128.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx.h` & `pyopa-0.8.4/c_source/simde/x86/avx.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx2.h` & `pyopa-0.8.4/c_source/simde/x86/avx2.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/2intersect.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/2intersect.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/4dpwssd.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/4dpwssd.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/4dpwssds.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/4dpwssds.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/abs.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/abs.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/add.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/add.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/adds.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/adds.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/and.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/and.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/andnot.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/andnot.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/avg.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/avg.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/bitshuffle.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/bitshuffle.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/blend.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/blend.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/broadcast.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/broadcast.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/cast.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/cast.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/cmp.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/cmp.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/cmpeq.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/cmpeq.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/cmpge.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/cmpge.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/cmpgt.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/cmpgt.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/cmple.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/cmple.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/cmplt.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/cmplt.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/cmpneq.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/cmpneq.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/compress.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/compress.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/conflict.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/conflict.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/copysign.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/copysign.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/cvt.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/cvt.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/cvts.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/cvts.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/cvtt.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/cvtt.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/dbsad.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/dbsad.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/div.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/div.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/dpbf16.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/dpbf16.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/dpbusd.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/dpbusd.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/dpbusds.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/dpbusds.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/dpwssd.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/dpwssd.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/dpwssds.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/dpwssds.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/expand.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/expand.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/extract.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/extract.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/fixupimm.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/fixupimm.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/fixupimm_round.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/fixupimm_round.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/flushsubnormal.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/flushsubnormal.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/fmadd.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/fmadd.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/fmsub.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/fmsub.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/fnmadd.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/fnmadd.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/fnmsub.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/fnmsub.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/insert.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/insert.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/kshift.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/kshift.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/load.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/load.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/loadu.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/loadu.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/lzcnt.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/lzcnt.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/madd.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/madd.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/maddubs.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/maddubs.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/max.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/max.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/min.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/min.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/mov.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/mov.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/mov_mask.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/mov_mask.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/movm.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/movm.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/mul.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/mul.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/mulhi.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/mulhi.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/mulhrs.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/mulhrs.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/mullo.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/mullo.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/multishift.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/multishift.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/negate.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/negate.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/or.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/or.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/packs.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/packs.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/packus.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/packus.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/permutex2var.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/permutex2var.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/permutexvar.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/permutexvar.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/popcnt.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/popcnt.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/range.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/range.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/range_round.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/range_round.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/rol.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/rol.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/rolv.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/rolv.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/ror.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/ror.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/rorv.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/rorv.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/round.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/round.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/roundscale.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/roundscale.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/roundscale_round.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/roundscale_round.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/sad.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/sad.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/scalef.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/scalef.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/set.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/set.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/set1.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/set1.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/set4.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/set4.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/setone.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/setone.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/setr.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/setr.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/setr4.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/setr4.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/setzero.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/setzero.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/shldv.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/shldv.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/shuffle.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/shuffle.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/sll.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/sll.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/slli.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/slli.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/sllv.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/sllv.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/sqrt.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/sqrt.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/sra.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/sra.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/srai.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/srai.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/srav.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/srav.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/srl.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/srl.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/srli.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/srli.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/srlv.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/srlv.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/store.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/store.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/storeu.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/storeu.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/sub.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/sub.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/subs.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/subs.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/ternarylogic.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/ternarylogic.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/test.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/test.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/testn.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/testn.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/types.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/types.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/unpackhi.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/unpackhi.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/unpacklo.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/unpacklo.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/xor.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/xor.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512/xorsign.h` & `pyopa-0.8.4/c_source/simde/x86/avx512/xorsign.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/avx512.h` & `pyopa-0.8.4/c_source/simde/x86/avx512.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/clmul.h` & `pyopa-0.8.4/c_source/simde/x86/clmul.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/f16c.h` & `pyopa-0.8.4/c_source/simde/x86/f16c.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/fma.h` & `pyopa-0.8.4/c_source/simde/x86/fma.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/gfni.h` & `pyopa-0.8.4/c_source/simde/x86/gfni.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/mmx.h` & `pyopa-0.8.4/c_source/simde/x86/mmx.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/sse.h` & `pyopa-0.8.4/c_source/simde/x86/sse.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/sse2.h` & `pyopa-0.8.4/c_source/simde/x86/sse2.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/sse3.h` & `pyopa-0.8.4/c_source/simde/x86/sse3.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/sse4.1.h` & `pyopa-0.8.4/c_source/simde/x86/sse4.1.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/sse4.2.h` & `pyopa-0.8.4/c_source/simde/x86/sse4.2.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/ssse3.h` & `pyopa-0.8.4/c_source/simde/x86/ssse3.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/svml.h` & `pyopa-0.8.4/c_source/simde/x86/svml.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/simde/x86/xop.h` & `pyopa-0.8.4/c_source/simde/x86/xop.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/c_source/swps3.h` & `pyopa-0.8.4/c_source/swps3.h`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/pyopa/aligner.py` & `pyopa-0.8.4/pyopa/aligner.py`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/pyopa/backend/cpyopa.pxd` & `pyopa-0.8.4/pyopa/backend/cpyopa.pxd`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/pyopa/backend/pyopa.c` & `pyopa-0.8.4/pyopa/backend/pyopa.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-/* Generated by Cython 0.29.28 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "c_source/DynProgr_sse_double.h",
             "c_source/EstimatePam.h",
             "c_source/Python_extension.h"
         ],
         "extra_compile_args": [
             "-O2",
             "-DSIMDE_ENABLE_NATIVE_ALIASES"
         ],
         "include_dirs": [
             "c_source/",
-            "/tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/core/include",
+            "/tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/core/include",
             "."
         ],
         "name": "pyopa.backend.pyopa",
         "sources": [
             "pyopa/backend/pyopa.pyx",
             "c_source/Python_extension.c",
             "c_source/DynProgr_sse_short.c",
@@ -43,16 +43,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_28"
-#define CYTHON_HEX_VERSION 0x001D1CF0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -83,14 +83,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -111,26 +112,34 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -160,18 +169,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -183,15 +241,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -213,31 +271,34 @@
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 0
   #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -342,17 +403,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -422,14 +480,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -529,35 +592,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -681,16 +744,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -1002,195 +1067,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":693
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":700
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":705
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":716
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":719
- * 
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1220,42 +1267,42 @@
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj_5pyopa_7backend_5pyopa_AlignmentProfile;
 struct __pyx_obj_5pyopa_7backend_5pyopa_MutipleAlEnv;
 struct __pyx_obj_5pyopa_7backend_5pyopa___pyx_scope_struct__create_scaled_matrices;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":733
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1461,26 +1508,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1504,14 +1551,20 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif // CYTHON_FAST_PYCALL
 #endif
@@ -1829,14 +1882,31 @@
 /* ObjectGetItem.proto */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject* key);
 #else
 #define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
 #endif
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* py_abs.proto */
 #if CYTHON_USE_PYLONG_INTERNALS
 static PyObject *__Pyx_PyLong_AbsNeg(PyObject *num);
 #define __Pyx_PyNumber_Absolute(x)\
     ((likely(PyLong_CheckExact(x))) ?\
          (likely(Py_SIZE(x) >= 0) ? (Py_INCREF(x), (x)) : __Pyx_PyLong_AbsNeg(x)) :\
          PyNumber_Absolute(x))
@@ -1965,22 +2035,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -7828,15 +7906,15 @@
  * 
  *                 reversed = profile1r.align_double(s2r, env, stop_at_threshold)
  *                 assert( abs(res[0]-reversed[0]) <= abs(res[0])*1e-10 )             # <<<<<<<<<<<<<<
  * 
  *                 res.extend([res[1] - reversed[1], res[2] - reversed[2]])
  */
       #ifndef CYTHON_WITHOUT_ASSERTIONS
-      if (unlikely(!Py_OptimizeFlag)) {
+      if (unlikely(__pyx_assertions_enabled())) {
         __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_res, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 356, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_t_8 = __Pyx_GetItemInt(__pyx_v_reversed, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 356, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __pyx_t_5 = PyNumber_Subtract(__pyx_t_2, __pyx_t_8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 356, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -15185,15 +15263,15 @@
   __Pyx_AddTraceback("pyopa.backend.pyopa.MutipleAlEnv.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":735
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -15202,29 +15280,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -15235,15 +15313,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":738
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -15252,29 +15330,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -15285,15 +15363,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":741
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -15302,29 +15380,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -15335,15 +15413,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":744
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -15352,29 +15430,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -15385,15 +15463,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":747
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -15402,29 +15480,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -15435,212 +15513,220 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":750
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 927, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":933
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":936
+    /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":941
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -15656,15 +15742,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -15672,84 +15758,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":943
+      /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 943, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 939, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 944, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 945, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 945, __pyx_L5_except_error)
+      __PYX_ERR(2, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":942
+    /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -15764,15 +15850,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":947
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -15788,15 +15874,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -15804,84 +15890,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":949
+      /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 949, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 945, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 950, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 951, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 951, __pyx_L5_except_error)
+      __PYX_ERR(2, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":948
+    /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -15896,15 +15982,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":953
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -15920,15 +16006,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":954
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -15936,84 +16022,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":955
+      /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 955, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 951, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 956, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 957, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 957, __pyx_L5_except_error)
+      __PYX_ERR(2, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":954
+    /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -16028,176 +16114,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":967
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":967
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":982
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":982
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":997
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":997
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":1007
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":1014
+/* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -16223,15 +16309,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_5pyopa_7backend_5pyopa_AlignmentProfile(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -16318,15 +16404,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_5pyopa_7backend_5pyopa_MutipleAlEnv(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_5pyopa_7backend_5pyopa_MutipleAlEnv *p;
   PyObject *o;
@@ -16344,15 +16430,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_5pyopa_7backend_5pyopa_MutipleAlEnv(PyObject *o) {
   struct __pyx_obj_5pyopa_7backend_5pyopa_MutipleAlEnv *p = (struct __pyx_obj_5pyopa_7backend_5pyopa_MutipleAlEnv *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -16455,15 +16541,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5pyopa_7backend_5pyopa___pyx_scope_struct__create_scaled_matrices *__pyx_freelist_5pyopa_7backend_5pyopa___pyx_scope_struct__create_scaled_matrices[8];
 static int __pyx_freecount_5pyopa_7backend_5pyopa___pyx_scope_struct__create_scaled_matrices = 0;
 
@@ -16573,15 +16659,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"c_align_scalar_normalized_reference_local", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5pyopa_7backend_5pyopa_23c_align_scalar_normalized_reference_local, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5pyopa_7backend_5pyopa_22c_align_scalar_normalized_reference_local},
   {"c_align_double_normalized_global", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5pyopa_7backend_5pyopa_25c_align_double_normalized_global, METH_VARARGS|METH_KEYWORDS, __pyx_doc_5pyopa_7backend_5pyopa_24c_align_double_normalized_global},
@@ -16849,15 +16935,15 @@
   __pyx_builtin_xrange = __Pyx_GetBuiltinName(__pyx_n_s_xrange); if (!__pyx_builtin_xrange) __PYX_ERR(0, 150, __pyx_L1_error)
   #endif
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 151, __pyx_L1_error)
   __pyx_builtin_open = __Pyx_GetBuiltinName(__pyx_n_s_open); if (!__pyx_builtin_open) __PYX_ERR(0, 171, __pyx_L1_error)
   __pyx_builtin_map = __Pyx_GetBuiltinName(__pyx_n_s_map); if (!__pyx_builtin_map) __PYX_ERR(0, 428, __pyx_L1_error)
   __pyx_builtin_NotImplemented = __Pyx_GetBuiltinName(__pyx_n_s_NotImplemented); if (!__pyx_builtin_NotImplemented) __PYX_ERR(0, 443, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 945, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 941, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -16974,33 +17060,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 945, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 951, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 947, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
   /* "pyopa/backend/pyopa.pyx":16
  * 
  * 
  * def matrix_dir():             # <<<<<<<<<<<<<<
@@ -17294,15 +17380,20 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_0_0 = PyFloat_FromDouble(0.0); if (unlikely(!__pyx_float_0_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_85_0 = PyFloat_FromDouble(85.0); if (unlikely(!__pyx_float_85_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_1eneg_10 = PyFloat_FromDouble(1e-10); if (unlikely(!__pyx_float_1eneg_10)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_255_0 = PyFloat_FromDouble(255.0); if (unlikely(!__pyx_float_255_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_7_434 = PyFloat_FromDouble(7.434); if (unlikely(!__pyx_float_7_434)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_65535_0 = PyFloat_FromDouble(65535.0); if (unlikely(!__pyx_float_65535_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_0_049449734348559203348 = PyFloat_FromDouble(0.049449734348559203348); if (unlikely(!__pyx_float_0_049449734348559203348)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -17410,55 +17501,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 200, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 223, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 227, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 789, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -17643,15 +17718,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_pyopa__backend__pyopa) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -18157,15 +18232,15 @@
  * import math
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../../tmp/build-env-d1qx5a6a/lib/python3.8/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-r60l06ip/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -18709,28 +18784,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -18739,15 +18814,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -18773,15 +18848,15 @@
         ps2 = PyBytes_AS_STRING(s2);
         if (ps1[0] != ps2[0]) {
             return (equals == Py_NE);
         } else if (length == 1) {
             return (equals == Py_EQ);
         } else {
             int result;
-#if CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
             Py_hash_t hash1, hash2;
             hash1 = ((PyBytesObject*)s1)->ob_shash;
             hash2 = ((PyBytesObject*)s2)->ob_shash;
             if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
                 return (equals == Py_NE);
             }
 #endif
@@ -19991,17 +20066,15 @@
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
     if (nogil)
         state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
-#endif
+    else state = (PyGILState_STATE)0;
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
     if (full_traceback) {
         Py_XINCREF(old_exc);
         Py_XINCREF(old_val);
         Py_XINCREF(old_tb);
@@ -20280,15 +20353,15 @@
                  Py_TYPE(obj)->tp_name, type->tp_name);
     return 0;
 }
 
 /* ObjectGetItem */
   #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -20984,14 +21057,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -21058,15 +21139,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -21448,25 +21532,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
 #endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -21503,71 +21605,91 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-      #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+      #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -21760,15 +21882,15 @@
     }
     Py_XDECREF(owned_metaclass);
     return result;
 }
 
 /* CLineInTraceback */
       #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -21884,14 +22006,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
       #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -21947,22 +22075,32 @@
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -22142,15 +22280,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -22296,15 +22434,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -22381,15 +22519,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -22615,15 +22753,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -22929,19 +23067,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
       static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
```

### Comparing `pyopa-0.8.2/pyopa/backend/pyopa.pyx` & `pyopa-0.8.4/pyopa/backend/pyopa.pyx`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/pyopa/matrices/json/all_matrices.json` & `pyopa-0.8.4/pyopa/matrices/json/all_matrices.json`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/pyopa/matrices/json/logPAM1.json` & `pyopa-0.8.4/pyopa/matrices/json/logPAM1.json`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/pyopa/matrices/json/logPAM1_unscaled.json` & `pyopa-0.8.4/pyopa/matrices/json/logPAM1_unscaled.json`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/pyopa/matrices/jtt.dat` & `pyopa-0.8.4/pyopa/matrices/jtt.dat`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/pyopa.egg-info/PKG-INFO` & `pyopa-0.8.4/pyopa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyopa
-Version: 0.8.2
+Version: 0.8.4
 Summary: PyOPA - optimal pairwise sequence alignments
 Home-page: http://omabrowser.org/
 Author: OMA Browser
 Author-email: contact@omabrowser.org
 License: MPL 2.0
 Keywords: sequence alignments Smith-Waterman Needleman-Wunsch dynamic programming bioinformatics
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -48,9 +47,7 @@
 
    # super fast check whether the alignment reaches a given min-score
    min_score = 100
    pam250_env = pyopa.generate_env(log_pam1_env, 250, min_score)
    pyopa.align_short(s1, s2, pam250_env)
 
    
-
-
```

### Comparing `pyopa-0.8.2/pyopa.egg-info/SOURCES.txt` & `pyopa-0.8.4/pyopa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/setup.py` & `pyopa-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/test/test_darwin.py` & `pyopa-0.8.4/test/test_darwin.py`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/test/test_env.py` & `pyopa-0.8.4/test/test_env.py`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/test/test_input.py` & `pyopa-0.8.4/test/test_input.py`

 * *Files identical despite different names*

### Comparing `pyopa-0.8.2/test/test_run_time_long_alignment.py` & `pyopa-0.8.4/test/test_run_time_long_alignment.py`

 * *Files identical despite different names*


# Comparing `tmp/uncertainty-datatypes-1.0.9.tar.gz` & `tmp/uncertainty-datatypes-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uncertainty-datatypes-1.0.9.tar", last modified: Wed Jul 19 10:09:00 2023, max compression
+gzip compressed data, was "uncertainty-datatypes-1.1.0.tar", last modified: Fri Jul 28 14:58:41 2023, max compression
```

## Comparing `uncertainty-datatypes-1.0.9.tar` & `uncertainty-datatypes-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,34 @@
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 10:09:00.091582 uncertainty-datatypes-1.0.9/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     1099 2023-07-17 07:54:55.000000 uncertainty-datatypes-1.0.9/LICENSE
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10844 2023-07-19 10:09:00.091429 uncertainty-datatypes-1.0.9/PKG-INFO
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10073 2023-07-19 10:06:41.000000 uncertainty-datatypes-1.0.9/README.md
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      854 2023-07-19 10:08:53.000000 uncertainty-datatypes-1.0.9/pyproject.toml
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       38 2023-07-19 10:09:00.091617 uncertainty-datatypes-1.0.9/setup.cfg
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 10:09:00.090049 uncertainty-datatypes-1.0.9/test/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4429 2023-07-19 09:42:56.000000 uncertainty-datatypes-1.0.9/test/test_ubool.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    19029 2023-07-19 09:43:27.000000 uncertainty-datatypes-1.0.9/test/test_ufloat.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      717 2023-07-19 09:43:54.000000 uncertainty-datatypes-1.0.9/test/test_ufuncs.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    17973 2023-07-19 09:43:23.000000 uncertainty-datatypes-1.0.9/test/test_uint.py
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 10:09:00.090669 uncertainty-datatypes-1.0.9/uncertainty/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-14 08:59:58.000000 uncertainty-datatypes-1.0.9/uncertainty/__init__.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      328 2023-07-17 11:29:42.000000 uncertainty-datatypes-1.0.9/uncertainty/result.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4311 2023-07-19 09:11:10.000000 uncertainty-datatypes-1.0.9/uncertainty/ubool.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    20722 2023-07-19 09:45:39.000000 uncertainty-datatypes-1.0.9/uncertainty/unumbers.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4306 2023-07-19 09:44:37.000000 uncertainty-datatypes-1.0.9/uncertainty/utypes.py
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 10:09:00.091268 uncertainty-datatypes-1.0.9/uncertainty_datatypes.egg-info/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10844 2023-07-19 10:09:00.000000 uncertainty-datatypes-1.0.9/uncertainty_datatypes.egg-info/PKG-INFO
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      446 2023-07-19 10:09:00.000000 uncertainty-datatypes-1.0.9/uncertainty_datatypes.egg-info/SOURCES.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        1 2023-07-19 10:09:00.000000 uncertainty-datatypes-1.0.9/uncertainty_datatypes.egg-info/dependency_links.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       14 2023-07-19 10:09:00.000000 uncertainty-datatypes-1.0.9/uncertainty_datatypes.egg-info/requires.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       12 2023-07-19 10:09:00.000000 uncertainty-datatypes-1.0.9/uncertainty_datatypes.egg-info/top_level.txt
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-28 14:58:41.738185 uncertainty-datatypes-1.1.0/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     1099 2023-07-17 07:54:55.000000 uncertainty-datatypes-1.1.0/LICENSE
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    16615 2023-07-28 14:58:41.738000 uncertainty-datatypes-1.1.0/PKG-INFO
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    15844 2023-07-28 14:49:01.000000 uncertainty-datatypes-1.1.0/README.md
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      854 2023-07-28 14:58:25.000000 uncertainty-datatypes-1.1.0/pyproject.toml
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       38 2023-07-28 14:58:41.738232 uncertainty-datatypes-1.1.0/setup.cfg
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-28 14:58:41.735166 uncertainty-datatypes-1.1.0/test/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     2497 2023-07-28 14:49:01.000000 uncertainty-datatypes-1.1.0/test/test_abool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10985 2023-07-28 14:49:01.000000 uncertainty-datatypes-1.1.0/test/test_afloat.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10830 2023-07-28 14:49:01.000000 uncertainty-datatypes-1.1.0/test/test_aint.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    15958 2023-07-28 14:49:01.000000 uncertainty-datatypes-1.1.0/test/test_sbool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     3246 2023-07-28 14:49:01.000000 uncertainty-datatypes-1.1.0/test/test_ubool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     1230 2023-07-20 12:01:17.000000 uncertainty-datatypes-1.1.0/test/test_uenum.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    16842 2023-07-20 12:01:17.000000 uncertainty-datatypes-1.1.0/test/test_ufloat.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    15829 2023-07-20 12:01:17.000000 uncertainty-datatypes-1.1.0/test/test_uint.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     7473 2023-07-28 14:49:01.000000 uncertainty-datatypes-1.1.0/test/test_ustr.py
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-28 14:58:41.736917 uncertainty-datatypes-1.1.0/uncertainty/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-14 08:59:58.000000 uncertainty-datatypes-1.1.0/uncertainty/__init__.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     5830 2023-07-28 14:49:01.000000 uncertainty-datatypes-1.1.0/uncertainty/abool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     3243 2023-07-28 14:49:01.000000 uncertainty-datatypes-1.1.0/uncertainty/afuncs.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    21656 2023-07-28 14:49:01.000000 uncertainty-datatypes-1.1.0/uncertainty/anumbers.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      328 2023-07-17 11:29:42.000000 uncertainty-datatypes-1.1.0/uncertainty/result.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    55475 2023-07-28 14:49:01.000000 uncertainty-datatypes-1.1.0/uncertainty/sbool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     5147 2023-07-28 14:49:01.000000 uncertainty-datatypes-1.1.0/uncertainty/ubool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     2367 2023-07-24 12:10:15.000000 uncertainty-datatypes-1.1.0/uncertainty/uenum.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    21643 2023-07-27 19:47:26.000000 uncertainty-datatypes-1.1.0/uncertainty/unumbers.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     7917 2023-07-28 14:49:01.000000 uncertainty-datatypes-1.1.0/uncertainty/ustr.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     6104 2023-07-28 14:49:01.000000 uncertainty-datatypes-1.1.0/uncertainty/utypes.py
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-28 14:58:41.737763 uncertainty-datatypes-1.1.0/uncertainty_datatypes.egg-info/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    16615 2023-07-28 14:58:41.000000 uncertainty-datatypes-1.1.0/uncertainty_datatypes.egg-info/PKG-INFO
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      668 2023-07-28 14:58:41.000000 uncertainty-datatypes-1.1.0/uncertainty_datatypes.egg-info/SOURCES.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        1 2023-07-28 14:58:41.000000 uncertainty-datatypes-1.1.0/uncertainty_datatypes.egg-info/dependency_links.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       14 2023-07-28 14:58:41.000000 uncertainty-datatypes-1.1.0/uncertainty_datatypes.egg-info/requires.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       12 2023-07-28 14:58:41.000000 uncertainty-datatypes-1.1.0/uncertainty_datatypes.egg-info/top_level.txt
```

### Comparing `uncertainty-datatypes-1.0.9/LICENSE` & `uncertainty-datatypes-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.9/pyproject.toml` & `uncertainty-datatypes-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uncertainty-datatypes"
-version = "1.0.9"
+version = "1.1.0"
 authors = [
   { name="Atenea Research Group, University of Malaga, Spain" },
 ]
 description = "Uncertainty Datatypes Library"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers=[
```

### Comparing `uncertainty-datatypes-1.0.9/test/test_ufloat.py` & `uncertainty-datatypes-1.1.0/test/test_ufloat.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,111 +2,14 @@
 sys.path.append(os.path.dirname(os.path.realpath(__file__)) + "/../")
 
 import unittest
 
 from uncertainty.utypes import *
 from funcs_testing import *
 
-def execute(l, r, e, func, method, op, rev_op):
-    t(func(l, r), e)            #   add(l, r)
-    if isinstance(l, ufloat): 
-        t(method(l, r), e)      #   l.add(r)
-        t(op(l, r),     e)      #   l + r
-    elif isinstance(r, ufloat): 
-        t(rev_op(r, l), e)      #   5 + r
-
-def negs(l, e):
-    t(neg(l),  e)
-    t(l.neg(), e)
-    t(-l,      e)
-
-def adds(l, r, e):
-    execute(l, r, e, add, ufloat.add, ufloat.__add__,  ufloat.__radd__)
-
-def subs(l, r, e):
-    execute(l, r, e, sub, ufloat.sub, ufloat.__sub__,  ufloat.__rsub__)
-
-def muls(l, r, e):
-    execute(l, r, e, mul, ufloat.mul, ufloat.__mul__,  ufloat.__rmul__)
-
-def divs(l, r, e):
-    execute(l, r, e, div, ufloat.div, ufloat.__truediv__,  ufloat.__rtruediv__)
-
-def floordivs(l, r, e):
-    execute(l, r, e, floordiv, ufloat.floordiv, ufloat.__floordiv__,  ufloat.__rfloordiv__)
-
-def pows(l, r, e):
-    execute(l, r, e, pow, ufloat.power, ufloat.__pow__,  ufloat.__pow__)
-
-def func_execute(l, e, func, method):
-    t(func(l), e)    #   sqrt(l)
-    t(method(l), e)  #   sqrt(l)
-
-def abss(l, e):
-    func_execute(l, e, abs, ufloat.abs)
-
-def sqrts(l, e):
-    func_execute(l, e, sqrt, ufloat.sqrt)
-
-def sins(l, e):
-    func_execute(l, e, sin, ufloat.sin)
-
-def coss(l, e):
-    func_execute(l, e, coss, ufloat.coss)
-
-def sins(l, e):
-    func_execute(l, e, sin, ufloat.sin)
-    
-def coss(l, e):
-    func_execute(l, e, cos, ufloat.cos)
-
-def tans(l, e):
-    func_execute(l, e, tan, ufloat.tan)
-    
-def atans(l, e):
-    func_execute(l, e, atan, ufloat.atan)
-
-def asins(l, e):
-    func_execute(l, e, asin, ufloat.asin)
-    
-def acoss(l, e):
-    func_execute(l, e, acos, ufloat.acos)
-
-def inverses(l, e):
-    func_execute(l, e, inverse, ufloat.inverse)
-
-def floors(l, e):
-    func_execute(l, e, floor, ufloat.floor)
-
-def rounds(l, e):
-    func_execute(l, e, round, ufloat.round)
-
-def comparison_execute(l, r, e, func, method, op):
-    t(func(l, r),   e)  #   lt(l, r)
-    t(method(l, r), e)  #   l.lt(r)
-    t(op(l, r),     e)  #   l < r
-
-def eqs(l, r, e):
-    comparison_execute(l, r, e, eq, ufloat.eq,  ufloat.__eq__)
-
-def nes(l, r, e):
-    comparison_execute(l, r, e, ne, ufloat.ne,  ufloat.__ne__)
-
-def lts(l, r, e):
-    comparison_execute(l, r, e, lt, ufloat.lt,  ufloat.__lt__)
-    
-def les(l, r, e):
-    comparison_execute(l, r, e, le, ufloat.le,  ufloat.__le__)
-    
-def gts(l, r, e):
-    comparison_execute(l, r, e, gt, ufloat.gt,  ufloat.__gt__)
-    
-def ges(l, r, e):
-    comparison_execute(l, r, e, ge, ufloat.ge,  ufloat.__ge__)
-
 class ufloatTest(unittest.TestCase):
     
     def setUp(self):
         self.ufa = ufloat(-4.0, 3.0)
         self.ufb = ufloat(2.0, 4.0)
         self.ufc = ufloat(23.0, 5.3)
         self.uia = uint(-4, 3.0)
@@ -438,22 +341,25 @@
 
     def test_max(self):
         ''' max '''
         t(max(self.ufa, self.ufb, self.ufc), self.ufc)
         t(max(abs(self.ufa), abs(self.ufb), abs(self.ufc)), self.ufc)
         t(max(ufloat(2.2, 12), ufloat(1.3, 12), ufloat(3.7, 12), ufloat(5.3, 12), ufloat(3.1, 12), ufloat(2.6, 12), ufloat(0.6, 12), ufloat(4.4, 12)), ufloat(5.3, 12))
         t(max(ufloat(2.2, 12), ufloat(-1.3, 12), ufloat(3.7, 12), ufloat(5.3, 12), ufloat(-3.1, 12), ufloat(2.6, 12), ufloat(-0.6, 12), ufloat(4.4, 12)), ufloat(5.3, 12))
+        t(max(2, ufloat(-1, 12), 3, ufloat(5, 12), -3, ufloat(2, 12), ufloat(-0, 12), 6), 6)
+        t(max(2, uint(-1, 1), ufloat(-3.5, 1.0), uint(3, 1), -2, uint(0, 1), -4, ufloat(5.5, 1.7)), ufloat(5.5, 1.7))
 
     def test_min(self):
         ''' min '''
         t(min(self.ufa, self.ufb, self.ufc), self.ufa)
         t(min(abs(self.ufa), abs(self.ufb), abs(self.ufc)), self.ufb)
         t(min(ufloat(2.2, 1), ufloat(1.3, 1), ufloat(3.7, 1), ufloat(3.3, 1), ufloat(2.1, 1), ufloat(0.6, 1), ufloat(4.6, 1), ufloat(5.4, 1)), ufloat(0.6, 1))
         t(min(ufloat(2.2, 1), ufloat(-1.3, 1), ufloat(3.7, 1), ufloat(3.3, 1), ufloat(-2.1, 1), ufloat(0.6, 1), ufloat(-4.6, 1), ufloat(5.4, 1)), ufloat(-4.6, 1))
-
+        t(min(2, ufloat(-1, 1), -3, ufloat(3, 1), -2, ufloat(0, 1), -4, -5), -5)
+        t(min(2, uint(-1, 1), ufloat(-3.5, 1.0), uint(3, 1), -2, uint(0, 1), -4, ufloat(-5.5, 1.7)), ufloat(-5.5, 1.7))
     '''
         Comparison Operators
     '''
     def test_eq(self):
         ''' eq == '''
         eqs(self.ufa, self.ufa, ubool(1.000))
         eqs(self.ufa, self.ufb, ubool(0.385))
```

### Comparing `uncertainty-datatypes-1.0.9/uncertainty/ubool.py` & `uncertainty-datatypes-1.1.0/uncertainty/ubool.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,145 +15,172 @@
             elif 'False' == c.capitalize():
                 c = False
 
         if isinstance(c, (int, float, str)):
             c = float(c)
             if c < 0.0 or c > 1.0: 
                 raise ValueError('Invalid parameter: c < 0.0 or c > 1.0. c=' + c)
-            self.c = float(c)
+            self._c = float(c)
         elif isinstance(c, bool):
-            self.c = 1.0 if c else 0.0
+            self._c = 1.0 if c else 0.0
         elif isinstance(c, ubool):
-            self.c = c.c
+            self._c = c.c
         else:
             raise ValueError('Invalid parameter c: not bool, ubool, str or number[0.0, 1.0]. C=' + c)
-
+    
+    def getCertainty():
+        return ubool.CERTAINTY
+    
     def setCertainty(certainty: float|int):
         if not isinstance(certainty, (int, float)):
             raise ValueError('Invalid parameter: certainty is not an integer or float [0.0, 1.0].')
-        
         if certainty < 0.0 or certainty > 1.0:
             raise ValueError('Invalid parameter: certainty is an integer and c < 0 or c > 1. C=')
         
         ubool.CERTAINTY = float(certainty)
 
-    def certainty() -> float:
-        return ubool.CERTAINTY
-
+    @property
+    def confidence(self):
+        return self._c
+
+    @property
+    def uncertainty(self):
+        return self._c
+
+    @confidence.setter
+    def confidence(self, c: int|float|str):
+        if not isinstance(c, (int, float, str)):
+            raise ValueError('Invalid parameter c: not a number[0.0, 1.0]. c=' + c)
+        self._c = float(c)
+    
     ''' Type Operations '''
     ''' Not (c) = (1-c)'''
     def NOT(self) -> ubool:
-        return ubool(1 - self.c)
+        return ubool(1 - self._c)
     
     def __invert__(self) -> ubool:
         return self.NOT()
-    
-    def __neg__(self) -> ubool:
-        return self.NOT()
            
-    def AND(self, o) -> ubool:
+    def AND(self, o: ubool) -> ubool:
         if (id(self) == id(o)):
-            return ubool(self.c) # x and x
+            return ubool(self._c) # x and x
         
         if not isinstance(o, ubool):
             o = ubool(o)
 
-        return ubool(self.c * o.c)
+        return ubool(self._c * o._c)
 
     def __and__(self, other) -> ubool:
         return self.AND(other)
     
     def __rand__(self, left) -> ubool:
         return ubool(left).AND(self)
 
     def OR(self, o: ubool|bool|int|float) -> ubool:
         if (id(self) == id(o)):
-            return ubool(self.c) # x or x
+            return ubool(self._c) # x or x
         
         if not isinstance(o, ubool):
             o = ubool(o)
 
-        return ubool(self.c + o.c - (self.c * o.c))
+        return ubool(self._c + o._c - (self._c * o._c))
 
     def __or__(self, other) -> ubool:
         if callable(other):
             return NotImplemented
         return self.OR(other)
 
     def __ror__(self, left) -> ubool:
         return ubool(left).OR(self)
     
-    def IMPLIES(self, o) -> ubool:
+    def IMPLIES(self, o: ubool) -> ubool:
         if (id(self) == id(o)):
-            return ubool(self.c) # x implies x
+            return ubool(self._c) # x implies x
+        
+        if not isinstance(o, ubool):
+            o = ubool(o)
 
-        return ubool((1-self.c) + o.c - ((1 - self.c) * o.c))
+        return ubool((1-self._c) + o._c - ((1 - self._c) * o._c))
     
     def __rshift__(self, other) -> ubool:
         return self.IMPLIES(other)
 
     def __rrshift__(self, left) -> ubool:
         return ubool(left).IMPLIES(self)
 
-    def EQUIVALENT(self, o) -> ubool:
-        return self.XOR(o).NOT()
+    def XOR(self, o: ubool) -> ubool:
+        if not isinstance(o, ubool):
+            o = ubool(o)
 
-    def XOR(self, o) -> ubool:
+        return ubool(abs(self._c - o._c))
+
+    def XOR2(self, o: ubool) -> ubool:
         if not isinstance(o, ubool):
             o = ubool(o)
 
-        return ubool(abs(self.c - o.c))
+        return self.EQUIVALENT2(o).NOT()
 
     def __xor__(self, other) -> ubool:
         return self.XOR(other)
     
     def __rxor__(self, left) -> ubool:
         return ubool(left).XOR(self)
+    
+    def EQUIVALENT(self, o: ubool) -> ubool:
+        return self.XOR(o).NOT()
+    
+    def EQUIVALENT2(self, o: ubool) -> ubool:
+        return self.IMPLIES(o).AND(o.IMPLIES(self))
+
+    def EQUALS(self, o: ubool) -> ubool:
+        if id(self) == id(o):
+            return True
+        if o is None or self.__class__ != o.__class__:
+            return False
 
-    def EQUALS(self, o) -> ubool:
-        return self.EQUIVALENT(o)
+        return abs(o.confidence - self.confidence) < 0.001
     
-    def equals(self, o) -> ubool:
+    def equals(self, o: ubool) -> ubool:
         return self.EQUALS(o)
 
     def __eq__(self, other) -> ubool:
         return self.EQUALS(other)
     
-    def DISTINCT(self, o) -> ubool: 
-        return self.EQUALS(o).NOT()
+    def DISTINCT(self, o: ubool) -> ubool: 
+        return not self.EQUALS(o)
     
-    def distinct(self, o) -> ubool: 
+    def distinct(self, o: ubool) -> ubool: 
         return self.DISTINCT(o)
     
     def __ne__(self, other) -> ubool:
         return self.DISTINCT(other)
 
     ''' Comparison operations '''
 
     def equalsC(self, o, conf) -> bool:
-        return abs(self.c - o.c) <= (1 - conf)
+        return abs(self._c - o._c) <= (1 - conf)
 
     ''' Other Methods  '''
     def compareTo(self, o) -> int:
-        x = self.c - o.c
+        x = self._c - o._c
         if (abs(x) < 0.001): return 0
         if (x < 0): return -1
         
         return 1    
 
     def copy(self) -> ubool:
-        return ubool(self.c)
+        return ubool(self._c)
 
     ''' Conversions '''
     def __str__(self) -> str:
-        return 'ubool({:5.3f})'.format(self.c)
+        return 'ubool({:5.3f})'.format(self._c)
     
     def __repr__(self) -> str:
-        return 'ubool({:5.3f})'.format(self.c)
+        return self.__str__()
 
     def tobool(self, c: float = None) -> bool:
         if c is None:
             c = self.__class__.CERTAINTY
-        return self.c >= c
+        return self._c >= c
     
     def __bool__(self) -> bool:
         return self.tobool()
```

### Comparing `uncertainty-datatypes-1.0.9/uncertainty/unumbers.py` & `uncertainty-datatypes-1.1.0/uncertainty/unumbers.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,47 +13,44 @@
     # x: int 
     # u: float 
 
 	def __init__(self, x: int|str|tuple = 0, u: int|float|str = 0.0) -> uint:
 		if isinstance(x, tuple) and len(x) == 2:
 			x, u = x
 		elif isinstance(x, (uint, ufloat)):
-			u = x.u
-			x = x.x
+			u = x.uncertainty
+			x = x.value
 
 		if not isinstance(x, (int, str)):
-			raise ValueError("Invalid parameter: x is not int or int as string")
+			raise ValueError('Invalid parameter: x is not int or int as string')
 		if not isinstance(u, (int, float, str)):
-			raise ValueError("Invalid parameter: u is not int, float or float/int as string")
+			raise ValueError('Invalid parameter: u is not int, float or float/int as string')
 		
-		self.x = int(x)
-		self.u = abs(float(u))
+		self._x = int(x)
+		self._u = abs(float(u))
 
 	@property
-	def u(self):
+	def uncertainty(self):
 		return self._u
 
-	@u.setter
-	def u(self, u: float|str):
-		if not isinstance(u, (float, str)):
-			raise ValueError("Invalid parameter: u not float or float as string")
-		
-		self._u = abs(float(u))
-		
+	@property
+	def value(self):
+		return self._x
+
 	''' Type Operations '''
 
 	def add(self, r: int|uint|float|ufloat, covariance: float = 0.0) -> uint:
 		if isinstance(r, float):
 			return self.toufloat() + ufloat(r)
 		elif isinstance(r, ufloat):
 			return self.toufloat() + r
 		elif isinstance(r, int):
 			r = uint(r)
 			
-		return uint(self.x + r.x, math.sqrt((self.u * self.u) + (r.u**2) + 2 * covariance))
+		return uint(self._x + r.value, math.sqrt((self._u * self._u) + (r.uncertainty**2) + 2 * covariance))
 	
 	def __add__(self, r: int|uint) -> uint:
 		return self.add(r)
 	
 	def __radd__(self, left) -> uint:
 		if isinstance(left, int):
 			left = uint(left)
@@ -67,17 +64,17 @@
 			return self.toufloat() - ufloat(r)
 		elif isinstance(r, ufloat):
 			return self.toufloat() - r
 		elif isinstance(r, int):
 			r = uint(r)
 
 		if id(r) == id(self): 
-			return uint(self.x - r.x, 0.0) 		# pathological case, x-x
+			return uint(self._x - r.value, 0.0) 		# pathological case, x-x
 		else: 
-			return uint(self.x - r.x, math.sqrt((self.u*self.u) + (r.u**2)  - 2 * covariance))
+			return uint(self._x - r.value, math.sqrt((self._u*self._u) + (r.uncertainty**2)  - 2 * covariance))
 	
 	def __sub__(self, r: int|uint|float|ufloat):
 		return self.sub(r)
 	
 	def __rsub__(self, left) -> uint:
 		if isinstance(left, int):
 			left = uint(left)
@@ -90,19 +87,19 @@
 		if isinstance(r, float):
 			return self.toufloat() * ufloat(r)
 		elif isinstance(r, ufloat):
 			return self.toufloat() * r
 		elif isinstance(r, int):
 			r = uint(r)
 
-		a = r.x**2 * self.u**2
-		b = self.x**2 * r.u**2
-		c = 2 * self.x * r.x * covariance
+		a = r.value**2 * self._u**2
+		b = self._x**2 * r.uncertainty**2
+		c = 2 * self._x * r.value * covariance
 
-		return uint(self.x * r.x, math.sqrt(a + b + c))
+		return uint(self._x * r.value, math.sqrt(a + b + c))
 
 	def __mul__(self, r) -> uint:
 		return self.mul(r)
 	
 	def __rmul__(self, left) -> uint:
 		if isinstance(left, int):
 			left = uint(left)
@@ -111,24 +108,24 @@
 			
 		return left * self
 
 	''' self operation returns a ufloat '''
 	def __div(self, r: ufloat, covariance:float = 0.0) -> ufloat:
 		if r == self:    		# pathological cases x/x
 			return 1, 0.0
-		elif r.u == 0.0:  		# r is a scalar
-			return self.x / r.x, self.u / r.x 		# "self" may be a scalar, too
-		elif self.u == 0.0:  		# "self is a scalar, r is not
-			return self.x / r.x, r.u / (r.x**2)
+		elif r.uncertainty == 0.0:  		# r is a scalar
+			return self._x / r.value, self._u / r.value 		# 'self' may be a scalar, too
+		elif self._u == 0.0:  		# 'self is a scalar, r is not
+			return self._x / r.value, r.uncertainty / (r.value**2)
 		
 		# both variables have associated uncertainty
-		a: float = self.x / r.x		
-		c: float = abs(((self.u**2) / r.x))
-		d: float = (self.x**2 * r.u**2) / (r.x**4)
-		e: float = abs((self.x * covariance)/(r.x**3))
+		a: float = self._x / r.value		
+		c: float = abs(((self._u**2) / r.value))
+		d: float = (self._x**2 * r.uncertainty**2) / (r.value**4)
+		e: float = abs((self._x * covariance)/(r.value**3))
 		
 		return a, math.sqrt(c + d - e)
 	
 	def div(self, r: uint|ufloat|int|float, covariance: float = 0.0) -> ufloat:
 		return self.toufloat() / (ufloat(r) if isinstance(r, (int,float)) else r.toufloat())
 
 	def __truediv__(self, r) -> uint:
@@ -145,15 +142,15 @@
 	def floordiv(self, r: uint|ufloat|int|float, covariance: float = 0.0) -> uint|ufloat:
 		if isinstance(r, (int, uint)):
 			x, u = self.__div(uint(r) if isinstance(r, int) else r , covariance)
 			return uint(math.floor(x), u)
 		elif isinstance(r, (float, ufloat)):
 			return self.toufloat().floordiv(ufloat(r) if isinstance(r, float) else r, covariance)
 		else:
-			raise RuntimeError("Invalid divisor")
+			raise RuntimeError('Invalid divisor')
 		
 	def __floordiv__(self, r):
 		return self.floordiv(r, 0.0)
 	
 	def __rfloordiv__(self, left):
 		if isinstance(left, int):
 			left = uint(left)
@@ -168,44 +165,44 @@
 	
 		if id(r) == id(self):  		# pathological cases x/x
 			return uint(0, 0.0)
 		
 		if isinstance(r, (float, ufloat)):
 			return self.toufloat() % r
 		elif isinstance(r, int):  		# r is a scalar
-			return uint(self.x % r, self.u / r) 		# "self" may be a scalar, too
-		elif r.u == 0.0:  		# r is a scalar
-			return uint(self.x % r.x, self.u / r.x) 		# "self" may be a scalar, too
-		elif self.u == 0.0: 		# "self is a scalar, r is not
-			return uint(self.x % r.x, r.u / (r.x**2))
+			return uint(self._x % r, self._u / r) 		# 'self' may be a scalar, too
+		elif r.uncertainty == 0.0:  		# r is a scalar
+			return uint(self._x % r.value, self._u / r.value) 		# 'self' may be a scalar, too
+		elif self._u == 0.0: 		# 'self is a scalar, r is not
+			return uint(self._x % r.value, r.uncertainty / (r.value**2))
 		
 		# both variables have associated uncertainty
-		a = self.x % r.x
+		a = self._x % r.value
 		
-		c = abs(((self.u**2) / r.x))
-		d = (self.x**2 * r.u**2) / (r.x**4)
-		e = abs((self.x * covariance) / (r.x**3))
+		c = abs(((self._u**2) / r.value))
+		d = (self._x**2 * r.uncertainty**2) / (r.value**4)
+		e = abs((self._x * covariance) / (r.value**3))
 		
 		return uint(math.floor(a), math.sqrt(c + d - e))
 		
 	def __mod__(self, r: uint|int):
 		if isinstance(r, int):
 			return self.mod(uint(r))
 		
 		return self.mod(r)
 
 	''' Rest of the type operations '''
 	def abs(self) -> uint:
-		return uint(abs(self.x), self.u)
+		return uint(abs(self._x), self._u)
 	
 	def __abs__(self) -> ufloat:
 		return self.abs()
 	
 	def neg(self) -> uint:
-		return uint(-self.x, self.u)
+		return uint(-self._x, self._u)
 	
 	def __neg__(self) -> uint:
 		return self.neg()
 	
 	def power(self, s: float|int) -> uint:
 		return (self.toufloat()**s).touint()
 	
@@ -225,187 +222,197 @@
 		return not self.equals(r)
 	
 	''' FuZZY COMPARISON OPERATIONS
 		Assume ufloat values (x,u) represent standard uncertainty values, i.e., they follow a Normal distribution
 	 	of mean x and standard deviation \sigma = u
 	 '''
 	def uEquals(self, r: uint|ufloat) -> ubool:
+		if isinstance(r, (int, float)):
+			r = ufloat(r)
 		return self.toufloat() == r.toufloat()
 	
 	def eq(self, other) -> ubool:
 		return self.uEquals(other)
 	
 	def __eq__(self, r: uint|ufloat) -> ubool:
 		return self.uEquals(r)
 
 	def uDistinct(self, r: uint|ufloat) -> ubool:
+		if isinstance(r, (int, float)):
+			r = ufloat(r)
 		return ~self.uEquals(r)
 	
 	def ne(self, other) -> ubool:
 		return self.uDistinct(other)
 	
 	def __ne__(self, r: uint|ufloat) -> ubool:
 		return self.uDistinct(r)
 
 	def lt(self, r: uint|ufloat) -> ubool:
+		if isinstance(r, (int, float)):
+			r = ufloat(r)
 		return self.toufloat() < r.toufloat()
 	
 	def __lt__(self, r: uint|ufloat) -> ubool:
 		return self.lt(r)
 
 	def le(self, r: uint|ufloat) -> ubool:
+		if isinstance(r, (int, float)):
+			r = ufloat(r)
 		return self.toufloat() <= r.toufloat()
 
 	def __le__(self, r: uint|ufloat) -> ubool:
 		return self.le(r)
 
 	def gt(self, r: uint|ufloat) -> ubool:
+		if isinstance(r, (int, float)):
+			r = ufloat(r)
 		return self.toufloat() > r.toufloat()
 	
 	def __gt__(self, r: uint|ufloat) -> ubool:
 		return self.gt(r)
 	
 	def ge(self, r: uint|ufloat) -> ubool:
+		if isinstance(r, (int, float)):
+			r = ufloat(r)
 		return self.toufloat() >= r.toufloat()
 	
 	def __ge__(self, r: uint|ufloat) -> ubool:
 		return self.ge(r)
 
 	''' END OF FuZZY COMPARISON OPERATIONS '''
 
 	''' Conversions '''
 	def __str__(self) -> str:
-		return "uint({:d}, {:5.3f})".format(self.x, self.u)
-	
+		return 'uint({:d}, {:5.3f})'.format(self._x, self._u)
+    
 	def __repr__(self) -> str:
-		return "uint({:d}, {:5.3f})".format(self.x, self.u)
+		return self.__str__()
 
 	def toint(self) -> int:
-		return self.x
+		return self._x
 	
 	def touint(self) -> uint:
 		return self
 	
 	def tofloat(self) -> float: 
-		return self.x
+		return self._x
 	
 	def toufloat(self) -> ufloat:
-		return ufloat(self.x, self.u)
+		return ufloat(self._x, self._u)
 	
 	''' Other Methods '''
 	def __hash__(self) -> int:
-		return round(float(self.x))
+		return round(float(self._x))
 
 	def copy(self) -> uint:
-		return uint(self.x,self.u)
+		return uint(self._x,self._u)
 
 class ufloat:
 	
     # Instance attributes:
     # x: float 
     # u: float 
 
 	''' Initializer '''
 	def __init__(self, x: float|int|str|tuple = 0.0, u: float|int|str = 0.0) -> ufloat:
 		if isinstance(x, tuple) and len(x) == 2:
 			x, u = x
 		elif isinstance(x, (uint, ufloat)):
-			u = x.u
-			x = x.x
+			u = x.uncertainty
+			x = x.value
 	
 		if not isinstance(x, (float, int, str)):
-			raise ValueError("Invalid parameter: x is not float, not int or float/int as string")
+			raise ValueError('Invalid parameter: x is not float, not int or float/int as string')
 		elif not isinstance(u, (float, int, str)):
-			raise ValueError("Invalid parameter: u is not float, not int or float/int as string")
+			raise ValueError('Invalid parameter: u is not float, not int or float/int as string')
 		
-		self.x = float(x)
-		self.u = abs(float(u))
+		self._x = float(x)
+		self._u = abs(float(u))
 
 	@property
-	def u(self):
+	def uncertainty(self):
 		return self._u
 
-	@u.setter
-	def u(self, u: float):
-		if not isinstance(u, float):
-			raise ValueError("Invalid parameter: u not float")
-		self._u = abs(u)
-
+	@property
+	def value(self):
+		return self._x
+	
 	def add(self, r: int|uint|float|ufloat, covariance: float = 0.0) -> ufloat:
 		if isinstance(r, (int, uint, float)):
 			r = ufloat(r)
 
-		return ufloat(self.x + r.x, math.sqrt(self.u**2 + r.u**2  + 2 * covariance))
+		return ufloat(self._x + r.value, math.sqrt(self._u**2 + r.uncertainty**2  + 2 * covariance))
 
 	def __add__(self, r) -> ufloat:
 		return self.add(r)
 	
 	def __radd__(self, left) -> ufloat:
 		return ufloat(left).add(self)
 
 	def sub(self, r: int|uint|float|ufloat, covariance: float = 0.0) -> ufloat:
 		if isinstance(r, (int, uint, float)):
 			r = ufloat(r)
 
 		if id(r) == id(self):
-			return ufloat(self.x - r.x, 0.0)
+			return ufloat(self._x - r.value, 0.0)
 		else:
-			return ufloat(self.x - r.x, math.sqrt(self.u**2 + r.u**2 - 2 * covariance))
+			return ufloat(self._x - r.value, math.sqrt(self._u**2 + r.uncertainty**2 - 2 * covariance))
 
 	def __sub__(self, other) -> ufloat:
 		return self.sub(other)
 	
 	def __rsub__(self, left) -> ufloat:
 		return ufloat(left).__sub__(self)
 
 	def mul(self, r: int|uint|float|ufloat, covariance: float = 0.0) -> ufloat:
 		if isinstance(r, (int, uint, float)):
 			r = ufloat(r)
 			
-		x = self.x * r.x
+		x = self._x * r.value
 
-		a = r.x**2 * self.u**2
-		b = self.x**2 * r.u**2
-		c = 2 * self.x * r.x * covariance
+		a = r.value**2 * self._u**2
+		b = self._x**2 * r.uncertainty**2
+		c = 2 * self._x * r.value * covariance
 
 		return ufloat(x, math.sqrt(a + b + c))
 	
 	def __mul__(self, other) -> ufloat:
 		return self.mul(other)
 	
 	def __rmul__(self, left) -> ufloat:
 		return ufloat(left).__mul__(self)
 
 	def __div(self, r: ufloat, covariance: float = 0.0) -> ufloat:
 		if id(r) == id(self): # pathological cases: x/x
 			return 1.0, 0.0
-		elif r.u == 0.0: # r is a scalar
-			return self.x / r.x, self.u / r.x # "self" may be a scalar, too
-		elif self.u == 0.0: # "this is a scalar, r is not
-			return self.x / r.x, r.u / (r.x**2)
+		elif r.uncertainty == 0.0: # r is a scalar
+			return self._x / r.value, self._u / r.value # 'self' may be a scalar, too
+		elif self._u == 0.0: # 'this is a scalar, r is not
+			return self._x / r.value, r.uncertainty / (r.value**2)
 		
 		# both variables have associated uncertainty	
 		
-		a: float = self.x / r.x
-		c: float = (self.u**2) / abs(r.x)
-		d: float = (self.x**2 * r.u**2) / (r.x**4)
+		a: float = self._x / r.value
+		c: float = (self._u**2) / abs(r.value)
+		d: float = (self._x**2 * r.uncertainty**2) / (r.value**4)
 		if covariance == 0.0:	
 			return a, math.sqrt(c + d)
 		else:
-			b: float = (self.x * r.u**2) / (r.x**3)
-			e: float = (self.x * covariance) / abs(r.x**3)			
+			b: float = (self._x * r.uncertainty**2) / (r.value**3)
+			e: float = (self._x * covariance) / abs(r.value**3)			
 			return a + b, math.sqrt(c + d - e)
 	
 	def div(self, r: uint|ufloat|int|float, covariance: float = 0.0) -> ufloat:
 		if isinstance(r, (int, uint)):
 			return ufloat(self.__div(uint(r) if isinstance(r, int) else r.toufloat() , covariance))
 		elif isinstance(r, (float, ufloat)):
 			return ufloat(self.__div(ufloat(r) if isinstance(r, float) else r, covariance))
 		else:
-			raise RuntimeError("Invalid divisor")
+			raise RuntimeError('Invalid divisor')
 
 	def __truediv__(self, other) -> ufloat:
 		return self.div(other, 0.0)
 	
 	def __rtruediv__(self, left) -> ufloat:
 		return ufloat(left).__truediv__(self)
 	
@@ -413,109 +420,109 @@
 		if isinstance(r, (int, uint)):
 			x, u = self.__div(uint(r) if isinstance(r, int) else r.toufloat() , covariance)
 			return ufloat(math.floor(x), u)
 		elif isinstance(r, (float, ufloat)):
 			x, u = self.__div(ufloat(r) if isinstance(r, float) else r, covariance)
 			return ufloat(math.floor(x), u)
 		else:
-			raise RuntimeError("Invalid divisor")
+			raise RuntimeError('Invalid divisor')
 
 	def __floordiv__(self, r):
 		return self.floordiv(r, 0.0)
 	
 	def __rfloordiv__(self, left):
 		return ufloat(left).__floordiv__(self)
 
 	def abs(self) -> ufloat:
-		return ufloat(abs(self.x), self.u)
+		return ufloat(abs(self._x), self._u)
 	
 	def __abs__(self) -> ufloat:
 		return self.abs()
 
 	def neg(self) -> ufloat:
-		return ufloat(-self.x, self.u)
+		return ufloat(-self._x, self._u)
 
 	def __neg__(self) -> ufloat:
 		return self.neg()
 	
 	def power(self, s: float|int) -> ufloat:
-		a = self.x**s
-		c = s * self.u * (self.x**(s-1))
+		a = self._x**s
+		c = s * self._u * (self._x**(s-1))
 
 		return ufloat(a, c)
 	
 	def __pow__(self, s: float|int) -> ufloat:
 		return self.power(s)
 	
 	def sqrt(self) -> ufloat:
-		if self.x == 0.0 and self.u == 0.0:
+		if self._x == 0.0 and self._u == 0.0:
 			return ufloat(0.0, 0.0)
-		elif self.x < 0.0:
+		elif self._x < 0.0:
 			raise ValueError('math domain error: negative number')
 		
-		x = math.sqrt(self.x)
-		u = (self.u) / (2 * math.sqrt(self.x))
+		x = math.sqrt(self._x)
+		u = (self._u) / (2 * math.sqrt(self._x))
 		
 		return ufloat(x, u)
 
 	def sin(self) -> ufloat:
-		return ufloat(math.sin(self.x), self.u * math.cos(self.x))
+		return ufloat(math.sin(self._x), self._u * math.cos(self._x))
 
 	def cos(self) -> ufloat:
-		return ufloat(math.cos(self.x), self.u * math.sin(self.x))
+		return ufloat(math.cos(self._x), self._u * math.sin(self._x))
 	
 	def tan(self) -> ufloat:
 		return self.sin().div(self.cos()) 
 	
 	def atan(self) -> ufloat:
-		return ufloat(math.atan(self.x), self.u / (1 + self.x**2))
+		return ufloat(math.atan(self._x), self._u / (1 + self._x**2))
 	
 	''' Type Operations '''
 
 	def acos(self) -> ufloat:
-		if abs(self.x) == 1.0:
-			return ufloat(math.acos(self.x), self.u)
+		if abs(self._x) == 1.0:
+			return ufloat(math.acos(self._x), self._u)
 		else:
-			return ufloat(math.acos(self.x), self.u / math.sqrt(1 - self.x**2))
+			return ufloat(math.acos(self._x), self._u / math.sqrt(1 - self._x**2))
 
 	def asin(self) -> ufloat:
-		if abs(self.x) == 1.0:
-			return ufloat(math.asin(self.x), self.u)
+		if abs(self._x) == 1.0:
+			return ufloat(math.asin(self._x), self._u)
 		else:
-			return ufloat(math.asin(self.x), self.u/math.sqrt((1 - self.x**2)))
+			return ufloat(math.asin(self._x), self._u/math.sqrt((1 - self._x**2)))
 
 	def inverse(self) -> ufloat: #inverse (reciprocal)
 		return ufloat(1.0, 0.0) / self
 
 	def floor(self) -> ufloat: #returns (i,u) with i the largest int such that (i,u)<=(x,u)
-		return ufloat(math.floor(self.x),self.u)
+		return ufloat(math.floor(self._x),self._u)
 
 	def round(self) -> ufloat: #returns (i,u) with i the closest int to x
-		return ufloat(round(self.x), self.u)
+		return ufloat(round(self._x), self._u)
 
 	''' Comparison operations '''
 	def equals(self, other) -> bool:
 		''' we compute the separation factor of the two distributions considered as a mixture
 		 	see http:#faculty.washington.edu/tamre/IsHumanHeightBimodal.pdf '''
 		if id(self) == id(other): return True
 		
-		s1 = self.u
-		s2 = other.u
+		s1 = self._u
+		s2 = other.uncertainty
 		# non-ufloat cases first
 		if s1 == 0 or s2 == 0:
-			return self.x == other.x
+			return self._x == other.value
 		# if both numbers have some uncertainty
 		r = (s1 * s1) / (s2 * s2)
 
 		S = math.sqrt(-2.0 + 3*r + 3*r*r - 2*r*r*r + 2 * math.pow(1 - r + r*r, 1.5) ) / (math.sqrt(r) * (1 + math.sqrt(r)))
 		if math.isnan(S): # similar to s1==0 or s2==0. No way to compute the separation test
-			return (self.x == other.x)
+			return (self._x == other.value)
 		
 		separation = S * (s1 + s2)
-		return abs(other.x - self.x) <= separation # they are indistinguishable
+		return abs(other.value - self._x) <= separation # they are indistinguishable
 
 	def distinct(self, other) -> bool:
 		return not self.equals(other)
 	
 	''' FUZZY COMPARISON OPERATIONS
 	    Assume ufloat values (x,u) represent standard uncertainty values, i.e., they follow a Normal distribution
 	    of mean x and standard deviation \sigma = u
@@ -583,18 +590,18 @@
      	eq: this = number
      	gt: this > number
 	'''
 	def calculate(self, number: ufloat|uint) -> Result:
 		r = Result()
 		m1 = 0.0; m2 = 0.0; s1 = 0.0; s2 = 0.0; swap = False
 
-		if self.x <= number.x: # m1 is less or equal than m2
-			m1 = self.x; m2 = float(number.x); s1 = self.u; s2 = number.u
+		if self._x <= number.value: # m1 is less or equal than m2
+			m1 = self._x; m2 = float(number.value); s1 = self._u; s2 = number.uncertainty
 		else:
-			m2 = self.x; m1 = float(number.x); s2 = self.u; s1 = number.u
+			m2 = self._x; m1 = float(number.value); s2 = self._u; s1 = number.uncertainty
 			swap = True # to return values in the correct order
 
 		if s1 == 0.0 and s2 == 0.0: #comparison between Real numbers
 			if m1 == m2:
 				r.lt = 0.0; r.eq = 1.0; r.gt = 0.0 
 				return r.check(swap) 
 	
@@ -641,89 +648,95 @@
 			else:
 				r.lt = self.CNDF(c1, m1, s1)-self.CNDF(c1, m2, s2)
 				r.gt = 1.0 - self.CNDF(c2, m1, s1) - (1.0 - self.CNDF(c2, m2, s2))
 				r.eq = self.CNDF(c1, m2, s2) + (1.0 - self.CNDF(c2, m2, s2)) + self.CNDF(c2,m1,s1) - self.CNDF(c1,m1,s1)
 	
 			return r.check(swap) 
 		
-	def uEquals(self, number: uint|ufloat) -> ubool:
-		r = self.calculate(number.toufloat())
+	def uEquals(self, other: uint|ufloat) -> ubool:
+		if isinstance(other, (int, float)):
+			other = ufloat(other)
+		r = self.calculate(other.toufloat())
 		return ubool(r.eq)
 
 	def eq(self, other) -> ubool:
 		return self.uEquals(other)
 
 	def __eq__(self, other) -> ubool:
 		return self.eq(other)
 
-	def uDistinct(self, r: uint|ufloat) -> ubool:
-		return ~self.uEquals(r)
+	def uDistinct(self, other: uint|ufloat) -> ubool:
+		if isinstance(other, (int, float)):
+			other = ufloat(other)
+		return ~self.uEquals(other)
 	
 	def ne(self, other) -> ubool:
+		if isinstance(other, (int, float)):
+			other = ufloat(other)
 		return self.uDistinct(other)
 
 	def __ne__(self, other) -> ubool:
 		return self.uDistinct(other)
 
 	def lt(self, number: uint|ufloat) -> ubool:
-		r = self.calculate(number.toufloat())
+		r = self.calculate(ufloat(number) if isinstance(number, (int, float)) else number.toufloat())
 		return ubool(r.lt)
 	
 	def __lt__(self, number: uint|ufloat) -> ubool:
 		return self.lt(number)
 	
 	def le(self, number: uint|ufloat) -> ubool:
-		r = self.calculate(number.toufloat())
+		r = self.calculate(ufloat(number) if isinstance(number, (int, float)) else number.toufloat())
 		return ubool(r.lt + r.eq)
 
 	def __le__(self, number: uint|ufloat) -> ubool:
 		return self.le(number)
 
 	def gt(self, number: uint|ufloat) -> ubool:
 		r = self.calculate(ufloat(number) if isinstance(number, (int, float)) else number.toufloat())
 		return ubool(r.gt)
 	
 	def __gt__(self, number: uint|ufloat) -> ubool:
 		return self.gt(number)
 	
 	def ge(self, number: uint|ufloat) -> ubool:
-		r = self.calculate(number.toufloat())
+		r = self.calculate(ufloat(number) if isinstance(number, (int, float)) else number.toufloat())
 		return ubool(r.gt + r.eq)
 	
 	def __ge__(self, number: uint|ufloat) -> ubool:
 		return self.ge(number)
 
 	''' END OF FUZZY COMPARISON OPERATIONS '''
 
 	''' Conversions '''
 	def toint(self) -> int:
-		return int(math.floor(self.x))
+		return int(math.floor(self._x))
 
 	def touint(self) -> uint:
-		x = int(math.floor(self.x))
-		u = math.sqrt((self.u * self.u) + (self.x - x) * (self.x - x))
+		x = int(math.floor(self._x))
+		u = math.sqrt((self._u * self._u) + (self._x - x) * (self._x - x))
 		return uint(x, u)
 	
 	def tofloat(self) -> float: 
-		return self.x
+		return self._x
 	
 	def toufloat(self) -> ufloat: 
 		return self
 
 	def toBestuint(self) -> uint:
-		x = int(round(self.x))
-		u = math.sqrt((self.u * self.u) + (self.x - x) * (self.x - x))
+		x = int(round(self._x))
+		u = math.sqrt((self._u * self._u) + (self._x - x) * (self._x - x))
 		return uint(x, u)
 
 	''' Other Methods '''
 	def __hash__(self):
-		return round(self.x)
+		return round(self._x)
 	
 	def copy(self) -> ufloat:
-		return ufloat(self.x, self.u)
+		return ufloat(self._x, self._u)
 
 	''' Conversions '''
 	def __str__(self) -> str:
-		return "ufloat({:5.3f}, {:5.3f})".format(self.x, self.u)
-	
+		return 'ufloat({:5.3f}, {:5.3f})'.format(self._x, self._u)
+    
 	def __repr__(self) -> str:
-		return "ufloat({:5.3f}, {:5.3f})".format(self.x, self.u)
+		return self.__str__()
```

### Comparing `uncertainty-datatypes-1.0.9/uncertainty/utypes.py` & `uncertainty-datatypes-1.1.0/uncertainty/utypes.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 from __future__ import annotations
 
 from collections.abc import Iterable
 
 from uncertainty.ubool import ubool
+from uncertainty.abool import abool
+from uncertainty.sbool import sbool
 from uncertainty.result import Result
 from uncertainty.unumbers import uint
 from uncertainty.unumbers import ufloat
+from uncertainty.anumbers import aint
+from uncertainty.anumbers import afloat
+from uncertainty.ustr import ustr
+from uncertainty.uenum import uenum
 	
 # Operator Class
 class infix:
     def __init__(self, function):
         self.function = function
     def __or__(self, other):
         return self.function(other)
     def __ror__(self, other):
         return infix(lambda x, self=self, other=other: self.function(other, x))
     def __call__(self, value1, value2):
         return self.function(value1, value2)
     
 # Operator functions
-AND = infix(lambda l, r: l.AND(r) if isinstance(l, ubool) else r.AND(l))
-OR = infix(lambda l, r: l.OR(r) if isinstance(l, ubool) else r.OR(l))
-XOR = infix(lambda l, r: l.XOR(r) if isinstance(l, ubool) else r.XOR(l))
-IMPLIES = infix(lambda l, r: l.IMPLIES(r) if isinstance(l, ubool) else r.IMPLIES(l))
-EQUIVALENT = infix(lambda l, r: l.EQUIVALENT(r) if isinstance(l, ubool) else r.EQUIVALENT(l))
-EQUALS = infix(lambda l, r: l.EQUALS(r) if isinstance(l, ubool) else r.EQUALS(l))
-DISTINCT = infix(lambda l, r: l.DISTINCT(r) if isinstance(l, ubool) else r.DISTINCT(l))
+AND = infix(lambda l, r: l.AND(r) if isinstance(l, (ubool, abool, sbool)) else r.AND(l))
+OR = infix(lambda l, r: l.OR(r) if isinstance(l, (ubool, abool, sbool)) else r.OR(l))
+XOR = infix(lambda l, r: l.XOR(r) if isinstance(l, (ubool, abool, sbool)) else r.XOR(l))
+IMPLIES = infix(lambda l, r: l.IMPLIES(r) if isinstance(l, (ubool, abool, sbool)) else r.IMPLIES(l))
+EQUIVALENT = infix(lambda l, r: l.EQUIVALENT(r) if isinstance(l, (ubool, abool, sbool)) else r.EQUIVALENT(l))
+EQUALS = infix(lambda l, r: l.EQUALS(r) if isinstance(l, (ubool, abool, sbool)) else r.EQUALS(l))
+DISTINCT = infix(lambda l, r: l.DISTINCT(r) if isinstance(l, (ubool, abool, sbool)) else r.DISTINCT(l))
 NOT = lambda x: x.NOT()
 
 add = infix(lambda l, r: l + r)
+concat = infix(lambda l, r: l + r)
 sub = infix(lambda l, r: l - r)
 mul = infix(lambda l, r: l * r)
 div = infix(lambda l, r: l / r)
 floordiv = infix(lambda l, r: l // r)
 neg = lambda l: -l
 pow = infix(lambda l, r: l ** r)
 mod = infix(lambda l, r: l % r)
@@ -42,15 +49,24 @@
 gt = infix(lambda l, r: l > r)
 ge = infix(lambda l, r: l >= r)
 eq = infix(lambda l, r: l == r)
 ne = infix(lambda l, r: l != r)
 
 # Data Functions
 def is_utype(obj) -> bool:
-    return isinstance(obj, (uint, ufloat, ubool))
+    return isinstance(obj, (uint, ufloat, ubool, ustr, uenum, abool, aint, afloat))
+
+def is_ubool(obj) -> bool:
+    return isinstance(obj, ubool)
+
+def is_ufloat(obj) -> bool:
+    return isinstance(obj, ufloat)
+
+def is_uint(obj) -> bool:
+    return isinstance(obj, uint)
 
 def is_unumber(obj) -> bool:
     return isinstance(obj, (uint, ufloat))
 
 def __call_func(obj: uint|ufloat, funcname: str):
     #attrname: str = '_' + str(type(obj).__name__) + '__' + funcname
     if hasattr(obj, funcname):
@@ -65,16 +81,18 @@
     
 def __check_objs(objs: Iterable):
     for o in objs:
         __check_obj(o)
 
 # abs
 def abs(obj: uint|ufloat) -> uint|ufloat:
-    __check_obj(obj)
-    return __call_func(obj, abs.__name__)
+    if is_unumber(obj):
+        return __call_func(obj, abs.__name__)
+    else:
+        obj.__abs__()
 
 # sqrt
 def sqrt(obj: uint|ufloat) -> uint|ufloat:
     __check_obj(obj)
     return __call_func(obj.toufloat(), sqrt.__name__)
 
 # inverse
@@ -85,24 +103,26 @@
 def __search(rs: Iterable, eval):
     if len(rs) == 0:
         raise ValueError('expected at least 1 argument, got 0')
     if len(rs) == 1:
         return rs[0]
     
     ev = eval(rs[0], rs[1]); rev = eval(rs[1], rs[0])
-    best = rs[0] if ev.c > rev.c else rs[1]
-    for r in rs:
-        ev = eval(best, r); rev = eval(r, best)
-        if ev.c < rev.c:
+    best = rs[0] if ev.uncertainty > rev.uncertainty else rs[1]
+    for i in range(2, len(rs)):
+        r = rs[i]
+        ur = r if is_utype(r) else ufloat(r)
+        ev = eval(best, ur); rev = eval(ur, best)
+        if ev.uncertainty < rev.uncertainty:
             best = r
     
     if is_utype(best):
         return best.copy()
     else:
-        best
+        return best
 
 # min
 def min(*rs):
     return __search(rs, lambda r, min : r < min)
 
 #max
 def max(*rs):
@@ -147,7 +167,34 @@
 
 # round
 def round(obj: uint|ufloat) -> uint|ufloat:
     __check_obj(obj)
     if isinstance(obj, uint):
         return obj
     return __call_func(obj.toufloat(), round.__name__)
+
+def beliefConstraintFusion(opinions: Iterable[sbool]) -> sbool:
+    return sbool.beliefConstraintFusion(opinions)
+
+def minimumBeliefFusion(opinions: Iterable[sbool]) -> sbool:
+    return sbool.minimumBeliefFusion(opinions)
+
+def majorityBeliefFusion(opinions: Iterable[sbool]) -> sbool:
+    return sbool.majorityBeliefFusion(opinions)
+
+def averageBeliefFusion(opinions: Iterable[sbool]) -> sbool:
+    return sbool.averageBeliefFusion(opinions)
+
+def productOfUncertainties(opinions: Iterable[sbool]) -> sbool:
+    return sbool.productOfUncertainties(opinions)
+
+def cumulativeBeliefFusion(opinions: Iterable[sbool]) -> sbool:
+    return sbool.cumulativeBeliefFusion(opinions)
+
+def epistemicCumulativeBeliefFusion(opinions: Iterable[sbool]) -> sbool:
+    return sbool.epistemicCumulativeBeliefFusion(opinions)
+
+def weightedBeliefFusion(opinions: Iterable[sbool]) -> sbool:
+    return sbool.weightedBeliefFusion(opinions)
+
+def consensusAndCompromiseFusion(opinions: Iterable[sbool]) -> sbool:
+    return sbool.consensusAndCompromiseFusion(opinions)
```


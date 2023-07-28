# Comparing `tmp/pywaf-0.9.4.tar.gz` & `tmp/pywaf-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywaf-0.9.4.tar", last modified: Fri Jul 28 18:14:36 2023, max compression
+gzip compressed data, was "pywaf-0.9.5.tar", last modified: Fri Jul 28 18:20:02 2023, max compression
```

## Comparing `pywaf-0.9.4.tar` & `pywaf-0.9.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 18:14:36.476542 pywaf-0.9.4/
--rw-rw-rw-   0        0        0      124 2023-07-28 18:14:36.476542 pywaf-0.9.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 18:14:36.470558 pywaf-0.9.4/pywaf.egg-info/
--rw-rw-rw-   0        0        0      124 2023-07-28 18:14:36.000000 pywaf-0.9.4/pywaf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-07-28 18:14:36.000000 pywaf-0.9.4/pywaf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 18:14:36.000000 pywaf-0.9.4/pywaf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-28 17:33:53.000000 pywaf-0.9.4/pywaf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        4 2023-07-28 18:14:36.000000 pywaf-0.9.4/pywaf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 18:14:36.478537 pywaf-0.9.4/setup.cfg
--rw-rw-rw-   0        0        0      215 2023-07-28 18:14:23.000000 pywaf-0.9.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:14:36.475544 pywaf-0.9.4/waf/
--rw-rw-rw-   0        0        0       85 2023-07-28 17:32:51.000000 pywaf-0.9.4/waf/__init__.py
--rw-rw-rw-   0        0        0    18615 2023-07-28 16:53:26.000000 pywaf-0.9.4/waf/kernel.py
--rw-rw-rw-   0        0        0     3881 2023-07-28 18:14:16.000000 pywaf-0.9.4/waf/wavelet.py
--rw-rw-rw-   0        0        0     1560 2023-07-28 17:38:16.000000 pywaf-0.9.4/waf/window.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:20:02.372123 pywaf-0.9.5/
+-rw-rw-rw-   0        0        0      124 2023-07-28 18:20:02.372123 pywaf-0.9.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 18:20:02.368134 pywaf-0.9.5/pywaf.egg-info/
+-rw-rw-rw-   0        0        0      124 2023-07-28 18:20:02.000000 pywaf-0.9.5/pywaf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-07-28 18:20:02.000000 pywaf-0.9.5/pywaf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 18:20:02.000000 pywaf-0.9.5/pywaf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-28 17:33:53.000000 pywaf-0.9.5/pywaf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        4 2023-07-28 18:20:02.000000 pywaf-0.9.5/pywaf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 18:20:02.373120 pywaf-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0      215 2023-07-28 18:19:45.000000 pywaf-0.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:20:02.371126 pywaf-0.9.5/waf/
+-rw-rw-rw-   0        0        0       85 2023-07-28 17:32:51.000000 pywaf-0.9.5/waf/__init__.py
+-rw-rw-rw-   0        0        0    18615 2023-07-28 16:53:26.000000 pywaf-0.9.5/waf/kernel.py
+-rw-rw-rw-   0        0        0     3891 2023-07-28 18:19:35.000000 pywaf-0.9.5/waf/wavelet.py
+-rw-rw-rw-   0        0        0     1560 2023-07-28 17:38:16.000000 pywaf-0.9.5/waf/window.py
```

### Comparing `pywaf-0.9.4/waf/kernel.py` & `pywaf-0.9.5/waf/kernel.py`

 * *Files identical despite different names*

### Comparing `pywaf-0.9.4/waf/wavelet.py` & `pywaf-0.9.5/waf/wavelet.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,19 +83,19 @@
 
         return fourier_series(self.H, n)
 
     def rec_lo(self, dec_lo):
         return np.conj(dec_lo)
 
     def dec_hi(self, dec_lo, n, N):
-        coef = (-1)**(n+1)
+        coef = np.power(-1,n+1)
         return coef*dec_lo
 
     def rec_hi(self, dec_lo, n, N):
-        coef = (-1)**(n+1)
+        coef = np.power(-1,n+1)
         return coef*dec_lo
 
     def filter(self, N):
         n = np.arange(-N//2, N//2)
         dec_lo_mass = self.dec_lo(n)
         dec_hi_mass = self.dec_hi(dec_lo_mass, n, N)
         rec_lo_mass = self.rec_lo(dec_lo_mass)
```

### Comparing `pywaf-0.9.4/waf/window.py` & `pywaf-0.9.5/waf/window.py`

 * *Files identical despite different names*


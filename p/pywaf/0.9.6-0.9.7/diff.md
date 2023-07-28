# Comparing `tmp/pywaf-0.9.6.tar.gz` & `tmp/pywaf-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywaf-0.9.6.tar", last modified: Fri Jul 28 18:22:51 2023, max compression
+gzip compressed data, was "pywaf-0.9.7.tar", last modified: Fri Jul 28 18:26:06 2023, max compression
```

## Comparing `pywaf-0.9.6.tar` & `pywaf-0.9.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 18:22:51.794067 pywaf-0.9.6/
--rw-rw-rw-   0        0        0      124 2023-07-28 18:22:51.794067 pywaf-0.9.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 18:22:51.789081 pywaf-0.9.6/pywaf.egg-info/
--rw-rw-rw-   0        0        0      124 2023-07-28 18:22:51.000000 pywaf-0.9.6/pywaf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-07-28 18:22:51.000000 pywaf-0.9.6/pywaf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 18:22:51.000000 pywaf-0.9.6/pywaf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-28 17:33:53.000000 pywaf-0.9.6/pywaf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        4 2023-07-28 18:22:51.000000 pywaf-0.9.6/pywaf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 18:22:51.795065 pywaf-0.9.6/setup.cfg
--rw-rw-rw-   0        0        0      215 2023-07-28 18:22:42.000000 pywaf-0.9.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:22:51.793070 pywaf-0.9.6/waf/
--rw-rw-rw-   0        0        0       85 2023-07-28 17:32:51.000000 pywaf-0.9.6/waf/__init__.py
--rw-rw-rw-   0        0        0    18615 2023-07-28 16:53:26.000000 pywaf-0.9.6/waf/kernel.py
--rw-rw-rw-   0        0        0     3911 2023-07-28 18:22:24.000000 pywaf-0.9.6/waf/wavelet.py
--rw-rw-rw-   0        0        0     1560 2023-07-28 17:38:16.000000 pywaf-0.9.6/waf/window.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:26:06.799007 pywaf-0.9.7/
+-rw-rw-rw-   0        0        0      124 2023-07-28 18:26:06.799007 pywaf-0.9.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 18:26:06.795018 pywaf-0.9.7/pywaf.egg-info/
+-rw-rw-rw-   0        0        0      124 2023-07-28 18:26:06.000000 pywaf-0.9.7/pywaf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-07-28 18:26:06.000000 pywaf-0.9.7/pywaf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 18:26:06.000000 pywaf-0.9.7/pywaf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-28 17:33:53.000000 pywaf-0.9.7/pywaf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        4 2023-07-28 18:26:06.000000 pywaf-0.9.7/pywaf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 18:26:06.800006 pywaf-0.9.7/setup.cfg
+-rw-rw-rw-   0        0        0      215 2023-07-28 18:25:51.000000 pywaf-0.9.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:26:06.798010 pywaf-0.9.7/waf/
+-rw-rw-rw-   0        0        0       85 2023-07-28 17:32:51.000000 pywaf-0.9.7/waf/__init__.py
+-rw-rw-rw-   0        0        0    18615 2023-07-28 16:53:26.000000 pywaf-0.9.7/waf/kernel.py
+-rw-rw-rw-   0        0        0     3923 2023-07-28 18:25:43.000000 pywaf-0.9.7/waf/wavelet.py
+-rw-rw-rw-   0        0        0     1560 2023-07-28 17:38:16.000000 pywaf-0.9.7/waf/window.py
```

### Comparing `pywaf-0.9.6/waf/kernel.py` & `pywaf-0.9.7/waf/kernel.py`

 * *Files identical despite different names*

### Comparing `pywaf-0.9.6/waf/wavelet.py` & `pywaf-0.9.7/waf/wavelet.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,19 +80,19 @@
             for i in n:
                 h.append(np.trapz(func*np.exp(1j*w*i), x=w)/(2**0.5*np.pi))
             return np.real(h)
 
         return fourier_series(self.H, n)
 
     def rec_lo(self, dec_lo):
-        return np.conj(dec_lo)
+        return np.conj(dec_lo[::-1])
 
     def dec_hi(self, dec_lo, n, N):
         coef = np.power(-np.ones(N), n+1)
-        return coef*dec_lo
+        return coef*dec_lo[::-1]
 
     def rec_hi(self, dec_lo, n, N):
         coef = np.power(-np.ones(N), n+1)
         return coef*dec_lo
 
     def filter(self, N):
         n = np.arange(-N//2, N//2)
```

### Comparing `pywaf-0.9.6/waf/window.py` & `pywaf-0.9.7/waf/window.py`

 * *Files identical despite different names*


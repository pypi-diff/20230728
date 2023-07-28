# Comparing `tmp/pywaf-0.9.3.tar.gz` & `tmp/pywaf-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywaf-0.9.3.tar", last modified: Fri Jul 28 17:38:34 2023, max compression
+gzip compressed data, was "pywaf-0.9.4.tar", last modified: Fri Jul 28 18:14:36 2023, max compression
```

## Comparing `pywaf-0.9.3.tar` & `pywaf-0.9.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 17:38:34.587391 pywaf-0.9.3/
--rw-rw-rw-   0        0        0      124 2023-07-28 17:38:34.588389 pywaf-0.9.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 17:38:34.581408 pywaf-0.9.3/pywaf.egg-info/
--rw-rw-rw-   0        0        0      124 2023-07-28 17:38:34.000000 pywaf-0.9.3/pywaf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-07-28 17:38:34.000000 pywaf-0.9.3/pywaf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 17:38:34.000000 pywaf-0.9.3/pywaf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-28 17:33:53.000000 pywaf-0.9.3/pywaf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        4 2023-07-28 17:38:34.000000 pywaf-0.9.3/pywaf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 17:38:34.589387 pywaf-0.9.3/setup.cfg
--rw-rw-rw-   0        0        0      215 2023-07-28 17:38:26.000000 pywaf-0.9.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 17:38:34.586395 pywaf-0.9.3/waf/
--rw-rw-rw-   0        0        0       85 2023-07-28 17:32:51.000000 pywaf-0.9.3/waf/__init__.py
--rw-rw-rw-   0        0        0    18615 2023-07-28 16:53:26.000000 pywaf-0.9.3/waf/kernel.py
--rw-rw-rw-   0        0        0     3884 2023-07-28 17:38:17.000000 pywaf-0.9.3/waf/wavelet.py
--rw-rw-rw-   0        0        0     1560 2023-07-28 17:38:16.000000 pywaf-0.9.3/waf/window.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:14:36.476542 pywaf-0.9.4/
+-rw-rw-rw-   0        0        0      124 2023-07-28 18:14:36.476542 pywaf-0.9.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 18:14:36.470558 pywaf-0.9.4/pywaf.egg-info/
+-rw-rw-rw-   0        0        0      124 2023-07-28 18:14:36.000000 pywaf-0.9.4/pywaf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-07-28 18:14:36.000000 pywaf-0.9.4/pywaf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 18:14:36.000000 pywaf-0.9.4/pywaf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-28 17:33:53.000000 pywaf-0.9.4/pywaf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        4 2023-07-28 18:14:36.000000 pywaf-0.9.4/pywaf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 18:14:36.478537 pywaf-0.9.4/setup.cfg
+-rw-rw-rw-   0        0        0      215 2023-07-28 18:14:23.000000 pywaf-0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:14:36.475544 pywaf-0.9.4/waf/
+-rw-rw-rw-   0        0        0       85 2023-07-28 17:32:51.000000 pywaf-0.9.4/waf/__init__.py
+-rw-rw-rw-   0        0        0    18615 2023-07-28 16:53:26.000000 pywaf-0.9.4/waf/kernel.py
+-rw-rw-rw-   0        0        0     3881 2023-07-28 18:14:16.000000 pywaf-0.9.4/waf/wavelet.py
+-rw-rw-rw-   0        0        0     1560 2023-07-28 17:38:16.000000 pywaf-0.9.4/waf/window.py
```

### Comparing `pywaf-0.9.3/waf/kernel.py` & `pywaf-0.9.4/waf/kernel.py`

 * *Files identical despite different names*

### Comparing `pywaf-0.9.3/waf/wavelet.py` & `pywaf-0.9.4/waf/wavelet.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,32 +80,32 @@
             for i in n:
                 h.append(np.trapz(func*np.exp(1j*w*i), x=w)/(2**0.5*np.pi))
             return np.real(h)
 
         return fourier_series(self.H, n)
 
     def rec_lo(self, dec_lo):
-        return np.conj(dec_lo[::-1])
+        return np.conj(dec_lo)
 
     def dec_hi(self, dec_lo, n, N):
-        coef = np.power(-np.ones(N), n)
-        return coef*dec_lo[::-1]
+        coef = (-1)**(n+1)
+        return coef*dec_lo
 
     def rec_hi(self, dec_lo, n, N):
-        coef = np.power(-np.ones(N), n+1)
+        coef = (-1)**(n+1)
         return coef*dec_lo
 
     def filter(self, N):
         n = np.arange(-N//2, N//2)
         dec_lo_mass = self.dec_lo(n)
         dec_hi_mass = self.dec_hi(dec_lo_mass, n, N)
         rec_lo_mass = self.rec_lo(dec_lo_mass)
         rec_hi_mass = self.rec_hi(dec_lo_mass, n, N)
 
-        return (dec_lo_mass, dec_hi_mass, rec_lo_mass, rec_hi_mass)
+        return {'dec_lo': dec_lo_mass,'dec_hi': dec_hi_mass,'rec_lo': rec_lo_mass,'rec_hi': rec_hi_mass}
 
     def psi_f(self, w):
         return np.exp(1j*w/2)*(self.phi_f(w-2*np.pi) + self.phi_f(w+2*np.pi))*self.phi_f(w/2)
 
     def psi(self, x, N=10000):
         w = np.linspace(2*np.pi/3, 8*np.pi/3, N)
         psi = []
```

### Comparing `pywaf-0.9.3/waf/window.py` & `pywaf-0.9.4/waf/window.py`

 * *Files identical despite different names*


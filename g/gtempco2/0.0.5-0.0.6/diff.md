# Comparing `tmp/gtempco2-0.0.5.tar.gz` & `tmp/gtempco2-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtempco2-0.0.5.tar", last modified: Fri Jul 28 08:28:28 2023, max compression
+gzip compressed data, was "gtempco2-0.0.6.tar", last modified: Fri Jul 28 08:46:43 2023, max compression
```

## Comparing `gtempco2-0.0.5.tar` & `gtempco2-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-07-28 08:28:28.573273 gtempco2-0.0.5/
--rw-r--r--   0 yt        (1000) yt        (1000)     1780 2023-07-28 08:28:28.571935 gtempco2-0.0.5/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     1249 2023-06-12 04:59:29.000000 gtempco2-0.0.5/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-07-28 08:28:28.573273 gtempco2-0.0.5/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      951 2023-07-28 08:25:28.000000 gtempco2-0.0.5/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-07-28 08:28:28.565485 gtempco2-0.0.5/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-07-28 08:28:28.570938 gtempco2-0.0.5/src/gtempco2.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1780 2023-07-28 08:28:28.000000 gtempco2-0.0.5/src/gtempco2.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      217 2023-07-28 08:28:28.000000 gtempco2-0.0.5/src/gtempco2.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-07-28 08:28:28.000000 gtempco2-0.0.5/src/gtempco2.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       44 2023-07-28 08:28:28.000000 gtempco2-0.0.5/src/gtempco2.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        9 2023-07-28 08:28:28.000000 gtempco2-0.0.5/src/gtempco2.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     3013 2023-07-28 08:23:57.000000 gtempco2-0.0.5/src/gtempco2.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-07-28 08:46:43.016628 gtempco2-0.0.6/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1780 2023-07-28 08:46:43.015627 gtempco2-0.0.6/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)     1249 2023-06-12 04:59:29.000000 gtempco2-0.0.6/README.md
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-07-28 08:46:43.016628 gtempco2-0.0.6/setup.cfg
+-rw-r--r--   0 yt        (1000) yt        (1000)      951 2023-07-28 08:45:51.000000 gtempco2-0.0.6/setup.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-07-28 08:46:43.005072 gtempco2-0.0.6/src/
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-07-28 08:46:43.015627 gtempco2-0.0.6/src/gtempco2.egg-info/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1780 2023-07-28 08:46:42.000000 gtempco2-0.0.6/src/gtempco2.egg-info/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      217 2023-07-28 08:46:42.000000 gtempco2-0.0.6/src/gtempco2.egg-info/SOURCES.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-07-28 08:46:42.000000 gtempco2-0.0.6/src/gtempco2.egg-info/dependency_links.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       44 2023-07-28 08:46:42.000000 gtempco2-0.0.6/src/gtempco2.egg-info/entry_points.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        9 2023-07-28 08:46:42.000000 gtempco2-0.0.6/src/gtempco2.egg-info/top_level.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)     3084 2023-07-28 08:40:40.000000 gtempco2-0.0.6/src/gtempco2.py
```

### Comparing `gtempco2-0.0.5/PKG-INFO` & `gtempco2-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtempco2
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for displaying global temperature and co2
 Home-page: https://github.com/ytakefuji/gtempco2
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/gtempco2
 Platform: UNKNOWN
```

### Comparing `gtempco2-0.0.5/README.md` & `gtempco2-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `gtempco2-0.0.5/setup.py` & `gtempco2-0.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gtempco2",
-    version="0.0.5",
+    version="0.0.6",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for displaying global temperature and co2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/gtempco2",
     project_urls={
```

### Comparing `gtempco2-0.0.5/src/gtempco2.egg-info/PKG-INFO` & `gtempco2-0.0.6/src/gtempco2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtempco2
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for displaying global temperature and co2
 Home-page: https://github.com/ytakefuji/gtempco2
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/gtempco2
 Platform: UNKNOWN
```

### Comparing `gtempco2-0.0.5/src/gtempco2.py` & `gtempco2-0.0.6/src/gtempco2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.ticker import MaxNLocator
 from scipy import stats
 import subprocess as sp
+import warnings
+warnings.filterwarnings('ignore', category=UserWarning)
 
 def main():
  import requests
  from bs4 import BeautifulSoup
  url = 'https://www.ncei.noaa.gov/data/noaa-global-surface-temperature/v5.1/access/timeseries/'
  response = requests.get(url)
  soup = BeautifulSoup(response.text, 'html.parser')
@@ -16,15 +18,15 @@
     href = link.get('href')
     if href and 'aravg.mon.land_ocean.90S.90N' in href:
      filenm=href
  print(url+filenm)
  print('enter start_date: e.g. 1960-04')
  print('co2 measurement started from 1958-03')
  start=input('yyyy-mo: ')
- print('enter end_date: e.g. 2023-04')
+ print('enter end_date: e.g. 2023-06')
  end=input('yyyy-mo: ')
  print('start_date=',start,'end_date=',end)
  sp.call(f'wget -nc {url+filenm}', shell=True)
  d=pd.read_csv(filenm,sep='\\s+',header=None)
  d=d.iloc[:, :3]
  d.to_csv('noaa.csv',index=False)
  noaa = pd.read_csv('noaa.csv',comment='#')
@@ -69,14 +71,13 @@
  x = np.arange(len(noaa))
  slope, intercept, r_value, p_value, std_err = stats.linregress(x, noaa['change'])
  ax2.plot(noaa['date'].values, intercept + slope * x, 'r', label=f'Temperature Anomaly: y={slope:.3f}x+{intercept:.3f}, R^2={r_value**2:.3f}')
  ax2.legend(loc='lower right')
  
  ax1.xaxis.set_major_locator(MaxNLocator(7))
  ax1.set_xticklabels(ax1.get_xticklabels(), rotation=90)
- 
  fig.tight_layout()
  plt.savefig(start+'_'+end+'.png',dpi=300,bbox_inches='tight')
  plt.show()
  
 if __name__ == "__main__":
      main()
```


# Comparing `tmp/neoscr-2.1.0.tar.gz` & `tmp/neoscr-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neoscr-2.1.0.tar", last modified: Thu Jul 27 20:00:49 2023, max compression
+gzip compressed data, was "neoscr-2.1.1.tar", last modified: Fri Jul 28 12:46:33 2023, max compression
```

## Comparing `neoscr-2.1.0.tar` & `neoscr-2.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-07-27 20:00:49.580377 neoscr-2.1.0/
--rw-rw-r--   0 joaonogueira   (501) staff       (20)    11337 2023-01-20 02:50:04.000000 neoscr-2.1.0/LICENSE
--rw-rw-r--   0 joaonogueira   (501) staff       (20)      111 2023-01-20 02:50:04.000000 neoscr-2.1.0/MANIFEST.in
--rw-r--r--   0 joaonogueira   (501) staff       (20)     4752 2023-07-27 20:00:49.580204 neoscr-2.1.0/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)     3958 2023-07-27 19:54:52.000000 neoscr-2.1.0/README.md
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-07-27 20:00:49.578327 neoscr-2.1.0/neoscr/
--rw-r--r--   0 joaonogueira   (501) staff       (20)       22 2023-07-27 19:55:21.000000 neoscr-2.1.0/neoscr/__init__.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)     2339 2023-07-27 19:55:21.000000 neoscr-2.1.0/neoscr/_modidx.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)     2024 2023-07-27 19:55:21.000000 neoscr-2.1.0/neoscr/cli.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)     8431 2023-07-27 19:55:21.000000 neoscr-2.1.0/neoscr/core.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)     3773 2023-07-27 19:55:21.000000 neoscr-2.1.0/neoscr/utils.py
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-07-27 20:00:49.579985 neoscr-2.1.0/neoscr.egg-info/
--rw-r--r--   0 joaonogueira   (501) staff       (20)     4752 2023-07-27 20:00:49.000000 neoscr-2.1.0/neoscr.egg-info/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)      344 2023-07-27 20:00:49.000000 neoscr-2.1.0/neoscr.egg-info/SOURCES.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-07-27 20:00:49.000000 neoscr-2.1.0/neoscr.egg-info/dependency_links.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)      173 2023-07-27 20:00:49.000000 neoscr-2.1.0/neoscr.egg-info/entry_points.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-03-10 22:07:48.000000 neoscr-2.1.0/neoscr.egg-info/not-zip-safe
--rw-r--r--   0 joaonogueira   (501) staff       (20)       46 2023-07-27 20:00:49.000000 neoscr-2.1.0/neoscr.egg-info/requires.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        7 2023-07-27 20:00:49.000000 neoscr-2.1.0/neoscr.egg-info/top_level.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)      999 2023-07-27 19:55:21.000000 neoscr-2.1.0/settings.ini
--rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-07-27 20:00:49.580440 neoscr-2.1.0/setup.cfg
--rw-rw-r--   0 joaonogueira   (501) staff       (20)     2560 2023-01-20 02:50:04.000000 neoscr-2.1.0/setup.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-07-28 12:46:33.359003 neoscr-2.1.1/
+-rw-rw-r--   0 joaonogueira   (501) staff       (20)    11337 2023-01-20 02:50:04.000000 neoscr-2.1.1/LICENSE
+-rw-rw-r--   0 joaonogueira   (501) staff       (20)      111 2023-01-20 02:50:04.000000 neoscr-2.1.1/MANIFEST.in
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     4752 2023-07-28 12:46:33.358833 neoscr-2.1.1/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     3958 2023-07-28 12:43:32.000000 neoscr-2.1.1/README.md
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-07-28 12:46:33.356762 neoscr-2.1.1/neoscr/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       22 2023-07-28 12:44:57.000000 neoscr-2.1.1/neoscr/__init__.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     2339 2023-07-28 12:44:57.000000 neoscr-2.1.1/neoscr/_modidx.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     2024 2023-07-28 12:44:57.000000 neoscr-2.1.1/neoscr/cli.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     8903 2023-07-28 12:44:57.000000 neoscr-2.1.1/neoscr/core.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     3773 2023-07-28 12:44:57.000000 neoscr-2.1.1/neoscr/utils.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-07-28 12:46:33.358573 neoscr-2.1.1/neoscr.egg-info/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     4752 2023-07-28 12:46:33.000000 neoscr-2.1.1/neoscr.egg-info/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      344 2023-07-28 12:46:33.000000 neoscr-2.1.1/neoscr.egg-info/SOURCES.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-07-28 12:46:33.000000 neoscr-2.1.1/neoscr.egg-info/dependency_links.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      173 2023-07-28 12:46:33.000000 neoscr-2.1.1/neoscr.egg-info/entry_points.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-03-10 22:07:48.000000 neoscr-2.1.1/neoscr.egg-info/not-zip-safe
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       46 2023-07-28 12:46:33.000000 neoscr-2.1.1/neoscr.egg-info/requires.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        7 2023-07-28 12:46:33.000000 neoscr-2.1.1/neoscr.egg-info/top_level.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      999 2023-07-28 12:44:57.000000 neoscr-2.1.1/settings.ini
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-07-28 12:46:33.359062 neoscr-2.1.1/setup.cfg
+-rw-rw-r--   0 joaonogueira   (501) staff       (20)     2560 2023-01-20 02:50:04.000000 neoscr-2.1.1/setup.py
```

### Comparing `neoscr-2.1.0/LICENSE` & `neoscr-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neoscr-2.1.0/PKG-INFO` & `neoscr-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neoscr
-Version: 2.1.0
+Version: 2.1.1
 Summary: Wrapper to query the SCR api
 Home-page: https://github.com/datarisk-io/neoscr
 Author: João Nogueira
 Author-email: joao.nogueira@datarisk.io
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `neoscr-2.1.0/README.md` & `neoscr-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `neoscr-2.1.0/neoscr/_modidx.py` & `neoscr-2.1.1/neoscr/_modidx.py`

 * *Files identical despite different names*

### Comparing `neoscr-2.1.0/neoscr/cli.py` & `neoscr-2.1.1/neoscr/cli.py`

 * *Files identical despite different names*

### Comparing `neoscr-2.1.0/neoscr/core.py` & `neoscr-2.1.1/neoscr/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -137,14 +137,17 @@
     ) -> Tuple[pd.DataFrame, pd.DataFrame]:
         "Query CPFs and return a tuple of DataFrames: (df_cpf_resumo_cliente_traduzido, df_cpf_resumo_modalidade)"
         
         data_consulta = datetime.today().strftime("%d/%m/%Y")
         response_json = self._request(cpf, ano, mes)
         if response_json.get("Erro"):
             raise Exception(response_json.get("Msg").strip() + f": {cpf}")
+        if response_json.get("MensagemOperador") == '(50) - Cliente não possui dados no SCR na data-base.':
+            print(f"Cliente não possui dados no SCR na data-base: {cnpj}")
+            return None, None, None
         
         df_traduzido = self._get_resumo_cliente_traduzido(response_json, doc=cpf, data_consulta=data_consulta, mes_referencia=f"{ano}{mes:02d}")
         df_modalidade = self._get_resumo_modalidade(response_json, doc=cpf, data_consulta=data_consulta, mes_referencia=f"{ano}{mes:02d}")
         df_resumo_lista_das_operacoes = self._get_resumo_lista_das_operacoes(response_json, doc=cpf, data_consulta=data_consulta, mes_referencia=f"{ano}{mes:02d}")
         
         return df_traduzido, df_modalidade, df_resumo_lista_das_operacoes
 
@@ -155,13 +158,16 @@
                       mes: int       # Month to be consulted. Ex: 8, 10
     ) -> Tuple[pd.DataFrame, pd.DataFrame]:
         "Query CNPJs and return a tuple of DataFrames: (df_cnpj_resumo_cliente_traduzido, df_cnpj_resumo_modalidade)"
         data_consulta = datetime.today().strftime("%d/%m/%Y")
         response_json = self._request(cnpj, ano, mes)
         if response_json.get("Erro"):
             raise Exception(response_json.get("Msg").strip() + f": {cnpj}")
+        if response_json.get("MensagemOperador") == '(50) - Cliente não possui dados no SCR na data-base.':
+            print(f"Cliente não possui dados no SCR na data-base: {cnpj}")
+            return pd.DataFrame(), pd.DataFrame(), pd.DataFrame()
         
         df_traduzido = self._get_resumo_cliente_traduzido(response_json, doc=cnpj, data_consulta=data_consulta, mes_referencia=f"{ano}{mes:02d}")
         df_modalidade = self._get_resumo_modalidade(response_json, doc=cnpj, data_consulta=data_consulta, mes_referencia=f"{ano}{mes:02d}")
         df_resumo_lista_das_operacoes = self._get_resumo_lista_das_operacoes(response_json, doc=cnpj, data_consulta=data_consulta, mes_referencia=f"{ano}{mes:02d}")
 
         return df_traduzido, df_modalidade, df_resumo_lista_das_operacoes
```

### Comparing `neoscr-2.1.0/neoscr/utils.py` & `neoscr-2.1.1/neoscr/utils.py`

 * *Files identical despite different names*

### Comparing `neoscr-2.1.0/neoscr.egg-info/PKG-INFO` & `neoscr-2.1.1/neoscr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neoscr
-Version: 2.1.0
+Version: 2.1.1
 Summary: Wrapper to query the SCR api
 Home-page: https://github.com/datarisk-io/neoscr
 Author: João Nogueira
 Author-email: joao.nogueira@datarisk.io
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `neoscr-2.1.0/settings.ini` & `neoscr-2.1.1/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = neoscr
 lib_name = neoscr
-version = 2.1.0
+version = 2.1.1
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = neoscr
 nbs_path = nbs
 recursive = True
```

### Comparing `neoscr-2.1.0/setup.py` & `neoscr-2.1.1/setup.py`

 * *Files identical despite different names*


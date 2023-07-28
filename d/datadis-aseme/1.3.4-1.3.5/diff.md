# Comparing `tmp/datadis-aseme-1.3.4.tar.gz` & `tmp/datadis-aseme-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadis-aseme-1.3.4.tar", last modified: Tue Apr 25 10:59:53 2023, max compression
+gzip compressed data, was "dist/datadis-aseme-1.3.5.tar", last modified: Fri Jul 28 10:18:20 2023, max compression
```

## Comparing `datadis-aseme-1.3.4.tar` & `datadis-aseme-1.3.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-25 10:59:53.372600 datadis-aseme-1.3.4/
--rw-rw-r--   0 david     (1000) david     (1000)     1516 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)      119 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     1549 2023-04-25 10:59:53.372600 datadis-aseme-1.3.4/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1231 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-25 10:59:53.372600 datadis-aseme-1.3.4/datadis/
--rw-rw-r--   0 david     (1000) david     (1000)       75 2023-04-25 10:55:31.000000 datadis-aseme-1.3.4/datadis/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4373 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/datadis/adaptors.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-25 10:59:53.372600 datadis-aseme-1.3.4/datadis/data/
--rw-rw-r--   0 david     (1000) david     (1000)   216244 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/datadis/data/20codmun.csv
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-25 10:59:53.372600 datadis-aseme-1.3.4/datadis/templates/
--rw-rw-r--   0 david     (1000) david     (1000)      125 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/datadis/templates/autoconsumo.json
--rw-rw-r--   0 david     (1000) david     (1000)      440 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/datadis/templates/codigos_error.error
--rw-rw-r--   0 david     (1000) david     (1000)      532 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/datadis/templates/contrato.json
--rw-rw-r--   0 david     (1000) david     (1000)       35 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/datadis/templates/maximaspotencia.json
--rw-rw-r--   0 david     (1000) david     (1000)     5273 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/datadis/validators.py
--rw-rw-r--   0 david     (1000) david     (1000)     9839 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/datadis/webservice.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-25 10:59:53.372600 datadis-aseme-1.3.4/datadis_aseme.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     1549 2023-04-25 10:59:53.000000 datadis-aseme-1.3.4/datadis_aseme.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      493 2023-04-25 10:59:53.000000 datadis-aseme-1.3.4/datadis_aseme.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-04-25 10:59:53.000000 datadis-aseme-1.3.4/datadis_aseme.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)        9 2023-04-25 10:59:53.000000 datadis-aseme-1.3.4/datadis_aseme.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        8 2023-04-25 10:59:53.000000 datadis-aseme-1.3.4/datadis_aseme.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)        8 2022-11-15 17:50:53.000000 datadis-aseme-1.3.4/requirements.txt
--rw-rw-r--   0 david     (1000) david     (1000)       38 2023-04-25 10:59:53.372600 datadis-aseme-1.3.4/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)      841 2023-04-25 10:55:20.000000 datadis-aseme-1.3.4/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-28 10:18:20.000000 datadis-aseme-1.3.5/
+-rw-rw-r--   0 david     (1000) david     (1000)     1231 2022-11-15 17:50:53.000000 datadis-aseme-1.3.5/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)      119 2022-11-15 17:50:53.000000 datadis-aseme-1.3.5/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)     1926 2023-07-28 10:18:20.000000 datadis-aseme-1.3.5/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     1516 2022-11-15 17:50:53.000000 datadis-aseme-1.3.5/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)      841 2023-04-25 10:55:20.000000 datadis-aseme-1.3.5/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-28 10:18:20.000000 datadis-aseme-1.3.5/datadis/
+-rw-rw-r--   0 david     (1000) david     (1000)     9839 2022-11-15 17:50:53.000000 datadis-aseme-1.3.5/datadis/webservice.py
+-rw-rw-r--   0 david     (1000) david     (1000)       75 2023-07-28 10:14:57.000000 datadis-aseme-1.3.5/datadis/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-28 10:18:20.000000 datadis-aseme-1.3.5/datadis/data/
+-rw-rw-r--   0 david     (1000) david     (1000)   216244 2022-11-15 17:50:53.000000 datadis-aseme-1.3.5/datadis/data/20codmun.csv
+-rw-rw-r--   0 david     (1000) david     (1000)     6609 2023-07-28 10:14:33.000000 datadis-aseme-1.3.5/datadis/validators.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-28 10:18:20.000000 datadis-aseme-1.3.5/datadis/templates/
+-rw-rw-r--   0 david     (1000) david     (1000)       35 2022-11-15 17:50:53.000000 datadis-aseme-1.3.5/datadis/templates/maximaspotencia.json
+-rw-rw-r--   0 david     (1000) david     (1000)      244 2023-07-28 10:14:33.000000 datadis-aseme-1.3.5/datadis/templates/autoconsumo.json
+-rw-rw-r--   0 david     (1000) david     (1000)      532 2022-11-15 17:50:53.000000 datadis-aseme-1.3.5/datadis/templates/contrato.json
+-rw-rw-r--   0 david     (1000) david     (1000)      440 2022-11-15 17:50:53.000000 datadis-aseme-1.3.5/datadis/templates/codigos_error.error
+-rw-rw-r--   0 david     (1000) david     (1000)     4513 2023-07-28 10:14:33.000000 datadis-aseme-1.3.5/datadis/adaptors.py
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2022-11-15 17:50:53.000000 datadis-aseme-1.3.5/requirements.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-07-28 10:18:20.000000 datadis-aseme-1.3.5/setup.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-28 10:18:20.000000 datadis-aseme-1.3.5/datadis_aseme.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     1926 2023-07-28 10:18:20.000000 datadis-aseme-1.3.5/datadis_aseme.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-07-28 10:18:20.000000 datadis-aseme-1.3.5/datadis_aseme.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        9 2023-07-28 10:18:20.000000 datadis-aseme-1.3.5/datadis_aseme.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2023-07-28 10:18:20.000000 datadis-aseme-1.3.5/datadis_aseme.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      493 2023-07-28 10:18:20.000000 datadis-aseme-1.3.5/datadis_aseme.egg-info/SOURCES.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `datadis-aseme-1.3.4/LICENSE` & `datadis-aseme-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datadis-aseme-1.3.4/PKG-INFO` & `datadis-aseme-1.3.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 Metadata-Version: 2.1
 Name: datadis-aseme
-Version: 1.3.4
+Version: 1.3.5
 Summary: Herramienta gestión API ASEME DATADIS
 Home-page: https://github.com/gisce/datadis-aseme
 Author: Francesc Puig
 Author-email: devel@gisce.net
 License: BSD 3-Clause License
+Description: ## Herramienta para facilitar la interactividad con el WebService del sistema DATADIS
+        - Publicación de datos de distribuidora al sistema DATADIS
+        - Gestión de peticiones
+        
+        
+        ### Informaciones de:
+        
+        - Contrato
+        - Máximas potencia
+        - AUtoconsumo
+        
+        
+        ### Fácil de utilizar
+        
+        ```python
+        from datadis.webservice import DatadisWebServiceController
+        controller = DatadisWebserviceController()
+        controller.autenticar(usuario, password)
+        controller.contrato.__doc__
+        >>>
+        Publicar contrato al sistema DATADIS.
+                Si el contrato ya existe en el sistema, se modificara
+                Enviar un diccionario con las claves requeridas indicadas a continuacion
+                data: {
+                    "nif": "",
+                    "nombre": "",
+                    "comercializadora": "",
+                    "tensionConexion": "",
+                    "tarifaAcceso": "",
+                    "discriminacionHoraria": "",
+                    "tipoPunto": "",
+                    "modoControlPotencia": "",
+                    "fechaInicioContrato": "",
+                    "cups": "",
+                    "distribuidora": "",
+                    "codigoPostal": "",
+                    "provincia": "",
+                    "municipio": ""
+                }
+                method: 'POST' por defecto, utilizar 'DELETE' para eliminar contrato
+        
+        >>>
+        respuesta = controller.contrato(data)
+        ```
+        
+        
+        
+Platform: UNKNOWN
 Provides: datadis
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## Herramienta para facilitar la interactividad con el WebService del sistema DATADIS
-- Publicación de datos de distribuidora al sistema DATADIS
-- Gestión de peticiones
-
-
-### Informaciones de:
-
-- Contrato
-- Máximas potencia
-- AUtoconsumo
-
-
-### Fácil de utilizar
-
-```python
-from datadis.webservice import DatadisWebServiceController
-controller = DatadisWebserviceController()
-controller.autenticar(usuario, password)
-controller.contrato.__doc__
->>>
-Publicar contrato al sistema DATADIS.
-        Si el contrato ya existe en el sistema, se modificara
-        Enviar un diccionario con las claves requeridas indicadas a continuacion
-        data: {
-            "nif": "",
-            "nombre": "",
-            "comercializadora": "",
-            "tensionConexion": "",
-            "tarifaAcceso": "",
-            "discriminacionHoraria": "",
-            "tipoPunto": "",
-            "modoControlPotencia": "",
-            "fechaInicioContrato": "",
-            "cups": "",
-            "distribuidora": "",
-            "codigoPostal": "",
-            "provincia": "",
-            "municipio": ""
-        }
-        method: 'POST' por defecto, utilizar 'DELETE' para eliminar contrato
-
->>>
-respuesta = controller.contrato(data)
-```
-
-
```

### Comparing `datadis-aseme-1.3.4/README.md` & `datadis-aseme-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `datadis-aseme-1.3.4/datadis/adaptors.py` & `datadis-aseme-1.3.5/datadis/adaptors.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,16 @@
     'fechaInicioContrato', 'nif', 'nombre', 'cups', 'distribuidora', 'codigoPostal', 'provincia', 'municipio', 'CNAE'
 ]
 REQUIRED_MAXIMAS_POTENCIA_KEYS = [
     'medida', 'fecha', 'periodo'
 ]
 
 REQUIRED_AUTOCONSUMO_KEYS = [
-    'cau', 'tipoAutoConsumo', 'seccion', 'subseccion'
+    'cau', 'tipoAutoConsumo', 'seccion', 'subseccion',
+    'Tecnologia', 'Colectivo', 'InstalacionProximaRed', 'NoDisponeUnicoContratoSuministro'
 ]
 
 def adaptar_contrato(data):
     for key in REQUIRED_CONTRATO_KEYS:
         if key not in data:
             raise KeyError("Clave requerida {} no encontrada!".format(key))
     if len(str(data['municipio'])) != 3:
@@ -94,10 +95,11 @@
     for key in REQUIRED_AUTOCONSUMO_KEYS:
         if key not in data:
             raise KeyError("Clave requerida {} no encontrada!".format(key))
     data.update({
         'tipoAutoConsumo': str(data['tipoAutoConsumo']),
         'seccion': str(data['seccion']),
         'subseccion': str(data['subseccion'].lower()),
-        'potenciaInstaladaGeneracion': float(data['potenciaInstaladaGeneracion'])
+        'potenciaInstaladaGeneracion': float(data['potenciaInstaladaGeneracion']),
+        'Tecnologia': str(data['Tecnologia']),
     })
     return data
```

### Comparing `datadis-aseme-1.3.4/datadis/data/20codmun.csv` & `datadis-aseme-1.3.5/datadis/data/20codmun.csv`

 * *Files identical despite different names*

### Comparing `datadis-aseme-1.3.4/datadis/templates/contrato.json` & `datadis-aseme-1.3.5/datadis/templates/contrato.json`

 * *Files identical despite different names*

### Comparing `datadis-aseme-1.3.4/datadis/validators.py` & `datadis-aseme-1.3.5/datadis/validators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 from os import path
 
 CODIGOS_TARIFA = ['30', '31', '62', '63', '64', '65', '21', '2A', '6A', '2T', '3T', '3V', '6V']
 CODIGOS_TENSION = ['E0', 'E1', 'E2', 'E3', 'E4', 'E5', 'E6']
 CODIGOS_DH = ['G0', 'E3', 'E2', 'E1']
 CODIGOS_AUTOCONSUMO = ['31', '32', '33', '41', '42', '51', '52', '53', '54', '55', '56', '61', '62', '63', '64', '71', '72', '73', '74']
+CODIGOS_TECNOLOGIA = ['1', '2', '3', '4', '5', '6']
 
 def validar_contrato(data):
     if not isinstance(data, dict):
         raise Exception("El formato de datos debe ser un diccionario")
 
     validar_provincia(data['provincia'])
     validar_municipio(data['municipio'])
@@ -29,14 +30,18 @@
 def validar_autoconsumo(data):
     if not isinstance(data, dict):
         raise Exception("El formato de datos debe ser un diccionario")
 
     validar_cau(data['cau'])
     validar_tipo_autoconsumo(data['tipoAutoConsumo'])
     validar_seccion(data['seccion'])
+    validar_instalacion_proxima_a_red(data['InstalacionProximaRed'])
+    validar_tecnologia(data['Tecnologia'])
+    validar_colectivo(data['Colectivo'])
+    validar_no_dispone_unico_contrato_suministro(data['NoDisponeUnicoContratoSuministro'])
 
 def validar_provincia(provincia):
     provincias, municipios = read_provincias_municipios()
     if provincia not in provincias:
         raise Exception('El codigo provincia {} no existe en el INE'.format(provincia))
 
 def validar_municipio(municipio):
@@ -107,14 +112,34 @@
         raise Exception(
             "Seccion incorrecta {}: Solo se permite seccion 1 Sin excedentes o 2 Con excedentes".format(seccion))
 
 def validar_coeficiente_reparto(coeficiente_reparto):
     if not isinstance(coeficiente_reparto, (int, float)):
         raise TypeError("El formato de Coeficiente de reparto {} es incorrecto.".format(coeficiente_reparto))
 
+def validar_instalacion_proxima_a_red(instalacion_proxima_a_red):
+    if not isinstance(instalacion_proxima_a_red, bool):
+        raise TypeError("El formato de InstalacionProximaRed {} es incorrecto.".format(instalacion_proxima_a_red))
+
+def validar_tecnologia(tecnologia):
+    if not isinstance(tecnologia, str):
+        raise TypeError("El formato de Tecnologia {} es incorrecto.".format(tecnologia))
+    if tecnologia not in CODIGOS_TECNOLOGIA:
+        raise TypeError("Tecnologia {} no catalogada en las tablas -> {}".format(tecnologia, CODIGOS_TECNOLOGIA))
+
+def validar_colectivo(colectivo):
+    if not isinstance(colectivo, bool):
+        raise TypeError("El formato de Colectivo {} es incorrecto.".format(colectivo))
+
+def validar_no_dispone_unico_contrato_suministro(no_dispone_unico_contrato_suministro):
+    if not isinstance(no_dispone_unico_contrato_suministro, bool):
+        raise TypeError("El formato de NoDisponeUnicoContratoSuministro {} es incorrecto.".format(
+            no_dispone_unico_contrato_suministro)
+        )
+
 def read_provincias_municipios():
     import csv
     municipios = []
     provincias = []
     abs_route_fname = path.join(
         path.dirname(path.realpath(__file__)), 'data/20codmun.csv'
     )
```

### Comparing `datadis-aseme-1.3.4/datadis/webservice.py` & `datadis-aseme-1.3.5/datadis/webservice.py`

 * *Files identical despite different names*

### Comparing `datadis-aseme-1.3.4/datadis_aseme.egg-info/PKG-INFO` & `datadis-aseme-1.3.5/datadis_aseme.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 Metadata-Version: 2.1
 Name: datadis-aseme
-Version: 1.3.4
+Version: 1.3.5
 Summary: Herramienta gestión API ASEME DATADIS
 Home-page: https://github.com/gisce/datadis-aseme
 Author: Francesc Puig
 Author-email: devel@gisce.net
 License: BSD 3-Clause License
+Description: ## Herramienta para facilitar la interactividad con el WebService del sistema DATADIS
+        - Publicación de datos de distribuidora al sistema DATADIS
+        - Gestión de peticiones
+        
+        
+        ### Informaciones de:
+        
+        - Contrato
+        - Máximas potencia
+        - AUtoconsumo
+        
+        
+        ### Fácil de utilizar
+        
+        ```python
+        from datadis.webservice import DatadisWebServiceController
+        controller = DatadisWebserviceController()
+        controller.autenticar(usuario, password)
+        controller.contrato.__doc__
+        >>>
+        Publicar contrato al sistema DATADIS.
+                Si el contrato ya existe en el sistema, se modificara
+                Enviar un diccionario con las claves requeridas indicadas a continuacion
+                data: {
+                    "nif": "",
+                    "nombre": "",
+                    "comercializadora": "",
+                    "tensionConexion": "",
+                    "tarifaAcceso": "",
+                    "discriminacionHoraria": "",
+                    "tipoPunto": "",
+                    "modoControlPotencia": "",
+                    "fechaInicioContrato": "",
+                    "cups": "",
+                    "distribuidora": "",
+                    "codigoPostal": "",
+                    "provincia": "",
+                    "municipio": ""
+                }
+                method: 'POST' por defecto, utilizar 'DELETE' para eliminar contrato
+        
+        >>>
+        respuesta = controller.contrato(data)
+        ```
+        
+        
+        
+Platform: UNKNOWN
 Provides: datadis
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## Herramienta para facilitar la interactividad con el WebService del sistema DATADIS
-- Publicación de datos de distribuidora al sistema DATADIS
-- Gestión de peticiones
-
-
-### Informaciones de:
-
-- Contrato
-- Máximas potencia
-- AUtoconsumo
-
-
-### Fácil de utilizar
-
-```python
-from datadis.webservice import DatadisWebServiceController
-controller = DatadisWebserviceController()
-controller.autenticar(usuario, password)
-controller.contrato.__doc__
->>>
-Publicar contrato al sistema DATADIS.
-        Si el contrato ya existe en el sistema, se modificara
-        Enviar un diccionario con las claves requeridas indicadas a continuacion
-        data: {
-            "nif": "",
-            "nombre": "",
-            "comercializadora": "",
-            "tensionConexion": "",
-            "tarifaAcceso": "",
-            "discriminacionHoraria": "",
-            "tipoPunto": "",
-            "modoControlPotencia": "",
-            "fechaInicioContrato": "",
-            "cups": "",
-            "distribuidora": "",
-            "codigoPostal": "",
-            "provincia": "",
-            "municipio": ""
-        }
-        method: 'POST' por defecto, utilizar 'DELETE' para eliminar contrato
-
->>>
-respuesta = controller.contrato(data)
-```
-
-
```

### Comparing `datadis-aseme-1.3.4/setup.py` & `datadis-aseme-1.3.5/setup.py`

 * *Files identical despite different names*


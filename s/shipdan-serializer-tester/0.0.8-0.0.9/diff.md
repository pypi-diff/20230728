# Comparing `tmp/shipdan_serializer_tester-0.0.8.tar.gz` & `tmp/shipdan_serializer_tester-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipdan_serializer_tester-0.0.8.tar", last modified: Mon Jul 24 09:24:54 2023, max compression
+gzip compressed data, was "shipdan_serializer_tester-0.0.9.tar", last modified: Fri Jul 28 02:23:28 2023, max compression
```

## Comparing `shipdan_serializer_tester-0.0.8.tar` & `shipdan_serializer_tester-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 09:24:54.339825 shipdan_serializer_tester-0.0.8/
--rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-24 09:24:54.339686 shipdan_serializer_tester-0.0.8/PKG-INFO
--rw-r--r--   0 dare       (501) staff       (20)        0 2023-07-24 02:21:51.000000 shipdan_serializer_tester-0.0.8/README.md
--rw-r--r--   0 dare       (501) staff       (20)       38 2023-07-24 09:24:54.339865 shipdan_serializer_tester-0.0.8/setup.cfg
--rw-r--r--   0 dare       (501) staff       (20)      718 2023-07-24 09:24:27.000000 shipdan_serializer_tester-0.0.8/setup.py
-drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 09:24:54.338683 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester/
--rw-r--r--   0 dare       (501) staff       (20)       60 2023-07-24 09:24:27.000000 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester/__init__.py
--rw-r--r--   0 dare       (501) staff       (20)     2932 2023-07-24 09:24:27.000000 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester/model_serializer_tester.py
-drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-24 09:24:54.339509 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester.egg-info/
--rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-24 09:24:54.000000 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester.egg-info/PKG-INFO
--rw-r--r--   0 dare       (501) staff       (20)      401 2023-07-24 09:24:54.000000 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester.egg-info/SOURCES.txt
--rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-24 09:24:54.000000 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester.egg-info/dependency_links.txt
--rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-24 02:30:24.000000 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester.egg-info/not-zip-safe
--rw-r--r--   0 dare       (501) staff       (20)        7 2023-07-24 09:24:54.000000 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester.egg-info/requires.txt
--rw-r--r--   0 dare       (501) staff       (20)       26 2023-07-24 09:24:54.000000 shipdan_serializer_tester-0.0.8/shipdan_serializer_tester.egg-info/top_level.txt
+drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-28 02:23:28.228255 shipdan_serializer_tester-0.0.9/
+-rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-28 02:23:28.228119 shipdan_serializer_tester-0.0.9/PKG-INFO
+-rw-r--r--   0 dare       (501) staff       (20)        0 2023-07-24 02:21:51.000000 shipdan_serializer_tester-0.0.9/README.md
+-rw-r--r--   0 dare       (501) staff       (20)       38 2023-07-28 02:23:28.228295 shipdan_serializer_tester-0.0.9/setup.cfg
+-rw-r--r--   0 dare       (501) staff       (20)      718 2023-07-28 02:23:10.000000 shipdan_serializer_tester-0.0.9/setup.py
+drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-28 02:23:28.226959 shipdan_serializer_tester-0.0.9/shipdan_serializer_tester/
+-rw-r--r--   0 dare       (501) staff       (20)       60 2023-07-28 02:23:10.000000 shipdan_serializer_tester-0.0.9/shipdan_serializer_tester/__init__.py
+-rw-r--r--   0 dare       (501) staff       (20)     2932 2023-07-28 02:22:46.000000 shipdan_serializer_tester-0.0.9/shipdan_serializer_tester/model_serializer_tester.py
+drwxr-xr-x   0 dare       (501) staff       (20)        0 2023-07-28 02:23:28.227940 shipdan_serializer_tester-0.0.9/shipdan_serializer_tester.egg-info/
+-rw-r--r--   0 dare       (501) staff       (20)      490 2023-07-28 02:23:28.000000 shipdan_serializer_tester-0.0.9/shipdan_serializer_tester.egg-info/PKG-INFO
+-rw-r--r--   0 dare       (501) staff       (20)      401 2023-07-28 02:23:28.000000 shipdan_serializer_tester-0.0.9/shipdan_serializer_tester.egg-info/SOURCES.txt
+-rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-28 02:23:28.000000 shipdan_serializer_tester-0.0.9/shipdan_serializer_tester.egg-info/dependency_links.txt
+-rw-r--r--   0 dare       (501) staff       (20)        1 2023-07-28 02:23:28.000000 shipdan_serializer_tester-0.0.9/shipdan_serializer_tester.egg-info/not-zip-safe
+-rw-r--r--   0 dare       (501) staff       (20)        7 2023-07-28 02:23:28.000000 shipdan_serializer_tester-0.0.9/shipdan_serializer_tester.egg-info/requires.txt
+-rw-r--r--   0 dare       (501) staff       (20)       26 2023-07-28 02:23:28.000000 shipdan_serializer_tester-0.0.9/shipdan_serializer_tester.egg-info/top_level.txt
```

### Comparing `shipdan_serializer_tester-0.0.8/setup.py` & `shipdan_serializer_tester-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='shipdan_serializer_tester',
-    version='0.0.8',
+    version='0.0.9',
     description='for shipdan_application, shipdan_operation basic ModelSerializer field test',
     author='dare',
     author_email='gdare1999@gmail.com',
     url='https://github.com/G-D4R3/shipdan_serializer_tester.git',
     install_requires=['django',],
     packages=find_packages(exclude=[]),
     keywords=['dare', 'darever', 'bunkerkids', 'shipdan', 'pypi'],
```

### Comparing `shipdan_serializer_tester-0.0.8/shipdan_serializer_tester/model_serializer_tester.py` & `shipdan_serializer_tester-0.0.9/shipdan_serializer_tester/model_serializer_tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,21 +50,21 @@
                     raise cls.SerializerClassIsNotDefined(f'{model_name}Serializer가 정의되어있지 않습니다.')
 
                 instances = model_class.objects.all()[:10]
                 serializer = serializer_class(instances, many=True)
                 try:
                     serializer.data
                 except Exception as e:
-                    raise cls.FieldNameError(message=f'{model_name}Serializer FieldNameError: {e}')
+                    raise cls.FieldNameError(message=f'{model_name}Serializer FieldNameError, {e}')
 
                 model_fields = [f.name for f in filter(lambda f: f.related_model is None, \
                                                        [f for f in model_class._meta.get_fields()])]
                 serializer_fields = serializer_class.Meta.fields
 
                 if set(model_fields) != set(serializer_fields):
                     diff_at_model = set(model_fields).difference(set(serializer_fields))
                     diff_at_serializer = set(serializer_fields).difference(set(model_fields))
-                    raise cls.FieldDoesNotMatch(f'[{model_name}] model, serializer 간의 필드가 맞지 않음 \n    model: ',
-                                                diff_at_model, '\n    serializer', diff_at_serializer)
+                    raise cls.FieldDoesNotMatch(f'[{model_name}] model, serializer 간의 필드가 맞지 않음 \n    model=',
+                                                diff_at_model, '\n    serializer=', diff_at_serializer)
             except Exception as e:
-                raise cls.UnexpectedError(f'{model_name}: {e}')
+                raise cls.UnexpectedError(f'{model_name}, {e}')
         print("Success!!")
```


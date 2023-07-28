# Comparing `tmp/valcheck-1.1.tar.gz` & `tmp/valcheck-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valcheck-1.1.tar", last modified: Sat Jul 22 13:53:28 2023, max compression
+gzip compressed data, was "valcheck-1.2.tar", last modified: Fri Jul 28 18:00:00 2023, max compression
```

## Comparing `valcheck-1.1.tar` & `valcheck-1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 13:53:28.954332 valcheck-1.1/
--rw-rw-rw-   0        0        0     1087 2023-07-02 09:39:38.000000 valcheck-1.1/LICENSE
--rw-rw-rw-   0        0        0      758 2023-07-22 13:53:28.951338 valcheck-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1228 2023-07-22 13:50:59.000000 valcheck-1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-22 13:53:28.954332 valcheck-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1566 2023-07-22 13:50:59.000000 valcheck-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 13:53:28.935381 valcheck-1.1/valcheck/
--rw-rw-rw-   0        0        0        0 2023-07-02 09:39:38.000000 valcheck-1.1/valcheck/__init__.py
--rw-rw-rw-   0        0        0     1736 2023-07-21 18:09:50.000000 valcheck-1.1/valcheck/exceptions.py
--rw-rw-rw-   0        0        0    21939 2023-07-22 07:07:06.000000 valcheck-1.1/valcheck/fields.py
--rw-rw-rw-   0        0        0     2780 2023-07-21 03:21:34.000000 valcheck-1.1/valcheck/models.py
--rw-rw-rw-   0        0        0     3156 2023-07-16 07:09:18.000000 valcheck-1.1/valcheck/utils.py
--rw-rw-rw-   0        0        0     8621 2023-07-22 13:49:13.000000 valcheck-1.1/valcheck/validator.py
-drwxrwxrwx   0        0        0        0 2023-07-22 13:53:28.950341 valcheck-1.1/valcheck.egg-info/
--rw-rw-rw-   0        0        0      758 2023-07-22 13:53:28.000000 valcheck-1.1/valcheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-07-22 13:53:28.000000 valcheck-1.1/valcheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 13:53:28.000000 valcheck-1.1/valcheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-22 13:53:28.000000 valcheck-1.1/valcheck.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 18:00:00.607467 valcheck-1.2/
+-rw-rw-rw-   0        0        0     1087 2023-07-02 09:39:38.000000 valcheck-1.2/LICENSE
+-rw-rw-rw-   0        0        0      758 2023-07-28 18:00:00.605381 valcheck-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1228 2023-07-28 17:59:50.000000 valcheck-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-28 18:00:00.607467 valcheck-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1566 2023-07-28 17:59:50.000000 valcheck-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:00:00.582867 valcheck-1.2/valcheck/
+-rw-rw-rw-   0        0        0        0 2023-07-02 09:39:38.000000 valcheck-1.2/valcheck/__init__.py
+-rw-rw-rw-   0        0        0     1736 2023-07-21 18:09:50.000000 valcheck-1.2/valcheck/exceptions.py
+-rw-rw-rw-   0        0        0    22468 2023-07-28 17:59:50.000000 valcheck-1.2/valcheck/fields.py
+-rw-rw-rw-   0        0        0     2780 2023-07-21 03:21:34.000000 valcheck-1.2/valcheck/models.py
+-rw-rw-rw-   0        0        0     3156 2023-07-16 07:09:18.000000 valcheck-1.2/valcheck/utils.py
+-rw-rw-rw-   0        0        0     8621 2023-07-22 13:49:13.000000 valcheck-1.2/valcheck/validator.py
+drwxrwxrwx   0        0        0        0 2023-07-28 18:00:00.603388 valcheck-1.2/valcheck.egg-info/
+-rw-rw-rw-   0        0        0      758 2023-07-28 18:00:00.000000 valcheck-1.2/valcheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-07-28 18:00:00.000000 valcheck-1.2/valcheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 18:00:00.000000 valcheck-1.2/valcheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 18:00:00.000000 valcheck-1.2/valcheck.egg-info/top_level.txt
```

### Comparing `valcheck-1.1/LICENSE` & `valcheck-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `valcheck-1.1/PKG-INFO` & `valcheck-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valcheck
-Version: 1.1
+Version: 1.2
 Summary: Package for quick data validation (in Python)
 Home-page: https://github.com/Nishant173/valcheck
 Author: Nishant Rao
 Author-email: nishant.rao173@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `valcheck-1.1/README.md` & `valcheck-1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ```
 
 ## Usage
 - Refer to the `examples/` folder, based on the **valcheck** version you are using
 
 ## Performance benchmarks
 - On comparison of the performance of Django Rest Framework's (version 3.14.0) serializer with Valcheck's
-validator, we found that Valcheck (version 1.1) is ~3.8 times faster for cases where the data is
+validator, we found that Valcheck (version 1.2) is ~3.8 times faster for cases where the data is
 valid, and ~2.7 times faster for cases where the data is invalid.
 - These numbers are averaged over 25,000 iterations.
 
 ```python
 from rest_framework import serializers
 from valcheck import fields, models, validator
```

### Comparing `valcheck-1.1/setup.py` & `valcheck-1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import find_packages, setup
 
 # Constants
 PACKAGE_NAME = "valcheck"
-PACKAGE_VERSION = "1.1"
+PACKAGE_VERSION = "1.2"
 AUTHOR_NAME = "Nishant Rao"
 AUTHOR_EMAIL_ID = "nishant.rao173@gmail.com"
 FILEPATH_TO_README = os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md")
 FILEPATH_TO_REQUIREMENTS = os.path.join(os.path.abspath(os.path.dirname(__file__)), "requirements.txt")
 REPOSITORY_URL = "https://github.com/Nishant173/valcheck"
 
 # Requirements
```

### Comparing `valcheck-1.1/valcheck/exceptions.py` & `valcheck-1.2/valcheck/exceptions.py`

 * *Files identical despite different names*

### Comparing `valcheck-1.1/valcheck/fields.py` & `valcheck-1.2/valcheck/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
             f"is_valid={not bool(self.errors)}",
             f"field_identifier={utils.wrap_in_quotes_if_string(self.field.field_identifier)}",
             f"field_value={utils.wrap_in_quotes_if_string(self.field.field_value)}",
             f"source={utils.wrap_in_quotes_if_string(self.field.source)}",
             f"target={utils.wrap_in_quotes_if_string(self.field.target)}",
             f"required={self.field.required}",
             f"nullable={self.field.nullable}",
+            f"type_alias={utils.wrap_in_quotes_if_string(self.field.type_alias)}",
         ]
         kwargs_string = "(" + ", ".join(kwargs_list) + ")"
         return f"{self.__class__.__name__}{kwargs_string}"
 
     @property
     def field(self) -> Field:
         return self._field
@@ -67,28 +68,30 @@
             target: Optional[str] = None,
             required: Optional[bool] = True,
             nullable: Optional[bool] = False,
             default_factory: Optional[Callable] = None,
             converter_factory: Optional[Callable] = None,
             validators: Optional[List[Callable]] = None,
             error: Optional[Error] = None,
+            type_alias: Optional[str] = None,
         ) -> None:
         """
         Parameters:
             - source (str): Field name used in the input data (optional)
             - target (str): Field name used in the validated data (optional)
             - required (bool): True if the field is required, else False. Default: True
             - nullable (bool): True if the field is nullable, else False. Default: False
             - default_factory (callable): Callable that returns the default value to set for the field
             if `required=False` and the field is missing.
             - converter_factory (callable): Callable that takes in the validated value (of the field), and returns
             the converted value (for the field).
             - validators (list of callables): List of callables that each return a boolean (takes the field value as a param).
             The callable returns True if validation is successful, else False.
             - error (Error instance): Instance of type `valcheck.models.Error`.
+            - type_alias (str): Alias of the field type (optional).
         """
         assert source is None or utils.is_valid_object_of_type(source, type_=str, allow_empty=False), (
             "Param `source` must be of type 'str' and must be non-empty"
         )
         assert target is None or utils.is_valid_object_of_type(target, type_=str, allow_empty=False), (
             "Param `target` must be of type 'str' and must be non-empty"
         )
@@ -102,38 +105,43 @@
             " the converted value (for the field)."
         )
         assert validators is None or isinstance(validators, list), "Param `validators` must be of type 'list'"
         if isinstance(validators, list):
             for validator in validators:
                 assert callable(validator), "Param `validators` must be a list of callables"
         assert error is None or isinstance(error, Error), "Param `error` must be of type `valcheck.models.Error`"
+        assert type_alias is None or utils.is_valid_object_of_type(type_alias, type_=str, allow_empty=False), (
+            "Param `type_alias` must be of type 'str' and must be non-empty"
+        )
 
         self._field_identifier = utils.set_as_empty()
         self._field_value = utils.set_as_empty()
         self.source = source
         self.target = target
         self.required = required
         self.nullable = nullable
         self.default_factory = default_factory
         self.converter_factory = converter_factory
         self.validators = validators or []
         self.error = error or Error()
+        self.type_alias = type_alias or self.__class__.__name__
 
     def copy(self) -> Field:
         """Returns deep-copy of current `Field` object"""
         return copy.deepcopy(self)
 
     def __str__(self) -> str:
         kwargs_list = [
             f"field_identifier={utils.wrap_in_quotes_if_string(self.field_identifier)}",
             f"field_value={utils.wrap_in_quotes_if_string(self.field_value)}",
             f"source={utils.wrap_in_quotes_if_string(self.source)}",
             f"target={utils.wrap_in_quotes_if_string(self.target)}",
             f"required={self.required}",
             f"nullable={self.nullable}",
+            f"type_alias={utils.wrap_in_quotes_if_string(self.type_alias)}",
         ]
         kwargs_string = "(" + ", ".join(kwargs_list) + ")"
         return f"{self.__class__.__name__}{kwargs_string}"
 
     @property
     def field_identifier(self) -> str:
         return self._field_identifier
@@ -197,22 +205,22 @@
             return validated_field
         validated_field.field.field_value = self._convert_field_value_if_needed()
         return validated_field
 
     def invalid_field_error_message(self, *, prefix: Optional[str] = None, suffix: Optional[str] = None) -> str:
         return (
             f"{prefix if prefix else ''}"
-            f"Invalid {self.__class__.__name__} '{self.source}'"
+            f"Invalid {self.type_alias} '{self.source}'"
             f"{suffix if suffix else ''}"
         )
 
     def missing_field_error_message(self, *, prefix: Optional[str] = None, suffix: Optional[str] = None) -> str:
         return (
             f"{prefix if prefix else ''}"
-            f"Missing {self.__class__.__name__} '{self.source}'"
+            f"Missing {self.type_alias} '{self.source}'"
             f"{suffix if suffix else ''}"
         )
 
     def create_error_instance(self, *, validator_message: str) -> Error:
         """Creates and returns a new `valcheck.models.Error` instance for the field"""
         error_copy = self.error.copy()
         error_copy.validator_message = validator_message
```

### Comparing `valcheck-1.1/valcheck/models.py` & `valcheck-1.2/valcheck/models.py`

 * *Files identical despite different names*

### Comparing `valcheck-1.1/valcheck/utils.py` & `valcheck-1.2/valcheck/utils.py`

 * *Files identical despite different names*

### Comparing `valcheck-1.1/valcheck/validator.py` & `valcheck-1.2/valcheck/validator.py`

 * *Files identical despite different names*

### Comparing `valcheck-1.1/valcheck.egg-info/PKG-INFO` & `valcheck-1.2/valcheck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valcheck
-Version: 1.1
+Version: 1.2
 Summary: Package for quick data validation (in Python)
 Home-page: https://github.com/Nishant173/valcheck
 Author: Nishant Rao
 Author-email: nishant.rao173@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```


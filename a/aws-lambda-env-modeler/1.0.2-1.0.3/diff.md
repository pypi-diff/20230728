# Comparing `tmp/aws_lambda_env_modeler-1.0.2.tar.gz` & `tmp/aws_lambda_env_modeler-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_lambda_env_modeler-1.0.2.tar", max compression
+gzip compressed data, was "aws_lambda_env_modeler-1.0.3.tar", max compression
```

## Comparing `aws_lambda_env_modeler-1.0.2.tar` & `aws_lambda_env_modeler-1.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-15 21:17:59.659913 aws_lambda_env_modeler-1.0.2/LICENSE
--rw-r--r--   0        0        0     5030 2023-07-15 21:17:59.659913 aws_lambda_env_modeler-1.0.2/README.md
--rw-r--r--   0        0        0      281 2023-07-15 21:17:59.659913 aws_lambda_env_modeler-1.0.2/aws_lambda_env_modeler/__init__.py
--rw-r--r--   0        0        0     2377 2023-07-15 21:17:59.659913 aws_lambda_env_modeler-1.0.2/aws_lambda_env_modeler/modeler.py
--rw-r--r--   0        0        0        0 2023-07-15 21:17:59.659913 aws_lambda_env_modeler-1.0.2/aws_lambda_env_modeler/py.typed
--rw-r--r--   0        0        0      136 2023-07-15 21:17:59.659913 aws_lambda_env_modeler-1.0.2/aws_lambda_env_modeler/types.py
--rw-r--r--   0        0        0     1521 2023-07-15 21:17:59.663913 aws_lambda_env_modeler-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 aws_lambda_env_modeler-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-28 06:08:26.008182 aws_lambda_env_modeler-1.0.3/LICENSE
+-rw-r--r--   0        0        0     4861 2023-07-28 06:08:26.008182 aws_lambda_env_modeler-1.0.3/README.md
+-rw-r--r--   0        0        0      281 2023-07-28 06:08:26.008182 aws_lambda_env_modeler-1.0.3/aws_lambda_env_modeler/__init__.py
+-rw-r--r--   0        0        0     2377 2023-07-28 06:08:26.008182 aws_lambda_env_modeler-1.0.3/aws_lambda_env_modeler/modeler.py
+-rw-r--r--   0        0        0        0 2023-07-28 06:08:26.008182 aws_lambda_env_modeler-1.0.3/aws_lambda_env_modeler/py.typed
+-rw-r--r--   0        0        0      136 2023-07-28 06:08:26.008182 aws_lambda_env_modeler-1.0.3/aws_lambda_env_modeler/types.py
+-rw-r--r--   0        0        0     1631 2023-07-28 06:08:26.008182 aws_lambda_env_modeler-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6176 1970-01-01 00:00:00.000000 aws_lambda_env_modeler-1.0.3/PKG-INFO
```

### Comparing `aws_lambda_env_modeler-1.0.2/LICENSE` & `aws_lambda_env_modeler-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_lambda_env_modeler-1.0.2/README.md` & `aws_lambda_env_modeler-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 # AWS Lambda Environment Variables Modeler (Python)
 
 [![license](https://img.shields.io/github/license/ran-isenberg/aws-lambda-env-modeler)](https://github.com/ran-isenberg/aws-lambda-env-modeler/blob/master/LICENSE)
-![PythonSupport](https://img.shields.io/static/v1?label=python&message=3.8.1&color=blue?style=flat-square&logo=python)
-![PythonSupport](https://img.shields.io/static/v1?label=python&message=3.9&color=blue?style=flat-square&logo=python)
-![PythonSupport](https://img.shields.io/static/v1?label=python&message=3.10&color=blue?style=flat-square&logo=python)
+![PythonSupport](https://img.shields.io/static/v1?label=python&message=%203.8.17|%203.9|%203.10|%203.11&color=blue?style=flat-square&logo=python)
+![PyPI version](https://badge.fury.io/py/aws-lambda-env-modeler.svg)
+![PyPi monthly downloads](https://img.shields.io/pypi/dm/aws-lambda-env-modeler)
 [![codecov](https://codecov.io/gh/ran-isenberg/aws-lambda-env-modeler/branch/main/graph/badge.svg?token=P2K7K4KICF)](https://codecov.io/gh/ran-isenberg/aws-lambda-env-modeler)
 ![version](https://img.shields.io/github/v/release/ran-isenberg/aws-lambda-env-modeler)
-![github-star-badge](https://img.shields.io/github/stars/ran-isenberg/aws-lambda-env-modeler.svg?style=social)
 ![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/ran-isenberg/aws-lambda-env-modeler/badge)
 ![issues](https://img.shields.io/github/issues/ran-isenberg/aws-lambda-env-modeler)
 
 ![alt text](https://github.com/ran-isenberg/aws-lambda-env-modeler/blob/main/docs/media/banner.png?raw=true)
 
 AWS-Lambda-Env-Modeler is a Python library designed to simplify the process of managing and validating environment variables in your AWS Lambda functions.
```

### Comparing `aws_lambda_env_modeler-1.0.2/aws_lambda_env_modeler/modeler.py` & `aws_lambda_env_modeler-1.0.3/aws_lambda_env_modeler/modeler.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_env_modeler-1.0.2/pyproject.toml` & `aws_lambda_env_modeler-1.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 [tool.poetry]
 name = "aws_lambda_env_modeler"
-version = "1.0.2"
+version = "1.0.3"
 description = "AWS-Lambda-Env-Modeler is a Python library designed to simplify the process of managing and validating environment variables in your AWS Lambda functions."
 authors = ["Ran Isenberg"]
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 repository="https://github.com/ran-isenberg/aws-lambda-env-modeler"
 readme = "README.md"
-keywords = ["environment variables parser", "aws lambda", "serverless best practices", "aws serverless"]
+keywords = ["environment variables parser", "aws lambda", "serverless best practices", "aws serverless", "lambda environment variables"]
 license = "MIT-0"
 packages = [
     { include = "aws_lambda_env_modeler" }]
 
 [tool.poetry.urls]
 "Issue tracker" = "https://github.com/ran-isenberg/aws-lambda-env-modeler/issues"
 "Releases" = "https://github.com/ran-isenberg/aws-lambda-env-modeler/releases"
 
 
 [tool.poetry.dependencies]
-python = "^3.8.17"
+python = "^3.8.17 || ^3.9.0 || ^3.10.0 || ^3.11.0"
 pydantic = {version = "^2.0.0"}
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-mock = "*"
 pycodestyle = "*"
 pytest-cov = "*"
```

### Comparing `aws_lambda_env_modeler-1.0.2/PKG-INFO` & `aws_lambda_env_modeler-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: aws-lambda-env-modeler
-Version: 1.0.2
+Version: 1.0.3
 Summary: AWS-Lambda-Env-Modeler is a Python library designed to simplify the process of managing and validating environment variables in your AWS Lambda functions.
 Home-page: https://github.com/ran-isenberg/aws-lambda-env-modeler
 License: MIT-0
-Keywords: environment variables parser,aws lambda,serverless best practices,aws serverless
+Keywords: environment variables parser,aws lambda,serverless best practices,aws serverless,lambda environment variables
 Author: Ran Isenberg
 Requires-Python: >=3.8.17,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
@@ -23,20 +23,19 @@
 Project-URL: Releases, https://github.com/ran-isenberg/aws-lambda-env-modeler/releases
 Description-Content-Type: text/markdown
 
 
 # AWS Lambda Environment Variables Modeler (Python)
 
 [![license](https://img.shields.io/github/license/ran-isenberg/aws-lambda-env-modeler)](https://github.com/ran-isenberg/aws-lambda-env-modeler/blob/master/LICENSE)
-![PythonSupport](https://img.shields.io/static/v1?label=python&message=3.8.1&color=blue?style=flat-square&logo=python)
-![PythonSupport](https://img.shields.io/static/v1?label=python&message=3.9&color=blue?style=flat-square&logo=python)
-![PythonSupport](https://img.shields.io/static/v1?label=python&message=3.10&color=blue?style=flat-square&logo=python)
+![PythonSupport](https://img.shields.io/static/v1?label=python&message=%203.8.17|%203.9|%203.10|%203.11&color=blue?style=flat-square&logo=python)
+![PyPI version](https://badge.fury.io/py/aws-lambda-env-modeler.svg)
+![PyPi monthly downloads](https://img.shields.io/pypi/dm/aws-lambda-env-modeler)
 [![codecov](https://codecov.io/gh/ran-isenberg/aws-lambda-env-modeler/branch/main/graph/badge.svg?token=P2K7K4KICF)](https://codecov.io/gh/ran-isenberg/aws-lambda-env-modeler)
 ![version](https://img.shields.io/github/v/release/ran-isenberg/aws-lambda-env-modeler)
-![github-star-badge](https://img.shields.io/github/stars/ran-isenberg/aws-lambda-env-modeler.svg?style=social)
 ![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/ran-isenberg/aws-lambda-env-modeler/badge)
 ![issues](https://img.shields.io/github/issues/ran-isenberg/aws-lambda-env-modeler)
 
 ![alt text](https://github.com/ran-isenberg/aws-lambda-env-modeler/blob/main/docs/media/banner.png?raw=true)
 
 AWS-Lambda-Env-Modeler is a Python library designed to simplify the process of managing and validating environment variables in your AWS Lambda functions.
```


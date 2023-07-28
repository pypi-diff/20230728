# Comparing `tmp/AugmentedSocialScientist-2.0.0.tar.gz` & `tmp/AugmentedSocialScientist-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AugmentedSocialScientist-2.0.0.tar", last modified: Fri Jul 28 15:30:17 2023, max compression
+gzip compressed data, was "AugmentedSocialScientist-2.0.1.tar", last modified: Fri Jul 28 16:25:28 2023, max compression
```

## Comparing `AugmentedSocialScientist-2.0.0.tar` & `AugmentedSocialScientist-2.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-28 15:30:17.049722 AugmentedSocialScientist-2.0.0/
-drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-28 15:30:17.046973 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist/
--rw-r--r--   0 rubing     (501) staff       (20)      434 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist/__init__.py
--rw-r--r--   0 rubing     (501) staff       (20)     1221 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist/bert_abc.py
--rw-r--r--   0 rubing     (501) staff       (20)    19661 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist/bert_base.py
--rw-r--r--   0 rubing     (501) staff       (20)     4184 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist/models.py
-drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-28 15:30:17.049360 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist.egg-info/
--rw-r--r--   0 rubing     (501) staff       (20)     5723 2023-07-28 15:30:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist.egg-info/PKG-INFO
--rw-r--r--   0 rubing     (501) staff       (20)      469 2023-07-28 15:30:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist.egg-info/SOURCES.txt
--rw-r--r--   0 rubing     (501) staff       (20)        1 2023-07-28 15:30:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist.egg-info/dependency_links.txt
--rw-r--r--   0 rubing     (501) staff       (20)        1 2023-07-28 15:30:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist.egg-info/not-zip-safe
--rw-r--r--   0 rubing     (501) staff       (20)       63 2023-07-28 15:30:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist.egg-info/requires.txt
--rw-r--r--   0 rubing     (501) staff       (20)       25 2023-07-28 15:30:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist.egg-info/top_level.txt
--rw-r--r--   0 rubing     (501) staff       (20)     1068 2023-07-14 19:52:59.000000 AugmentedSocialScientist-2.0.0/LICENSE
--rw-r--r--   0 rubing     (501) staff       (20)     5723 2023-07-28 15:30:17.049900 AugmentedSocialScientist-2.0.0/PKG-INFO
--rw-r--r--   0 rubing     (501) staff       (20)     5257 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.0/README.md
--rw-r--r--   0 rubing     (501) staff       (20)       79 2023-07-28 15:30:17.050623 AugmentedSocialScientist-2.0.0/setup.cfg
--rw-r--r--   0 rubing     (501) staff       (20)      853 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.0/setup.py
+drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-28 16:25:28.732818 AugmentedSocialScientist-2.0.1/
+drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-28 16:25:28.729346 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist/
+-rw-r--r--   0 rubing     (501) staff       (20)      434 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist/__init__.py
+-rw-r--r--   0 rubing     (501) staff       (20)     1221 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist/bert_abc.py
+-rw-r--r--   0 rubing     (501) staff       (20)    19661 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist/bert_base.py
+-rw-r--r--   0 rubing     (501) staff       (20)     4604 2023-07-28 16:13:40.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist/models.py
+drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-28 16:25:28.732529 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist.egg-info/
+-rw-r--r--   0 rubing     (501) staff       (20)     5735 2023-07-28 16:25:27.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist.egg-info/PKG-INFO
+-rw-r--r--   0 rubing     (501) staff       (20)      469 2023-07-28 16:25:28.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist.egg-info/SOURCES.txt
+-rw-r--r--   0 rubing     (501) staff       (20)        1 2023-07-28 16:25:27.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist.egg-info/dependency_links.txt
+-rw-r--r--   0 rubing     (501) staff       (20)        1 2023-07-28 15:30:16.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist.egg-info/not-zip-safe
+-rw-r--r--   0 rubing     (501) staff       (20)       63 2023-07-28 16:25:28.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist.egg-info/requires.txt
+-rw-r--r--   0 rubing     (501) staff       (20)       25 2023-07-28 16:25:28.000000 AugmentedSocialScientist-2.0.1/AugmentedSocialScientist.egg-info/top_level.txt
+-rw-r--r--   0 rubing     (501) staff       (20)     1068 2023-07-14 19:52:59.000000 AugmentedSocialScientist-2.0.1/LICENSE
+-rw-r--r--   0 rubing     (501) staff       (20)     5735 2023-07-28 16:25:28.732951 AugmentedSocialScientist-2.0.1/PKG-INFO
+-rw-r--r--   0 rubing     (501) staff       (20)     5269 2023-07-28 16:21:34.000000 AugmentedSocialScientist-2.0.1/README.md
+-rw-r--r--   0 rubing     (501) staff       (20)       79 2023-07-28 16:25:28.733491 AugmentedSocialScientist-2.0.1/setup.cfg
+-rw-r--r--   0 rubing     (501) staff       (20)      853 2023-07-28 16:16:23.000000 AugmentedSocialScientist-2.0.1/setup.py
```

### Comparing `AugmentedSocialScientist-2.0.0/AugmentedSocialScientist/bert_abc.py` & `AugmentedSocialScientist-2.0.1/AugmentedSocialScientist/bert_abc.py`

 * *Files identical despite different names*

### Comparing `AugmentedSocialScientist-2.0.0/AugmentedSocialScientist/bert_base.py` & `AugmentedSocialScientist-2.0.1/AugmentedSocialScientist/bert_base.py`

 * *Files identical despite different names*

### Comparing `AugmentedSocialScientist-2.0.0/AugmentedSocialScientist/models.py` & `AugmentedSocialScientist-2.0.1/AugmentedSocialScientist/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,158 +5,170 @@
 
 from AugmentedSocialScientist.bert_base import BertBase
 
 
 class Bert(BertBase):
     def __init__(
             self,
+            model_name='bert-base-uncased',
             device=None
     ):
         super().__init__(
-            model_name='bert-base-uncased', 
+            model_name=model_name, 
             tokenizer=BertTokenizer,
             device=device,
             model_sequence_classifier=BertForSequenceClassification
         )
 
 
 class ArabicBert(BertBase):
     def __init__(
             self,
+            model_name="asafaya/bert-base-arabic",
             device=None
     ):
         super().__init__(
-            model_name="asafaya/bert-base-arabic",
+            model_name=model_name,
             tokenizer=BertTokenizer,
             device=device,
             model_sequence_classifier=BertForSequenceClassification
         )
 
 
 class Camembert(BertBase):
     def __init__(
             self,
+            model_name='camembert-base',
             device=None
     ):
         super().__init__(
-            model_name='camembert-base',
+            model_name=model_name,
             tokenizer=CamembertTokenizer,
             device=device,
             model_sequence_classifier=CamembertForSequenceClassification
         )
 
 
 class ChineseBert(BertBase):
     def __init__(
             self,
+            model_name="bert-base-chinese",
             device=None
     ):
         super().__init__(
-            model_name="bert-base-chinese",
+            model_name=model_name,
             tokenizer=BertTokenizer.from_pretrained("bert-base-chinese"),
             device=device,
             model_sequence_classifier=BertForSequenceClassification
         )
 
 
 class GermanBert(BertBase):
     def __init__(
             self,
+            model_name="dbmdz/bert-base-german-uncased",
             device=None
     ):
         super().__init__(
-            model_name="dbmdz/bert-base-german-uncased",
+            model_name=model_name,
             tokenizer=BertTokenizer,
             device=device,
             model_sequence_classifier=BertForSequenceClassification
         )
 
 
 class HindiBert(BertBase):
     def __init__(
             self,
+            model_name="monsoon-nlp/hindi-bert",
             device=None
     ):
         super().__init__(
-            model_name="monsoon-nlp/hindi-bert",
+            model_name=model_name,
             tokenizer=BertTokenizer,
             device=device,
             model_sequence_classifier=BertForSequenceClassification
         )
 
 
 class ItalianBert(BertBase):
     def __init__(
             self,
+            model_name="dbmdz/bert-base-italian-cased",
             device=None
     ):
         super().__init__(
-            model_name="dbmdz/bert-base-italian-cased",
+            model_name=model_name,
             tokenizer=BertTokenizer,
             device=device,
             model_sequence_classifier=BertForSequenceClassification
         )
 
 
 class PortugueseBert(BertBase):
     def __init__(
             self,
+            model_name='neuralmind/bert-base-portuguese-cased',
             device=None
     ):
         super().__init__(
-            model_name='neuralmind/bert-base-portuguese-cased',
+            model_name=model_name,
             tokenizer=BertTokenizer,
             device=device,
             model_sequence_classifier=BertForSequenceClassification
         )
 
 
 class RussianBert(BertBase):
     def __init__(
             self,
+            model_name="DeepPavlov/rubert-base-cased",
             device=None
     ):
         super().__init__(
-            model_name="DeepPavlov/rubert-base-cased",
+            model_name=model_name,
             tokenizer=BertTokenizer,
             device=device,
             model_sequence_classifier=BertForSequenceClassification
         )
 
 
 class SpanishBert(BertBase):
     def __init__(
             self,
+            model_name="dccuchile/bert-base-spanish-wwm-uncased",
             device=None
     ):
         super().__init__(
-            model_name="dccuchile/bert-base-spanish-wwm-uncased",
+            model_name=model_name,
             tokenizer=BertTokenizer,
             device=device,
             model_sequence_classifier=BertForSequenceClassification
         )
 
 
 class SwedishBert(BertBase):
     def __init__(
             self,
+            model_name='KB/bert-base-swedish-cased',
             device=None
     ):
         super().__init__(
-            model_name='KB/bert-base-swedish-cased',
+            model_name=model_name,
             tokenizer=BertTokenizer,
             device=device,
             model_sequence_classifier=BertForSequenceClassification
         )
 
 
 class XLMRoberta(BertBase):
     def __init__(
             self,
+            model_name='xlm-roberta-base',
             device=None
     ):
         super().__init__(
-            model_name='xlm-roberta-base',
+            model_name=model_name,
             tokenizer=XLMRobertaTokenizer,
             device=device,
             model_sequence_classifier=XLMRobertaForSequenceClassification
         )
```

### Comparing `AugmentedSocialScientist-2.0.0/AugmentedSocialScientist.egg-info/PKG-INFO` & `AugmentedSocialScientist-2.0.1/AugmentedSocialScientist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: AugmentedSocialScientist
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Package to Easily Train Bert-Like Models for Text Classification
 Home-page: https://github.com/rubingshen/AugmentedSocialScientist
-Download-URL: https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.0.0.tar.gz
+Download-URL: https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.0.1.tar.gz
 Author: Rubing Shen
 Author-email: shenrubing1996@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The Augmented Social Scientist
 
-**New release v2.0.0**
+**New release v2**
 
 This package makes it extremely easy to train BERT-like models for text classifications. 
 
 For more information on the method and for some use cases from social sciences, see "[The Augmented Social Scientist: Using Sequential Transfer Learning to Annotate Millions of Texts with Human-Level Accuracy](https://journals.sagepub.com/doi/abs/10.1177/00491241221134526)" published on *Sociological Methods & Research* by [Salomé Do](https://sally14.github.io), [Étienne Ollion](https://ollion.cnrs.fr/english/) and [Rubing Shen](https://rubingshen.github.io). 
 
 
 
@@ -134,15 +134,15 @@
 
 To use them, just import the corresponding model and instanciate it as in the previous example.
 
 For example, to use the French language model `Camembert`:
 ```python
 from AugmentedSocialScientist.models import Camembert
 
-bert = Camembert() #instanciation
+bert = Camembert()  #instanciation
 ```
 You can then use the functions `bert.encode()`, `bert.run_training()`, `bert.predict_with_model()` as in the previous example.
 
 ## To use a custom model from Hugging Face
 
 The package also allows you to use other BERT-like models from [Hugging Face](https://huggingface.co/models), by changing the argument `model_name` to the desired model name when instanciating the class `Bert`. 
 
@@ -150,16 +150,17 @@
 
 ```python
 from AugmentedSocialScientist.models import Bert
 
 bert = Bert(model_name="DJSammy/bert-base-danish-uncased_BotXO-ai")
 ``````
 
-## GPU acceleration
+## To use a custom `torch.Device`
 By default, the package automatically detects the presence of a GPU and uses it to accelerate computation. You can also set your own device, by providing a `torch.Device` object to the parameter `device` when instanciating `Bert`.
 
 ```python
 from AugmentedSocialScientist.models import Bert
 
 bert = Bert(device=...)  #set your own device
 ```
 
+
```

### Comparing `AugmentedSocialScientist-2.0.0/LICENSE` & `AugmentedSocialScientist-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AugmentedSocialScientist-2.0.0/PKG-INFO` & `AugmentedSocialScientist-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: AugmentedSocialScientist
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Package to Easily Train Bert-Like Models for Text Classification
 Home-page: https://github.com/rubingshen/AugmentedSocialScientist
-Download-URL: https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.0.0.tar.gz
+Download-URL: https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.0.1.tar.gz
 Author: Rubing Shen
 Author-email: shenrubing1996@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The Augmented Social Scientist
 
-**New release v2.0.0**
+**New release v2**
 
 This package makes it extremely easy to train BERT-like models for text classifications. 
 
 For more information on the method and for some use cases from social sciences, see "[The Augmented Social Scientist: Using Sequential Transfer Learning to Annotate Millions of Texts with Human-Level Accuracy](https://journals.sagepub.com/doi/abs/10.1177/00491241221134526)" published on *Sociological Methods & Research* by [Salomé Do](https://sally14.github.io), [Étienne Ollion](https://ollion.cnrs.fr/english/) and [Rubing Shen](https://rubingshen.github.io). 
 
 
 
@@ -134,15 +134,15 @@
 
 To use them, just import the corresponding model and instanciate it as in the previous example.
 
 For example, to use the French language model `Camembert`:
 ```python
 from AugmentedSocialScientist.models import Camembert
 
-bert = Camembert() #instanciation
+bert = Camembert()  #instanciation
 ```
 You can then use the functions `bert.encode()`, `bert.run_training()`, `bert.predict_with_model()` as in the previous example.
 
 ## To use a custom model from Hugging Face
 
 The package also allows you to use other BERT-like models from [Hugging Face](https://huggingface.co/models), by changing the argument `model_name` to the desired model name when instanciating the class `Bert`. 
 
@@ -150,16 +150,17 @@
 
 ```python
 from AugmentedSocialScientist.models import Bert
 
 bert = Bert(model_name="DJSammy/bert-base-danish-uncased_BotXO-ai")
 ``````
 
-## GPU acceleration
+## To use a custom `torch.Device`
 By default, the package automatically detects the presence of a GPU and uses it to accelerate computation. You can also set your own device, by providing a `torch.Device` object to the parameter `device` when instanciating `Bert`.
 
 ```python
 from AugmentedSocialScientist.models import Bert
 
 bert = Bert(device=...)  #set your own device
 ```
 
+
```

### Comparing `AugmentedSocialScientist-2.0.0/README.md` & `AugmentedSocialScientist-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # The Augmented Social Scientist
 
-**New release v2.0.0**
+**New release v2**
 
 This package makes it extremely easy to train BERT-like models for text classifications. 
 
 For more information on the method and for some use cases from social sciences, see "[The Augmented Social Scientist: Using Sequential Transfer Learning to Annotate Millions of Texts with Human-Level Accuracy](https://journals.sagepub.com/doi/abs/10.1177/00491241221134526)" published on *Sociological Methods & Research* by [Salomé Do](https://sally14.github.io), [Étienne Ollion](https://ollion.cnrs.fr/english/) and [Rubing Shen](https://rubingshen.github.io). 
 
 
 
@@ -121,15 +121,15 @@
 
 To use them, just import the corresponding model and instanciate it as in the previous example.
 
 For example, to use the French language model `Camembert`:
 ```python
 from AugmentedSocialScientist.models import Camembert
 
-bert = Camembert() #instanciation
+bert = Camembert()  #instanciation
 ```
 You can then use the functions `bert.encode()`, `bert.run_training()`, `bert.predict_with_model()` as in the previous example.
 
 ## To use a custom model from Hugging Face
 
 The package also allows you to use other BERT-like models from [Hugging Face](https://huggingface.co/models), by changing the argument `model_name` to the desired model name when instanciating the class `Bert`. 
 
@@ -137,15 +137,15 @@
 
 ```python
 from AugmentedSocialScientist.models import Bert
 
 bert = Bert(model_name="DJSammy/bert-base-danish-uncased_BotXO-ai")
 ``````
 
-## GPU acceleration
+## To use a custom `torch.Device`
 By default, the package automatically detects the presence of a GPU and uses it to accelerate computation. You can also set your own device, by providing a `torch.Device` object to the parameter `device` when instanciating `Bert`.
 
 ```python
 from AugmentedSocialScientist.models import Bert
 
 bert = Bert(device=...)  #set your own device
-```
+```
```

### Comparing `AugmentedSocialScientist-2.0.0/setup.py` & `AugmentedSocialScientist-2.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     long_description = fh.read()
     
 setup(name='AugmentedSocialScientist',
       author='Rubing Shen',
       license='MIT',
       author_email='shenrubing1996@gmail.com',
       url='https://github.com/rubingshen/AugmentedSocialScientist',
-      download_url='https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.0.0.tar.gz',
-      version='2.0.0',
+      download_url='https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.0.1.tar.gz',
+      version='2.0.1',
       description='A Package to Easily Train Bert-Like Models for Text Classification',
       long_description=long_description,
       long_description_content_type="text/markdown",
       packages=['AugmentedSocialScientist'],
       zip_safe=False,
       install_requires=environment)
```


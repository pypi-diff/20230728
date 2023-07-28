# Comparing `tmp/stressed_cyrillic_tools-0.1.8.tar.gz` & `tmp/stressed_cyrillic_tools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stressed_cyrillic_tools-0.1.8.tar", max compression
+gzip compressed data, was "stressed_cyrillic_tools-0.1.9.tar", max compression
```

## Comparing `stressed_cyrillic_tools-0.1.8.tar` & `stressed_cyrillic_tools-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35823 2022-06-13 12:39:09.254077 stressed_cyrillic_tools-0.1.8/LICENSE
--rw-r--r--   0        0        0      361 2022-10-23 12:59:40.793011 stressed_cyrillic_tools-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       45 2022-06-04 20:30:33.770549 stressed_cyrillic_tools-0.1.8/stressed_cyrillic_tools/__init__.py
--rw-r--r--   0        0        0     7155 2022-10-23 12:59:34.480060 stressed_cyrillic_tools-0.1.8/stressed_cyrillic_tools/tools.py
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 stressed_cyrillic_tools-0.1.8/setup.py
--rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 stressed_cyrillic_tools-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-06-13 12:39:09.254077 stressed_cyrillic_tools-0.1.9/LICENSE
+-rw-r--r--   0        0        0      361 2022-10-26 12:42:09.543623 stressed_cyrillic_tools-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       45 2022-06-04 20:30:33.770549 stressed_cyrillic_tools-0.1.9/stressed_cyrillic_tools/__init__.py
+-rw-r--r--   0        0        0     7275 2022-10-26 12:41:57.409528 stressed_cyrillic_tools-0.1.9/stressed_cyrillic_tools/tools.py
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 stressed_cyrillic_tools-0.1.9/setup.py
+-rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 stressed_cyrillic_tools-0.1.9/PKG-INFO
```

### Comparing `stressed_cyrillic_tools-0.1.8/LICENSE` & `stressed_cyrillic_tools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stressed_cyrillic_tools-0.1.8/stressed_cyrillic_tools/tools.py` & `stressed_cyrillic_tools-0.1.9/stressed_cyrillic_tools/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -180,29 +180,31 @@
 
         #return word
     else:
         # Keep the first acute accent and remove the rest
         word = word.split("\u0301")[0] + "\u0301" + "".join(word.split("\u0301")[1:])
         return word.replace("\u0300", "")
 
+WORDS_WITHOUT_STRESS = ["обо"]
 
 def is_unhelpfully_unstressed(word: str) -> bool:
     """Returns True if the word would be of no use in a stress dictionary. This filters out mostly unstressed words,
     but also words with one syllable where the stress is clear"""
 
     if " " in word:
         # Return True if all of the words in the phrase are unhelpfully unstressed
         return all(is_unhelpfully_unstressed(word) for word in word.split(" "))
 
+    # Check if word is in the list of words without stress
+    if word.lower() in WORDS_WITHOUT_STRESS:
+        return False
+
     if "ё" in word or "Ё" in word:
         return False
     if has_only_one_syllable(word):
         if "е" in word or "Е" in word:
             # The word лес tells us that it is not written like "лёс"
             return False
         else:
             # Words with only one syllable are never marked with an accent
             return True
     return not is_accented(word)
-
-
-print(has_two_stress_marks("зу̀б"))
```

### Comparing `stressed_cyrillic_tools-0.1.8/setup.py` & `stressed_cyrillic_tools-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['stressed_cyrillic_tools']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'stressed-cyrillic-tools',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': 'None',
     'author': 'Vuizur',
     'author_email': 'Vuizur@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```


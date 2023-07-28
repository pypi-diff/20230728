# Comparing `tmp/flynt-1.0.0.tar.gz` & `tmp/flynt-1.0.1.tar.gz`

## Comparing `flynt-1.0.0.tar` & `flynt-1.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/__init__.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/__main__.py
--rw-r--r--   0        0        0    10215 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/api.py
--rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/cli.py
--rw-r--r--   0        0        0     9634 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/code_editor.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/exceptions.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/candidates/__init__.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/candidates/ast_call_candidates.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/candidates/ast_chunk.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/candidates/ast_percent_candidates.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/linting/__init__.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/linting/fstr_lint.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/static_join/__init__.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/static_join/candidates.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/static_join/transformer.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/static_join/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/string_concat/__init__.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/string_concat/candidates.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/string_concat/string_in_string.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/string_concat/transformer.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/transform/FstringifyTransformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/transform/__init__.py
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/transform/format_call_transforms.py
--rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/transform/percent_transformer.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/transform/transform.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/transform/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/utils/__init__.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/utils/format.py
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/utils/pyproject_finder.py
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 flynt-1.0.0/src/flynt/utils/utils.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 flynt-1.0.0/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 flynt-1.0.0/LICENSE
--rw-r--r--   0        0        0     8319 2020-02-02 00:00:00.000000 flynt-1.0.0/README.md
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 flynt-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     9357 2020-02-02 00:00:00.000000 flynt-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/__init__.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/__main__.py
+-rw-r--r--   0        0        0    10215 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/api.py
+-rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/cli.py
+-rw-r--r--   0        0        0     9634 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/code_editor.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/exceptions.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/candidates/__init__.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/candidates/ast_call_candidates.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/candidates/ast_chunk.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/candidates/ast_percent_candidates.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/linting/__init__.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/linting/fstr_lint.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/static_join/__init__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/static_join/candidates.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/static_join/transformer.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/static_join/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/string_concat/__init__.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/string_concat/candidates.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/string_concat/string_in_string.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/string_concat/transformer.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/transform/FstringifyTransformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/transform/__init__.py
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/transform/format_call_transforms.py
+-rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/transform/percent_transformer.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/transform/transform.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/transform/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/utils/__init__.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/utils/format.py
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/utils/pyproject_finder.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 flynt-1.0.1/src/flynt/utils/utils.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 flynt-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 flynt-1.0.1/LICENSE
+-rw-r--r--   0        0        0     8319 2020-02-02 00:00:00.000000 flynt-1.0.1/README.md
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 flynt-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     9357 2020-02-02 00:00:00.000000 flynt-1.0.1/PKG-INFO
```

### Comparing `flynt-1.0.0/src/flynt/api.py` & `flynt-1.0.1/src/flynt/api.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/cli.py` & `flynt-1.0.1/src/flynt/cli.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/code_editor.py` & `flynt-1.0.1/src/flynt/code_editor.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/state.py` & `flynt-1.0.1/src/flynt/state.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/candidates/ast_call_candidates.py` & `flynt-1.0.1/src/flynt/candidates/ast_call_candidates.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/candidates/ast_chunk.py` & `flynt-1.0.1/src/flynt/candidates/ast_chunk.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/candidates/ast_percent_candidates.py` & `flynt-1.0.1/src/flynt/candidates/ast_percent_candidates.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/linting/fstr_lint.py` & `flynt-1.0.1/src/flynt/linting/fstr_lint.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/static_join/candidates.py` & `flynt-1.0.1/src/flynt/static_join/candidates.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/static_join/transformer.py` & `flynt-1.0.1/src/flynt/static_join/transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,10 +38,14 @@
             )
         return ast.JoinedStr(args_with_interleaved_joiner)
 
 
 def transform_join(tree: ast.AST, *args, **kwargs) -> Tuple[str, bool]:
 
     jt = JoinTransformer()
-    jt.visit(tree)
-    new_code = fixup_transformed(tree)
-    return new_code, jt.counter > 0
+    new_tree = jt.visit(tree)
+    changed = jt.counter > 0
+    if changed:
+        new_code = fixup_transformed(new_tree)
+    else:
+        new_code = ""
+    return new_code, changed
```

### Comparing `flynt-1.0.0/src/flynt/static_join/utils.py` & `flynt-1.0.1/src/flynt/static_join/utils.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/string_concat/candidates.py` & `flynt-1.0.1/src/flynt/string_concat/candidates.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/string_concat/string_in_string.py` & `flynt-1.0.1/src/flynt/string_concat/string_in_string.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/string_concat/transformer.py` & `flynt-1.0.1/src/flynt/string_concat/transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,10 +61,13 @@
         return ast.JoinedStr(segments)
 
 
 def transform_concat(tree: ast.AST, *args, **kwargs) -> Tuple[str, bool]:
 
     ft = ConcatTransformer()
     new = ft.visit(tree)
-    new_code = fixup_transformed(new)
-
-    return new_code, ft.counter > 0
+    changed = ft.counter > 0
+    if changed:
+        new_code = fixup_transformed(new)
+    else:
+        new_code = ""
+    return new_code, changed
```

### Comparing `flynt-1.0.0/src/flynt/transform/FstringifyTransformer.py` & `flynt-1.0.1/src/flynt/transform/FstringifyTransformer.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/transform/format_call_transforms.py` & `flynt-1.0.1/src/flynt/transform/format_call_transforms.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/transform/percent_transformer.py` & `flynt-1.0.1/src/flynt/transform/percent_transformer.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/transform/transform.py` & `flynt-1.0.1/src/flynt/transform/transform.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/transform/util.py` & `flynt-1.0.1/src/flynt/transform/util.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/utils/format.py` & `flynt-1.0.1/src/flynt/utils/format.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/utils/pyproject_finder.py` & `flynt-1.0.1/src/flynt/utils/pyproject_finder.py`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/src/flynt/utils/utils.py` & `flynt-1.0.1/src/flynt/utils/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -97,25 +97,37 @@
     )
 
 
 def ast_string_node(string: str) -> ast.Str:
     return ast.Str(s=string)
 
 
+def check_is_string_node(tree: ast.AST):
+    """Raise an exception is tree doesn't represent a string"""
+    if isinstance(tree, ast.Module):
+        tree = tree.body[0]
+    if isinstance(tree, ast.Expr):
+        tree = tree.value
+    assert isinstance(tree, (ast.JoinedStr, ast.Str)), f"found {type(tree)}"
+
+
 def fixup_transformed(tree: ast.AST, quote_type: Optional[str] = None) -> str:
+    """Given a transformed string / fstring ast node, transform it to a string."""
+    # check_is_string_node(tree)
     il = FstrInliner()
     il.visit(tree)
     new_code = ast_to_string(tree)
     if quote_type is None:
         if new_code[:4] == 'f"""' or new_code[:3] == "'''" or new_code[:3] == '"""':
             quote_type = QuoteTypes.double
     if quote_type is not None:
         new_code = set_quote_type(new_code, quote_type)
     new_code = new_code.replace("\n", "\\n")
     new_code = new_code.replace("\t", "\\t")
+    # ast.parse(new_code)
     return new_code
 
 
 def contains_comment(code: str) -> bool:
     tokens = tokenize.generate_tokens(io.StringIO(code).readline)
     for token in tokens:
         if token.type == tokenize.COMMENT:
```

### Comparing `flynt-1.0.0/LICENSE` & `flynt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/README.md` & `flynt-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `flynt-1.0.0/pyproject.toml` & `flynt-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 [tool.ruff.pylint]
 max-args = 7
 max-branches = 18
 max-statements = 67
 
 [tool.ruff.per-file-ignores]
-"test/*" = ["I"]
+"test/*" = ["I", "S"]
 "test/integration/*" = [
     "F523",
     "F821",
     "F841",
     "I",
  ]
 "test/test_lexer.py" = ["F841"]
```

### Comparing `flynt-1.0.0/PKG-INFO` & `flynt-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flynt
-Version: 1.0.0
+Version: 1.0.1
 Summary: CLI tool to convert a python project's %-formatted strings to f-strings.
 Project-URL: Homepage, https://github.com/ikamensh/flynt
 Author: Ilya Kamenshchikov
 License-Expression: MIT
 License-File: LICENSE
 Keywords: strings,utility
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flynt Version: 1.0.0 Summary: CLI tool to convert a
+Metadata-Version: 2.1 Name: flynt Version: 1.0.1 Summary: CLI tool to convert a
 python project's %-formatted strings to f-strings. Project-URL: Homepage,
 https://github.com/ikamensh/flynt Author: Ilya Kamenshchikov License-
 Expression: MIT License-File: LICENSE Keywords: strings,utility Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```


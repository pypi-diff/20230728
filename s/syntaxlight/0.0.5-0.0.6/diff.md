# Comparing `tmp/syntaxlight-0.0.5.tar.gz` & `tmp/syntaxlight-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntaxlight-0.0.5.tar", max compression
+gzip compressed data, was "syntaxlight-0.0.6.tar", max compression
```

## Comparing `syntaxlight-0.0.5.tar` & `syntaxlight-0.0.6.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.0.5/LICENSE
--rw-r--r--   0        0        0      464 2023-07-24 08:09:12.714704 syntaxlight-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2183 2023-07-22 12:55:46.842043 syntaxlight-0.0.5/README.md
--rw-r--r--   0        0        0      209 2023-07-23 11:29:29.575296 syntaxlight-0.0.5/syntaxlight/__init__.py
--rw-r--r--   0        0        0    14933 2023-07-24 07:57:41.164021 syntaxlight-0.0.5/syntaxlight/ast.py
--rw-r--r--   0        0        0     2223 2023-07-19 06:56:41.644931 syntaxlight-0.0.5/syntaxlight/css/all.css
--rw-r--r--   0        0        0      665 2023-07-22 15:03:22.184483 syntaxlight-0.0.5/syntaxlight/css/bnf.css
--rw-r--r--   0        0        0     2118 2023-07-23 15:21:29.646891 syntaxlight-0.0.5/syntaxlight/css/c.css
--rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.0.5/syntaxlight/css/index.css
--rw-r--r--   0        0        0      529 2023-07-21 12:50:35.868013 syntaxlight-0.0.5/syntaxlight/css/json.css
--rw-r--r--   0        0        0     2720 2023-07-20 08:04:28.110565 syntaxlight-0.0.5/syntaxlight/css/themes.json
--rw-r--r--   0        0        0      557 2023-07-19 08:11:34.232315 syntaxlight-0.0.5/syntaxlight/css/toml.css
--rw-r--r--   0        0        0      495 2023-07-19 08:15:19.310673 syntaxlight-0.0.5/syntaxlight/css/xml.css
--rw-r--r--   0        0        0     2379 2023-07-17 06:49:24.804921 syntaxlight-0.0.5/syntaxlight/error.py
--rw-r--r--   0        0        0     2009 2023-07-24 08:05:40.440581 syntaxlight-0.0.5/syntaxlight/example.py
--rw-r--r--   0        0        0     1664 2023-07-19 08:35:00.594467 syntaxlight-0.0.5/syntaxlight/export.py
--rw-r--r--   0        0        0     2725 2023-07-23 15:16:02.280132 syntaxlight-0.0.5/syntaxlight/gdt.py
--rw-r--r--   0        0        0      388 2023-07-22 13:46:05.416059 syntaxlight-0.0.5/syntaxlight/lexers/__init__.py
--rw-r--r--   0        0        0     1923 2023-07-22 13:45:56.258345 syntaxlight-0.0.5/syntaxlight/lexers/bnf_lexer.py
--rw-r--r--   0        0        0    12472 2023-07-24 01:14:51.430992 syntaxlight-0.0.5/syntaxlight/lexers/c_lexer.py
--rw-r--r--   0        0        0     1997 2023-07-21 12:49:29.104139 syntaxlight-0.0.5/syntaxlight/lexers/json_lexer.py
--rw-r--r--   0        0        0    19933 2023-07-24 06:59:03.624407 syntaxlight-0.0.5/syntaxlight/lexers/lexer.py
--rw-r--r--   0        0        0     4090 2023-06-16 15:53:43.032864 syntaxlight-0.0.5/syntaxlight/lexers/lua_lexer.py
--rw-r--r--   0        0        0     1801 2023-07-12 06:24:11.777365 syntaxlight-0.0.5/syntaxlight/lexers/shell_lexer.py
--rw-r--r--   0        0        0     2870 2023-07-22 13:41:57.282224 syntaxlight-0.0.5/syntaxlight/lexers/toml_lexer.py
--rw-r--r--   0        0        0     4578 2023-07-20 13:32:30.928035 syntaxlight-0.0.5/syntaxlight/lexers/xml_lexer.py
--rw-r--r--   0        0        0      240 2023-07-21 14:12:28.396351 syntaxlight-0.0.5/syntaxlight/parsers/__init__.py
--rw-r--r--   0        0        0     6858 2023-07-24 01:35:24.029532 syntaxlight-0.0.5/syntaxlight/parsers/bnf_parser.py
--rw-r--r--   0        0        0   100128 2023-07-24 08:05:22.752514 syntaxlight-0.0.5/syntaxlight/parsers/c_parser.py
--rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.0.5/syntaxlight/parsers/json_parser.py
--rw-r--r--   0        0        0     9682 2023-07-24 07:47:18.356056 syntaxlight-0.0.5/syntaxlight/parsers/parser.py
--rw-r--r--   0        0        0      405 2023-07-12 06:09:27.902688 syntaxlight-0.0.5/syntaxlight/parsers/shell_parser.py
--rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.0.5/syntaxlight/parsers/toml_parser.py
--rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.0.5/syntaxlight/parsers/xml_parser.py
--rw-r--r--   0        0        0     3906 2023-07-24 01:38:00.242828 syntaxlight-0.0.5/syntaxlight/syntax_parse.py
--rw-r--r--   0        0        0      405 2023-06-15 12:50:36.421265 syntaxlight-0.0.5/syntaxlight/template.html
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 syntaxlight-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.0.6/LICENSE
+-rw-r--r--   0        0        0      464 2023-07-28 02:44:41.315769 syntaxlight-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2183 2023-07-22 12:55:46.842043 syntaxlight-0.0.6/README.md
+-rw-r--r--   0        0        0      209 2023-07-23 11:29:29.575296 syntaxlight-0.0.6/syntaxlight/__init__.py
+-rw-r--r--   0        0        0    15135 2023-07-25 14:41:59.387948 syntaxlight-0.0.6/syntaxlight/ast.py
+-rw-r--r--   0        0        0     2223 2023-07-19 06:56:41.644931 syntaxlight-0.0.6/syntaxlight/css/all.css
+-rw-r--r--   0        0        0      665 2023-07-22 15:03:22.184483 syntaxlight-0.0.6/syntaxlight/css/bnf.css
+-rw-r--r--   0        0        0     2118 2023-07-23 15:21:29.646891 syntaxlight-0.0.6/syntaxlight/css/c.css
+-rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.0.6/syntaxlight/css/index.css
+-rw-r--r--   0        0        0      529 2023-07-21 12:50:35.868013 syntaxlight-0.0.6/syntaxlight/css/json.css
+-rw-r--r--   0        0        0     1101 2023-07-26 09:05:41.943038 syntaxlight-0.0.6/syntaxlight/css/lua.css
+-rw-r--r--   0        0        0     2720 2023-07-20 08:04:28.110565 syntaxlight-0.0.6/syntaxlight/css/themes.json
+-rw-r--r--   0        0        0      557 2023-07-19 08:11:34.232315 syntaxlight-0.0.6/syntaxlight/css/toml.css
+-rw-r--r--   0        0        0      495 2023-07-19 08:15:19.310673 syntaxlight-0.0.6/syntaxlight/css/xml.css
+-rw-r--r--   0        0        0     2428 2023-07-26 07:25:50.581952 syntaxlight-0.0.6/syntaxlight/error.py
+-rw-r--r--   0        0        0     2011 2023-07-25 01:37:18.564742 syntaxlight-0.0.6/syntaxlight/example.py
+-rw-r--r--   0        0        0     1664 2023-07-19 08:35:00.594467 syntaxlight-0.0.6/syntaxlight/export.py
+-rw-r--r--   0        0        0     2733 2023-07-26 00:54:45.614318 syntaxlight-0.0.6/syntaxlight/gdt.py
+-rw-r--r--   0        0        0      401 2023-07-24 09:03:19.313778 syntaxlight-0.0.6/syntaxlight/lexers/__init__.py
+-rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.0.6/syntaxlight/lexers/bnf_lexer.py
+-rw-r--r--   0        0        0    12468 2023-07-26 05:58:00.354541 syntaxlight-0.0.6/syntaxlight/lexers/c_lexer.py
+-rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.0.6/syntaxlight/lexers/json_lexer.py
+-rw-r--r--   0        0        0    22509 2023-07-26 07:30:31.563233 syntaxlight-0.0.6/syntaxlight/lexers/lexer.py
+-rw-r--r--   0        0        0     8150 2023-07-26 08:57:37.822371 syntaxlight-0.0.6/syntaxlight/lexers/lua_lexer.py
+-rw-r--r--   0        0        0     1801 2023-07-12 06:24:11.777365 syntaxlight-0.0.6/syntaxlight/lexers/shell_lexer.py
+-rw-r--r--   0        0        0     3002 2023-07-26 02:47:58.836633 syntaxlight-0.0.6/syntaxlight/lexers/toml_lexer.py
+-rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.0.6/syntaxlight/lexers/xml_lexer.py
+-rw-r--r--   0        0        0      275 2023-07-25 01:05:05.983118 syntaxlight-0.0.6/syntaxlight/parsers/__init__.py
+-rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.0.6/syntaxlight/parsers/bnf_parser.py
+-rw-r--r--   0        0        0    98600 2023-07-26 01:24:49.618931 syntaxlight-0.0.6/syntaxlight/parsers/c_parser.py
+-rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.0.6/syntaxlight/parsers/json_parser.py
+-rw-r--r--   0        0        0    35078 2023-07-26 09:03:07.504849 syntaxlight-0.0.6/syntaxlight/parsers/lua_parser.py
+-rw-r--r--   0        0        0    12749 2023-07-26 01:33:24.433880 syntaxlight-0.0.6/syntaxlight/parsers/parser.py
+-rw-r--r--   0        0        0      405 2023-07-12 06:09:27.902688 syntaxlight-0.0.6/syntaxlight/parsers/shell_parser.py
+-rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.0.6/syntaxlight/parsers/toml_parser.py
+-rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.0.6/syntaxlight/parsers/xml_parser.py
+-rw-r--r--   0        0        0     4250 2023-07-25 01:39:58.341430 syntaxlight-0.0.6/syntaxlight/syntax_parse.py
+-rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.0.6/syntaxlight/template.html
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 syntaxlight-0.0.6/PKG-INFO
```

### Comparing `syntaxlight-0.0.5/LICENSE` & `syntaxlight-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.5/README.md` & `syntaxlight-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.5/syntaxlight/ast.py` & `syntaxlight-0.0.6/syntaxlight/ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,18 @@
         self.node_info: str = f"[{self.class_name}:{self._created_index}]"
 
         self._indent = " " * 4
         # AST 树包含的 Token
         self._tokens: List[Token] = []
         self._depth = 0  # 节点深度
         self.is_leaf_ast = False  # 底层 AST, 叶节点
-        self.update_subnode = False  # update 时将 class_name 传递到所有的子 AST 节点中
+
+        # 默认 update 的时候只会为一级 AST 添加当前类名, 启用此选项后会递归地将类名传递给其下的每一个叶节点
+        # 默认不开启以减少对子类的影响
+        self.update_subnode = False  
 
     def register_token(self, tokens: List[Token], extra_class_name: str = None):
         """
         将 token 注册到 AST 树中以更新 token 的属性
         """
         for token in tokens:
             token.class_list.add(self.class_name)
@@ -78,19 +81,19 @@
         """
         node_visitor.depth -= 1  # 到达叶节点, 退出到上一层
         # print(f'visit {self.class_name}, depth = {self.depth}')
 
     def formatter(self, depth: int = 0):
         raise NotImplementedError(self.class_name + " should override format function to display")
 
-    # def __str__(self) -> str:
-    #     return self.formatter()
+    def __str__(self) -> str:
+        return self.formatter()
 
-    # def __repr__(self) -> str:
-    #     return self.__str__()
+    def __repr__(self) -> str:
+        return self.__str__()
 
     def get_node_info(self):
         # f'depth={self.depth}\\n'
         node_content = self.node_info + "\\n" + f"depth={self._depth}"
         return f'node{self._created_index} [label="{node_content}"]'
 
 
@@ -192,14 +195,16 @@
 class Identifier(AST):
     def __init__(self, id) -> None:
         super().__init__()
         self.id: str = id
         self.is_leaf_ast = True
         self.node_info += f"\\n{self.id}"
 
+    def formatter(self, depth: int = 0):
+        return self.id
 
 class Punctuator(AST):
     def __init__(self) -> None:
         super().__init__()
         self.op = self.op
         self.is_leaf_ast = True
         self.node_info += f"\\n{self.op}"
```

### Comparing `syntaxlight-0.0.5/syntaxlight/css/all.css` & `syntaxlight-0.0.6/syntaxlight/css/all.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.5/syntaxlight/css/bnf.css` & `syntaxlight-0.0.6/syntaxlight/css/bnf.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.5/syntaxlight/css/c.css` & `syntaxlight-0.0.6/syntaxlight/css/c.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.5/syntaxlight/css/index.css` & `syntaxlight-0.0.6/syntaxlight/css/index.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.5/syntaxlight/css/json.css` & `syntaxlight-0.0.6/syntaxlight/css/json.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.5/syntaxlight/css/themes.json` & `syntaxlight-0.0.6/syntaxlight/css/themes.json`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.5/syntaxlight/css/toml.css` & `syntaxlight-0.0.6/syntaxlight/css/toml.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.5/syntaxlight/error.py` & `syntaxlight-0.0.6/syntaxlight/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 class ErrorCode(Enum):
     # lexer error code
     EXPONENT_NO_DIGITS = "Exponent has no digits"
     NUMBER_INVALID = "Number invalid"
     UNKNOWN_CHARACTER = "unknown character"
     UNTERMINATED_COMMENT = "unterminated comment"
+    UNTERMINATED_STRING = 'unterminated string'
     MULTICHARACTER_CONSTANT = 'Multi-character character constant'
 
     # parser error code
     UNEXPECTED_TOKEN = "Unexpected token"
     MISS_EXPECTED_TOKEN = "Miss expected token"
     TRAILING_COMMA = "Trailing comma not allowed"
```

### Comparing `syntaxlight-0.0.5/syntaxlight/example.py` & `syntaxlight-0.0.6/syntaxlight/example.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,47 +5,48 @@
 from typing import Union, List
 
 
 def example_display(
     file_path: Union[str, List[str]] = None,
     style="vscode",
     save_ast_tree=False,
-    language: str = "guess",
+    language= None,
 ):
     example_folder_name = os.path.join(os.getcwd(), "syntaxlight_example")
-    if language == "guess":
-        if type(file_path) == list:
-            language = guess_language(file_path[0])
-        else:
-            language = guess_language(file_path)
-
     syntaxlight_path = os.path.dirname(__file__)
     html_template_file = os.path.join(syntaxlight_path, "template.html")
     index_css_file = os.path.join(syntaxlight_path, "css", "index.css")
     css_files = [index_css_file]
-    css_scope = f"<link rel='stylesheet' href='./{language}.css' />"
+    
 
     example_html_file = os.path.join(example_folder_name, "index.html")
 
     if not os.path.exists(example_folder_name):
         os.mkdir(example_folder_name)
 
     if type(file_path) == str:
         file_path = [file_path]
 
+    all_languages = []
     code_html = ""
     for fp in file_path:
+        if language is None:
+            language = guess_language(fp)
+            all_languages.append(language)
         html = parse_file(fp, language, save_ast_tree=save_ast_tree)
         if html is None:
             continue
         code_html += f'<p>{fp}</p><pre class="language-{language}"><code>{html}</code></pre>'
 
     code_html = f'<div class="markdown-body">{code_html}</div>'
-    with open(html_template_file, "r", encoding="utf-8") as f:
-        content = f.read().replace("html-scope", code_html).replace("css-scope", css_scope)
+
+    for language in all_languages:
+        css_scope = f"<link rel='stylesheet' href='./{language}.css' />"
+        with open(html_template_file, "r", encoding="utf-8") as f:
+            content = f.read().replace("html-scope", code_html).replace("css-scope", css_scope)
 
     with open(os.path.join(example_folder_name, example_html_file), "w", encoding="utf-8") as f:
         f.write(content)
 
     for file in css_files:
         shutil.copyfile(file, os.path.join(example_folder_name, file.split(os.sep)[-1]))
```

### Comparing `syntaxlight-0.0.5/syntaxlight/export.py` & `syntaxlight-0.0.6/syntaxlight/export.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.5/syntaxlight/gdt.py` & `syntaxlight-0.0.6/syntaxlight/gdt.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,20 @@
     ENUM_ID = "EnumID"  # 枚举类型
 
 
 class Descriptor(TypedDict):
     type: Enum
     scope: str
 
-class Argument(TypedDict):
+
+class FuncArgument(TypedDict):
     name: str
     type: Tuple[str]
 
 
-
 class GlobalDescriptorTable:
     def __init__(self) -> None:
         self._descriptors: Dict[str, Descriptor] = {}  # 内部维护的全局描述符表
         self._classname_map = {}
         self._loginfo = []
 
     def _log(self, info: str):
@@ -46,15 +46,15 @@
             self._log(f"[register_id]: cover {id_name}")
 
         self._descriptors[id_name] = {"type": id_type, "scope": scope}
 
     def register_function(
         self,
         function_name: str,
-        arguments: List[Argument],
+        arguments: List[FuncArgument],
         return_value: Tuple[str],
         type: Enum,
         scope: str = "global",
     ):
         """
         注册函数
```

### Comparing `syntaxlight-0.0.5/syntaxlight/lexers/bnf_lexer.py` & `syntaxlight-0.0.6/syntaxlight/lexers/bnf_lexer.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             if self.current_char in ("'", '"'):
                 return self.get_str()
             
             if self.current_char.isalnum() or self.current_char == '_':
                 return self.get_id(extend_chars=['_','-'])
             
             if self.current_char == '#':
-                return self.get_comment(("#",'\n'))
+                return self.get_comment("#",'\n')
             
             if self.current_char in self.long_op_dict:
                 return self.get_long_op()
             
             try:
                 token_type = TokenType(self.current_char)
             except ValueError: # pragma: no cover
```

### Comparing `syntaxlight-0.0.5/syntaxlight/lexers/c_lexer.py` & `syntaxlight-0.0.6/syntaxlight/lexers/c_lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,17 +140,17 @@
             if self.current_char == TokenType.SPACE.value:
                 return self.skip_whitespace()
 
             if self.current_char in self.invisible_characters:
                 return self.skip_invisiable_character()
 
             if self.current_char == "/" and self.peek() == "/":
-                return self.get_comment(("//", "\n"))
+                return self.get_comment("//", "\n")
             if self.current_char == "/" and self.peek() == "*":
-                return self.get_comment(("/*", "*/"))
+                return self.get_comment("/*", "*/")
 
             if self.current_char.isdigit():
                 return self.get_number()
 
             if self.current_char.isalpha() or self.current_char == TokenType.UNDERLINE.value:
                 return self.get_id()
```

### Comparing `syntaxlight-0.0.5/syntaxlight/lexers/json_lexer.py` & `syntaxlight-0.0.6/syntaxlight/lexers/json_lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             if self.current_char.isdigit():
                 return self.get_number()
 
             if self.current_char.isalnum() or self.current_char == '_':
                 return self.get_id()
             
             if self.current_char == '/' and self.peek() == '/':
-                return self.get_comment(('//','\n'))
+                return self.get_comment('//','\n')
             
             try:
                 token_type = TokenType(self.current_char)
             except ValueError: # pragma: no cover
                 token = Token(None, self.current_char, self.line, self.column)
                 self.error(ErrorCode.UNKNOWN_CHARACTER, token)
             else:
```

### Comparing `syntaxlight-0.0.5/syntaxlight/lexers/lexer.py` & `syntaxlight-0.0.6/syntaxlight/lexers/lexer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from enum import Enum
 from ..error import ErrorCode, LexerError
-from typing import Dict, List
+from typing import Dict, List, Tuple
+import re
 
 GLOBAL_TOKEN_ID = 0
 
 # class NewTokenType(Enum):
 #     RESERVED_KEYWORD_START = "RESERVED_KEYWORD_START"
 #     RESERVED_KEYWORD_END = "RESERVED_KEYWORD_END"
 
@@ -62,49 +63,52 @@
     FLOAT = "FLOAT"  # 小数
     COMMENT = "COMMENT"
     SHL = "<<"
     SHR = ">>"
     EQ = "=="
     STRICT_EQ = "==="
     NE = "!="
+    NORE = "~="
     STRICT_NE = "!=="
+    DOUBLE_DIV = "//"
     LT = "LT"  # => LANGLE_BRACE
     GT = "GT"  # => RANGLE_BRACE
     LE = "<="
     GE = ">="
     MUL_ASSIGN = "*="
     DIV_ASSIGN = "/="
     MOD_ASSIGN = "%="
     ADD_ASSIGN = "+="
     SUB_ASSIGN = "-="
     LSHIFT_ASSIGN = "<<="
     RSHIFT_ASSIGN = ">>="
     AND_ASSIGN = "&="
     XOR_ASSIGN = "^="
     OR_ASSIGN = "|="
+    CONCAT = ".."
     VARARGS = "..."
-    DB_COLON = "::"
+    DOUBLE_COLON = "::"
     INC = "++"
     DEC = "--"
     OR = "||"
     AND = "&&"
     POINT = "->"
     PRODUCTION_SYMBOL = "::="
     DOUBLE_HASH = "##"
 
 
 class TTYColor(Enum):
     BLACK = 30
-    RED = 31
-    GREEN = 32
-    YELLOW = 33
-    BLUE = 34
-    MAGENTA = 35
-    CYAN = 36
-    WHITE = 37
+    RED = 91
+    GREEN = 92
+    YELLOW = 93
+    BLUE = 94
+    MAGENTA = 95
+    CYAN = 96
+    WHITE = 97
 
 
 class Token:
     def __init__(self, type: Enum, value, line=None, column=None):
         self.type: Enum = type
         self.value = value
         self.line: int = line
@@ -132,15 +136,15 @@
         column 指该 token 最后一个字符的位置
         """
         return "Token[{ID}]({type}, {value}, position={lineno}:{column})".format(
             ID=self._id,
             type=self.type,
             value=repr(self.value),
             lineno=self.line,
-            column=self.column
+            column=self.column,
         )
 
     def __repr__(self):
         return self.__str__()
 
 
 class Lexer:
@@ -157,15 +161,15 @@
         self.pos: int = 0  # 当前指针指向的字符
         self.current_char: str = self.text[self.pos]  # 当前指针指向的字符
         self.line: int = 1
         self.column: int = 1  # 指向 token 的 value 中最后出现的字符的位置
         self.LanguageTokenType: Enum = LanguageTokenType
         self.context_bias = 10  # 发生错误时 token 的前后文行数
         self.file_path = None  # 手动修改文件路径, 用于后期错误处理的输出
-        self._status_stack = [] # 状态栈
+        self._status_stack = []  # 状态栈
 
         # 获取 RESERVED_KEYWORD_START - RESERVED_KEYWORD_END 之间的保留关键字
         tt_list = list(LanguageTokenType)
         start_index = tt_list.index(LanguageTokenType.RESERVED_KEYWORD_START)
         end_index = tt_list.index(LanguageTokenType.RESERVED_KEYWORD_END)
         self.reserved_keywords = {
             token_type.value: token_type for token_type in tt_list[start_index + 1 : end_index]
@@ -193,40 +197,45 @@
         self._long_ops = sorted(supported_long_op, key=len, reverse=True)
         for long_op in self._long_ops:
             assert len(long_op) >= 2, f"{long_op} should be longer"
             if self.long_op_dict.get(long_op[0]) is None:
                 self.long_op_dict[long_op[0]] = []
             self.long_op_dict[long_op[0]].append(long_op[1:])
 
-    def ttyinfo(self, text: str, color: TTYColor = TTYColor.RED) -> str:
+    def ttyinfo(self, text: str, color: TTYColor = TTYColor.RED, underline=True) -> str:
         """
         tty 彩色输出, 默认红色
         """
         ESC = "\033"
         UNDERLINE = 4
-        return f"{ESC}[{color.value}m{ESC}[{UNDERLINE}m{text}{ESC}[0m"
+        if underline:
+            return f"{ESC}[{color.value}m{ESC}[{UNDERLINE}m{text}{ESC}[0m"
+        else:
+            return f"{ESC}[{color.value}m{text}{ESC}[0m"
 
     def _record(self):
         """
         用于 parser 中 peek_next_token
 
         记录当前 lexer 解析状态, 被 _reset 调用时恢复
         """
         # 采用栈的方式保存数据状态, 避免由于 peek_next_token 中的 eat 导致多次嵌套调用覆盖数据
-        self._status_stack.append({"pos": self.pos, 'c':self.current_char, "line": self.line, "column": self.column})
+        self._status_stack.append(
+            {"pos": self.pos, "c": self.current_char, "line": self.line, "column": self.column}
+        )
 
     def _reset(self):
         """
         用于 parser 中 peek_next_token
 
         恢复为 lexer 之前的状态
         """
         status = self._status_stack.pop()
         self.pos = status["pos"]
-        self.current_char = status['c']
+        self.current_char = status["c"]
         self.line = status["line"]
         self.column = status["column"]
 
     def error(self, error_code: ErrorCode = None, token: Token = None, message: str = ""):
         raise LexerError(
             error_code=error_code,
             token=token,
@@ -337,47 +346,92 @@
         """
         peek_pos = self.pos + n
         if peek_pos > len(self.text) - 1:
             return None
         else:
             return self.text[self.pos + 1 : peek_pos + 1]
 
-    def get_number(self) -> Token:
+    def get_number(self, accept_float = True, accept_hex = False, accept_bit = False, accept_p = False) -> Token:
         """
          <digit> ::= [0-9]
         <digits> ::= <digit>*
         <number> ::= <digits>(.<digits>)?(E|e[+-]?<digits>)?
-        """
+
+        @accept_float: 允许小数和科学计数法
+        @accept_hex  : 允许16进制表示 0xfff
+        @accept_bit  : 允许二进制表示 0b111
+        """
+        bit_matching_status = False
+        hex_matching_status = False
+        def is_match_char(char:str) -> bool:
+            
+            if hex_matching_status:
+                return bool(re.match(r'[0-9a-fA-F]',char))
+            if bit_matching_status:
+                return bool(re.match(r'[01]',char))
+            return char.isdigit()
 
         result = ""
+
+        if accept_hex:
+            if self.current_char == '0' and self.peek() in ('x', 'X'):
+                result = self.current_char
+                self.advance()
+                result += self.current_char
+                self.advance()
+                hex_matching_status = True
+
+        if accept_bit:
+            if self.current_char == '0' and self.peek() in ('b', 'B'):
+                result = self.current_char
+                self.advance()
+                result += self.current_char
+                self.advance()
+                # 如果此时已经处于 hex_matching_status 状态了则忽略 
+                if not hex_matching_status:
+                    bit_matching_status = True
+
+
         # <digits>
-        while self.current_char is not None and self.current_char.isdigit():
+        while self.current_char is not None and is_match_char(self.current_char):
             result += self.current_char
             self.advance()
 
-        # (.<digits>)?
-        if self.current_char == ".":
-            result += self.current_char
-            self.advance()
-            while self.current_char is not None and self.current_char.isdigit():
+        if accept_float:
+            # (.<digits>)?
+            if self.current_char == ".":
                 result += self.current_char
                 self.advance()
+                while self.current_char is not None and is_match_char(self.current_char):
+                    result += self.current_char
+                    self.advance()
 
-        # (E|e[+-]?<digits>)?
-        if self.current_char == "e" or self.current_char == "E":
-            result += self.current_char
-            self.advance()
-            if self.current_char in (TokenType.MINUS.value, TokenType.PLUS.value):
+            # (E|e[+-]?<digits>)?
+            if self.current_char == "e" or self.current_char == "E":
                 result += self.current_char
                 self.advance()
-            while self.current_char is not None and self.current_char.isdigit():
+                if self.current_char in (TokenType.MINUS.value, TokenType.PLUS.value):
+                    result += self.current_char
+                    self.advance()
+                while self.current_char is not None and is_match_char(self.current_char):
+                    result += self.current_char
+                    self.advance()
+        
+        if accept_p:
+            if self.current_char in ('P','p'):
                 result += self.current_char
                 self.advance()
-        # column - 1, 因为判断结束需要跳出 number
+                if self.current_char in (TokenType.MINUS.value, TokenType.PLUS.value):
+                    result += self.current_char
+                    self.advance()
+                while self.current_char is not None and is_match_char(self.current_char):
+                    result += self.current_char
+                    self.advance()
 
+        # column - 1, 因为判断结束需要跳出 number
         return Token(TokenType.NUMBER, result, self.line, self.column - 1)
 
     def get_string(self):
         """
         严格双引号 ""
         """
         result = self.current_char
@@ -400,61 +454,77 @@
         result += end_character
         token = Token(TokenType.STRING, result, self.line, self.column)
         self.advance()
         return token
 
     def get_str(self):
         """
-        'xxx' "xxx" \"\"\"xxx\"\"\" '''xxx''' 都可以
+        匹配 "" 和 '' 之间的字符
         """
         result = self.current_char
-        if result not in (TokenType.QUOTO.value, TokenType.APOSTROPHE.value):
+        if result not in ("'", '"'):
             token = Token(TokenType.STRING, result, self.line, self.column)
             self.advance()
             self.error(ErrorCode.UNEXPECTED_TOKEN, token)
         end_character = self.current_char  # 结束标志一定是和开始标志相同的
         self.advance()
 
         while self.current_char is not None and self.current_char != end_character:
             result += self.current_char
             if self.current_char == "\\":
                 self.advance()
                 if self.current_char is None:
                     self.error(
                         ErrorCode.UNEXPECTED_TOKEN,
-                        Token(TokenType.STRING, result, self.line, self.column),
+                        Token(TokenType.STRING, result, self.line, self.column - 1),
                     )
                 result += self.current_char
             self.advance()
 
         result += end_character
+        token = Token(TokenType.STR, result, self.line, self.column)
         self.advance()
-        # ''' or """
-        if len(result) == 2 and self.current_char == end_character:
-            result += self.current_char
+        return token
+
+    def get_extend_str(self, extend_symbol_pair: Tuple[str, str], token_type: Enum = TokenType.STR):
+        """
+        扩展匹配字符串, 比如 """ """ 和 ''' '''
+        """
+        start_symbol, end_symbol = extend_symbol_pair
+        assert len(start_symbol) > 0 and len(end_symbol) > 0
+        assert self.current_char == start_symbol[0]
+        if len(start_symbol) > 1:
+            assert self.peek(len(start_symbol) - 1) == start_symbol[1:]
+
+        result = start_symbol
+        for _ in range(len(start_symbol)):
             self.advance()
-            count = 0
-            while self.current_char is not None and count != 3:
-                if self.current_char == end_character:
-                    count += 1
-                else:
-                    count = 0
-                result += self.current_char
+
+        end_symbol_length = len(end_symbol)
+        while self.current_char is not None:
+            if (
+                self.current_char == end_symbol[0]
+                and self.peek(end_symbol_length - 1) == end_symbol[1:]
+            ):
+                break
+            else:
                 if self.current_char == "\\":
-                    self.advance()
-                    if self.current_char is None:
-                        self.error(
-                            ErrorCode.UNEXPECTED_TOKEN,
-                            Token(TokenType.STRING, result, self.line, self.column),
-                        )
-                    count = 0
                     result += self.current_char
+                    self.advance()
+                result += self.current_char
+                self.advance()
+
+        if self.current_char is None:
+            token = Token(token_type, result, self.line, self.column - 1)
+        else:
+            result += end_symbol
+            for _ in range(end_symbol_length):
                 self.advance()
+            token = Token(token_type, result, self.line, self.column - 1)
 
-        token = Token(TokenType.STR, result, self.line, self.column - 1)
         return token
 
     def get_id(self, ignore_case=False, extend_chars: List[str] = ["_"]):
         """
         获取标识符, 留给后续的语法分析处理
         @ignore_case : 是否忽略大小写
         @extend_chars: 扩展字符, 默认扩展 "_", 一般还可修改为 ["_", "-"]
@@ -481,25 +551,25 @@
         if token_type is None:
             token = Token(type=TokenType.ID, value=result, line=self.line, column=self.column - 1)
         else:
             # 作为保留关键字
             token = Token(type=token_type, value=result, line=self.line, column=self.column - 1)
         return token
 
-    def get_comment(self, comment_symbol=("#", "\n")):
+    def get_comment(self, start_symbol="#", end_symbol="\n"):
         """
         跳过注释部分, 单行注释不包括最后的换行
 
+        多个注释的情况分多个 get_comment 函数处理
+
         python 风格: ("#", "\n")
              C 风格: ("//", "\n"), ("/*", "*/")
         pascal 风格: ("//", "\n"), ("{", "}"), ("(*", "*)")
-           lua 风格: ("--[[", "]]"), ("--", "\n") # 有二义性的放前面
         """
 
-        start_symbol, end_symbol = comment_symbol
         assert start_symbol[0] == self.current_char
 
         result = start_symbol
         for _ in range(len(start_symbol)):
             self.advance()
 
         end_symbol_length = len(end_symbol)
```

### Comparing `syntaxlight-0.0.5/syntaxlight/lexers/shell_lexer.py` & `syntaxlight-0.0.6/syntaxlight/lexers/shell_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.5/syntaxlight/lexers/toml_lexer.py` & `syntaxlight-0.0.6/syntaxlight/lexers/toml_lexer.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 
 class TomlLexer(Lexer):
     def __init__(self, text: str, LanguageTokenType: Enum = TomlTokenType):
         super().__init__(text, LanguageTokenType)
 
     def get_next_token(self):
         while self.current_char is not None:
+            if self.current_char == "'" and self.peek(2) == "''":
+                return self.get_extend_str(("'''", "'''"))
+            if self.current_char == '"' and self.peek(2) == '""':
+                return self.get_extend_str(('"""', '"""'))
+
             # TOML 单双引号都可以
-            if (
-                self.current_char == TokenType.QUOTO.value
-                or self.current_char == TokenType.APOSTROPHE.value
-            ):
+            if self.current_char in ('"', "'"):
                 return self.get_str()
 
             if self.current_char == TokenType.SPACE.value:
                 return self.skip_whitespace()
 
             if self.current_char in self.invisible_characters:
                 return self.skip_invisiable_character()
-            
+
             if self.current_char == TokenType.HASH.value:
                 # match comment
                 return self.get_comment()
 
             if self.current_char.isdigit():
                 token = self.get_number()
                 # https://datatracker.ietf.org/doc/html/rfc3339
@@ -49,27 +51,27 @@
                         result += self.current_char
                         self.advance()
                     return Token(TomlTokenType.DATE, result, self.line, self.column - 1)
                 else:
                     return token
 
             if self.current_char.isalpha():
-                return self.get_id(extend_chars=['_'])
+                return self.get_id(extend_chars=["_"])
 
             try:
                 token_type = TokenType(self.current_char)
-            except ValueError: # pragma: no cover
+            except ValueError:  # pragma: no cover
                 token = Token(None, self.current_char, self.line, self.column)
                 self.error(ErrorCode.UNKNOWN_CHARACTER, token)
             else:
                 token = Token(
                     type=token_type,
                     value=token_type.value,  # e.g. ';', '.', etc
                     line=self.line,
                     column=self.column,
                 )
                 self.advance()
                 return token
 
         # EOF (end-of-file) token indicates that there is no more
         # input left for lexical analysis
-        return Token(type=TokenType.EOF, value='EOF', line=self.line, column=self.column)
+        return Token(type=TokenType.EOF, value="EOF", line=self.line, column=self.column)
```

### Comparing `syntaxlight-0.0.5/syntaxlight/lexers/xml_lexer.py` & `syntaxlight-0.0.6/syntaxlight/lexers/xml_lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                     self.advance()
                     self.advance()
                     self.advance()
                     token = Token(XmlTokenType.PROLOG_START, result, self.line, self.column)
                     self.advance()
                     return token
                 elif self.peek(3) == "!--":
-                    return self.get_comment(("<!--", "-->"))
+                    return self.get_comment("<!--", "-->")
                 elif self.peek() == "/":
                     self.advance()
                     token = Token(XmlTokenType.TAG_COMPLETE_BEGIN, "</", self.line, self.column)
                     self.advance()
                     return token
                 else:
                     token = Token(
```

### Comparing `syntaxlight-0.0.5/syntaxlight/parsers/bnf_parser.py` & `syntaxlight-0.0.6/syntaxlight/parsers/bnf_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from .parser import Parser
 from ..lexers import TokenType
 from ..error import ErrorCode
 from ..ast import String, AST, Identifier, Expression, NodeVisitor, Punctuator, add_ast_type
+from enum import Enum
+
+class BNF_CSS(Enum):
+    BUILTIN_SYMBOL = "BuiltinSymbol"
 
 
 class Syntax(AST):
     def __init__(self) -> None:
         super().__init__()
         self.rules = None
 
@@ -204,9 +208,9 @@
         node.register_token(self.eat(TokenType.STR))
         return node
 
     def identifer(self):
         node = Identifier(self.current_token.value)
         node.register_token(self.eat(TokenType.ID))
         if node.id.isupper():
-            add_ast_type(node, "BuiltinSymbol")
+            add_ast_type(node, BNF_CSS.BUILTIN_SYMBOL)
         return node
```

### Comparing `syntaxlight-0.0.5/syntaxlight/parsers/c_parser.py` & `syntaxlight-0.0.6/syntaxlight/parsers/c_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 *@date: 2023-07-16
 *@email: luzhixing12345@163.com
 *@Github: luzhixing12345
 """
 
 import re
 
-from syntaxlight.ast import AST, NodeVisitor
 from .parser import Parser
 from ..lexers import TokenType, CTokenType, CTokenSet, Token
 from ..error import ErrorCode
 from ..ast import (
     AST,
     String,
     Keyword,
@@ -543,14 +542,15 @@
         super().__init__()
         self.group_parts = None
 
     def visit(self, node_visitor: NodeVisitor = None):
         node_visitor.link(self, self.group_parts)
         return super().visit(node_visitor)
 
+
 class IfSection(AST):
     def __init__(self) -> None:
         super().__init__()
         self.group = None
 
     def visit(self, node_visitor: NodeVisitor = None):
         node_visitor.link(self, self.group)
@@ -751,15 +751,15 @@
         """
         <storage-class-specifier> ::= 'auto'
                                     | 'register'
                                     | 'static'
                                     | 'extern'
                                     | 'typedef'
         """
-        return self.keyword(css_type=C_CSS.STORAGE_TYPE)
+        return self.get_keyword(css_type=C_CSS.STORAGE_TYPE)
 
     def type_specifier(self):
         """
         <type-specifier> ::= void
                            | char
                            | short
                            | int
@@ -784,34 +784,34 @@
         elif self.current_token.type in self.cfirst_set.struct_or_union_specifier:
             node = self.struct_or_union_specifier()
         elif self.current_token.type in self.cfirst_set.enum_specifier:
             node = self.enum_specifier()
         elif self.current_token.type in self.cfirst_set.typedef_name:
             node = self.typedef_name()
         elif self.current_token.type in self.cfirst_set.type_specifier:
-            node = self.keyword(css_type=C_CSS.BASE_TYPE)
+            node = self.get_keyword(css_type=C_CSS.BASE_TYPE)
         else:  # pragma: no cover
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be type specifier")
         add_ast_type(node, C_CSS.TYPE_SPECIFIER)
         return node
 
     def function_specifier(self):
         """
         <function-specifier> ::= inline
                                | _Noreturn
         """
-        return self.keyword(css_type=C_CSS.FUNCTION_TYPE)
+        return self.get_keyword(css_type=C_CSS.FUNCTION_TYPE)
 
     def alignment_specifier(self):
         """
         <alignment-specifier> ::= _Alignas "(" <type-name> ")"
                                 | _Alignas "(" <constant-expression> ")"
         """
         node = TypeSpecifier()
-        node.update(keyword=self.keyword(CTokenType._ALIGNAS))
+        node.update(keyword=self.get_keyword(CTokenType._ALIGNAS))
         node.register_token(self.eat(TokenType.LPAREN))
         if self.current_token.type in self.cfirst_set.type_name:
             node.update(sub_node=self.type_name())
             node.register_token(self.eat(TokenType.RPAREN))
         elif self.current_token.type in self.cfirst_set.constant_expression:
             node.update(sub_node=self.constant_expression())
             node.register_token(self.eat(TokenType.RPAREN))
@@ -821,15 +821,15 @@
         return node
 
     def atomic_type_specifier(self):
         """
         <atomic-type-specifier> ::= _Atomic "(" <type-name> ")"
         """
         node = TypeSpecifier()
-        node.update(keyword=self.keyword(CTokenType._ATOMIC))
+        node.update(keyword=self.get_keyword(CTokenType._ATOMIC))
         node.register_token(self.eat(TokenType.LPAREN))
         node.update(sub_node=self.type_name())
         node.register_token(self.eat(TokenType.RPAREN))
         add_ast_type(node, C_CSS.ATOMAIC_TYPE_SPECIFIER)
         return node
 
     def struct_or_union_specifier(self):
@@ -869,15 +869,15 @@
         return node
 
     def struct_or_union(self):
         """
         <struct-or-union> ::= "struct"
                             | "union"
         """
-        return self.keyword(css_type=C_CSS.STRUCTURE_TYPE)
+        return self.get_keyword(css_type=C_CSS.STRUCTURE_TYPE)
 
     def struct_declaration(self):
         """
         <struct-declaration> ::= <specifier-qualifier-list> <struct-declarator-list>? ";"
                                | <static_assert-declaration>
         """
         node = StructDeclaration()
@@ -903,28 +903,27 @@
                 result.append(self.type_qualifier())
         return result
 
     def after_eat(self):
         if self.current_token.type == TokenType.ID and self.current_token.value in GDT:
             if GDT[self.current_token.value] == CSS.TYPEDEF:
                 self.current_token.type = CTokenType.TYPEDEF_ID
-        
+
         if self.in_preprocessing:
             if self.current_token.type == CTokenType.IF:
                 self.current_token.type = CTokenType.IF_P
             elif self.current_token.type == CTokenType.ELSE:
                 self.current_token.type = CTokenType.ELSE_P
             elif self.current_token.value in self.preprocessing_keywords:
                 self.current_token.type = CTokenType(self.current_token.value)
-                
+
         elif self.current_token.type == TokenType.HASH:
             # 多根节点树
             # TODO: 考虑如何格式化
             self.group()
-            
 
     def struct_declarator_list(self) -> List[AST]:
         """
         <struct-declarator-list> ::= <struct-declarator> ("," <struct-declarator>)*
         """
         result = [self.struct_declarator()]
         while self.current_token.type == TokenType.COMMA:
@@ -989,15 +988,15 @@
     def type_qualifier(self):
         """
         <type-qualifier> ::= const
                            | volatile
                            | restrict
                            | _Atomic
         """
-        return self.keyword(css_type=C_CSS.QUALIFY_TYPE)
+        return self.get_keyword(css_type=C_CSS.QUALIFY_TYPE)
 
     def direct_declaractor(self):
         """
         <direct-declarator> ::= <identifier>
                               | "(" <declarator> ")"
                               | <direct-declarator> "[" <type-qualifier-list>? <assignment-expression>? "]"
                               | <direct-declarator> "[" static <type-qualifier-list>? <assignment-expression> "]"
@@ -1032,23 +1031,27 @@
         sub_nodes = []
         while self.current_token.type in (TokenType.LPAREN, TokenType.LSQUAR_PAREN):
             sub_node = DirectDeclaractorPostfix()
             if self.current_token.type == TokenType.LSQUAR_PAREN:
                 sub_node.register_token(self.eat(TokenType.LSQUAR_PAREN))
 
                 if self.current_token.type == CTokenType.STATIC:
-                    sub_node.update(static_head=self.keyword(CTokenType.STATIC, C_CSS.STORAGE_TYPE))
+                    sub_node.update(
+                        static_head=self.get_keyword(CTokenType.STATIC, C_CSS.STORAGE_TYPE)
+                    )
 
                 if self.current_token.type in self.cfirst_set.type_qualifier:
                     sub_node.update(type_qualifiers=self.type_qualifier_list())
 
                 if self.current_token.type == CTokenType.STATIC:
                     if sub_node.static_head is not None:
                         self.error(ErrorCode.UNEXPECTED_TOKEN, "multi static")
-                    sub_node.update(static_foot=self.keyword(CTokenType.STATIC, C_CSS.STORAGE_TYPE))
+                    sub_node.update(
+                        static_foot=self.get_keyword(CTokenType.STATIC, C_CSS.STORAGE_TYPE)
+                    )
 
                 if self.current_token.type == TokenType.MUL:
                     self.current_token.type = CTokenType.STAR
                     sub_node.register_token(self.eat(CTokenType.STAR))
                 elif self.current_token.type in self.cfirst_set.assignment_expression:
                     sub_node.update(assignment_expr=self.assignment_expression())
 
@@ -1298,15 +1301,15 @@
             if self.current_token.type == TokenType.MUL:
                 self.current_token.type = CTokenType.POINTER
             unary_expr = UnaryOp(op=self.current_token.value)
             unary_expr.register_token(self.eat(self.current_token.type))
             unary_expr.update(expr=self.cast_expression())
             node.update(expr=unary_expr)
         elif self.current_token.type == CTokenType.SIZEOF:
-            node.update(keyword=self.keyword(CTokenType.SIZEOF))
+            node.update(keyword=self.get_keyword(CTokenType.SIZEOF))
 
             # 这里的判断有点复杂, 因为 可以
             # A: sizeof "(" <type-name> ")"
             #
             # B: sizeof <unary-expression> => sizeof <postfix-expression> => sizeof <primary-expression>
             # => sizeof "(" <expression> ")"
             # 需要区分 type-name 和 expression
@@ -1327,15 +1330,15 @@
                     self.error(ErrorCode.UNEXPECTED_TOKEN, "should be type name or expression")
 
             else:
                 self.error(
                     ErrorCode.UNEXPECTED_TOKEN, "sizeof should follow with unary expr or typename"
                 )
         elif self.current_token.type == CTokenType._ALIGNOF:
-            node.update(keyword=self.keyword(CTokenType._ALIGNOF))
+            node.update(keyword=self.get_keyword(CTokenType._ALIGNOF))
             node.register_token(self.eat(TokenType.LPAREN))
             node.update(expr=self.type_name())
             node.register_token(self.eat(TokenType.RPAREN))
         else:
             self.error(
                 ErrorCode.UNEXPECTED_TOKEN,
                 "unary expression should follow with postfix or ++ or -- or unary operator or sizeof",
@@ -1454,15 +1457,15 @@
         return node
 
     def generic_selection(self):
         """
         <generic-selection> ::= _Generic "(" <assignment-expression> "," <generic-assoc-list> ")"
         """
         node = GenericSelection()
-        node.update(keyword=self.keyword(CTokenType._GENERIC))
+        node.update(keyword=self.get_keyword(CTokenType._GENERIC))
         node.register_token(self.eat(TokenType.LPAREN))
         node.update(assignment_expr=self.assignment_expression())
         node.register_token(self.eat(TokenType.COMMA))
         node.update(generic_assoc_list=self.generic_assoc_list())
         return node
 
     def generic_assoc_list(self) -> List[AST]:
@@ -1478,15 +1481,15 @@
     def generic_association(self):
         """
         <generic-association> ::= <type-name> ":" <assignment-expression>
                                 | default ":" <assignment-expression>
         """
         node = GenericAssociation()
         if self.current_token.type == CTokenType.DEFAULT:
-            node.update(keyword=self.keyword(CTokenType.DEFAULT))
+            node.update(keyword=self.get_keyword(CTokenType.DEFAULT))
         elif self.current_token.type in self.cfirst_set.type_name:
             node.update(type_name=self.type_name())
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be default or type-name")
         node.register_token(self.eat(TokenType.COLON))
         node.update(assignment_expr=self.assignment_expression())
         return node
@@ -1510,15 +1513,15 @@
         """
         # <conditional-expression> => <cast-expression> => ("(" <type-name> ")")* <unary-expression>
         # 无法 LL1 判断, 需要额外处理
         if self.current_token.type not in self.cfirst_set.assignment_expression:
             self.error(
                 ErrorCode.UNEXPECTED_TOKEN, "should be unary expression or conditional expression"
             )
-        
+
         node = AssignmentExpression()
         expr = self.conditional_expression()
         if isinstance(expr.condition_expr, BinaryOp):
             # 含双目运算符, 必为 conditional expression
             node.update(expr=expr)
         elif isinstance(expr.condition_expr, CastExpression):
             # CastExpression 含 type_names 必为 conditional expression
@@ -1633,22 +1636,26 @@
                     self.current_token.type = CTokenType.STAR
                     sub_node.register_token(self.eat(CTokenType.STAR))
                     sub_node.register_token(self.eat(TokenType.RSQUAR_PAREN))
                     sub_nodes.append(sub_node)
                     continue
 
                 if self.current_token.type == CTokenType.STATIC:
-                    sub_node.update(static_head=self.keyword(CTokenType.STATIC, C_CSS.STORAGE_TYPE))
+                    sub_node.update(
+                        static_head=self.get_keyword(CTokenType.STATIC, C_CSS.STORAGE_TYPE)
+                    )
                 if self.current_token.type in self.cfirst_set.type_qualifier:
                     sub_node.update(type_qualifiers=self.type_qualifier_list())
 
                 if self.current_token.type == CTokenType.STATIC:
                     if sub_node.static_head is not None:
                         self.error(ErrorCode.UNEXPECTED_TOKEN, "multi static")
-                    sub_node.update(static_foot=self.keyword(CTokenType.STATIC, C_CSS.STORAGE_TYPE))
+                    sub_node.update(
+                        static_foot=self.get_keyword(CTokenType.STATIC, C_CSS.STORAGE_TYPE)
+                    )
 
                 if self.current_token.type in self.cfirst_set.assignment_expression:
                     sub_node.update(assignment_expr=self.assignment_expression())
 
                 sub_node.register_token(self.eat(TokenType.RSQUAR_PAREN))
                 sub_nodes.append(sub_node)
 
@@ -1657,15 +1664,15 @@
 
     def enum_specifier(self):
         """
         <enum-specifier> ::= enum (<identifier>)? "{" <enumerator> ("," <enumerator>)* ","? "}"
                            | enum <identifier>
         """
         node = EnumSpecifier()
-        node.update(keyword=self.keyword(CTokenType.ENUM))
+        node.update(keyword=self.get_keyword(CTokenType.ENUM))
         if self.current_token.type in self.cfirst_set.identifier:
             node.update(id=self.identifier())
             delete_ast_type(node.id, CSS.MACRO_DEFINE)
             add_ast_type(node.id, CSS.ENUM_ID)
             GDT.register_id(node.id.id, CSS.ENUM_ID)
         if self.current_token.type == TokenType.LCURLY_BRACE:
             node.register_token(self.eat(TokenType.LCURLY_BRACE))
@@ -1693,15 +1700,15 @@
             node.update(const_expr=self.constant_expression())
         return node
 
     def typedef_name(self):
         """
         <typedef-name> ::= <identifier>
         """
-        node = self.keyword(CTokenType.TYPEDEF_ID, css_type=CSS.TYPEDEF)
+        node = self.get_keyword(CTokenType.TYPEDEF_ID, css_type=CSS.TYPEDEF)
         return node
 
     def declaration(self):
         """
         <declaration> ::= <declaration-specifier>+ (<init-declarator-list>)? ";"
                         | <static-assert-declaration>
 
@@ -1834,33 +1841,33 @@
         node = Initializer()
         if self.current_token.type in self.cfirst_set.assignment_expression:
             node.update(assignment_expr=self.assignment_expression())
         elif self.current_token.type == TokenType.LCURLY_BRACE:
             node.register_token(self.eat(TokenType.LCURLY_BRACE))
             if self.current_token.type in self.cfirst_set.initializer_list:
                 node.update(initializer_list=self.initializer_list())
-                
+
             if self.current_token.type == TokenType.COMMA:
                 node.register_token(self.eat(TokenType.COMMA))
-                
+
             node.register_token(self.eat(TokenType.RCURLY_BRACE))
         else:
             self.error(
                 ErrorCode.UNEXPECTED_TOKEN, "should be initializer list or assignment expression"
             )
         return node
 
     def initializer_list(self) -> List[AST]:
         """
         <initializer-list> ::= <designation>? <initializer> ("," <designation>? <initializer>)*
         """
         node = DesignationInitializer()
         if self.current_token.type in self.cfirst_set.designation:
             node.update(designation=self.designation())
-        
+
         node.update(initializer=self.initializer())
         result = [node]
         while self.current_token.type == TokenType.COMMA:
             next_token_type = self.peek_next_token().type
             if (
                 next_token_type not in self.cfirst_set.designation
                 and next_token_type not in self.cfirst_set.initializer
@@ -1968,18 +1975,18 @@
 
         if self.current_token.type in self.cfirst_set.identifier:
             node.update(id=self.identifier())
             # goto 的标签
             add_ast_type(node.id, C_CSS.GOTO_LABEL)
             GDT.register_id(node.id.id, C_CSS.GOTO_LABEL)
         elif self.current_token.type == CTokenType.CASE:
-            node.update(keyword=self.keyword(CTokenType.CASE))
+            node.update(keyword=self.get_keyword(CTokenType.CASE))
             node.update(const_expr=self.constant_expression())
         elif self.current_token.type == CTokenType.DEFAULT:
-            node.update(keyword=self.keyword(CTokenType.DEFAULT))
+            node.update(keyword=self.get_keyword(CTokenType.DEFAULT))
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be id or case or default")
         node.register_token(self.eat(TokenType.COLON))
         node.update(stmt=self.statement())
         return node
 
     def expression_statement(self):
@@ -1996,50 +2003,50 @@
         """
         <selection-statement> ::= if "(" <expression> ")" <statement>
                                 | if "(" <expression> ")" <statement> else <statement>
                                 | switch "(" <expression> ")" <statement>
         """
         node = SelectionStatement()
         if self.current_token.type in (CTokenType.IF, CTokenType.SWITCH):
-            node.update(if_keyword=self.keyword())
+            node.update(if_keyword=self.get_keyword())
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be if or switch")
         node.register_token(self.eat(TokenType.LPAREN))
         node.update(expr=self.expression())
         node.register_token(self.eat(TokenType.RPAREN))
         node.update(if_stmt=self.statement())
         if self.current_token.type == CTokenType.ELSE:
-            node.update(else_keyword=self.keyword())
+            node.update(else_keyword=self.get_keyword())
             node.update(else_stmt=self.statement())
         return node
 
     def iteration_statement(self):
         """
         <iteration-statement> ::= while "(" <expression> ")" <statement>
                                 | do <statement> while "(" <expression> ")" ";"
                                 | for "(" {<expression>}? ";" {<expression>}? ";" {<expression>}? ")" <statement>
                                 | for "(" <declaration> <expression>? ";" <expression>? ")" <statement>
         """
         node = IterationStatement()
         if self.current_token.type == CTokenType.WHILE:
-            node.update(keyword=self.keyword())
+            node.update(keyword=self.get_keyword())
             node.register_token(self.eat(TokenType.LPAREN))
             node.update(expr=self.expression())
             node.register_token(self.eat(TokenType.RPAREN))
             node.update(stmt=self.statement())
         elif self.current_token.type == CTokenType.DO:
-            node.update(keyword=self.keyword())
+            node.update(keyword=self.get_keyword())
             node.update(stmt=self.statement())
-            node.update(while_keyword=self.keyword())
+            node.update(while_keyword=self.get_keyword())
             node.register_token(self.eat(TokenType.LPAREN))
             node.update(expr=self.expression())
             node.register_token(self.eat(TokenType.RPAREN))
             node.register_token(self.eat(TokenType.SEMI))
         elif self.current_token.type == CTokenType.FOR:
-            node.update(keyword=self.keyword())
+            node.update(keyword=self.get_keyword())
 
             exprs = []
             node.register_token(self.eat(TokenType.LPAREN))
             # for "(" <declaration> <expression>? ";" <expression>? ")" <statement>
             if self.current_token.type in self.cfirst_set.declaration:
                 node.update(declaration=self.declaration())
                 if self.current_token.type in self.cfirst_set.expression:
@@ -2072,23 +2079,23 @@
                            | continue ";"
                            | break ";"
                            | return {<expression>}? ";"
         """
         node = JumpStatement()
         if self.current_token.type in self.cfirst_set.jump_statement:
             if self.current_token.type == CTokenType.GOTO:
-                node.update(keyword=self.keyword())
+                node.update(keyword=self.get_keyword())
                 node.update(expr=self.identifier())
                 add_ast_type(node.expr, C_CSS.GOTO_LABEL)
             elif self.current_token.type == CTokenType.RETURN:
-                node.update(keyword=self.keyword())
+                node.update(keyword=self.get_keyword())
                 if self.current_token.type in self.cfirst_set.expression:
                     node.update(expr=self.expression())
             else:
-                node.update(keyword=self.keyword())
+                node.update(keyword=self.get_keyword())
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be goto continue break return")
         node.register_token(self.eat(TokenType.SEMI))
         return node
 
     def identifier(self):
         """
@@ -2104,71 +2111,26 @@
         elif bool(re.match(r"^[A-Z0-9_]+$", token_value)):
             # ID 全部为 大写/数字/下划线, 很可能为宏
             add_ast_type(node, CSS.MACRO_DEFINE)
             GDT.register_id(node.id, CSS.MACRO_DEFINE)
 
         return node
 
-    def keyword(self, token_type: Enum = None, css_type: Enum = None):
-        """
-        keyword
-
-        @token_type: keyword 的类型,默认为 current_token.type
-        @class_name: 修改 Keyword 的类名
-        """
-        keyword = Keyword(self.current_token.value)
-        if token_type:
-            keyword.register_token(self.eat(token_type))
-        else:
-            keyword.register_token(self.eat())
-        if css_type is not None:
-            add_ast_type(keyword, css_type)
-        return keyword
-
     def string(self):
         """
         string
         """
-        return self._string_inside_format(self.current_token)
-
-    def _string_inside_format(self, token: Token):
-        """
-        取出其中格式化字符 %d %x \n 并新建 token
-        """
-        pattern = r"(%[0-9ldiufFeEgGxXoscpaAn]+|(?:\\\\|\\n|\\t|\\v|\\f))"
-        sub_strings = re.split(pattern, token.value)
-        new_asts = []
-        line = token.line
-        column = token.column - len(token.value)
-        for sub_string in sub_strings:
-            if len(sub_string) == 0:
-                continue
-            column += len(sub_string)
-            token = Token(TokenType.STRING, sub_string, line, column)
-            if bool(re.match(r"%[0-9ldiufFeEgGxXoscpaAn]+", sub_string)):
-                token.class_list.add("Format")
-            elif sub_string in ["\\n", "\\t", "\\f", "\\v", "\\a", "\\b", "\\\\"]:
-                token.class_list.add("Control")
-
-            self._register_token(token)
-            node = String(token.value)
-            node.register_token([token])
-            new_asts.append(node)
-
-        self.current_token = self.lexer.get_next_token()
-        self._skip()
-        self.after_eat()
-        return new_asts
+        return self.string_inside_format(self.current_token)
 
     def static_assert_declaration(self):
         """
         <static_assert-declaration> ::= _Static_assert "(" <constant-expression> "," <string> ")"
         """
         node = StaticAssertDeclaration()
-        node.update(keyword=self.keyword(CTokenType._STATIC_ASSERT))
+        node.update(keyword=self.get_keyword(CTokenType._STATIC_ASSERT))
         node.register_token(self.eat(TokenType.LPAREN))
         node.update(const_expr=self.constant_expression())
         node.register_token(self.eat(TokenType.COMMA))
         node.update(string=self.string())
         return node
 
     def group(self):
@@ -2257,18 +2219,18 @@
         <if-group> ::= "#" if <constant-expression> <CRLF>
                      | "#" ifdef <identifier> <CRLF
                      | "#" ifndef <identifier> <CRLF>
         """
         self.eat(TokenType.HASH)
         node = IfGroup()
         if self.current_token.type == CTokenType.IF_P:
-            node.update(keyword=self.keyword(CTokenType.IF_P, CSS.PREPROCESS))
+            node.update(keyword=self.get_keyword(CTokenType.IF_P, CSS.PREPROCESS))
             node.update(const_expr=self.constant_expression())
         elif self.current_token.type in (CTokenType.IFDEF, CTokenType.IFNDEF):
-            node.update(keyword=self.keyword(css_type=CSS.PREPROCESS))
+            node.update(keyword=self.get_keyword(css_type=CSS.PREPROCESS))
             node.update(id=self.identifier())
             add_ast_type(node.id, CSS.MACRO_DEFINE)
             GDT.register_id(node.id.id, CSS.MACRO_DEFINE)
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be if ifdef ifndef")
         self.eat_lf()
         self._end_preprocessing()
@@ -2276,42 +2238,42 @@
 
     def elif_group(self):
         """
         <elif-group> ::= "#" elif <constant-expression> <CRLF>
         """
         self.eat(TokenType.HASH)
         node = ElifGroup()
-        node.update(keyword=self.keyword(CTokenType.ELIF, css_type=CSS.PREPROCESS))
+        node.update(keyword=self.get_keyword(CTokenType.ELIF, css_type=CSS.PREPROCESS))
         node.update(const_expr=self.constant_expression())
         self.eat_lf()
         self._end_preprocessing()
         return node
 
     def else_group(self):
         """
         <else-group> ::= "#" else <CRLF>
         """
         self.eat(TokenType.HASH)
         node = ElseGroup()
         if self.current_token.type == CTokenType.ELSE:
             self.current_token.type == CTokenType.ELSE_P
-            node.update(keyword=self.keyword(CTokenType.ELSE_P, css_type=CSS.PREPROCESS))
+            node.update(keyword=self.get_keyword(CTokenType.ELSE_P, css_type=CSS.PREPROCESS))
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be else")
         self.eat_lf()
         self._end_preprocessing()
         return node
 
     def endif_line(self):
         """
         <endif-line> ::= "#" endif <CRLF>
         """
         self.eat(TokenType.HASH)
         node = EndifLine()
-        node.update(keyword=self.keyword(CTokenType.ENDIF, css_type=CSS.PREPROCESS))
+        node.update(keyword=self.get_keyword(CTokenType.ENDIF, css_type=CSS.PREPROCESS))
         self.eat_lf()
         self._end_preprocessing()
         # if self.current_token.type in self.cfirst_set.external_declaration:
         #     node.update(group=self.external_declaration())
         return node
 
     def control_line(self):
@@ -2328,18 +2290,18 @@
                          | "#" <CRLF>
 
         <pp-token> ::= any
         """
         self.eat(TokenType.HASH)
         node = ControlLine()
         if self.current_token.type == CTokenType.INCLUDE:
-            node.update(keyword=self.keyword(css_type=CSS.PREPROCESS))
+            node.update(keyword=self.get_keyword(css_type=CSS.PREPROCESS))
             node.update(header_name=self.header_name())
         elif self.current_token.type == CTokenType.DEFINE:
-            node.update(keyword=self.keyword(css_type=CSS.PREPROCESS))
+            node.update(keyword=self.get_keyword(css_type=CSS.PREPROCESS))
             # define 这里需要考虑空格的影响, 作为函数括号要求前面无空格
             # define A(a,b) 1
             # define A (a,b)
             #
             # 这里禁用skip_space和skip_invisible_characters以单步匹配下一个 token
             self.skip_space = False
             self.skip_invisible_characters = False
@@ -2350,39 +2312,39 @@
                 # paramters 或 parameterization 被定义了说明是函数
                 node.register_token(self.eat(TokenType.LPAREN))
                 if self.current_token.type in self.cfirst_set.identifier_list:
                     node.update(paramters=self.identifier_list())
                 if self.current_token.type == TokenType.COMMA:
                     node.register_token(self.eat())
                 if self.current_token.type == TokenType.VARARGS:
-                    node.update(parameterization=self.keyword(TokenType.VARARGS))
+                    node.update(parameterization=self.get_keyword(TokenType.VARARGS))
                 node.register_token(self.eat(TokenType.RPAREN))
 
             pp_tokens = []
             while self.current_token.type not in (TokenType.EOF, TokenType.LF):
                 if self.current_token.type == TokenType.BACK_SLASH:
                     pp_tokens.append(self.pp_token())
                 pp_tokens.append(self.pp_token())
             node.update(pp_tokens=pp_tokens)
 
         elif self.current_token.type == CTokenType.UNDEF:
-            node.update(keyword=self.keyword(css_type=CSS.PREPROCESS))
+            node.update(keyword=self.get_keyword(css_type=CSS.PREPROCESS))
             node.update(id=self.identifier())
         elif self.current_token.type in (CTokenType.LINE, CTokenType.ERROR, CTokenType.PRAGMA):
-            node.update(keyword=self.keyword(css_type=CSS.PREPROCESS))
+            node.update(keyword=self.get_keyword(css_type=CSS.PREPROCESS))
             node.update(id=self.identifier())
 
         if node.id is not None:
             if node.paramters is not None:
                 # paramters 被定义了说明是函数
                 # TODO: parameterization
                 add_ast_type(node.id, CSS.MACRO_FUNCTION)
                 arguments = []
                 for i_node in node.paramters:
-                    arguments.append(Argument(name=i_node.id, type=None))
+                    arguments.append(FuncArgument(name=i_node.id, type=None))
                 GDT.register_function(node.id.id, arguments, (), CSS.MACRO_FUNCTION)
             else:
                 # 常规宏定义变量
                 add_ast_type(node.id, CSS.MACRO_DEFINE)
                 GDT.register_id(node.id.id, CSS.MACRO_DEFINE)
 
         self.eat_lf()
@@ -2428,24 +2390,22 @@
             column = -1
             while self.current_token.type != TokenType.RANGLE_BRACE:
                 if self.current_token.type in (TokenType.EOF, TokenType.LF):
                     break
                 result += self.current_token.value
                 line = self.current_token.line
                 column = self.current_token.column
-                self.current_token = self.lexer.get_next_token()
-                self._skip()
-                self.after_eat()
+                self.manual_get_next_token()
             if self.current_token.type == TokenType.EOF:
                 self.error(ErrorCode.UNEXPECTED_TOKEN, "miss >")
             if self.current_token.type == TokenType.LF:
                 self.error(ErrorCode.UNEXPECTED_TOKEN, "\\n inside include <>")
 
             new_token = Token(TokenType.STRING, result, line, column)
             file_path = String(new_token.value)
             file_path.register_token([new_token])
-            self._register_token(new_token)
+            self.manual_register_token(new_token)
             node.update(file_path=file_path)
             node.register_token(self.eat(TokenType.RANGLE_BRACE))
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, '<> or ""')
         return node
```

### Comparing `syntaxlight-0.0.5/syntaxlight/parsers/json_parser.py` & `syntaxlight-0.0.6/syntaxlight/parsers/json_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.5/syntaxlight/parsers/parser.py` & `syntaxlight-0.0.6/syntaxlight/parsers/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from ..lexers.lexer import Lexer, Token, TokenType, TTYColor
 from ..error import ParserError, ErrorCode
 from enum import Enum
-from ..ast import AST
+from ..ast import AST, Keyword, add_ast_type, Identifier, Punctuator, String
 from typing import List
 import sys
 import html
 import traceback
-import copy
+import re
+
 
 DEBUG = False
 DEBUG = True
 
 
 class Parser:
     def __init__(
@@ -68,23 +69,26 @@
         语法解析过程中的警告信息
         """
         if not self.display_warning:
             return
 
         warning_color = TTYColor.MAGENTA
 
-        sys.stderr.write(self.lexer.ttyinfo("warning: ", warning_color) + message + "\n")
-        sys.stderr.write(self.lexer.ttyinfo(str(ast), warning_color))
+        sys.stderr.write(
+            self.lexer.ttyinfo("warning: ", warning_color, underline=False) + message + "\n"
+        )
+        # sys.stderr.write(self.lexer.ttyinfo(str(ast), warning_color))
 
     def _log_trace(self):
         """
         查看 python 函数调用栈
         """
         if DEBUG:
-            stack_trace = traceback.extract_stack()
+            # 前4后2不重要
+            stack_trace = traceback.extract_stack()[4:-2]
             function_length = 0
             line_length = 0
             for stack in stack_trace:
                 _, line_number, function_name, _ = stack
                 function_length = max(function_length, len(function_name))
                 line_length = max(line_length, len(str(line_number)))
             for stack in stack_trace:
@@ -125,17 +129,33 @@
                 expected_value = token_type.name
             self.error(
                 error_code=ErrorCode.UNEXPECTED_TOKEN,
                 token=self.current_token,
                 message=f"should match {expected_value} but got {current_value}",
             )
 
+    def manual_get_next_token(self):
+        """
+        正常情况下调用 eat 获取下一个 token, 如果需要合并多个 token 并生成一个新的 token 时可调用此函数
+        """
+        self.current_token = self.lexer.get_next_token()
+        self._skip()
+        self.after_eat()
+
+    def manual_register_token(self, token):
+        """
+        正常情况下不需要手动将 token 注册到 _token_list 当中, eat 内部会调用此方法
+
+        如果因为合并或分割创建了新的 token 可调用此方法注册
+        """
+        self._register_token(token)
+
     def after_eat(self):
         """
-        eat 之后对于 current_token 的一些操作
+        如果希望在 eat 之后对于 current_token 进行一些操作, 比如查 GDT 或处理预处理关键字, 可在继承类中重载此方法
         """
         return
 
     def _skip(self) -> List[Token]:
         """
         跳过不可见字符和空格
 
@@ -257,7 +277,70 @@
                         brace_depth += 1
 
             html_str += f'<span class="{token.get_css_class()}">{html.escape(token.value)}</span>'
         return html_str
 
     def parse(self):
         raise NotImplementedError(self.__class__.__name__ + " must override the parse function")
+
+    def get_keyword(self, token_type: Enum = None, css_type: Enum = None) -> Keyword:
+        """
+        keyword
+
+        @token_type: keyword 的类型,默认为 current_token.type
+        @class_name: 修改 Keyword 的类名
+        """
+        keyword = Keyword(self.current_token.value)
+        if token_type:
+            keyword.register_token(self.eat(token_type))
+        else:
+            keyword.register_token(self.eat())
+        if css_type is not None:
+            add_ast_type(keyword, css_type)
+        return keyword
+
+    def identifier(self) -> Identifier:
+        """
+        ID
+        """
+        node = Identifier(self.current_token.value)
+        node.register_token(self.eat(TokenType.ID))
+        return node
+
+    def punctuator(self, token_type: Enum = None) -> Punctuator:
+        """
+        获取运算符
+        """
+        node = Punctuator(self.current_token.value)
+        if token_type is None:
+            node.register_token(self.eat())
+        else:
+            node.register_token(self.eat(token_type))
+        return node
+
+    def string_inside_format(self, token: Token) -> List[String]:
+        """
+        取出其中格式化字符(如 %d %x \n) 并新建 token
+        """
+        pattern = r"(%[0-9ldiufFeEgGxXoscpaAn]+|(?:\\\\|\\n|\\t|\\v|\\f))"
+        sub_strings = re.split(pattern, token.value)
+        new_asts = []
+        line = token.line
+        column = token.column - len(token.value)
+        token_type = token.type
+        for sub_string in sub_strings:
+            if len(sub_string) == 0:
+                continue
+            column += len(sub_string)
+            token = Token(token_type, sub_string, line, column)
+            if bool(re.match(r"%[0-9ldiufFeEgGxXoscpaAn]+", sub_string)):
+                token.class_list.add("Format")
+            elif sub_string in ["\\n", "\\t", "\\f", "\\v", "\\a", "\\b", "\\\\"]:
+                token.class_list.add("Control")
+
+            self.manual_register_token(token)
+            node = String(token.value)
+            node.register_token([token])
+            new_asts.append(node)
+
+        self.manual_get_next_token()
+        return new_asts
```

### Comparing `syntaxlight-0.0.5/syntaxlight/parsers/toml_parser.py` & `syntaxlight-0.0.6/syntaxlight/parsers/toml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.5/syntaxlight/parsers/xml_parser.py` & `syntaxlight-0.0.6/syntaxlight/parsers/xml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.0.5/syntaxlight/syntax_parse.py` & `syntaxlight-0.0.6/syntaxlight/syntax_parse.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,150 +2,132 @@
 from .lexers import *
 from .error import Error
 from .parsers import *
 from .ast import display_ast
 import sys
 
 
+SUPPORTED_SYNTAX = {
+    "json": {"lexer": JsonLexer, "parser": JsonParser, "suffix": ["json"]},
+    "c": {"lexer": CLexer, "parser": CParser, "suffix": ["c", "h"]},
+    "lua": {"lexer": LuaLexer, "parser": LuaParser, "suffix": ["lua"]},
+    "bnf": {"lexer": BNFLexer, "parser": BNFParser, "suffix": ["bnf"]},
+    "makefile": {"lexer": None, "parser": None, "suffix": ["Makefile", "mk", "mak", "makefile"]},
+    "java": {"lexer": None, "parser": None, "suffix": ["java"]},
+    "rust": {"lexer": None, "parser": None, "suffix": ["rs"]},
+    "javascript": {"lexer": None, "parser": None, "suffix": ["js"]},
+    "typescript": {"lexer": None, "parser": None, "suffix": ["ts", "tsx", "tsc"]},
+    "pascal": {"lexer": None, "parser": None, "suffix": ["pas"]},
+    "toml": {"lexer": TomlLexer, "parser": TomlParser, "suffix": ["toml"]},
+    "xml": {"lexer": XmlLexer, "parser": XmlParser, "suffix": ["xml"]},
+    "shell": {"lexer": ShellLexer, "parser": ShellParser, "suffix": ["sh"]},
+}
+
+
 def parse(
-    text: str, language: str = "guess", file_path=None, show_error_context=True, save_ast_tree=False
+    text: str, language=None, file_path=None, show_error_context=True, save_ast_tree=False
 ) -> str:
-    assert type(text) == str
-    assert type(language) == str
-
     if len(text) == 0:
         return ""
 
-    language = language.lower()
-    lexer = get_lexer(text, language)
-    if file_path is not None:
-        lexer.file_path = file_path
-    parser = get_parser(lexer)
+    parser = get_parser(text, language)
+    parser.lexer.file_path = file_path
 
     try:
         parser.parse()
     except Error as e:
         sys.stderr.write(e.message)
         if show_error_context:
             sys.stderr.write(e.context)
     else:
-        display_ast(parser.root,parser.sub_roots, save_ast_tree=save_ast_tree)
+        display_ast(parser.root, parser.sub_roots, save_ast_tree=save_ast_tree)
         # print(parser.node)
         return parser.to_html()
 
 
-def parse_file(
-    file_path: str, language: str = "guess", show_error_context=True, save_ast_tree=False
-) -> str:
+def parse_file(file_path: str, language=None, show_error_context=True, save_ast_tree=False) -> str:
     if not os.path.exists(file_path):
         print(f"{file_path} file not exsist")
 
     with open(file_path, "r", encoding="utf-8") as f:
         text = f.read()
 
-    if language == "guess":
+    if language is None:
         language = guess_language(file_path)
-        if language is None:
-            print(f"unknown syntax {file_path}")
-            exit(1)
 
     return parse(
         text,
-        language,
+        language=language,
         file_path=file_path,
         show_error_context=show_error_context,
         save_ast_tree=save_ast_tree,
     )
 
 
 def guess_language(file_path: str) -> str:
     """
     通过文件名猜测文法类型
     """
-    file_name = file_path.split(os.sep)[-1]
+    suffix_name = file_path.split(os.sep)[-1].split(".")[-1]
+    for language in SUPPORTED_SYNTAX:
+        if suffix_name in SUPPORTED_SYNTAX[language]["suffix"]:
+            return language
 
-    languages = {
-        "json": ["json"],
-        "c": ["c", "h"],
-        "lua": ["lua"],
-        "bnf": ["bnf"],
-        "Makefile": ["Makefile", "mk", "mak"],
-        "java": ["java"],
-        "rust": ["rs"],
-        "javascript": ["js"],
-        "typescript": ["ts", "tsx", "tsc"],
-        "pascal": ["pas"],
-        "toml": ["toml"],
-        "xml": ["xml"],
-        "shell": ["sh"],
-        "bnf": ["bnf"],
-    }
-
-    if "." in file_name:
-        suffix = file_name.split(".")[-1]
-        for language, suffix_names in languages.items():
-            if suffix in suffix_names:
-                return language
-        file_name = file_name.split(".")[:-1]
+    if suffix_name in SUPPORTED_SYNTAX:
+        return suffix_name
 
-    for language, suffix_names in languages.items():
-        if file_name in suffix_names:
-            return language
+    print("fail to guess language")
+    show_help_info()
+    exit(1)
 
-    return None
+
+def show_help_info():
+    print(f"supported language:")
+    for language in SUPPORTED_SYNTAX:
+        print(f"{language:>10}:", SUPPORTED_SYNTAX[language]["suffix"])
+    exit(1)
 
 
 def get_tokens(lexer: Lexer):
     token = lexer.get_next_token()
     tokens = [token]
     while token.type.value != "EOF":
-        # if token.type.value == 'ID':
-        # print(token)
-        # print(token)
         try:
             token = lexer.get_next_token()
             tokens.append(token)
         except Error as e:
             print(e.message)
             print(e.context)
     return tokens
 
 
-def get_lexer(code: str, language: str) -> Lexer:
-    language = language.lower()
-
-    lexers = {
-        "c": CLexer,
-        "lua": LuaLexer,
-        "json": JsonLexer,
-        "toml": TomlLexer,
-        "xml": XmlLexer,
-        "shell": ShellLexer,
-        "bnf": BNFLexer,
-    }
-
-    lexer_class = lexers.get(language, None)
-    if lexer_class is None:
-        print("unknown language type: ", language)
+def get_lexer(code_or_path: str, language: str = None) -> Lexer:
+    """
+    @code_or_path: 代码或者文件的路径
+    @lanaguge: 选择的语言, 如果第一个参数为文件路径则不需要传入 language
+    """
+    code, language = _preprocess(code_or_path, language)
+    if language not in SUPPORTED_SYNTAX:
+        print("lexer not support")
+        show_help_info()
         exit(1)
+    return SUPPORTED_SYNTAX[language]["lexer"](code)
 
-    return lexers[language](code)
 
+def get_parser(code_or_path: str, language: str = None) -> Parser:
+    code, language = _preprocess(code_or_path, language)
+    lexer = get_lexer(code, language)
+    parser = SUPPORTED_SYNTAX[language]["parser"](lexer)
+    return parser
 
-def get_parser(lexer: Lexer) -> Parser:
-    parsers = {
-        "json": JsonParser,
-        "toml": TomlParser,
-        "c": CParser,
-        "xml": XmlParser,
-        "shell": ShellParser,
-        "bnf": BNFParser,
-    }
 
-    syntax_type = lexer.__class__.__name__.replace("Lexer", "").lower()
-    parser_class = parsers.get(syntax_type, None)
+def _preprocess(code_or_path: str, language: str = None):
+    if os.path.exists(code_or_path):
+        with open(code_or_path, "r", encoding="utf-8") as f:
+            code = f.read()
 
-    if parser_class is None:
-        print("unknown lexer type: ", lexer.__class__.__name__)
-        exit(1)
+        if language is None:
+            language = guess_language(code_or_path)
+    else:
+        code = code_or_path
 
-    return parsers[syntax_type](lexer)
+    return code, language
```

### Comparing `syntaxlight-0.0.5/PKG-INFO` & `syntaxlight-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntaxlight
-Version: 0.0.5
+Version: 0.0.6
 Summary: syntax highlight based on EBNF
 Home-page: https://github.com/luzhixing12345/syntaxlight
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


# Comparing `tmp/minecraft_script-0.1.408.tar.gz` & `tmp/minecraft_script-0.1.409.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft_script-0.1.408.tar", last modified: Thu Jul 27 21:12:11 2023, max compression
+gzip compressed data, was "minecraft_script-0.1.409.tar", last modified: Thu Jul 27 23:05:45 2023, max compression
```

## Comparing `minecraft_script-0.1.408.tar` & `minecraft_script-0.1.409.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 21:12:11.229390 minecraft_script-0.1.408/
--rw-rw-rw-   0        0        0     1684 2023-07-27 21:12:11.229390 minecraft_script-0.1.408/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 21:12:11.208375 minecraft_script-0.1.408/minecraft_script/
--rw-rw-rw-   0        0        0     1426 2023-07-26 22:22:30.000000 minecraft_script-0.1.408/minecraft_script/__init__.py
--rw-rw-rw-   0        0        0      378 2023-07-26 22:23:11.000000 minecraft_script-0.1.408/minecraft_script/__main__.py
--rw-rw-rw-   0        0        0     1168 2023-07-26 12:31:03.000000 minecraft_script-0.1.408/minecraft_script/build_interpreter.py
-drwxrwxrwx   0        0        0        0 2023-07-27 21:12:11.226388 minecraft_script-0.1.408/minecraft_script/build_templates/
--rw-rw-rw-   0        0        0       41 2023-07-25 21:27:11.000000 minecraft_script-0.1.408/minecraft_script/build_templates/function_tags.json
--rw-rw-rw-   0        0        0      131 2023-07-25 21:27:11.000000 minecraft_script-0.1.408/minecraft_script/build_templates/pack.mcmeta
--rw-rw-rw-   0        0        0     2276 2023-07-26 12:32:37.000000 minecraft_script-0.1.408/minecraft_script/builder.py
--rw-rw-rw-   0        0        0       72 2023-07-27 21:10:53.000000 minecraft_script-0.1.408/minecraft_script/common.py
--rw-rw-rw-   0        0        0     2070 2023-07-26 21:29:02.000000 minecraft_script-0.1.408/minecraft_script/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-27 21:12:11.228389 minecraft_script-0.1.408/minecraft_script/grammar/
--rw-rw-rw-   0        0        0       88 2023-07-25 21:27:11.000000 minecraft_script-0.1.408/minecraft_script/grammar/LANG_KEYWORDS.json
--rw-rw-rw-   0        0        0      579 2023-07-27 17:14:29.000000 minecraft_script-0.1.408/minecraft_script/grammar/LANG_TOKENS.json
--rw-rw-rw-   0        0        0     5512 2023-07-27 21:07:11.000000 minecraft_script-0.1.408/minecraft_script/interpreter.py
--rw-rw-rw-   0        0        0     4883 2023-07-27 20:35:04.000000 minecraft_script-0.1.408/minecraft_script/lexer.py
--rw-rw-rw-   0        0        0     4085 2023-07-27 20:20:40.000000 minecraft_script-0.1.408/minecraft_script/nodes.py
--rw-rw-rw-   0        0        0     9244 2023-07-27 20:43:18.000000 minecraft_script-0.1.408/minecraft_script/parser.py
--rw-rw-rw-   0        0        0     2084 2023-07-25 21:27:11.000000 minecraft_script-0.1.408/minecraft_script/shell_commands.py
--rw-rw-rw-   0        0        0     1143 2023-07-25 21:27:11.000000 minecraft_script-0.1.408/minecraft_script/text_additions.py
--rw-rw-rw-   0        0        0      211 2023-07-25 21:27:11.000000 minecraft_script-0.1.408/minecraft_script/tokens.py
--rw-rw-rw-   0        0        0     5159 2023-07-26 21:57:47.000000 minecraft_script-0.1.408/minecraft_script/types.py
-drwxrwxrwx   0        0        0        0 2023-07-27 21:12:11.222382 minecraft_script-0.1.408/minecraft_script.egg-info/
--rw-rw-rw-   0        0        0     1684 2023-07-27 21:12:11.000000 minecraft_script-0.1.408/minecraft_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2023-07-27 21:12:11.000000 minecraft_script-0.1.408/minecraft_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 21:12:11.000000 minecraft_script-0.1.408/minecraft_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-27 21:12:11.000000 minecraft_script-0.1.408/minecraft_script.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 21:12:11.229390 minecraft_script-0.1.408/setup.cfg
--rw-rw-rw-   0        0        0     1107 2023-07-27 14:00:51.000000 minecraft_script-0.1.408/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 23:05:45.085451 minecraft_script-0.1.409/
+-rw-rw-rw-   0        0        0     1684 2023-07-27 23:05:45.084450 minecraft_script-0.1.409/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 23:05:45.067435 minecraft_script-0.1.409/minecraft_script/
+-rw-rw-rw-   0        0        0     1426 2023-07-26 22:22:30.000000 minecraft_script-0.1.409/minecraft_script/__init__.py
+-rw-rw-rw-   0        0        0      378 2023-07-26 22:23:11.000000 minecraft_script-0.1.409/minecraft_script/__main__.py
+-rw-rw-rw-   0        0        0     1168 2023-07-26 12:31:03.000000 minecraft_script-0.1.409/minecraft_script/build_interpreter.py
+drwxrwxrwx   0        0        0        0 2023-07-27 23:05:45.081447 minecraft_script-0.1.409/minecraft_script/build_templates/
+-rw-rw-rw-   0        0        0       41 2023-07-25 21:27:11.000000 minecraft_script-0.1.409/minecraft_script/build_templates/function_tags.json
+-rw-rw-rw-   0        0        0      131 2023-07-25 21:27:11.000000 minecraft_script-0.1.409/minecraft_script/build_templates/pack.mcmeta
+-rw-rw-rw-   0        0        0     2276 2023-07-26 12:32:37.000000 minecraft_script-0.1.409/minecraft_script/builder.py
+-rw-rw-rw-   0        0        0       72 2023-07-27 23:04:46.000000 minecraft_script-0.1.409/minecraft_script/common.py
+-rw-rw-rw-   0        0        0     2070 2023-07-26 21:29:02.000000 minecraft_script-0.1.409/minecraft_script/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-27 23:05:45.083449 minecraft_script-0.1.409/minecraft_script/grammar/
+-rw-rw-rw-   0        0        0      158 2023-07-27 21:44:13.000000 minecraft_script-0.1.409/minecraft_script/grammar/LANG_KEYWORDS.json
+-rw-rw-rw-   0        0        0      579 2023-07-27 17:14:29.000000 minecraft_script-0.1.409/minecraft_script/grammar/LANG_TOKENS.json
+-rw-rw-rw-   0        0        0     5608 2023-07-27 22:03:53.000000 minecraft_script-0.1.409/minecraft_script/interpreter.py
+-rw-rw-rw-   0        0        0     4883 2023-07-27 22:36:13.000000 minecraft_script-0.1.409/minecraft_script/lexer.py
+-rw-rw-rw-   0        0        0     4370 2023-07-27 22:03:28.000000 minecraft_script-0.1.409/minecraft_script/nodes.py
+-rw-rw-rw-   0        0        0     9662 2023-07-27 23:02:16.000000 minecraft_script-0.1.409/minecraft_script/parser.py
+-rw-rw-rw-   0        0        0     2084 2023-07-25 21:27:11.000000 minecraft_script-0.1.409/minecraft_script/shell_commands.py
+-rw-rw-rw-   0        0        0     1143 2023-07-25 21:27:11.000000 minecraft_script-0.1.409/minecraft_script/text_additions.py
+-rw-rw-rw-   0        0        0      211 2023-07-25 21:27:11.000000 minecraft_script-0.1.409/minecraft_script/tokens.py
+-rw-rw-rw-   0        0        0     5612 2023-07-27 22:30:35.000000 minecraft_script-0.1.409/minecraft_script/types.py
+drwxrwxrwx   0        0        0        0 2023-07-27 23:05:45.079446 minecraft_script-0.1.409/minecraft_script.egg-info/
+-rw-rw-rw-   0        0        0     1684 2023-07-27 23:05:45.000000 minecraft_script-0.1.409/minecraft_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-07-27 23:05:45.000000 minecraft_script-0.1.409/minecraft_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 23:05:45.000000 minecraft_script-0.1.409/minecraft_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-27 23:05:45.000000 minecraft_script-0.1.409/minecraft_script.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 23:05:45.085451 minecraft_script-0.1.409/setup.cfg
+-rw-rw-rw-   0        0        0     1107 2023-07-27 14:00:51.000000 minecraft_script-0.1.409/setup.py
```

### Comparing `minecraft_script-0.1.408/PKG-INFO` & `minecraft_script-0.1.409/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft_script
-Version: 0.1.408
+Version: 0.1.409
 Summary: Minecraft Script Programming language
 Author: Joyful-Bard
 Author-email: <thisis@notarealemail.com>
 Keywords: minecraft,mc,script,language
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `minecraft_script-0.1.408/minecraft_script/__init__.py` & `minecraft_script-0.1.409/minecraft_script/__init__.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.408/minecraft_script/build_interpreter.py` & `minecraft_script-0.1.409/minecraft_script/build_interpreter.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.408/minecraft_script/builder.py` & `minecraft_script-0.1.409/minecraft_script/builder.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.408/minecraft_script/errors.py` & `minecraft_script-0.1.409/minecraft_script/errors.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.408/minecraft_script/grammar/LANG_TOKENS.json` & `minecraft_script-0.1.409/minecraft_script/grammar/LANG_TOKENS.json`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.408/minecraft_script/interpreter.py` & `minecraft_script-0.1.409/minecraft_script/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .text_additions import text_error, text_underline
-from .types import Number, List, Function, BuiltinFunction
+from .types import Number, List, Boolean, Function, BuiltinFunction
 from .errors import MCSNameError, MCSTypeError, MCSIndexError
 
 
 class Context:
     def __init__(self, display_name: str, symbol_table, parent=None):
         self.display_name = display_name
         self.parent: None | Context = parent
@@ -55,14 +55,17 @@
     def visit_NumberNode(self, node, context) -> int:
         return node.get_value()
 
     def visit_ListNode(self, node, context):
         value_array = [self.visit(element, context) for element in node.array]
         return List(value_array)
 
+    def visit_BooleanNode(self, node, context):
+        return Boolean(node.value)
+
     def visit_ListGetNode(self, node, context):
         name = node.name_token.value
         index = self.visit(node.index, context)
         variable = context.symbol_table.get(name)
 
         if type(variable).__name__ == 'List':
             value = variable.get_index(index)
```

### Comparing `minecraft_script-0.1.408/minecraft_script/lexer.py` & `minecraft_script-0.1.409/minecraft_script/lexer.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.408/minecraft_script/nodes.py` & `minecraft_script-0.1.409/minecraft_script/nodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,25 @@
     def __str__(self):
         return f'array get: {self.name_token.value} {self.index}'
 
     def __repr__(self):
         return f'ListGetNode({self.name_token !r}, {self.index !r})'
 
 
+class BooleanNode:
+    def __init__(self, value: str):
+        self.value = True if value == 'true' else False
+
+    def __str__(self):
+        return f'boolean: {str(self.value).lower()}'
+
+    def __repr__(self):
+        return f'BooleanNode({str(self.value).lower()})'
+
+
 class VariableAssignNode:
     def __init__(self, name_token: Token, value_node):
         self.name_token = name_token
         self.value_node = value_node
 
     def get_name(self) -> str:
         return self.name_token.value
@@ -136,8 +147,8 @@
     def __init__(self, statements: list):
         self.statements = statements
 
     def __str__(self):
         return f'Code Block: {self.statements}'
 
     def __repr__(self):
-        return f'CodeBlockNode({self.statements})'
+        return f'CodeBlockNode({self.statements})'
```

### Comparing `minecraft_script-0.1.408/minecraft_script/parser.py` & `minecraft_script-0.1.409/minecraft_script/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from .tokens import Token
 from .errors import MCSSyntaxError
 from .text_additions import text_underline
 from .nodes import NumberNode, BinaryOperationNode, UnaryOperationNode, VariableAssignNode, VariableAccessNode, \
-    FunctionAssignNode, FunctionCallNode, MultipleStatementsNode, ListNode, ListGetNode, CodeBlockNode
+    FunctionAssignNode, FunctionCallNode, MultipleStatementsNode, ListNode, ListGetNode, CodeBlockNode, BooleanNode
 
 
 class Parser:
     def __init__(self, token_list: list[Token]):
         self.token_list = token_list
         self.current_index = -1
         self.current_token = None
 
         self.advance()
 
     def advance(self):
-        self.current_index += 1
-        if self.current_index < len(self.token_list):
+        if self.current_index < len(self.token_list) - 1:
+            self.current_index += 1
             self.current_token = self.token_list[self.current_index]
 
     def parse(self):
         result = self.statement()
         return result
 
-    def factor(self) -> NumberNode | UnaryOperationNode | BinaryOperationNode | VariableAccessNode | FunctionCallNode | ListNode:
+    def factor(self) -> NumberNode | UnaryOperationNode | BinaryOperationNode | VariableAccessNode | FunctionCallNode | ListNode | ListGetNode | BooleanNode:
         token = self.current_token
 
         if token.value in ['+', '-']:
             self.advance()
             factor = self.factor()
             return UnaryOperationNode(token, factor)
 
@@ -44,14 +44,18 @@
         elif token.tt_type == 'TT_LEFT_PARENTHESIS':
             self.advance()
             expression = self.expression()
             if self.current_token.tt_type == 'TT_RIGHT_PARENTHESIS':
                 self.advance()
                 return expression
 
+        elif token.tt_type == 'TT_BOOLEAN':
+            self.advance()
+            return BooleanNode(token.value)
+
         elif token.tt_type == 'TT_LEFT_BRACKET':
             return self.array()
 
         elif token.tt_type == 'TT_NUMBER':
             self.advance()
             return NumberNode(token)
 
@@ -96,18 +100,24 @@
 
     def statement(self) -> MultipleStatementsNode:
         statements = []
         while self.current_token.tt_type == 'TT_NEWLINE':
             self.advance()
         statements.append(self.expression())
 
-        while self.current_token.tt_type == 'TT_NEWLINE':
-            while self.current_token.tt_type == 'TT_NEWLINE':
+        more_statements = True
+        while self.current_token.tt_type == 'TT_NEWLINE' and more_statements:
+            while self.current_token.tt_type == 'TT_NEWLINE' and more_statements:
+                index = self.current_index
                 self.advance()
-            statements.append(self.expression())
+                if index == self.current_index:
+                    more_statements = False
+
+            if more_statements:
+                statements.append(self.expression())
 
         return MultipleStatementsNode(statements)
 
     def function_define(self) -> FunctionAssignNode:
         self.advance()
 
         function_name_token = None
```

### Comparing `minecraft_script-0.1.408/minecraft_script/shell_commands.py` & `minecraft_script-0.1.409/minecraft_script/shell_commands.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.408/minecraft_script/text_additions.py` & `minecraft_script-0.1.409/minecraft_script/text_additions.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.408/minecraft_script/types.py` & `minecraft_script-0.1.409/minecraft_script/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,34 @@
     def __str__(self):
         return str([str(element) for element in self.array]).replace("'", "")
 
     def __repr__(self):
         return f'List({self.array})'
 
 
+class Boolean:
+    def __init__(self, value):
+        self.value = value
+
+    def logical_invert(self):
+        return not self.value
+
+    def logical_and(self, other):
+        return self.value and other
+
+    def logical_or(self, other):
+        return self.value or other
+
+    def __str__(self):
+        return str(self.value).lower()
+
+    def __repr__(self):
+        return f'Boolean({self.value})'
+
+
 class Function:
     def __init__(self, name: str, parameter_names: list[str], body_node, context):
         self.name = f'<function {name}>' if name else "<function anonymous>"
         self.parameter_names = parameter_names
         self.body_node = body_node
         self.context = context
 
@@ -95,15 +115,17 @@
         local_context = Context(self.name, local_symbol_table)
 
         for i in range(len(arguments)):
             arg_name = self.parameter_names[i]
             arg_value = arguments[i]
             local_context.symbol_table.set(arg_name, arg_value)
 
-        return local_interpreter.visit(self.body_node, local_context)
+        local_interpreter.visit(self.body_node, local_context)
+
+        return Boolean(False)
 
     def __str__(self):
         return f'{self.name}'
 
     def __repr__(self):
         return f'Function({self.name !r}, {self.parameter_names !r}, {self.body_node !r}, {self.context !r})'
 
@@ -112,54 +134,56 @@
     names = ['log', 'append', 'extend']
 
     def __init__(self, name):
         self.name = name
 
     def call(self, arguments: list):
         method = getattr(self, f'call_{self.name}', 'unknown_name')
-        method(arguments)
+        return method(arguments)
 
     @staticmethod
     def call_log(arguments: list):
         print(', '.join([str(argument) for argument in arguments]))
-        return Number(0)
+        return Boolean(False)
 
     @staticmethod
     def call_append(arguments: list):
         if len(arguments) > 2:
             MCSTypeError('append() takes 2 arguments')
             exit()
-        list: List = arguments[0]
+        base_list: List = arguments[0]
         value = arguments[1]
 
-        if type(list).__name__ != 'List':
-            MCSTypeError(f'{text_underline(f"{list}")} is not a list')
+        if isinstance(base_list, List):
+            MCSTypeError(f'{text_underline(f"{base_list}")} is not a list')
             exit()
 
-        new_list = list.array.append(value)
-        return new_list
+        base_list.array.append(value)
+
+        return base_list
 
     @staticmethod
     def call_extend(arguments: list):
         if len(arguments) > 2:
             MCSTypeError('append() takes 2 arguments')
             exit()
         base_list: List = arguments[0]
         extend_list: List = arguments[1]
 
-        if type(base_list).__name__ != 'List':
+        if not isinstance(base_list, List):
             MCSTypeError(f'{text_underline(f"{base_list}")} is not a list')
             exit()
 
-        if type(extend_list).__name__ != 'List':
+        if not isinstance(extend_list, List):
             MCSTypeError(f'{text_underline(f"{extend_list}")} is not a list')
             exit()
 
-        new_list = base_list.array.extend(extend_list.array)
-        return new_list
+        base_list.array.extend(extend_list.array)
+
+        return base_list
 
     def unknown_name(self, arguments: list):
         print(f'Interpreter built-in error ({self.name !r})')
         exit()
 
     def __str__(self):
         return f'<builtin function {self.name}>'
```

### Comparing `minecraft_script-0.1.408/minecraft_script.egg-info/PKG-INFO` & `minecraft_script-0.1.409/minecraft_script.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft-script
-Version: 0.1.408
+Version: 0.1.409
 Summary: Minecraft Script Programming language
 Author: Joyful-Bard
 Author-email: <thisis@notarealemail.com>
 Keywords: minecraft,mc,script,language
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `minecraft_script-0.1.408/minecraft_script.egg-info/SOURCES.txt` & `minecraft_script-0.1.409/minecraft_script.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.408/setup.py` & `minecraft_script-0.1.409/setup.py`

 * *Files identical despite different names*


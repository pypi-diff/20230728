# Comparing `tmp/minecraft_script-0.1.409.tar.gz` & `tmp/minecraft_script-0.1.410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft_script-0.1.409.tar", last modified: Thu Jul 27 23:05:45 2023, max compression
+gzip compressed data, was "minecraft_script-0.1.410.tar", last modified: Fri Jul 28 00:58:18 2023, max compression
```

## Comparing `minecraft_script-0.1.409.tar` & `minecraft_script-0.1.410.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 23:05:45.085451 minecraft_script-0.1.409/
--rw-rw-rw-   0        0        0     1684 2023-07-27 23:05:45.084450 minecraft_script-0.1.409/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 23:05:45.067435 minecraft_script-0.1.409/minecraft_script/
--rw-rw-rw-   0        0        0     1426 2023-07-26 22:22:30.000000 minecraft_script-0.1.409/minecraft_script/__init__.py
--rw-rw-rw-   0        0        0      378 2023-07-26 22:23:11.000000 minecraft_script-0.1.409/minecraft_script/__main__.py
--rw-rw-rw-   0        0        0     1168 2023-07-26 12:31:03.000000 minecraft_script-0.1.409/minecraft_script/build_interpreter.py
-drwxrwxrwx   0        0        0        0 2023-07-27 23:05:45.081447 minecraft_script-0.1.409/minecraft_script/build_templates/
--rw-rw-rw-   0        0        0       41 2023-07-25 21:27:11.000000 minecraft_script-0.1.409/minecraft_script/build_templates/function_tags.json
--rw-rw-rw-   0        0        0      131 2023-07-25 21:27:11.000000 minecraft_script-0.1.409/minecraft_script/build_templates/pack.mcmeta
--rw-rw-rw-   0        0        0     2276 2023-07-26 12:32:37.000000 minecraft_script-0.1.409/minecraft_script/builder.py
--rw-rw-rw-   0        0        0       72 2023-07-27 23:04:46.000000 minecraft_script-0.1.409/minecraft_script/common.py
--rw-rw-rw-   0        0        0     2070 2023-07-26 21:29:02.000000 minecraft_script-0.1.409/minecraft_script/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-27 23:05:45.083449 minecraft_script-0.1.409/minecraft_script/grammar/
--rw-rw-rw-   0        0        0      158 2023-07-27 21:44:13.000000 minecraft_script-0.1.409/minecraft_script/grammar/LANG_KEYWORDS.json
--rw-rw-rw-   0        0        0      579 2023-07-27 17:14:29.000000 minecraft_script-0.1.409/minecraft_script/grammar/LANG_TOKENS.json
--rw-rw-rw-   0        0        0     5608 2023-07-27 22:03:53.000000 minecraft_script-0.1.409/minecraft_script/interpreter.py
--rw-rw-rw-   0        0        0     4883 2023-07-27 22:36:13.000000 minecraft_script-0.1.409/minecraft_script/lexer.py
--rw-rw-rw-   0        0        0     4370 2023-07-27 22:03:28.000000 minecraft_script-0.1.409/minecraft_script/nodes.py
--rw-rw-rw-   0        0        0     9662 2023-07-27 23:02:16.000000 minecraft_script-0.1.409/minecraft_script/parser.py
--rw-rw-rw-   0        0        0     2084 2023-07-25 21:27:11.000000 minecraft_script-0.1.409/minecraft_script/shell_commands.py
--rw-rw-rw-   0        0        0     1143 2023-07-25 21:27:11.000000 minecraft_script-0.1.409/minecraft_script/text_additions.py
--rw-rw-rw-   0        0        0      211 2023-07-25 21:27:11.000000 minecraft_script-0.1.409/minecraft_script/tokens.py
--rw-rw-rw-   0        0        0     5612 2023-07-27 22:30:35.000000 minecraft_script-0.1.409/minecraft_script/types.py
-drwxrwxrwx   0        0        0        0 2023-07-27 23:05:45.079446 minecraft_script-0.1.409/minecraft_script.egg-info/
--rw-rw-rw-   0        0        0     1684 2023-07-27 23:05:45.000000 minecraft_script-0.1.409/minecraft_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2023-07-27 23:05:45.000000 minecraft_script-0.1.409/minecraft_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 23:05:45.000000 minecraft_script-0.1.409/minecraft_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-27 23:05:45.000000 minecraft_script-0.1.409/minecraft_script.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 23:05:45.085451 minecraft_script-0.1.409/setup.cfg
--rw-rw-rw-   0        0        0     1107 2023-07-27 14:00:51.000000 minecraft_script-0.1.409/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 00:58:18.582955 minecraft_script-0.1.410/
+-rw-rw-rw-   0        0        0     1684 2023-07-28 00:58:18.582955 minecraft_script-0.1.410/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 00:58:18.566472 minecraft_script-0.1.410/minecraft_script/
+-rw-rw-rw-   0        0        0     1433 2023-07-28 00:03:26.000000 minecraft_script-0.1.410/minecraft_script/__init__.py
+-rw-rw-rw-   0        0        0      378 2023-07-26 22:23:11.000000 minecraft_script-0.1.410/minecraft_script/__main__.py
+-rw-rw-rw-   0        0        0     1168 2023-07-26 12:31:03.000000 minecraft_script-0.1.410/minecraft_script/build_interpreter.py
+drwxrwxrwx   0        0        0        0 2023-07-28 00:58:18.572982 minecraft_script-0.1.410/minecraft_script/build_templates/
+-rw-rw-rw-   0        0        0       41 2023-07-25 21:27:11.000000 minecraft_script-0.1.410/minecraft_script/build_templates/function_tags.json
+-rw-rw-rw-   0        0        0      131 2023-07-25 21:27:11.000000 minecraft_script-0.1.410/minecraft_script/build_templates/pack.mcmeta
+-rw-rw-rw-   0        0        0     2276 2023-07-26 12:32:37.000000 minecraft_script-0.1.410/minecraft_script/builder.py
+-rw-rw-rw-   0        0        0       72 2023-07-28 00:58:04.000000 minecraft_script-0.1.410/minecraft_script/common.py
+-rw-rw-rw-   0        0        0     2070 2023-07-26 21:29:02.000000 minecraft_script-0.1.410/minecraft_script/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-28 00:58:18.582955 minecraft_script-0.1.410/minecraft_script/grammar/
+-rw-rw-rw-   0        0        0      189 2023-07-27 23:32:34.000000 minecraft_script-0.1.410/minecraft_script/grammar/LANG_KEYWORDS.json
+-rw-rw-rw-   0        0        0      579 2023-07-27 17:14:29.000000 minecraft_script-0.1.410/minecraft_script/grammar/LANG_TOKENS.json
+-rw-rw-rw-   0        0        0     5982 2023-07-28 00:24:54.000000 minecraft_script-0.1.410/minecraft_script/interpreter.py
+-rw-rw-rw-   0        0        0     4883 2023-07-27 22:36:13.000000 minecraft_script-0.1.410/minecraft_script/lexer.py
+-rw-rw-rw-   0        0        0     4768 2023-07-27 23:58:49.000000 minecraft_script-0.1.410/minecraft_script/nodes.py
+-rw-rw-rw-   0        0        0     9950 2023-07-28 00:02:02.000000 minecraft_script-0.1.410/minecraft_script/parser.py
+-rw-rw-rw-   0        0        0     2084 2023-07-25 21:27:11.000000 minecraft_script-0.1.410/minecraft_script/shell_commands.py
+-rw-rw-rw-   0        0        0     1143 2023-07-25 21:27:11.000000 minecraft_script-0.1.410/minecraft_script/text_additions.py
+-rw-rw-rw-   0        0        0      211 2023-07-25 21:27:11.000000 minecraft_script-0.1.410/minecraft_script/tokens.py
+-rw-rw-rw-   0        0        0     6067 2023-07-28 00:34:07.000000 minecraft_script-0.1.410/minecraft_script/types.py
+drwxrwxrwx   0        0        0        0 2023-07-28 00:58:18.572982 minecraft_script-0.1.410/minecraft_script.egg-info/
+-rw-rw-rw-   0        0        0     1684 2023-07-28 00:58:18.000000 minecraft_script-0.1.410/minecraft_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-07-28 00:58:18.000000 minecraft_script-0.1.410/minecraft_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 00:58:18.000000 minecraft_script-0.1.410/minecraft_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 00:58:18.000000 minecraft_script-0.1.410/minecraft_script.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 00:58:18.582955 minecraft_script-0.1.410/setup.cfg
+-rw-rw-rw-   0        0        0     1107 2023-07-27 14:00:51.000000 minecraft_script-0.1.410/setup.py
```

### Comparing `minecraft_script-0.1.409/PKG-INFO` & `minecraft_script-0.1.410/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft_script
-Version: 0.1.409
+Version: 0.1.410
 Summary: Minecraft Script Programming language
 Author: Joyful-Bard
 Author-email: <thisis@notarealemail.com>
 Keywords: minecraft,mc,script,language
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `minecraft_script-0.1.409/minecraft_script/__init__.py` & `minecraft_script-0.1.410/minecraft_script/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 def run_file(filepath: str):  # currently line-by-line
     with open(filepath, 'rt') as file:
         file_content = file.read()
 
     global_symbol_table = SymbolTable()
 
-    run_lexer = Lexer(file_content)
+    run_lexer = Lexer(file_content + "\n")
     tokens = run_lexer.tokenize()
 
     run_parser = Parser(tokens)
     ast = run_parser.parse()
 
     run_interpreter = Interpreter()
     context = Context('main', global_symbol_table)
```

### Comparing `minecraft_script-0.1.409/minecraft_script/build_interpreter.py` & `minecraft_script-0.1.410/minecraft_script/build_interpreter.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.409/minecraft_script/builder.py` & `minecraft_script-0.1.410/minecraft_script/builder.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.409/minecraft_script/errors.py` & `minecraft_script-0.1.410/minecraft_script/errors.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.409/minecraft_script/grammar/LANG_TOKENS.json` & `minecraft_script-0.1.410/minecraft_script/grammar/LANG_TOKENS.json`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.409/minecraft_script/interpreter.py` & `minecraft_script-0.1.410/minecraft_script/interpreter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .text_additions import text_error, text_underline
-from .types import Number, List, Boolean, Function, BuiltinFunction
+from .types import Number, List, Boolean, Function, BuiltinFunction, Return
 from .errors import MCSNameError, MCSTypeError, MCSIndexError
 
 
 class Context:
     def __init__(self, display_name: str, symbol_table, parent=None):
         self.display_name = display_name
         self.parent: None | Context = parent
@@ -152,15 +152,26 @@
     def visit_MultipleStatementsNode(self, node, context):
         return [self.visit(statement, context) for statement in node.statements]
 
     def visit_CodeBlockNode(self, node, context):
         local_symbol_table = SymbolTable(context.symbol_table, load_builtins=False)
         local_context = Context(f'code_block at {id(node)}', local_symbol_table)
 
-        return [self.visit(statement, local_context) for statement in node.statements]
+        visit_list = []
+        for statement in node.statements:
+            if type(statement).__name__ == 'ReturnNode':
+                visit_list.append(self.visit(statement, local_context))
+                break
+            visit_list.append(self.visit(statement, local_context))
+
+        return visit_list
+
+    def visit_ReturnNode(self, node, context):
+        if node.value:
+            return Return(self.visit(node.value, context))
 
     def no_visit_node(self, node, context):
         print(text_error(f'No visit method defined for {text_underline(type(node).__name__)}'))
 
 
 if __name__ == '__main__':
     Interpreter()
```

### Comparing `minecraft_script-0.1.409/minecraft_script/lexer.py` & `minecraft_script-0.1.410/minecraft_script/lexer.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.409/minecraft_script/nodes.py` & `minecraft_script-0.1.410/minecraft_script/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .tokens import Token
-from .errors import MCSValueError
+from .errors import MCSValueError, MCSSyntaxError
 
 
 class NumberNode:
     def __init__(self, number_token: Token):
         self.token = number_token
 
     def get_value(self):
@@ -131,14 +131,17 @@
     def __repr__(self):
         return f'UnaryOperationNode({self.operator !r}, {self.right_node !r})'
 
 
 class MultipleStatementsNode:
     def __init__(self, statements: list):
         self.statements = statements
+        if any(isinstance(element, ReturnNode) for element in self.statements):
+            MCSSyntaxError('Illegal return statement')
+            exit()
 
     def __str__(self):
         return f'statements: {self.statements}'
 
     def __repr__(self):
         return f'MultipleStatementsNode({self.statements})'
 
@@ -148,7 +151,18 @@
         self.statements = statements
 
     def __str__(self):
         return f'Code Block: {self.statements}'
 
     def __repr__(self):
         return f'CodeBlockNode({self.statements})'
+
+
+class ReturnNode:
+    def __init__(self, value=None):
+        self.value = value
+
+    def __str__(self):
+        return f'return: {self.value}'
+
+    def __repr__(self):
+        return f'ReturnNode({self.value})'
```

### Comparing `minecraft_script-0.1.409/minecraft_script/parser.py` & `minecraft_script-0.1.410/minecraft_script/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .tokens import Token
 from .errors import MCSSyntaxError
 from .text_additions import text_underline
 from .nodes import NumberNode, BinaryOperationNode, UnaryOperationNode, VariableAssignNode, VariableAccessNode, \
-    FunctionAssignNode, FunctionCallNode, MultipleStatementsNode, ListNode, ListGetNode, CodeBlockNode, BooleanNode
+    FunctionAssignNode, FunctionCallNode, MultipleStatementsNode, ListNode, ListGetNode, CodeBlockNode, BooleanNode, \
+    ReturnNode
 
 
 class Parser:
     def __init__(self, token_list: list[Token]):
         self.token_list = token_list
         self.current_index = -1
         self.current_token = None
@@ -58,15 +59,15 @@
         elif token.tt_type == 'TT_NUMBER':
             self.advance()
             return NumberNode(token)
 
     def term(self) -> BinaryOperationNode:
         return self.binary_operation(self.factor, ['*', '/', '%'])
 
-    def expression(self) -> BinaryOperationNode | VariableAssignNode | FunctionAssignNode | CodeBlockNode:
+    def expression(self) -> BinaryOperationNode | VariableAssignNode | FunctionAssignNode | CodeBlockNode | ReturnNode:
         if self.current_token.tt_type == 'VAR_DEFINE':
             self.advance()
             if self.current_token.tt_type != 'TT_NAME':
                 MCSSyntaxError(f'Expected name. Got {text_underline(f"{self.current_token.value !r}")} instead.')
                 exit()
 
             var_name_token = self.current_token
@@ -81,14 +82,21 @@
 
         elif self.current_token.tt_type == 'FUNC_DEFINE':
             return self.function_define()
 
         elif self.current_token.tt_type == 'TT_LEFT_BRACE':
             return self.code_block()
 
+        elif self.current_token.tt_type == 'TT_RETURN':
+            self.advance()
+            if self.current_token.tt_type in ['TT_NEWLINE', 'TT_RIGHT_BRACE']:
+                return ReturnNode()
+
+            return ReturnNode(self.expression())
+
         return self.binary_operation(self.term, ['+', '-'])
 
     def binary_operation(self, function, operators) -> BinaryOperationNode:
         left_node = function()
         # self.current_token is now the operator
 
         while self.current_token.value in operators:
```

### Comparing `minecraft_script-0.1.409/minecraft_script/shell_commands.py` & `minecraft_script-0.1.410/minecraft_script/shell_commands.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.409/minecraft_script/text_additions.py` & `minecraft_script-0.1.410/minecraft_script/text_additions.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.409/minecraft_script/types.py` & `minecraft_script-0.1.410/minecraft_script/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,17 +115,23 @@
         local_context = Context(self.name, local_symbol_table)
 
         for i in range(len(arguments)):
             arg_name = self.parameter_names[i]
             arg_value = arguments[i]
             local_context.symbol_table.set(arg_name, arg_value)
 
-        local_interpreter.visit(self.body_node, local_context)
+        output = local_interpreter.visit(self.body_node, local_context)
+        if isinstance(output, list):
+            try:
+                return next(element for element in output if isinstance(element, Return)).value
+            except StopIteration:
+                return Boolean(False)
 
-        return Boolean(False)
+        else:
+            return output
 
     def __str__(self):
         return f'{self.name}'
 
     def __repr__(self):
         return f'Function({self.name !r}, {self.parameter_names !r}, {self.body_node !r}, {self.context !r})'
 
@@ -185,8 +191,18 @@
         print(f'Interpreter built-in error ({self.name !r})')
         exit()
 
     def __str__(self):
         return f'<builtin function {self.name}>'
 
     def __repr__(self):
-        return f'BuiltinFunction({self.name})'
+        return f'BuiltinFunction({self.name !r})'
+
+class Return:
+    def __init__(self, value):
+        self.value = value
+
+    def __str__(self):
+        return f'{self.value}'
+
+    def __repr__(self):
+        return f'Return({self.value !r})'
```

### Comparing `minecraft_script-0.1.409/minecraft_script.egg-info/PKG-INFO` & `minecraft_script-0.1.410/minecraft_script.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft-script
-Version: 0.1.409
+Version: 0.1.410
 Summary: Minecraft Script Programming language
 Author: Joyful-Bard
 Author-email: <thisis@notarealemail.com>
 Keywords: minecraft,mc,script,language
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `minecraft_script-0.1.409/minecraft_script.egg-info/SOURCES.txt` & `minecraft_script-0.1.410/minecraft_script.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.409/setup.py` & `minecraft_script-0.1.410/setup.py`

 * *Files identical despite different names*


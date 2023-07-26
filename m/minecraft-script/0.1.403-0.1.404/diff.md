# Comparing `tmp/minecraft_script-0.1.403.tar.gz` & `tmp/minecraft_script-0.1.404.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft_script-0.1.403.tar", last modified: Tue Jul 25 19:11:35 2023, max compression
+gzip compressed data, was "minecraft_script-0.1.404.tar", last modified: Wed Jul 26 17:21:34 2023, max compression
```

## Comparing `minecraft_script-0.1.403.tar` & `minecraft_script-0.1.404.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 19:11:35.529521 minecraft_script-0.1.403/
--rw-rw-rw-   0        0        0     3188 2023-07-25 19:11:35.529521 minecraft_script-0.1.403/PKG-INFO
--rw-rw-rw-   0        0        0     2697 2023-07-25 18:41:58.000000 minecraft_script-0.1.403/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 19:11:35.504095 minecraft_script-0.1.403/minecraft_script/
--rw-rw-rw-   0        0        0     1445 2023-07-25 19:09:57.000000 minecraft_script-0.1.403/minecraft_script/__init__.py
--rw-rw-rw-   0        0        0      372 2023-07-19 19:22:33.000000 minecraft_script-0.1.403/minecraft_script/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:11:35.524080 minecraft_script-0.1.403/minecraft_script/build_templates/
--rw-rw-rw-   0        0        0       41 2023-07-25 18:52:26.000000 minecraft_script-0.1.403/minecraft_script/build_templates/function_tags.json
--rw-rw-rw-   0        0        0      131 2023-07-20 19:42:42.000000 minecraft_script-0.1.403/minecraft_script/build_templates/pack.mcmeta
--rw-rw-rw-   0        0        0     2276 2023-07-25 18:56:13.000000 minecraft_script-0.1.403/minecraft_script/builder.py
--rw-rw-rw-   0        0        0       51 2023-07-20 19:42:42.000000 minecraft_script-0.1.403/minecraft_script/common.py
--rw-rw-rw-   0        0        0     1809 2023-07-25 15:57:38.000000 minecraft_script-0.1.403/minecraft_script/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:11:35.528084 minecraft_script-0.1.403/minecraft_script/grammar/
--rw-rw-rw-   0        0        0       88 2023-07-25 16:40:21.000000 minecraft_script-0.1.403/minecraft_script/grammar/LANG_KEYWORDS.json
--rw-rw-rw-   0        0        0      382 2023-07-25 17:17:44.000000 minecraft_script-0.1.403/minecraft_script/grammar/LANG_TOKENS.json
--rw-rw-rw-   0        0        0     4311 2023-07-25 18:26:05.000000 minecraft_script-0.1.403/minecraft_script/interpreter.py
--rw-rw-rw-   0        0        0     3763 2023-07-25 18:29:48.000000 minecraft_script-0.1.403/minecraft_script/lexer.py
--rw-rw-rw-   0        0        0     2922 2023-07-25 18:24:44.000000 minecraft_script-0.1.403/minecraft_script/nodes.py
--rw-rw-rw-   0        0        0     5700 2023-07-25 18:29:48.000000 minecraft_script-0.1.403/minecraft_script/parser.py
--rw-rw-rw-   0        0        0     2084 2023-07-25 18:37:26.000000 minecraft_script-0.1.403/minecraft_script/shell_commands.py
--rw-rw-rw-   0        0        0     1143 2023-07-20 14:14:30.000000 minecraft_script-0.1.403/minecraft_script/text_additions.py
--rw-rw-rw-   0        0        0      211 2023-07-20 15:18:51.000000 minecraft_script-0.1.403/minecraft_script/tokens.py
--rw-rw-rw-   0        0        0     2843 2023-07-25 18:21:13.000000 minecraft_script-0.1.403/minecraft_script/types.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:11:35.519081 minecraft_script-0.1.403/minecraft_script.egg-info/
--rw-rw-rw-   0        0        0     3188 2023-07-25 19:11:35.000000 minecraft_script-0.1.403/minecraft_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-07-25 19:11:35.000000 minecraft_script-0.1.403/minecraft_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 19:11:35.000000 minecraft_script-0.1.403/minecraft_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-25 19:11:35.000000 minecraft_script-0.1.403/minecraft_script.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 19:11:35.529521 minecraft_script-0.1.403/setup.cfg
--rw-rw-rw-   0        0        0     1083 2023-07-25 19:10:29.000000 minecraft_script-0.1.403/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:21:34.044550 minecraft_script-0.1.404/
+-rw-rw-rw-   0        0        0     2070 2023-07-26 17:21:34.044550 minecraft_script-0.1.404/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 17:21:34.021738 minecraft_script-0.1.404/minecraft_script/
+-rw-rw-rw-   0        0        0     1449 2023-07-26 17:21:15.000000 minecraft_script-0.1.404/minecraft_script/__init__.py
+-rw-rw-rw-   0        0        0      372 2023-07-19 19:22:33.000000 minecraft_script-0.1.404/minecraft_script/__main__.py
+-rw-rw-rw-   0        0        0     1168 2023-07-26 12:31:03.000000 minecraft_script-0.1.404/minecraft_script/build_interpreter.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:21:34.040547 minecraft_script-0.1.404/minecraft_script/build_templates/
+-rw-rw-rw-   0        0        0       41 2023-07-25 21:27:11.000000 minecraft_script-0.1.404/minecraft_script/build_templates/function_tags.json
+-rw-rw-rw-   0        0        0      131 2023-07-25 21:27:11.000000 minecraft_script-0.1.404/minecraft_script/build_templates/pack.mcmeta
+-rw-rw-rw-   0        0        0     2276 2023-07-26 12:32:37.000000 minecraft_script-0.1.404/minecraft_script/builder.py
+-rw-rw-rw-   0        0        0       51 2023-07-25 21:27:11.000000 minecraft_script-0.1.404/minecraft_script/common.py
+-rw-rw-rw-   0        0        0     1837 2023-07-26 12:37:44.000000 minecraft_script-0.1.404/minecraft_script/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:21:34.042548 minecraft_script-0.1.404/minecraft_script/grammar/
+-rw-rw-rw-   0        0        0       88 2023-07-25 21:27:11.000000 minecraft_script-0.1.404/minecraft_script/grammar/LANG_KEYWORDS.json
+-rw-rw-rw-   0        0        0      483 2023-07-26 12:47:05.000000 minecraft_script-0.1.404/minecraft_script/grammar/LANG_TOKENS.json
+-rw-rw-rw-   0        0        0     4526 2023-07-26 17:12:09.000000 minecraft_script-0.1.404/minecraft_script/interpreter.py
+-rw-rw-rw-   0        0        0     4435 2023-07-26 16:04:57.000000 minecraft_script-0.1.404/minecraft_script/lexer.py
+-rw-rw-rw-   0        0        0     3197 2023-07-26 17:12:09.000000 minecraft_script-0.1.404/minecraft_script/nodes.py
+-rw-rw-rw-   0        0        0     6248 2023-07-26 16:30:16.000000 minecraft_script-0.1.404/minecraft_script/parser.py
+-rw-rw-rw-   0        0        0     2084 2023-07-25 21:27:11.000000 minecraft_script-0.1.404/minecraft_script/shell_commands.py
+-rw-rw-rw-   0        0        0     1143 2023-07-25 21:27:11.000000 minecraft_script-0.1.404/minecraft_script/text_additions.py
+-rw-rw-rw-   0        0        0      211 2023-07-25 21:27:11.000000 minecraft_script-0.1.404/minecraft_script/tokens.py
+-rw-rw-rw-   0        0        0     3515 2023-07-26 17:16:21.000000 minecraft_script-0.1.404/minecraft_script/types.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:21:34.039544 minecraft_script-0.1.404/minecraft_script.egg-info/
+-rw-rw-rw-   0        0        0     2070 2023-07-26 17:21:33.000000 minecraft_script-0.1.404/minecraft_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-07-26 17:21:33.000000 minecraft_script-0.1.404/minecraft_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 17:21:33.000000 minecraft_script-0.1.404/minecraft_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 17:21:33.000000 minecraft_script-0.1.404/minecraft_script.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 17:21:34.044550 minecraft_script-0.1.404/setup.cfg
+-rw-rw-rw-   0        0        0     1083 2023-07-26 17:21:18.000000 minecraft_script-0.1.404/setup.py
```

### Comparing `minecraft_script-0.1.403/PKG-INFO` & `minecraft_script-0.1.404/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft_script
-Version: 0.1.403
+Version: 0.1.404
 Summary: Minecraft Script Programming language
 Author: Joyful-Bard
 Author-email: <thisis@notarealemail.com>
 Keywords: minecraft,mc,script,language
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -24,71 +24,38 @@
 python -m minecraft_script run [files: optional, multiple allowed]
 python -m minecraft_script build [file]
 ```
 
 ## Objects
 ### Variables
 The var keyword can be used to initialize new variables.
-It can either be simply followed by a variable name, in which case it will default to 0,
-or you can directly assign a value to it.
+Use it by following it by the variable's name, then an equals sign and a value.
 
 ```js
-var hello1;  // initalized variable "hello1" with value 0 (default)
-var hello2 = 500;  // initialized variable "hello2" with value 500
+var hello2 = 500  // initialized variable "hello2" with value 500
 
-hello2 = 300;  // assigned new value 300 to variable hello2
-hello2 = hello2 + 500;  // adds 500 to hello2
-
-logtype hello2; // logs "var" in the console
-log hello2;  // logs "800" in the console
-```
-
-### Constants
-The const keyword can be used to initialize and define new constants.
-Unlike vars, these cannot be reassigned new values. Trying to initialize
-a new constant without a value brings raises a Syntax Error.
-
-```js
-const hello1;  // raises 'Syntax Error: Missing value in const declaration'
-const hello1 = 500;
-hello1 = 300;  // raises 'Type Error: Tried to assign new value to const "hello1"'
-
-logtype hello1;  // logs "const" in the console
-log hello1;  // logs "500" in the console
+var hello2 = 300  // assigned new value 300 to variable hello2
+var hello2 = hello2 + 500  // adds 500 to hello2
 ```
 
-## Functions
+### Functions
 Functions are defined with the "function" keyword. They can be anonymous,
 or be attributed a name. Parentheses around the arguments are required (currently, subject to change).
 
 ```js
 function = (a) => a * 3  // anonymous function
 
 function add = (a, b) => a + b  // define a simple add function
 add(2, 7)  // call the function; returns 9
-
 ```
 
-## Console logging
-### Console logging values with log
-Logging values in MCS is as simple as typing "log", followed by an expression.
-Example:
-```js
-var hello1 = 500;
-const hello2 = 600;
-
-log 200 + 200;  // logs 400 in console
-log hello1;  // logs 500 in console
-log hello2;  // logs 600 in console
-```
+## Builtin Functions
+### log
+The log functions allows you to keep track of values in the console.
+It is equivalent to JavaScript's console.log() or Python's print() function.
 
-### Console logging types with logtype
-Logging types in MCS is equally as simple. To log an object's type, simply type "logtype" followed by the object.
-Example:
 ```js
-var hello1 = 500;
-const hello2 = 600;
+var hello1 = 500
 
-logtype 400;  // logs "number" in console
-logtype hello1;  // logs "var" in console
-logtype hello2;  // logs "const" in console
+log(200 + 200)  // logs "400" in console
+log(hello1, 300)  // logs "500, 300" in console
 ```
```

### Comparing `minecraft_script-0.1.403/README.md` & `minecraft_script-0.1.404/minecraft_script.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,81 +1,61 @@
-# Minecraft Script
-
-Minecraft script is primarily a tool to make Minecraft Datapack creation easier.
-Minecraft Script is an interpreted programming language which goes through the Python interpreter for output.
-However, interpretation is not its main feature, and is rather more of a debugging tool, as its sole
-purpose is to allow you to validate your code before building it into a full datapack.
-
-# Commands
-```cmd
-python -m minecraft_script help
-python -m minecraft_script run [files: optional, multiple allowed]
-python -m minecraft_script build [file]
-```
-
-## Objects
-### Variables
-The var keyword can be used to initialize new variables.
-It can either be simply followed by a variable name, in which case it will default to 0,
-or you can directly assign a value to it.
-
-```js
-var hello1;  // initalized variable "hello1" with value 0 (default)
-var hello2 = 500;  // initialized variable "hello2" with value 500
-
-hello2 = 300;  // assigned new value 300 to variable hello2
-hello2 = hello2 + 500;  // adds 500 to hello2
-
-logtype hello2; // logs "var" in the console
-log hello2;  // logs "800" in the console
-```
-
-### Constants
-The const keyword can be used to initialize and define new constants.
-Unlike vars, these cannot be reassigned new values. Trying to initialize
-a new constant without a value brings raises a Syntax Error.
-
-```js
-const hello1;  // raises 'Syntax Error: Missing value in const declaration'
-const hello1 = 500;
-hello1 = 300;  // raises 'Type Error: Tried to assign new value to const "hello1"'
-
-logtype hello1;  // logs "const" in the console
-log hello1;  // logs "500" in the console
+Metadata-Version: 2.1
+Name: minecraft-script
+Version: 0.1.404
+Summary: Minecraft Script Programming language
+Author: Joyful-Bard
+Author-email: <thisis@notarealemail.com>
+Keywords: minecraft,mc,script,language
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+
+
+# Minecraft Script
+
+Minecraft script is primarily a tool to make Minecraft Datapack creation easier.
+Minecraft Script is an interpreted programming language which goes through the Python interpreter for output.
+However, interpretation is not its main feature, and is rather more of a debugging tool, as its sole
+purpose is to allow you to validate your code before building it into a full datapack.
+
+# Commands
+```cmd
+python -m minecraft_script help
+python -m minecraft_script run [files: optional, multiple allowed]
+python -m minecraft_script build [file]
+```
+
+## Objects
+### Variables
+The var keyword can be used to initialize new variables.
+Use it by following it by the variable's name, then an equals sign and a value.
+
+```js
+var hello2 = 500  // initialized variable "hello2" with value 500
+
+var hello2 = 300  // assigned new value 300 to variable hello2
+var hello2 = hello2 + 500  // adds 500 to hello2
+```
+
+### Functions
+Functions are defined with the "function" keyword. They can be anonymous,
+or be attributed a name. Parentheses around the arguments are required (currently, subject to change).
+
+```js
+function = (a) => a * 3  // anonymous function
+
+function add = (a, b) => a + b  // define a simple add function
+add(2, 7)  // call the function; returns 9
+```
+
+## Builtin Functions
+### log
+The log functions allows you to keep track of values in the console.
+It is equivalent to JavaScript's console.log() or Python's print() function.
+
+```js
+var hello1 = 500
+
+log(200 + 200)  // logs "400" in console
+log(hello1, 300)  // logs "500, 300" in console
 ```
-
-## Functions
-Functions are defined with the "function" keyword. They can be anonymous,
-or be attributed a name. Parentheses around the arguments are required (currently, subject to change).
-
-```js
-function = (a) => a * 3  // anonymous function
-
-function add = (a, b) => a + b  // define a simple add function
-add(2, 7)  // call the function; returns 9
-
-```
-
-## Console logging
-### Console logging values with log
-Logging values in MCS is as simple as typing "log", followed by an expression.
-Example:
-```js
-var hello1 = 500;
-const hello2 = 600;
-
-log 200 + 200;  // logs 400 in console
-log hello1;  // logs 500 in console
-log hello2;  // logs 600 in console
-```
-
-### Console logging types with logtype
-Logging types in MCS is equally as simple. To log an object's type, simply type "logtype" followed by the object.
-Example:
-```js
-var hello1 = 500;
-const hello2 = 600;
-
-logtype 400;  // logs "number" in console
-logtype hello1;  // logs "var" in console
-logtype hello2;  // logs "const" in console
-```
```

### Comparing `minecraft_script-0.1.403/minecraft_script/__init__.py` & `minecraft_script-0.1.404/minecraft_script/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 from .lexer import Lexer
 from .parser import Parser
 from .interpreter import Interpreter, Context, SymbolTable
 
-version = "0.1.403"
+version = "0.1.404"
 
 
 def run(text: str):
     global_symbol_table = SymbolTable()
 
     run_lexer = Lexer(text)
     tokens = run_lexer.tokenize()
+    print(repr(tokens))
 
     run_parser = Parser(tokens)
     ast = run_parser.parse()
+    print(repr(ast))
 
     run_interpreter = Interpreter()
     context = Context('main', global_symbol_table)
     print(run_interpreter.visit(ast, context))
 
 
 def run_file(filepath: str):  # currently line-by-line
     with open(filepath, 'rt') as file:
         file_content = file.read()
 
     global_symbol_table = SymbolTable()
 
-    for line in filter(lambda x: not (x.strip(' ') == ''), file_content.split('\n')):
-        run_lexer = Lexer(line)
-        tokens = run_lexer.tokenize()
+    run_lexer = Lexer(file_content)
+    tokens = run_lexer.tokenize()
 
-        run_parser = Parser(tokens)
-        ast = run_parser.parse()
+    run_parser = Parser(tokens)
+    ast = run_parser.parse()
 
-        run_interpreter = Interpreter()
-        context = Context('main', global_symbol_table)
-        print(run_interpreter.visit(ast, context))
+    run_interpreter = Interpreter()
+    context = Context('main', global_symbol_table)
+    run_interpreter.visit(ast, context)
 
 
 def run_shell():
     global_symbol_table = SymbolTable()
 
     while True:
-        text = input("> ")
+        text = input('> ')
+        while text.strip(' ') == '':
+            text = input('> ')
 
         run_lexer = Lexer(text)
         tokens = run_lexer.tokenize()
 
         run_parser = Parser(tokens)
         ast = run_parser.parse()
 
         run_interpreter = Interpreter()
         context = Context('main', global_symbol_table)
-        print(run_interpreter.visit(ast, context))
+        print(run_interpreter.visit(ast, context)[0])
```

### Comparing `minecraft_script-0.1.403/minecraft_script/builder.py` & `minecraft_script-0.1.404/minecraft_script/builder.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.403/minecraft_script/errors.py` & `minecraft_script-0.1.404/minecraft_script/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,17 @@
         self.error_type = error_type
         self.line_number = line_number
 
         print(self)
 
     def __str__(self):
         if self.line_number:
-            return text_error(f'{self.error_type}: {text_underline(f"{self.details !r}")} at line {self.line_number}')
+            return text_error(f'{self.error_type}: {self.details} at line {self.line_number}')
         else:
-            return text_error(f'{self.error_type}: {text_underline(f"{self.details !r}")}')
+            return text_error(f'{self.error_type}: {self.details}')
 
     def __repr__(self):
         return f'{self.__class__.__name__}({self.error_type !r}, {self.details !r}, {self.line_number !r})'
 
 
 class MCSSyntaxError(MCSError):
     def __init__(self, details: str, line_number: int = None):
@@ -42,13 +42,14 @@
 class MCSZeroDivisionError(MCSError):
     def __init__(self, details: str, line_number: int = None):
         super().__init__(details, "Zero Division Error", line_number)
 
 
 class MCSNameError(MCSError):
     def __init__(self, details: str, line_number: int = None):
+        details = f'Name {text_underline(f"{details !r}")} is not defined'
         super().__init__(details, "Name Error", line_number)
 
 
 if __name__ == '__main__':
     a = MCSTypeError('const')
     print(a)
```

### Comparing `minecraft_script-0.1.403/minecraft_script/interpreter.py` & `minecraft_script-0.1.404/minecraft_script/interpreter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from .text_additions import text_error, text_underline
-from .types import Number, Function
+from .types import Number, Function, BuiltinFunction
 from .errors import MCSNameError
 
 
 class Context:
-    def __init__(self, display_name: str, symbol_table, parent = None):
+    def __init__(self, display_name: str, symbol_table, parent=None):
         self.display_name = display_name
         self.parent: None | Context = parent
         self.symbol_table: SymbolTable = symbol_table
 
     def display(self):
         return f'<{self.display_name}>'
 
     def __repr__(self):
         return f'Context({self.display_name}, {self.symbol_table}, {self.parent})'
 
 
 class SymbolTable:
-    def __init__(self, parent = None):
+    def __init__(self, parent=None, *, load_builtins=True):
         self.symbols: dict = {}
         self.parent = parent
 
+        if load_builtins:
+            self.set('log', BuiltinFunction('log'))
+
     def get(self, variable_name):
         value = self.symbols.get(variable_name, None)
 
         if value is None and self.parent:
             return self.parent.get(variable_name)
 
         return value
@@ -37,29 +40,30 @@
 
     def __repr__(self):
         return f'SymbolTable({self.parent})'
 
     def __str__(self):
         return f'{self.symbols}'
 
+
 class Interpreter:
     def visit(self, node, context: Context):
         method_name = f'visit_{type(node).__name__}'
         method = getattr(self, method_name, self.no_visit_node)
         return method(node, context)
 
     def visit_NumberNode(self, node, context: Context) -> int:
         return node.get_value()
 
     def visit_VariableAccessNode(self, node, context: Context) -> any:
         var_name: str = node.get_name()
         var_value = context.symbol_table.get(var_name)
 
         if var_value is None:
-            MCSNameError(f'Name {text_underline(f"{var_name !r}")} is not defined')
+            MCSNameError(var_name)
             exit()
 
         return var_value
 
     def visit_VariableAssignNode(self, node, context: Context) -> any:
         var_name: str = node.get_name()
         var_new_value = self.visit(node.value_node, context)
@@ -115,13 +119,16 @@
         if operator == '+':
             result = Number(0).add(right_node)
         elif operator == '-':
             result = Number(0).subtract(right_node)
 
         return result
 
+    def visit_MultipleStatementsNode(self, node, context):
+        return [self.visit(statement, context) for statement in node.statements]
+
     def no_visit_node(self, node, context: Context):
         print(text_error(f'No visit method defined for {text_underline(type(node).__name__)}'))
 
 
 if __name__ == '__main__':
     Interpreter()
```

### Comparing `minecraft_script-0.1.403/minecraft_script/lexer.py` & `minecraft_script-0.1.404/minecraft_script/lexer.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 class Lexer:
     def __init__(self, text: str):
         self.text = text
         self.current_index = -1
         self.current_char = None
         self.current_line = 0
 
+        self.bracket_depth = 0
+
         self.advance()
 
     def advance(self) -> None:
         self.current_index += 1
         self.current_char = self.text[self.current_index] if self.current_index < len(self.text) else None
 
         if self.current_char == '\n':
             self.current_line += 1
-            self.advance()
 
     def make_name(self):
         name_str = ''
         # allow numbers after first character
         while self.current_char and (self.current_char in LANG_TOKENS['TT_NAME'] or self.current_char in LANG_TOKENS['TT_NUMBER']):
             name_str += self.current_char
             self.advance()
@@ -70,14 +71,29 @@
                 tokens.append(Token(self.current_char, 'TT_RIGHT_PARENTHESIS'))
                 self.advance()
 
             elif self.current_char == LANG_TOKENS['TT_COMMA']:
                 tokens.append(Token(self.current_char, 'TT_COMMA'))
                 self.advance()
 
+            elif self.current_char in LANG_TOKENS['TT_NEWLINE']:
+                if self.bracket_depth == 0:
+                    tokens.append(Token(self.current_char, 'TT_NEWLINE'))
+                self.advance()
+
+            elif self.current_char == LANG_TOKENS['TT_LEFT_BRACKET']:
+                tokens.append(Token(self.current_char, 'TT_LEFT_BRACKET'))
+                self.bracket_depth += 1
+                self.advance()
+
+            elif self.current_char == LANG_TOKENS['TT_RIGHT_BRACKET']:
+                tokens.append(Token(self.current_char, 'TT_RIGHT_BRACKET'))
+                self.bracket_depth -= 1
+                self.advance()
+
             elif self.current_char == LANG_TOKENS['TT_EQUALS']:
                 token_value = self.make_equals()
 
                 if token_value == LANG_TOKENS['TT_FUNCTION_ARROW']:
                     tokens.append(Token(token_value, 'TT_FUNCTION_ARROW'))
                 else:
                     tokens.append(Token(token_value, 'TT_EQUALS'))
```

### Comparing `minecraft_script-0.1.403/minecraft_script/nodes.py` & `minecraft_script-0.1.404/minecraft_script/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         self.name_token = name_token
         self.argument_nodes = argument_nodes
 
     def __str__(self):
         return f'Func call:{self.name_token.value !r}'
 
     def __repr__(self):
-        return f'FunctionAssignNode({self.name_token !r}, {self.argument_nodes !r})'
+        return f'FunctionCallNode({self.name_token !r}, {self.argument_nodes !r})'
 
 
 class BinaryOperationNode:
     def __init__(self, left_node: NumberNode, operator: Token, right_node: NumberNode):
         self.left_node = left_node
         self.operator = operator
         self.right_node = right_node
@@ -89,7 +89,18 @@
         self.right_node = right_node
 
     def __str__(self):
         return f'{str(self.right_node)[:-1]}{self.operator.value !s}{self.right_node.token.value !s}'
 
     def __repr__(self):
         return f'UnaryOperationNode({self.operator !r}, {self.right_node !r})'
+
+
+class MultipleStatementsNode:
+    def __init__(self, statements: list):
+        self.statements = statements
+
+    def __str__(self):
+        return f'statements: {self.statements}'
+
+    def __repr__(self):
+        return f'MultipleStatementsNode({self.statements})'
```

### Comparing `minecraft_script-0.1.403/minecraft_script/parser.py` & `minecraft_script-0.1.404/minecraft_script/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .tokens import Token
 from .errors import MCSSyntaxError
 from .text_additions import text_underline
-from .nodes import NumberNode, BinaryOperationNode, UnaryOperationNode, VariableAssignNode, VariableAccessNode, FunctionAssignNode, FunctionCallNode
+from .nodes import NumberNode, BinaryOperationNode, UnaryOperationNode, VariableAssignNode, VariableAccessNode, \
+    FunctionAssignNode, FunctionCallNode, MultipleStatementsNode
 
 
 class Parser:
     def __init__(self, token_list: list[Token]):
         self.token_list = token_list
         self.current_index = -1
         self.current_token = None
@@ -14,15 +15,15 @@
 
     def advance(self):
         self.current_index += 1
         if self.current_index < len(self.token_list):
             self.current_token = self.token_list[self.current_index]
 
     def parse(self):
-        result = self.expression()
+        result = self.statement()
         return result
 
     def factor(self) -> NumberNode | UnaryOperationNode | BinaryOperationNode | VariableAccessNode | FunctionCallNode:
         token = self.current_token
 
         if token.value in ['+', '-']:
             self.advance()
@@ -80,14 +81,27 @@
         while self.current_token.value in operators:
             operator = self.current_token
             self.advance()
             right_node = function()
             left_node = BinaryOperationNode(left_node, operator, right_node)
         return left_node
 
+    def statement(self) -> MultipleStatementsNode:
+        statements = []
+        while self.current_token.tt_type == 'TT_NEWLINE':
+            self.advance()
+        statements.append(self.expression())
+
+        while self.current_token.tt_type == 'TT_NEWLINE':
+            while self.current_token.tt_type == 'TT_NEWLINE':
+                self.advance()
+            statements.append(self.expression())
+
+        return MultipleStatementsNode(statements)
+
     def function_define(self) -> FunctionAssignNode:
         self.advance()
 
         function_name_token = None
         if self.current_token.tt_type == 'TT_NAME':
             function_name_token = self.current_token
             self.advance()
@@ -139,10 +153,14 @@
         while self.current_token.tt_type == 'TT_COMMA':
             self.advance()
             argument_tokens.append(self.factor())
 
         if self.current_token.tt_type == 'TT_RIGHT_PARENTHESIS':
             return FunctionCallNode(name_token, argument_tokens)
 
+
 if __name__ == '__main__':
-    tokens = [Token(5, 'TT_NUMBER'), Token('+', 'TT_BINARY_OPERATOR'), Token(5, 'TT_NUMBER'), Token('*', 'TT_BINARY_OPERATOR'), Token('(', 'TT_LEFT_PARENTHESIS'), Token(3, 'TT_NUMBER'), Token('+', 'TT_BINARY_OPERATOR'), Token('-', 'TT_BINARY_OPERATOR'), Token(5, 'TT_NUMBER'), Token(')', 'TT_RIGHT_PARENTHESIS')]
+    tokens = [Token(5, 'TT_NUMBER'), Token('+', 'TT_BINARY_OPERATOR'), Token(5, 'TT_NUMBER'),
+              Token('*', 'TT_BINARY_OPERATOR'), Token('(', 'TT_LEFT_PARENTHESIS'), Token(3, 'TT_NUMBER'),
+              Token('+', 'TT_BINARY_OPERATOR'), Token('-', 'TT_BINARY_OPERATOR'), Token(5, 'TT_NUMBER'),
+              Token(')', 'TT_RIGHT_PARENTHESIS')]
     print(Parser(tokens).parse())
```

### Comparing `minecraft_script-0.1.403/minecraft_script/shell_commands.py` & `minecraft_script-0.1.404/minecraft_script/shell_commands.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.403/minecraft_script/text_additions.py` & `minecraft_script-0.1.404/minecraft_script/text_additions.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.403/minecraft_script/types.py` & `minecraft_script-0.1.404/minecraft_script/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,22 +65,46 @@
         self.body_node = body_node
         self.context = context
 
     def call(self, arguments: list):
         from .interpreter import Interpreter, Context, SymbolTable
         local_interpreter = Interpreter()
 
-        local_symbol_table = SymbolTable(self.context.symbol_table)
+        local_symbol_table = SymbolTable(self.context.symbol_table, load_builtins=False)
         local_context = Context(self.name, local_symbol_table)
 
         for i in range(len(arguments)):
             arg_name = self.parameter_names[i]
             arg_value = arguments[i]
             local_context.symbol_table.set(arg_name, arg_value)
 
         return local_interpreter.visit(self.body_node, local_context)
 
+    def __str__(self):
+        return f'{self.name}'
+
     def __repr__(self):
         return f'Function({self.name !r}, {self.parameter_names !r}, {self.body_node !r}, {self.context !r})'
 
+
+class BuiltinFunction:
+    def __init__(self, name):
+        self.name = name
+
+    def call(self, arguments: list):
+        method = getattr(self, f'call_{self.name}', 'unknown_name')
+        method(arguments)
+
+    @staticmethod
+    def call_log(arguments: list):
+        print(', '.join([str(argument) for argument in arguments]))
+        return Number(0)
+
+    def unknown_name(self, arguments: list):
+        print(f'Interpreter built-in error ({self.name !r})')
+        exit()
+
     def __str__(self):
-        return f'{self.name}'
+        return f'<builtin function {self.name}>'
+
+    def __repr__(self):
+        return f'BuiltinFunction({self.name})'
```

### Comparing `minecraft_script-0.1.403/minecraft_script.egg-info/SOURCES.txt` & `minecraft_script-0.1.404/minecraft_script.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-README.md
 setup.py
 minecraft_script/__init__.py
 minecraft_script/__main__.py
+minecraft_script/build_interpreter.py
 minecraft_script/builder.py
 minecraft_script/common.py
 minecraft_script/errors.py
 minecraft_script/interpreter.py
 minecraft_script/lexer.py
 minecraft_script/nodes.py
 minecraft_script/parser.py
```

### Comparing `minecraft_script-0.1.403/setup.py` & `minecraft_script-0.1.404/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.403'
+VERSION = '0.1.404'
 DESCRIPTION = 'Minecraft Script Programming language'
 
 # Setting up
 setup(
     name="minecraft_script",
     version=VERSION,
     author="Joyful-Bard",
```


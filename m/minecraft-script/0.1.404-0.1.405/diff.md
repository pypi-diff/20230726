# Comparing `tmp/minecraft_script-0.1.404.tar.gz` & `tmp/minecraft_script-0.1.405.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft_script-0.1.404.tar", last modified: Wed Jul 26 17:21:34 2023, max compression
+gzip compressed data, was "minecraft_script-0.1.405.tar", last modified: Wed Jul 26 17:50:01 2023, max compression
```

## Comparing `minecraft_script-0.1.404.tar` & `minecraft_script-0.1.405.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 17:21:34.044550 minecraft_script-0.1.404/
--rw-rw-rw-   0        0        0     2070 2023-07-26 17:21:34.044550 minecraft_script-0.1.404/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 17:21:34.021738 minecraft_script-0.1.404/minecraft_script/
--rw-rw-rw-   0        0        0     1449 2023-07-26 17:21:15.000000 minecraft_script-0.1.404/minecraft_script/__init__.py
--rw-rw-rw-   0        0        0      372 2023-07-19 19:22:33.000000 minecraft_script-0.1.404/minecraft_script/__main__.py
--rw-rw-rw-   0        0        0     1168 2023-07-26 12:31:03.000000 minecraft_script-0.1.404/minecraft_script/build_interpreter.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:21:34.040547 minecraft_script-0.1.404/minecraft_script/build_templates/
--rw-rw-rw-   0        0        0       41 2023-07-25 21:27:11.000000 minecraft_script-0.1.404/minecraft_script/build_templates/function_tags.json
--rw-rw-rw-   0        0        0      131 2023-07-25 21:27:11.000000 minecraft_script-0.1.404/minecraft_script/build_templates/pack.mcmeta
--rw-rw-rw-   0        0        0     2276 2023-07-26 12:32:37.000000 minecraft_script-0.1.404/minecraft_script/builder.py
--rw-rw-rw-   0        0        0       51 2023-07-25 21:27:11.000000 minecraft_script-0.1.404/minecraft_script/common.py
--rw-rw-rw-   0        0        0     1837 2023-07-26 12:37:44.000000 minecraft_script-0.1.404/minecraft_script/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:21:34.042548 minecraft_script-0.1.404/minecraft_script/grammar/
--rw-rw-rw-   0        0        0       88 2023-07-25 21:27:11.000000 minecraft_script-0.1.404/minecraft_script/grammar/LANG_KEYWORDS.json
--rw-rw-rw-   0        0        0      483 2023-07-26 12:47:05.000000 minecraft_script-0.1.404/minecraft_script/grammar/LANG_TOKENS.json
--rw-rw-rw-   0        0        0     4526 2023-07-26 17:12:09.000000 minecraft_script-0.1.404/minecraft_script/interpreter.py
--rw-rw-rw-   0        0        0     4435 2023-07-26 16:04:57.000000 minecraft_script-0.1.404/minecraft_script/lexer.py
--rw-rw-rw-   0        0        0     3197 2023-07-26 17:12:09.000000 minecraft_script-0.1.404/minecraft_script/nodes.py
--rw-rw-rw-   0        0        0     6248 2023-07-26 16:30:16.000000 minecraft_script-0.1.404/minecraft_script/parser.py
--rw-rw-rw-   0        0        0     2084 2023-07-25 21:27:11.000000 minecraft_script-0.1.404/minecraft_script/shell_commands.py
--rw-rw-rw-   0        0        0     1143 2023-07-25 21:27:11.000000 minecraft_script-0.1.404/minecraft_script/text_additions.py
--rw-rw-rw-   0        0        0      211 2023-07-25 21:27:11.000000 minecraft_script-0.1.404/minecraft_script/tokens.py
--rw-rw-rw-   0        0        0     3515 2023-07-26 17:16:21.000000 minecraft_script-0.1.404/minecraft_script/types.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:21:34.039544 minecraft_script-0.1.404/minecraft_script.egg-info/
--rw-rw-rw-   0        0        0     2070 2023-07-26 17:21:33.000000 minecraft_script-0.1.404/minecraft_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2023-07-26 17:21:33.000000 minecraft_script-0.1.404/minecraft_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 17:21:33.000000 minecraft_script-0.1.404/minecraft_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 17:21:33.000000 minecraft_script-0.1.404/minecraft_script.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 17:21:34.044550 minecraft_script-0.1.404/setup.cfg
--rw-rw-rw-   0        0        0     1083 2023-07-26 17:21:18.000000 minecraft_script-0.1.404/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:50:01.465750 minecraft_script-0.1.405/
+-rw-rw-rw-   0        0        0     2070 2023-07-26 17:50:01.464748 minecraft_script-0.1.405/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 17:50:01.447593 minecraft_script-0.1.405/minecraft_script/
+-rw-rw-rw-   0        0        0     1449 2023-07-26 17:49:37.000000 minecraft_script-0.1.405/minecraft_script/__init__.py
+-rw-rw-rw-   0        0        0      372 2023-07-19 19:22:33.000000 minecraft_script-0.1.405/minecraft_script/__main__.py
+-rw-rw-rw-   0        0        0     1168 2023-07-26 12:31:03.000000 minecraft_script-0.1.405/minecraft_script/build_interpreter.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:50:01.461746 minecraft_script-0.1.405/minecraft_script/build_templates/
+-rw-rw-rw-   0        0        0       41 2023-07-25 21:27:11.000000 minecraft_script-0.1.405/minecraft_script/build_templates/function_tags.json
+-rw-rw-rw-   0        0        0      131 2023-07-25 21:27:11.000000 minecraft_script-0.1.405/minecraft_script/build_templates/pack.mcmeta
+-rw-rw-rw-   0        0        0     2276 2023-07-26 12:32:37.000000 minecraft_script-0.1.405/minecraft_script/builder.py
+-rw-rw-rw-   0        0        0       51 2023-07-25 21:27:11.000000 minecraft_script-0.1.405/minecraft_script/common.py
+-rw-rw-rw-   0        0        0     1837 2023-07-26 12:37:44.000000 minecraft_script-0.1.405/minecraft_script/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:50:01.463748 minecraft_script-0.1.405/minecraft_script/grammar/
+-rw-rw-rw-   0        0        0       88 2023-07-25 21:27:11.000000 minecraft_script-0.1.405/minecraft_script/grammar/LANG_KEYWORDS.json
+-rw-rw-rw-   0        0        0      483 2023-07-26 12:47:05.000000 minecraft_script-0.1.405/minecraft_script/grammar/LANG_TOKENS.json
+-rw-rw-rw-   0        0        0     4526 2023-07-26 17:42:04.000000 minecraft_script-0.1.405/minecraft_script/interpreter.py
+-rw-rw-rw-   0        0        0     4435 2023-07-26 16:04:57.000000 minecraft_script-0.1.405/minecraft_script/lexer.py
+-rw-rw-rw-   0        0        0     3197 2023-07-26 17:12:09.000000 minecraft_script-0.1.405/minecraft_script/nodes.py
+-rw-rw-rw-   0        0        0     6276 2023-07-26 17:44:50.000000 minecraft_script-0.1.405/minecraft_script/parser.py
+-rw-rw-rw-   0        0        0     2084 2023-07-25 21:27:11.000000 minecraft_script-0.1.405/minecraft_script/shell_commands.py
+-rw-rw-rw-   0        0        0     1143 2023-07-25 21:27:11.000000 minecraft_script-0.1.405/minecraft_script/text_additions.py
+-rw-rw-rw-   0        0        0      211 2023-07-25 21:27:11.000000 minecraft_script-0.1.405/minecraft_script/tokens.py
+-rw-rw-rw-   0        0        0     3515 2023-07-26 17:16:21.000000 minecraft_script-0.1.405/minecraft_script/types.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:50:01.460744 minecraft_script-0.1.405/minecraft_script.egg-info/
+-rw-rw-rw-   0        0        0     2070 2023-07-26 17:50:01.000000 minecraft_script-0.1.405/minecraft_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-07-26 17:50:01.000000 minecraft_script-0.1.405/minecraft_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 17:50:01.000000 minecraft_script-0.1.405/minecraft_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 17:50:01.000000 minecraft_script-0.1.405/minecraft_script.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 17:50:01.465750 minecraft_script-0.1.405/setup.cfg
+-rw-rw-rw-   0        0        0     1083 2023-07-26 17:49:34.000000 minecraft_script-0.1.405/setup.py
```

### Comparing `minecraft_script-0.1.404/PKG-INFO` & `minecraft_script-0.1.405/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft_script
-Version: 0.1.404
+Version: 0.1.405
 Summary: Minecraft Script Programming language
 Author: Joyful-Bard
 Author-email: <thisis@notarealemail.com>
 Keywords: minecraft,mc,script,language
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `minecraft_script-0.1.404/minecraft_script/__init__.py` & `minecraft_script-0.1.405/minecraft_script/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .lexer import Lexer
 from .parser import Parser
 from .interpreter import Interpreter, Context, SymbolTable
 
-version = "0.1.404"
+version = "0.1.405"
 
 
 def run(text: str):
     global_symbol_table = SymbolTable()
 
     run_lexer = Lexer(text)
     tokens = run_lexer.tokenize()
```

### Comparing `minecraft_script-0.1.404/minecraft_script/build_interpreter.py` & `minecraft_script-0.1.405/minecraft_script/build_interpreter.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.404/minecraft_script/builder.py` & `minecraft_script-0.1.405/minecraft_script/builder.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.404/minecraft_script/errors.py` & `minecraft_script-0.1.405/minecraft_script/errors.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.404/minecraft_script/interpreter.py` & `minecraft_script-0.1.405/minecraft_script/interpreter.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.404/minecraft_script/lexer.py` & `minecraft_script-0.1.405/minecraft_script/lexer.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.404/minecraft_script/nodes.py` & `minecraft_script-0.1.405/minecraft_script/nodes.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.404/minecraft_script/parser.py` & `minecraft_script-0.1.405/minecraft_script/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
         argument_tokens.append(self.factor())
 
         while self.current_token.tt_type == 'TT_COMMA':
             self.advance()
             argument_tokens.append(self.factor())
 
         if self.current_token.tt_type == 'TT_RIGHT_PARENTHESIS':
+            self.advance()
             return FunctionCallNode(name_token, argument_tokens)
 
 
 if __name__ == '__main__':
     tokens = [Token(5, 'TT_NUMBER'), Token('+', 'TT_BINARY_OPERATOR'), Token(5, 'TT_NUMBER'),
               Token('*', 'TT_BINARY_OPERATOR'), Token('(', 'TT_LEFT_PARENTHESIS'), Token(3, 'TT_NUMBER'),
               Token('+', 'TT_BINARY_OPERATOR'), Token('-', 'TT_BINARY_OPERATOR'), Token(5, 'TT_NUMBER'),
```

### Comparing `minecraft_script-0.1.404/minecraft_script/shell_commands.py` & `minecraft_script-0.1.405/minecraft_script/shell_commands.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.404/minecraft_script/text_additions.py` & `minecraft_script-0.1.405/minecraft_script/text_additions.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.404/minecraft_script/types.py` & `minecraft_script-0.1.405/minecraft_script/types.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.404/minecraft_script.egg-info/PKG-INFO` & `minecraft_script-0.1.405/minecraft_script.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft-script
-Version: 0.1.404
+Version: 0.1.405
 Summary: Minecraft Script Programming language
 Author: Joyful-Bard
 Author-email: <thisis@notarealemail.com>
 Keywords: minecraft,mc,script,language
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `minecraft_script-0.1.404/minecraft_script.egg-info/SOURCES.txt` & `minecraft_script-0.1.405/minecraft_script.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.404/setup.py` & `minecraft_script-0.1.405/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.404'
+VERSION = '0.1.405'
 DESCRIPTION = 'Minecraft Script Programming language'
 
 # Setting up
 setup(
     name="minecraft_script",
     version=VERSION,
     author="Joyful-Bard",
```


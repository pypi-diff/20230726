# Comparing `tmp/shell_whiz-0.2.1.tar.gz` & `tmp/shell_whiz-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_whiz-0.2.1.tar", max compression
+gzip compressed data, was "shell_whiz-0.2.2.tar", max compression
```

## Comparing `shell_whiz-0.2.1.tar` & `shell_whiz-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-07-25 22:50:24.716074 shell_whiz-0.2.1/LICENSE
--rw-r--r--   0        0        0     3353 2023-07-25 22:50:24.716074 shell_whiz-0.2.1/README.md
--rw-r--r--   0        0        0      538 2023-07-25 22:50:24.724074 shell_whiz-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4186 2023-07-25 22:50:24.724074 shell_whiz-0.2.1/shell_whiz/__init__.py
--rw-r--r--   0        0        0       58 2023-07-25 22:50:24.724074 shell_whiz-0.2.1/shell_whiz/__main__.py
--rw-r--r--   0        0        0     1686 2023-07-25 22:50:24.724074 shell_whiz-0.2.1/shell_whiz/config.py
--rw-r--r--   0        0        0      378 2023-07-25 22:50:24.724074 shell_whiz-0.2.1/shell_whiz/constants.py
--rw-r--r--   0        0        0      108 2023-07-25 22:50:24.724074 shell_whiz-0.2.1/shell_whiz/exceptions.py
--rw-r--r--   0        0        0     8293 2023-07-25 22:50:24.724074 shell_whiz-0.2.1/shell_whiz/openai.py
--rw-r--r--   0        0        0     3954 1970-01-01 00:00:00.000000 shell_whiz-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-25 23:02:35.900916 shell_whiz-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3294 2023-07-25 23:02:35.900916 shell_whiz-0.2.2/README.md
+-rw-r--r--   0        0        0      538 2023-07-25 23:02:35.904917 shell_whiz-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4186 2023-07-25 23:02:35.904917 shell_whiz-0.2.2/shell_whiz/__init__.py
+-rw-r--r--   0        0        0       58 2023-07-25 23:02:35.904917 shell_whiz-0.2.2/shell_whiz/__main__.py
+-rw-r--r--   0        0        0     1686 2023-07-25 23:02:35.904917 shell_whiz-0.2.2/shell_whiz/config.py
+-rw-r--r--   0        0        0      378 2023-07-25 23:02:35.904917 shell_whiz-0.2.2/shell_whiz/constants.py
+-rw-r--r--   0        0        0      108 2023-07-25 23:02:35.904917 shell_whiz-0.2.2/shell_whiz/exceptions.py
+-rw-r--r--   0        0        0     8293 2023-07-25 23:02:35.904917 shell_whiz-0.2.2/shell_whiz/openai.py
+-rw-r--r--   0        0        0     3895 1970-01-01 00:00:00.000000 shell_whiz-0.2.2/PKG-INFO
```

### Comparing `shell_whiz-0.2.1/LICENSE` & `shell_whiz-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.1/README.md` & `shell_whiz-0.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -39,17 +39,16 @@
 
 This adds the command `sw` to your PATH.
 
 To use Shell Whiz, you need an API key from OpenAI. You can get this key by visiting https://platform.openai.com/account/api-keys.
 
 Then, run `sw config` to set up your API key.
 
-<details closed><summary>A note about the free API plan for new users</summary>
+### Free API plan for new users
 New users receive $5 for free to try and test the API during the first 3 months. However, it is recommended to upgrade to a paid plan in order to have a more comfortable experience using Shell Whiz. This is because the free plan has restrictions on the number of requests allowed per minute.
-</details>
 
 ## Upgrading
 To upgrade GitHub Copilot CLI, run the following command:
 ```
 $ pip install --upgrade shell-whiz
 ```
```

### Comparing `shell_whiz-0.2.1/pyproject.toml` & `shell_whiz-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shell-whiz"
-version = "0.2.1"
+version = "0.2.2"
 description = "Shell Whiz: AI assistant right in your terminal"
 authors = ["Tamerlan Bimzhanov <bimzhanovt.net@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shell_whiz"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `shell_whiz-0.2.1/shell_whiz/__init__.py` & `shell_whiz-0.2.2/shell_whiz/__init__.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.1/shell_whiz/config.py` & `shell_whiz-0.2.2/shell_whiz/config.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.1/shell_whiz/openai.py` & `shell_whiz-0.2.2/shell_whiz/openai.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.2.1/PKG-INFO` & `shell_whiz-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-whiz
-Version: 0.2.1
+Version: 0.2.2
 Summary: Shell Whiz: AI assistant right in your terminal
 Author: Tamerlan Bimzhanov
 Author-email: bimzhanovt.net@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
@@ -56,17 +56,16 @@
 
 This adds the command `sw` to your PATH.
 
 To use Shell Whiz, you need an API key from OpenAI. You can get this key by visiting https://platform.openai.com/account/api-keys.
 
 Then, run `sw config` to set up your API key.
 
-<details closed><summary>A note about the free API plan for new users</summary>
+### Free API plan for new users
 New users receive $5 for free to try and test the API during the first 3 months. However, it is recommended to upgrade to a paid plan in order to have a more comfortable experience using Shell Whiz. This is because the free plan has restrictions on the number of requests allowed per minute.
-</details>
 
 ## Upgrading
 To upgrade GitHub Copilot CLI, run the following command:
 ```
 $ pip install --upgrade shell-whiz
 ```
```


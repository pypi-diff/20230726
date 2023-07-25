# Comparing `tmp/shell_whiz-0.1.9.tar.gz` & `tmp/shell_whiz-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_whiz-0.1.9.tar", max compression
+gzip compressed data, was "shell_whiz-0.2.0.tar", max compression
```

## Comparing `shell_whiz-0.1.9.tar` & `shell_whiz-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-07-25 22:37:50.555686 shell_whiz-0.1.9/LICENSE
--rw-r--r--   0        0        0     3305 2023-07-25 22:37:50.555686 shell_whiz-0.1.9/README.md
--rw-r--r--   0        0        0      538 2023-07-25 22:37:50.559686 shell_whiz-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     4186 2023-07-25 22:37:50.559686 shell_whiz-0.1.9/shell_whiz/__init__.py
--rw-r--r--   0        0        0       58 2023-07-25 22:37:50.559686 shell_whiz-0.1.9/shell_whiz/__main__.py
--rw-r--r--   0        0        0     1686 2023-07-25 22:37:50.559686 shell_whiz-0.1.9/shell_whiz/config.py
--rw-r--r--   0        0        0      378 2023-07-25 22:37:50.559686 shell_whiz-0.1.9/shell_whiz/constants.py
--rw-r--r--   0        0        0      108 2023-07-25 22:37:50.559686 shell_whiz-0.1.9/shell_whiz/exceptions.py
--rw-r--r--   0        0        0     8293 2023-07-25 22:37:50.559686 shell_whiz-0.1.9/shell_whiz/openai.py
--rw-r--r--   0        0        0     3906 1970-01-01 00:00:00.000000 shell_whiz-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-25 22:43:33.792382 shell_whiz-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3323 2023-07-25 22:43:33.792382 shell_whiz-0.2.0/README.md
+-rw-r--r--   0        0        0      538 2023-07-25 22:43:33.796382 shell_whiz-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4186 2023-07-25 22:43:33.796382 shell_whiz-0.2.0/shell_whiz/__init__.py
+-rw-r--r--   0        0        0       58 2023-07-25 22:43:33.796382 shell_whiz-0.2.0/shell_whiz/__main__.py
+-rw-r--r--   0        0        0     1686 2023-07-25 22:43:33.796382 shell_whiz-0.2.0/shell_whiz/config.py
+-rw-r--r--   0        0        0      378 2023-07-25 22:43:33.796382 shell_whiz-0.2.0/shell_whiz/constants.py
+-rw-r--r--   0        0        0      108 2023-07-25 22:43:33.796382 shell_whiz-0.2.0/shell_whiz/exceptions.py
+-rw-r--r--   0        0        0     8293 2023-07-25 22:43:33.796382 shell_whiz-0.2.0/shell_whiz/openai.py
+-rw-r--r--   0        0        0     3924 1970-01-01 00:00:00.000000 shell_whiz-0.2.0/PKG-INFO
```

### Comparing `shell_whiz-0.1.9/LICENSE` & `shell_whiz-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.9/README.md` & `shell_whiz-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,17 +68,19 @@
 To track API usage and costs, you can check the [OpenAI API Usage](https://platform.openai.com/account/usage) page.
 
 ## More examples
 <p align="center">
   <img
     src="https://github.com/beimzhan/shell-whiz/blob/main/examples/create_a_4_GB_file_with_random_data.gif?raw=true"
   />
+  <br />
   <img
     src="https://github.com/beimzhan/shell-whiz/blob/main/examples/list_processes_sorted_by_memory_usage.gif?raw=true"
   />
   <img
     src="https://github.com/beimzhan/shell-whiz/blob/main/examples/most_frequently_modified_files_in_the_repository.gif?raw=true"
   />
+  <br />
 </p>
 
 ## License
 Shell Whiz is licensed under the GNU General Public License v3.0. See [LICENSE](LICENSE) for more information.
```

### Comparing `shell_whiz-0.1.9/pyproject.toml` & `shell_whiz-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shell-whiz"
-version = "0.1.9"
+version = "0.2.0"
 description = "Shell Whiz: AI assistant right in your terminal"
 authors = ["Tamerlan Bimzhanov <bimzhanovt.net@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shell_whiz"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `shell_whiz-0.1.9/shell_whiz/__init__.py` & `shell_whiz-0.2.0/shell_whiz/__init__.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.9/shell_whiz/config.py` & `shell_whiz-0.2.0/shell_whiz/config.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.9/shell_whiz/openai.py` & `shell_whiz-0.2.0/shell_whiz/openai.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.9/PKG-INFO` & `shell_whiz-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-whiz
-Version: 0.1.9
+Version: 0.2.0
 Summary: Shell Whiz: AI assistant right in your terminal
 Author: Tamerlan Bimzhanov
 Author-email: bimzhanovt.net@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
@@ -85,18 +85,20 @@
 To track API usage and costs, you can check the [OpenAI API Usage](https://platform.openai.com/account/usage) page.
 
 ## More examples
 <p align="center">
   <img
     src="https://github.com/beimzhan/shell-whiz/blob/main/examples/create_a_4_GB_file_with_random_data.gif?raw=true"
   />
+  <br />
   <img
     src="https://github.com/beimzhan/shell-whiz/blob/main/examples/list_processes_sorted_by_memory_usage.gif?raw=true"
   />
   <img
     src="https://github.com/beimzhan/shell-whiz/blob/main/examples/most_frequently_modified_files_in_the_repository.gif?raw=true"
   />
+  <br />
 </p>
 
 ## License
 Shell Whiz is licensed under the GNU General Public License v3.0. See [LICENSE](LICENSE) for more information.
```


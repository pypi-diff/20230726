# Comparing `tmp/json-grep-1.2.2.tar.gz` & `tmp/json-grep-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-grep-1.2.2.tar", last modified: Tue Jun 27 08:53:04 2023, max compression
+gzip compressed data, was "json-grep-1.3.0.tar", last modified: Wed Jul 26 09:41:31 2023, max compression
```

## Comparing `json-grep-1.2.2.tar` & `json-grep-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-06-27 08:53:04.698366 json-grep-1.2.2/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)       24 2021-03-10 21:40:32.000000 json-grep-1.2.2/MANIFEST.in
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1793 2023-06-27 08:53:04.698366 json-grep-1.2.2/PKG-INFO
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1372 2023-05-15 09:17:46.000000 json-grep-1.2.2/README.md
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-06-27 08:53:04.698366 json-grep-1.2.2/json_grep.egg-info/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1793 2023-06-27 08:53:04.000000 json-grep-1.2.2/json_grep.egg-info/PKG-INFO
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      396 2023-06-27 08:53:04.000000 json-grep-1.2.2/json_grep.egg-info/SOURCES.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-06-27 08:53:04.000000 json-grep-1.2.2/json_grep.egg-info/dependency_links.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      106 2023-06-27 08:53:04.000000 json-grep-1.2.2/json_grep.egg-info/entry_points.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-06-27 08:53:04.000000 json-grep-1.2.2/json_grep.egg-info/not-zip-safe
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        9 2023-06-27 08:53:04.000000 json-grep-1.2.2/json_grep.egg-info/top_level.txt
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-06-27 08:53:04.698366 json-grep-1.2.2/jsongrep/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        5 2023-06-27 08:52:37.000000 json-grep-1.2.2/jsongrep/VERSION
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 18:47:36.000000 json-grep-1.2.2/jsongrep/__init__.py
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-06-27 08:53:04.698366 json-grep-1.2.2/jsongrep/libs/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 21:48:52.000000 json-grep-1.2.2/jsongrep/libs/__init__.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      766 2023-06-27 07:16:08.000000 json-grep-1.2.2/jsongrep/libs/cli_colors.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     3350 2023-06-27 08:49:11.000000 json-grep-1.2.2/jsongrep/libs/json_filter.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      333 2021-08-06 07:59:08.000000 json-grep-1.2.2/jsongrep/libs/setuptools.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     2364 2023-06-27 07:00:36.000000 json-grep-1.2.2/jsongrep/main.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)       38 2023-06-27 08:53:04.698366 json-grep-1.2.2/setup.cfg
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1142 2021-03-10 21:46:39.000000 json-grep-1.2.2/setup.py
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-07-26 09:41:31.294892 json-grep-1.3.0/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)       24 2021-03-10 21:40:32.000000 json-grep-1.3.0/MANIFEST.in
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1974 2023-07-26 09:41:31.294892 json-grep-1.3.0/PKG-INFO
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1553 2023-07-26 09:40:21.000000 json-grep-1.3.0/README.md
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-07-26 09:41:31.294892 json-grep-1.3.0/json_grep.egg-info/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1974 2023-07-26 09:41:31.000000 json-grep-1.3.0/json_grep.egg-info/PKG-INFO
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      396 2023-07-26 09:41:31.000000 json-grep-1.3.0/json_grep.egg-info/SOURCES.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-07-26 09:41:31.000000 json-grep-1.3.0/json_grep.egg-info/dependency_links.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      106 2023-07-26 09:41:31.000000 json-grep-1.3.0/json_grep.egg-info/entry_points.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-07-26 09:41:31.000000 json-grep-1.3.0/json_grep.egg-info/not-zip-safe
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        9 2023-07-26 09:41:31.000000 json-grep-1.3.0/json_grep.egg-info/top_level.txt
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-07-26 09:41:31.294892 json-grep-1.3.0/jsongrep/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        5 2023-07-26 09:39:26.000000 json-grep-1.3.0/jsongrep/VERSION
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 18:47:36.000000 json-grep-1.3.0/jsongrep/__init__.py
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-07-26 09:41:31.294892 json-grep-1.3.0/jsongrep/libs/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2021-03-10 21:48:52.000000 json-grep-1.3.0/jsongrep/libs/__init__.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      766 2023-06-27 07:16:08.000000 json-grep-1.3.0/jsongrep/libs/cli_colors.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     4519 2023-07-26 09:38:08.000000 json-grep-1.3.0/jsongrep/libs/json_filter.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      333 2021-08-06 07:59:08.000000 json-grep-1.3.0/jsongrep/libs/setuptools.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     2681 2023-07-26 09:34:46.000000 json-grep-1.3.0/jsongrep/main.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)       38 2023-07-26 09:41:31.294892 json-grep-1.3.0/setup.cfg
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1142 2021-03-10 21:46:39.000000 json-grep-1.3.0/setup.py
```

### Comparing `json-grep-1.2.2/PKG-INFO` & `json-grep-1.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-grep
-Version: 1.2.2
+Version: 1.3.0
 Summary: Filtering JSON dict keys from STDOUT
 Home-page: https://gitlab.com/alda78/json-grep
 Author: Ales Adamek
 Author-email: alda78@seznam.cz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,30 +16,32 @@
 
 ## Description
 Simple tool for filtering JSON dict keys from STDOUT
 
 ## Usage
 ```
 json-grep --help
-usage: json-grep [-h] [-m] [-v] [-e] filter_keys [filter_keys ...]
 
-JSON GREP v1.2.0 is utility for filtering selected keys from json string piped from STDOUT
+usage: json-grep [-h] [-m] [-v] [-l HIGHLIGHT] [-i IHIGHLIGHT] [-e] filter_keys [filter_keys ...]
+
+JSON GREP v1.3.0 is utility for filtering selected keys from json string piped from STDOUT
 
 positional arguments:
-  filter_keys           List of keys which you want to filter from json dict.If key is in deeper level of tree 
-                        structure use '.' separator to specify how deep is key in dict tree structure.
-                        You can also use '*' at the end of key name to filter keys as 'beginning with'.
-                        You can also specify value of item which you want to pass only by operator '=' or
+  filter_keys           List of keys which you want to filter from json dict. If key is in deeper level of tree structure use '.' separator to specify how deep is key in dict tree structure. You can also use '*' at the end of key name to filter keys as 'beginning with'. You can also specify value of item which you want to pass only by operator '=' or
                         '~'. '~' means that value is somewhere in string.
 
 options:
   -h, --help            show this help message and exit
   -m, --multiline-output
                         Use multiline output for filtered result
   -v, --values_only     Show only values without keys description
+  -l HIGHLIGHT, --hl HIGHLIGHT
+                        Highlight case sensitively words in filtered results
+  -i IHIGHLIGHT, --ihl IHIGHLIGHT
+                        Highlight case insensitively words in filtered results
   -e, --show-errors     Show errors caused by json decode
 ```
 
 ## Installation
 ```bash
 wget https://gitlab.com/alda78/json-grep/-/archive/master/json-grep-master.tar && \
 tar -xf json-grep-master.tar && \
```

### Comparing `json-grep-1.2.2/README.md` & `json-grep-1.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 
 ## Description
 Simple tool for filtering JSON dict keys from STDOUT
 
 ## Usage
 ```
 json-grep --help
-usage: json-grep [-h] [-m] [-v] [-e] filter_keys [filter_keys ...]
 
-JSON GREP v1.2.0 is utility for filtering selected keys from json string piped from STDOUT
+usage: json-grep [-h] [-m] [-v] [-l HIGHLIGHT] [-i IHIGHLIGHT] [-e] filter_keys [filter_keys ...]
+
+JSON GREP v1.3.0 is utility for filtering selected keys from json string piped from STDOUT
 
 positional arguments:
-  filter_keys           List of keys which you want to filter from json dict.If key is in deeper level of tree 
-                        structure use '.' separator to specify how deep is key in dict tree structure.
-                        You can also use '*' at the end of key name to filter keys as 'beginning with'.
-                        You can also specify value of item which you want to pass only by operator '=' or
+  filter_keys           List of keys which you want to filter from json dict. If key is in deeper level of tree structure use '.' separator to specify how deep is key in dict tree structure. You can also use '*' at the end of key name to filter keys as 'beginning with'. You can also specify value of item which you want to pass only by operator '=' or
                         '~'. '~' means that value is somewhere in string.
 
 options:
   -h, --help            show this help message and exit
   -m, --multiline-output
                         Use multiline output for filtered result
   -v, --values_only     Show only values without keys description
+  -l HIGHLIGHT, --hl HIGHLIGHT
+                        Highlight case sensitively words in filtered results
+  -i IHIGHLIGHT, --ihl IHIGHLIGHT
+                        Highlight case insensitively words in filtered results
   -e, --show-errors     Show errors caused by json decode
 ```
 
 ## Installation
 ```bash
 wget https://gitlab.com/alda78/json-grep/-/archive/master/json-grep-master.tar && \
 tar -xf json-grep-master.tar && \
```

### Comparing `json-grep-1.2.2/json_grep.egg-info/PKG-INFO` & `json-grep-1.3.0/json_grep.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-grep
-Version: 1.2.2
+Version: 1.3.0
 Summary: Filtering JSON dict keys from STDOUT
 Home-page: https://gitlab.com/alda78/json-grep
 Author: Ales Adamek
 Author-email: alda78@seznam.cz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,30 +16,32 @@
 
 ## Description
 Simple tool for filtering JSON dict keys from STDOUT
 
 ## Usage
 ```
 json-grep --help
-usage: json-grep [-h] [-m] [-v] [-e] filter_keys [filter_keys ...]
 
-JSON GREP v1.2.0 is utility for filtering selected keys from json string piped from STDOUT
+usage: json-grep [-h] [-m] [-v] [-l HIGHLIGHT] [-i IHIGHLIGHT] [-e] filter_keys [filter_keys ...]
+
+JSON GREP v1.3.0 is utility for filtering selected keys from json string piped from STDOUT
 
 positional arguments:
-  filter_keys           List of keys which you want to filter from json dict.If key is in deeper level of tree 
-                        structure use '.' separator to specify how deep is key in dict tree structure.
-                        You can also use '*' at the end of key name to filter keys as 'beginning with'.
-                        You can also specify value of item which you want to pass only by operator '=' or
+  filter_keys           List of keys which you want to filter from json dict. If key is in deeper level of tree structure use '.' separator to specify how deep is key in dict tree structure. You can also use '*' at the end of key name to filter keys as 'beginning with'. You can also specify value of item which you want to pass only by operator '=' or
                         '~'. '~' means that value is somewhere in string.
 
 options:
   -h, --help            show this help message and exit
   -m, --multiline-output
                         Use multiline output for filtered result
   -v, --values_only     Show only values without keys description
+  -l HIGHLIGHT, --hl HIGHLIGHT
+                        Highlight case sensitively words in filtered results
+  -i IHIGHLIGHT, --ihl IHIGHLIGHT
+                        Highlight case insensitively words in filtered results
   -e, --show-errors     Show errors caused by json decode
 ```
 
 ## Installation
 ```bash
 wget https://gitlab.com/alda78/json-grep/-/archive/master/json-grep-master.tar && \
 tar -xf json-grep-master.tar && \
```

### Comparing `json-grep-1.2.2/jsongrep/libs/cli_colors.py` & `json-grep-1.3.0/jsongrep/libs/cli_colors.py`

 * *Files identical despite different names*

### Comparing `json-grep-1.2.2/jsongrep/main.py` & `json-grep-1.3.0/jsongrep/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,32 +21,38 @@
         "at the end of key name to filter keys as 'beginning with'. "
         "You can also specify value of item which you want to pass "
         "only by operator '=' or '~'. '~' means "
         "that value is somewhere in string.")
                         )
     parser.add_argument("-m", "--multiline-output", dest="multiline_output", default=False, action="store_true", help="Use multiline output for filtered result")
     parser.add_argument("-v", "--values_only", dest="values_only", default=False, action="store_true", help="Show only values without keys description")
+    parser.add_argument("-l", "--hl", dest="highlight", action="append", help="Highlight case sensitively words in filtered results")
+    parser.add_argument("-i", "--ihl", dest="ihighlight", action="append", help="Highlight case insensitively words in filtered results")
     parser.add_argument("-e", "--show-errors", dest="show_errors", default=False, action="store_true", help="Show errors caused by json decode")
 
     args = parser.parse_args()
     return args
 
 
 def main():
     signal.signal(signal.SIGINT, _handle_exit)
     args = _handle_args()
 
-    is_value_operator_used = any([True for key in args.filter_keys if JsonFilter.parse_key(key)[2]])
+    json_filter = JsonFilter(args.filter_keys)
+    json_filter.multiline_output = args.multiline_output
+    json_filter.values_only = args.values_only
+    json_filter.highlight_values = args.highlight
+    json_filter.ihighlight_values = args.ihighlight
 
     for line in sys.stdin:
         try:
-            results_data = JsonFilter.filter_keys_and_values(line, args.filter_keys, is_value_operator_used)
-            if results_data:
-                result = JsonFilter.format_result(results_data, multiline_output=args.multiline_output, values_only=args.values_only)
-                sys.stdout.write(result)
+            filtered_data = json_filter.filter_keys_and_values(line)
+            if filtered_data:
+                output = json_filter.format_result(filtered_data)
+                sys.stdout.write(output)
         except JsonFilterException as ex:
             if args.show_errors:
                 sys.stderr.write("\33[31mJsonFilterException\33[0m: {}\n".format(ex))
     print("DONE.")
 
 
 if __name__ == '__main__':
```

### Comparing `json-grep-1.2.2/setup.py` & `json-grep-1.3.0/setup.py`

 * *Files identical despite different names*


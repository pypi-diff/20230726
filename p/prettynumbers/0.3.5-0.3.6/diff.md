# Comparing `tmp/prettynumbers-0.3.5.tar.gz` & `tmp/prettynumbers-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettynumbers-0.3.5.tar", max compression
+gzip compressed data, was "prettynumbers-0.3.6.tar", max compression
```

## Comparing `prettynumbers-0.3.5.tar` & `prettynumbers-0.3.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    14849 2023-07-26 08:59:46.080920 prettynumbers-0.3.5/LICENSE.txt
--rw-r--r--   0        0        0     1138 2023-07-26 08:59:46.080920 prettynumbers-0.3.5/README.md
--rw-r--r--   0        0        0      138 2023-07-26 08:59:46.080920 prettynumbers-0.3.5/pretty_numbers/__init__.py
--rwxr-xr-x   0        0        0     2580 2023-07-26 08:59:46.080920 prettynumbers-0.3.5/pretty_numbers/pretty_numbers.py
--rw-r--r--   0        0        0        0 2023-07-26 08:59:46.080920 prettynumbers-0.3.5/pretty_numbers/py.typed
--rw-r--r--   0        0        0      807 2023-07-26 08:59:46.080920 prettynumbers-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 prettynumbers-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    14849 2023-07-26 10:44:02.217744 prettynumbers-0.3.6/LICENSE.txt
+-rw-r--r--   0        0        0     1138 2023-07-26 10:44:02.217744 prettynumbers-0.3.6/README.md
+-rw-r--r--   0        0        0      138 2023-07-26 10:44:02.217744 prettynumbers-0.3.6/pretty_numbers/__init__.py
+-rwxr-xr-x   0        0        0     2405 2023-07-26 10:44:02.221744 prettynumbers-0.3.6/pretty_numbers/pretty_numbers.py
+-rw-r--r--   0        0        0        0 2023-07-26 10:44:02.221744 prettynumbers-0.3.6/pretty_numbers/py.typed
+-rw-r--r--   0        0        0      807 2023-07-26 10:44:02.221744 prettynumbers-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 prettynumbers-0.3.6/PKG-INFO
```

### Comparing `prettynumbers-0.3.5/LICENSE.txt` & `prettynumbers-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.3.5/README.md` & `prettynumbers-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.3.5/pretty_numbers/pretty_numbers.py` & `prettynumbers-0.3.6/pretty_numbers/pretty_numbers.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,24 +42,17 @@
 
 
 def getPrettyNumbersText(list_of_strings: Sequence[Any]) -> str:
     nums = set()
     text_result = set()
     for i in list_of_strings:
         try:
-            is_digit = i.isdigit()
-        except AttributeError:
-            is_digit = True
-        if is_digit:
-            try:
-                nums.add(int(i))
-            except TypeError:
-                text_result.add(str(i))
-        else:
-            text_result.add(i)
+            nums.add(int(i))
+        except (TypeError, ValueError):
+            text_result.add(str(i))
     result = getPrettyTextFromSet(nums)
     if not text_result:
         return result
     texts = list(text_result)
     texts.sort()
     final_text = ",".join(texts)
     if result:
```

### Comparing `prettynumbers-0.3.5/pyproject.toml` & `prettynumbers-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prettynumbers"
-version = "0.3.5"
+version = "0.3.6"
 authors = ["gerardk <gerardk@gmail.com>"]
 description="Display a range of numbers in a human readable way"
 license="GNU GENERAL PUBLIC LICENSE"
 packages = [{include = "pretty_numbers"}]
 readme = "README.md"
 repository = "https://github.com/vfxGer/pretty-numbers"
```

### Comparing `prettynumbers-0.3.5/PKG-INFO` & `prettynumbers-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettynumbers
-Version: 0.3.5
+Version: 0.3.6
 Summary: Display a range of numbers in a human readable way
 Home-page: https://github.com/vfxGer/pretty-numbers
 License: GNU GENERAL PUBLIC LICENSE
 Author: gerardk
 Author-email: gerardk@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: Other/Proprietary License
```


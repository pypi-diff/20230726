# Comparing `tmp/unexpected_isaves-2.1.2.tar.gz` & `tmp/unexpected_isaves-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unexpected_isaves-2.1.2.tar", last modified: Mon Apr 17 22:15:15 2023, max compression
+gzip compressed data, was "unexpected_isaves-2.1.3.tar", last modified: Tue Jul 25 23:11:25 2023, max compression
```

## Comparing `unexpected_isaves-2.1.2.tar` & `unexpected_isaves-2.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:15:15.866954 unexpected_isaves-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-17 22:15:06.000000 unexpected_isaves-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-04-17 22:15:15.866954 unexpected_isaves-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-17 22:15:06.000000 unexpected_isaves-2.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-17 22:15:06.000000 unexpected_isaves-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 22:15:15.866954 unexpected_isaves-2.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:15:15.862954 unexpected_isaves-2.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:15:15.862954 unexpected_isaves-2.1.2/src/unexpected_isaves/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:15:06.000000 unexpected_isaves-2.1.2/src/unexpected_isaves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24301 2023-04-17 22:15:06.000000 unexpected_isaves-2.1.2/src/unexpected_isaves/blocks.json
--rw-r--r--   0 runner    (1001) docker     (123)    18648 2023-04-17 22:15:06.000000 unexpected_isaves-2.1.2/src/unexpected_isaves/save_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:15:15.862954 unexpected_isaves-2.1.2/src/unexpected_isaves.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-04-17 22:15:15.000000 unexpected_isaves-2.1.2/src/unexpected_isaves.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-17 22:15:15.000000 unexpected_isaves-2.1.2/src/unexpected_isaves.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:15:15.000000 unexpected_isaves-2.1.2/src/unexpected_isaves.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-17 22:15:15.000000 unexpected_isaves-2.1.2/src/unexpected_isaves.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 22:15:15.000000 unexpected_isaves-2.1.2/src/unexpected_isaves.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:11:25.414724 unexpected_isaves-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-25 23:11:15.000000 unexpected_isaves-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-07-25 23:11:25.414724 unexpected_isaves-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-07-25 23:11:15.000000 unexpected_isaves-2.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-25 23:11:15.000000 unexpected_isaves-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 23:11:25.414724 unexpected_isaves-2.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:11:25.410724 unexpected_isaves-2.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:11:25.414724 unexpected_isaves-2.1.3/src/unexpected_isaves/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 23:11:15.000000 unexpected_isaves-2.1.3/src/unexpected_isaves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24301 2023-07-25 23:11:15.000000 unexpected_isaves-2.1.3/src/unexpected_isaves/blocks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18718 2023-07-25 23:11:15.000000 unexpected_isaves-2.1.3/src/unexpected_isaves/save_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:11:25.414724 unexpected_isaves-2.1.3/src/unexpected_isaves.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-07-25 23:11:25.000000 unexpected_isaves-2.1.3/src/unexpected_isaves.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-25 23:11:25.000000 unexpected_isaves-2.1.3/src/unexpected_isaves.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 23:11:25.000000 unexpected_isaves-2.1.3/src/unexpected_isaves.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-25 23:11:25.000000 unexpected_isaves-2.1.3/src/unexpected_isaves.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 23:11:25.000000 unexpected_isaves-2.1.3/src/unexpected_isaves.egg-info/top_level.txt
```

### Comparing `unexpected_isaves-2.1.2/LICENSE` & `unexpected_isaves-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unexpected_isaves-2.1.2/PKG-INFO` & `unexpected_isaves-2.1.3/src/unexpected_isaves.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: unexpected_isaves
-Version: 2.1.2
+Name: unexpected-isaves
+Version: 2.1.3
 Summary: A Python library that paints an image on a spreadsheet, builds its pixel art in Minecraft, makes its ascii art, or makes a rubik's cube art out of it.
 Author-email: Eric Mendes <ericvelasco.2000@gmail.com>, Henrique Souza <henriquesoliveira05@gmail.com>
 Maintainer-email: Eric Mendes <ericvelasco.2000@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Eric Mendes
         
@@ -114,10 +114,10 @@
 
 ## Contributing :pencil:
 Just like Minecraft, everything's better when shared and built together.
 
 Contributions are welcome and appreciated. Make sure to read our [guide for contributing](https://github.com/Eric-Mendes/unexpected_isaves/blob/main/CONTRIBUTING.md) and don't forget to check out our [code of conduct](https://github.com/Eric-Mendes/unexpected_isaves/blob/main/CODE_OF_CONDUCT.md).
 
 ## Into the wild
-So you've used this tool to create the most awesome art ever, and now you want to share it in your social media? Please use *#unexpected_isaves* when you post it.
+So you've used this tool to create the most awesome art ever? Please consider leaving a star on the repo. It helps a lot.
 
 Have fun!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unexpected_isaves Version: 2.1.2 Summary: A Python
+Metadata-Version: 2.1 Name: unexpected-isaves Version: 2.1.3 Summary: A Python
 library that paints an image on a spreadsheet, builds its pixel art in
 Minecraft, makes its ascii art, or makes a rubik's cube art out of it. Author-
 email: Eric Mendes
 2000@gmail.com>, Henrique Souza
 gmail.com> Maintainer-email: Eric Mendes
 2000@gmail.com> License: MIT License Copyright (c) 2022 Eric Mendes Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
@@ -78,10 +78,9 @@
 github.com/Eric-Mendes/unexpected-isaves/wiki) for more information about this
 project if you want. ## Contributing :pencil: Just like Minecraft, everything's
 better when shared and built together. Contributions are welcome and
 appreciated. Make sure to read our [guide for contributing](https://github.com/
 Eric-Mendes/unexpected_isaves/blob/main/CONTRIBUTING.md) and don't forget to
 check out our [code of conduct](https://github.com/Eric-Mendes/
 unexpected_isaves/blob/main/CODE_OF_CONDUCT.md). ## Into the wild So you've
-used this tool to create the most awesome art ever, and now you want to share
-it in your social media? Please use *#unexpected_isaves* when you post it. Have
-fun!
+used this tool to create the most awesome art ever? Please consider leaving a
+star on the repo. It helps a lot. Have fun!
```

### Comparing `unexpected_isaves-2.1.2/README.md` & `unexpected_isaves-2.1.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -67,10 +67,10 @@
 
 ## Contributing :pencil:
 Just like Minecraft, everything's better when shared and built together.
 
 Contributions are welcome and appreciated. Make sure to read our [guide for contributing](https://github.com/Eric-Mendes/unexpected_isaves/blob/main/CONTRIBUTING.md) and don't forget to check out our [code of conduct](https://github.com/Eric-Mendes/unexpected_isaves/blob/main/CODE_OF_CONDUCT.md).
 
 ## Into the wild
-So you've used this tool to create the most awesome art ever, and now you want to share it in your social media? Please use *#unexpected_isaves* when you post it.
+So you've used this tool to create the most awesome art ever? Please consider leaving a star on the repo. It helps a lot.
 
 Have fun!
```

#### html2text {}

```diff
@@ -45,10 +45,9 @@
 github.com/Eric-Mendes/unexpected-isaves/wiki) for more information about this
 project if you want. ## Contributing :pencil: Just like Minecraft, everything's
 better when shared and built together. Contributions are welcome and
 appreciated. Make sure to read our [guide for contributing](https://github.com/
 Eric-Mendes/unexpected_isaves/blob/main/CONTRIBUTING.md) and don't forget to
 check out our [code of conduct](https://github.com/Eric-Mendes/
 unexpected_isaves/blob/main/CODE_OF_CONDUCT.md). ## Into the wild So you've
-used this tool to create the most awesome art ever, and now you want to share
-it in your social media? Please use *#unexpected_isaves* when you post it. Have
-fun!
+used this tool to create the most awesome art ever? Please consider leaving a
+star on the repo. It helps a lot. Have fun!
```

### Comparing `unexpected_isaves-2.1.2/pyproject.toml` & `unexpected_isaves-2.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "unexpected_isaves"
-version = "2.1.2"
+version = "2.1.3"
 description = "A Python library that paints an image on a spreadsheet, builds its pixel art in Minecraft, makes its ascii art, or makes a rubik's cube art out of it."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["minecraft", "pixel", "art", "excel", "spreadsheet", "ascii", "rubiks"]
 authors = [
   {name = "Eric Mendes", email = "ericvelasco.2000@gmail.com" },
```

### Comparing `unexpected_isaves-2.1.2/src/unexpected_isaves/blocks.json` & `unexpected_isaves-2.1.3/src/unexpected_isaves/blocks.json`

 * *Files identical despite different names*

### Comparing `unexpected_isaves-2.1.2/src/unexpected_isaves/save_image.py` & `unexpected_isaves-2.1.3/src/unexpected_isaves/save_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,16 @@
         datapack_version = 8
     elif minecraft_version == "1.18.2":
         datapack_version = 9
     elif minecraft_version >= "1.19.0" and minecraft_version <= "1.19.3":
         datapack_version = 10
     elif minecraft_version == "1.19.4":
         datapack_version = 12
+    elif minecraft_version == "1.20.0":
+        datapack_version = 15
     else:
         raise ValueError(
             "Unsupported minecraft_version. If you feel like this is a mistake, open an issue at https://github.com/Eric-Mendes/unexpected-isaves/issues to let us know."
         )
 
     pack_mcmeta = {
         "pack": {
```

### Comparing `unexpected_isaves-2.1.2/src/unexpected_isaves.egg-info/PKG-INFO` & `unexpected_isaves-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: unexpected-isaves
-Version: 2.1.2
+Name: unexpected_isaves
+Version: 2.1.3
 Summary: A Python library that paints an image on a spreadsheet, builds its pixel art in Minecraft, makes its ascii art, or makes a rubik's cube art out of it.
 Author-email: Eric Mendes <ericvelasco.2000@gmail.com>, Henrique Souza <henriquesoliveira05@gmail.com>
 Maintainer-email: Eric Mendes <ericvelasco.2000@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Eric Mendes
         
@@ -114,10 +114,10 @@
 
 ## Contributing :pencil:
 Just like Minecraft, everything's better when shared and built together.
 
 Contributions are welcome and appreciated. Make sure to read our [guide for contributing](https://github.com/Eric-Mendes/unexpected_isaves/blob/main/CONTRIBUTING.md) and don't forget to check out our [code of conduct](https://github.com/Eric-Mendes/unexpected_isaves/blob/main/CODE_OF_CONDUCT.md).
 
 ## Into the wild
-So you've used this tool to create the most awesome art ever, and now you want to share it in your social media? Please use *#unexpected_isaves* when you post it.
+So you've used this tool to create the most awesome art ever? Please consider leaving a star on the repo. It helps a lot.
 
 Have fun!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unexpected-isaves Version: 2.1.2 Summary: A Python
+Metadata-Version: 2.1 Name: unexpected_isaves Version: 2.1.3 Summary: A Python
 library that paints an image on a spreadsheet, builds its pixel art in
 Minecraft, makes its ascii art, or makes a rubik's cube art out of it. Author-
 email: Eric Mendes
 2000@gmail.com>, Henrique Souza
 gmail.com> Maintainer-email: Eric Mendes
 2000@gmail.com> License: MIT License Copyright (c) 2022 Eric Mendes Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
@@ -78,10 +78,9 @@
 github.com/Eric-Mendes/unexpected-isaves/wiki) for more information about this
 project if you want. ## Contributing :pencil: Just like Minecraft, everything's
 better when shared and built together. Contributions are welcome and
 appreciated. Make sure to read our [guide for contributing](https://github.com/
 Eric-Mendes/unexpected_isaves/blob/main/CONTRIBUTING.md) and don't forget to
 check out our [code of conduct](https://github.com/Eric-Mendes/
 unexpected_isaves/blob/main/CODE_OF_CONDUCT.md). ## Into the wild So you've
-used this tool to create the most awesome art ever, and now you want to share
-it in your social media? Please use *#unexpected_isaves* when you post it. Have
-fun!
+used this tool to create the most awesome art ever? Please consider leaving a
+star on the repo. It helps a lot. Have fun!
```


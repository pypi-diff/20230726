# Comparing `tmp/dynrender_skia-0.1.5.tar.gz` & `tmp/dynrender_skia-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynrender_skia-0.1.5.tar", max compression
+gzip compressed data, was "dynrender_skia-0.1.6.tar", max compression
```

## Comparing `dynrender_skia-0.1.5.tar` & `dynrender_skia-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    35149 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/LICENSE
--rw-r--r--   0        0        0     1504 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/README.md
--rw-r--r--   0        0        0     2225 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/Core.py
--rw-r--r--   0        0        0    18382 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/DynAdditional.py
--rw-r--r--   0        0        0     5499 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/DynConfig.py
--rw-r--r--   0        0        0    11153 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/DynHeader.py
--rw-r--r--   0        0        0    30723 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/DynMajor.py
--rw-r--r--   0        0        0     1204 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/DynRepost.py
--rw-r--r--   0        0        0      849 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/DynStyle.py
--rw-r--r--   0        0        0    12798 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/DynText.py
--rw-r--r--   0        0        0     4084 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/DynTools.py
--rw-r--r--   0        0        0   334112 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/Static.zip
--rw-r--r--   0        0        0        0 2023-07-24 12:25:53.009645 dynrender_skia-0.1.5/dynrender_skia/__init__.py
--rw-r--r--   0        0        0      538 2023-07-24 12:25:53.013645 dynrender_skia-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2261 1970-01-01 00:00:00.000000 dynrender_skia-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-26 13:25:02.586640 dynrender_skia-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1504 2023-07-26 13:25:02.586640 dynrender_skia-0.1.6/README.md
+-rw-r--r--   0        0        0     2225 2023-07-26 13:25:02.586640 dynrender_skia-0.1.6/dynrender_skia/Core.py
+-rw-r--r--   0        0        0    18382 2023-07-26 13:25:02.586640 dynrender_skia-0.1.6/dynrender_skia/DynAdditional.py
+-rw-r--r--   0        0        0     5499 2023-07-26 13:25:02.586640 dynrender_skia-0.1.6/dynrender_skia/DynConfig.py
+-rw-r--r--   0        0        0    11153 2023-07-26 13:25:02.586640 dynrender_skia-0.1.6/dynrender_skia/DynHeader.py
+-rw-r--r--   0        0        0    30723 2023-07-26 13:25:02.586640 dynrender_skia-0.1.6/dynrender_skia/DynMajor.py
+-rw-r--r--   0        0        0     1209 2023-07-26 13:25:02.586640 dynrender_skia-0.1.6/dynrender_skia/DynRepost.py
+-rw-r--r--   0        0        0      849 2023-07-26 13:25:02.586640 dynrender_skia-0.1.6/dynrender_skia/DynStyle.py
+-rw-r--r--   0        0        0    12798 2023-07-26 13:25:02.586640 dynrender_skia-0.1.6/dynrender_skia/DynText.py
+-rw-r--r--   0        0        0     4084 2023-07-26 13:25:02.586640 dynrender_skia-0.1.6/dynrender_skia/DynTools.py
+-rw-r--r--   0        0        0   334112 2023-07-26 13:25:02.586640 dynrender_skia-0.1.6/dynrender_skia/Static.zip
+-rw-r--r--   0        0        0        0 2023-07-26 13:25:02.586640 dynrender_skia-0.1.6/dynrender_skia/__init__.py
+-rw-r--r--   0        0        0      538 2023-07-26 13:25:02.590641 dynrender_skia-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2261 1970-01-01 00:00:00.000000 dynrender_skia-0.1.6/PKG-INFO
```

### Comparing `dynrender_skia-0.1.5/LICENSE` & `dynrender_skia-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.5/README.md` & `dynrender_skia-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.5/dynrender_skia/Core.py` & `dynrender_skia-0.1.6/dynrender_skia/Core.py`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.5/dynrender_skia/DynAdditional.py` & `dynrender_skia-0.1.6/dynrender_skia/DynAdditional.py`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.5/dynrender_skia/DynConfig.py` & `dynrender_skia-0.1.6/dynrender_skia/DynConfig.py`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.5/dynrender_skia/DynHeader.py` & `dynrender_skia-0.1.6/dynrender_skia/DynHeader.py`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.5/dynrender_skia/DynMajor.py` & `dynrender_skia-0.1.6/dynrender_skia/DynMajor.py`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.5/dynrender_skia/DynRepost.py` & `dynrender_skia-0.1.6/dynrender_skia/DynRepost.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,11 +25,12 @@
 
     async def run(self, message: Forward):
         tasks = [RepostHeader(self.static_path, self.style).run(message.header)]
         if message.text is not None:
             tasks.append(BiliText(self.static_path, self.style).run(message.text, repost=True))
         if message.major is not None:
             tasks.append(BiliMajor(self.static_path, self.style).run(message.major, True))
-            if message.additional is not None:
-                tasks.append(BiliAdditional(self.static_path, self.style).run(message.additional, True))
+        if message.additional is not None:
+            
+            tasks.append(BiliAdditional(self.static_path, self.style).run(message.additional, True))
         result = await asyncio.gather(*tasks)
         return await merge_pictures(result)
```

### Comparing `dynrender_skia-0.1.5/dynrender_skia/DynStyle.py` & `dynrender_skia-0.1.6/dynrender_skia/DynStyle.py`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.5/dynrender_skia/DynText.py` & `dynrender_skia-0.1.6/dynrender_skia/DynText.py`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.5/dynrender_skia/DynTools.py` & `dynrender_skia-0.1.6/dynrender_skia/DynTools.py`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.5/dynrender_skia/Static.zip` & `dynrender_skia-0.1.6/dynrender_skia/Static.zip`

 * *Files identical despite different names*

### Comparing `dynrender_skia-0.1.5/pyproject.toml` & `dynrender_skia-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dynrender-skia"
-version = "0.1.5"
+version = "0.1.6"
 description = "使用skia-python将BiliBili动态渲染为图片"
 authors = ["DMC <lzxder@outlook.com>"]
 license = "GNU GPLv3"
 readme = "README.md"
 packages = [{include = "dynrender_skia"}]
 
 [tool.poetry.dependencies]
```

### Comparing `dynrender_skia-0.1.5/PKG-INFO` & `dynrender_skia-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynrender-skia
-Version: 0.1.5
+Version: 0.1.6
 Summary: 使用skia-python将BiliBili动态渲染为图片
 License: GNU GPLv3
 Author: DMC
 Author-email: lzxder@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```


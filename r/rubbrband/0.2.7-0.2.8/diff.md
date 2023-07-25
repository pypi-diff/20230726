# Comparing `tmp/rubbrband-0.2.7.tar.gz` & `tmp/rubbrband-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubbrband-0.2.7.tar", last modified: Tue Jul 18 03:17:46 2023, max compression
+gzip compressed data, was "rubbrband-0.2.8.tar", last modified: Tue Jul 25 23:05:41 2023, max compression
```

## Comparing `rubbrband-0.2.7.tar` & `rubbrband-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-07-18 03:17:46.047404 rubbrband-0.2.7/
--rw-r--r--   0 llewyn     (501) staff       (20)    11357 2023-03-07 10:22:28.000000 rubbrband-0.2.7/LICENSE
--rw-r--r--   0 llewyn     (501) staff       (20)       48 2023-02-24 08:26:52.000000 rubbrband-0.2.7/MANIFEST.in
--rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-07-18 03:17:46.047470 rubbrband-0.2.7/PKG-INFO
--rw-r--r--   0 llewyn     (501) staff       (20)       54 2023-06-07 21:39:04.000000 rubbrband-0.2.7/README.md
--rw-r--r--   0 llewyn     (501) staff       (20)      103 2023-06-19 21:09:40.000000 rubbrband-0.2.7/pyproject.toml
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-07-18 03:17:46.046405 rubbrband-0.2.7/rubbrband/
--rw-r--r--   0 llewyn     (501) staff       (20)       61 2023-06-07 21:45:01.000000 rubbrband-0.2.7/rubbrband/__init__.py
--rw-r--r--   0 llewyn     (501) staff       (20)     1206 2023-07-18 03:16:46.000000 rubbrband-0.2.7/rubbrband/main.py
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-07-18 03:17:46.047264 rubbrband-0.2.7/rubbrband.egg-info/
--rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-07-18 03:17:46.000000 rubbrband-0.2.7/rubbrband.egg-info/PKG-INFO
--rw-r--r--   0 llewyn     (501) staff       (20)      267 2023-07-18 03:17:46.000000 rubbrband-0.2.7/rubbrband.egg-info/SOURCES.txt
--rw-r--r--   0 llewyn     (501) staff       (20)        1 2023-07-18 03:17:46.000000 rubbrband-0.2.7/rubbrband.egg-info/dependency_links.txt
--rw-r--r--   0 llewyn     (501) staff       (20)       16 2023-07-18 03:17:46.000000 rubbrband-0.2.7/rubbrband.egg-info/requires.txt
--rw-r--r--   0 llewyn     (501) staff       (20)       10 2023-07-18 03:17:46.000000 rubbrband-0.2.7/rubbrband.egg-info/top_level.txt
--rw-r--r--   0 llewyn     (501) staff       (20)      259 2023-07-18 03:17:46.047746 rubbrband-0.2.7/setup.cfg
--rw-r--r--   0 llewyn     (501) staff       (20)      182 2023-06-19 21:09:40.000000 rubbrband-0.2.7/setup.py
+drwxr-xr-x   0 darren     (501) staff       (20)        0 2023-07-25 23:05:41.239253 rubbrband-0.2.8/
+-rw-r--r--   0 darren     (501) staff       (20)    11357 2023-06-13 23:04:48.000000 rubbrband-0.2.8/LICENSE
+-rw-r--r--   0 darren     (501) staff       (20)       48 2023-06-13 23:04:48.000000 rubbrband-0.2.8/MANIFEST.in
+-rw-r--r--   0 darren     (501) staff       (20)      125 2023-07-25 23:05:41.239318 rubbrband-0.2.8/PKG-INFO
+-rw-r--r--   0 darren     (501) staff       (20)       54 2023-06-13 23:22:30.000000 rubbrband-0.2.8/README.md
+-rw-r--r--   0 darren     (501) staff       (20)      103 2023-07-25 21:52:43.000000 rubbrband-0.2.8/pyproject.toml
+drwxr-xr-x   0 darren     (501) staff       (20)        0 2023-07-25 23:05:41.238263 rubbrband-0.2.8/rubbrband/
+-rw-r--r--   0 darren     (501) staff       (20)       61 2023-06-13 23:28:05.000000 rubbrband-0.2.8/rubbrband/__init__.py
+-rw-r--r--   0 darren     (501) staff       (20)     1613 2023-07-25 23:05:10.000000 rubbrband-0.2.8/rubbrband/main.py
+drwxr-xr-x   0 darren     (501) staff       (20)        0 2023-07-25 23:05:41.239087 rubbrband-0.2.8/rubbrband.egg-info/
+-rw-r--r--   0 darren     (501) staff       (20)      125 2023-07-25 23:05:41.000000 rubbrband-0.2.8/rubbrband.egg-info/PKG-INFO
+-rw-r--r--   0 darren     (501) staff       (20)      267 2023-07-25 23:05:41.000000 rubbrband-0.2.8/rubbrband.egg-info/SOURCES.txt
+-rw-r--r--   0 darren     (501) staff       (20)        1 2023-07-25 23:05:41.000000 rubbrband-0.2.8/rubbrband.egg-info/dependency_links.txt
+-rw-r--r--   0 darren     (501) staff       (20)       16 2023-07-25 23:05:41.000000 rubbrband-0.2.8/rubbrband.egg-info/requires.txt
+-rw-r--r--   0 darren     (501) staff       (20)       10 2023-07-25 23:05:41.000000 rubbrband-0.2.8/rubbrband.egg-info/top_level.txt
+-rw-r--r--   0 darren     (501) staff       (20)      259 2023-07-25 23:05:41.239615 rubbrband-0.2.8/setup.cfg
+-rw-r--r--   0 darren     (501) staff       (20)      182 2023-07-25 21:52:43.000000 rubbrband-0.2.8/setup.py
```

### Comparing `rubbrband-0.2.7/LICENSE` & `rubbrband-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rubbrband-0.2.7/rubbrband/main.py` & `rubbrband-0.2.8/rubbrband/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import io
-import uuid
+import re
 
 import PIL
+import PIL.PngImagePlugin
 import requests
 
 api_key = None
 
 
 def init(apikey):
     global api_key
@@ -17,39 +18,47 @@
     imgByteArr = io.BytesIO()
     # image.save expects a file-like as a argument
     image.save(imgByteArr, format=image.format)
     # Turn the BytesIO object back into a bytes object
     imgByteArr = imgByteArr.getvalue()
     return imgByteArr
 
+def is_url(string):
+    regex_pattern = r"^(https?|ftp):\/\/([^\s/$.?#].[^\s]*)$"
+    return bool(re.match(regex_pattern, string))
 
 def upload(image, prompt, metadata={}):
     if api_key is None:
         print("Provide an API key in the init function")
-
         return False
 
+    if type(image) == str and is_url(image):
+        image_url_response = requests.get(image)
+        if image_url_response.status_code != 200 or image_url_response.content is None:
+            return False
+        image = image_url_response.content
+
     if type(image) == PIL.PngImagePlugin.PngImageFile:
         image = image_to_byte_array(image)
 
     metadata["prompt"] = prompt
-    name = str(uuid.uuid4()) + ".jpg"
 
     response = requests.post(
         "https://block.rubbrband.com/upload_img?api_key=" + api_key,
         json={"metadata": metadata},
     )
 
     if response is None:
         return False
 
     response = response.json()
 
     if "url" not in response:
         return False
 
+    filename = response["filename"]
     response = response["url"]
 
-    files = {"file": (name, image)}
+    files = {"file": (filename, image)}
     requests.post(response["url"], data=response["fields"], files=files)
 
     return True
```


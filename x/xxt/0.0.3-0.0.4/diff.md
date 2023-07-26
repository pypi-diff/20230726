# Comparing `tmp/xxt-0.0.3.tar.gz` & `tmp/xxt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xxt-0.0.3.tar", last modified: Sat Jul 22 17:09:26 2023, max compression
+gzip compressed data, was "xxt-0.0.4.tar", last modified: Mon Jul 24 07:18:58 2023, max compression
```

## Comparing `xxt-0.0.3.tar` & `xxt-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 17:09:26.949814 xxt-0.0.3/
--rw-rw-rw-   0        0        0     2622 2023-07-22 17:09:26.946586 xxt-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2085 2023-07-22 17:07:39.000000 xxt-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-22 17:09:26.950791 xxt-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1050 2023-07-22 17:09:21.000000 xxt-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:09:26.914166 xxt-0.0.3/xxt/
--rw-rw-rw-   0        0        0       23 2023-07-17 09:53:32.000000 xxt-0.0.3/xxt/__init__.py
--rw-rw-rw-   0        0        0     6144 2023-07-22 16:59:22.000000 xxt-0.0.3/xxt/funcs.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:09:26.943465 xxt-0.0.3/xxt.egg-info/
--rw-rw-rw-   0        0        0     2622 2023-07-22 17:09:26.000000 xxt-0.0.3/xxt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2023-07-22 17:09:26.000000 xxt-0.0.3/xxt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 17:09:26.000000 xxt-0.0.3/xxt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-22 17:09:26.000000 xxt-0.0.3/xxt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-22 17:09:26.000000 xxt-0.0.3/xxt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 07:18:58.907750 xxt-0.0.4/
+-rw-rw-rw-   0        0        0     1446 2023-07-24 07:18:58.906772 xxt-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      752 2023-07-24 07:06:16.000000 xxt-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 07:18:58.908726 xxt-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1255 2023-07-22 19:30:54.000000 xxt-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:18:58.847687 xxt-0.0.4/xxt/
+-rw-rw-rw-   0        0        0       23 2023-07-17 09:53:32.000000 xxt-0.0.4/xxt/__init__.py
+-rw-rw-rw-   0        0        0     6877 2023-07-24 07:02:57.000000 xxt-0.0.4/xxt/funcs.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:18:58.901892 xxt-0.0.4/xxt.egg-info/
+-rw-rw-rw-   0        0        0     1446 2023-07-24 07:18:58.000000 xxt-0.0.4/xxt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2023-07-24 07:18:58.000000 xxt-0.0.4/xxt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 07:18:58.000000 xxt-0.0.4/xxt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-24 07:18:58.000000 xxt-0.0.4/xxt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-24 07:18:58.000000 xxt-0.0.4/xxt.egg-info/top_level.txt
```

### Comparing `xxt-0.0.3/xxt/funcs.py` & `xxt-0.0.4/xxt/funcs.py`

 * *Files 12% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 {traits_str}"""
 
 class Chatbot:
     def ___init__(self, name, description, key):
         "Class for a chatbot. Uses openai's API, so it needs a key. Description is the chatbot's description, do not include the chatbot's name."
         self.name = name
         self.description = description
-        self.key = key
+        openai.api_key = key
         self.messages = []
         self.messages.append({"role":"system","content": f"You are {name}. {description}"})
 
     def chat(self, message):
         "Chat with the chatbot"
         self.messages.append({"role":"user","content": message})
         response = openai.ChatCompletion.create(
@@ -149,14 +149,33 @@
         return reply
     
     def clear(self):
         "Clears the chat"
         self.messages = []
         self.messages.append({"role":"system","content": self.description})
 
+class Imagebot:
+    def __init__(self, key):
+        "Class for an imagebot. Uses openai's API, so it needs a key."
+        openai.api_key = key
+
+    def generate(self, prompt, width, height):
+        """Generates an image from a prompt
+        The width of the image. Must be 256, 512, or 1024.
+        The height of the image. Must be 256, 512, or 1024."""
+        if width not in [256, 512, 1024] or height not in [256, 512, 1024]:
+            return "Invalid width or height. Width and height must be 256, 512, or 1024."
+        response = openai.Image.create(
+            prompt=prompt,
+            n=1,
+            size = f"{width}x{height}"
+        )
+        return f"""View at:
+{response["url"]}"""
+
 class Random:
     def __init__(self):
         pass
     
     def integer(self, min, max):
         "Returns a random integer between min and max"
         return random.randint(min, max)
```


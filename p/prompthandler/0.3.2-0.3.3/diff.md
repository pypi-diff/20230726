# Comparing `tmp/prompthandler-0.3.2.tar.gz` & `tmp/prompthandler-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompthandler-0.3.2.tar", last modified: Tue Jul 25 16:06:08 2023, max compression
+gzip compressed data, was "prompthandler-0.3.3.tar", last modified: Wed Jul 26 14:43:25 2023, max compression
```

## Comparing `prompthandler-0.3.2.tar` & `prompthandler-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:06:08.507188 prompthandler-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-25 16:05:54.000000 prompthandler-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-07-25 16:06:08.503188 prompthandler-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-25 16:05:54.000000 prompthandler-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:06:08.503188 prompthandler-0.3.2/prompthandler/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-25 16:05:54.000000 prompthandler-0.3.2/prompthandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-25 16:05:54.000000 prompthandler-0.3.2/prompthandler/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-25 16:05:54.000000 prompthandler-0.3.2/prompthandler/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:06:08.503188 prompthandler-0.3.2/prompthandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-07-25 16:06:08.000000 prompthandler-0.3.2/prompthandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 16:06:08.000000 prompthandler-0.3.2/prompthandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:06:08.000000 prompthandler-0.3.2/prompthandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 16:06:08.000000 prompthandler-0.3.2/prompthandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 16:06:08.000000 prompthandler-0.3.2/prompthandler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 16:06:08.507188 prompthandler-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-25 16:05:54.000000 prompthandler-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:43:25.859355 prompthandler-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-26 14:43:15.000000 prompthandler-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-07-26 14:43:25.859355 prompthandler-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-26 14:43:15.000000 prompthandler-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:43:25.855355 prompthandler-0.3.3/prompthandler/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 14:43:15.000000 prompthandler-0.3.3/prompthandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-26 14:43:15.000000 prompthandler-0.3.3/prompthandler/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-07-26 14:43:15.000000 prompthandler-0.3.3/prompthandler/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:43:25.859355 prompthandler-0.3.3/prompthandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-07-26 14:43:25.000000 prompthandler-0.3.3/prompthandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-26 14:43:25.000000 prompthandler-0.3.3/prompthandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:43:25.000000 prompthandler-0.3.3/prompthandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 14:43:25.000000 prompthandler-0.3.3/prompthandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 14:43:25.000000 prompthandler-0.3.3/prompthandler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:43:25.859355 prompthandler-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-26 14:43:15.000000 prompthandler-0.3.3/setup.py
```

### Comparing `prompthandler-0.3.2/LICENSE` & `prompthandler-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prompthandler-0.3.2/PKG-INFO` & `prompthandler-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompthandler
-Version: 0.3.2
+Version: 0.3.3
 Summary: Token Management system for chatgpt and more. Keeps your prompt under token with summary support
 Author: prasannan-robots
 License: MIT License
         
         Copyright (c) 2023 Prasanna
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,14 +47,15 @@
 from prompthandler import Prompthandler
 model = Prompthandler()
 model.add_system("You are now user's girlfriend so take care of him",to_head=True) # Makes this to go on to the head. Head is not rolled so it stays the same
 model.add_user("Hi")
 model.chat() # you can chat with it in terminal
 ```
 For more examples see [examples.ipynb](https://github.com/prasannan-robots/Prompt-handler/blob/main/examples.ipynb)
+Example Projects [my silicon version](https://prasannanrobots.pythonanywhere.com/) [github_repo](https://github.com/prasannan-robots/prasannan-robots.github.io)
 ## Behind the scenes
 
 ### models.py
 
 #### `openai_chat_gpt` class
 
 This class represents the interaction with the GPT-3.5-turbo model (or other OpenAI models). It provides methods for generating completions for given messages and managing the conversation history.
```

### Comparing `prompthandler-0.3.2/README.md` & `prompthandler-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from prompthandler import Prompthandler
 model = Prompthandler()
 model.add_system("You are now user's girlfriend so take care of him",to_head=True) # Makes this to go on to the head. Head is not rolled so it stays the same
 model.add_user("Hi")
 model.chat() # you can chat with it in terminal
 ```
 For more examples see [examples.ipynb](https://github.com/prasannan-robots/Prompt-handler/blob/main/examples.ipynb)
+Example Projects [my silicon version](https://prasannanrobots.pythonanywhere.com/) [github_repo](https://github.com/prasannan-robots/prasannan-robots.github.io)
 ## Behind the scenes
 
 ### models.py
 
 #### `openai_chat_gpt` class
 
 This class represents the interaction with the GPT-3.5-turbo model (or other OpenAI models). It provides methods for generating completions for given messages and managing the conversation history.
```

### Comparing `prompthandler-0.3.2/prompthandler/models.py` & `prompthandler-0.3.3/prompthandler/models.py`

 * *Files identical despite different names*

### Comparing `prompthandler-0.3.2/prompthandler/prompts.py` & `prompthandler-0.3.3/prompthandler/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,23 +28,22 @@
             super().__init__(MAX_TOKEN=MAX_TOKEN, api_key=api_key, temperature=temperature, model=model)
         self.update()
     def dump(self):
         """
         Get a dict of head,body and messages
         """
         self.update_messages()
-        return {'head':self.headers,'body':self.body,'messages':self.messages}
+        return {'head':self.headers,'body':self.body}
         
     def load(self,dictionary):
         """
         Load the data from the dictionary
         """
         self.headers = dictionary['head']
         self.body = dictionary['body']
-        self.messages = dictionary['messages']
         self.update()
 
     def get_completion(self, message='', update_history=True, temperature=None):
         """
         Generates a completion for the conversation history.
 
         Args:
```

### Comparing `prompthandler-0.3.2/prompthandler.egg-info/PKG-INFO` & `prompthandler-0.3.3/prompthandler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompthandler
-Version: 0.3.2
+Version: 0.3.3
 Summary: Token Management system for chatgpt and more. Keeps your prompt under token with summary support
 Author: prasannan-robots
 License: MIT License
         
         Copyright (c) 2023 Prasanna
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,14 +47,15 @@
 from prompthandler import Prompthandler
 model = Prompthandler()
 model.add_system("You are now user's girlfriend so take care of him",to_head=True) # Makes this to go on to the head. Head is not rolled so it stays the same
 model.add_user("Hi")
 model.chat() # you can chat with it in terminal
 ```
 For more examples see [examples.ipynb](https://github.com/prasannan-robots/Prompt-handler/blob/main/examples.ipynb)
+Example Projects [my silicon version](https://prasannanrobots.pythonanywhere.com/) [github_repo](https://github.com/prasannan-robots/prasannan-robots.github.io)
 ## Behind the scenes
 
 ### models.py
 
 #### `openai_chat_gpt` class
 
 This class represents the interaction with the GPT-3.5-turbo model (or other OpenAI models). It provides methods for generating completions for given messages and managing the conversation history.
```

### Comparing `prompthandler-0.3.2/setup.py` & `prompthandler-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 with open("README.md", "r") as fh:
     long_description = fh.read()
 with open("LICENSE", "r") as fg:
     license_val = fg.read()
 setup(
     name="prompthandler",
-    version="0.3.2",
+    version="0.3.3",
     author="prasannan-robots",
     description="Token Management system for chatgpt and more. Keeps your prompt under token with summary support",
     install_requires=["openai","tiktoken"],
     packages=['prompthandler'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```


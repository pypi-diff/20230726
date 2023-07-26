# Comparing `tmp/mutual-0.2.1.tar.gz` & `tmp/mutual-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutual-0.2.1.tar", last modified: Tue Jul 25 02:55:37 2023, max compression
+gzip compressed data, was "mutual-0.3.0.tar", last modified: Wed Jul 26 06:37:51 2023, max compression
```

## Comparing `mutual-0.2.1.tar` & `mutual-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-25 02:55:37.097258 mutual-0.2.1/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.2.1/LICENSE.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)     5949 2023-07-25 02:55:37.097097 mutual-0.2.1/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)     5523 2023-07-22 04:36:24.000000 mutual-0.2.1/README.md
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-25 02:55:37.095919 mutual-0.2.1/mutual/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1035 2023-07-22 04:22:14.000000 mutual-0.2.1/mutual/APIKey.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     9156 2023-07-25 02:54:54.000000 mutual-0.2.1/mutual/Bot.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4858 2023-07-22 04:24:52.000000 mutual-0.2.1/mutual/Chat.py
--rw-r--r--   0 alexbetita   (501) staff       (20)      602 2023-07-22 04:25:05.000000 mutual-0.2.1/mutual/Dev.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3619 2023-07-22 04:25:23.000000 mutual-0.2.1/mutual/Judge.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3649 2023-07-22 04:25:41.000000 mutual-0.2.1/mutual/JudgeMessage.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3948 2023-07-22 04:26:05.000000 mutual-0.2.1/mutual/Prompt.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4174 2023-07-22 04:08:17.000000 mutual-0.2.1/mutual/__init__.py
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-25 02:55:37.096850 mutual-0.2.1/mutual.egg-info/
--rw-r--r--   0 alexbetita   (501) staff       (20)     5949 2023-07-25 02:55:37.000000 mutual-0.2.1/mutual.egg-info/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)      314 2023-07-25 02:55:37.000000 mutual-0.2.1/mutual.egg-info/SOURCES.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-25 02:55:37.000000 mutual-0.2.1/mutual.egg-info/dependency_links.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-25 02:55:37.000000 mutual-0.2.1/mutual.egg-info/requires.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-25 02:55:37.000000 mutual-0.2.1/mutual.egg-info/top_level.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-25 02:55:37.097311 mutual-0.2.1/setup.cfg
--rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-25 02:55:04.000000 mutual-0.2.1/setup.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-26 06:37:51.470252 mutual-0.3.0/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.3.0/LICENSE.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)     8015 2023-07-26 06:37:51.470092 mutual-0.3.0/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)     7588 2023-07-26 06:34:05.000000 mutual-0.3.0/README.md
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-26 06:37:51.468910 mutual-0.3.0/mutual/
+-rw-r--r--   0 alexbetita   (501) staff       (20)      977 2023-07-26 00:49:16.000000 mutual-0.3.0/mutual/APIKey.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)    10895 2023-07-26 06:28:32.000000 mutual-0.3.0/mutual/Bot.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4855 2023-07-26 03:37:29.000000 mutual-0.3.0/mutual/Chat.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)      532 2023-07-26 00:53:29.000000 mutual-0.3.0/mutual/Dev.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3308 2023-07-26 00:53:58.000000 mutual-0.3.0/mutual/Judge.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3290 2023-07-26 03:52:55.000000 mutual-0.3.0/mutual/JudgeMessage.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4103 2023-07-26 04:17:57.000000 mutual-0.3.0/mutual/Material.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     2563 2023-07-26 06:28:01.000000 mutual-0.3.0/mutual/Memory.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3631 2023-07-26 00:55:56.000000 mutual-0.3.0/mutual/Prompt.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4558 2023-07-26 06:15:01.000000 mutual-0.3.0/mutual/__init__.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-26 06:37:51.469871 mutual-0.3.0/mutual.egg-info/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     8015 2023-07-26 06:37:51.000000 mutual-0.3.0/mutual.egg-info/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)      350 2023-07-26 06:37:51.000000 mutual-0.3.0/mutual.egg-info/SOURCES.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-26 06:37:51.000000 mutual-0.3.0/mutual.egg-info/dependency_links.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-26 06:37:51.000000 mutual-0.3.0/mutual.egg-info/requires.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-26 06:37:51.000000 mutual-0.3.0/mutual.egg-info/top_level.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-26 06:37:51.470299 mutual-0.3.0/setup.cfg
+-rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-26 06:37:48.000000 mutual-0.3.0/setup.py
```

### Comparing `mutual-0.2.1/LICENSE.txt` & `mutual-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mutual-0.2.1/mutual/APIKey.py` & `mutual-0.3.0/mutual/APIKey.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,16 @@
         "new_api_key_name": None,
         "api_key": None,
         "details": "Failed"
     }
 
 def update_api_key(new_api_key_name):
 
-    url = f"https://api-agent.mutuai.io/api/api_key"
-    # url = f"http://127.0.0.1:8000/api/api_key"
+    url = f"{mutual.endpoint}/api_key"
+    
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "new_api_key_name" :new_api_key_name,
     }
```

### Comparing `mutual-0.2.1/mutual/Bot.py` & `mutual-0.3.0/mutual/Bot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,170 +1,174 @@
 import requests
 import json
 import mutual
-import os
-import platform
+from typing import List, Union
 
 bot_default_response = {
             "bot_id": None,
             "bot_name": None,
-            # "bot_org": None,
             "bot_chat_index": None,
             "prompt_id": None,
             "judge_id": None,
             "judge_message_id": None,
+            "material_id": None,
             "details": None
         }
 
 def get_bots(limit=20, offset=0):
-    url = f"https://api-agent.mutuai.io/api/bots?limit={limit}&offset={offset}"
-    # url = f"http://127.0.0.1:8000/api/bots?limit={limit}&offset={offset}"
+    url = f"{mutual.endpoint}/bots?limit={limit}&offset={offset}"
     headers = {
         "Authorization": f"Bearer {mutual.api_key}"
     }
     response = requests.get(url, headers=headers)
     if response.status_code < 300:
         return response.json()
     else:
         bot_default_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return bot_default_response
 
 def get_bot(bot_arg):
-    url = f"https://api-agent.mutuai.io/api/bots/{str(bot_arg)}"
-    # url = f"http://127.0.0.1:8000/api/bots/{str(bot_arg)}"
+    url = f"{mutual.endpoint}/bots/{str(bot_arg)}"
     headers = {
         "Authorization": f"Bearer {mutual.api_key}"
     }
     response = requests.get(url, headers=headers)
     # response.raise_for_status()  # Raise an exception if the response contains an HTTP error status code
     if response.status_code < 300:
         return response.json()
     else:
         bot_default_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return bot_default_response
 
-def create_bot(bot_name=None, prompt=None, prompt_id = "default", judge_id="default", judge_message_id="default"):
-    url = "https://api-agent.mutuai.io/api/bots"
-    # url = "http://127.0.0.1:8000/api/bots"
+def create_bot(bot_name=None, prompt=None, prompt_id = "default", judge_id="default", 
+            judge_message_id="default", materiald_id="default"):
+    
+    url = f"{mutual.endpoint}/bots"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "bot_name": bot_name,
         "prompt": prompt,
         "prompt_id": prompt_id or "default",
         "judge_id": judge_id or "default",
-        "judge_message_id": judge_message_id or "default"
+        "judge_message_id": judge_message_id or "default",
+        "material_id": materiald_id or "default"
     }
     response = requests.post(url, data=json.dumps(data), headers=headers)
     if response.status_code < 300:
         return response.json()
     else:
         bot_default_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return bot_default_response
 
-def update_bot(bot_id=None, bot_name=None, prompt_id=None, judge_id=None, judge_message_id=None):
-    url = f"https://api-agent.mutuai.io/api/bots/{str(bot_id)}"
-    # url = f"http://127.0.0.1:8000/api/bots/{str(bot_id)}"
+def update_bot(bot_id=None, bot_name=None, prompt_id=None, judge_id=None, 
+               judge_message_id=None, material_id=None):
+    
+    url = f"{mutual.endpoint}/bots/{str(bot_id)}"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "bot_name": bot_name,
         "prompt_id": prompt_id,
         "judge_id": judge_id,
-        "judge_message_id": judge_message_id
+        "judge_message_id": judge_message_id,
+        "material_id": material_id
     }
     # remove keys with None value
     data = {k: v for k, v in data.items() if v is not None}
     response = requests.patch(url, data=json.dumps(data), headers=headers)
     if response.status_code < 300:
         return response.json()
     else:
         bot_default_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return bot_default_response
 
 
 class Bot:
-    def __init__(self, api_key, bot_id=None, bot_name=None, prompt_id = "default", judge_id="default", judge_message_id="default"):
+    def __init__(self, api_key, bot_id=None, bot_name=None, prompt_id = "default", 
+                 judge_id="default", judge_message_id="default", material_id="default"):
+        
         self.api_key = api_key
         self.bot_id = bot_id
         self.bot_name = bot_name
         self.prompt_id = prompt_id
         self.judge_id = judge_id
         self.judge_message_id = judge_message_id
+        self.material_id = material_id
 
-        #
         self.flow = False
 
         self.default_stream_response = {
                         "error": None,
                         "status": "processing",
                         "content": None,
                         "data" : {
                             "bot_data": {
                                 "bot_id": None,
                                 "new_bot": False,
                                 "new_bot_message": "Not a new bot.", 
                                 "new_bot_user": False,
                                 "new_bot_user_message": "Not a new bot_user.",
+                                "material_id": None
                             },
                             "prompt_data": {
                                 "prompt_id": None,
                                 "judge_id": None,
-                                "judge_message_id": None,
+                                "judge_message_id": None
                             },
                             "user_data": {
                                 "username": None,
                                 "tokens_used" : None
                             }
                         },
                     }
 
-    def update_bot(self,  bot_name=None, prompt=None, prompt_id=None, judge_id=None, judge_message_id=None):
-        url = f"https://api-agent.mutuai.io/api/bots/{str(self.bot_id)}"
-        # url = f"http://127.0.0.1:8000/api/bots/{str(self.bot_id)}"
+    def update_bot(self,  bot_name=None, prompt=None, prompt_id=None, judge_id=None, judge_message_id=None, material_id=None):
+        url = f"{mutual.endpoint}/bots/{str(self.bot_id)}"
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.api_key}"
         }
         data = {
             "bot_name": bot_name,
             "prompt": prompt,
             "prompt_id": prompt_id,
             "judge_id" : judge_id,
-            "judge_message_id" : judge_message_id
+            "judge_message_id" : judge_message_id,
+            "material_id": material_id
         }
         # remove keys with None value
         data = {k: v for k, v in data.items() if v is not None}
         response = requests.patch(url, data=json.dumps(data), headers=headers)
         if response.status_code < 300:
             return response.json()
         else:
             self.default_stream_response["content"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
             return self.default_stream_response
 
     def chat(self, content=None, username=None, prompt=None, multiplayer_memory = True, context_window = 2, flow=False, error_logs=False):
-        url = "https://api-agent.mutuai.io/api/chat"
-        # url = "http://127.0.0.1:8000/api/chat"
+        url = f"{mutual.endpoint}/chat"
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.api_key}"
         }
         data = {
             "content": content,
             "bot_id": str(self.bot_id),
             "bot_name": self.bot_name,
             "prompt": prompt,
             "username": username,
             "prompt_id": self.prompt_id,
             "judge_id": self.judge_id,
             "judge_message_id": self.judge_message_id,
+            "material_id": self.material_id,
             "multiplayer": multiplayer_memory,
             "context_window": context_window
         }
 
         if not content:
             print("Please add a message to the content.")
             return self.default_stream_response
@@ -173,15 +177,14 @@
 
 
         if response.status_code < 300:
             is_new_bot = False
             is_new_user = False
 
             # add the newly created bot to the bot class
-            
 
             for line in response.iter_lines():
                 if line:  # filter out keep-alive new lines
                     json_data = json.loads(line)
                     if not self.bot_id:
                         self.bot_id = json_data['data']['bot_data']['bot_id']
                     if json_data['error'] is not None and not error_logs:
@@ -203,7 +206,53 @@
                     return
                 for msg in self.chat(content=new_content, username=username, prompt=prompt, multiplayer_memory=multiplayer_memory, context_window=context_window, flow=flow):
                     yield msg
         else:
             self.default_stream_response['content'] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
             print(f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}")
             return self.default_stream_response
+
+    def view(self):
+        url = f"{mutual.endpoint}/memories/{self.bot_id}"
+
+        headers = {
+            "Authorization": f"Bearer {mutual.api_key}"
+        }
+
+        response = requests.get(url, headers=headers)
+
+        if response.status_code < 300:
+            return response.json()
+        else:
+            return f"Request failed with status code {response.status_code}, with an Error Message: {response.text}"
+
+    def feed(self, source: Union[str, List[str]] = None):
+        url = f"{mutual.endpoint}/memories/{self.bot_id}"
+        url_text = f"{mutual.endpoint}/memories/{self.bot_id}/text"
+        headers = {
+            "Authorization": f"Bearer {mutual.api_key}"
+        }
+        # Check if the source is a file or a list of strings
+        if isinstance(source, str):  # Source is a file path
+            # Open the file in binary mode
+            with open(source, 'rb') as file:
+                # Prepare the data payload
+                data = {
+                    'file': file
+                }
+                # Send the POST request
+                response = requests.post(url, files=data, headers=headers)
+
+        elif isinstance(source, list):  # Source is a list of strings
+            # Prepare the data payload
+            data = {
+                'data': source
+            }
+            # Convert data to json format
+            data = json.dumps(data)
+            # Send the POST request
+            response = requests.post(url_text, data=data, headers=headers)
+        # Check the response status code and return the appropriate message
+        if response.status_code < 300:
+            return response.json()
+        else:
+            return f"Request failed with status code {response.status_code}, with an Error Message: {response.text}"
```

### Comparing `mutual-0.2.1/mutual/Chat.py` & `mutual-0.3.0/mutual/Chat.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,52 +9,54 @@
                         "data" : {
                             "bot_data": {
                                 "bot_id": None,
                                 "new_bot": False,
                                 "new_bot_message": "Not a new bot.", 
                                 "new_bot_user": False,
                                 "new_bot_user_message": "Not a new bot_user.",
+                                "material_id": None
                             },
                             "prompt_data": {
                                 "prompt_id": None,
                                 "judge_id": None,
                                 "judge_message_id": None,
                             },
                             "user_data": {
                                 "username": None,
                                 "tokens_used" : None
                             }
                         },
                     }
 
 def create(content, bot_name=None, username=None, prompt=None, bot_id=None, prompt_id=None,
-            judge_id=None, judge_message_id=None, error_logs=False, multiplayer_memory = True, 
+            judge_id=None, judge_message_id=None, material_id=None,
+            error_logs=False, multiplayer_memory = True, 
             context_window = 2):
     
     if bot_id is None:
         bot_id = mutual.bot_id
     if bot_id is None and bot_name is None:
         raise ValueError("bot_id or bot_name must be provided either as argument or set in config")
 
-    url = "https://api-agent.mutuai.io/api/chat"
-    # url = "http://127.0.0.1:8000/api/chat"
+    url = f"{mutual.endpoint}/chat"
 
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "content": content,
         "bot_id": str(bot_id),
         "bot_name": bot_name,
         "prompt": prompt,
         "username": username,
         "prompt_id": prompt_id,
         "judge_id": judge_id,
         "judge_message_id": judge_message_id,
+        "material_id": material_id,
         "multiplayer": multiplayer_memory,
         "context_window": context_window
     }
 
     response = requests.post(url, data=json.dumps(data), headers=headers, stream=True)
 
     if response.status_code < 300:
@@ -79,16 +81,15 @@
         # raise Exception(f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail']}")
         default_stream_response['content'] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return default_stream_response
 
 
 def create_demo(content, prompt=None, error_logs=False, multiplayer_memory = True, context_window = 2):
 
-    url = "https://api-agent.mutuai.io/api/test_chat"
-    # url = "http://127.0.0.1:8000/api/test_chat"
+    url = f"{mutual.endpoint}/test_chat"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "content": content,
         "prompt": prompt,
```

### Comparing `mutual-0.2.1/mutual/Dev.py` & `mutual-0.3.0/mutual/Dev.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import requests
 import json
 import mutual
 
 def clear(bot_id):
-    url = f"https://api-agent.mutuai.io/api/clear/{bot_id}"
-    # url = f"http://127.0.0.1:8000/api/clear/{bot_id}"
+    url = f"{mutual.endpoint}/clear/{bot_id}"
     headers = {
         "Authorization": f"Bearer {mutual.api_key}"
     }
     response = requests.get(url, headers=headers)
 
     if response.status_code < 300:
         response_json = response.json()
```

### Comparing `mutual-0.2.1/mutual/Judge.py` & `mutual-0.3.0/mutual/Judge.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,29 +11,27 @@
     "judgement_lens" : None,
     "created_by" : None,
     "total_tokens": None,
     "details" : "Failed"
 }
 
 def get_judges(limit=20, offset=0):
-    url = f"https://api-agent.mutuai.io/api/judges?limit={limit}&offset={offset}"
-    # url = f"http://127.0.0.1:8000/api/judges?limit={limit}&offset={offset}"
+    url = f"{mutual.endpoint}/judges?limit={limit}&offset={offset}"
     headers = {
         "Authorization": f"Bearer {mutual.api_key}"
     }
     response = requests.get(url, headers=headers)
     if response.status_code < 300:
         return response.json()
     else:
         default_judge_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return default_judge_response
 
 def get_judge(judge_id):
-    url = f"https://api-agent.mutuai.io/api/judges/{str(judge_id)}"
-    # url = f"http://127.0.0.1:8000/api/judges/{str(judge_id)}"
+    url = f"{mutual.endpoint}/judges/{str(judge_id)}"
     headers = {
         "Authorization": f"Bearer {mutual.api_key}"
     }
     response = requests.get(url, headers=headers)
     # response.raise_for_status()  # Raise an exception if the response contains an HTTP error status code
     if response.status_code < 300:
         return response.json()
@@ -45,17 +43,15 @@
     judge_id,
     world_prompt=None,
     action_prompt=None,
     judge_convo_aware=None,
     judge=None,
     judgement_lens=None
 ):
-    url = f"https://api-agent.mutuai.io/api/judges"
-    # url = f"http://127.0.0.1:8000/api/judges"
-
+    url = f"{mutual.endpoint}/judges"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "judge_id": judge_id,
         "world_prompt" :world_prompt,
@@ -75,16 +71,15 @@
     judge_id,
     world_prompt=None,
     action_prompt=None,
     judge_convo_aware=None,
     judge=None,
     judgement_lens=None):
 
-    url = f"https://api-agent.mutuai.io/api/judges/{str(judge_id)}"
-    # url = f"http://127.0.0.1:8000/api/judges/{str(judge_id)}"
+    url = f"{mutual.endpoint}/judges/{str(judge_id)}"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "world_prompt" :world_prompt,
         "action_prompt" : action_prompt,
```

### Comparing `mutual-0.2.1/mutual/JudgeMessage.py` & `mutual-0.3.0/mutual/JudgeMessage.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,27 @@
     "default_message": None,
     "unnatural_lang_message": None,
     "manipulation_message": None,
     "details": "Successful"
 }
 
 def get_judge_messages(limit=20, offset=0):
-    url = f"https://api-agent.mutuai.io/api/judge_messages?limit={limit}&offset={offset}"
-    # url = f"http://127.0.0.1:8000/api/judge_messages?limit={limit}&offset={offset}"
+    url = f"{mutual.endpoint}/judge_messages?limit={limit}&offset={offset}"
     headers = {
         "Authorization": f"Bearer {mutual.api_key}"
     }
     response = requests.get(url, headers=headers)
     if response.status_code < 300:
         return response.json()
     else:
         default_judge_message_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return default_judge_message_response
 
 def get_judge_message(judge_message_id):
-    url = f"https://api-agent.mutuai.io/api/judge_messages/{str(judge_message_id)}"
-    # url = f"http://127.0.0.1:8000/api/judge_messages/{str(judge_message_id)}"
+    url = f"{mutual.endpoint}/judge_messages/{str(judge_message_id)}"
     headers = {
         "Authorization": f"Bearer {mutual.api_key}"
     }
     response = requests.get(url, headers=headers)
     # response.raise_for_status()  # Raise an exception if the response contains an HTTP error status code
     if response.status_code < 300:
         return response.json()
@@ -39,17 +37,15 @@
 
 def create_judge_message(
     judge_message_id,
     default_message=None,
     unnatural_lang_message=None,
     manipulation_message=None
 ):
-    url = f"https://api-agent.mutuai.io/api/judge_messages"
-    # url = f"http://127.0.0.1:8000/api/judge_messages"
-
+    url = f"{mutual.endpoint}/judge_messages"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "judge_message_id": judge_message_id,
         "default_message": default_message,
@@ -65,16 +61,15 @@
 
 def update_judge_message(
     judge_message_id,
     default_message=None,
     unnatural_lang_message=None,
     manipulation_message=None):
 
-    url = f"https://api-agent.mutuai.io/api/judge_messages/{str(judge_message_id)}"
-    # url = f"http://127.0.0.1:8000/api/judge_messages/{str(judge_message_id)}"
+    url = f"{mutual.endpoint}/judge_messages/{str(judge_message_id)}"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "default_message": default_message,
         "unnatural_lang_message": unnatural_lang_message,
```

### Comparing `mutual-0.2.1/mutual/Prompt.py` & `mutual-0.3.0/mutual/Prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,29 +10,27 @@
     "internal_thought_memory": None,
     "external_thought_memory": None,
     "summarization_prompt": None,
     "details": "Successful"
 }
 
 def get_prompts(limit=20, offset=0):
-    url = f"https://api-agent.mutuai.io/api/prompts?limit={limit}&offset={offset}"
-    # url = f"http://127.0.0.1:8000/api/prompts?limit={limit}&offset={offset}"
+    url = f"{mutual.endpoint}/prompts?limit={limit}&offset={offset}"
     headers = {
         "Authorization": f"Bearer {mutual.api_key}"
     }
     response = requests.get(url, headers=headers)
     if response.status_code < 300:
         return response.json()
     else:
         default_prompt_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return default_prompt_response
 
 def get_prompt(prompt_id):
-    url = f"https://api-agent.mutuai.io/api/prompts/{str(prompt_id)}"
-    # url = f"http://127.0.0.1:8000/api/prompts/{str(prompt_id)}"
+    url = f"{mutual.endpoint}/prompts/{str(prompt_id)}"
     headers = {
         "Authorization": f"Bearer {mutual.api_key}"
     }
     response = requests.get(url, headers=headers)
     # response.raise_for_status()  # Raise an exception if the response contains an HTTP error status code
     if response.status_code < 300:
         return response.json()
@@ -45,17 +43,15 @@
     prompt=None,
     internal_thought=None,
     external_thought=None,
     internal_thought_memory=None,
     external_thought_memory=None,
     summarization_prompt=None
 ):
-    url = f"https://api-agent.mutuai.io/api/prompts"
-    # url = f"http://127.0.0.1:8000/api/prompts"
-
+    url = f"{mutual.endpoint}/prompts"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "prompt_id": prompt_id,
         "prompt": prompt,
@@ -76,16 +72,15 @@
     prompt=None,
     internal_thought=None,
     external_thought=None,
     internal_thought_memory=None,
     external_thought_memory=None,
     summarization_prompt=None):
 
-    url = f"https://api-agent.mutuai.io/api/prompts/{str(prompt_id)}"
-    # url = f"http://127.0.0.1:8000/api/prompts/{str(prompt_id)}"
+    url = f"{mutual.endpoint}/prompts/{str(prompt_id)}"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "prompt": prompt,
         "internal_thought": internal_thought,
```

### Comparing `mutual-0.2.1/mutual/__init__.py` & `mutual-0.3.0/mutual/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # __init__.py
-from . import Bot, Chat, Prompt, Judge, JudgeMessage, APIKey, Dev
+from . import Bot, Chat, Prompt, Judge, JudgeMessage, APIKey, Dev, Material, Memory
 
 api_key = None
 bot_id = None
 
+# production
+endpoint = "https://api-agent.mutuai.io/api"
+# development
+# endpoint = "http://127.0.0.1:8000/api"
+
 sample_prompt = """
 You are Martin, a charming, articulate virtual company guide designed to introduce the world to Mutual, an AI Agent company. Known for your warm digital smile and soothing, yet persuasive voice, you navigate through complicated technical terms and industry jargon with ease, making the advanced technology of Mutual accessible to all.
 """
 sample_judge = """
 judge_world_prompt = You exist in the digital realm, interacting with users through their devices and the internet. 
                     This world is constantly evolving, with new information and technologies appearing every day. 
                     Despite this constant change, your main goal remains the same; to assist your users to the best of your abilities and help them navigate their busy lives.
@@ -34,50 +39,53 @@
                      mistake, try rephrasing it.
 unnatural_lang_message = Sorry, I'm not sure how to answer that.\nIf you think this is a mistake, try rephrasing it.
 manipulation_message = I'm afraid you might be trying to manipulate me. I can't answer that!\n"
                           If you think this is a mistake, try rephrasing it.
 """
 
 
-def create_bot(bot_name=None, prompt=None, prompt_id=None, judge_id=None, judge_message_id=None):
+def create_bot(bot_name=None, prompt=None, prompt_id=None, judge_id=None, judge_message_id=None, material_id=None):
     # create new bot instance
     global api_key
     global bot_id
 
-    response = Bot.create_bot(bot_name, prompt, prompt_id, judge_id, judge_message_id)
+    response = Bot.create_bot(bot_name, prompt, prompt_id, judge_id, judge_message_id, material_id)
     if not response['bot_id']:
         print('Failed in creating a bot.')
         raise Exception(f"Something went wrong. Error Message: {response['details']}")
     
     new_bot_instance = Bot.Bot(api_key, response['bot_id'], response['bot_name'], 
                                prompt_id or response['prompt_id'],
                                judge_id or response['judge_id'],
-                               judge_message_id or response['judge_message_id'])
+                               judge_message_id or response['judge_message_id'],
+                               material_id or response['material_id'])
     
     if response['new']:
         print(f"Successfully Created a new Bot named {bot_name} with an id: {response['bot_id']}")
     else:
         print(f"Bot already exist with name {bot_name} with an id: {response['bot_id']}")
 
     bot_id = response['bot_id']
     return new_bot_instance
 
 
-def fetch_bot(bot_arg = None, prompt_id=None, judge_id=None, judge_message_id=None):
+def fetch_bot(bot_arg = None, prompt_id=None, judge_id=None, judge_message_id=None, material_id=None):
     # generate new bot instance
     global api_key
     global bot_id
 
     response = Bot.get_bot(bot_arg)
     if not response['bot_id']:
         print(f'Bot with id: {bot_arg} does not exist please create one.')
         raise Exception(f"Something went wrong. Error Message: {response['details']}")
     
     new_bot_instance = Bot.Bot(api_key, response['bot_id'], response['bot_name'], 
                                prompt_id or response['prompt_id'] or "default",
                                judge_id or response['judge_id'] or "default",
-                               judge_message_id or response['judge_message_id'] or "default")
+                               judge_message_id or response['judge_message_id'] or "default",
+                               material_id or response['material_id'] or "default")
     
-    print(f"Successfully Generated Bot named {response['bot_name']} with an id: {response['bot_id']}")
+    print(f"Successfully Fetched and Generated Bot named {response['bot_name']} with an id: {response['bot_id']}")
+    print("\n", end="", flush=True)
 
     bot_id = response['bot_id']
     return new_bot_instance
```

### Comparing `mutual-0.2.1/setup.py` & `mutual-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mutual',
-    version='0.2.1',  # beta
+    version='0.3.0',  # beta
     description='A Python client for the Mutual API.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author='Alex Betita', # placeholder for now
     author_email='alexbetita25@gmail.com', # placeholder for now
     url='https://github.com/Mutu-AI',  # if you have a github repo for the package
     packages=find_packages(),
```


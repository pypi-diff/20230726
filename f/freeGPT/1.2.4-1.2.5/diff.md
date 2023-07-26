# Comparing `tmp/freeGPT-1.2.4.tar.gz` & `tmp/freeGPT-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeGPT-1.2.4.tar", last modified: Sun Jul 16 18:28:51 2023, max compression
+gzip compressed data, was "freeGPT-1.2.5.tar", last modified: Wed Jul 26 20:12:54 2023, max compression
```

## Comparing `freeGPT-1.2.4.tar` & `freeGPT-1.2.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 18:28:51.103456 freeGPT-1.2.4/
--rw-rw-rw-   0        0        0    18092 2023-07-16 18:28:26.000000 freeGPT-1.2.4/LICENSE
--rw-rw-rw-   0        0        0     4173 2023-07-16 18:28:51.102469 freeGPT-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     2868 2023-07-16 18:28:26.000000 freeGPT-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 18:28:51.088457 freeGPT-1.2.4/freeGPT/
--rw-rw-rw-   0        0        0      136 2023-07-16 18:28:26.000000 freeGPT-1.2.4/freeGPT/__init__.py
--rw-rw-rw-   0        0        0     1900 2023-07-16 18:28:27.000000 freeGPT-1.2.4/freeGPT/alpaca_7b.py
--rw-rw-rw-   0        0        0     2087 2023-07-16 18:28:27.000000 freeGPT-1.2.4/freeGPT/gpt3.py
--rw-rw-rw-   0        0        0     4647 2023-07-16 18:28:27.000000 freeGPT-1.2.4/freeGPT/gpt4.py
--rw-rw-rw-   0        0        0     3299 2023-07-16 18:28:27.000000 freeGPT-1.2.4/freeGPT/prodia.py
-drwxrwxrwx   0        0        0        0 2023-07-16 18:28:51.101466 freeGPT-1.2.4/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     4173 2023-07-16 18:28:51.000000 freeGPT-1.2.4/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-07-16 18:28:51.000000 freeGPT-1.2.4/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 18:28:51.000000 freeGPT-1.2.4/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-16 18:28:51.000000 freeGPT-1.2.4/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-16 18:28:51.000000 freeGPT-1.2.4/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 18:28:51.104456 freeGPT-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1670 2023-07-16 18:28:26.000000 freeGPT-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:12:54.009432 freeGPT-1.2.5/
+-rw-rw-rw-   0        0        0    18092 2023-07-26 19:50:03.000000 freeGPT-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0     4463 2023-07-26 20:12:54.002432 freeGPT-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3154 2023-07-26 19:50:03.000000 freeGPT-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 20:12:53.981433 freeGPT-1.2.5/freeGPT/
+-rw-rw-rw-   0        0        0      164 2023-07-26 19:50:03.000000 freeGPT-1.2.5/freeGPT/__init__.py
+-rw-rw-rw-   0        0        0     1968 2023-07-26 19:50:03.000000 freeGPT-1.2.5/freeGPT/alpaca_7b.py
+-rw-rw-rw-   0        0        0     2697 2023-07-26 19:50:03.000000 freeGPT-1.2.5/freeGPT/gpt3.py
+-rw-rw-rw-   0        0        0     4715 2023-07-26 19:50:03.000000 freeGPT-1.2.5/freeGPT/gpt4.py
+-rw-rw-rw-   0        0        0      614 2023-07-26 19:50:03.000000 freeGPT-1.2.5/freeGPT/pollinations.py
+-rw-rw-rw-   0        0        0     3351 2023-07-26 19:50:03.000000 freeGPT-1.2.5/freeGPT/prodia.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:12:53.999431 freeGPT-1.2.5/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     4463 2023-07-26 20:12:53.000000 freeGPT-1.2.5/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-07-26 20:12:53.000000 freeGPT-1.2.5/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 20:12:53.000000 freeGPT-1.2.5/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 20:12:53.000000 freeGPT-1.2.5/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-26 20:12:53.000000 freeGPT-1.2.5/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 20:12:54.009432 freeGPT-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1663 2023-07-26 19:50:03.000000 freeGPT-1.2.5/setup.py
```

### Comparing `freeGPT-1.2.4/LICENSE` & `freeGPT-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.2.4/PKG-INFO` & `freeGPT-1.2.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.2.4
+Version: 1.2.5
 Summary: freeGPT provides free access to GPT3, GPT4 and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv2
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Discord, https://discord.gg/XH6pUGkwRr
 Keywords: artificial-intelligence,machine-learning,deep-learning,gpt4free,gpt4all,chatbot,freegpt,chatgpt,python,openai,llama,free,gpt,ai
@@ -20,40 +20,43 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+#### Sorry, The freeGPT bot is in 100 servers and I can't verify it ATM. Please join my [Discord server](https://discord.gg/XH6pUGkwRr) if you wish to use it.
+
 [![PyPI](https://img.shields.io/pypi/v/freeGPT)](https://pypi.org/project/freeGPT)
 [![Downloads](https://static.pepy.tech/badge/freeGPT)](https://pypi.org/project/freeGPT)
 [![Status](https://img.shields.io/pypi/status/freeGPT)](https://pypi.org/project/freeGPT)
 
 # freeGPT
 
 freeGPT provides free access to GPT3, GPT4 and more models.
 
 ## Get started:
 
 ```
-python -m pip install --upgrade freeGPT
+python -m pip install -U freeGPT
 ```
 
 **Or add the [freeGPT Discord bot](https://dsc.gg/freegpt), it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot)!**
 
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Source:
 
-| Models   | Websites                                                |
-| -------- | ------------------------------------------------------- |
-| gpt3     | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
-| gpt4     | [<you.com>](https://you.com/)                           |
-| alpaca_7b| [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
-| prodia   | [<prodia.com>](https://prodia.com/)                     |
+| Models       | Websites                                                |
+| ------------ | ------------------------------------------------------- |
+| gpt3         | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
+| gpt4         | [<you.com>](https://you.com/)                           |
+| alpaca_7b    | [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
+| prodia       | [<prodia.com>](https://prodia.com/)                     |
+| pollinations | [<pollinations.ai>](https://pollinations.ai/)           |
 
 
 ## Support this repository:
 
 - Star this repository :D
 - Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
 - Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
@@ -78,47 +81,48 @@
 - And lastly, it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot).
 
 ## Example:
 
 **Text Completion:**
 ```python
 import freeGPT
-import asyncio
+from asyncio import run
 
 
 async def main():
     while True:
         prompt = input("👦: ")
         try:
             resp = await getattr(freeGPT, "MODEL NAME").Completion.create(prompt)
             print(f"🤖: {resp}")
         except Exception as e:
             print(f"🤖: {e}")
 
 
-asyncio.run(main())
+run(main())
 ```
 
 **Image Generation:**
 ```python
 import freeGPT
-import asyncio
 from PIL import Image
+from io import BytesIO
+from asyncio import run
 
 
 async def main():
     while True:
         prompt = input("👦: ")
         try:
             resp = await getattr(freeGPT, "MODEL NAME").Generation.create(prompt)
-            Image.open(resp).show()
+            Image.open(BytesIO(resp)).show()
             print(f"🤖: Image shown.")
         except Exception as e:
             print(f"🤖: {e}")
 
 
-asyncio.run(main())
+run(main())
 ```
 
 ## Star History Chart:
 
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.2.4/README.md` & `freeGPT-1.2.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,36 @@
+#### Sorry, The freeGPT bot is in 100 servers and I can't verify it ATM. Please join my [Discord server](https://discord.gg/XH6pUGkwRr) if you wish to use it.
+
 [![PyPI](https://img.shields.io/pypi/v/freeGPT)](https://pypi.org/project/freeGPT)
 [![Downloads](https://static.pepy.tech/badge/freeGPT)](https://pypi.org/project/freeGPT)
 [![Status](https://img.shields.io/pypi/status/freeGPT)](https://pypi.org/project/freeGPT)
 
 # freeGPT
 
 freeGPT provides free access to GPT3, GPT4 and more models.
 
 ## Get started:
 
 ```
-python -m pip install --upgrade freeGPT
+python -m pip install -U freeGPT
 ```
 
 **Or add the [freeGPT Discord bot](https://dsc.gg/freegpt), it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot)!**
 
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Source:
 
-| Models   | Websites                                                |
-| -------- | ------------------------------------------------------- |
-| gpt3     | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
-| gpt4     | [<you.com>](https://you.com/)                           |
-| alpaca_7b| [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
-| prodia   | [<prodia.com>](https://prodia.com/)                     |
+| Models       | Websites                                                |
+| ------------ | ------------------------------------------------------- |
+| gpt3         | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
+| gpt4         | [<you.com>](https://you.com/)                           |
+| alpaca_7b    | [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
+| prodia       | [<prodia.com>](https://prodia.com/)                     |
+| pollinations | [<pollinations.ai>](https://pollinations.ai/)           |
 
 
 ## Support this repository:
 
 - Star this repository :D
 - Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
 - Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
@@ -52,47 +55,48 @@
 - And lastly, it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot).
 
 ## Example:
 
 **Text Completion:**
 ```python
 import freeGPT
-import asyncio
+from asyncio import run
 
 
 async def main():
     while True:
         prompt = input("👦: ")
         try:
             resp = await getattr(freeGPT, "MODEL NAME").Completion.create(prompt)
             print(f"🤖: {resp}")
         except Exception as e:
             print(f"🤖: {e}")
 
 
-asyncio.run(main())
+run(main())
 ```
 
 **Image Generation:**
 ```python
 import freeGPT
-import asyncio
 from PIL import Image
+from io import BytesIO
+from asyncio import run
 
 
 async def main():
     while True:
         prompt = input("👦: ")
         try:
             resp = await getattr(freeGPT, "MODEL NAME").Generation.create(prompt)
-            Image.open(resp).show()
+            Image.open(BytesIO(resp)).show()
             print(f"🤖: Image shown.")
         except Exception as e:
             print(f"🤖: {e}")
 
 
-asyncio.run(main())
+run(main())
 ```
 
 ## Star History Chart:
 
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.2.4/freeGPT/alpaca_7b.py` & `freeGPT-1.2.5/freeGPT/alpaca_7b.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from requests import post, exceptions
-from fake_useragent import UserAgent
 
 
 class Completion:
     """
     A class for generating text completions using an API.
 
     Attributes:
@@ -39,15 +38,15 @@
                     "Content-Type": "application/json",
                     "Sec-Ch-Ua": '"Google Chrome";v="89", "Chromium";v="89", ";Not A Brand";v="99"',
                     "Sec-Ch-Ua-Mobile": "?0",
                     "Sec-Ch-Ua-Platform": "Windows",
                     "Sec-Fetch-Dest": "empty",
                     "Sec-Fetch-Mode": "cors",
                     "Sec-Fetch-Site": "cross-site",
-                    "User-Agent": UserAgent().random,
+                    "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.79 Safari/537.36",
                 },
                 json={"prompt": prompt},
                 timeout=30,
             ).json()
         except exceptions.RequestException:
             raise Exception("Unable to fetch the response.")
```

### Comparing `freeGPT-1.2.4/freeGPT/gpt3.py` & `freeGPT-1.2.5/freeGPT/gpt3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,67 @@
+from aiohttp import ClientSession, ClientError
 from json import loads, JSONDecodeError
-from requests import post, exceptions
 
 
 class Completion:
     """
     This class provides methods for generating completions based on prompts.
     """
 
-    async def create(prompt):
+    @classmethod
+    async def create(cls, prompt):
         """
         Create a new completion based on the given prompt.
 
         Args:
             prompt (str): The prompt to generate a completion for.
 
         Returns:
             str: The generated completion.
 
         Raises:
             Exception: If unable to fetch the response.
         """
         try:
-            resp_obj = post(
-                "https://ava-alpha-api.codelink.io/api/chat",
-                headers={"Content-Type": "application/json"},
-                json={
-                    "model": "gpt-4",
-                    "temperature": 0.6,
-                    "stream": True,
-                    "messages": [
-                        {"role": "system", "content": "You are Ava, an AI assistant."},
-                        {"role": "user", "content": prompt},
-                    ],
-                },
-                timeout=30,
-            )
-        except exceptions.RequestException:
+            async with ClientSession() as session:
+                async with session.post(
+                    "https://ava-alpha-api.codelink.io/api/chat",
+                    headers={"Content-Type": "application/json"},
+                    json={
+                        "model": "gpt-4",
+                        "temperature": 0.6,
+                        "stream": True,
+                        "messages": [
+                            {
+                                "role": "system",
+                                "content": "You are Ava, an AI assistant.",
+                            },
+                            {"role": "user", "content": prompt},
+                        ],
+                    },
+                    timeout=45,
+                ) as resp_obj:
+                    resp = ""
+                    async for line in resp_obj.content:
+                        line_text = line.decode("utf-8").strip()
+                        if line_text.startswith("data:"):
+                            data = line_text.split("data:")[1]
+                            try:
+                                data_json = loads(data)
+                                if "choices" in data_json:
+                                    choices = data_json["choices"]
+                                    for choice in choices:
+                                        if (
+                                            "finish_reason" in choice
+                                            and choice["finish_reason"] == "stop"
+                                        ):
+                                            break
+                                        if (
+                                            "delta" in choice
+                                            and "content" in choice["delta"]
+                                        ):
+                                            resp += choice["delta"]["content"]
+                            except JSONDecodeError:
+                                pass
+                    return resp
+        except ClientError:
             raise Exception("Unable to fetch the response.")
-
-        resp = ""
-        for line in resp_obj.iter_lines():
-            line_text = line.decode("utf-8").strip()
-            if line_text.startswith("data:"):
-                data = line_text.split("data:")[1]
-                try:
-                    data_json = loads(data)
-                    if "choices" in data_json:
-                        choices = data_json["choices"]
-                        for choice in choices:
-                            if (
-                                "finish_reason" in choice
-                                and choice["finish_reason"] == "stop"
-                            ):
-                                break
-                            if "delta" in choice and "content" in choice["delta"]:
-                                resp += choice["delta"]["content"]
-                except JSONDecodeError:
-                    pass
-        return resp
```

### Comparing `freeGPT-1.2.4/freeGPT/gpt4.py` & `freeGPT-1.2.5/freeGPT/gpt4.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 import json
 import subprocess
 from uuid import uuid4
 from typing import Optional, List
-from fake_useragent import UserAgent
 
 try:
     import tls_client
 except Exception:
     subprocess.run(["pip", "install", "tls_client", "--no-cache-dir"])
 
 
@@ -65,15 +64,15 @@
             "sec-ch-ua": '"Not_A Brand";v="99", "Google Chrome";v="109", "Chromium";v="109"',
             "sec-ch-ua-mobile": "?0",
             "sec-ch-ua-platform": "Linux",
             "sec-fetch-dest": "empty",
             "sec-fetch-mode": "cors",
             "sec-fetch-site": "same-origin",
             "cookie": f"safesearch_guest=Off; uuid_guest={str(uuid4())}",
-            "user-agent": UserAgent().random,
+            "user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.79 Safari/537.36",
         }
         client.proxies = proxies
 
         response = client.get(
             "https://you.com/api/streamingSearch",
             params={
                 "q": prompt,
```

### Comparing `freeGPT-1.2.4/freeGPT/prodia.py` & `freeGPT-1.2.5/freeGPT/prodia.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-from io import BytesIO
+from random import randint
 from aiohttp import ClientSession
-from fake_useragent import UserAgent
 
 
 class Generation:
     async def create(prompt):
         """
         Create a new image generation based on the given prompt.
 
         Args:
             prompt (str): The prompt for generating the image.
 
         Returns:
-            BytesIO: The generated image content as a BytesIO object.
+            resp: The generated image content
         """
         params = {
             "new": "true",
             "prompt": prompt,
             "model": "Realistic_Vision_V2.0.safetensors [79587710]",
             "negative_prompt": "(nsfw:1.5),verybadimagenegative_v1.3, ng_deepnegative_v1_75t, (ugly face:0.5),cross-eyed,sketches, (worst quality:2), (low quality:2.1), (normal quality:2), lowres, normal quality, ((monochrome)), ((grayscale)), skin spots, acnes, skin blemishes, bad anatomy, DeepNegative, facing away, tilted head, {Multiple people}, lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worstquality, low quality, normal quality, jpegartifacts, signature, watermark, username, blurry, bad feet, cropped, poorly drawn hands, poorly drawn face, mutation, deformed, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, extra fingers, fewer digits, extra limbs, extra arms,extra legs, malformed limbs, fused fingers, too many fingers, long neck, cross-eyed,mutated hands, polar lowres, bad body, bad proportions, gross proportions, text, error, missing fingers, missing arms, missing legs, extra digit, extra arms, extra leg, extra foot, repeating hair",
             "steps": "50",
             "cfg": "9.5",
-            "seed": "84187",
+            "seed": randint(1, 10000),
             "sampler": "Euler",
             "aspect_ratio": "square",
         }
         headers = {
             "authority": "api.prodia.com",
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.6",
@@ -35,28 +34,30 @@
             "sec-ch-ua": '"Brave";v="113", "Chromium";v="113", "Not-A.Brand";v="24"',
             "sec-ch-ua-mobile": "?0",
             "sec-ch-ua-platform": '"Linux"',
             "sec-fetch-dest": "empty",
             "sec-fetch-mode": "cors",
             "sec-fetch-site": "same-site",
             "sec-gpc": "1",
-            "user-agent": UserAgent().random,
+            "user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.79 Safari/537.36",
         }
 
         async with ClientSession() as session:
             async with session.get(
-                "https://api.prodia.com/generate", params=params, headers=headers
-            ) as response:
-                data = await response.json()
+                "https://api.prodia.com/generate",
+                params=params,
+                headers=headers,
+                timeout=45,
+            ) as resp:
+                data = await resp.json()
                 job_id = data["job"]
                 while True:
                     async with session.get(
                         f"https://api.prodia.com/job/{job_id}", headers=headers
                     ) as resp:
                         json = await resp.json()
                         if json["status"] == "succeeded":
                             async with session.get(
                                 f"https://images.prodia.xyz/{job_id}.png?download=1",
                                 headers=headers,
                             ) as resp:
-                                content = await resp.content.read()
-                                return BytesIO(content)
+                                return await resp.content.read()
```

### Comparing `freeGPT-1.2.4/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.2.5/freeGPT.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.2.4
+Version: 1.2.5
 Summary: freeGPT provides free access to GPT3, GPT4 and more models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv2
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Discord, https://discord.gg/XH6pUGkwRr
 Keywords: artificial-intelligence,machine-learning,deep-learning,gpt4free,gpt4all,chatbot,freegpt,chatgpt,python,openai,llama,free,gpt,ai
@@ -20,40 +20,43 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+#### Sorry, The freeGPT bot is in 100 servers and I can't verify it ATM. Please join my [Discord server](https://discord.gg/XH6pUGkwRr) if you wish to use it.
+
 [![PyPI](https://img.shields.io/pypi/v/freeGPT)](https://pypi.org/project/freeGPT)
 [![Downloads](https://static.pepy.tech/badge/freeGPT)](https://pypi.org/project/freeGPT)
 [![Status](https://img.shields.io/pypi/status/freeGPT)](https://pypi.org/project/freeGPT)
 
 # freeGPT
 
 freeGPT provides free access to GPT3, GPT4 and more models.
 
 ## Get started:
 
 ```
-python -m pip install --upgrade freeGPT
+python -m pip install -U freeGPT
 ```
 
 **Or add the [freeGPT Discord bot](https://dsc.gg/freegpt), it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot)!**
 
 Join my [Discord server](https://discord.gg/XH6pUGkwRr) for live chat, support, or if you have any issues with this package.
 
 ## Source:
 
-| Models   | Websites                                                |
-| -------- | ------------------------------------------------------- |
-| gpt3     | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
-| gpt4     | [<you.com>](https://you.com/)                           |
-| alpaca_7b| [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
-| prodia   | [<prodia.com>](https://prodia.com/)                     |
+| Models       | Websites                                                |
+| ------------ | ------------------------------------------------------- |
+| gpt3         | [<ava-ai-ef611.web.app>](https://ava-ai-ef611.web.app/) |
+| gpt4         | [<you.com>](https://you.com/)                           |
+| alpaca_7b    | [<chatllama.baseten.co>](https://chatllama.baseten.co/) |
+| prodia       | [<prodia.com>](https://prodia.com/)                     |
+| pollinations | [<pollinations.ai>](https://pollinations.ai/)           |
 
 
 ## Support this repository:
 
 - Star this repository :D
 - Add the [freeGPT Discord bot](https://dsc.gg/freegpt).
 - Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
@@ -78,47 +81,48 @@
 - And lastly, it's [open-sourced](https://github.com/Ruu3f/freeGPT-discord-bot).
 
 ## Example:
 
 **Text Completion:**
 ```python
 import freeGPT
-import asyncio
+from asyncio import run
 
 
 async def main():
     while True:
         prompt = input("👦: ")
         try:
             resp = await getattr(freeGPT, "MODEL NAME").Completion.create(prompt)
             print(f"🤖: {resp}")
         except Exception as e:
             print(f"🤖: {e}")
 
 
-asyncio.run(main())
+run(main())
 ```
 
 **Image Generation:**
 ```python
 import freeGPT
-import asyncio
 from PIL import Image
+from io import BytesIO
+from asyncio import run
 
 
 async def main():
     while True:
         prompt = input("👦: ")
         try:
             resp = await getattr(freeGPT, "MODEL NAME").Generation.create(prompt)
-            Image.open(resp).show()
+            Image.open(BytesIO(resp)).show()
             print(f"🤖: Image shown.")
         except Exception as e:
             print(f"🤖: {e}")
 
 
-asyncio.run(main())
+run(main())
 ```
 
 ## Star History Chart:
 
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.2.4/setup.py` & `freeGPT-1.2.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.2.4",
+    version="1.2.5",
     description="freeGPT provides free access to GPT3, GPT4 and more models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv2",
     keywords=[
@@ -42,14 +42,14 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
     packages=find_packages(exclude=[".github"]),
     install_requires=[
         "requests",
-        "fake-useragent",
+        "aiohttp",
     ],
     project_urls={
         "Source": "https://github.com/Ruu3f/freeGPT",
         "Discord": "https://discord.gg/XH6pUGkwRr",
     },
 )
```


# Comparing `tmp/django-alert-winglet-0.1.4.tar.gz` & `tmp/django-alert-winglet-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-alert-winglet-0.1.4.tar", last modified: Thu Jun  8 13:18:06 2023, max compression
+gzip compressed data, was "django-alert-winglet-0.1.5.tar", last modified: Wed Jul 26 12:43:17 2023, max compression
```

## Comparing `django-alert-winglet-0.1.4.tar` & `django-alert-winglet-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 13:18:06.130201 django-alert-winglet-0.1.4/
--rw-rw-rw-   0        0        0     1076 2023-06-06 16:54:37.000000 django-alert-winglet-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       37 2023-06-06 11:31:41.000000 django-alert-winglet-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2446 2023-06-08 13:18:06.130708 django-alert-winglet-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1529 2023-06-06 16:54:37.000000 django-alert-winglet-0.1.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-08 13:18:06.117099 django-alert-winglet-0.1.4/alert_wing/
--rw-rw-rw-   0        0        0        0 2023-06-06 05:41:02.000000 django-alert-winglet-0.1.4/alert_wing/__init__.py
--rw-rw-rw-   0        0        0      157 2023-06-06 12:24:22.000000 django-alert-winglet-0.1.4/alert_wing/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-08 13:18:06.118677 django-alert-winglet-0.1.4/alert_wing/managers/
--rw-rw-rw-   0        0        0        0 2023-06-06 08:42:15.000000 django-alert-winglet-0.1.4/alert_wing/managers/__init__.py
--rw-rw-rw-   0        0        0      248 2023-06-06 08:42:15.000000 django-alert-winglet-0.1.4/alert_wing/managers/base_manager.py
--rw-rw-rw-   0        0        0     4568 2023-06-08 13:17:32.000000 django-alert-winglet-0.1.4/alert_wing/managers/discord_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-08 13:18:06.120362 django-alert-winglet-0.1.4/alert_wing/senders/
--rw-rw-rw-   0        0        0        0 2023-06-06 05:41:02.000000 django-alert-winglet-0.1.4/alert_wing/senders/__init__.py
--rw-rw-rw-   0        0        0      142 2023-06-06 05:41:02.000000 django-alert-winglet-0.1.4/alert_wing/senders/base.py
--rw-rw-rw-   0        0        0     4563 2023-06-06 17:08:24.000000 django-alert-winglet-0.1.4/alert_wing/senders/discord.py
-drwxrwxrwx   0        0        0        0 2023-06-08 13:18:06.129970 django-alert-winglet-0.1.4/django_alert_winglet.egg-info/
--rw-rw-rw-   0        0        0     2446 2023-06-08 13:18:06.000000 django-alert-winglet-0.1.4/django_alert_winglet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-06-08 13:18:06.000000 django-alert-winglet-0.1.4/django_alert_winglet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 13:18:06.000000 django-alert-winglet-0.1.4/django_alert_winglet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-08 13:18:06.000000 django-alert-winglet-0.1.4/django_alert_winglet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-08 13:18:06.000000 django-alert-winglet-0.1.4/django_alert_winglet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       90 2023-06-06 11:27:00.000000 django-alert-winglet-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0      992 2023-06-08 13:18:06.131260 django-alert-winglet-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-06-06 11:30:18.000000 django-alert-winglet-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:17.710616 django-alert-winglet-0.1.5/
+-rw-rw-rw-   0        0        0     1064 2023-07-26 12:38:37.000000 django-alert-winglet-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-06-06 11:31:41.000000 django-alert-winglet-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2009 2023-07-26 12:43:17.710817 django-alert-winglet-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1143 2023-07-26 12:41:19.000000 django-alert-winglet-0.1.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:17.692280 django-alert-winglet-0.1.5/alert_winglet/
+-rw-rw-rw-   0        0        0        0 2023-06-06 05:41:02.000000 django-alert-winglet-0.1.5/alert_winglet/__init__.py
+-rw-rw-rw-   0        0        0      160 2023-07-26 11:36:28.000000 django-alert-winglet-0.1.5/alert_winglet/apps.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:17.693825 django-alert-winglet-0.1.5/alert_winglet/base/
+-rw-rw-rw-   0        0        0        0 2023-07-21 15:58:29.000000 django-alert-winglet-0.1.5/alert_winglet/base/__init__.py
+-rw-rw-rw-   0        0        0      317 2023-07-21 11:39:55.000000 django-alert-winglet-0.1.5/alert_winglet/base/manager.py
+-rw-rw-rw-   0        0        0      142 2023-06-06 05:41:02.000000 django-alert-winglet-0.1.5/alert_winglet/base/sender.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:17.695185 django-alert-winglet-0.1.5/alert_winglet/discord/
+-rw-rw-rw-   0        0        0        0 2023-07-21 09:53:37.000000 django-alert-winglet-0.1.5/alert_winglet/discord/__init__.py
+-rw-rw-rw-   0        0        0     4544 2023-07-26 11:37:00.000000 django-alert-winglet-0.1.5/alert_winglet/discord/manager.py
+-rw-rw-rw-   0        0        0     4448 2023-07-26 11:37:00.000000 django-alert-winglet-0.1.5/alert_winglet/discord/sender.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:43:17.709733 django-alert-winglet-0.1.5/django_alert_winglet.egg-info/
+-rw-rw-rw-   0        0        0     2009 2023-07-26 12:43:17.000000 django-alert-winglet-0.1.5/django_alert_winglet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-07-26 12:43:17.000000 django-alert-winglet-0.1.5/django_alert_winglet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 12:43:17.000000 django-alert-winglet-0.1.5/django_alert_winglet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-26 12:43:17.000000 django-alert-winglet-0.1.5/django_alert_winglet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-26 12:43:17.000000 django-alert-winglet-0.1.5/django_alert_winglet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       90 2023-06-06 11:27:00.000000 django-alert-winglet-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      952 2023-07-26 12:43:17.714033 django-alert-winglet-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-06-06 11:30:18.000000 django-alert-winglet-0.1.5/setup.py
```

### Comparing `django-alert-winglet-0.1.4/LICENSE` & `django-alert-winglet-0.1.5/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 MojtabaDavi
+Copyright (c) 2023
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `django-alert-winglet-0.1.4/PKG-INFO` & `django-alert-winglet-0.1.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,85 +1,72 @@
 Metadata-Version: 2.1
 Name: django-alert-winglet
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Django app to send any exception to discord channel.
 Author: Mojtaba
 Author-email: Mojtabadavi14@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: Django :: 4.1
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: ~=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-
-===========
-alert-wing
-===========
-
 alert-wing
 ===========
 A Django app to send any exception to a Discord channel.
 
-Introduction
-------------
-alert-wing is a Django app that allows you to send any exception to various apps, such as Discord. You can easily implement the functionality you need for each app.
-
 Quick start
 -----------
 
 1. Add "alert-wing" to your `INSTALLED_APPS` setting in your Django project's settings file:
 
-   .. code-block:: python
+   .. code-block:: Django
 
         INSTALLED_APPS = [
             ...,
-            "alert-wing",
+            "alert-winglet",
         ]
 
-2. Set the `DISCORD_WEBHOOK_URL` variable in your Django settings. This is the URL of the Discord webhook you want to use for sending exceptions.
 
-3. Use the `DiscordEmbedManager` class to create a Discord Embed object, and then use the `Discord` delivery method to send the exception to your Discord channel using the webhook.
+Discord:
+    1.Set the `DISCORD_WEBHOOK_URL` variable in your Django settings. This is the URL of the Discord webhook you want to use for sending exceptions.
 
-Documentation
--------------
+    2.Use the `DiscordEmbedManager` class to create a Discord Embed object, and then use the `Discord` delivery method to send the exception to your Discord channel using the webhook.
 
-For detailed documentation and usage instructions, please refer to the "docs" directory.
 
 Requirements
 ------------
 
 - django ~= 4.1.5
 - discord.py ~=2.2.3
 - requests ~=2.28.2
 
 License
 -------
-
 This project is licensed under the MIT License.
 
-Contributing
-------------
-
-We welcome contributions! Please refer to the "CONTRIBUTING.md" file for more information.
 
 Bug Reports and Feature Requests
 --------------------------------
 
-Please use the GitHub issue tracker to report any bugs or submit feature requests.
+Please use the GitHub_issue_ tracker to report any bugs or submit feature requests.
+
 
 Authors
 -------
 
 - Mojtaba
 - Email: Mojtabadavi14@gmail.com
+
+
+.. _GitHub_issue: https://github.com/Mojitaba34/alert-winglet/issues
```

### Comparing `django-alert-winglet-0.1.4/alert_wing/senders/discord.py` & `django-alert-winglet-0.1.5/alert_winglet/discord/sender.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-import json
-from typing import Any
-
-import requests
-from django.conf import settings
-
-from alert_wing.senders.base import BaseSender
-
-
-class Discord(BaseSender):
-    """
-    A class for sending messages or files to a Discord webhook.
-
-    Attributes:
-        DATA (dict): A class-level dictionary to store the message data.
-
-    Args:
-        content (str): The text content of the message. If `None`, either `file` or `embeds` must be provided.
-        username (str): The username to display for the message sender.
-        avatar_url (str): The URL of the avatar image to display for the message sender.
-        tts (bool): Specifies if the message should be sent as a text-to-speech message.
-        file (file-like object): A file-like object to upload and send along with the message.
-        embeds (list): A list of Discord embed objects to include with the message.
-        allowed_mentions (dict): A dictionary specifying the allowed mentions in the message.
-        webhook (str): The URL of the Discord webhook to send the message to.
-
-    Raises:
-        ValueError: If neither `content`, `file`, nor `embeds` are provided.
-        ValueError: If `webhook` is not provided.
-
-    Methods:
-        post():
-            Sends the constructed message or file to the specified Discord webhook.
-
-    Usage example:
-        discord = Discord(
-            content="Hello, everyone!",
-            username="MyBot",
-            avatar_url="https://example.com/avatar.png",
-            tts=False,
-            file=open("example.txt", "rb"),
-            embeds=[{
-                "title": "Example Embed",
-                "description": "This is an example embed."
-            }],
-            allowed_mentions={"users": [1234567890]},
-            webhook="https://discord.com/api/webhooks/1234567890/abcdefgh"
-        )
-        response = discord.post()
-        print(response.status_code)
-    """
-
-    DATA = {}
-
-    def __init__(
-        self,
-        content: str = None,
-        username: str = None,
-        avatar_url: str = None,
-        tts: bool = False,
-        file: Any = None,
-        embeds: list = None,
-        allowed_mentions=None,
-    ):
-        """
-        Initializes a new Discord message or file.
-
-        Args:
-            content (str): The text content of the message. If `None`, either `file` or `embeds` must be provided.
-            username (str): The username to display for the message sender.
-            avatar_url (str): The URL of the avatar image to display for the message sender.
-            tts (bool): Specifies if the message should be sent as a text-to-speech message.
-            file (file-like object): A file-like object to upload and send along with the message.
-            embeds (list): A list of Discord embed objects to include with the message.
-            allowed_mentions (dict): A dictionary specifying the allowed mentions in the message.
-            webhook (str): The URL of the Discord webhook to send the message to.
-
-        Raises:
-            ValueError: If neither `content`, `file`, nor `embeds` are provided.
-            ValueError: If `webhook` is not provided.
-        """
-        if content is None and file is None and embeds is None:
-            raise ValueError("Required one of content, file, embeds")
-
-        if content is not None:
-            self.DATA["content"] = content
-
-        if username is not None:
-            self.DATA["username"] = username
-
-        if avatar_url is not None:
-            self.DATA["avatar_url"] = avatar_url
-
-        if embeds is not None:
-            self.DATA["embeds"] = embeds
-
-        if allowed_mentions is not None:
-            self.DATA["allowed_mentions"] = allowed_mentions
-
-        self.file = file
-
-        try:
-            self.webhook = settings.DISCORD_WEBHOOK_URL
-        except AttributeError:
-            raise ValueError("DISCORD_WEBHOOK_URL variable must set in django settings")
-
-        self.DATA["tts"] = tts
-
-    def send(self):
-        """
-        Sends the constructed message or file to the specified Discord webhook.
-
-        Returns:
-            The response
-        """
-        if self.file is not None:
-            return requests.post(
-                self.webhook, {"payload_json": json.dumps(self.DATA)}, files=self.file
-            )
-
-        return requests.post(
-            self.webhook,
-            json.dumps(self.DATA),
-            headers={"Content-Type": "application/json"},
-        )
+import json
+from typing import Any
+
+import requests
+from django.conf import settings
+
+from alert_winglet.base.sender import BaseSender
+
+
+class DiscordDelivery(BaseSender):
+    """
+    A class for sending messages or files to a Discord webhook.
+
+    Attributes:
+        DATA (dict): A class-level dictionary to store the message data.
+
+    Args:
+        content (str): The text content of the message. If `None`, either `file` or `embeds` must be provided.
+        username (str): The username to display for the message sender.
+        avatar_url (str): The URL of the avatar image to display for the message sender.
+        tts (bool): Specifies if the message should be sent as a text-to-speech message.
+        file (file-like object): A file-like object to upload and send along with the message.
+        embeds (list): A list of Discord embed objects to include with the message.
+        allowed_mentions (dict): A dictionary specifying the allowed mentions in the message.
+        webhook (str): The URL of the Discord webhook to send the message to.
+
+    Raises:
+        ValueError: If neither `content`, `file`, nor `embeds` are provided.
+        ValueError: If `webhook` is not provided.
+
+    Methods:
+        post():
+            Sends the constructed message or file to the specified Discord webhook.
+
+    Usage example:
+        discord = Discord(
+            content="Hello, everyone!",
+            username="MyBot",
+            avatar_url="https://example.com/avatar.png",
+            tts=False,
+            file=open("example.txt", "rb"),
+            embeds=[{
+                "title": "Example Embed",
+                "description": "This is an example embed."
+            }],
+            allowed_mentions={"users": [1234567890]},
+            webhook="https://discord.com/api/webhooks/1234567890/abcdefgh"
+        )
+        response = discord.post()
+        print(response.status_code)
+    """
+
+    DATA = {}
+
+    def __init__(
+        self,
+        content: str = None,
+        username: str = None,
+        avatar_url: str = None,
+        tts: bool = False,
+        file: Any = None,
+        embeds: list = None,
+        allowed_mentions=None,
+    ):
+        """
+        Initializes a new Discord message or file.
+
+        Args:
+            content (str): The text content of the message. If `None`, either `file` or `embeds` must be provided.
+            username (str): The username to display for the message sender.
+            avatar_url (str): The URL of the avatar image to display for the message sender.
+            tts (bool): Specifies if the message should be sent as a text-to-speech message.
+            file (file-like object): A file-like object to upload and send along with the message.
+            embeds (list): A list of Discord embed objects to include with the message.
+            allowed_mentions (dict): A dictionary specifying the allowed mentions in the message.
+            webhook (str): The URL of the Discord webhook to send the message to.
+
+        Raises:
+            ValueError: If neither `content`, `file`, nor `embeds` are provided.
+            ValueError: If `webhook` is not provided.
+        """
+        if content is None and file is None and embeds is None:
+            raise ValueError("Required one of content, file, embeds")
+
+        if content is not None:
+            self.DATA["content"] = content
+
+        if username is not None:
+            self.DATA["username"] = username
+
+        if avatar_url is not None:
+            self.DATA["avatar_url"] = avatar_url
+
+        if embeds is not None:
+            self.DATA["embeds"] = embeds
+
+        if allowed_mentions is not None:
+            self.DATA["allowed_mentions"] = allowed_mentions
+
+        self.file = file
+
+        try:
+            self.webhook = settings.DISCORD_WEBHOOK_URL
+        except AttributeError:
+            raise ValueError("DISCORD_WEBHOOK_URL variable must set in django settings")
+
+        self.DATA["tts"] = tts
+
+    def send(self):
+        """
+        Sends the constructed message or file to the specified Discord webhook.
+
+        Returns:
+            The response
+        """
+        if self.file is not None:
+            return requests.post(
+                self.webhook, {"payload_json": json.dumps(self.DATA)}, files=self.file
+            )
+
+        return requests.post(
+            self.webhook,
+            json.dumps(self.DATA),
+            headers={"Content-Type": "application/json"},
+        )
```

### Comparing `django-alert-winglet-0.1.4/django_alert_winglet.egg-info/PKG-INFO` & `django-alert-winglet-0.1.5/django_alert_winglet.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,85 +1,72 @@
 Metadata-Version: 2.1
 Name: django-alert-winglet
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Django app to send any exception to discord channel.
 Author: Mojtaba
 Author-email: Mojtabadavi14@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: Django :: 4.1
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: ~=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-
-===========
-alert-wing
-===========
-
 alert-wing
 ===========
 A Django app to send any exception to a Discord channel.
 
-Introduction
-------------
-alert-wing is a Django app that allows you to send any exception to various apps, such as Discord. You can easily implement the functionality you need for each app.
-
 Quick start
 -----------
 
 1. Add "alert-wing" to your `INSTALLED_APPS` setting in your Django project's settings file:
 
-   .. code-block:: python
+   .. code-block:: Django
 
         INSTALLED_APPS = [
             ...,
-            "alert-wing",
+            "alert-winglet",
         ]
 
-2. Set the `DISCORD_WEBHOOK_URL` variable in your Django settings. This is the URL of the Discord webhook you want to use for sending exceptions.
 
-3. Use the `DiscordEmbedManager` class to create a Discord Embed object, and then use the `Discord` delivery method to send the exception to your Discord channel using the webhook.
+Discord:
+    1.Set the `DISCORD_WEBHOOK_URL` variable in your Django settings. This is the URL of the Discord webhook you want to use for sending exceptions.
 
-Documentation
--------------
+    2.Use the `DiscordEmbedManager` class to create a Discord Embed object, and then use the `Discord` delivery method to send the exception to your Discord channel using the webhook.
 
-For detailed documentation and usage instructions, please refer to the "docs" directory.
 
 Requirements
 ------------
 
 - django ~= 4.1.5
 - discord.py ~=2.2.3
 - requests ~=2.28.2
 
 License
 -------
-
 This project is licensed under the MIT License.
 
-Contributing
-------------
-
-We welcome contributions! Please refer to the "CONTRIBUTING.md" file for more information.
 
 Bug Reports and Feature Requests
 --------------------------------
 
-Please use the GitHub issue tracker to report any bugs or submit feature requests.
+Please use the GitHub_issue_ tracker to report any bugs or submit feature requests.
+
 
 Authors
 -------
 
 - Mojtaba
 - Email: Mojtabadavi14@gmail.com
+
+
+.. _GitHub_issue: https://github.com/Mojitaba34/alert-winglet/issues
```

### Comparing `django-alert-winglet-0.1.4/setup.cfg` & `django-alert-winglet-0.1.5/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 616c 6572 742d   = django-alert-
 00000020: 7769 6e67 6c65 740d 0a76 6572 7369 6f6e  winglet..version
-00000030: 203d 2030 2e31 2e34 0d0a 6465 7363 7269   = 0.1.4..descri
+00000030: 203d 2030 2e31 2e35 0d0a 6465 7363 7269   = 0.1.5..descri
 00000040: 7074 696f 6e20 3d20 4120 446a 616e 676f  ption = A Django
 00000050: 2061 7070 2074 6f20 7365 6e64 2061 6e79   app to send any
 00000060: 2065 7863 6570 7469 6f6e 2074 6f20 6469   exception to di
 00000070: 7363 6f72 6420 6368 616e 6e65 6c2e 0d0a  scord channel...
 00000080: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000090: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 000000a0: 7465 7874 2f78 2d72 7374 0d0a 6c6f 6e67  text/x-rst..long
@@ -22,41 +22,39 @@
 00000150: 740d 0a09 4672 616d 6577 6f72 6b20 3a3a  t...Framework ::
 00000160: 2044 6a61 6e67 6f0d 0a09 4672 616d 6577   Django...Framew
 00000170: 6f72 6b20 3a3a 2044 6a61 6e67 6f20 3a3a  ork :: Django ::
 00000180: 2034 2e31 0d0a 0949 6e74 656e 6465 6420   4.1...Intended 
 00000190: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
 000001a0: 6c6f 7065 7273 0d0a 094c 6963 656e 7365  lopers...License
 000001b0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-000001c0: 203a 3a20 4253 4420 4c69 6365 6e73 650d   :: BSD License.
+000001c0: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
 000001d0: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
 000001e0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
 000001f0: 6465 6e74 0d0a 0950 726f 6772 616d 6d69  dent...Programmi
 00000200: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000210: 7974 686f 6e0d 0a09 5072 6f67 7261 6d6d  ython...Programm
-00000220: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000230: 5079 7468 6f6e 203a 3a20 330d 0a09 5072  Python :: 3...Pr
-00000240: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000250: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000260: 3320 3a3a 204f 6e6c 790d 0a09 5072 6f67  3 :: Only...Prog
-00000270: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000280: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000290: 380d 0a09 5072 6f67 7261 6d6d 696e 6720  8...Programming 
-000002a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002b0: 6f6e 203a 3a20 332e 390d 0a09 546f 7069  on :: 3.9...Topi
-000002c0: 6320 3a3a 2049 6e74 6572 6e65 7420 3a3a  c :: Internet ::
-000002d0: 2057 5757 2f48 5454 500d 0a09 546f 7069   WWW/HTTP...Topi
-000002e0: 6320 3a3a 2049 6e74 6572 6e65 7420 3a3a  c :: Internet ::
-000002f0: 2057 5757 2f48 5454 5020 3a3a 2044 796e   WWW/HTTP :: Dyn
-00000300: 616d 6963 2043 6f6e 7465 6e74 0d0a 0d0a  amic Content....
-00000310: 5b6f 7074 696f 6e73 5d0d 0a69 6e63 6c75  [options]..inclu
-00000320: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
-00000330: 3d20 7472 7565 0d0a 7061 636b 6167 6573  = true..packages
-00000340: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
-00000350: 5f72 6571 7569 7265 7320 3d20 7e3d 332e  _requires = ~=3.
-00000360: 3130 0d0a 696e 7374 616c 6c5f 7265 7175  10..install_requ
-00000370: 6972 6573 203d 200d 0a09 446a 616e 676f  ires = ...Django
-00000380: 207e 3d20 342e 312e 350d 0a09 6469 7363   ~= 4.1.5...disc
-00000390: 6f72 642e 7079 207e 3d32 2e32 2e33 0d0a  ord.py ~=2.2.3..
-000003a0: 0972 6571 7565 7374 7320 7e3d 322e 3238  .requests ~=2.28
-000003b0: 2e32 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  .2....[egg_info]
-000003c0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-000003d0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000210: 7974 686f 6e20 3a3a 2033 203a 3a20 4f6e  ython :: 3 :: On
+00000220: 6c79 0d0a 0950 726f 6772 616d 6d69 6e67  ly...Programming
+00000230: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000240: 686f 6e20 3a3a 2033 2e31 300d 0a09 5072  hon :: 3.10...Pr
+00000250: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000260: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000270: 332e 3131 0d0a 0946 7261 6d65 776f 726b  3.11...Framework
+00000280: 203a 3a20 446a 616e 676f 203a 3a20 342e   :: Django :: 4.
+00000290: 310d 0a09 546f 7069 6320 3a3a 2049 6e74  1...Topic :: Int
+000002a0: 6572 6e65 7420 3a3a 2057 5757 2f48 5454  ernet :: WWW/HTT
+000002b0: 500d 0a09 546f 7069 6320 3a3a 2049 6e74  P...Topic :: Int
+000002c0: 6572 6e65 7420 3a3a 2057 5757 2f48 5454  ernet :: WWW/HTT
+000002d0: 5020 3a3a 2044 796e 616d 6963 2043 6f6e  P :: Dynamic Con
+000002e0: 7465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  tent....[options
+000002f0: 5d0d 0a69 6e63 6c75 6465 5f70 6163 6b61  ]..include_packa
+00000300: 6765 5f64 6174 6120 3d20 7472 7565 0d0a  ge_data = true..
+00000310: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+00000320: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+00000330: 7320 3d20 7e3d 332e 3130 0d0a 696e 7374  s = ~=3.10..inst
+00000340: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
+00000350: 0a09 446a 616e 676f 207e 3d20 342e 312e  ..Django ~= 4.1.
+00000360: 350d 0a09 6469 7363 6f72 642e 7079 207e  5...discord.py ~
+00000370: 3d32 2e32 2e33 0d0a 0972 6571 7565 7374  =2.2.3...request
+00000380: 7320 7e3d 322e 3238 2e32 0d0a 0d0a 5b65  s ~=2.28.2....[e
+00000390: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+000003a0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+000003b0: 203d 2030 0d0a 0d0a                       = 0....
```


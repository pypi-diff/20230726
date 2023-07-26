# Comparing `tmp/slack-react-0.2.1.tar.gz` & `tmp/slack-react-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-react-0.2.1.tar", last modified: Wed Jul 26 08:44:07 2023, max compression
+gzip compressed data, was "slack-react-0.2.2.tar", last modified: Wed Jul 26 10:07:56 2023, max compression
```

## Comparing `slack-react-0.2.1.tar` & `slack-react-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:44:07.193352 slack-react-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:44:07.193352 slack-react-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-26 08:43:51.000000 slack-react-0.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:44:07.193352 slack-react-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-26 08:43:51.000000 slack-react-0.2.1/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-26 08:43:51.000000 slack-react-0.2.1/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-26 08:43:51.000000 slack-react-0.2.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 08:43:51.000000 slack-react-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 08:43:51.000000 slack-react-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42415 2023-07-26 08:44:07.193352 slack-react-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-26 08:43:51.000000 slack-react-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-26 08:43:51.000000 slack-react-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 08:44:07.193352 slack-react-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:44:07.193352 slack-react-0.2.1/slack_react.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42415 2023-07-26 08:44:07.000000 slack-react-0.2.1/slack_react.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-26 08:44:07.000000 slack-react-0.2.1/slack_react.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 08:44:07.000000 slack-react-0.2.1/slack_react.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 08:44:07.000000 slack-react-0.2.1/slack_react.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 08:44:07.000000 slack-react-0.2.1/slack_react.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 08:44:07.000000 slack-react-0.2.1/slack_react.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     7430 2023-07-26 08:43:51.000000 slack-react-0.2.1/slack_react.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:07:56.092526 slack-react-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:07:56.088526 slack-react-0.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-26 10:07:45.000000 slack-react-0.2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:07:56.088526 slack-react-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-26 10:07:45.000000 slack-react-0.2.2/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-26 10:07:45.000000 slack-react-0.2.2/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-26 10:07:45.000000 slack-react-0.2.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 10:07:45.000000 slack-react-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 10:07:45.000000 slack-react-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42415 2023-07-26 10:07:56.092526 slack-react-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-26 10:07:45.000000 slack-react-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-26 10:07:45.000000 slack-react-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 10:07:56.092526 slack-react-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:07:56.092526 slack-react-0.2.2/slack_react.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42415 2023-07-26 10:07:56.000000 slack-react-0.2.2/slack_react.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-26 10:07:56.000000 slack-react-0.2.2/slack_react.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 10:07:56.000000 slack-react-0.2.2/slack_react.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 10:07:56.000000 slack-react-0.2.2/slack_react.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 10:07:56.000000 slack-react-0.2.2/slack_react.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 10:07:56.000000 slack-react-0.2.2/slack_react.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8372 2023-07-26 10:07:45.000000 slack-react-0.2.2/slack_react.py
```

### Comparing `slack-react-0.2.1/.github/workflows/pypi.yaml` & `slack-react-0.2.2/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `slack-react-0.2.1/.github/workflows/release.yaml` & `slack-react-0.2.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `slack-react-0.2.1/LICENSE` & `slack-react-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slack-react-0.2.1/PKG-INFO` & `slack-react-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-react
-Version: 0.2.1
+Version: 0.2.2
 Summary: Add reactions that spell out messages to Slack messages
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `slack-react-0.2.1/README.md` & `slack-react-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `slack-react-0.2.1/pyproject.toml` & `slack-react-0.2.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "rich",
   "slack_sdk"
 ]
-version = "0.2.1"
+version = "0.2.2"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 slack-react = "slack_react:main"
```

### Comparing `slack-react-0.2.1/slack_react.egg-info/PKG-INFO` & `slack-react-0.2.2/slack_react.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-react
-Version: 0.2.1
+Version: 0.2.2
 Summary: Add reactions that spell out messages to Slack messages
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `slack-react-0.2.1/slack_react.py` & `slack-react-0.2.2/slack_react.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 import argparse
+import logging
 import os
 import re
 import sys
 from typing import Dict, List
 
 import slack_sdk
 from rich import print
+from rich.logging import RichHandler
 
 
 def parse_args():
     # create the top-level parser
     parser = argparse.ArgumentParser()
-
+    parser.add_argument(
+        "-d", "--debug", action="store_true", default=False, help="Debug mode"
+    )
     parser.add_argument("-c", "--channel", help="Channel name")
     parser.add_argument(
         "-t",
         "--token",
         default=os.environ.get("SLACK_USER_OAUTH_TOKEN"),
         help="Slack OAUTH Token",
     )
@@ -51,15 +55,15 @@
         "h": ["alphabet-white-h", "alphabet-yellow-h"],
         "i": ["alphabet-white-i", "alphabet-yellow-i"],
         "j": ["alphabet-white-j", "alphabet-yellow-j"],
         "k": ["alphabet-white-k", "alphabet-yellow-k"],
         "l": ["alphabet-white-l", "alphabet-yellow-l"],
         "m": ["alphabet-white-m", "alphabet-yellow-m"],
         "n": ["alphabet-white-n", "alphabet-yellow-n"],
-        "o": ["alphabet-white-o", "alphabet-yellow-o"],
+        "o": ["alphabet-white-o", "alphabet-yellow-o", "o"],
         "p": ["alphabet-white-p", "alphabet-yellow-p"],
         "q": ["alphabet-white-q", "alphabet-yellow-q"],
         "r": ["alphabet-white-r", "alphabet-yellow-r"],
         "s": ["alphabet-white-s", "alphabet-yellow-s"],
         "t": ["alphabet-white-t", "alphabet-yellow-t"],
         "u": ["alphabet-white-u", "alphabet-yellow-u"],
         "v": ["alphabet-white-v", "alphabet-yellow-v"],
@@ -73,14 +77,31 @@
         "3": ["three", "three"],
         "4": ["four", "four"],
         "5": ["five", "five"],
         "6": ["six", "six"],
         "7": ["seven", "seven"],
         "8": ["eight", "eight"],
         "9": ["nine", "nine"],
+        "?": ["alphabet-white-question", "alphabet-yellow-question"],
+        "!": [
+            "exclamation",
+            "bangbang",
+            "gray_exclamation",
+            "alphabet-white-exclamation",
+            "alphabet-yellow-exclamation",
+        ],
+        "-": ["heavy_minus_sign", "wavy_dash"],
+        " ": [
+            "black_small_square",
+            "white_small_square",
+            "small_orange_diamond",
+            "small_blue_diamond",
+            "black_medium_square",
+            "white_medium_square",
+        ],
     }
 
     # create a list to hold the emojis
     emojis = []
     # create a dictionary to hold the index of the next emoji to use for
     # each character
     next_emoji_index = {}
@@ -192,22 +213,28 @@
             channel=channel_id, timestamp=timestamp, name=reaction
         )
 
 
 def add_reactions(client, channel_id, timestamp, message):
     for reaction in message_to_emoji_list(message):
         # react to a message
+        LOGGER.info("Adding reaction to message: %s", reaction)
         client.reactions_add(
             channel=channel_id, timestamp=timestamp, name=reaction
         )
 
 
 def main():
     args = parse_args()
 
+    logging.basicConfig(
+        level=logging.DEBUG if args.debug else logging.INFO,
+        handlers=[RichHandler()],
+    )
+
     # create a client instance
     client = slack_sdk.WebClient(token=args.token)
 
     channel_id = get_channel_id(client, args.channel)
 
     if not channel_id:
         print(f"Channel '{args.channel}' not found", file=sys.stderr)
@@ -229,9 +256,12 @@
 
     if args.reaction and not args.remove:
         add_reactions(client, channel_id, ts, args.reaction)
 
     return 0
 
 
+LOGGER = logging.getLogger(__name__)
+
+
 if __name__ == "__main__":
     sys.exit(main())
```


# Comparing `tmp/SMAGrader-0.1.6.tar.gz` & `tmp/SMAGrader-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMAGrader-0.1.6.tar", last modified: Tue Jul 25 21:44:59 2023, max compression
+gzip compressed data, was "SMAGrader-0.1.7.tar", last modified: Wed Jul 26 00:33:32 2023, max compression
```

## Comparing `SMAGrader-0.1.6.tar` & `SMAGrader-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 21:44:59.813421 SMAGrader-0.1.6/
--rw-rw-rw-   0        0        0      151 2023-07-25 21:44:59.812420 SMAGrader-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-25 21:44:59.781523 SMAGrader-0.1.6/SMAGrader/
--rw-rw-rw-   0        0        0        0 2023-07-25 19:17:05.000000 SMAGrader-0.1.6/SMAGrader/__init__.py
--rw-rw-rw-   0        0        0    18856 2023-07-25 21:44:43.000000 SMAGrader-0.1.6/SMAGrader/checker.py
-drwxrwxrwx   0        0        0        0 2023-07-25 21:44:59.809419 SMAGrader-0.1.6/SMAGrader.egg-info/
--rw-rw-rw-   0        0        0      151 2023-07-25 21:44:59.000000 SMAGrader-0.1.6/SMAGrader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-07-25 21:44:59.000000 SMAGrader-0.1.6/SMAGrader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 21:44:59.000000 SMAGrader-0.1.6/SMAGrader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-25 21:44:59.000000 SMAGrader-0.1.6/SMAGrader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-25 21:44:59.000000 SMAGrader-0.1.6/SMAGrader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 21:44:59.813421 SMAGrader-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      426 2023-07-25 21:44:25.000000 SMAGrader-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:33:32.844932 SMAGrader-0.1.7/
+-rw-rw-rw-   0        0        0      151 2023-07-26 00:33:32.843933 SMAGrader-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 00:33:32.813926 SMAGrader-0.1.7/SMAGrader/
+-rw-rw-rw-   0        0        0        0 2023-07-25 19:17:05.000000 SMAGrader-0.1.7/SMAGrader/__init__.py
+-rw-rw-rw-   0        0        0    18903 2023-07-26 00:32:33.000000 SMAGrader-0.1.7/SMAGrader/checker.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:33:32.840932 SMAGrader-0.1.7/SMAGrader.egg-info/
+-rw-rw-rw-   0        0        0      151 2023-07-26 00:33:32.000000 SMAGrader-0.1.7/SMAGrader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-07-26 00:33:32.000000 SMAGrader-0.1.7/SMAGrader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 00:33:32.000000 SMAGrader-0.1.7/SMAGrader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-26 00:33:32.000000 SMAGrader-0.1.7/SMAGrader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-26 00:33:32.000000 SMAGrader-0.1.7/SMAGrader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 00:33:32.844932 SMAGrader-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      426 2023-07-26 00:32:50.000000 SMAGrader-0.1.7/setup.py
```

### Comparing `SMAGrader-0.1.6/SMAGrader/checker.py` & `SMAGrader-0.1.7/SMAGrader/checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,18 @@
 from nltk.tag import pos_tag
 import json
 import praw
 import firebase_admin
 from firebase_admin import credentials, firestore
 import os
 
-with open("secret.json") as config_file:
-    config = json.load(config_file)
-
-client_id = config.get("client_id")
-client_secret = config.get("client_secret")
-user_agent = config.get("user_agent")
-path = config.get("google_credentials")
+# client_id = config.get("client_id")
+# client_secret = config.get("client_secret")
+# user_agent = config.get("user_agent")
+path = "C:/Users/arish/AppData/Roaming/gcloud/cmst-reddit-analysis-firebase-adminsdk-76tgx-265cb629e1.json"
 cred = credentials.Certificate(path)
 firebase_admin.initialize_app(cred)
 db = firestore.client()
 
 
 def authenticate():
     try:
@@ -558,40 +555,40 @@
             send_results(
                 "named_entity_recognition_check",
                 email,
                 (f"Case {i+1} failed"),
             )
 
 
-def scrape_from_reddit_check(func):
-    subreddit_name = "ut_sma"
-    actual_content = func(subreddit_name)
-
-    reddit = praw.Reddit(
-        client_id=client_id,
-        client_secret=client_secret,
-        user_agent=user_agent,
-    )
-    expected_content = []
-    subreddit = reddit.subreddit(subreddit_name)
-
-    for submission in subreddit.new(limit=100):
-        expected_content.append(submission.title)
-        submission.comments.replace_more(limit=None)
-        for comment in submission.comments.list():
-            expected_content.append(comment.body)
-
-    if expected_content == actual_content:
-        send_results(
-            "named_entity_recognition_check",
-            email,
-            ("Cases passed"),
-        )
-    else:
-        send_results(
-            "named_entity_recognition_check",
-            email,
-            ("Cases failed"),
-        )
+# def scrape_from_reddit_check(func):
+#     subreddit_name = "ut_sma"
+#     actual_content = func(subreddit_name)
+
+#     reddit = praw.Reddit(
+#         client_id=client_id,
+#         client_secret=client_secret,
+#         user_agent=user_agent,
+#     )
+#     expected_content = []
+#     subreddit = reddit.subreddit(subreddit_name)
+
+#     for submission in subreddit.new(limit=100):
+#         expected_content.append(submission.title)
+#         submission.comments.replace_more(limit=None)
+#         for comment in submission.comments.list():
+#             expected_content.append(comment.body)
+
+#     if expected_content == actual_content:
+#         send_results(
+#             "named_entity_recognition_check",
+#             email,
+#             ("Cases passed"),
+#         )
+#     else:
+#         send_results(
+#             "named_entity_recognition_check",
+#             email,
+#             ("Cases failed"),
+#         )
 
 
 # TODO: Upload to the official PyPi repo and try to download in google colab notebook and check if it works
```


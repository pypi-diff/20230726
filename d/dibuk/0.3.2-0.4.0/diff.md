# Comparing `tmp/dibuk-0.3.2.tar.gz` & `tmp/dibuk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dibuk-0.3.2.tar", last modified: Wed Jul 21 17:53:08 2021, max compression
+gzip compressed data, was "dibuk-0.4.0.tar", last modified: Wed Jul 26 21:23:00 2023, max compression
```

## Comparing `dibuk-0.3.2.tar` & `dibuk-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 palosopko   (501) staff       (20)        0 2021-07-21 17:53:08.858110 dibuk-0.3.2/
--rw-r--r--   0 palosopko   (501) staff       (20)      332 2021-07-20 21:41:51.000000 dibuk-0.3.2/.flake8
--rw-r--r--   0 palosopko   (501) staff       (20)     1054 2021-07-20 21:41:51.000000 dibuk-0.3.2/LICENSE
--rw-r--r--   0 palosopko   (501) staff       (20)       71 2021-07-20 21:41:51.000000 dibuk-0.3.2/MANIFEST.in
--rw-r--r--   0 palosopko   (501) staff       (20)     9328 2021-07-21 17:53:08.858327 dibuk-0.3.2/PKG-INFO
--rw-r--r--   0 palosopko   (501) staff       (20)     6953 2021-07-21 17:49:49.000000 dibuk-0.3.2/README.md
-drwxr-xr-x   0 palosopko   (501) staff       (20)        0 2021-07-21 17:53:08.854777 dibuk-0.3.2/dibuk/
--rw-r--r--   0 palosopko   (501) staff       (20)      368 2021-07-21 16:35:21.000000 dibuk-0.3.2/dibuk/__init__.py
--rw-r--r--   0 palosopko   (501) staff       (20)      332 2021-07-21 16:35:21.000000 dibuk-0.3.2/dibuk/error.py
--rw-r--r--   0 palosopko   (501) staff       (20)    12295 2021-07-21 16:35:21.000000 dibuk-0.3.2/dibuk/resource.py
--rw-r--r--   0 palosopko   (501) staff       (20)       18 2021-07-21 17:46:14.000000 dibuk-0.3.2/dibuk/version.py
-drwxr-xr-x   0 palosopko   (501) staff       (20)        0 2021-07-21 17:53:08.856885 dibuk-0.3.2/dibuk.egg-info/
--rw-r--r--   0 palosopko   (501) staff       (20)     9328 2021-07-21 17:53:08.000000 dibuk-0.3.2/dibuk.egg-info/PKG-INFO
--rw-r--r--   0 palosopko   (501) staff       (20)      328 2021-07-21 17:53:08.000000 dibuk-0.3.2/dibuk.egg-info/SOURCES.txt
--rw-r--r--   0 palosopko   (501) staff       (20)        1 2021-07-21 17:53:08.000000 dibuk-0.3.2/dibuk.egg-info/dependency_links.txt
--rw-r--r--   0 palosopko   (501) staff       (20)       36 2021-07-21 17:53:08.000000 dibuk-0.3.2/dibuk.egg-info/requires.txt
--rw-r--r--   0 palosopko   (501) staff       (20)        6 2021-07-21 17:53:08.000000 dibuk-0.3.2/dibuk.egg-info/top_level.txt
--rw-r--r--   0 palosopko   (501) staff       (20)      127 2021-07-20 21:41:51.000000 dibuk-0.3.2/pyproject.toml
--rw-r--r--   0 palosopko   (501) staff       (20)      102 2021-07-21 17:53:08.859226 dibuk-0.3.2/setup.cfg
--rw-r--r--   0 palosopko   (501) staff       (20)     1949 2021-07-20 21:41:51.000000 dibuk-0.3.2/setup.py
-drwxr-xr-x   0 palosopko   (501) staff       (20)        0 2021-07-21 17:53:08.857572 dibuk-0.3.2/tests/
--rw-r--r--   0 palosopko   (501) staff       (20)        0 2021-07-20 21:41:51.000000 dibuk-0.3.2/tests/__init__.py
--rw-r--r--   0 palosopko   (501) staff       (20)      948 2021-07-20 21:41:51.000000 dibuk-0.3.2/tests/test_auth.py
--rw-r--r--   0 palosopko   (501) staff       (20)      788 2021-07-20 21:41:51.000000 dibuk-0.3.2/tox.ini
+drwxr-xr-x   0 palosopko   (501) staff       (20)        0 2023-07-26 21:23:00.248757 dibuk-0.4.0/
+-rw-r--r--   0 palosopko   (501) staff       (20)      332 2021-07-20 21:41:51.000000 dibuk-0.4.0/.flake8
+-rw-r--r--   0 palosopko   (501) staff       (20)     1054 2021-07-20 21:41:51.000000 dibuk-0.4.0/LICENSE
+-rw-r--r--   0 palosopko   (501) staff       (20)       71 2021-07-20 21:41:51.000000 dibuk-0.4.0/MANIFEST.in
+-rw-r--r--   0 palosopko   (501) staff       (20)     7689 2023-07-26 21:23:00.248818 dibuk-0.4.0/PKG-INFO
+-rw-r--r--   0 palosopko   (501) staff       (20)     6648 2023-07-26 21:15:20.000000 dibuk-0.4.0/README.md
+drwxr-xr-x   0 palosopko   (501) staff       (20)        0 2023-07-26 21:23:00.247783 dibuk-0.4.0/dibuk/
+-rw-r--r--   0 palosopko   (501) staff       (20)      323 2023-07-26 08:56:36.000000 dibuk-0.4.0/dibuk/__init__.py
+-rw-r--r--   0 palosopko   (501) staff       (20)      332 2021-07-21 16:35:21.000000 dibuk-0.4.0/dibuk/error.py
+-rw-r--r--   0 palosopko   (501) staff       (20)    11845 2023-07-26 21:13:04.000000 dibuk-0.4.0/dibuk/resource.py
+-rw-r--r--   0 palosopko   (501) staff       (20)       18 2023-07-26 21:21:33.000000 dibuk-0.4.0/dibuk/version.py
+drwxr-xr-x   0 palosopko   (501) staff       (20)        0 2023-07-26 21:23:00.248427 dibuk-0.4.0/dibuk.egg-info/
+-rw-r--r--   0 palosopko   (501) staff       (20)     7689 2023-07-26 21:23:00.000000 dibuk-0.4.0/dibuk.egg-info/PKG-INFO
+-rw-r--r--   0 palosopko   (501) staff       (20)      328 2023-07-26 21:23:00.000000 dibuk-0.4.0/dibuk.egg-info/SOURCES.txt
+-rw-r--r--   0 palosopko   (501) staff       (20)        1 2023-07-26 21:23:00.000000 dibuk-0.4.0/dibuk.egg-info/dependency_links.txt
+-rw-r--r--   0 palosopko   (501) staff       (20)       17 2023-07-26 21:23:00.000000 dibuk-0.4.0/dibuk.egg-info/requires.txt
+-rw-r--r--   0 palosopko   (501) staff       (20)        6 2023-07-26 21:23:00.000000 dibuk-0.4.0/dibuk.egg-info/top_level.txt
+-rw-r--r--   0 palosopko   (501) staff       (20)      127 2021-07-20 21:41:51.000000 dibuk-0.4.0/pyproject.toml
+-rw-r--r--   0 palosopko   (501) staff       (20)      103 2023-07-26 21:23:00.249045 dibuk-0.4.0/setup.cfg
+-rw-r--r--   0 palosopko   (501) staff       (20)     1923 2023-07-26 09:02:36.000000 dibuk-0.4.0/setup.py
+drwxr-xr-x   0 palosopko   (501) staff       (20)        0 2023-07-26 21:23:00.248642 dibuk-0.4.0/tests/
+-rw-r--r--   0 palosopko   (501) staff       (20)        0 2021-07-20 21:41:51.000000 dibuk-0.4.0/tests/__init__.py
+-rw-r--r--   0 palosopko   (501) staff       (20)      947 2023-07-26 21:11:48.000000 dibuk-0.4.0/tests/test_auth.py
+-rw-r--r--   0 palosopko   (501) staff       (20)      822 2023-07-26 21:11:09.000000 dibuk-0.4.0/tox.ini
```

### Comparing `dibuk-0.3.2/LICENSE` & `dibuk-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dibuk-0.3.2/README.md` & `dibuk-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Dibuk Bindings for Python
 
-A Python library for [Dibuk](http://www.dibuk.eu/)'s API v2.1 to work with and order e-books in their catalogue.
+A Python library for [Dibuk](http://www.dibuk.eu/)'s API v2.3 to work with and order e-books in their catalogue.
 
 The bindings allow you to:
 
 1. Get book categories
 2. Get the catalogue of all books
 3. Get single books details with links to previews
 4. Check if given book has been previously bought by a given user
@@ -32,18 +32,14 @@
 ## Usage
 
 First off, you need to require the library and provide authentication information by providing your user handle and shared secret you got from the provider.
 
 	import dibuk
 	dibuk.api_credentials = (123, '00000000000000000000000000000000')
 
-You should also set the client's user agent string. For example when using [Django](https://www.djangoproject.com/) framework you would probably use something like `request.META['HTTP_USER_AGENT']` as the value.
-
-	dibuk.user_agent = 'Mozilla/5.0 (iPhone; CPU iPhone OS 7_1_1 like Mac OS X) AppleWebKit/537.51.2 (KHTML, like Gecko) Version/7.0 Mobile/11D201 Safari/9537.53'
-
 **Getting categories** is accomplished by calling `dibuk.Category.all()`. The method returns dictionary with category IDs as keys and `Category` object as values. `Category` object includes `id`, `parent_id` and `name` of the category.
 
 **Getting catalogue** works analogously to previous method for getting categories. You call it with `dibuk.Catalogue.all()` with optional argument of either type `int` (UNIX timestamp) or `datetime.datetime` noting the time of last synchronization to get only changed books since that time. The method returns dictionary with book IDs as keys and `Book` object as values.
 
 To **get details of a single book**, `dibuk.Book.get()` method should be run with Dibuk's book ID as its argument. Upon success a `Book` object is returned.
 
 `dibuk.Book.available()` should be run **to check whether a book has been previously bought** by a user with Dibuk's book ID and your user identifier that you have used when creating the order.
@@ -82,14 +78,18 @@
 The client library uses Black for code formatting. Code must be formatted with Black before PRs are submitted, otherwise CI will fail. Run the formatter with:
 
 	make fmt
 
 
 ## Changelog
 
+### v0.4.0: 26/07/2023
+
+Use API version 2.3 as the default version.
+
 ### v0.3.2: 21/07/2021
 
 Use API version 2.2 as the default version. Version 2.1 has been deprecated for some time and even though it could have been set from the application, it is better to have sensible defaults.
 
 Refactor getting previews of books including the ability (used internally) to silently ignore exceptions.
 
 ### v0.3.1: 09/01/2021
```

### Comparing `dibuk-0.3.2/dibuk/resource.py` & `dibuk-0.4.0/dibuk/resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import dibuk
 import hmac
 import requests
-import user_agents
 
 from .version import VERSION
 from base64 import b64decode
 from datetime import datetime
 from decimal import Decimal
-from hashlib import md5, sha1
+from hashlib import sha1
 from time import mktime
 from urllib.parse import urlencode
 
 
 class Auth:
     def __init__(self):
         try:
@@ -116,14 +115,16 @@
 
 
 class Book:
     INACTIVE = "inactive"
     ACTIVE = "active"
 
     def __init__(self, data={}):
+        self._source = data
+
         if data.get("status", "u") == "n":
             self.status = self.INACTIVE
         else:
             self.status = self.ACTIVE
 
         self.id = int(data.get("id"))
         self.language = data.get("lang")
@@ -331,34 +332,20 @@
 
         if not isinstance(books, list):
             books = [books]
 
         client = Requestor()
         download_links = {}
 
-        if dibuk.user_agent:
-            user_agent = md5(dibuk.user_agent.encode("utf-8")).hexdigest()
-        else:
-            user_agent = ""
-
-        if dibuk.user_agent_is_mobile:
-            user_agent_is_mobile = dibuk.user_agent_is_mobile
-        else:
-            user_agent_is_mobile = user_agents.parse(
-                dibuk.user_agent
-            ).is_mobile
-
         for book_id in books:
             status, data = client.request(
                 "downloadLinks",
                 [
                     ("book_id", book_id),
                     ("user_id", user_id),
-                    ("for_mobile", 1 if user_agent_is_mobile is True else 0),
-                    ("det", user_agent),
                     ("user_name", user_name),
                     ("user_surname", user_surname),
                     ("user_email", user_email),
                 ],
             )
 
             download_links[book_id] = []
@@ -387,15 +374,17 @@
 
         books = {}
 
         for book in response:
             book_id = int(book["id"])
 
             if include_previews is True and book["status"] != "n":
-                book["previews"] = Book.preview(book_id, ignore_exceptions=True)
+                book["previews"] = Book.preview(
+                    book_id, ignore_exceptions=True
+                )
 
             books[book_id] = Book(book)
 
         return books
 
 
 class Category:
```

### Comparing `dibuk-0.3.2/setup.py` & `dibuk-0.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     description="Dibuk Python Bindings",
     long_description=open("./README.md", "r").read(),
     long_description_content_type="text/markdown",
     author="Palo Sopko",
     author_email="pavol@sopko.sk",
     license="MIT",
     packages=find_packages(exclude=["tests", "tests.*"]),
-    install_requires=["requests >= 2.21.0", "user-agents >= 2.0.0"],
+    install_requires=["requests >= 2.21.0"],
     tests_require=["pytest >= 6.2.1"],
     cmdclass={"test": PyTest},
     project_urls={
         "Bug Tracker": "https://github.com/palosopko/dibuk-python/issues",
         "Source Code": "https://github.com/palosopko/dibuk-python",
     },
-    python_requires=">=3.6.*",
+    python_requires=">=3.6",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
```

### Comparing `dibuk-0.3.2/tests/test_auth.py` & `dibuk-0.4.0/tests/test_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,9 +23,9 @@
 
     def test_signing_data_with_unicode_strings(self):
         dibuk.api_credentials = (
             "client_id",
             "client_secret",
         )
         auth = Auth()
-        signature = auth.sign([("name", u"Gundar-Gošen Ajelet")])
+        signature = auth.sign([("name", "Gundar-Gošen Ajelet")])
         assert signature == "dea946d5dcc7ea93aedcf4709ecc680e7249c2aa"
```

### Comparing `dibuk-0.3.2/tox.ini` & `dibuk-0.4.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 # and then run "tox" from this directory.
 
 [tox]
 envlist = py36,
           py37,
           py38,
           py39,
+          py310,
+          py311,
           pypy3,
           lint
 skip_missing_interpreters = true
 
 [testenv]
 description = run the unit tests under {basepython}
 commands = python setup.py test
 
 [testenv:fmt]
 description = run code formatting using black
-basepython = python3.7
+basepython = python3.9
 deps = black
 commands = black . {posargs}
 
 [testenv:lint]
 description = run static analysis and style check using flake8
-basepython = python3.7
+basepython = python3.9
 deps = flake8
 commands = python -m flake8 --show-source dibuk tests setup.py {posargs}
```


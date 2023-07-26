# Comparing `tmp/aityz-1.0.1.tar.gz` & `tmp/aityz-1.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aityz-1.0.1.tar", last modified: Wed Jul 26 10:57:00 2023, max compression
+gzip compressed data, was "aityz-1.0.1.1.tar", last modified: Wed Jul 26 11:05:30 2023, max compression
```

## Comparing `aityz-1.0.1.tar` & `aityz-1.0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:00.898731 aityz-1.0.1/
--rw-rw-rw-   0        0        0    35821 2023-07-26 03:38:00.000000 aityz-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      369 2023-07-26 10:57:00.897608 aityz-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       99 2023-07-26 03:48:47.000000 aityz-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:00.865032 aityz-1.0.1/aityz/
--rw-rw-rw-   0        0        0        0 2023-07-26 03:36:45.000000 aityz-1.0.1/aityz/__init__.py
--rw-rw-rw-   0        0        0     4135 2023-07-26 10:34:37.000000 aityz-1.0.1/aityz/encryption.py
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:00.889739 aityz-1.0.1/aityz.egg-info/
--rw-rw-rw-   0        0        0      369 2023-07-26 10:57:00.000000 aityz-1.0.1/aityz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-07-26 10:57:00.000000 aityz-1.0.1/aityz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 10:57:00.000000 aityz-1.0.1/aityz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-26 10:57:00.000000 aityz-1.0.1/aityz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-26 10:57:00.000000 aityz-1.0.1/aityz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      625 2023-07-26 03:53:16.000000 aityz-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 10:57:00.898731 aityz-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      399 2023-07-26 10:56:25.000000 aityz-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:05:30.025861 aityz-1.0.1.1/
+-rw-rw-rw-   0        0        0    35821 2023-07-26 03:38:00.000000 aityz-1.0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      449 2023-07-26 11:05:30.023856 aityz-1.0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-26 11:03:01.000000 aityz-1.0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 11:05:29.981777 aityz-1.0.1.1/aityz/
+-rw-rw-rw-   0        0        0       10 2023-07-26 11:05:19.000000 aityz-1.0.1.1/aityz/__init__.py
+-rw-rw-rw-   0        0        0     4066 2023-07-26 11:05:19.000000 aityz-1.0.1.1/aityz/encryption.py
+-rw-rw-rw-   0        0        0      440 2023-07-26 11:05:19.000000 aityz-1.0.1.1/aityz/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:05:30.017768 aityz-1.0.1.1/aityz.egg-info/
+-rw-rw-rw-   0        0        0      449 2023-07-26 11:05:29.000000 aityz-1.0.1.1/aityz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-26 11:05:29.000000 aityz-1.0.1.1/aityz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 11:05:29.000000 aityz-1.0.1.1/aityz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-26 11:05:29.000000 aityz-1.0.1.1/aityz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-26 11:05:29.000000 aityz-1.0.1.1/aityz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      625 2023-07-26 03:53:16.000000 aityz-1.0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 11:05:30.025861 aityz-1.0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-07-26 11:05:28.000000 aityz-1.0.1.1/setup.py
```

### Comparing `aityz-1.0.1/LICENSE` & `aityz-1.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aityz-1.0.1/aityz/encryption.py` & `aityz-1.0.1.1/aityz/encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,8 @@
-import rsa
-
-
-class InitialisationError(Exception):
-    def __init__(self):
-        super().__init__()
-
+from aityz import exceptions
 
 def pad(pad, length=16):
     """
     Pad a given string `pad` with spaces to a specified `length`.
 
     :param pad: The string to be padded.
     :param length: The desired length of the padded string. Default is 16.
@@ -35,15 +29,15 @@
         :param priKey: The path to the file containing the private key in PKCS1 format. Required if fromFile is True.
         :param pubKey: The path to the file containing the public key in PKCS1 format. Required if fromFile is True.
         """
         super().__init__()
         if fromFile:
             print('From File is True, Using priKey and pubKey variables!')
             if priKey is None or pubKey is None:
-                raise InitialisationError
+                raise exceptions.InitialisationError
             else:
                 with open(pubKey, 'rb') as f:
                     pub_key_data = f.read()
                     self.Pub = rsa.PublicKey.load_pkcs1(pub_key_data)
 
                 with open(priKey, 'rb') as f:
                     pri_key_data = f.read()
```

### Comparing `aityz-1.0.1/pyproject.toml` & `aityz-1.0.1.1/pyproject.toml`

 * *Files identical despite different names*


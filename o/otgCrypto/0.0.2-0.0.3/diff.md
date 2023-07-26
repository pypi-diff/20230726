# Comparing `tmp/otgCrypto-0.0.2.tar.gz` & `tmp/otgCrypto-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otgCrypto-0.0.2.tar", last modified: Wed Jul 26 12:28:17 2023, max compression
+gzip compressed data, was "otgCrypto-0.0.3.tar", last modified: Wed Jul 26 12:30:27 2023, max compression
```

## Comparing `otgCrypto-0.0.2.tar` & `otgCrypto-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 12:28:17.800945 otgCrypto-0.0.2/
--rw-rw-rw-   0        0        0    35821 2023-07-26 09:00:53.000000 otgCrypto-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1840 2023-07-26 12:28:17.794426 otgCrypto-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2074 2023-07-26 12:04:21.000000 otgCrypto-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 12:28:17.793427 otgCrypto-0.0.2/otgCrypto.egg-info/
--rw-rw-rw-   0        0        0     1840 2023-07-26 12:28:17.000000 otgCrypto-0.0.2/otgCrypto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-07-26 12:28:17.000000 otgCrypto-0.0.2/otgCrypto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 12:28:17.000000 otgCrypto-0.0.2/otgCrypto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 12:28:17.000000 otgCrypto-0.0.2/otgCrypto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 12:28:17.800945 otgCrypto-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2133 2023-07-26 12:23:36.000000 otgCrypto-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:30:27.015772 otgCrypto-0.0.3/
+-rw-rw-rw-   0        0        0    35821 2023-07-26 09:00:53.000000 otgCrypto-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1901 2023-07-26 12:30:27.010771 otgCrypto-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2074 2023-07-26 12:04:21.000000 otgCrypto-0.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 12:30:27.009771 otgCrypto-0.0.3/otgCrypto.egg-info/
+-rw-rw-rw-   0        0        0     1901 2023-07-26 12:30:26.000000 otgCrypto-0.0.3/otgCrypto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-07-26 12:30:26.000000 otgCrypto-0.0.3/otgCrypto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 12:30:26.000000 otgCrypto-0.0.3/otgCrypto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 12:30:26.000000 otgCrypto-0.0.3/otgCrypto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 12:30:27.016770 otgCrypto-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2127 2023-07-26 12:30:11.000000 otgCrypto-0.0.3/setup.py
```

### Comparing `otgCrypto-0.0.2/LICENSE.txt` & `otgCrypto-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `otgCrypto-0.0.2/PKG-INFO` & `otgCrypto-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: otgCrypto
-Version: 0.0.2
+Version: 0.0.3
+Summary: OTG cryptography is architectured by Tahsin Ahmed.
 Home-page: 
 Author: Tahsin Ahmed
 Keywords: cryptography,encryption,decryption,otg,otg cryptography,one time gamble,one time gamble cryptography
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `otgCrypto-0.0.2/README.txt` & `otgCrypto-0.0.3/README.txt`

 * *Files identical despite different names*

### Comparing `otgCrypto-0.0.2/otgCrypto.egg-info/PKG-INFO` & `otgCrypto-0.0.3/otgCrypto.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: otgCrypto
-Version: 0.0.2
+Version: 0.0.3
+Summary: OTG cryptography is architectured by Tahsin Ahmed.
 Home-page: 
 Author: Tahsin Ahmed
 Keywords: cryptography,encryption,decryption,otg,otg cryptography,one time gamble,one time gamble cryptography
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `otgCrypto-0.0.2/setup.py` & `otgCrypto-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "otgCrypto",
     
-    version = "0.0.2",
+    version = "0.0.3",
     
     author = "Tahsin Ahmed",
 
-    short_description = "OTG cryptography is architectured by Tahsin Ahmed.",
+    description = "OTG cryptography is architectured by Tahsin Ahmed.",
 
     long_description = """The expansion of OTG cryptography is One Time Gamble. 
     It is a hybrid and lightweight cryptographic algorithm that transforms a plaintext into a ciphertext so that secret communication is to be ensured. 
     The original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives wrong password only at once. 
     As a result, it will be so much difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. 
     Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. 
     It is by far impossible for a regular user device to solve the math. It will need super computer to do the computation.
```


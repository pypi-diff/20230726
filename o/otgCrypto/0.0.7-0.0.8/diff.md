# Comparing `tmp/otgCrypto-0.0.7.tar.gz` & `tmp/otgCrypto-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otgCrypto-0.0.7.tar", last modified: Wed Jul 26 13:15:48 2023, max compression
+gzip compressed data, was "otgCrypto-0.0.8.tar", last modified: Wed Jul 26 13:18:01 2023, max compression
```

## Comparing `otgCrypto-0.0.7.tar` & `otgCrypto-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 13:15:48.868020 otgCrypto-0.0.7/
--rw-rw-rw-   0        0        0    35821 2023-07-26 09:00:53.000000 otgCrypto-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0     3432 2023-07-26 13:15:48.862021 otgCrypto-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2765 2023-07-26 13:15:26.000000 otgCrypto-0.0.7/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 13:15:48.861020 otgCrypto-0.0.7/otgCrypto.egg-info/
--rw-rw-rw-   0        0        0     3432 2023-07-26 13:15:48.000000 otgCrypto-0.0.7/otgCrypto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-07-26 13:15:48.000000 otgCrypto-0.0.7/otgCrypto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 13:15:48.000000 otgCrypto-0.0.7/otgCrypto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 13:15:48.000000 otgCrypto-0.0.7/otgCrypto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 13:15:48.868020 otgCrypto-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      865 2023-07-26 13:15:44.000000 otgCrypto-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:18:01.688196 otgCrypto-0.0.8/
+-rw-rw-rw-   0        0        0    35821 2023-07-26 09:00:53.000000 otgCrypto-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     3443 2023-07-26 13:18:01.682160 otgCrypto-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2781 2023-07-26 13:17:44.000000 otgCrypto-0.0.8/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 13:18:01.680161 otgCrypto-0.0.8/otgCrypto.egg-info/
+-rw-rw-rw-   0        0        0     3443 2023-07-26 13:18:01.000000 otgCrypto-0.0.8/otgCrypto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-07-26 13:18:01.000000 otgCrypto-0.0.8/otgCrypto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 13:18:01.000000 otgCrypto-0.0.8/otgCrypto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 13:18:01.000000 otgCrypto-0.0.8/otgCrypto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 13:18:01.689163 otgCrypto-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      865 2023-07-26 13:17:57.000000 otgCrypto-0.0.8/setup.py
```

### Comparing `otgCrypto-0.0.7/LICENSE.txt` & `otgCrypto-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `otgCrypto-0.0.7/PKG-INFO` & `otgCrypto-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otgCrypto
-Version: 0.0.7
+Version: 0.0.8
 Summary: OTG cryptography is architectured by Tahsin Ahmed.
 Home-page: 
 Author: Tahsin Ahmed
 Keywords: cryptography,encryption,decryption,otg,otg cryptography,one time gamble,one time gamble cryptography
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 **OTG Cryptography**
 ====================
 The expansion of OTG cryptography is One Time Gamble. It is a hybrid and lightweight cryptographic system. that transforms a plaintext into a ciphertext so that secret communication is to be ensured.
 
 --------------------
 **Description**
 --------------------
-In the OTG system, original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives wrong password only at once. As a result, it will be so much difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need super computer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware independent cryptography. In conclusion, this new innovation can make a fruitful impact in todayâ€™s security epidemic.
+In the OTG system, the original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives the wrong password only at once. As a result, it will be so much more difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need a supercomputer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware-independent cryptography. In conclusion, this new innovation can make a fruitful impact on the current security epidemic.
 
 ----------------------------
 **Program Utilization**
 ----------------------------
 * A user inputed password.
 * A user inputed secret message.
 * The secret messages is stored in a vault with ChaCha20poly1305 method.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `otgCrypto-0.0.7/README.txt` & `otgCrypto-0.0.8/README.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 **OTG Cryptography**
 ====================
 The expansion of OTG cryptography is One Time Gamble. It is a hybrid and lightweight cryptographic system. that transforms a plaintext into a ciphertext so that secret communication is to be ensured.
 
 --------------------
 **Description**
 --------------------
-In the OTG system, original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives wrong password only at once. As a result, it will be so much difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need super computer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware independent cryptography. In conclusion, this new innovation can make a fruitful impact in today’s security epidemic.
+In the OTG system, the original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives the wrong password only at once. As a result, it will be so much more difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need a supercomputer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware-independent cryptography. In conclusion, this new innovation can make a fruitful impact on the current security epidemic.
 
 ----------------------------
 **Program Utilization**
 ----------------------------
 * A user inputed password.
 * A user inputed secret message.
 * The secret messages is stored in a vault with ChaCha20poly1305 method.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `otgCrypto-0.0.7/otgCrypto.egg-info/PKG-INFO` & `otgCrypto-0.0.8/otgCrypto.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otgCrypto
-Version: 0.0.7
+Version: 0.0.8
 Summary: OTG cryptography is architectured by Tahsin Ahmed.
 Home-page: 
 Author: Tahsin Ahmed
 Keywords: cryptography,encryption,decryption,otg,otg cryptography,one time gamble,one time gamble cryptography
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 **OTG Cryptography**
 ====================
 The expansion of OTG cryptography is One Time Gamble. It is a hybrid and lightweight cryptographic system. that transforms a plaintext into a ciphertext so that secret communication is to be ensured.
 
 --------------------
 **Description**
 --------------------
-In the OTG system, original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives wrong password only at once. As a result, it will be so much difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need super computer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware independent cryptography. In conclusion, this new innovation can make a fruitful impact in todayâ€™s security epidemic.
+In the OTG system, the original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives the wrong password only at once. As a result, it will be so much more difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need a supercomputer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware-independent cryptography. In conclusion, this new innovation can make a fruitful impact on the current security epidemic.
 
 ----------------------------
 **Program Utilization**
 ----------------------------
 * A user inputed password.
 * A user inputed secret message.
 * The secret messages is stored in a vault with ChaCha20poly1305 method.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `otgCrypto-0.0.7/setup.py` & `otgCrypto-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "otgCrypto",
     
-    version = "0.0.7",
+    version = "0.0.8",
     
     author = "Tahsin Ahmed",
 
     description = "OTG cryptography is architectured by Tahsin Ahmed.",
 
     long_description = open("README.txt").read(),
```


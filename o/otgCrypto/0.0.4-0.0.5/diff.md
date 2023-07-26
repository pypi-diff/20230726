# Comparing `tmp/otgCrypto-0.0.4.tar.gz` & `tmp/otgCrypto-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otgCrypto-0.0.4.tar", last modified: Wed Jul 26 12:37:14 2023, max compression
+gzip compressed data, was "otgCrypto-0.0.5.tar", last modified: Wed Jul 26 12:57:19 2023, max compression
```

## Comparing `otgCrypto-0.0.4.tar` & `otgCrypto-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 12:37:14.828637 otgCrypto-0.0.4/
--rw-rw-rw-   0        0        0    35821 2023-07-26 09:00:53.000000 otgCrypto-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     2604 2023-07-26 12:37:14.822636 otgCrypto-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1965 2023-07-26 12:37:00.000000 otgCrypto-0.0.4/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 12:37:14.820639 otgCrypto-0.0.4/otgCrypto.egg-info/
--rw-rw-rw-   0        0        0     2604 2023-07-26 12:37:14.000000 otgCrypto-0.0.4/otgCrypto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-07-26 12:37:14.000000 otgCrypto-0.0.4/otgCrypto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 12:37:14.000000 otgCrypto-0.0.4/otgCrypto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 12:37:14.000000 otgCrypto-0.0.4/otgCrypto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 12:37:14.828637 otgCrypto-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      865 2023-07-26 12:32:17.000000 otgCrypto-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:57:19.761788 otgCrypto-0.0.5/
+-rw-rw-rw-   0        0        0    35821 2023-07-26 09:00:53.000000 otgCrypto-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     2886 2023-07-26 12:57:19.755761 otgCrypto-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2194 2023-07-26 12:57:10.000000 otgCrypto-0.0.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 12:57:19.752762 otgCrypto-0.0.5/otgCrypto.egg-info/
+-rw-rw-rw-   0        0        0     2886 2023-07-26 12:57:19.000000 otgCrypto-0.0.5/otgCrypto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-07-26 12:57:19.000000 otgCrypto-0.0.5/otgCrypto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 12:57:19.000000 otgCrypto-0.0.5/otgCrypto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 12:57:19.000000 otgCrypto-0.0.5/otgCrypto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 12:57:19.761788 otgCrypto-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      906 2023-07-26 12:53:09.000000 otgCrypto-0.0.5/setup.py
```

### Comparing `otgCrypto-0.0.4/LICENSE.txt` & `otgCrypto-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `otgCrypto-0.0.4/PKG-INFO` & `otgCrypto-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 Metadata-Version: 2.1
 Name: otgCrypto
-Version: 0.0.4
-Summary: OTG cryptography is architectured by Tahsin Ahmed.
+Version: 0.0.5
+Summary: OTG cryptography is architectured by Tahsin Ahmed. The expansion of OTG is One Time Gamble.
 Home-page: 
 Author: Tahsin Ahmed
 Keywords: cryptography,encryption,decryption,otg,otg cryptography,one time gamble,one time gamble cryptography
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Natural Language :: English
 License-File: LICENSE.txt
 
-OTG Cryptography
-Introduction
-The expansion of OTG cryptography is One Time Gamble. It is a hybrid and lightweight cryptographic algorithm that transforms a plaintext into a ciphertext so that secret communication is to be ensured. The original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives wrong password only at once. As a result, it will be so much difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need super computer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware independent cryptography. In conclusion, this new innovation can make a fruitful impact in todayâ€™s security epidemic.
+====================
+*OTG Cryptography**
+====================
 
-Ideal applications to use in Government Secret Message, Sensitive Business Communication and Low Computational Powered Device.
+--------------------
+**Introduction**
+--------------------
+OTG is a hybrid and lightweight cryptographic algorithm that transforms a plaintext into a ciphertext so that secret communication is to be ensured. The original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives wrong password only at once. As a result, it will be so much difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need super computer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware independent cryptography. In conclusion, this new innovation can make a fruitful impact in todayâ€™s security epidemic.
 
-This program utilizes:
-A user inputed password.
-A user inputed secret message.
-A hardcoded dictionary of secret messages.
-A dictionary containing manipulated (fake) passwords in addition to the real password.
-A dictionary containing seeds (Seed generator). Seeds are simply pointers that point to the secret message.
-The encryption algorithm: cipher = password XOR key
-The decrpytion algorithm: key = password XOR cipher.
-A try/except block to search for actual password that do exist in the password dictionary.
-The message will be deleted if a user give wrong password.
+----------------------------
+***Program Utilization***
+----------------------------
+* A user inputed password.
+* A user inputed secret message.
+* The secret messages is stored in a vault with ChaCha20poly1305 method.
+* A dictionary is containing manipulated (fake) passwords in addition to the real password.
+* A dictionary containing seeds (Seed generator). Seeds are simply pointers that point to the secret message.
+* The encryption algorithm: ***cipher = password XOR key***.
+* The decrpytion algorithm: ***key = password XOR cipher***.
+* A try/except block to search for actual password that do exist in the password dictionary.
+* The message will be deleted if a user give wrong password.
+
+--------------------------------
+**Ideal Applications To Use**
+--------------------------------
+* Government Secret Message
+* Sensitive Business Communication
+* Low Computational Powered Device
```

### Comparing `otgCrypto-0.0.4/README.txt` & `otgCrypto-0.0.5/README.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,28 @@
-OTG Cryptography
-Introduction
-The expansion of OTG cryptography is One Time Gamble. It is a hybrid and lightweight cryptographic algorithm that transforms a plaintext into a ciphertext so that secret communication is to be ensured. The original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives wrong password only at once. As a result, it will be so much difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need super computer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware independent cryptography. In conclusion, this new innovation can make a fruitful impact in today’s security epidemic.
+====================
+*OTG Cryptography**
+====================
 
-Ideal applications to use in Government Secret Message, Sensitive Business Communication and Low Computational Powered Device.
+--------------------
+**Introduction**
+--------------------
+OTG is a hybrid and lightweight cryptographic algorithm that transforms a plaintext into a ciphertext so that secret communication is to be ensured. The original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives wrong password only at once. As a result, it will be so much difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need super computer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware independent cryptography. In conclusion, this new innovation can make a fruitful impact in today’s security epidemic.
 
-This program utilizes:
-A user inputed password.
-A user inputed secret message.
-A hardcoded dictionary of secret messages.
-A dictionary containing manipulated (fake) passwords in addition to the real password.
-A dictionary containing seeds (Seed generator). Seeds are simply pointers that point to the secret message.
-The encryption algorithm: cipher = password XOR key
-The decrpytion algorithm: key = password XOR cipher.
-A try/except block to search for actual password that do exist in the password dictionary.
-The message will be deleted if a user give wrong password.
+----------------------------
+***Program Utilization***
+----------------------------
+* A user inputed password.
+* A user inputed secret message.
+* The secret messages is stored in a vault with ChaCha20poly1305 method.
+* A dictionary is containing manipulated (fake) passwords in addition to the real password.
+* A dictionary containing seeds (Seed generator). Seeds are simply pointers that point to the secret message.
+* The encryption algorithm: ***cipher = password XOR key***.
+* The decrpytion algorithm: ***key = password XOR cipher***.
+* A try/except block to search for actual password that do exist in the password dictionary.
+* The message will be deleted if a user give wrong password.
+
+--------------------------------
+**Ideal Applications To Use**
+--------------------------------
+* Government Secret Message
+* Sensitive Business Communication
+* Low Computational Powered Device
```

### Comparing `otgCrypto-0.0.4/otgCrypto.egg-info/PKG-INFO` & `otgCrypto-0.0.5/otgCrypto.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 Metadata-Version: 2.1
 Name: otgCrypto
-Version: 0.0.4
-Summary: OTG cryptography is architectured by Tahsin Ahmed.
+Version: 0.0.5
+Summary: OTG cryptography is architectured by Tahsin Ahmed. The expansion of OTG is One Time Gamble.
 Home-page: 
 Author: Tahsin Ahmed
 Keywords: cryptography,encryption,decryption,otg,otg cryptography,one time gamble,one time gamble cryptography
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Natural Language :: English
 License-File: LICENSE.txt
 
-OTG Cryptography
-Introduction
-The expansion of OTG cryptography is One Time Gamble. It is a hybrid and lightweight cryptographic algorithm that transforms a plaintext into a ciphertext so that secret communication is to be ensured. The original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives wrong password only at once. As a result, it will be so much difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need super computer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware independent cryptography. In conclusion, this new innovation can make a fruitful impact in todayâ€™s security epidemic.
+====================
+*OTG Cryptography**
+====================
 
-Ideal applications to use in Government Secret Message, Sensitive Business Communication and Low Computational Powered Device.
+--------------------
+**Introduction**
+--------------------
+OTG is a hybrid and lightweight cryptographic algorithm that transforms a plaintext into a ciphertext so that secret communication is to be ensured. The original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives wrong password only at once. As a result, it will be so much difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need super computer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware independent cryptography. In conclusion, this new innovation can make a fruitful impact in todayâ€™s security epidemic.
 
-This program utilizes:
-A user inputed password.
-A user inputed secret message.
-A hardcoded dictionary of secret messages.
-A dictionary containing manipulated (fake) passwords in addition to the real password.
-A dictionary containing seeds (Seed generator). Seeds are simply pointers that point to the secret message.
-The encryption algorithm: cipher = password XOR key
-The decrpytion algorithm: key = password XOR cipher.
-A try/except block to search for actual password that do exist in the password dictionary.
-The message will be deleted if a user give wrong password.
+----------------------------
+***Program Utilization***
+----------------------------
+* A user inputed password.
+* A user inputed secret message.
+* The secret messages is stored in a vault with ChaCha20poly1305 method.
+* A dictionary is containing manipulated (fake) passwords in addition to the real password.
+* A dictionary containing seeds (Seed generator). Seeds are simply pointers that point to the secret message.
+* The encryption algorithm: ***cipher = password XOR key***.
+* The decrpytion algorithm: ***key = password XOR cipher***.
+* A try/except block to search for actual password that do exist in the password dictionary.
+* The message will be deleted if a user give wrong password.
+
+--------------------------------
+**Ideal Applications To Use**
+--------------------------------
+* Government Secret Message
+* Sensitive Business Communication
+* Low Computational Powered Device
```

### Comparing `otgCrypto-0.0.4/setup.py` & `otgCrypto-0.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "otgCrypto",
     
-    version = "0.0.4",
+    version = "0.0.5",
     
     author = "Tahsin Ahmed",
 
-    description = "OTG cryptography is architectured by Tahsin Ahmed.",
+    description = "OTG cryptography is architectured by Tahsin Ahmed. The expansion of OTG is One Time Gamble.",
 
     long_description = open("README.txt").read(),
     
     keywords = ["cryptography", "encryption", "decryption", "otg", "otg cryptography", "one time gamble", "one time gamble cryptography"],
     
     url = "",
```


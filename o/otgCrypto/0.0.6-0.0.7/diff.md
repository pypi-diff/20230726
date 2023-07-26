# Comparing `tmp/otgCrypto-0.0.6.tar.gz` & `tmp/otgCrypto-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otgCrypto-0.0.6.tar", last modified: Wed Jul 26 13:09:52 2023, max compression
+gzip compressed data, was "otgCrypto-0.0.7.tar", last modified: Wed Jul 26 13:15:48 2023, max compression
```

## Comparing `otgCrypto-0.0.6.tar` & `otgCrypto-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 13:09:52.717726 otgCrypto-0.0.6/
--rw-rw-rw-   0        0        0    35821 2023-07-26 09:00:53.000000 otgCrypto-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0     3115 2023-07-26 13:09:52.711695 otgCrypto-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2456 2023-07-26 13:08:48.000000 otgCrypto-0.0.6/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 13:09:52.710695 otgCrypto-0.0.6/otgCrypto.egg-info/
--rw-rw-rw-   0        0        0     3115 2023-07-26 13:09:52.000000 otgCrypto-0.0.6/otgCrypto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-07-26 13:09:52.000000 otgCrypto-0.0.6/otgCrypto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 13:09:52.000000 otgCrypto-0.0.6/otgCrypto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 13:09:52.000000 otgCrypto-0.0.6/otgCrypto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 13:09:52.717726 otgCrypto-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      865 2023-07-26 13:09:44.000000 otgCrypto-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:15:48.868020 otgCrypto-0.0.7/
+-rw-rw-rw-   0        0        0    35821 2023-07-26 09:00:53.000000 otgCrypto-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     3432 2023-07-26 13:15:48.862021 otgCrypto-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2765 2023-07-26 13:15:26.000000 otgCrypto-0.0.7/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 13:15:48.861020 otgCrypto-0.0.7/otgCrypto.egg-info/
+-rw-rw-rw-   0        0        0     3432 2023-07-26 13:15:48.000000 otgCrypto-0.0.7/otgCrypto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-07-26 13:15:48.000000 otgCrypto-0.0.7/otgCrypto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 13:15:48.000000 otgCrypto-0.0.7/otgCrypto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 13:15:48.000000 otgCrypto-0.0.7/otgCrypto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 13:15:48.868020 otgCrypto-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      865 2023-07-26 13:15:44.000000 otgCrypto-0.0.7/setup.py
```

### Comparing `otgCrypto-0.0.6/LICENSE.txt` & `otgCrypto-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `otgCrypto-0.0.6/PKG-INFO` & `otgCrypto-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otgCrypto
-Version: 0.0.6
+Version: 0.0.7
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
-. The original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives wrong password only at once. As a result, it will be so much difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need super computer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware independent cryptography. In conclusion, this new innovation can make a fruitful impact in todayâ€™s security epidemic.
+In the OTG system, original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives wrong password only at once. As a result, it will be so much difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need super computer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware independent cryptography. In conclusion, this new innovation can make a fruitful impact in todayâ€™s security epidemic.
 
 ----------------------------
 **Program Utilization**
 ----------------------------
 * A user inputed password.
 * A user inputed secret message.
 * The secret messages is stored in a vault with ChaCha20poly1305 method.
@@ -40,12 +40,20 @@
 **Ideal Applications To Use**
 --------------------------------
 * Government Secret Message
 * Sensitive Business Communication
 * Low Computational Powered Device
 
 --------------------------------
+**Caution**
+--------------------------------
+* OTG is a very typo sensitive system.
+* It should be used only for very sensitive work.
+* This cryptography ensures OTC (One Time Chance) method.
+* Message will be deleted if a user give wrong password only at once.
+
+--------------------------------
 **Do You Want To Know Me?**
 --------------------------------
 * **Call**: +8801818832925
 * **Email**: tahsin.ahmed@gbracu.ac.bd
 * **Facebook**: https://www.facebook.com/ahmedinsider
```

### Comparing `otgCrypto-0.0.6/README.txt` & `otgCrypto-0.0.7/README.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 **OTG Cryptography**
 ====================
 The expansion of OTG cryptography is One Time Gamble. It is a hybrid and lightweight cryptographic system. that transforms a plaintext into a ciphertext so that secret communication is to be ensured.
 
 --------------------
 **Description**
 --------------------
-. The original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives wrong password only at once. As a result, it will be so much difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need super computer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware independent cryptography. In conclusion, this new innovation can make a fruitful impact in today’s security epidemic.
+In the OTG system, original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives wrong password only at once. As a result, it will be so much difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need super computer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware independent cryptography. In conclusion, this new innovation can make a fruitful impact in today’s security epidemic.
 
 ----------------------------
 **Program Utilization**
 ----------------------------
 * A user inputed password.
 * A user inputed secret message.
 * The secret messages is stored in a vault with ChaCha20poly1305 method.
@@ -25,12 +25,20 @@
 **Ideal Applications To Use**
 --------------------------------
 * Government Secret Message
 * Sensitive Business Communication
 * Low Computational Powered Device
 
 --------------------------------
+**Caution**
+--------------------------------
+* OTG is a very typo sensitive system.
+* It should be used only for very sensitive work.
+* This cryptography ensures OTC (One Time Chance) method.
+* Message will be deleted if a user give wrong password only at once.
+
+--------------------------------
 **Do You Want To Know Me?**
 --------------------------------
 * **Call**: +8801818832925
 * **Email**: tahsin.ahmed@gbracu.ac.bd
 * **Facebook**: https://www.facebook.com/ahmedinsider
```

### Comparing `otgCrypto-0.0.6/otgCrypto.egg-info/PKG-INFO` & `otgCrypto-0.0.7/otgCrypto.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otgCrypto
-Version: 0.0.6
+Version: 0.0.7
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
-. The original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives wrong password only at once. As a result, it will be so much difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need super computer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware independent cryptography. In conclusion, this new innovation can make a fruitful impact in todayâ€™s security epidemic.
+In the OTG system, original password is hidden under several fake passwords in a vault. Also, these passwords are hashed by bcrypt hash function which is a one-way encryption and cannot be reversed. Moreover, the secret message will be deleted by itself if a user gives wrong password only at once. As a result, it will be so much difficult for a hacker to guess, retrieve and use the password correctly among fake passwords. Furthermore, the key is 128 bits long. So, a hacker needs to go for 2128 = 3.402e+38 possible ways in terms of finding the correct key to decrypt the ciphertext. It is by far impossible for a regular user device to solve the math. It will need super computer to do the computation. However, a low computational powered device (e.g. IOT device) can easily handle it because of its symmetric and stream cipher architecture. Thus, it makes the algorithm lightweight. Also, OTG is a software and hardware independent cryptography. In conclusion, this new innovation can make a fruitful impact in todayâ€™s security epidemic.
 
 ----------------------------
 **Program Utilization**
 ----------------------------
 * A user inputed password.
 * A user inputed secret message.
 * The secret messages is stored in a vault with ChaCha20poly1305 method.
@@ -40,12 +40,20 @@
 **Ideal Applications To Use**
 --------------------------------
 * Government Secret Message
 * Sensitive Business Communication
 * Low Computational Powered Device
 
 --------------------------------
+**Caution**
+--------------------------------
+* OTG is a very typo sensitive system.
+* It should be used only for very sensitive work.
+* This cryptography ensures OTC (One Time Chance) method.
+* Message will be deleted if a user give wrong password only at once.
+
+--------------------------------
 **Do You Want To Know Me?**
 --------------------------------
 * **Call**: +8801818832925
 * **Email**: tahsin.ahmed@gbracu.ac.bd
 * **Facebook**: https://www.facebook.com/ahmedinsider
```

### Comparing `otgCrypto-0.0.6/setup.py` & `otgCrypto-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "otgCrypto",
     
-    version = "0.0.6",
+    version = "0.0.7",
     
     author = "Tahsin Ahmed",
 
     description = "OTG cryptography is architectured by Tahsin Ahmed.",
 
     long_description = open("README.txt").read(),
```


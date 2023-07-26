# Comparing `tmp/pyaadhaar-2.0.0-py3-none-any.whl.zip` & `tmp/pyaadhaar-2.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7256 bytes, number of entries: 8
+Zip file size: 7252 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-26 04:31 pyaadhaar/__init__.py
--rw-rw-r--  2.0 unx    13256 b- defN 23-Jul-26 05:23 pyaadhaar/decode.py
+-rw-rw-r--  2.0 unx    13218 b- defN 23-Jul-26 05:39 pyaadhaar/decode.py
 -rw-rw-r--  2.0 unx      278 b- defN 23-Jul-26 04:51 pyaadhaar/test.py
 -rw-rw-r--  2.0 unx     1902 b- defN 23-Jul-26 04:31 pyaadhaar/utils.py
--rw-rw-r--  2.0 unx     6561 b- defN 23-Jul-26 05:32 pyaadhaar-2.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-26 05:32 pyaadhaar-2.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jul-26 05:32 pyaadhaar-2.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      606 b- defN 23-Jul-26 05:32 pyaadhaar-2.0.0.dist-info/RECORD
-8 files, 22705 bytes uncompressed, 6204 bytes compressed:  72.7%
+-rw-rw-r--  2.0 unx     6561 b- defN 23-Jul-26 05:39 pyaadhaar-2.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-26 05:39 pyaadhaar-2.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jul-26 05:39 pyaadhaar-2.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      606 b- defN 23-Jul-26 05:39 pyaadhaar-2.0.1.dist-info/RECORD
+8 files, 22667 bytes uncompressed, 6200 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: pyaadhaar/test.py
 Comment: 
 
 Filename: pyaadhaar/utils.py
 Comment: 
 
-Filename: pyaadhaar-2.0.0.dist-info/METADATA
+Filename: pyaadhaar-2.0.1.dist-info/METADATA
 Comment: 
 
-Filename: pyaadhaar-2.0.0.dist-info/WHEEL
+Filename: pyaadhaar-2.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyaadhaar-2.0.0.dist-info/top_level.txt
+Filename: pyaadhaar-2.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyaadhaar-2.0.0.dist-info/RECORD
+Filename: pyaadhaar-2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyaadhaar/decode.py

```diff
@@ -2,17 +2,16 @@
 from io import BytesIO
 from PIL import Image, ImageFile
 ImageFile.LOAD_TRUNCATED_IMAGES = True
 import xml.etree.ElementTree as ET
 from io import BytesIO
 import base64
 import zipfile
-import pyaadhaar
 from typing import Union
-
+from . import utils
 
 class AadhaarSecureQr:
     # This is the class for Adhaar Secure Qr code..  In this version of code the data is in encrypted format
     # The special thing of this type of QR is that we can extract the photo of user from the data
     # This class now supports 2022 version of Aadhaar QR codes [version-2]
     # For more information check here : https://103.57.226.101/images/resource/User_manulal_QR_Code_15032019.pdf
 
@@ -167,22 +166,22 @@
         image.load()
         image.save(filepath)
 
     # Verify the email id
     def verifyEmail(self, emailid:str) -> bool:
         if type(emailid) != str:
             raise TypeError("Email id should be string")
-        generated_sha_mail = pyaadhaar.utils.SHAGenerator(emailid, self.data['adhaar_last_digit'])
+        generated_sha_mail = utils.SHAGenerator(emailid, self.data['adhaar_last_digit'])
         return generated_sha_mail == self.sha256hashOfEMail()
 
     # Verify the mobile no  
     def verifyMobileNumber(self, mobileno:str) -> bool:
         if type(mobileno) != str:
             raise TypeError("Mobile number should be string")
-        generated_sha_mobile = pyaadhaar.utils.SHAGenerator(mobileno, self.data['adhaar_last_digit'])
+        generated_sha_mobile = utils.SHAGenerator(mobileno, self.data['adhaar_last_digit'])
         return generated_sha_mobile == self.sha256hashOfMobileNumber()
 
 
 class AadhaarOldQr:
     # This is the class for Adhaar Normal Qr code..  In this version of code the data is in XML v1.0 format
     # For more information check here : https://103.57.226.101/images/resource/User_manulal_QR_Code_15032019.pdf
 
@@ -301,22 +300,22 @@
         # Will save the image of user
         image = self.image()
         image.save(filepath)
 
     # Verify the email id
     def verifyEmail(self, emailid:str) -> bool:
         # Will return True if emailid match with the given email id
-        generated_sha_mail = pyaadhaar.utils.SHAGenerator(
+        generated_sha_mail = utils.SHAGenerator(
             str(emailid)+str(self.passcode), self.data['adhaar_last_digit'])
         if generated_sha_mail == self.sha256hashOfEMail():
             return True
         else:
             return False
 
     # Verify the mobile number
     def verifyMobileNumber(self, mobileno:str) -> bool:
         # Will return True if mobileno match with the given mobile no
-        generated_sha_mobile = pyaadhaar.utils.SHAGenerator(str(mobileno)+str(self.passcode), self.data['adhaar_last_digit'])
+        generated_sha_mobile = utils.SHAGenerator(str(mobileno)+str(self.passcode), self.data['adhaar_last_digit'])
         if generated_sha_mobile == self.sha256hashOfMobileNumber():
             return True
         else:
             return False
```

## Comparing `pyaadhaar-2.0.0.dist-info/METADATA` & `pyaadhaar-2.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaadhaar
-Version: 2.0.0
+Version: 2.0.1
 Summary: This library is built to ease the process of decoding aadhaar QR codes and XML. It supprts old aadhaar QR codes , newly released Secure aadhaar QR codes and also Offline e-KYC XML. This library also can decode QR codes with Opncv. This library bundled with all the features to verify user's Email Id and Mobile Number & also to extract the photo of user. 
 Home-page: https://github.com/Tanmoy741127/pyaadhaar
 Author: Tanmoy Sarkar
 Author-email: ts741127@gmail.com
 License: MIT
 Keywords: software development aadhaar e-kyc verification
 Classifier: Development Status :: 4 - Beta
```

## Comparing `pyaadhaar-2.0.0.dist-info/RECORD` & `pyaadhaar-2.0.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 pyaadhaar/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pyaadhaar/decode.py,sha256=ELn88qzm5mFfTjKTAcMbTZCO--zKlQJjm69lwigozHg,13256
+pyaadhaar/decode.py,sha256=t-u5JPwT3HY7A95SGgSoAUKUb8CDtuD-rXPnfCe0vfU,13218
 pyaadhaar/test.py,sha256=O5e9rx_SCs80vFMGCKBSYTGoJBwYE8Gb3T5vKYUkI8M,278
 pyaadhaar/utils.py,sha256=-YNGx3hi1OtFsDI34KGrFKdE8ewX8w6zCml17xyqWwI,1902
-pyaadhaar-2.0.0.dist-info/METADATA,sha256=xyOGVmJBrgfxeKJqDQD8GpW5MLIP5_CcbP8HcrFv5pM,6561
-pyaadhaar-2.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyaadhaar-2.0.0.dist-info/top_level.txt,sha256=rEyoHsyZ4LocoAvyGyZLBCp7zPbsSx3J_gyVjRZBzBI,10
-pyaadhaar-2.0.0.dist-info/RECORD,,
+pyaadhaar-2.0.1.dist-info/METADATA,sha256=SvU0JvSrGYTkxnobheoslyzcm4MrAc9NRLEM5lx2gBI,6561
+pyaadhaar-2.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyaadhaar-2.0.1.dist-info/top_level.txt,sha256=rEyoHsyZ4LocoAvyGyZLBCp7zPbsSx3J_gyVjRZBzBI,10
+pyaadhaar-2.0.1.dist-info/RECORD,,
```


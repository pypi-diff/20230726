# Comparing `tmp/pyaadhaar-2.0.1-py3-none-any.whl.zip` & `tmp/pyaadhaar-2.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7252 bytes, number of entries: 8
--rw-rw-r--  2.0 unx        0 b- defN 23-Jul-26 04:31 pyaadhaar/__init__.py
--rw-rw-r--  2.0 unx    13218 b- defN 23-Jul-26 05:39 pyaadhaar/decode.py
--rw-rw-r--  2.0 unx      278 b- defN 23-Jul-26 04:51 pyaadhaar/test.py
--rw-rw-r--  2.0 unx     1902 b- defN 23-Jul-26 04:31 pyaadhaar/utils.py
--rw-rw-r--  2.0 unx     6561 b- defN 23-Jul-26 05:39 pyaadhaar-2.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-26 05:39 pyaadhaar-2.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jul-26 05:39 pyaadhaar-2.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      606 b- defN 23-Jul-26 05:39 pyaadhaar-2.0.1.dist-info/RECORD
-8 files, 22667 bytes uncompressed, 6200 bytes compressed:  72.6%
+Zip file size: 7749 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-26 05:50 pyaadhaar/__init__.py
+-rw-rw-r--  2.0 unx    13229 b- defN 23-Jul-26 06:01 pyaadhaar/decode.py
+-rw-rw-r--  2.0 unx     1902 b- defN 23-Jul-26 05:50 pyaadhaar/utils.py
+-rw-rw-r--  2.0 unx     1070 b- defN 23-Jul-26 06:03 pyaadhaar-2.0.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6583 b- defN 23-Jul-26 06:03 pyaadhaar-2.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-26 06:03 pyaadhaar-2.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jul-26 06:03 pyaadhaar-2.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      623 b- defN 23-Jul-26 06:03 pyaadhaar-2.0.2.dist-info/RECORD
+8 files, 23509 bytes uncompressed, 6665 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: pyaadhaar/__init__.py
 Comment: 
 
 Filename: pyaadhaar/decode.py
 Comment: 
 
-Filename: pyaadhaar/test.py
+Filename: pyaadhaar/utils.py
 Comment: 
 
-Filename: pyaadhaar/utils.py
+Filename: pyaadhaar-2.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: pyaadhaar-2.0.1.dist-info/METADATA
+Filename: pyaadhaar-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: pyaadhaar-2.0.1.dist-info/WHEEL
+Filename: pyaadhaar-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pyaadhaar-2.0.1.dist-info/top_level.txt
+Filename: pyaadhaar-2.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pyaadhaar-2.0.1.dist-info/RECORD
+Filename: pyaadhaar-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyaadhaar/decode.py

```diff
@@ -6,15 +6,15 @@
 from io import BytesIO
 import base64
 import zipfile
 from typing import Union
 from . import utils
 
 class AadhaarSecureQr:
-    # This is the class for Adhaar Secure Qr code..  In this version of code the data is in encrypted format
+    # This is the class for Aadhaar Secure Qr code..  In this version of code the data is in encrypted format
     # The special thing of this type of QR is that we can extract the photo of user from the data
     # This class now supports 2022 version of Aadhaar QR codes [version-2]
     # For more information check here : https://103.57.226.101/images/resource/User_manulal_QR_Code_15032019.pdf
 
     def __init__(self, base10encodedstring:str) -> None:
         self.base10encodedstring = base10encodedstring
         self.details = ["version","email_mobile_status","referenceid", "name", "dob", "gender", "careof", "district", "landmark",
@@ -44,16 +44,16 @@
             if self.decompressed_array[i] == 255:
                 self.delimeter.append(i)
 
     # Extracts the information from the decompressed array
     def _extract_info_from_decompressed_array(self) -> None:
         for i in range(len(self.details)):
             self.data[self.details[i]] = self.decompressed_array[self.delimeter[i] + 1:self.delimeter[i+1]].decode("ISO-8859-1")
-        self.data['adhaar_last_4_digit'] = self.data['referenceid'][:4]
-        self.data['adhaar_last_digit'] = self.data['referenceid'][3]
+        self.data['aadhaar_last_4_digit'] = self.data['referenceid'][:4]
+        self.data['aadhaar_last_digit'] = self.data['referenceid'][3]
         # Default values to 'email' and 'mobile
         self.data['email'] = False
         self.data['mobile'] = False
         # Updating the fields of 'email' and 'mobile'
         if int(self.data['email_mobile_status']) in {3, 1}:
             self.data['email'] = True
         if int(self.data['email_mobile_status']) in {3, 2}:
@@ -166,27 +166,27 @@
         image.load()
         image.save(filepath)
 
     # Verify the email id
     def verifyEmail(self, emailid:str) -> bool:
         if type(emailid) != str:
             raise TypeError("Email id should be string")
-        generated_sha_mail = utils.SHAGenerator(emailid, self.data['adhaar_last_digit'])
+        generated_sha_mail = utils.SHAGenerator(emailid, self.data['aadhaar_last_digit'])
         return generated_sha_mail == self.sha256hashOfEMail()
 
     # Verify the mobile no  
     def verifyMobileNumber(self, mobileno:str) -> bool:
         if type(mobileno) != str:
             raise TypeError("Mobile number should be string")
-        generated_sha_mobile = utils.SHAGenerator(mobileno, self.data['adhaar_last_digit'])
+        generated_sha_mobile = utils.SHAGenerator(mobileno, self.data['aadhaar_last_digit'])
         return generated_sha_mobile == self.sha256hashOfMobileNumber()
 
 
 class AadhaarOldQr:
-    # This is the class for Adhaar Normal Qr code..  In this version of code the data is in XML v1.0 format
+    # This is the class for Aadhaar Normal Qr code..  In this version of code the data is in XML v1.0 format
     # For more information check here : https://103.57.226.101/images/resource/User_manulal_QR_Code_15032019.pdf
 
     def __init__(self, qrdata) -> None:
         self.qrdata = qrdata
         self.xmlparser = ET.XMLParser(encoding="utf-8")
         self.parsedxml = ET.fromstring(qrdata, parser=self.xmlparser)
         self.data = self.parsedxml.attrib
@@ -194,15 +194,15 @@
     def decodeddata(self) -> dict:
         # Will return the decoded datas inn dictionary format
         return self.data
 
 
 class AadhaarOfflineXML:
 
-    # This is the class for Adhaar Offline XML
+    # This is the class for Aadhaar Offline XML
     # The special thing of Offline XML is that we can extract the high quality photo of user from the data
     # For more information check here : https://103.57.226.101/images/resource/User_manulal_QR_Code_15032019.pdf
 
     def __init__(self, file:str, passcode:str) -> None:
         # Need to pass the zip file and passcode/sharecode to this function
         self.passcode = passcode
         self.data = {}
@@ -236,16 +236,16 @@
         self.data['location'] = self.root[0][1].attrib['loc']
         self.data['pincode'] = self.root[0][1].attrib['pc']
         self.data['postoffice'] = self.root[0][1].attrib['po']
         self.data['state'] = self.root[0][1].attrib['state']
         self.data['street'] = self.root[0][1].attrib['street']
         self.data['subdistrict'] = self.root[0][1].attrib['subdist']
         self.data['vtc'] = self.root[0][1].attrib['vtc']
-        self.data['adhaar_last_4_digit'] = self.data['referenceid'][0:4]
-        self.data['adhaar_last_digit'] = self.data['referenceid'][3]
+        self.data['aadhaar_last_4_digit'] = self.data['referenceid'][0:4]
+        self.data['aadhaar_last_digit'] = self.data['referenceid'][3]
 
         if self.data['email_mobile_status'] == "0":
             self.data['email'] = False
             self.data['mobile'] = False
         elif self.data['email_mobile_status'] == "1":
             self.data['email'] = True
             self.data['mobile'] = False
@@ -301,21 +301,21 @@
         image = self.image()
         image.save(filepath)
 
     # Verify the email id
     def verifyEmail(self, emailid:str) -> bool:
         # Will return True if emailid match with the given email id
         generated_sha_mail = utils.SHAGenerator(
-            str(emailid)+str(self.passcode), self.data['adhaar_last_digit'])
+            str(emailid)+str(self.passcode), self.data['aadhaar_last_digit'])
         if generated_sha_mail == self.sha256hashOfEMail():
             return True
         else:
             return False
 
     # Verify the mobile number
     def verifyMobileNumber(self, mobileno:str) -> bool:
         # Will return True if mobileno match with the given mobile no
-        generated_sha_mobile = utils.SHAGenerator(str(mobileno)+str(self.passcode), self.data['adhaar_last_digit'])
+        generated_sha_mobile = utils.SHAGenerator(str(mobileno)+str(self.passcode), self.data['aadhaar_last_digit'])
         if generated_sha_mobile == self.sha256hashOfMobileNumber():
             return True
         else:
             return False
```

## Comparing `pyaadhaar-2.0.1.dist-info/METADATA` & `pyaadhaar-2.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pyaadhaar
-Version: 2.0.1
+Version: 2.0.2
 Summary: This library is built to ease the process of decoding aadhaar QR codes and XML. It supprts old aadhaar QR codes , newly released Secure aadhaar QR codes and also Offline e-KYC XML. This library also can decode QR codes with Opncv. This library bundled with all the features to verify user's Email Id and Mobile Number & also to extract the photo of user. 
 Home-page: https://github.com/Tanmoy741127/pyaadhaar
 Author: Tanmoy Sarkar
 Author-email: ts741127@gmail.com
 License: MIT
 Keywords: software development aadhaar e-kyc verification
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers 
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: opencv-python
 Requires-Dist: Pillow
 Requires-Dist: pylibjpeg
 Requires-Dist: pylibjpeg-openjpeg
 Requires-Dist: python-dateutil
 Requires-Dist: pytz
```

## Comparing `pyaadhaar-2.0.1.dist-info/RECORD` & `pyaadhaar-2.0.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 pyaadhaar/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pyaadhaar/decode.py,sha256=t-u5JPwT3HY7A95SGgSoAUKUb8CDtuD-rXPnfCe0vfU,13218
-pyaadhaar/test.py,sha256=O5e9rx_SCs80vFMGCKBSYTGoJBwYE8Gb3T5vKYUkI8M,278
+pyaadhaar/decode.py,sha256=UJ9QNZpQFVctBiQWPsguekRuWEMKFq3RyQ2vmEZgbYY,13229
 pyaadhaar/utils.py,sha256=-YNGx3hi1OtFsDI34KGrFKdE8ewX8w6zCml17xyqWwI,1902
-pyaadhaar-2.0.1.dist-info/METADATA,sha256=SvU0JvSrGYTkxnobheoslyzcm4MrAc9NRLEM5lx2gBI,6561
-pyaadhaar-2.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyaadhaar-2.0.1.dist-info/top_level.txt,sha256=rEyoHsyZ4LocoAvyGyZLBCp7zPbsSx3J_gyVjRZBzBI,10
-pyaadhaar-2.0.1.dist-info/RECORD,,
+pyaadhaar-2.0.2.dist-info/LICENSE,sha256=lDLqnHyNi9VRrRkTT_-j-2Zgp5KBTzp2yJ-F5nZ9IkY,1070
+pyaadhaar-2.0.2.dist-info/METADATA,sha256=WKuKrja1QPGduh0L5L5yy5s7Hkd7XMMdBTSjDKTb-kk,6583
+pyaadhaar-2.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyaadhaar-2.0.2.dist-info/top_level.txt,sha256=rEyoHsyZ4LocoAvyGyZLBCp7zPbsSx3J_gyVjRZBzBI,10
+pyaadhaar-2.0.2.dist-info/RECORD,,
```


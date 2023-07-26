# Comparing `tmp/pytbai-1.3.6.tar.gz` & `tmp/pytbai-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytbai-1.3.6.tar", last modified: Fri Jul  7 12:07:58 2023, max compression
+gzip compressed data, was "pytbai-1.3.7.tar", last modified: Wed Jul 26 14:35:02 2023, max compression
```

## Comparing `pytbai-1.3.6.tar` & `pytbai-1.3.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 12:07:58.463699 pytbai-1.3.6/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1758 2023-07-07 12:07:57.000000 pytbai-1.3.6/CHANGELOG.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-07 12:07:57.000000 pytbai-1.3.6/CODE_OF_CONDUCT.md
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-07 12:07:57.000000 pytbai-1.3.6/LICENSE
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2023-07-07 12:07:57.000000 pytbai-1.3.6/MANIFEST.in
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-07 12:07:57.000000 pytbai-1.3.6/Makefile
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-07 12:07:58.463699 pytbai-1.3.6/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2023-07-07 12:07:57.000000 pytbai-1.3.6/README.md
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 12:07:58.459699 pytbai-1.3.6/pytbai/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2023-07-07 12:07:57.000000 pytbai-1.3.6/pytbai/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    10901 2023-07-07 12:07:57.000000 pytbai-1.3.6/pytbai/core.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2992 2023-07-07 12:07:57.000000 pytbai-1.3.6/pytbai/definitions.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 12:07:58.459699 pytbai-1.3.6/pytbai/templates/
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 12:07:58.459699 pytbai-1.3.6/pytbai/templates/PDF/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 12:07:57.000000 pytbai-1.3.6/pytbai/templates/PDF/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-07 12:07:57.000000 pytbai-1.3.6/pytbai/templates/PDF/ticketbai.css
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-07 12:07:57.000000 pytbai-1.3.6/pytbai/templates/PDF/ticketbai.html
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 12:07:58.459699 pytbai-1.3.6/pytbai/templates/XML/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 12:07:57.000000 pytbai-1.3.6/pytbai/templates/XML/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-07 12:07:57.000000 pytbai-1.3.6/pytbai/templates/XML/tbai_structure.xml
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 12:07:58.459699 pytbai-1.3.6/pytbai/templates/XSD/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-07 12:07:57.000000 pytbai-1.3.6/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 12:07:57.000000 pytbai-1.3.6/pytbai/templates/XSD/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-07 12:07:57.000000 pytbai-1.3.6/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 12:07:57.000000 pytbai-1.3.6/pytbai/templates/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 12:07:58.459699 pytbai-1.3.6/pytbai/utils/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 12:07:57.000000 pytbai-1.3.6/pytbai/utils/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2023-07-07 12:07:57.000000 pytbai-1.3.6/pytbai/utils/crypto.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-07 12:07:57.000000 pytbai-1.3.6/pytbai/utils/pdf.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4524 2023-07-07 12:07:57.000000 pytbai-1.3.6/pytbai/utils/xml.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 12:07:58.459699 pytbai-1.3.6/pytbai.egg-info/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-07 12:07:58.000000 pytbai-1.3.6/pytbai.egg-info/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      839 2023-07-07 12:07:58.000000 pytbai-1.3.6/pytbai.egg-info/SOURCES.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-07 12:07:58.000000 pytbai-1.3.6/pytbai.egg-info/dependency_links.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-07 12:07:58.000000 pytbai-1.3.6/pytbai.egg-info/top_level.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-07 12:07:57.000000 pytbai-1.3.6/requirements.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-07 12:07:58.463699 pytbai-1.3.6/setup.cfg
--rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1037 2023-07-07 12:07:57.000000 pytbai-1.3.6/setup.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 12:07:58.459699 pytbai-1.3.6/tests/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 12:07:57.000000 pytbai-1.3.6/tests/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 12:07:58.459699 pytbai-1.3.6/tests/certs/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2023-07-07 12:07:57.000000 pytbai-1.3.6/tests/certs/cert.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2023-07-07 12:07:57.000000 pytbai-1.3.6/tests/certs/cert_for_tests.p12
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2023-07-07 12:07:57.000000 pytbai-1.3.6/tests/certs/key.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-07 12:07:57.000000 pytbai-1.3.6/tests/context.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-07 12:07:58.463699 pytbai-1.3.6/tests/data/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2997 2023-07-07 12:07:57.000000 pytbai-1.3.6/tests/data/tbai_json.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2023-07-07 12:07:57.000000 pytbai-1.3.6/tests/test_basic.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2071 2023-07-26 14:35:01.000000 pytbai-1.3.7/CHANGELOG.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-26 14:35:01.000000 pytbai-1.3.7/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-26 14:35:01.000000 pytbai-1.3.7/LICENSE
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2023-07-26 14:35:01.000000 pytbai-1.3.7/MANIFEST.in
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-26 14:35:01.000000 pytbai-1.3.7/Makefile
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-26 14:35:02.905526 pytbai-1.3.7/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2023-07-26 14:35:01.000000 pytbai-1.3.7/README.md
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.901527 pytbai-1.3.7/pytbai/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    11073 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/core.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3186 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/definitions.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/pytbai/templates/
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/pytbai/templates/PDF/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/PDF/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/PDF/ticketbai.css
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/PDF/ticketbai.html
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/pytbai/templates/XML/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/XML/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/XML/tbai_structure.xml
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/pytbai/templates/XSD/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/XSD/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/pytbai/utils/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/utils/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/utils/crypto.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/utils/pdf.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4542 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/utils/xml.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/pytbai.egg-info/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-26 14:35:02.000000 pytbai-1.3.7/pytbai.egg-info/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      839 2023-07-26 14:35:02.000000 pytbai-1.3.7/pytbai.egg-info/SOURCES.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-26 14:35:02.000000 pytbai-1.3.7/pytbai.egg-info/dependency_links.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-26 14:35:02.000000 pytbai-1.3.7/pytbai.egg-info/top_level.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-26 14:35:01.000000 pytbai-1.3.7/requirements.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-26 14:35:02.905526 pytbai-1.3.7/setup.cfg
+-rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1037 2023-07-26 14:35:01.000000 pytbai-1.3.7/setup.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/tests/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:01.000000 pytbai-1.3.7/tests/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/tests/certs/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2023-07-26 14:35:01.000000 pytbai-1.3.7/tests/certs/cert.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2023-07-26 14:35:01.000000 pytbai-1.3.7/tests/certs/cert_for_tests.p12
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2023-07-26 14:35:01.000000 pytbai-1.3.7/tests/certs/key.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-26 14:35:01.000000 pytbai-1.3.7/tests/context.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/tests/data/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3042 2023-07-26 14:35:01.000000 pytbai-1.3.7/tests/data/tbai_json.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2023-07-26 14:35:01.000000 pytbai-1.3.7/tests/test_basic.py
```

### Comparing `pytbai-1.3.6/CHANGELOG.txt` & `pytbai-1.3.7/CHANGELOG.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+1.3.7 (2023-07-26)
+------------------
+
+- DEV and PROD urls configurable [Urtzi Odriozola <uodriozola@codesyntax.com>]
+
+- Update core.py [Urtzi Odriozola <uodriozola@codesyntax.com>]
+
+-  [Urtzi Odriozola <uodriozola@codesyntax.com>]
+
+- ResponseXML in string format [Urtzi Odriozola <uodriozola@codesyntax.com>]
+
+
+
 1.3.6 (2023-07-07)
 ------------------
 
 - Decimal cast [Urtzi Odriozola <uodriozola@codesyntax.com>]
 
 - get_json returns total_amount + default line values in Decimal [Urtzi Odriozola <uodriozola@codesyntax.com>]
```

### Comparing `pytbai-1.3.6/LICENSE` & `pytbai-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.6/PKG-INFO` & `pytbai-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.3.6
+Version: 1.3.7
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.3.6/README.md` & `pytbai-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.6/pytbai/core.py` & `pytbai-1.3.7/pytbai/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,23 +35,24 @@
     def __init__(
         self,
         entity_id,
         name,
         territory=GIPUZKOA,
         multi_recipient=N,
         external_invoice=N,
+        env="DEV",
     ):
         self.entity_id = entity_id
         self.name = name
         if not territory:
-            self.authority_api = GIPUZKOA["invoice"]
-            self.qr_api = GIPUZKOA["qr"]
+            self.authority_api = GIPUZKOA[env]["invoice"]
+            self.qr_api = GIPUZKOA[env]["qr"]
         elif territory in AUTHORITY_APIS:
-            self.authority_api = AUTHORITY_APIS[territory]["invoice"]
-            self.qr_api = AUTHORITY_APIS[territory]["qr"]
+            self.authority_api = AUTHORITY_APIS[territory][env]["invoice"]
+            self.qr_api = AUTHORITY_APIS[territory][env]["qr"]
         else:
             raise ValueError(
                 "Not a valid territory. Options are: Araba, Bizkaia, Gipuzkoa."
             )
         if multi_recipient in L3:
             self.multi_recipient = multi_recipient
         else:
@@ -278,16 +279,18 @@
     def default(self, o):
         if isinstance(o, Decimal):
             return float(o)
         return super().default(o)
 
 
 class TBai:
-    def __init__(self, config, version=TICKETBAI_ACTUAL_VERSION):
+    def __init__(self, config, version=TICKETBAI_ACTUAL_VERSION, env="DEV"):
         self.version = version
+        self.env = env
+        config["subject"].update({"env": env})
         self.subject = Subject(**config["subject"])
         self.software = Software(**config["software"])
 
     def create_invoice(
         self,
         serial_code,
         num,
@@ -307,16 +310,16 @@
             expedition_time=expedition_time
             or datetime.now().time().strftime("%H:%M:%S"),
             transaction_date=transaction_date
             or datetime.now().date().isoformat(),
         )
         return invoice
 
-    def sign_and_send(self, invoice, p12_path, password):
-        xml = build_xml(self, invoice)
+    def sign_and_send(self, invoice, p12_path, password, pre_invoice=None):
+        xml = build_xml(self, invoice, pre_invoice)
         key, cert = get_keycert_from_p12(p12_path, password.encode("utf-8"))
         signed_xml = sign_xml(xml, key, cert)
         if not validate_xml(signed_xml):
             return (None, None)
 
         key_file = tempfile.NamedTemporaryFile()
         key_file.write(key)
@@ -345,29 +348,29 @@
             "ResponseXML": None,
         }
         if response.ok:
             response_xml = etree.fromstring(response.content)
             state = response_xml.find(".//Estado").text
             if state == "01":
                 logger.error("XML not accepted")
-                result_json["ResponseXML"] = response_xml
+                result_json["ResponseXML"] = response.content
                 return result_json
             result_json["TBAI_ID"] = response_xml.find(
                 ".//IdentificadorTBAI"
             ).text
             result_json["CSV"] = response_xml.find(".//CSV").text
             result_json["SignedXML"] = etree.tostring(signed_xml).decode(
                 "utf-8"
             )
             return result_json
         logger.error("API connection error")
         return result_json
 
     def get_json(self, invoice=None):
-        tbai_json = {"version": self.version}
+        tbai_json = {"version": self.version, "env": self.env}
         if self.subject:
             tbai_json["subject"] = self.subject.get_dict()
         if invoice:
             tbai_json["invoice"] = invoice.get_dict()
         if self.software:
             tbai_json["software"] = self.software.get_dict()
         return json.dumps(tbai_json, cls=TBaiEncoder)
```

### Comparing `pytbai-1.3.6/pytbai/definitions.py` & `pytbai-1.3.7/pytbai/definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,22 @@
 DEFAULT_VAT_RATE = Decimal("21")
 
 GIPUZKOA = "Gipuzkoa"
 AUTHORITY_APIS = {
     "Araba": "",
     "Bizkaia": "",
     GIPUZKOA: {
-        "invoice": "https://tbai-z.prep.gipuzkoa.eus/sarrerak/alta",
-        "qr": "https://tbai.egoitza.gipuzkoa.eus/qr",
+        "DEV": {
+            "invoice": "https://tbai-z.prep.gipuzkoa.eus/sarrerak/alta",
+            "qr": "https://tbai.prep.gipuzkoa.eus/qr",
+        },
+        "PROD": {
+            "invoice": "https://tbai.egoitza.gipuzkoa.eus/sarrerak/alta",
+            "qr": "https://tbai.egoitza.gipuzkoa.eus/qr",
+        },
     },
 }
 
 S = "S"  # Bai
 N = "N"  # Ez
 
 # Hainbat hartzaile
```

### Comparing `pytbai-1.3.6/pytbai/templates/PDF/ticketbai.html` & `pytbai-1.3.7/pytbai/templates/PDF/ticketbai.html`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.6/pytbai/templates/XML/tbai_structure.xml` & `pytbai-1.3.7/pytbai/templates/XML/tbai_structure.xml`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.6/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd` & `pytbai-1.3.7/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.6/pytbai/templates/XSD/ticketBaiV1-2-1.xsd` & `pytbai-1.3.7/pytbai/templates/XSD/ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.6/pytbai/utils/pdf.py` & `pytbai-1.3.7/pytbai/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.6/pytbai/utils/xml.py` & `pytbai-1.3.7/pytbai/utils/xml.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     XAdESSignaturePolicy,
     XAdESDataObjectFormat,
 )
 
 logger = logging.getLogger("pytbai")
 
 
-def build_xml(tbai, invoice):
+def build_xml(tbai, invoice, pre_invoice=None):
     path = os.path.dirname(pytbai.__file__)
     structure_file = os.path.join(path, "templates/XML/tbai_structure.xml")
     with open(structure_file, "r") as file:
         template = file.read()
     temp = Template(template)
 
     expedition_date = datetime.strptime(
```

### Comparing `pytbai-1.3.6/pytbai.egg-info/PKG-INFO` & `pytbai-1.3.7/pytbai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.3.6
+Version: 1.3.7
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.3.6/pytbai.egg-info/SOURCES.txt` & `pytbai-1.3.7/pytbai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.6/setup.py` & `pytbai-1.3.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="pytbai",
-    version="1.3.6",
+    version="1.3.7",
     description=(
         "pytbai allows to create, manage and send TicketBai invoices to the"
         " Basque tax authorities"
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Urtzi Odriozola",
```

### Comparing `pytbai-1.3.6/tests/certs/cert.pem` & `pytbai-1.3.7/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.6/tests/certs/cert_for_tests.p12` & `pytbai-1.3.7/tests/certs/cert_for_tests.p12`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.6/tests/certs/key.pem` & `pytbai-1.3.7/tests/certs/key.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.6/tests/data/tbai_json.py` & `pytbai-1.3.7/tests/data/tbai_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 TBAI_JSON = {
     "version": "1.2",
+    "env": "DEV",
     "subject": {
         "entity_id": "99999974E",
         "name": "REPRESENTANTESPJ FICTICIO",
         "authority_api": "https://tbai-z.prep.gipuzkoa.eus/sarrerak/alta",
-        "qr_api": "https://tbai.egoitza.gipuzkoa.eus/qr",
+        "qr_api": "https://tbai.prep.gipuzkoa.eus/qr",
         "multi_recipient": "N",
         "external_invoice": "N",
     },
     "software": {
         "license": "TBAIGIPRE00000000501",
         "dev_entity": "P2000000F",
         "soft_name": "FAKTURABAI",
         "soft_version": "1.0",
     },
 }
 
 TBAI_INVOICE_JSON = {
     "version": "1.2",
+    "env": "DEV",
     "subject": {
         "entity_id": "99999974E",
         "name": "REPRESENTANTESPJ FICTICIO",
         "authority_api": "https://tbai-z.prep.gipuzkoa.eus/sarrerak/alta",
-        "qr_api": "https://tbai.egoitza.gipuzkoa.eus/qr",
+        "qr_api": "https://tbai.prep.gipuzkoa.eus/qr",
         "multi_recipient": "N",
         "external_invoice": "N",
     },
     "invoice": {
         "serial_code": "TB-2021-S",
         "num": 1,
         "description": "Primera factura",
@@ -45,19 +47,20 @@
         "soft_name": "FAKTURABAI",
         "soft_version": "1.0",
     },
 }
 
 TBAI_INVOICE_LINES_JSON = {
     "version": "1.2",
+    "env": "DEV",
     "subject": {
         "entity_id": "99999974E",
         "name": "REPRESENTANTESPJ FICTICIO",
         "authority_api": "https://tbai-z.prep.gipuzkoa.eus/sarrerak/alta",
-        "qr_api": "https://tbai.egoitza.gipuzkoa.eus/qr",
+        "qr_api": "https://tbai.prep.gipuzkoa.eus/qr",
         "multi_recipient": "N",
         "external_invoice": "N",
     },
     "invoice": {
         "serial_code": "TB-2021-S",
         "num": 1,
         "description": "Primera factura",
```

### Comparing `pytbai-1.3.6/tests/test_basic.py` & `pytbai-1.3.7/tests/test_basic.py`

 * *Files identical despite different names*


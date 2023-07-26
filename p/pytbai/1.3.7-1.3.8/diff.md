# Comparing `tmp/pytbai-1.3.7.tar.gz` & `tmp/pytbai-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytbai-1.3.7.tar", last modified: Wed Jul 26 14:35:02 2023, max compression
+gzip compressed data, was "pytbai-1.3.8.tar", last modified: Wed Jul 26 15:25:11 2023, max compression
```

## Comparing `pytbai-1.3.7.tar` & `pytbai-1.3.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2071 2023-07-26 14:35:01.000000 pytbai-1.3.7/CHANGELOG.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-26 14:35:01.000000 pytbai-1.3.7/CODE_OF_CONDUCT.md
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-26 14:35:01.000000 pytbai-1.3.7/LICENSE
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2023-07-26 14:35:01.000000 pytbai-1.3.7/MANIFEST.in
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-26 14:35:01.000000 pytbai-1.3.7/Makefile
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-26 14:35:02.905526 pytbai-1.3.7/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2023-07-26 14:35:01.000000 pytbai-1.3.7/README.md
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.901527 pytbai-1.3.7/pytbai/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    11073 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/core.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3186 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/definitions.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/pytbai/templates/
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/pytbai/templates/PDF/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/PDF/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/PDF/ticketbai.css
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/PDF/ticketbai.html
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/pytbai/templates/XML/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/XML/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/XML/tbai_structure.xml
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/pytbai/templates/XSD/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/XSD/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/templates/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/pytbai/utils/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/utils/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/utils/crypto.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/utils/pdf.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4542 2023-07-26 14:35:01.000000 pytbai-1.3.7/pytbai/utils/xml.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/pytbai.egg-info/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-26 14:35:02.000000 pytbai-1.3.7/pytbai.egg-info/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      839 2023-07-26 14:35:02.000000 pytbai-1.3.7/pytbai.egg-info/SOURCES.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-26 14:35:02.000000 pytbai-1.3.7/pytbai.egg-info/dependency_links.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-26 14:35:02.000000 pytbai-1.3.7/pytbai.egg-info/top_level.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-26 14:35:01.000000 pytbai-1.3.7/requirements.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-26 14:35:02.905526 pytbai-1.3.7/setup.cfg
--rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1037 2023-07-26 14:35:01.000000 pytbai-1.3.7/setup.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/tests/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:01.000000 pytbai-1.3.7/tests/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/tests/certs/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2023-07-26 14:35:01.000000 pytbai-1.3.7/tests/certs/cert.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2023-07-26 14:35:01.000000 pytbai-1.3.7/tests/certs/cert_for_tests.p12
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2023-07-26 14:35:01.000000 pytbai-1.3.7/tests/certs/key.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-26 14:35:01.000000 pytbai-1.3.7/tests/context.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 14:35:02.905526 pytbai-1.3.7/tests/data/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3042 2023-07-26 14:35:01.000000 pytbai-1.3.7/tests/data/tbai_json.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2023-07-26 14:35:01.000000 pytbai-1.3.7/tests/test_basic.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.351533 pytbai-1.3.8/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2175 2023-07-26 15:25:08.000000 pytbai-1.3.8/CHANGELOG.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-07-26 15:25:08.000000 pytbai-1.3.8/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-07-26 15:25:08.000000 pytbai-1.3.8/LICENSE
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2023-07-26 15:25:08.000000 pytbai-1.3.8/MANIFEST.in
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-26 15:25:08.000000 pytbai-1.3.8/Makefile
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-26 15:25:11.351533 pytbai-1.3.8/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2023-07-26 15:25:08.000000 pytbai-1.3.8/README.md
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.335533 pytbai-1.3.8/pytbai/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    11073 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/core.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/definitions.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.339532 pytbai-1.3.8/pytbai/templates/
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.343532 pytbai-1.3.8/pytbai/templates/PDF/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/PDF/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/PDF/ticketbai.css
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/PDF/ticketbai.html
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.343532 pytbai-1.3.8/pytbai/templates/XML/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/XML/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/XML/tbai_structure.xml
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.343532 pytbai-1.3.8/pytbai/templates/XSD/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/XSD/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/templates/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.347532 pytbai-1.3.8/pytbai/utils/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/utils/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/utils/crypto.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/utils/pdf.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4542 2023-07-26 15:25:08.000000 pytbai-1.3.8/pytbai/utils/xml.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.339532 pytbai-1.3.8/pytbai.egg-info/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3642 2023-07-26 15:25:11.000000 pytbai-1.3.8/pytbai.egg-info/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      839 2023-07-26 15:25:11.000000 pytbai-1.3.8/pytbai.egg-info/SOURCES.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-07-26 15:25:11.000000 pytbai-1.3.8/pytbai.egg-info/dependency_links.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-07-26 15:25:11.000000 pytbai-1.3.8/pytbai.egg-info/top_level.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-07-26 15:25:08.000000 pytbai-1.3.8/requirements.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-07-26 15:25:11.351533 pytbai-1.3.8/setup.cfg
+-rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1037 2023-07-26 15:25:08.000000 pytbai-1.3.8/setup.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.347532 pytbai-1.3.8/tests/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:08.000000 pytbai-1.3.8/tests/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.351533 pytbai-1.3.8/tests/certs/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2023-07-26 15:25:08.000000 pytbai-1.3.8/tests/certs/cert.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2023-07-26 15:25:08.000000 pytbai-1.3.8/tests/certs/cert_for_tests.p12
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2023-07-26 15:25:08.000000 pytbai-1.3.8/tests/certs/key.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-07-26 15:25:08.000000 pytbai-1.3.8/tests/context.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-07-26 15:25:11.351533 pytbai-1.3.8/tests/data/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3042 2023-07-26 15:25:08.000000 pytbai-1.3.8/tests/data/tbai_json.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2023-07-26 15:25:08.000000 pytbai-1.3.8/tests/test_basic.py
```

### Comparing `pytbai-1.3.7/CHANGELOG.txt` & `pytbai-1.3.8/CHANGELOG.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+1.3.8 (2023-07-26)
+------------------
+
+- DEV url fixed [Urtzi Odriozola <uodriozola@codesyntax.com>]
+
+
+
 1.3.7 (2023-07-26)
 ------------------
 
 - DEV and PROD urls configurable [Urtzi Odriozola <uodriozola@codesyntax.com>]
 
 - Update core.py [Urtzi Odriozola <uodriozola@codesyntax.com>]
```

### Comparing `pytbai-1.3.7/LICENSE` & `pytbai-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.7/PKG-INFO` & `pytbai-1.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.3.7
+Version: 1.3.8
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.3.7/README.md` & `pytbai-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.7/pytbai/core.py` & `pytbai-1.3.8/pytbai/core.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.7/pytbai/definitions.py` & `pytbai-1.3.8/pytbai/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 GIPUZKOA = "Gipuzkoa"
 AUTHORITY_APIS = {
     "Araba": "",
     "Bizkaia": "",
     GIPUZKOA: {
         "DEV": {
             "invoice": "https://tbai-z.prep.gipuzkoa.eus/sarrerak/alta",
-            "qr": "https://tbai.prep.gipuzkoa.eus/qr",
+            "qr": "https://tbai.prep.gipuzkoa.eus/qr/",
         },
         "PROD": {
             "invoice": "https://tbai.egoitza.gipuzkoa.eus/sarrerak/alta",
             "qr": "https://tbai.egoitza.gipuzkoa.eus/qr",
         },
     },
 }
```

### Comparing `pytbai-1.3.7/pytbai/templates/PDF/ticketbai.html` & `pytbai-1.3.8/pytbai/templates/PDF/ticketbai.html`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.7/pytbai/templates/XML/tbai_structure.xml` & `pytbai-1.3.8/pytbai/templates/XML/tbai_structure.xml`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.7/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd` & `pytbai-1.3.8/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.7/pytbai/templates/XSD/ticketBaiV1-2-1.xsd` & `pytbai-1.3.8/pytbai/templates/XSD/ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.7/pytbai/utils/pdf.py` & `pytbai-1.3.8/pytbai/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.7/pytbai/utils/xml.py` & `pytbai-1.3.8/pytbai/utils/xml.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.7/pytbai.egg-info/PKG-INFO` & `pytbai-1.3.8/pytbai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.3.7
+Version: 1.3.8
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.3.7/pytbai.egg-info/SOURCES.txt` & `pytbai-1.3.8/pytbai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.7/setup.py` & `pytbai-1.3.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="pytbai",
-    version="1.3.7",
+    version="1.3.8",
     description=(
         "pytbai allows to create, manage and send TicketBai invoices to the"
         " Basque tax authorities"
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Urtzi Odriozola",
```

### Comparing `pytbai-1.3.7/tests/certs/cert.pem` & `pytbai-1.3.8/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.7/tests/certs/cert_for_tests.p12` & `pytbai-1.3.8/tests/certs/cert_for_tests.p12`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.7/tests/certs/key.pem` & `pytbai-1.3.8/tests/certs/key.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.7/tests/data/tbai_json.py` & `pytbai-1.3.8/tests/data/tbai_json.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.3.7/tests/test_basic.py` & `pytbai-1.3.8/tests/test_basic.py`

 * *Files identical despite different names*


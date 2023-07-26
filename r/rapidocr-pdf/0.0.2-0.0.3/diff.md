# Comparing `tmp/rapidocr_pdf-0.0.2-py3-none-any.whl.zip` & `tmp/rapidocr_pdf-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8486 bytes, number of entries: 8
--rw-r--r--  2.0 unx      124 b- defN 23-Apr-27 02:38 rapidocr_pdf/__init__.py
--rw-r--r--  2.0 unx     4090 b- defN 23-Apr-27 02:38 rapidocr_pdf/main.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-27 02:38 rapidocr_pdf-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2714 b- defN 23-Apr-27 02:38 rapidocr_pdf-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 02:38 rapidocr_pdf-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       57 b- defN 23-Apr-27 02:38 rapidocr_pdf-0.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Apr-27 02:38 rapidocr_pdf-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      669 b- defN 23-Apr-27 02:38 rapidocr_pdf-0.0.2.dist-info/RECORD
-8 files, 19116 bytes uncompressed, 7310 bytes compressed:  61.8%
+Zip file size: 8495 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      124 b- defN 23-Jul-26 01:26 rapidocr_pdf/__init__.py
+-rw-r--r--  2.0 unx     4118 b- defN 23-Jul-26 01:26 rapidocr_pdf/main.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-26 01:27 rapidocr_pdf-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2714 b- defN 23-Jul-26 01:27 rapidocr_pdf-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-26 01:27 rapidocr_pdf-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       57 b- defN 23-Jul-26 01:27 rapidocr_pdf-0.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Jul-26 01:27 rapidocr_pdf-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      669 b- defN 23-Jul-26 01:27 rapidocr_pdf-0.0.3.dist-info/RECORD
+8 files, 19144 bytes uncompressed, 7319 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: rapidocr_pdf/__init__.py
 Comment: 
 
 Filename: rapidocr_pdf/main.py
 Comment: 
 
-Filename: rapidocr_pdf-0.0.2.dist-info/LICENSE
+Filename: rapidocr_pdf-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: rapidocr_pdf-0.0.2.dist-info/METADATA
+Filename: rapidocr_pdf-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: rapidocr_pdf-0.0.2.dist-info/WHEEL
+Filename: rapidocr_pdf-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: rapidocr_pdf-0.0.2.dist-info/entry_points.txt
+Filename: rapidocr_pdf-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapidocr_pdf-0.0.2.dist-info/top_level.txt
+Filename: rapidocr_pdf-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: rapidocr_pdf-0.0.2.dist-info/RECORD
+Filename: rapidocr_pdf-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapidocr_pdf/main.py

```diff
@@ -21,15 +21,15 @@
 
 class PDFExtracter():
     def __init__(self, dpi=200):
         self.dpi = dpi
         self.text_sys = RapidOCR()
         self.empyt_list = []
 
-    def __call__(self, content: Union[str, Path, bytes]) -> Dict:
+    def __call__(self, content: Union[str, Path, bytes]) -> List[List[Union[str, str, str]]]:
         try:
             file_type = self.which_type(content)
         except (FileExistsError, TypeError) as e:
             raise PDFExtracterError('The input content is empty.') from e
 
         if file_type != 'pdf':
             raise PDFExtracterError('The file type is not PDF format.')
```

## Comparing `rapidocr_pdf-0.0.2.dist-info/LICENSE` & `rapidocr_pdf-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rapidocr_pdf-0.0.2.dist-info/METADATA` & `rapidocr_pdf-0.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidocr-pdf
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools of extracting PDF content based on RapidOCR
 Home-page: https://github.com/RapidAI/RapidOCRPDF
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: rapidocr_pdf,rapidocr_onnxruntime,ocr,onnxruntime,openvino
 Platform: Any
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapidocr-pdf Version: 0.0.2 Summary: Tools of
+Metadata-Version: 2.1 Name: rapidocr-pdf Version: 0.0.3 Summary: Tools of
 extracting PDF content based on RapidOCR Home-page: https://github.com/RapidAI/
 RapidOCRPDF Author: SWHL Author-email: liekkaskono@163.com License: Apache-2.0
 Keywords: rapidocr_pdf,rapidocr_onnxruntime,ocr,onnxruntime,openvino Platform:
 Any Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Python:
 >=3.7,<=3.10 Description-Content-Type: text/markdown Requires-Dist: filetype
```

## Comparing `rapidocr_pdf-0.0.2.dist-info/RECORD` & `rapidocr_pdf-0.0.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 rapidocr_pdf/__init__.py,sha256=ZKLhEqbDsbmmJqfqgtEtdmttuP1lAahqwH1Pc3nFMlI,124
-rapidocr_pdf/main.py,sha256=7Cv_88_aPmnzdBGiXwzhuTXzWBRUZfoZl5hO8IcEx7A,4090
-rapidocr_pdf-0.0.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-rapidocr_pdf-0.0.2.dist-info/METADATA,sha256=FDtGooksplK3Xbe_ym3TBPjeT5Zg6UGYU05x3miqhfs,2714
-rapidocr_pdf-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rapidocr_pdf-0.0.2.dist-info/entry_points.txt,sha256=dQ50ORbkK0BYQBJ1BNsgwNQ00KG7qr9gGTdhb_-m8A4,57
-rapidocr_pdf-0.0.2.dist-info/top_level.txt,sha256=cUWcSy5Kx0UwXhykCHUGic4Ldb3_z-frD6O7gKShomQ,13
-rapidocr_pdf-0.0.2.dist-info/RECORD,,
+rapidocr_pdf/main.py,sha256=eR6HYvxMuqlRHVC1dccEsXF2ooe_Wpf6fDuYMZE761s,4118
+rapidocr_pdf-0.0.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+rapidocr_pdf-0.0.3.dist-info/METADATA,sha256=3P4rx81TFnSCShHhYA4n3X48pSM5In7R-5AIAlfOs10,2714
+rapidocr_pdf-0.0.3.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+rapidocr_pdf-0.0.3.dist-info/entry_points.txt,sha256=dQ50ORbkK0BYQBJ1BNsgwNQ00KG7qr9gGTdhb_-m8A4,57
+rapidocr_pdf-0.0.3.dist-info/top_level.txt,sha256=cUWcSy5Kx0UwXhykCHUGic4Ldb3_z-frD6O7gKShomQ,13
+rapidocr_pdf-0.0.3.dist-info/RECORD,,
```


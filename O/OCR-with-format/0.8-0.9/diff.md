# Comparing `tmp/OCR_with_format-0.8.tar.gz` & `tmp/OCR_with_format-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OCR_with_format-0.8.tar", last modified: Tue Jul 25 16:03:25 2023, max compression
+gzip compressed data, was "OCR_with_format-0.9.tar", last modified: Wed Jul 26 13:08:39 2023, max compression
```

## Comparing `OCR_with_format-0.8.tar` & `OCR_with_format-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 16:03:25.041263 OCR_with_format-0.8/
--rw-rw-r--   0 g         (1000) g         (1000)    35149 2023-07-25 14:23:49.000000 OCR_with_format-0.8/LICENSE
--rw-rw-r--   0 g         (1000) g         (1000)    46195 2023-07-25 16:03:25.041263 OCR_with_format-0.8/PKG-INFO
--rw-rw-r--   0 g         (1000) g         (1000)     5075 2023-07-25 16:02:37.000000 OCR_with_format-0.8/README.md
--rw-rw-r--   0 g         (1000) g         (1000)      956 2023-07-25 16:02:57.000000 OCR_with_format-0.8/pyproject.toml
--rw-rw-r--   0 g         (1000) g         (1000)       38 2023-07-25 16:03:25.041263 OCR_with_format-0.8/setup.cfg
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 16:03:25.037263 OCR_with_format-0.8/src/
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 16:03:25.041263 OCR_with_format-0.8/src/OCR_with_format/
--rw-rw-r--   0 g         (1000) g         (1000)    10639 2023-07-25 16:03:08.000000 OCR_with_format-0.8/src/OCR_with_format/__init__.py
--rw-rw-r--   0 g         (1000) g         (1000)       55 2023-07-25 15:15:12.000000 OCR_with_format-0.8/src/OCR_with_format/__main__.py
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-25 16:03:25.041263 OCR_with_format-0.8/src/OCR_with_format.egg-info/
--rw-rw-r--   0 g         (1000) g         (1000)    46195 2023-07-25 16:03:25.000000 OCR_with_format-0.8/src/OCR_with_format.egg-info/PKG-INFO
--rw-rw-r--   0 g         (1000) g         (1000)      356 2023-07-25 16:03:25.000000 OCR_with_format-0.8/src/OCR_with_format.egg-info/SOURCES.txt
--rw-rw-r--   0 g         (1000) g         (1000)        1 2023-07-25 16:03:25.000000 OCR_with_format-0.8/src/OCR_with_format.egg-info/dependency_links.txt
--rw-rw-r--   0 g         (1000) g         (1000)       56 2023-07-25 16:03:25.000000 OCR_with_format-0.8/src/OCR_with_format.egg-info/entry_points.txt
--rw-rw-r--   0 g         (1000) g         (1000)      105 2023-07-25 16:03:25.000000 OCR_with_format-0.8/src/OCR_with_format.egg-info/requires.txt
--rw-rw-r--   0 g         (1000) g         (1000)       16 2023-07-25 16:03:25.000000 OCR_with_format-0.8/src/OCR_with_format.egg-info/top_level.txt
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-26 13:08:39.275941 OCR_with_format-0.9/
+-rw-rw-r--   0 g         (1000) g         (1000)    35149 2023-07-26 12:56:22.000000 OCR_with_format-0.9/LICENSE
+-rw-rw-r--   0 g         (1000) g         (1000)    46247 2023-07-26 13:08:39.275941 OCR_with_format-0.9/PKG-INFO
+-rw-rw-r--   0 g         (1000) g         (1000)     5127 2023-07-26 13:07:56.000000 OCR_with_format-0.9/README.md
+-rw-rw-r--   0 g         (1000) g         (1000)      956 2023-07-26 13:07:08.000000 OCR_with_format-0.9/pyproject.toml
+-rw-rw-r--   0 g         (1000) g         (1000)       38 2023-07-26 13:08:39.275941 OCR_with_format-0.9/setup.cfg
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-26 13:08:39.271941 OCR_with_format-0.9/src/
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-26 13:08:39.275941 OCR_with_format-0.9/src/OCR_with_format/
+-rw-rw-r--   0 g         (1000) g         (1000)    12620 2023-07-26 13:07:00.000000 OCR_with_format-0.9/src/OCR_with_format/__init__.py
+-rw-rw-r--   0 g         (1000) g         (1000)       55 2023-07-26 12:56:22.000000 OCR_with_format-0.9/src/OCR_with_format/__main__.py
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2023-07-26 13:08:39.275941 OCR_with_format-0.9/src/OCR_with_format.egg-info/
+-rw-rw-r--   0 g         (1000) g         (1000)    46247 2023-07-26 13:08:39.000000 OCR_with_format-0.9/src/OCR_with_format.egg-info/PKG-INFO
+-rw-rw-r--   0 g         (1000) g         (1000)      356 2023-07-26 13:08:39.000000 OCR_with_format-0.9/src/OCR_with_format.egg-info/SOURCES.txt
+-rw-rw-r--   0 g         (1000) g         (1000)        1 2023-07-26 13:08:39.000000 OCR_with_format-0.9/src/OCR_with_format.egg-info/dependency_links.txt
+-rw-rw-r--   0 g         (1000) g         (1000)       56 2023-07-26 13:08:39.000000 OCR_with_format-0.9/src/OCR_with_format.egg-info/entry_points.txt
+-rw-rw-r--   0 g         (1000) g         (1000)      105 2023-07-26 13:08:39.000000 OCR_with_format-0.9/src/OCR_with_format.egg-info/requires.txt
+-rw-rw-r--   0 g         (1000) g         (1000)       16 2023-07-26 13:08:39.000000 OCR_with_format-0.9/src/OCR_with_format.egg-info/top_level.txt
```

### Comparing `OCR_with_format-0.8/LICENSE` & `OCR_with_format-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `OCR_with_format-0.8/PKG-INFO` & `OCR_with_format-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OCR_with_format
-Version: 0.8
+Version: 0.9
 Summary: Wrapper to pytesseract to preserve space and formatting
 Author: thiswillbeyourgithub
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -705,14 +705,18 @@
 
 POSITIONAL ARGUMENTS
     IMG_PATH
         Type: str
         path to the image you want to do OCR on
 
 FLAGS
+    -m, --method=METHOD
+        Type: str
+        Default: 'with_format'
+        if 'with_format', will use the author's code if 'none', will output tesseract's default output if 'stackoverflow', will output using another algorithm found on stackoverflow
     --thresholding_method=THRESHOLDING_METHOD
         Type: str
         Default: 'otsu'
         any from "otsu", "otsu_gaussian", "adaptative_gaussian", "all"
 
         If "all", the three methods will be tried and the final output will be the one which maximizes the mean and median confidences over each parsed words.
     -l, --language=LANGUAGE
@@ -726,20 +730,18 @@
     --tesseract_args=TESSERACT_ARGS
         Type: str
         Default: '-...
         default arguments for tesseract
     -q, --quiet=QUIET
         Default: False
         if True, will only print the output and no logs
-    -c, --comparison_run=COMPARISON_RUN
-        Default: False
-        if True, will just output the raw output from pytesseract. This can be used to convince yourself of the usefullness of this project.
 
 NOTES
     You can also use flags syntax for POSITIONAL ARGUMENTS
+
 ```
 
 ## Example
 
 * Image:
   * ![](https://github.com/thiswillbeyourgithub/OCR_with_format/blob/295e724b758045dc952934b6f0d98172fdc9a12e/screenshot.png?raw=true)
 * output from `OCR_with_format ./screenshot.png --thresholding_method="all"  --quiet`
```

### Comparing `OCR_with_format-0.8/README.md` & `OCR_with_format-0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 
 POSITIONAL ARGUMENTS
     IMG_PATH
         Type: str
         path to the image you want to do OCR on
 
 FLAGS
+    -m, --method=METHOD
+        Type: str
+        Default: 'with_format'
+        if 'with_format', will use the author's code if 'none', will output tesseract's default output if 'stackoverflow', will output using another algorithm found on stackoverflow
     --thresholding_method=THRESHOLDING_METHOD
         Type: str
         Default: 'otsu'
         any from "otsu", "otsu_gaussian", "adaptative_gaussian", "all"
 
         If "all", the three methods will be tried and the final output will be the one which maximizes the mean and median confidences over each parsed words.
     -l, --language=LANGUAGE
@@ -37,20 +41,18 @@
     --tesseract_args=TESSERACT_ARGS
         Type: str
         Default: '-...
         default arguments for tesseract
     -q, --quiet=QUIET
         Default: False
         if True, will only print the output and no logs
-    -c, --comparison_run=COMPARISON_RUN
-        Default: False
-        if True, will just output the raw output from pytesseract. This can be used to convince yourself of the usefullness of this project.
 
 NOTES
     You can also use flags syntax for POSITIONAL ARGUMENTS
+
 ```
 
 ## Example
 
 * Image:
   * ![](https://github.com/thiswillbeyourgithub/OCR_with_format/blob/295e724b758045dc952934b6f0d98172fdc9a12e/screenshot.png?raw=true)
 * output from `OCR_with_format ./screenshot.png --thresholding_method="all"  --quiet`
```

### Comparing `OCR_with_format-0.8/pyproject.toml` & `OCR_with_format-0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "OCR_with_format"
-version = "0.8"
+version = "0.9"
 description = "Wrapper to pytesseract to preserve space and formatting"
 readme = "README.md"
 authors = [{ name = "thiswillbeyourgithub"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python",
```

### Comparing `OCR_with_format-0.8/src/OCR_with_format/__init__.py` & `OCR_with_format-0.9/src/OCR_with_format/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import fire
 import pytesseract
+from pytesseract import Output
 import ftfy
 import numpy as np
 import cv2
 from bs4 import BeautifulSoup
 import re
 from textwrap import dedent
+import pandas as pd
 
 # pre compiled regex
 bbox_regex = re.compile(r'bbox\s(\d+)\s(\d+)\s(\d+)\s(\d+)')
 confidence_regex = re.compile(r'x_wconf\s(\d+)')
 newlines_regex = re.compile(r'\n\s*\n')
 
-__version__ = "0.8"
+__version__ = "0.9"
 
 # msic
 
 def _get_wdim(ocrx_word):
     "parse the dimansion of the word from the ocrx object"
     return [int(x) for x in re.findall(bbox_regex, ocrx_word["title"])[0]]
 
@@ -32,30 +34,78 @@
     return pytesseract.image_to_pdf_or_hocr(
             img,
             lang=lang,
             config=args,
             extension="hocr",
             )
 
+def stackoverflow_method(img, lang, args):
+    d = pytesseract.image_to_data(
+            img,
+            lang=lang,
+            config=args,
+            output_type=Output.DICT,
+            )
+    df = pd.DataFrame(d)
+
+    # clean up blanks
+    df1 = df[(df.conf!='-1')&(df.text!=' ')&(df.text!='')]
+    # sort blocks vertically
+    sorted_blocks = df1.groupby('block_num').first().sort_values('top').index.tolist()
+    output = []
+    for block in sorted_blocks:
+        curr = df1[df1['block_num']==block]
+        sel = curr[curr.text.str.len()>3]
+        char_w = (sel.width/sel.text.str.len()).mean()
+        prev_par, prev_line, prev_left = 0, 0, 0
+        text = ''
+        for ix, ln in curr.iterrows():
+            # add new line when necessary
+            if prev_par != ln['par_num']:
+                text += '\n'
+                prev_par = ln['par_num']
+                prev_line = ln['line_num']
+                prev_left = 0
+            elif prev_line != ln['line_num']:
+                text += '\n'
+                prev_line = ln['line_num']
+                prev_left = 0
+
+            added = 0  # num of spaces that should be added
+            if ln['left']/char_w > prev_left + 1:
+                added = int((ln['left'])/char_w) - prev_left
+                text += ' ' * added
+            text += ln['text'] + ' '
+            prev_left += len(ln['text']) + added + 1
+        #text += '\n'
+        output.append(text)
+    return "\n".join(output)
+
 
 def OCR_with_format(
         img_path: str,
+        method: str = "with_format",
         thresholding_method: str = "otsu",
         language: str = "eng",
         output_path: str = None,
         tesseract_args: str = "--oem 3 --psm 11 -c preserve_interword_spaces=1",
         quiet=False,
-        comparison_run=False,
         ):
     """
     Parameters
     ----------
     img_path: str
         path to the image you want to do OCR on
 
+    method: str, default 'with_format'
+        if 'with_format', will use the author's code
+        if 'none', will output tesseract's default output
+        if 'stackoverflow', will output using another algorithm found on stackoverflow
+        source : https://stackoverflow.com/questions/59582008/preserving-indentation-with-tesseract-ocr-4-x
+
     thresholding_method: str, default otsu
         any from "otsu", "otsu_gaussian", "adaptative_gaussian", "all"
 
         If "all", the three methods will be tried and the final output will be
         the one which maximizes the mean and median confidences over
         each parsed words.
 
@@ -67,18 +117,14 @@
 
     tesseract_args: str, default "--oem 3 --psm 11 -c preserve_interword_spaces=1"
         default arguments for tesseract
 
     quiet: bool, default False
         if True, will only print the output and no logs
 
-    comparison_run: bool, default False
-        if True, will just output the raw output from pytesseract. This
-        can be used to convince yourself of the usefullness of this project.
-
     """
     if quiet:
         pr = lambda x: None
     else:
         pr = print
     img = cv2.imread(img_path, flags=1)
 
@@ -91,19 +137,28 @@
 
     # preprocess several times then OCR, keep the one with the highest median confidence
     preprocessings = {}
 
     # sharpen a bit
     gray_sharp = cv2.addWeighted(gray, 1.5, cv2.GaussianBlur(gray, (0, 0), 10), -0.5, 0)
 
-    if comparison_run:
+    if method == "none" or not method:
+        pr("Using default tesseract method")
         return pytesseract.image_to_string(
                 img,
                 lang=language,
-                config="",
+                config=tesseract_args,
+                )
+
+    if method == "stackoverflow":
+        pr("Using method found on stackoverflow")
+        return stackoverflow_method(
+                img,
+                lang=language,
+                args=tesseract_args,
                 )
 
     # source:
     # https://opencv24-python-tutorials.readthedocs.io/en/latest/py_tutorials/py_imgproc/py_thresholding/py_thresholding.html#otsus-binarization
     if thresholding_method in ["otsu", "all"]:
         # Otsu's thresholding
         _, sharpened = cv2.threshold(gray, 0, 255, cv2.THRESH_BINARY+cv2.THRESH_OTSU)
```

### Comparing `OCR_with_format-0.8/src/OCR_with_format.egg-info/PKG-INFO` & `OCR_with_format-0.9/src/OCR_with_format.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OCR-with-format
-Version: 0.8
+Version: 0.9
 Summary: Wrapper to pytesseract to preserve space and formatting
 Author: thiswillbeyourgithub
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -705,14 +705,18 @@
 
 POSITIONAL ARGUMENTS
     IMG_PATH
         Type: str
         path to the image you want to do OCR on
 
 FLAGS
+    -m, --method=METHOD
+        Type: str
+        Default: 'with_format'
+        if 'with_format', will use the author's code if 'none', will output tesseract's default output if 'stackoverflow', will output using another algorithm found on stackoverflow
     --thresholding_method=THRESHOLDING_METHOD
         Type: str
         Default: 'otsu'
         any from "otsu", "otsu_gaussian", "adaptative_gaussian", "all"
 
         If "all", the three methods will be tried and the final output will be the one which maximizes the mean and median confidences over each parsed words.
     -l, --language=LANGUAGE
@@ -726,20 +730,18 @@
     --tesseract_args=TESSERACT_ARGS
         Type: str
         Default: '-...
         default arguments for tesseract
     -q, --quiet=QUIET
         Default: False
         if True, will only print the output and no logs
-    -c, --comparison_run=COMPARISON_RUN
-        Default: False
-        if True, will just output the raw output from pytesseract. This can be used to convince yourself of the usefullness of this project.
 
 NOTES
     You can also use flags syntax for POSITIONAL ARGUMENTS
+
 ```
 
 ## Example
 
 * Image:
   * ![](https://github.com/thiswillbeyourgithub/OCR_with_format/blob/295e724b758045dc952934b6f0d98172fdc9a12e/screenshot.png?raw=true)
 * output from `OCR_with_format ./screenshot.png --thresholding_method="all"  --quiet`
```


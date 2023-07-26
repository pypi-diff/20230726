# Comparing `tmp/tesstrain-0.1.tar.gz` & `tmp/tesstrain-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/sdostal/code/2023/python37/tesstrain/src/dist/tmp5rurwcsa/tesstrain-0.1.tar", last modified: Mon Jan  9 10:20:45 2023, max compression
+gzip compressed data, was "tesstrain-0.1.1.tar", last modified: Wed Jul 26 07:07:06 2023, max compression
```

## Comparing `tesstrain-0.1.tar` & `tesstrain-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-01-09 10:20:45.000000 tesstrain-0.1/
--rw-r--r--   0 sdostal   (6000) users      (100)     1765 2023-01-09 10:20:45.000000 tesstrain-0.1/PKG-INFO
--rw-r--r--   0 sdostal   (6000) users      (100)      818 2023-01-09 10:14:25.000000 tesstrain-0.1/README.md
--rw-r--r--   0 sdostal   (6000) users      (100)       88 2023-01-09 10:20:45.000000 tesstrain-0.1/setup.cfg
--rw-r--r--   0 sdostal   (6000) users      (100)     1308 2023-01-09 10:14:25.000000 tesstrain-0.1/setup.py
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-01-09 10:20:45.000000 tesstrain-0.1/tesstrain/
--rw-r--r--   0 sdostal   (6000) users      (100)      663 2023-01-09 10:14:25.000000 tesstrain-0.1/tesstrain/__init__.py
--rw-r--r--   0 sdostal   (6000) users      (100)     2242 2023-01-09 10:14:25.000000 tesstrain-0.1/tesstrain/__main__.py
--rw-r--r--   0 sdostal   (6000) users      (100)     8406 2023-01-09 10:14:25.000000 tesstrain-0.1/tesstrain/arguments.py
--rw-r--r--   0 sdostal   (6000) users      (100)    12479 2023-01-09 10:14:25.000000 tesstrain-0.1/tesstrain/generate.py
--rw-r--r--   0 sdostal   (6000) users      (100)    37251 2023-01-09 10:14:25.000000 tesstrain-0.1/tesstrain/language_specific.py
--rwxr-xr-x   0 sdostal   (6000) users      (100)     5445 2023-01-09 10:14:25.000000 tesstrain-0.1/tesstrain/wrapper.py
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-01-09 10:20:45.000000 tesstrain-0.1/tesstrain.egg-info/
--rw-r--r--   0 sdostal   (6000) users      (100)     1765 2023-01-09 10:20:45.000000 tesstrain-0.1/tesstrain.egg-info/PKG-INFO
--rw-r--r--   0 sdostal   (6000) users      (100)      369 2023-01-09 10:20:45.000000 tesstrain-0.1/tesstrain.egg-info/SOURCES.txt
--rw-r--r--   0 sdostal   (6000) users      (100)        1 2023-01-09 10:20:45.000000 tesstrain-0.1/tesstrain.egg-info/dependency_links.txt
--rw-r--r--   0 sdostal   (6000) users      (100)       20 2023-01-09 10:20:45.000000 tesstrain-0.1/tesstrain.egg-info/entry_points.txt
--rw-r--r--   0 sdostal   (6000) users      (100)        5 2023-01-09 10:20:45.000000 tesstrain-0.1/tesstrain.egg-info/requires.txt
--rw-r--r--   0 sdostal   (6000) users      (100)       10 2023-01-09 10:20:45.000000 tesstrain-0.1/tesstrain.egg-info/top_level.txt
+drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-07-26 07:07:06.482728 tesstrain-0.1.1/
+-rw-r--r--   0 sdostal   (6000) users      (100)    10173 2023-07-26 07:01:26.000000 tesstrain-0.1.1/LICENSE
+-rw-r--r--   0 sdostal   (6000) users      (100)     1923 2023-07-26 07:07:06.482728 tesstrain-0.1.1/PKG-INFO
+-rw-r--r--   0 sdostal   (6000) users      (100)      894 2023-07-26 06:56:45.000000 tesstrain-0.1.1/README.md
+-rw-r--r--   0 sdostal   (6000) users      (100)       88 2023-07-26 07:07:06.482728 tesstrain-0.1.1/setup.cfg
+-rw-r--r--   0 sdostal   (6000) users      (100)     1365 2023-07-26 06:57:57.000000 tesstrain-0.1.1/setup.py
+drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-07-26 07:07:06.482728 tesstrain-0.1.1/tesstrain/
+-rw-r--r--   0 sdostal   (6000) users      (100)      665 2023-07-26 07:00:24.000000 tesstrain-0.1.1/tesstrain/__init__.py
+-rw-r--r--   0 sdostal   (6000) users      (100)     2242 2023-07-26 06:48:53.000000 tesstrain-0.1.1/tesstrain/__main__.py
+-rw-r--r--   0 sdostal   (6000) users      (100)     8597 2023-07-26 06:48:53.000000 tesstrain-0.1.1/tesstrain/arguments.py
+-rw-r--r--   0 sdostal   (6000) users      (100)    12537 2023-07-26 06:48:53.000000 tesstrain-0.1.1/tesstrain/generate.py
+-rw-r--r--   0 sdostal   (6000) users      (100)    37251 2023-07-26 06:48:53.000000 tesstrain-0.1.1/tesstrain/language_specific.py
+-rwxr-xr-x   0 sdostal   (6000) users      (100)     5445 2023-07-26 06:48:53.000000 tesstrain-0.1.1/tesstrain/wrapper.py
+drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2023-07-26 07:07:06.482728 tesstrain-0.1.1/tesstrain.egg-info/
+-rw-r--r--   0 sdostal   (6000) users      (100)     1923 2023-07-26 07:07:06.000000 tesstrain-0.1.1/tesstrain.egg-info/PKG-INFO
+-rw-r--r--   0 sdostal   (6000) users      (100)      377 2023-07-26 07:07:06.000000 tesstrain-0.1.1/tesstrain.egg-info/SOURCES.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)        1 2023-07-26 07:07:06.000000 tesstrain-0.1.1/tesstrain.egg-info/dependency_links.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)       20 2023-07-26 07:07:06.000000 tesstrain-0.1.1/tesstrain.egg-info/entry_points.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)        5 2023-07-26 07:07:06.000000 tesstrain-0.1.1/tesstrain.egg-info/requires.txt
+-rw-r--r--   0 sdostal   (6000) users      (100)       10 2023-07-26 07:07:06.000000 tesstrain-0.1.1/tesstrain.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tesstrain-0.1/PKG-INFO` & `tesstrain-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 Metadata-Version: 2.1
 Name: tesstrain
-Version: 0.1
+Version: 0.1.1
 Summary: Training utils for Tesseract
-Home-page: https://github.com/tesseract-ocr/tesstrain
+Home-page: https://github.com/stefan6419846/tesstrain_package
 Author: Tesseract contributors
 License: Apache Software License 2.0
 Keywords: Tesseract,tesseract-ocr,OCR,optical character recognition
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # tesstrain.py
 
 Utilities for working with Tesseract >= 4 using artificial training data.
 
-## Install
+## About
 
-This package requires the Tesseract training tools to be available on your system.
+This repository contains a standalone fork of the official/upstream code at https://github.com/tesseract-ocr/tesstrain/tree/main/src to allow easier packaging for PyPI.
 
-To install the PIP package, either use `pip install tesstrain` (for existing packages) or `pip install .` (from source checkout).
-A supported Python version (at least 3.7) is required for running.
+## Installation
+
+This package requires the Tesseract training tools to be available on your system. Additionally, a supported Python version (at least 3.6) is required for running.
+
+You can install this package from PyPI:
+
+```bash
+python -m pip install tesstrain
+```
+
+Alternatively, you may use `pip install .` to install the package from a source checkout.
 
 ## Running
 
 * Use the terminal interface to directly interact with the tools: `python -m tesstrain --help`.
 * Call it from your own code using the high-level interface `tesstrain.run()`.
 
 ## License
 
-Software is provided under the terms of the `Apache 2.0` license.
-
-Sample training data provided by [Deutsches Textarchiv](https://deutschestextarchiv.de) is [in the public domain](http://creativecommons.org/publicdomain/mark/1.0/).
+This package is subject to the terms of the Apache-2.0 license.
```

### Comparing `tesstrain-0.1/README.md` & `tesstrain-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 # tesstrain.py
 
 Utilities for working with Tesseract >= 4 using artificial training data.
 
-## Install
+## About
 
-This package requires the Tesseract training tools to be available on your system.
+This repository contains a standalone fork of the official/upstream code at https://github.com/tesseract-ocr/tesstrain/tree/main/src to allow easier packaging for PyPI.
 
-To install the PIP package, either use `pip install tesstrain` (for existing packages) or `pip install .` (from source checkout).
-A supported Python version (at least 3.7) is required for running.
+## Installation
+
+This package requires the Tesseract training tools to be available on your system. Additionally, a supported Python version (at least 3.6) is required for running.
+
+You can install this package from PyPI:
+
+```bash
+python -m pip install tesstrain
+```
+
+Alternatively, you may use `pip install .` to install the package from a source checkout.
 
 ## Running
 
 * Use the terminal interface to directly interact with the tools: `python -m tesstrain --help`.
 * Call it from your own code using the high-level interface `tesstrain.run()`.
 
 ## License
 
-Software is provided under the terms of the `Apache 2.0` license.
-
-Sample training data provided by [Deutsches Textarchiv](https://deutschestextarchiv.de) is [in the public domain](http://creativecommons.org/publicdomain/mark/1.0/).
+This package is subject to the terms of the Apache-2.0 license.
```

### Comparing `tesstrain-0.1/setup.py` & `tesstrain-0.1.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,34 +6,35 @@
 ROOT_DIRECTORY = Path(__file__).parent.resolve()
 
 setuptools.setup(
     name='tesstrain',
     description='Training utils for Tesseract',
     long_description=(ROOT_DIRECTORY / 'README.md').read_text(encoding='utf-8'),
     long_description_content_type='text/markdown',
-    url='https://github.com/tesseract-ocr/tesstrain',
+    url='https://github.com/stefan6419846/tesstrain_package',
     packages=setuptools.find_packages(),
     license='Apache Software License 2.0',
     author='Tesseract contributors',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Scientific/Engineering :: Image Recognition',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
+        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     keywords='Tesseract,tesseract-ocr,OCR,optical character recognition',
 
-    python_requires='>=3.7',
+    python_requires='>=3.6',
     install_requires=[
         'tqdm',
     ],
 
     entry_points={
         'console_scripts': [
         ],
```

### Comparing `tesstrain-0.1/tesstrain/__init__.py` & `tesstrain-0.1.1/tesstrain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from tesstrain.wrapper import run
 
-__version__ = '0.1'
+__version__ = '0.1.1'
```

### Comparing `tesstrain-0.1/tesstrain/__main__.py` & `tesstrain-0.1.1/tesstrain/__main__.py`

 * *Files identical despite different names*

### Comparing `tesstrain-0.1/tesstrain/arguments.py` & `tesstrain-0.1.1/tesstrain/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,21 @@
     parser.add_argument(
         "--fontlist",
         dest="fonts",
         nargs="+",
         type=str,
         help="A list of fontnames to train on.",
     )
+    parser.add_argument(
+        "--vertical_fontlist",
+        dest="vertical_fonts",
+        nargs="+",
+        type=str,
+        help="A list of fontnames to render vertical text.",
+    )
     parser.add_argument("--fonts_dir", help="Path to font files.")
     parser.add_argument("--tmp_dir", help="Path to temporary training directory.")
     parser.add_argument(
         "--lang", metavar="LANG_CODE", dest="lang_code", help="ISO 639 code."
     )
     parser.add_argument(
         "--langdata_dir",
```

### Comparing `tesstrain-0.1/tesstrain/generate.py` & `tesstrain-0.1.1/tesstrain/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,16 @@
     ]
 
     if ctx.distort_image:
         common_args.append("--distort_image")
 
     # add --writing_mode=vertical-upright to common_args if the font is
     # specified to be rendered vertically.
-    if font in VERTICAL_FONTS:
+    vertical_fonts = ctx.vertical_fonts or VERTICAL_FONTS
+    if font in vertical_fonts:
         common_args.append("--writing_mode=vertical-upright")
 
     run_command(
         "text2image",
         *common_args,
         f"--font={font}",
         f"--text={ctx.training_text}",
```

### Comparing `tesstrain-0.1/tesstrain/language_specific.py` & `tesstrain-0.1.1/tesstrain/language_specific.py`

 * *Files identical despite different names*

### Comparing `tesstrain-0.1/tesstrain/wrapper.py` & `tesstrain-0.1.1/tesstrain/wrapper.py`

 * *Files identical despite different names*

### Comparing `tesstrain-0.1/tesstrain.egg-info/PKG-INFO` & `tesstrain-0.1.1/tesstrain.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 Metadata-Version: 2.1
 Name: tesstrain
-Version: 0.1
+Version: 0.1.1
 Summary: Training utils for Tesseract
-Home-page: https://github.com/tesseract-ocr/tesstrain
+Home-page: https://github.com/stefan6419846/tesstrain_package
 Author: Tesseract contributors
 License: Apache Software License 2.0
 Keywords: Tesseract,tesseract-ocr,OCR,optical character recognition
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # tesstrain.py
 
 Utilities for working with Tesseract >= 4 using artificial training data.
 
-## Install
+## About
 
-This package requires the Tesseract training tools to be available on your system.
+This repository contains a standalone fork of the official/upstream code at https://github.com/tesseract-ocr/tesstrain/tree/main/src to allow easier packaging for PyPI.
 
-To install the PIP package, either use `pip install tesstrain` (for existing packages) or `pip install .` (from source checkout).
-A supported Python version (at least 3.7) is required for running.
+## Installation
+
+This package requires the Tesseract training tools to be available on your system. Additionally, a supported Python version (at least 3.6) is required for running.
+
+You can install this package from PyPI:
+
+```bash
+python -m pip install tesstrain
+```
+
+Alternatively, you may use `pip install .` to install the package from a source checkout.
 
 ## Running
 
 * Use the terminal interface to directly interact with the tools: `python -m tesstrain --help`.
 * Call it from your own code using the high-level interface `tesstrain.run()`.
 
 ## License
 
-Software is provided under the terms of the `Apache 2.0` license.
-
-Sample training data provided by [Deutsches Textarchiv](https://deutschestextarchiv.de) is [in the public domain](http://creativecommons.org/publicdomain/mark/1.0/).
+This package is subject to the terms of the Apache-2.0 license.
```


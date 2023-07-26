# Comparing `tmp/render50-9.2.0.tar.gz` & `tmp/render50-9.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render50-9.2.0.tar", last modified: Wed Jul 26 15:09:06 2023, max compression
+gzip compressed data, was "render50-9.2.1.tar", last modified: Wed Jul 26 16:11:49 2023, max compression
```

## Comparing `render50-9.2.0.tar` & `render50-9.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:09:06.078648 render50-9.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 15:08:38.000000 render50-9.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-26 15:09:06.078648 render50-9.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-26 15:08:38.000000 render50-9.2.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    20611 2023-07-26 15:08:38.000000 render50-9.2.0/render50
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:09:06.074648 render50-9.2.0/render50.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-26 15:09:06.000000 render50-9.2.0/render50.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-26 15:09:06.000000 render50-9.2.0/render50.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:09:06.000000 render50-9.2.0/render50.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-26 15:09:06.000000 render50-9.2.0/render50.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:09:06.000000 render50-9.2.0/render50.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:09:06.078648 render50-9.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-26 15:08:38.000000 render50-9.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:11:49.520497 render50-9.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 16:11:28.000000 render50-9.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-26 16:11:49.520497 render50-9.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-26 16:11:28.000000 render50-9.2.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20631 2023-07-26 16:11:28.000000 render50-9.2.1/render50
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:11:49.516497 render50-9.2.1/render50.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-26 16:11:49.000000 render50-9.2.1/render50.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-26 16:11:49.000000 render50-9.2.1/render50.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 16:11:49.000000 render50-9.2.1/render50.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-26 16:11:49.000000 render50-9.2.1/render50.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 16:11:49.000000 render50-9.2.1/render50.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 16:11:49.520497 render50-9.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-26 16:11:28.000000 render50-9.2.1/setup.py
```

### Comparing `render50-9.2.0/LICENSE` & `render50-9.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `render50-9.2.0/render50` & `render50-9.2.1/render50`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from natsort import natsorted, ns
 from pkg_resources import DistributionNotFound, get_distribution
 from pygments import highlight
 from pygments.formatters import HtmlFormatter
 from pygments.lexers import get_lexer_for_filename, guess_lexer
 from pygments.lexers.special import TextLexer
 from pygments.styles import get_all_styles
-from PyPDF2 import PdfReader, PdfFileWriter
+from pypdf import PdfReader, PdfWriter, Transformation
 from requests.exceptions import RequestException
 from tempfile import mkstemp
 from textwrap import fill
 from traceback import print_exception
 from urllib.parse import urljoin
 from warnings import filterwarnings
 
@@ -344,34 +344,34 @@
     """Concatenate (PDF) inputs side by side."""
 
     # Read files
     readers = list(map(PdfReader, inputs))
 
     # Render blank page, inferring size from first input's first page
     temp = mkstemp()
-    size = "{}pt {}pt".format(readers[0].getPage(0).mediaBox[2], readers[0].getPage(0).mediaBox[3])
+    size = "{}pt {}pt".format(readers[0].pages[0].mediabox[2], readers[0].pages[0].mediabox[3])
     write(temp[1], [blank(size)], False)
-    page = PdfReader(temp[1]).getPage(0)
+    page = PdfReader(temp[1]).pages[0]
 
     # Concatenate files side by side
-    writer = PdfFileWriter()
+    writer = PdfWriter()
 
     # Concatenate pages
-    for i in range(max(map(lambda r: r.getNumPages(), readers))):
+    for i in range(max(map(lambda r: len(r.pages), readers))):
 
         # Leftmost page
-        left = copy(readers[0].getPage(i)) if i < readers[0].getNumPages() else copy(page)
+        left = copy(readers[0].pages[i]) if i < len(readers[0].pages) else copy(page)
 
         # Rightmost pages
         for reader in readers[1:]:
-            right = copy(reader.getPage(i)) if i < reader.getNumPages() else copy(page)
-            left.mergeTranslatedPage(right, left.mediaBox[2], 0, expand=True)
+            right = copy(reader.pages[i]) if i < len(reader.pages) else copy(page)
+            left.merge_transformed_page(right, Transformation().translate(left.mediabox[2], 0), expand=True)
 
         # Add pages to output
-        writer.addPage(left)
+        writer.add_page(left)
 
     # Ouput PDF
     with open(output, "wb") as file:
         writer.write(file)
 
     # Remove temporary files
     os.close(temp[0]), os.remove(temp[1])
```

### Comparing `render50-9.2.0/setup.py` & `render50-9.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     classifiers=[
         "Intended Audience :: Education",
         "Programming Language :: Python :: 3",
         "Topic :: Education",
         "Topic :: Utilities"
     ],
     description="This is render50, with which you can render source code as PDFs.",
-    install_requires=["backports.shutil_get_terminal_size", "backports.shutil_which", "braceexpand", "beautifulsoup4", "natsort", "Pygments>=2.7.1", "PyPDF2==2.12.1", "requests", "six>=1.10.0", "termcolor", "WeasyPrint"],
+    install_requires=["backports.shutil_get_terminal_size", "backports.shutil_which", "braceexpand", "beautifulsoup4", "natsort", "Pygments>=2.7.1", "pypdf", "requests", "six>=1.10.0", "termcolor", "WeasyPrint"],
     keywords=["render", "render50"],
     license="GPLv3",
     long_description_content_type="text/markdown",
     name="render50",
     python_requires=">=3.9",
     scripts=["render50"],
     url="https://github.com/cs50/render50",
-    version="9.2.0"
+    version="9.2.1"
 )
```


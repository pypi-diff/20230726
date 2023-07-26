# Comparing `tmp/render50-9.1.2.tar.gz` & `tmp/render50-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render50-9.1.2.tar", last modified: Fri Apr 21 14:08:58 2023, max compression
+gzip compressed data, was "render50-9.2.0.tar", last modified: Wed Jul 26 15:09:06 2023, max compression
```

## Comparing `render50-9.1.2.tar` & `render50-9.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:08:58.058109 render50-9.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 14:08:37.000000 render50-9.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-21 14:08:58.058109 render50-9.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-21 14:08:37.000000 render50-9.1.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    20439 2023-04-21 14:08:37.000000 render50-9.1.2/render50
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:08:58.058109 render50-9.1.2/render50.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-21 14:08:58.000000 render50-9.1.2/render50.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-21 14:08:58.000000 render50-9.1.2/render50.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:08:58.000000 render50-9.1.2/render50.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-21 14:08:58.000000 render50-9.1.2/render50.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:08:58.000000 render50-9.1.2/render50.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:08:58.058109 render50-9.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-21 14:08:37.000000 render50-9.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:09:06.078648 render50-9.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 15:08:38.000000 render50-9.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-26 15:09:06.078648 render50-9.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-26 15:08:38.000000 render50-9.2.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20611 2023-07-26 15:08:38.000000 render50-9.2.0/render50
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:09:06.074648 render50-9.2.0/render50.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-26 15:09:06.000000 render50-9.2.0/render50.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-26 15:09:06.000000 render50-9.2.0/render50.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:09:06.000000 render50-9.2.0/render50.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-26 15:09:06.000000 render50-9.2.0/render50.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:09:06.000000 render50-9.2.0/render50.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:09:06.078648 render50-9.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-26 15:08:38.000000 render50-9.2.0/setup.py
```

### Comparing `render50-9.1.2/LICENSE` & `render50-9.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `render50-9.1.2/render50` & `render50-9.2.0/render50`

 * *Files 0% similar despite different names*

```diff
@@ -555,32 +555,33 @@
 
 
 def write(output, documents, echo=True):
     """
     Write documents to output as PDF.
     https://github.com/Kozea/WeasyPrint/issues/212#issuecomment-52408306
     https://github.com/Kozea/WeasyPrint/issues/1662#issuecomment-1226058917
+    https://github.com/Kozea/WeasyPrint/issues/531#issuecomment-1635857701
     """
     if documents:
         pages = [page for document in documents for page in document.pages]
-        documents[0].copy(pages).write_pdf(output)
-
+        options = DEFAULT_OPTIONS | {"pdf_variant": "pdf/ua-1"}
+        documents[0].copy(pages).write_pdf(output, options=options)
         if echo:
             cprint("Rendered {}.".format(output), "green")
         return True
     else:
         return False
 
 
 # Check for dependencies
 # http://weasyprint.readthedocs.io/en/latest/install.html
 try:
     # Ignore warnings about outdated Cairo and Pango (on Ubuntu 14.04, at least)
     filterwarnings("ignore", category=UserWarning, module="weasyprint")
-    from weasyprint import CSS, HTML
+    from weasyprint import CSS, DEFAULT_OPTIONS, HTML
     from weasyprint.urls import URLFetchingError
 except OSError as e:
     if "pangocairo" in str(e):
         raise RuntimeError("Missing dependency. Install Pango.")
     elif "cairo" in str(e):
         raise RuntimeError("Missing dependency. Install cairo.")
     else:
```

### Comparing `render50-9.1.2/setup.py` & `render50-9.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,12 +11,12 @@
     ],
     description="This is render50, with which you can render source code as PDFs.",
     install_requires=["backports.shutil_get_terminal_size", "backports.shutil_which", "braceexpand", "beautifulsoup4", "natsort", "Pygments>=2.7.1", "PyPDF2==2.12.1", "requests", "six>=1.10.0", "termcolor", "WeasyPrint"],
     keywords=["render", "render50"],
     license="GPLv3",
     long_description_content_type="text/markdown",
     name="render50",
-    python_requires=">=3.6",
+    python_requires=">=3.9",
     scripts=["render50"],
     url="https://github.com/cs50/render50",
-    version="9.1.2"
+    version="9.2.0"
 )
```


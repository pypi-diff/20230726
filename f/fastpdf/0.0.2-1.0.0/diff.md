# Comparing `tmp/fastpdf-0.0.2.tar.gz` & `tmp/fastpdf-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastpdf-0.0.2.tar", last modified: Wed Jul 12 19:45:28 2023, max compression
+gzip compressed data, was "fastpdf-1.0.0.tar", last modified: Wed Jul 26 07:11:45 2023, max compression
```

## Comparing `fastpdf-0.0.2.tar` & `fastpdf-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ko        (1000) ko        (1000)        0 2023-07-12 19:45:28.314751 fastpdf-0.0.2/
--rw-rw-r--   0 ko        (1000) ko        (1000)     2801 2023-07-12 19:45:28.314751 fastpdf-0.0.2/PKG-INFO
--rw-rw-r--   0 ko        (1000) ko        (1000)     2150 2023-07-12 19:42:37.000000 fastpdf-0.0.2/README.md
-drwxrwxr-x   0 ko        (1000) ko        (1000)        0 2023-07-12 19:45:28.314751 fastpdf-0.0.2/fastpdf/
--rw-rw-r--   0 ko        (1000) ko        (1000)       68 2023-06-29 11:16:02.000000 fastpdf-0.0.2/fastpdf/__init__.py
--rw-rw-r--   0 ko        (1000) ko        (1000)    17713 2023-07-12 12:56:50.000000 fastpdf-0.0.2/fastpdf/api.py
--rw-rw-r--   0 ko        (1000) ko        (1000)      671 2023-06-29 11:15:01.000000 fastpdf-0.0.2/fastpdf/exceptions.py
--rw-rw-r--   0 ko        (1000) ko        (1000)     3956 2023-07-12 15:28:56.000000 fastpdf-0.0.2/fastpdf/models.py
-drwxrwxr-x   0 ko        (1000) ko        (1000)        0 2023-07-12 19:45:28.314751 fastpdf-0.0.2/fastpdf.egg-info/
--rw-rw-r--   0 ko        (1000) ko        (1000)     2801 2023-07-12 19:45:28.000000 fastpdf-0.0.2/fastpdf.egg-info/PKG-INFO
--rw-rw-r--   0 ko        (1000) ko        (1000)      247 2023-07-12 19:45:28.000000 fastpdf-0.0.2/fastpdf.egg-info/SOURCES.txt
--rw-rw-r--   0 ko        (1000) ko        (1000)        1 2023-07-12 19:45:28.000000 fastpdf-0.0.2/fastpdf.egg-info/dependency_links.txt
--rw-rw-r--   0 ko        (1000) ko        (1000)       22 2023-07-12 19:45:28.000000 fastpdf-0.0.2/fastpdf.egg-info/requires.txt
--rw-rw-r--   0 ko        (1000) ko        (1000)        8 2023-07-12 19:45:28.000000 fastpdf-0.0.2/fastpdf.egg-info/top_level.txt
--rw-rw-r--   0 ko        (1000) ko        (1000)       38 2023-07-12 19:45:28.314751 fastpdf-0.0.2/setup.cfg
--rw-rw-r--   0 ko        (1000) ko        (1000)     1059 2023-07-12 19:45:14.000000 fastpdf-0.0.2/setup.py
+drwxrwxr-x   0 ko        (1000) ko        (1000)        0 2023-07-26 07:11:45.247278 fastpdf-1.0.0/
+-rw-rw-r--   0 ko        (1000) ko        (1000)    13814 2023-07-26 07:11:45.247278 fastpdf-1.0.0/PKG-INFO
+-rw-rw-r--   0 ko        (1000) ko        (1000)    13196 2023-07-17 15:26:34.000000 fastpdf-1.0.0/README.md
+drwxrwxr-x   0 ko        (1000) ko        (1000)        0 2023-07-26 07:11:45.247278 fastpdf-1.0.0/fastpdf/
+-rw-rw-r--   0 ko        (1000) ko        (1000)       68 2023-06-29 11:16:02.000000 fastpdf-1.0.0/fastpdf/__init__.py
+-rw-rw-r--   0 ko        (1000) ko        (1000)    36041 2023-07-17 15:11:41.000000 fastpdf-1.0.0/fastpdf/api.py
+-rw-rw-r--   0 ko        (1000) ko        (1000)      671 2023-06-29 11:15:01.000000 fastpdf-1.0.0/fastpdf/exceptions.py
+-rw-rw-r--   0 ko        (1000) ko        (1000)     4015 2023-07-19 11:30:28.000000 fastpdf-1.0.0/fastpdf/models.py
+drwxrwxr-x   0 ko        (1000) ko        (1000)        0 2023-07-26 07:11:45.247278 fastpdf-1.0.0/fastpdf.egg-info/
+-rw-rw-r--   0 ko        (1000) ko        (1000)    13814 2023-07-26 07:11:45.000000 fastpdf-1.0.0/fastpdf.egg-info/PKG-INFO
+-rw-rw-r--   0 ko        (1000) ko        (1000)      247 2023-07-26 07:11:45.000000 fastpdf-1.0.0/fastpdf.egg-info/SOURCES.txt
+-rw-rw-r--   0 ko        (1000) ko        (1000)        1 2023-07-26 07:11:45.000000 fastpdf-1.0.0/fastpdf.egg-info/dependency_links.txt
+-rw-rw-r--   0 ko        (1000) ko        (1000)       22 2023-07-26 07:11:45.000000 fastpdf-1.0.0/fastpdf.egg-info/requires.txt
+-rw-rw-r--   0 ko        (1000) ko        (1000)        8 2023-07-26 07:11:45.000000 fastpdf-1.0.0/fastpdf.egg-info/top_level.txt
+-rw-rw-r--   0 ko        (1000) ko        (1000)       38 2023-07-26 07:11:45.247278 fastpdf-1.0.0/setup.cfg
+-rw-rw-r--   0 ko        (1000) ko        (1000)     1026 2023-07-26 07:11:41.000000 fastpdf-1.0.0/setup.py
```

### Comparing `fastpdf-0.0.2/fastpdf/exceptions.py` & `fastpdf-1.0.0/fastpdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastpdf-0.0.2/fastpdf/models.py` & `fastpdf-1.0.0/fastpdf/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     flask = "flask"
     chrome = "chrome"
     webkit = "webkit"
     
 
 @dataclass
 class StyleFile:
-    format: str
+    format: str = field(default="css")
     description: Optional[str] = field(default="fastpdf-python StyleFile")
     stylesheet_file: Optional[bytes] = field(default=None)
     id: Optional[str] = field(default=None)
     number: Optional[int] = field(default=None)
     timestamp: Optional[datetime.datetime] = field(default=None)
     template_name: Optional[str] = field(default=None)
     template_id: Optional[str] = field(default=None)
@@ -44,26 +44,26 @@
     template_name: Optional[str] = field(default=None)
     template_id: Optional[str] = field(default=None)
 
 
 @dataclass
 class Template:
     name: str
-    format: str
+    format: str = field(default="html")
     description: Optional[str] = field(default="fastpdf-python Template")
     id: Optional[str] = field(default=None)
     #style_files: list[StyleFile]
     #image_files: list[ImageFile]
     #template_file: Optional[bytes]
     header_file: Optional[bytes] = field(default=None)
     footer_file: Optional[bytes] = field(default=None)
     
     landscape: Optional[bool] = field(default=None)
     paper_format: Optional[str] = field(default=None)
-    background: Optional[bool] = field(default=None)
+    print_background: Optional[bool] = field(default=None)
     page_range: Optional[str] = field(default=None)
     scale: Optional[float] = field(default=None)
     
     margin_top: Optional[float] = field(default=None)
     margin_right: Optional[float] = field(default=None)
     margin_bottom: Optional[float] = field(default=None)
     margin_left: Optional[float] = field(default=None)
@@ -80,15 +80,15 @@
     display_header_footer: Optional[bool] = field(default=None)
 
     header_file: Optional[bytes] = field(default=None)
     footer_file: Optional[bytes] = field(default=None)
     
     landscape: Optional[bool] = field(default=None)
     paper_format: Optional[str] = field(default=None)
-    background: Optional[bool] = field(default=None)
+    print_background: Optional[bool] = field(default=None)
     page_range: Optional[str] = field(default=None)
     scale: Optional[float] = field(default=None)
     
     margin_top: Optional[float] = field(default=None)
     margin_right: Optional[float] = field(default=None)
     margin_bottom: Optional[float] = field(default=None)
     margin_left: Optional[float] = field(default=None)
```

### Comparing `fastpdf-0.0.2/setup.py` & `fastpdf-1.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
     
 setup(
     name='fastpdf',
-    version='0.0.2',
+    version='1.0.0',
     url='https://github.com/fastpdfservices/fastpdf-python',
     author='Korian',
     author_email='korian@fastpdfservice.com',
-    description='SDK for PDF rendering, generation & transformation via Fast PDF Service. Visit https://fastpdfservice.com',
+    description='SDK for PDF rendering, generation & transformation via Fast PDF Service.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     packages=find_packages(),    
     install_requires=[
      'requests',
      'python-magic'
```


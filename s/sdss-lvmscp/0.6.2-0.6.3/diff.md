# Comparing `tmp/sdss_lvmscp-0.6.2.tar.gz` & `tmp/sdss_lvmscp-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_lvmscp-0.6.2.tar", max compression
+gzip compressed data, was "sdss_lvmscp-0.6.3.tar", max compression
```

## Comparing `sdss_lvmscp-0.6.2.tar` & `sdss_lvmscp-0.6.3.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1504 2023-07-26 18:46:34.225582 sdss_lvmscp-0.6.2/LICENSE.md
--rw-r--r--   0        0        0     1578 2023-07-26 18:46:34.225822 sdss_lvmscp-0.6.2/README.md
--rw-r--r--   0        0        0     2715 2023-07-26 18:46:34.296863 sdss_lvmscp-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      369 2023-07-26 18:46:34.297312 sdss_lvmscp-0.6.2/python/lvmscp/__init__.py
--rw-r--r--   0        0        0     1618 2023-07-26 18:46:34.297615 sdss_lvmscp-0.6.2/python/lvmscp/__main__.py
--rw-r--r--   0        0        0      258 2023-07-26 18:46:34.297978 sdss_lvmscp-0.6.2/python/lvmscp/actor/__init__.py
--rw-r--r--   0        0        0     8321 2023-07-26 18:46:34.298249 sdss_lvmscp-0.6.2/python/lvmscp/actor/actor.py
--rw-r--r--   0        0        0      859 2023-07-26 18:46:34.298549 sdss_lvmscp-0.6.2/python/lvmscp/actor/commands/__init__.py
--rw-r--r--   0        0        0     1515 2023-07-26 18:46:34.298778 sdss_lvmscp-0.6.2/python/lvmscp/actor/commands/expose.py
--rw-r--r--   0        0        0     3827 2023-07-26 18:46:34.298987 sdss_lvmscp-0.6.2/python/lvmscp/actor/commands/focus.py
--rw-r--r--   0        0        0     1272 2023-07-26 18:46:34.299188 sdss_lvmscp-0.6.2/python/lvmscp/actor/commands/hardware_status.py
--rw-r--r--   0        0        0      758 2023-07-26 18:46:34.299399 sdss_lvmscp-0.6.2/python/lvmscp/controller.py
--rw-r--r--   0        0        0    14890 2023-07-26 18:46:34.299726 sdss_lvmscp-0.6.2/python/lvmscp/delegate.py
--rw-r--r--   0        0        0    40889 2023-07-26 18:46:34.300173 sdss_lvmscp-0.6.2/python/lvmscp/etc/LVM_100kHz.acf
--rw-r--r--   0        0        0     5736 2023-07-26 18:46:34.301624 sdss_lvmscp-0.6.2/python/lvmscp/etc/lvmscp.yml
--rw-r--r--   0        0        0      161 2023-07-26 18:46:34.301857 sdss_lvmscp-0.6.2/python/lvmscp/etc/schema.json
--rw-r--r--   0        0        0    18807 2023-07-26 18:46:34.302143 sdss_lvmscp-0.6.2/python/lvmscp/ln2.py
--rw-r--r--   0        0        0     2812 1970-01-01 00:00:00.000000 sdss_lvmscp-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-26 19:25:37.157604 sdss_lvmscp-0.6.3/LICENSE.md
+-rw-r--r--   0        0        0     1578 2023-07-26 19:25:37.157880 sdss_lvmscp-0.6.3/README.md
+-rw-r--r--   0        0        0     2673 2023-07-26 19:25:37.202549 sdss_lvmscp-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      369 2023-07-26 19:25:37.203053 sdss_lvmscp-0.6.3/python/lvmscp/__init__.py
+-rw-r--r--   0        0        0     1618 2023-07-26 19:25:37.203359 sdss_lvmscp-0.6.3/python/lvmscp/__main__.py
+-rw-r--r--   0        0        0      258 2023-07-26 19:25:37.203767 sdss_lvmscp-0.6.3/python/lvmscp/actor/__init__.py
+-rw-r--r--   0        0        0     3455 2023-07-26 19:25:37.204035 sdss_lvmscp-0.6.3/python/lvmscp/actor/actor.py
+-rw-r--r--   0        0        0      859 2023-07-26 19:25:37.204392 sdss_lvmscp-0.6.3/python/lvmscp/actor/commands/__init__.py
+-rw-r--r--   0        0        0     3827 2023-07-26 19:25:37.204684 sdss_lvmscp-0.6.3/python/lvmscp/actor/commands/focus.py
+-rw-r--r--   0        0        0     1272 2023-07-26 19:25:37.204961 sdss_lvmscp-0.6.3/python/lvmscp/actor/commands/hardware_status.py
+-rw-r--r--   0        0        0      758 2023-07-26 19:25:37.205411 sdss_lvmscp-0.6.3/python/lvmscp/controller.py
+-rw-r--r--   0        0        0    14890 2023-07-26 19:25:37.205762 sdss_lvmscp-0.6.3/python/lvmscp/delegate.py
+-rw-r--r--   0        0        0    40889 2023-07-26 19:25:37.206165 sdss_lvmscp-0.6.3/python/lvmscp/etc/LVM_100kHz.acf
+-rw-r--r--   0        0        0     5502 2023-07-26 19:25:37.206522 sdss_lvmscp-0.6.3/python/lvmscp/etc/lvmscp.yml
+-rw-r--r--   0        0        0      161 2023-07-26 19:25:37.206710 sdss_lvmscp-0.6.3/python/lvmscp/etc/schema.json
+-rw-r--r--   0        0        0    18807 2023-07-26 19:25:37.207019 sdss_lvmscp-0.6.3/python/lvmscp/ln2.py
+-rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 sdss_lvmscp-0.6.3/PKG-INFO
```

### Comparing `sdss_lvmscp-0.6.2/LICENSE.md` & `sdss_lvmscp-0.6.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.2/README.md` & `sdss_lvmscp-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.2/pyproject.toml` & `sdss_lvmscp-0.6.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-lvmscp"
-version = "0.6.2"
+version = "0.6.3"
 description = "LVM spectrograph control package."
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>", "Changgon Kim <changgonkim@khu.ac.kr>"]
 maintainers = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmscp"
 repository = "https://github.com/sdss/lvmscp"
@@ -29,16 +29,14 @@
 lvmscp = "lvmscp.__main__:main"
 ln2fill = "lvmscp.ln2:ln2fill"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 click-default-group = "^1.2.2"
 sdss-archon = "^0.11.0"
-httpx = ">=0.18.1"
-Authlib = ">=1.0.0rc1"
 
 [tool.poetry.dev-dependencies]
 ipython = ">=7.11.0"
 flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
 isort = ">=4.3.21"
 ipdb = ">=0.12.3"
```

### Comparing `sdss_lvmscp-0.6.2/python/lvmscp/__main__.py` & `sdss_lvmscp-0.6.3/python/lvmscp/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.2/python/lvmscp/actor/commands/__init__.py` & `sdss_lvmscp-0.6.3/python/lvmscp/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.2/python/lvmscp/actor/commands/focus.py` & `sdss_lvmscp-0.6.3/python/lvmscp/actor/commands/focus.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.2/python/lvmscp/actor/commands/hardware_status.py` & `sdss_lvmscp-0.6.3/python/lvmscp/actor/commands/hardware_status.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.2/python/lvmscp/controller.py` & `sdss_lvmscp-0.6.3/python/lvmscp/controller.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.2/python/lvmscp/delegate.py` & `sdss_lvmscp-0.6.3/python/lvmscp/delegate.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.2/python/lvmscp/etc/LVM_100kHz.acf` & `sdss_lvmscp-0.6.3/python/lvmscp/etc/LVM_100kHz.acf`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.2/python/lvmscp/etc/lvmscp.yml` & `sdss_lvmscp-0.6.3/python/lvmscp/etc/lvmscp.yml`

 * *Files 13% similar despite different names*

```diff
@@ -136,17 +136,14 @@
       MOD12\HEATERATARGET: -112
       MOD12\HEATERBTARGET: -117
     sp3:
       MOD2\HEATERATARGET: -109.5
       MOD12\HEATERATARGET: -111.5
       MOD12\HEATERBTARGET: -110.5
 
-# Write a log for each exposure (requires files.lab_log to be set).
-write_log: true
-
 # The base directory where the data will be saved (and MJD subdirectory is always added)
 # and the format of the saved filename. Available placeholders are {observatory} which
 # is replaced with "apo" or "lco", {hemisphere} replaced with "n" if the observatory is
 # "apo" and "s" if "lco", {controller} which is replaced with the name of the Archon
 # controller defined above, {ccd} which is the name do the CCD (including the controller
 # identifier), and {exposure} which is a never-repeating sequence identifier. "split"
 # controls whether the CCD frames from each controller are saved as individual files
@@ -156,21 +153,15 @@
   split: true
   template: 'sdR-{hemisphere}-{ccd}-{exposure_no:08d}.fits.gz'
 
 checksum:
   write: true
   mode: md5
 
-credentials_file: ~/.config/sdss/lvmscp_credentials.yml
-
-exposure_list:
-  id: 103BNxjlZ59Sob3jDO4EN1z6zp2q5YrYA6nTjGlZM6XY
-  sheet:
-    sp2: 'Spec 2'
-    sp3: 'Spec 3'
+status_delay: 30.0
 
 # Actor configuration for the AMQPActor class
 actor:
   name: lvmscp
   host: localhost
   port: 5672
   log_dir: '/data/logs/lvmscp'
```

### Comparing `sdss_lvmscp-0.6.2/python/lvmscp/ln2.py` & `sdss_lvmscp-0.6.3/python/lvmscp/ln2.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.6.2/PKG-INFO` & `sdss_lvmscp-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-lvmscp
-Version: 0.6.2
+Version: 0.6.3
 Summary: LVM spectrograph control package.
 Home-page: https://github.com/sdss/lvmscp
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Maintainer: José Sánchez-Gallego
@@ -17,17 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: Authlib (>=1.0.0rc1)
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
-Requires-Dist: httpx (>=0.18.1)
 Requires-Dist: sdss-archon (>=0.11.0,<0.12.0)
 Project-URL: Documentation, https://sdss-lvmscp.readthedocs.org
 Project-URL: Repository, https://github.com/sdss/lvmscp
 Description-Content-Type: text/markdown
 
 # lvmscp
```


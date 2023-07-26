# Comparing `tmp/c4m_flexcell-0.4.0.dev3.tar.gz` & `tmp/c4m_flexcell-0.4.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4m_flexcell-0.4.0.dev3.tar", last modified: Sat Jun 24 19:34:06 2023, max compression
+gzip compressed data, was "c4m_flexcell-0.4.0.dev9.tar", last modified: Wed Jul 26 13:21:54 2023, max compression
```

## Comparing `c4m_flexcell-0.4.0.dev3.tar` & `c4m_flexcell-0.4.0.dev9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.517446 c4m_flexcell-0.4.0.dev3/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       96 2022-07-12 15:00:24.000000 c4m_flexcell-0.4.0.dev3/.gitignore
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1264 2023-06-24 18:59:02.000000 c4m_flexcell-0.4.0.dev3/.gitlab-ci.yml
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      484 2020-07-06 13:05:29.000000 c4m_flexcell-0.4.0.dev3/COPYRIGHT.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      782 2021-03-14 14:00:40.000000 c4m_flexcell-0.4.0.dev3/LICENSE.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.509446 c4m_flexcell-0.4.0.dev3/LICENSES/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2021-03-14 14:00:40.000000 c4m_flexcell-0.4.0.dev3/LICENSES/agpl-3.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2020-07-06 09:58:12.000000 c4m_flexcell-0.4.0.dev3/LICENSES/cern_ohl_s_v2.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2021-03-14 14:00:40.000000 c4m_flexcell-0.4.0.dev3/LICENSES/gpl-2.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4355 2023-06-24 19:34:06.517446 c4m_flexcell-0.4.0.dev3/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3878 2023-06-24 18:59:02.000000 c4m_flexcell-0.4.0.dev3/README.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.513446 c4m_flexcell-0.4.0.dev3/ReleaseNotes/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      321 2021-03-14 14:00:41.000000 c4m_flexcell-0.4.0.dev3/ReleaseNotes/v0.0.4.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      462 2022-08-22 13:25:11.000000 c4m_flexcell-0.4.0.dev3/ReleaseNotes/v0.1.0.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.513446 c4m_flexcell-0.4.0.dev3/c4m/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      149 2021-03-14 14:00:40.000000 c4m_flexcell-0.4.0.dev3/c4m/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2247 2021-05-15 12:46:28.000000 c4m_flexcell-0.4.0.dev3/c4m/cell_canvas.ipynb
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.513446 c4m_flexcell-0.4.0.dev3/c4m/flexcell/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      129 2023-05-26 12:28:32.000000 c4m_flexcell-0.4.0.dev3/c4m/flexcell/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)   509363 2023-06-24 19:24:29.000000 c4m_flexcell-0.4.0.dev3/c4m/flexcell/_cells.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    89759 2023-06-24 19:24:29.000000 c4m_flexcell-0.4.0.dev3/c4m/flexcell/activecolumnscell.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    11848 2023-06-24 19:24:29.000000 c4m_flexcell-0.4.0.dev3/c4m/flexcell/canvas.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4297 2023-06-24 19:24:29.000000 c4m_flexcell-0.4.0.dev3/c4m/flexcell/cell.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)   126383 2023-06-24 19:24:29.000000 c4m_flexcell-0.4.0.dev3/c4m/flexcell/factory.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    52730 2023-05-09 10:49:53.000000 c4m_flexcell-0.4.0.dev3/c4m/flexcell/stdcell.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.517446 c4m_flexcell-0.4.0.dev3/c4m_flexcell.egg-info/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4355 2023-06-24 19:34:06.000000 c4m_flexcell-0.4.0.dev3/c4m_flexcell.egg-info/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      764 2023-06-24 19:34:06.000000 c4m_flexcell-0.4.0.dev3/c4m_flexcell.egg-info/SOURCES.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-06-24 19:34:06.000000 c4m_flexcell-0.4.0.dev3/c4m_flexcell.egg-info/dependency_links.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       28 2023-06-24 19:34:06.000000 c4m_flexcell-0.4.0.dev3/c4m_flexcell.egg-info/requires.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        4 2023-06-24 19:34:06.000000 c4m_flexcell-0.4.0.dev3/c4m_flexcell.egg-info/top_level.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        6 2022-11-01 15:19:21.000000 c4m_flexcell-0.4.0.dev3/ci-requirements.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2022-09-30 12:33:15.000000 c4m_flexcell-0.4.0.dev3/dev-requirements.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2133 2023-06-24 16:45:30.000000 c4m_flexcell-0.4.0.dev3/dodo.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      165 2021-03-14 14:00:40.000000 c4m_flexcell-0.4.0.dev3/run_unittests.sh
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-06-24 19:34:06.517446 c4m_flexcell-0.4.0.dev3/setup.cfg
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1387 2023-06-24 19:24:22.000000 c4m_flexcell-0.4.0.dev3/setup.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.517446 c4m_flexcell-0.4.0.dev3/test/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       84 2021-03-14 14:00:40.000000 c4m_flexcell-0.4.0.dev3/test/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.517446 c4m_flexcell-0.4.0.dev3/test/interactive/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       16 2020-07-14 09:04:04.000000 c4m_flexcell-0.4.0.dev3/test/interactive/.gitignore
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2683 2020-10-06 14:32:17.000000 c4m_flexcell-0.4.0.dev3/test/interactive/export.ipynb
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.517446 c4m_flexcell-0.4.0.dev3/test/unit/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       84 2021-03-14 14:00:40.000000 c4m_flexcell-0.4.0.dev3/test/unit/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2762 2023-03-03 17:44:42.000000 c4m_flexcell-0.4.0.dev3/test/unit/test_library.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 13:21:54.000337 c4m_flexcell-0.4.0.dev9/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       96 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/.gitignore
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1282 2023-07-26 13:12:03.000000 c4m_flexcell-0.4.0.dev9/.gitlab-ci.yml
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      484 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/COPYRIGHT.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      782 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/LICENSE.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 13:21:53.992336 c4m_flexcell-0.4.0.dev9/LICENSES/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/LICENSES/agpl-3.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/LICENSES/cern_ohl_s_v2.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/LICENSES/gpl-2.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4355 2023-07-26 13:21:54.000337 c4m_flexcell-0.4.0.dev9/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3878 2023-07-26 13:11:36.000000 c4m_flexcell-0.4.0.dev9/README.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 13:21:53.996337 c4m_flexcell-0.4.0.dev9/ReleaseNotes/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      321 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/ReleaseNotes/v0.0.4.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      462 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/ReleaseNotes/v0.1.0.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 13:21:53.996337 c4m_flexcell-0.4.0.dev9/c4m/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      149 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/c4m/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2247 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/c4m/cell_canvas.ipynb
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 13:21:53.996337 c4m_flexcell-0.4.0.dev9/c4m/flexcell/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      129 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/c4m/flexcell/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)   509363 2023-07-26 13:11:36.000000 c4m_flexcell-0.4.0.dev9/c4m/flexcell/_cells.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    90343 2023-07-26 13:12:03.000000 c4m_flexcell-0.4.0.dev9/c4m/flexcell/activecolumnscell.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13337 2023-07-26 13:20:53.000000 c4m_flexcell-0.4.0.dev9/c4m/flexcell/canvas.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4297 2023-07-26 13:11:36.000000 c4m_flexcell-0.4.0.dev9/c4m/flexcell/cell.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)   127811 2023-07-26 13:12:03.000000 c4m_flexcell-0.4.0.dev9/c4m/flexcell/factory.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    52730 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/c4m/flexcell/stdcell.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 13:21:54.000337 c4m_flexcell-0.4.0.dev9/c4m_flexcell.egg-info/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4355 2023-07-26 13:21:53.000000 c4m_flexcell-0.4.0.dev9/c4m_flexcell.egg-info/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      764 2023-07-26 13:21:53.000000 c4m_flexcell-0.4.0.dev9/c4m_flexcell.egg-info/SOURCES.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-07-26 13:21:53.000000 c4m_flexcell-0.4.0.dev9/c4m_flexcell.egg-info/dependency_links.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       28 2023-07-26 13:21:53.000000 c4m_flexcell-0.4.0.dev9/c4m_flexcell.egg-info/requires.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        4 2023-07-26 13:21:53.000000 c4m_flexcell-0.4.0.dev9/c4m_flexcell.egg-info/top_level.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        6 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/ci-requirements.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/dev-requirements.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2161 2023-07-26 13:12:03.000000 c4m_flexcell-0.4.0.dev9/dodo.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      165 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/run_unittests.sh
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-07-26 13:21:54.000337 c4m_flexcell-0.4.0.dev9/setup.cfg
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1387 2023-07-26 13:12:03.000000 c4m_flexcell-0.4.0.dev9/setup.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 13:21:54.000337 c4m_flexcell-0.4.0.dev9/test/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       84 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/test/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 13:21:54.000337 c4m_flexcell-0.4.0.dev9/test/interactive/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       16 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/test/interactive/.gitignore
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2683 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/test/interactive/export.ipynb
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 13:21:54.000337 c4m_flexcell-0.4.0.dev9/test/unit/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       84 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/test/unit/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2762 2023-07-14 12:23:34.000000 c4m_flexcell-0.4.0.dev9/test/unit/test_library.py
```

### Comparing `c4m_flexcell-0.4.0.dev3/.gitlab-ci.yml` & `c4m_flexcell-0.4.0.dev9/.gitlab-ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -15,29 +15,30 @@
   - pip install pyinotify # needed for doit and does not have binary
   - pip install --only-binary ":all:" -r dev-requirements.txt
   - pip install --only-binary ":all:" -r ci-requirements.txt
 
 dist:
   only:
     - main
-    - dev_*
+    - dev_v0.4
   variables:
     TWINE_PASSWORD: '${CI_JOB_TOKEN}'
     TWINE_USERNAME: 'gitlab-ci-token'
     TWINE_REPOSITORY_URL: 'https://gitlab.com/api/v4/projects/${CI_PROJECT_ID}/packages/pypi'
   script:
     # Need to fetch tags
     - git fetch --depth=1 origin +refs/tags/*:refs/tags/*
     - doit dist
     - python -m twine check --strict dist/*
     - python -m twine upload --verbose dist/*
 
 dist-test:
   except:
     - main
+    - dev_v0.4
   script:
     # Need to fetch tags
     - git fetch --depth=1 origin +refs/tags/*:refs/tags/*
     - doit dist
     - python -m twine check --strict dist/*
 
 install:
```

### Comparing `c4m_flexcell-0.4.0.dev3/LICENSE.md` & `c4m_flexcell-0.4.0.dev9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.4.0.dev3/LICENSES/agpl-3.0.txt` & `c4m_flexcell-0.4.0.dev9/LICENSES/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.4.0.dev3/LICENSES/cern_ohl_s_v2.txt` & `c4m_flexcell-0.4.0.dev9/LICENSES/cern_ohl_s_v2.txt`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.4.0.dev3/LICENSES/gpl-2.0.txt` & `c4m_flexcell-0.4.0.dev9/LICENSES/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.4.0.dev3/PKG-INFO` & `c4m_flexcell-0.4.0.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4m_flexcell
-Version: 0.4.0.dev3
+Version: 0.4.0.dev9
 Summary: PDKMaster based scalable standard cell library
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/c4m-flexcell
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/c4m-flexcell/issues
 Requires-Python: ~=3.6
```

### Comparing `c4m_flexcell-0.4.0.dev3/README.md` & `c4m_flexcell-0.4.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.4.0.dev3/c4m/cell_canvas.ipynb` & `c4m_flexcell-0.4.0.dev9/c4m/cell_canvas.ipynb`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.4.0.dev3/c4m/flexcell/_cells.py` & `c4m_flexcell-0.4.0.dev9/c4m/flexcell/_cells.py`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.4.0.dev3/c4m/flexcell/activecolumnscell.py` & `c4m_flexcell-0.4.0.dev9/c4m/flexcell/activecolumnscell.py`

 * *Files 1% similar despite different names*

```diff
@@ -2133,15 +2133,15 @@
             shape = _geo.Rect(left=left, bottom=bottom, right=right, top=top)
             layouter.add_portless(prim=nimplant, shape=shape)
         # Draw implants
         if pimplant is not None:
             enc = canvas._min_active_pimplant_enc.first
             left = -enc
             right = width + enc
-            top = ac_canvas._pact_top + canvas._min_nsd_enc.second
+            top = ac_canvas._pact_top + canvas._min_psd_enc.second
             bottom = canvas._well_edge_height
             shape = _geo.Rect(left=left, bottom=bottom, right=right, top=top)
             layouter.add_portless(prim=pimplant, shape=shape)
 
     def _add_taps(self) -> None:
         cell = self.cell
         tech = cell.tech
@@ -2149,45 +2149,69 @@
         layouter = cell.layouter
 
         width = cell.width
 
         pwell = canvas._pwell
         nwell = canvas._nwell
         nimplant = canvas._nimplant
-        nenc = canvas._min_active_nimplant_enc.wide()
+        nenc = (
+            canvas._min_active_nimplant_enc.wide()
+            if canvas._min_active_nimplant_enc is not None
+            else None
+        )
         pimplant = canvas._pimplant
-        penc = canvas._min_active_pimplant_enc.wide()
+        penc = (
+            canvas._min_active_pimplant_enc.wide()
+            if canvas._min_active_pimplant_enc is not None
+            else None
+        )
         active = canvas._active
         contact = canvas._contact
         metal1 = canvas._metal1
 
         tap_height = tech.computed.min_width(active, up=True, min_enclosure=True)
 
         # ntap
-        act_left = 0.5*pimplant.min_space + penc.first
+        act_left = (
+            0.5*pimplant.min_space + penc.first
+            if pimplant is not None
+            else active.min_space
+        )
         act_right = width - act_left
-        act_bottom = 0.5*pimplant.min_space + penc.second
+        act_bottom = (
+            0.5*pimplant.min_space + penc.second
+            if pimplant is not None
+            else active.min_space
+        )
         act_top = act_bottom + tap_height
         layouter.add_wire(
             net=cell.vss, well_net=cell.pwell_net, wire=contact,
             bottom=active, bottom_well=pwell, bottom_enclosure="wide",
             bottom_implant=pimplant, bottom_implant_enclosure=nenc,
             bottom_left=act_left, bottom_bottom=act_bottom,
             bottom_right=act_right, bottom_top=act_top,
         )
 
         # ptap
-        act_left = 0.5*nimplant.min_space + nenc.first
+        act_left = (
+            0.5*nimplant.min_space + nenc.first
+            if nimplant is not None
+            else active.min_space
+        )
         act_right = width - act_left
-        act_top = canvas._cell_height - (0.5*nimplant.min_space + nenc.second)
+        act_top = canvas._cell_height - (
+            0.5*nimplant.min_space + nenc.second
+            if nimplant is not None
+            else active.min_space
+        )
         act_bottom = act_top - tap_height
         layouter.add_wire(
             net=cell.vdd, well_net=cell.nwell_net, wire=contact,
             bottom=active, bottom_well=nwell, bottom_enclosure="wide",
-            bottom_implant=nimplant, bottom_implant_enclosure=penc,
+            bottom_implant=nimplant, bottom_implant_enclosure=nenc,
             bottom_left=act_left, bottom_bottom=act_bottom,
             bottom_right=act_right, bottom_top=act_top,
         )
 
     def log(self, *args):
         print(f"[{self.cell.name}:Constraints]", *args)
 ConstraintsT = _Constraints
```

### Comparing `c4m_flexcell-0.4.0.dev3/c4m/flexcell/canvas.py` & `c4m_flexcell-0.4.0.dev9/c4m/flexcell/canvas.py`

 * *Files 16% similar despite different names*

```diff
@@ -53,15 +53,20 @@
         inside_enclosure: OptMultiT[_prp.Enclosure]=None,
     ):
         if nmos not in tech.primitives:
             raise ValueError(
                 f"provided nmos transistor {nmos.name} not of technology '{tech.name}'",
             )
         if nimplant is None:
-            nimplant = nmos.implant[0]
+            try:
+                nimplant = nmos.implant[0]
+            except:
+                pass
+            else:
+                assert nimplant.type_ == _prm.nImpl
         else:
             if nimplant.type_ != _prm.nImpl:
                 raise ValueError(
                     f"nimplant '{nimplant.name}' is not n type",
                 )
             if nimplant not in nmos.implant:
                 raise NotImplementedError(
@@ -69,25 +74,33 @@
                 )
 
         if pmos not in tech.primitives:
             raise ValueError(
                 f"provided pmos transistor {pmos.name} not of technology '{tech.name}'",
             )
         if pimplant is None:
-            pimplant = pmos.implant[0]
+            try:
+                pimplant = pmos.implant[0]
+            except:
+                pass
+            else:
+                assert pimplant.type_ == _prm.pImpl
         else:
             if pimplant.type_ != _prm.pImpl:
                 raise ValueError(
                     f"pimplant '{pimplant.name}' is not p type",
                 )
             if pimplant not in pmos.implant:
                 raise NotImplementedError(
                     f"pimplant '{pimplant.name}' not part of pmos implants"
                 )
 
+        if (nimplant is None) and (pimplant is None):
+            raise ValueError("both nimplant and pimplant are None")
+
         if l is None:
             l = nmos.computed.min_l
             if nmos.computed.min_l != pmos.computed.min_l:
                 raise NotImplementedError(
                     "Differing minimal l of nmos and pmos"
                 )
         else:
@@ -141,31 +154,65 @@
         if poly != pmos.gate.poly:
             raise NotImplementedError(
                 "Different poly wire for nmos and pmos transistor"
             )
 
         self._min_active_poly_space = tech.computed.min_space(active, poly)
 
+        self._nactive = nactive = active if nimplant is None else active.in_(nimplant)
+        self._pactive = pactive = active if pimplant is None else active.in_(pimplant)
+
+        self._min_nactive_pactive_space = tech.computed.min_space(nactive, pactive)
+        self._min_nactive_pactive_space_maxenc = tech.computed.min_space(
+            nactive, pactive, max_enclosure=True,
+        )
+
         # Draw SD regions with vertical implant enclosure the same as the
         # gate implant enclosure
-        gate_enc = nmos.min_gateimplant_enclosure[0]
-        idx = active.implant.index(nimplant)
-        act_enc = active.min_implant_enclosure[idx]
+        try:
+            gate_enc = nmos.min_gateimplant_enclosure[0]
+        except:
+            gate_enc = None
+        try:
+            idx = active.implant.index(nimplant)
+            act_enc = active.min_implant_enclosure[idx]
+        except:
+            act_enc = None
         self._min_active_nimplant_enc = act_enc
-        self._min_nsd_enc = _prp.Enclosure((
-            act_enc.first, max(act_enc.min(), gate_enc.second),
-        ))
-
-        gate_enc = nmos.min_gateimplant_enclosure[0]
-        idx = active.implant.index(pimplant)
-        act_enc = active.min_implant_enclosure[idx]
+        if gate_enc is None:
+            if act_enc is None:
+                self._min_nsd_enc = None
+            else:
+                self._min_nsd_enc = act_enc
+        else:
+            assert act_enc is not None
+            self._min_nsd_enc = _prp.Enclosure((
+                act_enc.first, max(act_enc.min(), gate_enc.second),
+            ))
+
+        try:
+            gate_enc = pmos.min_gateimplant_enclosure[0]
+        except:
+            gate_enc = None
+        try:
+            idx = active.implant.index(pimplant)
+            act_enc = active.min_implant_enclosure[idx]
+        except:
+            act_enc = None
         self._min_active_pimplant_enc = act_enc
-        self._min_psd_enc = _prp.Enclosure((
-            act_enc.first, max(act_enc.min(), gate_enc.second),
-        ))
+        if gate_enc is None:
+            if act_enc is None:
+                self._min_psd_enc = None
+            else:
+                self._min_psd_enc = act_enc
+        else:
+            assert act_enc is not None
+            self._min_psd_enc = _prp.Enclosure((
+                act_enc.first, max(act_enc.min(), gate_enc.second),
+            ))
 
         self._vias = vias = tuple(tech.primitives.__iter_type__(_prm.Via))
         self._contact = cont = vias[0]
         min_contact_active_space = None
         try:
             min_contact_active_space = tech.computed.min_space(
                 primitive1=cont, primitive2=active,
```

### Comparing `c4m_flexcell-0.4.0.dev3/c4m/flexcell/cell.py` & `c4m_flexcell-0.4.0.dev9/c4m/flexcell/cell.py`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.4.0.dev3/c4m/flexcell/factory.py` & `c4m_flexcell-0.4.0.dev9/c4m/flexcell/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,17 +88,22 @@
 
             # vdd min tap
             l_ch = layouter.wire_layout(
                 net=vdd, well_net=vdd, wire=contact, rows=canvas._min_tap_chs,
                 bottom=active, bottom_implant=nimplant, bottom_well=nwell,
                 bottom_enclosure="wide",
             )
-            impl_bb = l_ch.bounds(mask=nimplant.mask)
             x = 0.5*cell_width
-            y = canvas._cell_height - 0.5*pimplant.min_space - impl_bb.top
+            if nimplant is not None:
+                impl_bb = l_ch.bounds(mask=nimplant.mask)
+                y = canvas._cell_height - 0.5*nimplant.min_space - impl_bb.top
+            else:
+                # TODO: Proper value
+                act_bb = l_ch.bounds(mask=active.mask)
+                y = canvas._cell_height - active.min_space - act_bb.top
             vdd_tap_lay = layouter.place(object_=l_ch, x=x, y=y)
 
             if max_poly:
                 # Add big poly
                 vss_dio_tap_bb = vss_tap_lay.bounds(mask=active.mask)
                 vdd_dio_tap_bb = vdd_tap_lay.bounds(mask=active.mask)
                 left = 0.5*poly.min_space
@@ -124,74 +129,97 @@
                 if vss_polych_m1_bb.bottom > canvas._m1_vssrail_width:
                     layouter.add_wire(net=vss, wire=metal1, shape=_geo.Rect.from_rect(
                         rect=vss_polych_m1_bb, bottom=0.0,
                     ))
         else: # max_diff == True
             # vss tap
             # First create ch to compute dimension of big diode
-            l_ch = layouter.wire_layout(
-                net=vss, wire=contact, bottom=active, bottom_implant=pimplant,
-            )
-            impl_bb = l_ch.bounds(mask=pimplant.mask)
-            impl_w = impl_bb.width
-            # Compute the possible hor. expansion
-            d = cell_width - impl_w - pimplant.min_space
-            assert tech.on_grid(d) >= 0.0
-            act_bb = l_ch.bounds(mask=active.mask)
-            # Maximize width
-            act_w = act_bb.width + d
-            # Maximize height
-            enc = act_bb.bottom - impl_bb.bottom
-            bottom = 0.5*pimplant.min_space + enc
-            top = canvas._well_edge_height - min_actwell_space
-            act_h = tech.on_grid(
-                top - bottom, mult=2, rounding="floor",
-            )
+            if pimplant is not None:
+                l_ch = layouter.wire_layout(
+                    net=vss, wire=contact, bottom=active, bottom_implant=pimplant,
+                )
+                impl_bb = l_ch.bounds(mask=pimplant.mask)
+                impl_w = impl_bb.width
+                # Compute the possible hor. expansion
+                d = cell_width - impl_w - pimplant.min_space
+                assert tech.on_grid(d) >= 0.0
+                act_bb = l_ch.bounds(mask=active.mask)
+                # Maximize width
+                act_w = act_bb.width + d
+                # Maximize height
+                enc = act_bb.bottom - impl_bb.bottom
+                bottom = 0.5*pimplant.min_space + enc
+                top = canvas._well_edge_height - min_actwell_space
+                act_h = tech.on_grid(
+                    top - bottom, mult=2, rounding="floor",
+                )
+            else:
+                act_w = cell_width - 2*active.min_space
+                bottom = active.min_space
+                top = canvas._well_edge_height - min_actwell_space
+                act_h = tech.on_grid(
+                    top - bottom, mult=2, rounding="floor",
+                )
 
             # diode with right dimensions
             l_ch = layouter.wire_layout(
                 net=vss, wire=contact, bottom=active, bottom_implant=pimplant,
                 bottom_width=act_w, bottom_height=act_h,
             )
-            impl_bb = l_ch.bounds(mask=pimplant.mask)
             x = 0.5*cell_width
-            y = 0.5*pimplant.min_space - impl_bb.bottom
+            if pimplant is not None:
+                impl_bb = l_ch.bounds(mask=pimplant.mask)
+                y = 0.5*pimplant.min_space - impl_bb.bottom
+            else:
+                act_bb = l_ch.bounds(mask=active.mask)
+                y = active.min_space - act_bb.bottom
             layouter.place(object_=l_ch, x=x, y=y)
 
             # vdd tap
             # First create ch to compute dimension of big diode
-            l_ch = layouter.wire_layout(
-                net=vdd, well_net=vdd, wire=contact,
-                bottom=active, bottom_implant=nimplant, bottom_well=nwell,
-            )
-            impl_bb = l_ch.bounds(mask=nimplant.mask)
-            impl_w = impl_bb.width
-            # Compute the possible hor. expansion
-            d = cell_width - impl_w - nimplant.min_space
-            assert tech.on_grid(d) >= 0.0
-            act_bb = l_ch.bounds(mask=active.mask)
-            # Maximize width
-            act_w = act_bb.width + d
-            # Maximize height
-            enc = act_bb.bottom - impl_bb.bottom
-            bottom = canvas._well_edge_height + canvas._min_active_well_enclosure
-            top = canvas._cell_height - 0.5*nimplant.min_space - enc
-            act_h = tech.on_grid(
-                top - bottom, mult=2, rounding="floor",
-            )
+            if nimplant is not None:
+                l_ch = layouter.wire_layout(
+                    net=vdd, well_net=vdd, wire=contact,
+                    bottom=active, bottom_implant=nimplant, bottom_well=nwell,
+                )
+                impl_bb = l_ch.bounds(mask=nimplant.mask)
+                impl_w = impl_bb.width
+                # Compute the possible hor. expansion
+                d = cell_width - impl_w - nimplant.min_space
+                assert tech.on_grid(d) >= 0.0
+                act_bb = l_ch.bounds(mask=active.mask)
+                act_w = act_bb.width + d
+                # Maximize height
+                enc = act_bb.bottom - impl_bb.bottom
+                bottom = canvas._well_edge_height + canvas._min_active_well_enclosure
+                top = canvas._cell_height - 0.5*nimplant.min_space - enc
+                act_h = tech.on_grid(
+                    top - bottom, mult=2, rounding="floor",
+                )
+            else:
+                act_w = cell_width - 2*active.min_space
+                bottom = canvas._well_edge_height + canvas._min_active_well_enclosure
+                top = canvas._cell_height - active.min_space
+                act_h = tech.on_grid(
+                    top - bottom, mult=2, rounding="floor",
+                )
 
             # diode with right dimensions
             l_ch = layouter.wire_layout(
                 net=vdd, well_net=vdd, wire=contact,
                 bottom=active, bottom_implant=nimplant, bottom_well=nwell,
                 bottom_width=act_w, bottom_height=act_h,
             )
-            impl_bb = l_ch.bounds(mask=nimplant.mask)
             x = 0.5*cell_width
-            y = canvas._cell_height - 0.5*nimplant.min_space - impl_bb.top
+            if nimplant is not None:
+                impl_bb = l_ch.bounds(mask=nimplant.mask)
+                y = canvas._cell_height - 0.5*nimplant.min_space - impl_bb.top
+            else:
+                act_bb = l_ch.bounds(mask=active.mask)
+                y = canvas._cell_height - active.min_space - act_bb.top
             layouter.place(object_=l_ch, x=x, y=y)
 
 
 class _Diode(_Cell):
     def __init__(self, *,
         fab: "StdCellFactory", name: str,
     ):
@@ -226,50 +254,48 @@
             pass
         else:
             min_actwell_space = max(min_actwell_space, s)
         enc = active.min_substrate_enclosure
         if enc is not None:
             min_actwell_space = max(min_actwell_space, enc.max())
 
-        nimpl_idx = active.implant.index(nimplant)
-        pimpl_idx = active.implant.index(pimplant)
-        min_actnimpl_enc = active.min_implant_enclosure[nimpl_idx].max()
-        min_actpimpl_enc = active.min_implant_enclosure[pimpl_idx].max()
-
         # Min active space without implants overlapping
-        min_act_space = max(
-            active.min_space,
-            min_actnimpl_enc + min_actpimpl_enc,
-        )
-
         # vss min tap
         l_ch = layouter.wire_layout(
             net=vss, wire=contact, rows=canvas._min_tap_chs,
             bottom=active, bottom_implant=pimplant,
         )
-        impl_bb = l_ch.bounds(mask=pimplant.mask)
         x = 0.5*cell_width
-        y = 0.5*pimplant.min_space - impl_bb.bottom
+        if pimplant is not None:
+            impl_bb = l_ch.bounds(mask=pimplant.mask)
+            y = 0.5*pimplant.min_space - impl_bb.bottom
+        else:
+            act_bb = l_ch.bounds(mask=active.mask)
+            y = active.min_space - act_bb.bottom
         vss_tap_lay = layouter.place(object_=l_ch, x=x, y=y)
         vss_tap_act_bb = vss_tap_lay.bounds(mask=active.mask)
 
         # vdd min tap
         l_ch = layouter.wire_layout(
             net=vdd, well_net=vdd, wire=contact, rows=canvas._min_tap_chs,
             bottom=active, bottom_implant=nimplant, bottom_well=nwell
         )
-        impl_bb = l_ch.bounds(mask=nimplant.mask)
         x = 0.5*cell_width
-        y = canvas._cell_height - 0.5*pimplant.min_space - impl_bb.top
+        if nimplant is not None:
+            impl_bb = l_ch.bounds(mask=nimplant.mask)
+            y = canvas._cell_height - 0.5*nimplant.min_space - impl_bb.top
+        else:
+            act_bb = l_ch.bounds(mask=active.mask)
+            y = canvas._cell_height - active.min_space - act_bb.top
         vdd_tap_lay = layouter.place(object_=l_ch, x=x, y=y)
         vdd_tap_act_bb = vdd_tap_lay.bounds(mask=active.mask)
 
         # vss diode
         bottom = max(
-            vss_tap_act_bb.top + min_act_space,
+            vss_tap_act_bb.top + canvas._min_nactive_pactive_space_maxenc,
             canvas._m1_vssrail_width + metal1.min_space,
         )
         top = canvas._well_edge_height - min_actwell_space
         h = tech.on_grid(top - bottom, mult=2, rounding="floor")
         vss_dio_x = 0.5*cell_width
         vss_dio_y = bottom + 0.5*h
         vss_dio_lay = layouter.add_wire(
@@ -277,15 +303,15 @@
             x=vss_dio_x, y=vss_dio_y, bottom_height=h, top_height=h,
         )
         vss_dio_m1_bb = vss_dio_lay.bounds(mask=metal1.mask)
 
         # vdd diode
         bottom = canvas._well_edge_height + canvas._min_active_well_enclosure
         top = min(
-            vdd_tap_act_bb.bottom - min_act_space,
+            vdd_tap_act_bb.bottom - canvas._min_nactive_pactive_space_maxenc,
             canvas._cell_height - canvas._m1_vddrail_width - metal1.min_space,
         )
         h = tech.on_grid(top - bottom, mult=2, rounding="floor")
         vdd_dio_x = 0.5*cell_width
         vdd_dio_y = top - 0.5*h
         vdd_dio_lay = layouter.add_wire(
             net=vdd, well_net=vdd, wire=contact,
```

### Comparing `c4m_flexcell-0.4.0.dev3/c4m/flexcell/stdcell.py` & `c4m_flexcell-0.4.0.dev9/c4m/flexcell/stdcell.py`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.4.0.dev3/c4m_flexcell.egg-info/PKG-INFO` & `c4m_flexcell-0.4.0.dev9/c4m_flexcell.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4m-flexcell
-Version: 0.4.0.dev3
+Version: 0.4.0.dev9
 Summary: PDKMaster based scalable standard cell library
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/c4m-flexcell
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/c4m-flexcell/issues
 Requires-Python: ~=3.6
```

### Comparing `c4m_flexcell-0.4.0.dev3/c4m_flexcell.egg-info/SOURCES.txt` & `c4m_flexcell-0.4.0.dev9/c4m_flexcell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.4.0.dev3/dodo.py` & `c4m_flexcell-0.4.0.dev9/dodo.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,9 +86,10 @@
 
     return {
         "title": lambda _: "Installing python module",
         "file_dep": c4m_py_files,
         "targets": (flexcell_inst_dir,),
         "actions": (
             f"{pip} install --no-deps {top_dir}",
+            f"{pip} check",
         ),
     }
```

### Comparing `c4m_flexcell-0.4.0.dev3/setup.py` & `c4m_flexcell-0.4.0.dev9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     author_email="staf@fibraservi.eu",
     description="PDKMaster based scalable standard cell library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+",
     python_requires="~=3.6",
     setup_requires=["setuptools_scm"],
-    install_requires=["setuptools", "PDKMaster~=0.9.3"],
+    install_requires=["setuptools", "PDKMaster~=0.9.4"],
     include_package_data=True,
     packages=_packages,
     project_urls={
         #"Documentation": "???",
         "Source Code": "https://gitlab.com/Chips4Makers/c4m-flexcell",
         "Bug Tracker": "https://gitlab.com/Chips4Makers/c4m-flexcell/issues",
     },
```

### Comparing `c4m_flexcell-0.4.0.dev3/test/interactive/export.ipynb` & `c4m_flexcell-0.4.0.dev9/test/interactive/export.ipynb`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.4.0.dev3/test/unit/test_library.py` & `c4m_flexcell-0.4.0.dev9/test/unit/test_library.py`

 * *Files identical despite different names*


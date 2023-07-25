# Comparing `tmp/qtmetabolabpy-0.9.5.tar.gz` & `tmp/qtmetabolabpy-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtmetabolabpy-0.9.5.tar", last modified: Tue Jul 25 19:32:44 2023, max compression
+gzip compressed data, was "qtmetabolabpy-0.9.6.tar", last modified: Tue Jul 25 22:36:10 2023, max compression
```

## Comparing `qtmetabolabpy-0.9.5.tar` & `qtmetabolabpy-0.9.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:32:44.008589 qtmetabolabpy-0.9.5/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079    35149 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.5/LICENSE
--rw-r--r--   0 ludwigc  (1699341573) 1311385079      364 2023-07-11 15:01:39.000000 qtmetabolabpy-0.9.5/MANIFEST.in
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     3745 2023-07-25 19:32:44.008368 qtmetabolabpy-0.9.5/PKG-INFO
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     2977 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.5/README.rst
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:32:44.005553 qtmetabolabpy-0.9.5/qtmetabolabpy/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079      195 2023-07-25 19:28:49.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/__init__.py
--rwxr-xr-x   0 ludwigc  (1699341573) 1311385079     5014 2023-07-16 19:58:28.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/__main__.py
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:32:44.006656 qtmetabolabpy-0.9.5/qtmetabolabpy/bash/
--rwxr-xr-x   0 ludwigc  (1699341573) 1311385079      556 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/bash/fix_pyside2
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:32:44.007026 qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:32:44.007480 qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/Contents/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079      884 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/Contents/Info.plist
--rw-r--r--   0 ludwigc  (1699341573) 1311385079        9 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/Contents/PkgInfo
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:32:44.007656 qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/Contents/Resources/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079   173336 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns
--rw-r--r--   0 ludwigc  (1699341573) 1311385079        0 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/Icon
--rwxr-xr-x   0 ludwigc  (1699341573) 1311385079   376308 2023-07-24 18:45:31.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/qtMetaboLabPy.py
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:32:44.008009 qtmetabolabpy-0.9.5/qtmetabolabpy/ui/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079   242054 2023-07-24 23:32:39.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/ui/metabolabpy_mainwindow.ui
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:32:44.006517 qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     3745 2023-07-25 19:32:43.000000 qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/PKG-INFO
--rw-r--r--   0 ludwigc  (1699341573) 1311385079      607 2023-07-25 19:32:43.000000 qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/SOURCES.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079        1 2023-07-25 19:32:43.000000 qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/dependency_links.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       62 2023-07-25 19:32:43.000000 qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/entry_points.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       97 2023-07-25 19:32:43.000000 qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/requires.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       14 2023-07-25 19:32:43.000000 qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/top_level.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079      323 2023-07-21 11:26:22.000000 qtmetabolabpy-0.9.5/requirements.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       38 2023-07-25 19:32:44.008635 qtmetabolabpy-0.9.5/setup.cfg
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     3912 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.5/setup.py
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-25 22:36:10.098477 qtmetabolabpy-0.9.6/
+-rw-r--r--   0 ludwigc    (501) staff       (20)    35149 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.6/LICENSE
+-rw-r--r--   0 ludwigc    (501) staff       (20)      364 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.6/MANIFEST.in
+-rw-r--r--   0 ludwigc    (501) staff       (20)     3745 2023-07-25 22:36:10.098338 qtmetabolabpy-0.9.6/PKG-INFO
+-rw-r--r--   0 ludwigc    (501) staff       (20)     2977 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.6/README.rst
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-25 22:36:10.094465 qtmetabolabpy-0.9.6/qtmetabolabpy/
+-rw-r--r--   0 ludwigc    (501) staff       (20)      195 2023-07-25 22:36:02.000000 qtmetabolabpy-0.9.6/qtmetabolabpy/__init__.py
+-rwxr-xr-x   0 ludwigc    (501) staff       (20)     5014 2023-07-16 17:08:05.000000 qtmetabolabpy-0.9.6/qtmetabolabpy/__main__.py
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-25 22:36:10.096643 qtmetabolabpy-0.9.6/qtmetabolabpy/bash/
+-rwxr-xr-x   0 ludwigc    (501) staff       (20)      556 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.6/qtmetabolabpy/bash/fix_pyside2
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-25 22:36:10.096873 qtmetabolabpy-0.9.6/qtmetabolabpy/mlStarter/
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-25 22:36:10.097194 qtmetabolabpy-0.9.6/qtmetabolabpy/mlStarter/Contents/
+-rw-r--r--   0 ludwigc    (501) staff       (20)      884 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.6/qtmetabolabpy/mlStarter/Contents/Info.plist
+-rw-r--r--   0 ludwigc    (501) staff       (20)        9 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.6/qtmetabolabpy/mlStarter/Contents/PkgInfo
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-25 22:36:10.097492 qtmetabolabpy-0.9.6/qtmetabolabpy/mlStarter/Contents/Resources/
+-rw-r--r--   0 ludwigc    (501) staff       (20)   173336 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.6/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns
+-rw-r--r--   0 ludwigc    (501) staff       (20)        0 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.6/qtmetabolabpy/mlStarter/Icon
+-rwxr-xr-x   0 ludwigc    (501) staff       (20)   375369 2023-07-25 22:23:25.000000 qtmetabolabpy-0.9.6/qtmetabolabpy/qtMetaboLabPy.py
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-25 22:36:10.097960 qtmetabolabpy-0.9.6/qtmetabolabpy/ui/
+-rw-r--r--   0 ludwigc    (501) staff       (20)   242054 2023-07-25 22:17:55.000000 qtmetabolabpy-0.9.6/qtmetabolabpy/ui/metabolabpy_mainwindow.ui
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-25 22:36:10.096511 qtmetabolabpy-0.9.6/qtmetabolabpy.egg-info/
+-rw-r--r--   0 ludwigc    (501) staff       (20)     3745 2023-07-25 22:36:09.000000 qtmetabolabpy-0.9.6/qtmetabolabpy.egg-info/PKG-INFO
+-rw-r--r--   0 ludwigc    (501) staff       (20)      607 2023-07-25 22:36:09.000000 qtmetabolabpy-0.9.6/qtmetabolabpy.egg-info/SOURCES.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)        1 2023-07-25 22:36:09.000000 qtmetabolabpy-0.9.6/qtmetabolabpy.egg-info/dependency_links.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       62 2023-07-25 22:36:09.000000 qtmetabolabpy-0.9.6/qtmetabolabpy.egg-info/entry_points.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       97 2023-07-25 22:36:09.000000 qtmetabolabpy-0.9.6/qtmetabolabpy.egg-info/requires.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       14 2023-07-25 22:36:09.000000 qtmetabolabpy-0.9.6/qtmetabolabpy.egg-info/top_level.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)      323 2023-07-25 22:17:55.000000 qtmetabolabpy-0.9.6/requirements.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       38 2023-07-25 22:36:10.098520 qtmetabolabpy-0.9.6/setup.cfg
+-rw-r--r--   0 ludwigc    (501) staff       (20)     3912 2023-07-11 16:27:55.000000 qtmetabolabpy-0.9.6/setup.py
```

### Comparing `qtmetabolabpy-0.9.5/LICENSE` & `qtmetabolabpy-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.5/PKG-INFO` & `qtmetabolabpy-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmetabolabpy
-Version: 0.9.5
+Version: 0.9.6
 Summary: Python package for data processing of NMR 1D and 2D metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/qtmetabolabpy
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `qtmetabolabpy-0.9.5/README.rst` & `qtmetabolabpy-0.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.5/qtmetabolabpy/__main__.py` & `qtmetabolabpy-0.9.6/qtmetabolabpy/__main__.py`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.5/qtmetabolabpy/bash/fix_pyside2` & `qtmetabolabpy-0.9.6/qtmetabolabpy/bash/fix_pyside2`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/Contents/Info.plist` & `qtmetabolabpy-0.9.6/qtmetabolabpy/mlStarter/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns` & `qtmetabolabpy-0.9.6/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.5/qtmetabolabpy/qtMetaboLabPy.py` & `qtmetabolabpy-0.9.6/qtmetabolabpy/qtMetaboLabPy.py`

 * *Files 0% similar despite different names*

```diff
@@ -3832,18 +3832,15 @@
         self.w.resetSplineBaselineButton.setHidden(True)
         self.w.plotBaselineButton.setHidden(True)
         self.w.correctAllButton.setHidden(True)
         # end hide_spline_baseline
 
     def html(self, url=''):
         if len(url) == 0:
-            nmr_dir = os.path.split(inspect.getmodule(nmrDataSet).__file__)[0]
-            base_dir = os.path.split(nmr_dir)[0]
-            f_name = os.path.join(base_dir, "nmr", "web", "index.html")
-            url = "file:///" + f_name.replace('\\', '/')
+            url = "https://ludwigc.github.io/metabolabpy"
 
         self.w.helpView.setUrl(url)
         self.w.nmrSpectrum.setCurrentIndex(12)
         # end html
 
     def show_peak_picking(self):
         self.w.preProcPeak.setHidden(False)
@@ -4132,18 +4129,15 @@
     def load_dark_mode(self):
         for k in range(len(self.nd.nmrdat[self.nd.s])):
             self.nd.nmrdat[self.nd.s][k].display.pos_col_rgb = self.std_pos_col2
             self.nd.nmrdat[self.nd.s][k].display.neg_col_rgb = self.std_neg_col2
 
         idx = self.w.helpComboBox.currentIndex()
         url = []
-        nmr_dir = os.path.split(inspect.getmodule(nmrDataSet).__file__)[0]
-        base_dir = os.path.split(nmr_dir)[0]
-        f_name = os.path.join(base_dir, "nmr", "web", "index.html")
-        url.append("file:///" + f_name.replace('\\', '/'))
+        url.append("https://ludwigc.github.io/metabolabpy")
         url.append("http://www.bml-nmr.org")
         url.append("https://www.hmdb.ca")
         url.append("https://www.smpdb.ca")
         url.append("https://bmrb.io/metabolomics/")
         url.append("https://www.genome.jp/kegg/pathway.html#metabolism")
         url.append("https://nmrshiftdb.nmr.uni-koeln.de")
         url.append("https://sdbs.db.aist.go.jp/sdbs/cgi-bin/cre_index.cgi")
@@ -4227,18 +4221,15 @@
     def load_light_mode(self):
         for k in range(len(self.nd.nmrdat[self.nd.s])):
             self.nd.nmrdat[self.nd.s][k].display.pos_col_rgb = self.std_pos_col1
             self.nd.nmrdat[self.nd.s][k].display.neg_col_rgb = self.std_neg_col1
 
         idx = self.w.helpComboBox.currentIndex()
         url = []
-        nmr_dir = os.path.split(inspect.getmodule(nmrDataSet).__file__)[0]
-        base_dir = os.path.split(nmr_dir)[0]
-        f_name = os.path.join(base_dir, "nmr", "web", "index.html")
-        url.append("file:///" + f_name.replace('\\', '/'))
+        url.append("https://ludwigc.github.io/metabolabpy")
         url.append("http://www.bml-nmr.org")
         url.append("https://www.hmdb.ca")
         url.append("https://www.smpdb.ca")
         url.append("https://bmrb.io/metabolomics/")
         url.append("https://www.genome.jp/kegg/pathway.html#metabolism")
         url.append("https://nmrshiftdb.nmr.uni-koeln.de")
         url.append("https://sdbs.db.aist.go.jp/sdbs/cgi-bin/cre_index.cgi")
@@ -5758,15 +5749,15 @@
         nmr_dir = os.path.split(inspect.getmodule(nmrDataSet).__file__)[0]
         base_dir = os.path.split(nmr_dir)[0]
         if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
             f_name = os.path.join(base_dir, "nmr", "web", "index.html")
         else:
             f_name = os.path.join(base_dir, "nmr", "web", "index.html")
 
-        url = "file:///" + f_name.replace('\\', '/')
+        url = "https://ludwigc.github.io/metabolabpy"
         self.w.helpView.setUrl(url)
         self.w.nmrSpectrum.setCurrentIndex(12)
         # end reset_help
 
     def reset_ml_info(self):
         idx = self.w.hsqcMetabolites.currentIndex().row()
         if idx == -1:
@@ -6824,22 +6815,15 @@
         self.w.cmdLine.setFont(f)
         self.w.setStyleSheet("font-size: " + str(font_size) + "pt")
         # end set_font_size
 
     def set_help(self):
         url = []
         idx = self.w.helpComboBox.currentIndex()
-        nmr_dir = os.path.split(inspect.getmodule(nmrDataSet).__file__)[0]
-        base_dir = os.path.split(nmr_dir)[0]
-        if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
-            f_name = os.path.join(base_dir, "nmr", "web", "index.html")
-        else:
-            f_name = os.path.join(base_dir, "nmr", "web", "index.html")
-
-        url.append("file:///" + f_name.replace('\\', '/'))
+        url.append("https://ludwigc.github.io/metabolabpy")
         url.append("http://www.bml-nmr.org")
         url.append("https://www.hmdb.ca")
         url.append("https://www.smpdb.ca")
         url.append("https://bmrb.io/metabolomics/")
         url.append("https://www.genome.jp/kegg/pathway.html#metabolism")
         url.append("https://nmrshiftdb.nmr.uni-koeln.de")
         url.append("https://sdbs.db.aist.go.jp/sdbs/cgi-bin/cre_index.cgi")
```

### Comparing `qtmetabolabpy-0.9.5/qtmetabolabpy/ui/metabolabpy_mainwindow.ui` & `qtmetabolabpy-0.9.6/qtmetabolabpy/ui/metabolabpy_mainwindow.ui`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/PKG-INFO` & `qtmetabolabpy-0.9.6/qtmetabolabpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmetabolabpy
-Version: 0.9.5
+Version: 0.9.6
 Summary: Python package for data processing of NMR 1D and 2D metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/qtmetabolabpy
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/SOURCES.txt` & `qtmetabolabpy-0.9.6/qtmetabolabpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.5/setup.py` & `qtmetabolabpy-0.9.6/setup.py`

 * *Files identical despite different names*


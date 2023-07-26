# Comparing `tmp/f311-23.7.25.0.tar.gz` & `tmp/f311-23.7.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f311-23.7.25.0.tar", last modified: Tue Jul 25 15:47:27 2023, max compression
+gzip compressed data, was "f311-23.7.26.0.tar", last modified: Wed Jul 26 17:10:59 2023, max compression
```

## Comparing `f311-23.7.25.0.tar` & `f311-23.7.26.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 15:47:27.599886 f311-23.7.25.0/
--rw-rw-r--   0 j         (1000) j         (1000)       40 2020-07-20 14:21:24.000000 f311-23.7.25.0/MANIFEST.in
--rw-rw-r--   0 j         (1000) j         (1000)      430 2023-07-25 15:47:27.599886 f311-23.7.25.0/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)      152 2020-07-20 14:21:24.000000 f311-23.7.25.0/README.md
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 15:47:27.583886 f311-23.7.25.0/f311/
--rw-rw-r--   0 j         (1000) j         (1000)      144 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)     8609 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/collaboration.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 15:47:27.583886 f311-23.7.25.0/f311/explorer/
--rw-rw-r--   0 j         (1000) j         (1000)      595 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/explorer/__init__.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 15:47:27.587885 f311-23.7.25.0/f311/explorer/gui/
--rw-rw-r--   0 j         (1000) j         (1000)      197 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/explorer/gui/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)    26066 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/explorer/gui/a_XExplorer.py
--rw-rw-r--   0 j         (1000) j         (1000)    15613 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/explorer/gui/a_XFileMainWindow.py
--rw-rw-r--   0 j         (1000) j         (1000)     3426 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/explorer/gui/a_XSelectDataFile.py
--rw-rw-r--   0 j         (1000) j         (1000)     1367 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/explorer/gui/a_XText.py
--rw-rw-r--   0 j         (1000) j         (1000)      712 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/explorer/util.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 15:47:27.591886 f311-23.7.25.0/f311/explorer/vis/
--rw-rw-r--   0 j         (1000) j         (1000)      211 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/explorer/vis/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)     1459 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/explorer/vis/basic.py
--rw-rw-r--   0 j         (1000) j         (1000)    10717 2023-07-24 20:12:10.000000 f311-23.7.25.0/f311/explorer/vis/plotsp.py
--rw-rw-r--   0 j         (1000) j         (1000)      228 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/explorer/vis/visprint.py
--rw-rw-r--   0 j         (1000) j         (1000)      552 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/explorer/vis/visspectrum.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 15:47:27.595886 f311-23.7.25.0/f311/filetypes/
--rw-rw-r--   0 j         (1000) j         (1000)      233 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/filetypes/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)     3677 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/filetypes/datafile.py
--rw-rw-r--   0 j         (1000) j         (1000)     1460 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/filetypes/filefits.py
--rw-rw-r--   0 j         (1000) j         (1000)     3034 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/filetypes/filepy.py
--rw-rw-r--   0 j         (1000) j         (1000)     3020 2023-07-21 15:37:16.000000 f311-23.7.25.0/f311/filetypes/filespectrum.py
--rw-rw-r--   0 j         (1000) j         (1000)     6276 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/filetypes/filesqlitedb.py
--rw-rw-r--   0 j         (1000) j         (1000)    13438 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/filetypes/spectrum.py
--rw-rw-r--   0 j         (1000) j         (1000)   561633 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/hapi.py
--rw-rw-r--   0 j         (1000) j         (1000)     2097 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/pathfinder.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 15:47:27.595886 f311-23.7.25.0/f311/scripts/
--rwxrwxr-x   0 j         (1000) j         (1000)     1362 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/scripts/cut-spectrum.py
--rwxrwxr-x   0 j         (1000) j         (1000)      645 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/scripts/explorer.py
--rwxrwxr-x   0 j         (1000) j         (1000)     5010 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/scripts/plot-spectra.py
--rwxrwxr-x   0 j         (1000) j         (1000)     3461 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/scripts/programs.py
--rw-rw-r--   0 j         (1000) j         (1000)     8708 2020-07-20 14:21:24.000000 f311-23.7.25.0/f311/util.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 15:47:27.583886 f311-23.7.25.0/f311.egg-info/
--rw-rw-r--   0 j         (1000) j         (1000)      430 2023-07-25 15:47:27.000000 f311-23.7.25.0/f311.egg-info/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)      922 2023-07-25 15:47:27.000000 f311-23.7.25.0/f311.egg-info/SOURCES.txt
--rw-rw-r--   0 j         (1000) j         (1000)        1 2023-07-25 15:47:27.000000 f311-23.7.25.0/f311.egg-info/dependency_links.txt
--rw-rw-r--   0 j         (1000) j         (1000)      133 2023-07-25 15:47:27.000000 f311-23.7.25.0/f311.egg-info/requires.txt
--rw-rw-r--   0 j         (1000) j         (1000)        5 2023-07-25 15:47:27.000000 f311-23.7.25.0/f311.egg-info/top_level.txt
--rw-rw-r--   0 j         (1000) j         (1000)       38 2023-07-25 15:47:27.599886 f311-23.7.25.0/setup.cfg
--rw-rw-r--   0 j         (1000) j         (1000)     1568 2023-07-25 15:47:16.000000 f311-23.7.25.0/setup.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-26 17:10:59.392867 f311-23.7.26.0/
+-rw-rw-r--   0 j         (1000) j         (1000)       40 2020-07-20 14:21:24.000000 f311-23.7.26.0/MANIFEST.in
+-rw-rw-r--   0 j         (1000) j         (1000)      430 2023-07-26 17:10:59.392867 f311-23.7.26.0/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)      152 2020-07-20 14:21:24.000000 f311-23.7.26.0/README.md
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-26 17:10:59.392867 f311-23.7.26.0/f311/
+-rw-rw-r--   0 j         (1000) j         (1000)      144 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     8609 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/collaboration.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-26 17:10:59.392867 f311-23.7.26.0/f311/explorer/
+-rw-rw-r--   0 j         (1000) j         (1000)      595 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/explorer/__init__.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-26 17:10:59.392867 f311-23.7.26.0/f311/explorer/gui/
+-rw-rw-r--   0 j         (1000) j         (1000)      197 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/explorer/gui/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)    26066 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/explorer/gui/a_XExplorer.py
+-rw-rw-r--   0 j         (1000) j         (1000)    15613 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/explorer/gui/a_XFileMainWindow.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3426 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/explorer/gui/a_XSelectDataFile.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1367 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/explorer/gui/a_XText.py
+-rw-rw-r--   0 j         (1000) j         (1000)      712 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/explorer/util.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-26 17:10:59.392867 f311-23.7.26.0/f311/explorer/vis/
+-rw-rw-r--   0 j         (1000) j         (1000)      211 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/explorer/vis/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1459 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/explorer/vis/basic.py
+-rw-rw-r--   0 j         (1000) j         (1000)    10909 2023-07-26 17:09:58.000000 f311-23.7.26.0/f311/explorer/vis/plotsp.py
+-rw-rw-r--   0 j         (1000) j         (1000)      228 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/explorer/vis/visprint.py
+-rw-rw-r--   0 j         (1000) j         (1000)      552 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/explorer/vis/visspectrum.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-26 17:10:59.392867 f311-23.7.26.0/f311/filetypes/
+-rw-rw-r--   0 j         (1000) j         (1000)      233 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/filetypes/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3677 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/filetypes/datafile.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1460 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/filetypes/filefits.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3034 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/filetypes/filepy.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3020 2023-07-21 15:37:16.000000 f311-23.7.26.0/f311/filetypes/filespectrum.py
+-rw-rw-r--   0 j         (1000) j         (1000)     6276 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/filetypes/filesqlitedb.py
+-rw-rw-r--   0 j         (1000) j         (1000)    13438 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/filetypes/spectrum.py
+-rw-rw-r--   0 j         (1000) j         (1000)   561633 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/hapi.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2097 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/pathfinder.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-26 17:10:59.392867 f311-23.7.26.0/f311/scripts/
+-rwxrwxr-x   0 j         (1000) j         (1000)     1362 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/scripts/cut-spectrum.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      645 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/scripts/explorer.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     5010 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/scripts/plot-spectra.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     3457 2023-07-25 23:27:39.000000 f311-23.7.26.0/f311/scripts/programs.py
+-rw-rw-r--   0 j         (1000) j         (1000)     8708 2020-07-20 14:21:24.000000 f311-23.7.26.0/f311/util.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-26 17:10:59.392867 f311-23.7.26.0/f311.egg-info/
+-rw-rw-r--   0 j         (1000) j         (1000)      430 2023-07-26 17:10:59.000000 f311-23.7.26.0/f311.egg-info/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)      922 2023-07-26 17:10:59.000000 f311-23.7.26.0/f311.egg-info/SOURCES.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        1 2023-07-26 17:10:59.000000 f311-23.7.26.0/f311.egg-info/dependency_links.txt
+-rw-rw-r--   0 j         (1000) j         (1000)      133 2023-07-26 17:10:59.000000 f311-23.7.26.0/f311.egg-info/requires.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        5 2023-07-26 17:10:59.000000 f311-23.7.26.0/f311.egg-info/top_level.txt
+-rw-rw-r--   0 j         (1000) j         (1000)       38 2023-07-26 17:10:59.392867 f311-23.7.26.0/setup.cfg
+-rw-rw-r--   0 j         (1000) j         (1000)     1568 2023-07-26 17:10:28.000000 f311-23.7.26.0/setup.py
```

### Comparing `f311-23.7.25.0/f311/collaboration.py` & `f311-23.7.26.0/f311/collaboration.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/explorer/__init__.py` & `f311-23.7.26.0/f311/explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/explorer/gui/a_XExplorer.py` & `f311-23.7.26.0/f311/explorer/gui/a_XExplorer.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/explorer/gui/a_XFileMainWindow.py` & `f311-23.7.26.0/f311/explorer/gui/a_XFileMainWindow.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/explorer/gui/a_XSelectDataFile.py` & `f311-23.7.26.0/f311/explorer/gui/a_XSelectDataFile.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/explorer/gui/a_XText.py` & `f311-23.7.26.0/f311/explorer/gui/a_XText.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/explorer/util.py` & `f311-23.7.26.0/f311/explorer/util.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/explorer/vis/basic.py` & `f311-23.7.26.0/f311/explorer/vis/basic.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/explorer/vis/plotsp.py` & `f311-23.7.26.0/f311/explorer/vis/plotsp.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,18 @@
         plt.ylim([ymin - yspan * _T, ymax + yspan * _T])
         if setup.flag_legend:
             leg = plt.legend(loc=0)
             a99.format_legend(leg)
         plt.tight_layout()
 
     if title is not None:
-        plt.gcf().canvas.set_window_title(title)
+        try:
+            plt.gcf().canvas.set_window_title(title)
+        except AttributeError:
+            plt.gcf().canvas.setWindowTitle(title)
 
 
 def _plot_with_styles(ax, x, y, label, stylespecs, i):
     ax.plot(x, y, label=label,
             c=stylespecs.get(f"c{i}"),
             lw=stylespecs.get(f"lw{i}"),
             linestyle=stylespecs.get(f"s{i}"))
@@ -307,9 +310,12 @@
         ax.set_xlim([xmin - span * _T, xmax + span * _T])
     for j in range(num_cols):
         ax = axarr[num_rows - 1, j]
         if setup.flag_xlabel and setup.fmt_xlabel:
             _set_plot(ax.set_xlabel, setup.fmt_xlabel, s)
     plt.tight_layout()
     if title is not None:
-        fig.canvas.set_window_title(title)
+        try:
+            fig.canvas.set_window_title(title)
+        except AttributeError:
+            fig.canvas.setWindowTitle(title)
     return fig
```

### Comparing `f311-23.7.25.0/f311/explorer/vis/visspectrum.py` & `f311-23.7.26.0/f311/explorer/vis/visspectrum.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/filetypes/datafile.py` & `f311-23.7.26.0/f311/filetypes/datafile.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/filetypes/filefits.py` & `f311-23.7.26.0/f311/filetypes/filefits.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/filetypes/filepy.py` & `f311-23.7.26.0/f311/filetypes/filepy.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/filetypes/filespectrum.py` & `f311-23.7.26.0/f311/filetypes/filespectrum.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/filetypes/filesqlitedb.py` & `f311-23.7.26.0/f311/filetypes/filesqlitedb.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/filetypes/spectrum.py` & `f311-23.7.26.0/f311/filetypes/spectrum.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/hapi.py` & `f311-23.7.26.0/f311/hapi.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/pathfinder.py` & `f311-23.7.26.0/f311/pathfinder.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/scripts/cut-spectrum.py` & `f311-23.7.26.0/f311/scripts/cut-spectrum.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/scripts/explorer.py` & `f311-23.7.26.0/f311/scripts/explorer.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/scripts/plot-spectra.py` & `f311-23.7.26.0/f311/scripts/plot-spectra.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311/scripts/programs.py` & `f311-23.7.26.0/f311/scripts/programs.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
      help='If format=="rest-list", '
           'renders program names as links to their respective documentation pages')
     parser.add_argument('-n', '--no-pfant', action="store_true",
      help='Does not list PFANT binaries')
     parser.add_argument('-_', '--protected', action="store_true", help="Includes protected scripts (starting with '_')")
     args = parser.parse_args()
 
-    pkgname_only = args.pkgname if args.pkgname is not "(all)" else None
+    pkgname_only = args.pkgname if args.pkgname != "(all)" else None
 
     if args.list_packages:
         _list_packages()
         sys.exit()
 
     if pkgname_only is not None:
         if pkgname_only not in f311.COLLABORATORS_S:
```

### Comparing `f311-23.7.25.0/f311/util.py` & `f311-23.7.26.0/f311/util.py`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/f311.egg-info/SOURCES.txt` & `f311-23.7.26.0/f311.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `f311-23.7.25.0/setup.py` & `f311-23.7.26.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 pkgs = find_packages()
 scripts = find_scripts([PACKAGE_NAME])
 
 setup(
     name=PACKAGE_NAME,
     packages=find_packages(),
     include_package_data=True,
-    version='23.7.25.0',
+    version='23.7.26.0',
     license='GNU GPLv3',
     platforms='any',
     description='Astronomy-related API, command-line tools, and windowed applications',
     author='Julio Trevisan',
     author_email='juliotrevisan@gmail.com',
     url='https://github.com/trevisanj/f311',
     keywords= ['astronomy', "fits", "spectroscopy", "spectral synthesis", "photometry",
```


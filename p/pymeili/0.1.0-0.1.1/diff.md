# Comparing `tmp/pymeili-0.1.0.tar.gz` & `tmp/pymeili-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeili-0.1.0.tar", last modified: Wed Jul 26 10:57:02 2023, max compression
+gzip compressed data, was "pymeili-0.1.1.tar", last modified: Wed Jul 26 11:32:39 2023, max compression
```

## Comparing `pymeili-0.1.0.tar` & `pymeili-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:02.044776 pymeili-0.1.0/
--rw-rw-rw-   0        0        0      194 2023-07-26 10:55:15.000000 pymeili-0.1.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.1.0/LISCENCE.txt
--rw-rw-rw-   0        0        0       36 2023-07-25 15:28:50.000000 pymeili-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1141 2023-07-26 10:57:02.043779 pymeili-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      495 2023-07-25 15:43:41.000000 pymeili-0.1.0/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:02.019861 pymeili-0.1.0/pymeili/
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:02.042782 pymeili-0.1.0/pymeili/FONT/
--rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.1.0/pymeili/FONT/Futura Extra Black font.ttf
--rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.1.0/pymeili/FONT/Futura Heavy font.ttf
--rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.1.0/pymeili/FONT/futura medium bt.ttf
--rw-rw-rw-   0        0        0      625 2023-07-26 04:13:49.000000 pymeili-0.1.0/pymeili/__init__.py
--rw-rw-rw-   0        0        0    54863 2023-07-26 10:54:57.000000 pymeili-0.1.0/pymeili/beautifyplot.py
-drwxrwxrwx   0        0        0        0 2023-07-26 10:57:02.030812 pymeili-0.1.0/pymeili.egg-info/
--rw-rw-rw-   0        0        0     1141 2023-07-26 10:57:01.000000 pymeili-0.1.0/pymeili.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-07-26 10:57:01.000000 pymeili-0.1.0/pymeili.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 10:57:01.000000 pymeili-0.1.0/pymeili.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-26 10:57:01.000000 pymeili-0.1.0/pymeili.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 10:57:02.044776 pymeili-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      741 2023-07-26 01:08:19.000000 pymeili-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:32:39.883041 pymeili-0.1.1/
+-rw-rw-rw-   0        0        0      194 2023-07-26 11:24:34.000000 pymeili-0.1.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.1.1/LISCENCE.txt
+-rw-rw-rw-   0        0        0       36 2023-07-25 15:28:50.000000 pymeili-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1141 2023-07-26 11:32:39.883041 pymeili-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2023-07-25 15:43:41.000000 pymeili-0.1.1/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 11:32:39.871067 pymeili-0.1.1/pymeili/
+drwxrwxrwx   0        0        0        0 2023-07-26 11:32:39.882044 pymeili-0.1.1/pymeili/FONT/
+-rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.1.1/pymeili/FONT/Futura Extra Black font.ttf
+-rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.1.1/pymeili/FONT/Futura Heavy font.ttf
+-rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.1.1/pymeili/FONT/futura medium bt.ttf
+-rw-rw-rw-   0        0        0      723 2023-07-26 11:32:13.000000 pymeili-0.1.1/pymeili/__init__.py
+-rw-rw-rw-   0        0        0    54190 2023-07-26 11:32:04.000000 pymeili-0.1.1/pymeili/beautifyplot.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:32:39.880050 pymeili-0.1.1/pymeili.egg-info/
+-rw-rw-rw-   0        0        0     1141 2023-07-26 11:32:39.000000 pymeili-0.1.1/pymeili.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-07-26 11:32:39.000000 pymeili-0.1.1/pymeili.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 11:32:39.000000 pymeili-0.1.1/pymeili.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-26 11:32:39.000000 pymeili-0.1.1/pymeili.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 11:32:39.884038 pymeili-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      741 2023-07-26 11:24:46.000000 pymeili-0.1.1/setup.py
```

### Comparing `pymeili-0.1.0/LISCENCE.txt` & `pymeili-0.1.1/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.0/PKG-INFO` & `pymeili-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.1.0
+Version: 0.1.1
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
@@ -32,9 +32,9 @@
 
 0.0.2 (25/07/2023)
 - Add Font Packages
 
 0.0.10 (25/07/2023)
 - Fix Some Problems
 
-0.1.0 (26/07/2023)
+0.1.1 (26/07/2023)
 - Add Subplot Function
```

### Comparing `pymeili-0.1.0/pymeili/FONT/Futura Extra Black font.ttf` & `pymeili-0.1.1/pymeili/FONT/Futura Extra Black font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.0/pymeili/FONT/Futura Heavy font.ttf` & `pymeili-0.1.1/pymeili/FONT/Futura Heavy font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.0/pymeili/FONT/futura medium bt.ttf` & `pymeili-0.1.1/pymeili/FONT/futura medium bt.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.0/pymeili/__init__.py` & `pymeili-0.1.1/pymeili/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from pymeili.beautifyplot import (
-    init, colorlist, cmaplist, getSCATTERNO, getPLOTNO, getBARNO, getBARHNO, getHISTNO,
-    savefig, title, lefttitle, righttitle, xlabel, ylabel, xticks, yticks, axvline, axhline,
-    spines, legend, grid, show, close, boxplot, plot, scatter, bar, barh, hist, hist2d, pie,
-    xylim, xlim, ylim, xlog, ylog, xyticks, xscale, yscale, text, labeltext, clf, figsize,
-    imsave, imshow, contour, contourf, colorbar, figure, subplots, table, subplots2grid,
-    hidespines, xaxisposition, yaxisposition,
+    initplot,
+    colorlist,
+    cmaplist,
+    getBARHNO,
+    getBARNO,
+    getHISTNO,
+    getPLOTNO,
+    getSCATTERNO,
+    savefig,
+    title, lefttitle, righttitle,
+    scatter, plot, bar, hist, hist2d, pie, barh, table,
+    contour, contourf, colorbar,
+    xlabel, ylabel, xticks, yticks, xyticks, ticksall,
+    xlim, ylim, xylim, xscale, yscale, xlog, ylog,
+    grid, spines, legend, hidespines, xaxisposition, yaxisposition,
+    axhline, axvline, text, annotate, labeltext,
+    fill_between, fill_betweenx,
+    figsize, show, clf, close, figure,
+    imread, imshow, imsave,
+    
 )
 
-__version__: str = '0.1.0'
+__version__: str = '0.1.1'
```

### Comparing `pymeili-0.1.0/pymeili/beautifyplot.py` & `pymeili-0.1.1/pymeili/beautifyplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,14 @@
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from pathlib import Path
 import matplotlib.font_manager as fm
 from matplotlib.colors import LinearSegmentedColormap
 from mpl_toolkits.basemap import Basemap as Bp
 
-#! UNSOLVE: twinx
-'''
-import numpy as np
-import matplotlib.pyplot as plt
-
-fig, ax1 = plt.subplots()
-t = np.arange(0.01, 10.0, 0.01)
-s1 = np.exp(t)
-ax1.plot(t, s1, 'b-')
-ax1.set_xlabel('time (s)')
-# Make the y-axis label, ticks and tick labels match the line color.
-ax1.set_ylabel('exp', color='b')
-ax1.tick_params('y', colors='b')
-
-ax2 = ax1.twinx()
-s2 = np.sin(2 * np.pi * t)
-ax2.plot(t, s2, 'r.')
-ax2.set_ylabel('sin', color='r')
-ax2.tick_params('y', colors='r')
-
-fig.tight_layout()
-plt.show()
-'''
-
 global fontscale
 fontscale = 0.6
 
 # 獲取當前檔案位址
 currentfilepath = __file__
 
 # 刪去__file__中最後面自"\"開始的字串(刪除檔名)
@@ -267,18 +243,14 @@
 
 def lefttitle(title, loc='left', color='1', font=fontpath_bold, fontsize=24):
     plt.title(title, loc=loc, color=colorlist(color), fontproperties=fm.FontProperties(fname=font, size=fontsize))
 
 def righttitle(title, loc='right', color='2', font=fontpath_bold, fontsize=24):
     plt.title(title, loc=loc, color=colorlist(color), fontproperties=fm.FontProperties(fname=font, size=fontsize))
 
-# 圖表
-def subplot(nrows=1, ncols=1, index=1, figsize=(8,10), **kwargs):
-    return plt.subplots(nrows, ncols, index, figsize=figsize, **kwargs)
-
 # scatter繪圖
 def scatter(x, y, color='fg', size=3, marker='o', linewidth=None, label=getSCATTERNO(), linestyle='-', **kwargs):
     plt.scatter(x, y, color=colorlist(color), s=size, marker=marker, linewidth=linewidth, label=label, linestyle=linestyle, **kwargs)
 
 # plot繪圖
 def plot(x, y, color='fg', linewidth=2, linestyle='-', label=getPLOTNO(),**kwargs):
     plt.plot(x, y, color=colorlist(color), linewidth=linewidth, label=label,linestyle=linestyle, **kwargs)
@@ -515,14 +487,16 @@
 
 def imshow(X, cmap='2', vmin=None, vmax=None, interpolation='nearest', alpha=None, aspect=None, **kwargs):
     plt.imshow(X, cmap=cmaplist(cmap), vmin=vmin, vmax=vmax, interpolation=interpolation, alpha=alpha, aspect=aspect, **kwargs)
 
 def imsave(filename, arr, vmin=None, vmax=None, cmap='2', format=None, origin=None, dpi=300, **kwargs):
     plt.imsave(filename, arr, vmin=vmin, vmax=vmax, cmap=cmaplist(cmap), format=format, origin=origin, dpi=dpi, **kwargs)
 
+
+
 # Basemap系列
 class Basemap():
     import numpy as np
     def __init__(self,projection='cyl', llcrnrlon=0, llcrnrlat=0, urcrnrlon=0, urcrnrlat=0, resolution='l', area_thresh=1000, zone=None,**kwargs):
         self.projection = projection # merc:麥卡托, cyl:等距圓柱, mill:米勒, cea:等距圓錐, gall:加爾-彼得, lcc:蘭伯特等角, tmerc:橫麥卡托, stere:極射, npstere:北極極射, spstere:南極極射, aeqd:等距方位, poly:多邊形, nsper:自然地球
         if zone == 'taiwan':
             self.llcrnrlat = 21.5
```

### Comparing `pymeili-0.1.0/pymeili.egg-info/PKG-INFO` & `pymeili-0.1.1/pymeili.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.1.0
+Version: 0.1.1
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
@@ -32,9 +32,9 @@
 
 0.0.2 (25/07/2023)
 - Add Font Packages
 
 0.0.10 (25/07/2023)
 - Fix Some Problems
 
-0.1.0 (26/07/2023)
+0.1.1 (26/07/2023)
 - Add Subplot Function
```

### Comparing `pymeili-0.1.0/setup.py` & `pymeili-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='pymeili',
-    version='0.1.0',
+    version='0.1.1',
     description='a module to beautify your python plot.',
     long_description=open('README.txt',encoding="utf-8").read() + '\n\n' + open('CHANGELOG.txt',encoding="utf-8").read(),
     url='',
     author='VVVictorZhou',
     author_email='vichouro@gmail.com',
     license='MIT',
     classifiers=classifiers,
```


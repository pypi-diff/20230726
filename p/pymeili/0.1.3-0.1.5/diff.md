# Comparing `tmp/pymeili-0.1.3.tar.gz` & `tmp/pymeili-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeili-0.1.3.tar", last modified: Wed Jul 26 14:20:02 2023, max compression
+gzip compressed data, was "pymeili-0.1.5.tar", last modified: Wed Jul 26 16:18:48 2023, max compression
```

## Comparing `pymeili-0.1.3.tar` & `pymeili-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 14:20:02.046693 pymeili-0.1.3/
--rw-rw-rw-   0        0        0      243 2023-07-26 13:10:45.000000 pymeili-0.1.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.1.3/LISCENCE.txt
--rw-rw-rw-   0        0        0       36 2023-07-25 15:28:50.000000 pymeili-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1295 2023-07-26 14:20:02.046693 pymeili-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      600 2023-07-26 13:10:34.000000 pymeili-0.1.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 14:20:02.016217 pymeili-0.1.3/pymeili/
-drwxrwxrwx   0        0        0        0 2023-07-26 14:20:02.045694 pymeili-0.1.3/pymeili/FONT/
--rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.1.3/pymeili/FONT/Futura Extra Black font.ttf
--rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.1.3/pymeili/FONT/Futura Heavy font.ttf
--rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.1.3/pymeili/FONT/futura medium bt.ttf
--rw-rw-rw-   0        0        0      715 2023-07-26 14:19:47.000000 pymeili-0.1.3/pymeili/__init__.py
--rw-rw-rw-   0        0        0    54618 2023-07-26 14:18:21.000000 pymeili-0.1.3/pymeili/beautifyplot.py
-drwxrwxrwx   0        0        0        0 2023-07-26 14:20:02.031179 pymeili-0.1.3/pymeili.egg-info/
--rw-rw-rw-   0        0        0     1295 2023-07-26 14:20:01.000000 pymeili-0.1.3/pymeili.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-07-26 14:20:01.000000 pymeili-0.1.3/pymeili.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 14:20:01.000000 pymeili-0.1.3/pymeili.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-26 14:20:01.000000 pymeili-0.1.3/pymeili.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 14:20:02.046693 pymeili-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      741 2023-07-26 13:10:58.000000 pymeili-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:18:48.968382 pymeili-0.1.5/
+-rw-rw-rw-   0        0        0      314 2023-07-26 16:17:52.000000 pymeili-0.1.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.1.5/LISCENCE.txt
+-rw-rw-rw-   0        0        0       36 2023-07-25 15:28:50.000000 pymeili-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1480 2023-07-26 16:18:48.967385 pymeili-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      714 2023-07-26 14:23:15.000000 pymeili-0.1.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 16:18:48.935049 pymeili-0.1.5/pymeili/
+drwxrwxrwx   0        0        0        0 2023-07-26 16:18:48.965390 pymeili-0.1.5/pymeili/FONT/
+-rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.1.5/pymeili/FONT/Futura Extra Black font.ttf
+-rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.1.5/pymeili/FONT/Futura Heavy font.ttf
+-rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.1.5/pymeili/FONT/futura medium bt.ttf
+-rw-rw-rw-   0        0        0      785 2023-07-26 16:14:50.000000 pymeili-0.1.5/pymeili/__init__.py
+-rw-rw-rw-   0        0        0    55863 2023-07-26 16:18:19.000000 pymeili-0.1.5/pymeili/beautifyplot.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:18:48.949518 pymeili-0.1.5/pymeili.egg-info/
+-rw-rw-rw-   0        0        0     1480 2023-07-26 16:18:48.000000 pymeili-0.1.5/pymeili.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-07-26 16:18:48.000000 pymeili-0.1.5/pymeili.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 16:18:48.000000 pymeili-0.1.5/pymeili.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-26 16:18:48.000000 pymeili-0.1.5/pymeili.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 16:18:48.968382 pymeili-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      741 2023-07-26 14:22:16.000000 pymeili-0.1.5/setup.py
```

### Comparing `pymeili-0.1.3/LISCENCE.txt` & `pymeili-0.1.5/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.3/PKG-INFO` & `pymeili-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.1.3
+Version: 0.1.5
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 
-pymeili is a module to beautify your python plot with more simple way.
+pymeili is a module to beautify your python plot with more simple way. the design idea is from Navigraph aeronautical chart.
 
 【IMPORTANT】
 Before using this module, you need to install font-packages: https://dwl.freefontsfamily.com/download/futura/; moving the font file to installed module folder(e.g. C:\Users\Username\AppData\Local\Programs\Python\Python311\Lib\site-packages\pymeili).
-For more information and instruction, please go to https://github.com/VVVICTORZHOU/resources.git.
+For more information and instruction, please go to https://github.com/VVVICTORZHOU/resources.git; or you can just download the font file from the link above.
 
 
 Install guide: (run on your powershell or cmd)
 > pip install pymeili
 
 Update guide: (run on your powershell or cmd)
 > pip install --upgrade pymeili
@@ -41,7 +41,10 @@
 - Fix Some Problems
 
 0.1.0 (26/07/2023)
 - Add Subplot Function
 
 0.1.3 (26/07/2023)
 - Fix Some Minor Problems
+
+0.1.5 (27/07/2023)
+- Add Basic Basemap Function, fix some problems
```

### Comparing `pymeili-0.1.3/pymeili/FONT/Futura Extra Black font.ttf` & `pymeili-0.1.5/pymeili/FONT/Futura Extra Black font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.3/pymeili/FONT/Futura Heavy font.ttf` & `pymeili-0.1.5/pymeili/FONT/Futura Heavy font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.3/pymeili/FONT/futura medium bt.ttf` & `pymeili-0.1.5/pymeili/FONT/futura medium bt.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.3/pymeili/__init__.py` & `pymeili-0.1.5/pymeili/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,22 @@
     colorlist,
     cmaplist,
     getBARHNO,
     getBARNO,
     getHISTNO,
     getPLOTNO,
     getSCATTERNO,
-    savefig,
     title, lefttitle, righttitle,
     scatter, plot, bar, hist, hist2d, pie, barh, table,
-    contour, contourf, colorbar, 
+    contour, contourf, colorbar, polar,
     xlabel, ylabel, xticks, yticks, xyticks, ticksall,
     xlim, ylim, xylim, xscale, yscale, xlog, ylog,
     grid, spines, legend, hidespines, xaxisposition, yaxisposition,
-    axhline, axvline, text, labeltext, 
+    axhline, axvline, text, labeltext, annotate,
     fill_between, fill_betweenx,
-    figsize, show, clf, close, figure,
+    pause, normalize, adjust, addaxes, slider, set_xydata,
+    figsize, show, clf, close, figure, savefig,
     imread, imshow, imsave,
     
 )
 
-__version__: str = '0.1.3'
+__version__: str = '0.1.5'
```

### Comparing `pymeili-0.1.3/pymeili/beautifyplot.py` & `pymeili-0.1.5/pymeili/beautifyplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,16 +256,16 @@
     plt.plot(x, y, color=colorlist(color), linewidth=linewidth, label=label,linestyle=linestyle, **kwargs)
 
 # boxplot繪圖
 def boxplot(x, vert=True, patch_artist=True, showmeans = True, showcaps = True, showbox = True, widths = 0.5, boxfacecolor='1', boxcolor='fg', boxlinewidth=3, capcolor='fg', caplinewidth=3, whiskercolor='fg', whiskerlinewidth=3, fliercolor='fg', fliermarkeredgecolor='fg', flierlinewidth=3, mediancolor='fg', medianlinewidth=3, meancolor='fg', meanmarker='D', meanmarkeredgecolor='fg', meanmarkerfacecolor='2', meansize=20, meanmarkeredgewidth=3, **kwargs):
     plt.boxplot(x, vert=vert, patch_artist=patch_artist, showmeans = showmeans, showcaps = showcaps, showbox = showbox, widths = widths, boxprops=dict(facecolor=colorlist(boxfacecolor), color=colorlist(boxcolor), linewidth = boxlinewidth), capprops=dict(color=colorlist(capcolor), linewidth = caplinewidth), whiskerprops=dict(color=colorlist(whiskercolor), linewidth = whiskerlinewidth), flierprops=dict(color=colorlist(fliercolor), markeredgecolor=colorlist(fliermarkeredgecolor), linewidth = flierlinewidth), medianprops=dict(color=colorlist(mediancolor), linewidth = medianlinewidth), meanprops=dict(marker=meanmarker, markeredgecolor=colorlist(meanmarkeredgecolor), markerfacecolor=colorlist(meanmarkerfacecolor), markersize=meansize, markeredgewidth = meanmarkeredgewidth), **kwargs)
 
 # polar繪圖
-def polar(theta, r, color='fg', linewidth=2, linestyle='-',**kwargs):
-    plt.polar(theta, r, color=colorlist(color), linewidth=linewidth,linestyle=linestyle, **kwargs)
+def polar(theta, r, color='fg', linewidth=2, linestyle='-', label=getPLOTNO(),**kwargs):
+    plt.polar(theta, r, color=colorlist(color), linewidth=linewidth, label=label,linestyle=linestyle, **kwargs)
 
 # contour繪圖
 def contour(x, y, z, colors='fg', levels=10, linewidths=2, clabel=True, fontsize=12, color='fg', **kwargs):
     CS = plt.contour(x, y, z, colors=colorlist(colors), levels=levels, linewidths=linewidths, **kwargs)
     if clabel == True:
         CL = CS.clabel(fontsize=fontsize, colors=colorlist(color), inline=True)
 
@@ -491,14 +491,21 @@
 
 def imshow(X, cmap='2', vmin=None, vmax=None, interpolation='nearest', alpha=None, aspect=None, **kwargs):
     plt.imshow(X, cmap=cmaplist(cmap), vmin=vmin, vmax=vmax, interpolation=interpolation, alpha=alpha, aspect=aspect, **kwargs)
 
 def imsave(filename, arr, vmin=None, vmax=None, cmap='2', format=None, origin=None, dpi=300, **kwargs):
     plt.imsave(filename, arr, vmin=vmin, vmax=vmax, cmap=cmaplist(cmap), format=format, origin=origin, dpi=dpi, **kwargs)
 
+# 重設值
+def set_xydata(x=None, y=None):
+    if x != None:
+        plt.gca().set_xdata(x)
+    if y != None:
+        plt.gca().set_ydata(y)
+
 
 
 # Basemap系列
 class Basemap():
     import numpy as np
     def __init__(self,projection='cyl', llcrnrlon=0, llcrnrlat=0, urcrnrlon=0, urcrnrlat=0, resolution='l', area_thresh=1000, zone=None,**kwargs):
         self.projection = projection # merc:麥卡托, cyl:等距圓柱, mill:米勒, cea:等距圓錐, gall:加爾-彼得, lcc:蘭伯特等角, tmerc:橫麥卡托, stere:極射, npstere:北極極射, spstere:南極極射, aeqd:等距方位, poly:多邊形, nsper:自然地球
@@ -890,15 +897,14 @@
     # 繪製散點圖
     def scatter(self, x, y, color='fg', size=3, marker='o', linewidth=None, label=getSCATTERNO(), linestyle='-', **kwargs):
         self.ax[self.row,self.col].scatter(x, y, color=colorlist(color), s=size, marker=marker, linewidth=linewidth, label=label, linestyle=linestyle, **kwargs)
     # 繪製polar圖
     def polar(self, theta, r, color='fg', linewidth=2, linestyle='-', **kwargs):
         self.ax[self.row,self.col].polar(theta, r, color=colorlist(color), linewidth=linewidth, linestyle=linestyle, **kwargs)
     
-    
     # 繪製等值線
     def contour(self, x, y, z, colors='fg', levels=10, linewidths=2, clabel=True, fontsize=12*fontscale, color='fg', **kwargs):
         CS = self.ax[self.row,self.col].contour(x, y, z, colors=colorlist(colors), levels=levels, linewidths=linewidths, **kwargs)
         if clabel == True:
             CL = CS.clabel(fontsize=fontsize, colors=colorlist(color), inline=True)
     # 繪製等值線填色圖
     def contourf(self, x, y, z, levels=10, cmap='2', contour=True, clabel=True,linewidths=1.5, color='fg', **kwargs):
@@ -987,22 +993,39 @@
         if labelbottom: self.ax[self.row,self.col].tick_params(labelbottom=labelbottom, **kwargs)
         if labelleft: self.ax[self.row,self.col].tick_params(labelleft=labelleft, **kwargs)
         if labelright: self.ax[self.row,self.col].tick_params(labelright=labelright, **kwargs)
 
     # 大標題
     def suptitle(self, title, color='fg', font=fontpath_bold,fontsize=30, **kwargs):
         self.fig.suptitle(title, color=colorlist(color), fontproperties=fm.FontProperties(fname=font, size=fontsize), **kwargs)
-    
-
-
-
-
 
+    # 挪出額外空間
+    def adjust(self, left=None, bottom=None, right=None, top=None, wspace=None, hspace=None):
+        plt.subplots_adjust(left=left, bottom=bottom, right=right, top=top, wspace=wspace, hspace=hspace)
+    # 新增軸
+    def addaxes(self, position, **kwargs):
+        self.ax[self.row,self.col].add_axes(position, **kwargs)
 
+    # 重設值
+    def set_xydata(self, x=None, y=None):
+        if x != None: self.ax[self.row,self.col].set_xdata(x)
+        if y != None: self.ax[self.row,self.col].set_ydata(y)
+    
+    
+# 動畫
+from matplotlib.widgets import Slider, Button, RadioButtons
+def pause(interval=0.01):
+    plt.pause(interval)
 
+def normalize(data, vmin=None, vmax=None):
+    plt.Normalize(data, vmin=vmin, vmax=vmax)
 
+def slider(ax, label, valmin, valmax, valinit=0, valfmt='%1.2f', valstep=None, orientation='horizontal', **kwargs):
+    return Slider(ax, label, valmin, valmax, valinit=valinit, valfmt=valfmt, valstep=valstep, orientation=orientation, **kwargs)
 
 
+# https://matplotlib.org/stable/gallery/widgets/slider_demo.html
 
 
 
 
+
```

### Comparing `pymeili-0.1.3/pymeili.egg-info/PKG-INFO` & `pymeili-0.1.5/pymeili.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.1.3
+Version: 0.1.5
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 
-pymeili is a module to beautify your python plot with more simple way.
+pymeili is a module to beautify your python plot with more simple way. the design idea is from Navigraph aeronautical chart.
 
 【IMPORTANT】
 Before using this module, you need to install font-packages: https://dwl.freefontsfamily.com/download/futura/; moving the font file to installed module folder(e.g. C:\Users\Username\AppData\Local\Programs\Python\Python311\Lib\site-packages\pymeili).
-For more information and instruction, please go to https://github.com/VVVICTORZHOU/resources.git.
+For more information and instruction, please go to https://github.com/VVVICTORZHOU/resources.git; or you can just download the font file from the link above.
 
 
 Install guide: (run on your powershell or cmd)
 > pip install pymeili
 
 Update guide: (run on your powershell or cmd)
 > pip install --upgrade pymeili
@@ -41,7 +41,10 @@
 - Fix Some Problems
 
 0.1.0 (26/07/2023)
 - Add Subplot Function
 
 0.1.3 (26/07/2023)
 - Fix Some Minor Problems
+
+0.1.5 (27/07/2023)
+- Add Basic Basemap Function, fix some problems
```

### Comparing `pymeili-0.1.3/setup.py` & `pymeili-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='pymeili',
-    version='0.1.3',
+    version='0.1.5',
     description='a module to beautify your python plot.',
     long_description=open('README.txt',encoding="utf-8").read() + '\n\n' + open('CHANGELOG.txt',encoding="utf-8").read(),
     url='',
     author='VVVictorZhou',
     author_email='vichouro@gmail.com',
     license='MIT',
     classifiers=classifiers,
```


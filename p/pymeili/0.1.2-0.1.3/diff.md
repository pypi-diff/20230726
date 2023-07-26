# Comparing `tmp/pymeili-0.1.2.tar.gz` & `tmp/pymeili-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeili-0.1.2.tar", last modified: Wed Jul 26 11:38:24 2023, max compression
+gzip compressed data, was "pymeili-0.1.3.tar", last modified: Wed Jul 26 14:20:02 2023, max compression
```

## Comparing `pymeili-0.1.2.tar` & `pymeili-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:24.208387 pymeili-0.1.2/
--rw-rw-rw-   0        0        0      243 2023-07-26 11:35:22.000000 pymeili-0.1.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.1.2/LISCENCE.txt
--rw-rw-rw-   0        0        0       36 2023-07-25 15:28:50.000000 pymeili-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1190 2023-07-26 11:38:24.208387 pymeili-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      495 2023-07-25 15:43:41.000000 pymeili-0.1.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:24.195427 pymeili-0.1.2/pymeili/
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:24.207389 pymeili-0.1.2/pymeili/FONT/
--rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.1.2/pymeili/FONT/Futura Extra Black font.ttf
--rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.1.2/pymeili/FONT/Futura Heavy font.ttf
--rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.1.2/pymeili/FONT/futura medium bt.ttf
--rw-rw-rw-   0        0        0      714 2023-07-26 11:37:57.000000 pymeili-0.1.2/pymeili/__init__.py
--rw-rw-rw-   0        0        0    54186 2023-07-26 11:36:34.000000 pymeili-0.1.2/pymeili/beautifyplot.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:38:24.204397 pymeili-0.1.2/pymeili.egg-info/
--rw-rw-rw-   0        0        0     1190 2023-07-26 11:38:24.000000 pymeili-0.1.2/pymeili.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-07-26 11:38:24.000000 pymeili-0.1.2/pymeili.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 11:38:24.000000 pymeili-0.1.2/pymeili.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-26 11:38:24.000000 pymeili-0.1.2/pymeili.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 11:38:24.208387 pymeili-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      741 2023-07-26 11:35:26.000000 pymeili-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:20:02.046693 pymeili-0.1.3/
+-rw-rw-rw-   0        0        0      243 2023-07-26 13:10:45.000000 pymeili-0.1.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.1.3/LISCENCE.txt
+-rw-rw-rw-   0        0        0       36 2023-07-25 15:28:50.000000 pymeili-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1295 2023-07-26 14:20:02.046693 pymeili-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2023-07-26 13:10:34.000000 pymeili-0.1.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 14:20:02.016217 pymeili-0.1.3/pymeili/
+drwxrwxrwx   0        0        0        0 2023-07-26 14:20:02.045694 pymeili-0.1.3/pymeili/FONT/
+-rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.1.3/pymeili/FONT/Futura Extra Black font.ttf
+-rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.1.3/pymeili/FONT/Futura Heavy font.ttf
+-rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.1.3/pymeili/FONT/futura medium bt.ttf
+-rw-rw-rw-   0        0        0      715 2023-07-26 14:19:47.000000 pymeili-0.1.3/pymeili/__init__.py
+-rw-rw-rw-   0        0        0    54618 2023-07-26 14:18:21.000000 pymeili-0.1.3/pymeili/beautifyplot.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:20:02.031179 pymeili-0.1.3/pymeili.egg-info/
+-rw-rw-rw-   0        0        0     1295 2023-07-26 14:20:01.000000 pymeili-0.1.3/pymeili.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-07-26 14:20:01.000000 pymeili-0.1.3/pymeili.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 14:20:01.000000 pymeili-0.1.3/pymeili.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-26 14:20:01.000000 pymeili-0.1.3/pymeili.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 14:20:02.046693 pymeili-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      741 2023-07-26 13:10:58.000000 pymeili-0.1.3/setup.py
```

### Comparing `pymeili-0.1.2/LISCENCE.txt` & `pymeili-0.1.3/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.2/PKG-INFO` & `pymeili-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.1.2
+Version: 0.1.3
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
@@ -13,21 +13,25 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 
 pymeili is a module to beautify your python plot with more simple way.
 
 【IMPORTANT】
 Before using this module, you need to install font-packages: https://dwl.freefontsfamily.com/download/futura/; moving the font file to installed module folder(e.g. C:\Users\Username\AppData\Local\Programs\Python\Python311\Lib\site-packages\pymeili).
+For more information and instruction, please go to https://github.com/VVVICTORZHOU/resources.git.
+
 
 Install guide: (run on your powershell or cmd)
 > pip install pymeili
 
 Update guide: (run on your powershell or cmd)
 > pip install --upgrade pymeili
 
+
+
 Change Log
 ==========
 
 0.0.1 (25/07/2023)
 - First Release
 
 0.0.2 (25/07/2023)
@@ -35,9 +39,9 @@
 
 0.0.10 (25/07/2023)
 - Fix Some Problems
 
 0.1.0 (26/07/2023)
 - Add Subplot Function
 
-0.1.2 (26/07/2023)
+0.1.3 (26/07/2023)
 - Fix Some Minor Problems
```

### Comparing `pymeili-0.1.2/pymeili/FONT/Futura Extra Black font.ttf` & `pymeili-0.1.3/pymeili/FONT/Futura Extra Black font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.2/pymeili/FONT/Futura Heavy font.ttf` & `pymeili-0.1.3/pymeili/FONT/Futura Heavy font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.2/pymeili/FONT/futura medium bt.ttf` & `pymeili-0.1.3/pymeili/FONT/futura medium bt.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.1.2/pymeili/__init__.py` & `pymeili-0.1.3/pymeili/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     getBARNO,
     getHISTNO,
     getPLOTNO,
     getSCATTERNO,
     savefig,
     title, lefttitle, righttitle,
     scatter, plot, bar, hist, hist2d, pie, barh, table,
-    contour, contourf, colorbar,
+    contour, contourf, colorbar, 
     xlabel, ylabel, xticks, yticks, xyticks, ticksall,
     xlim, ylim, xylim, xscale, yscale, xlog, ylog,
     grid, spines, legend, hidespines, xaxisposition, yaxisposition,
     axhline, axvline, text, labeltext, 
     fill_between, fill_betweenx,
     figsize, show, clf, close, figure,
     imread, imshow, imsave,
     
 )
 
-__version__: str = '0.1.2'
+__version__: str = '0.1.3'
```

### Comparing `pymeili-0.1.2/pymeili/beautifyplot.py` & `pymeili-0.1.3/pymeili/beautifyplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,14 +255,18 @@
 def plot(x, y, color='fg', linewidth=2, linestyle='-', label=getPLOTNO(),**kwargs):
     plt.plot(x, y, color=colorlist(color), linewidth=linewidth, label=label,linestyle=linestyle, **kwargs)
 
 # boxplot繪圖
 def boxplot(x, vert=True, patch_artist=True, showmeans = True, showcaps = True, showbox = True, widths = 0.5, boxfacecolor='1', boxcolor='fg', boxlinewidth=3, capcolor='fg', caplinewidth=3, whiskercolor='fg', whiskerlinewidth=3, fliercolor='fg', fliermarkeredgecolor='fg', flierlinewidth=3, mediancolor='fg', medianlinewidth=3, meancolor='fg', meanmarker='D', meanmarkeredgecolor='fg', meanmarkerfacecolor='2', meansize=20, meanmarkeredgewidth=3, **kwargs):
     plt.boxplot(x, vert=vert, patch_artist=patch_artist, showmeans = showmeans, showcaps = showcaps, showbox = showbox, widths = widths, boxprops=dict(facecolor=colorlist(boxfacecolor), color=colorlist(boxcolor), linewidth = boxlinewidth), capprops=dict(color=colorlist(capcolor), linewidth = caplinewidth), whiskerprops=dict(color=colorlist(whiskercolor), linewidth = whiskerlinewidth), flierprops=dict(color=colorlist(fliercolor), markeredgecolor=colorlist(fliermarkeredgecolor), linewidth = flierlinewidth), medianprops=dict(color=colorlist(mediancolor), linewidth = medianlinewidth), meanprops=dict(marker=meanmarker, markeredgecolor=colorlist(meanmarkeredgecolor), markerfacecolor=colorlist(meanmarkerfacecolor), markersize=meansize, markeredgewidth = meanmarkeredgewidth), **kwargs)
 
+# polar繪圖
+def polar(theta, r, color='fg', linewidth=2, linestyle='-',**kwargs):
+    plt.polar(theta, r, color=colorlist(color), linewidth=linewidth,linestyle=linestyle, **kwargs)
+
 # contour繪圖
 def contour(x, y, z, colors='fg', levels=10, linewidths=2, clabel=True, fontsize=12, color='fg', **kwargs):
     CS = plt.contour(x, y, z, colors=colorlist(colors), levels=levels, linewidths=linewidths, **kwargs)
     if clabel == True:
         CL = CS.clabel(fontsize=fontsize, colors=colorlist(color), inline=True)
 
 # contourf繪圖
@@ -882,14 +886,19 @@
         self.ax[self.row,self.col].barh(x, y, height=width, color=colorlist(color), edgecolor=colorlist(edgecolor), linewidth=linewidth, label=label, **kwargs)
     # 繪製直方圖
     def hist(self, x, bins=5, color='1', edgecolor='fg', linewidth=3, label=getHISTNO(), **kwargs):
         self.ax[self.row,self.col].hist(x, bins=bins, color=colorlist(color), edgecolor=colorlist(edgecolor), linewidth=linewidth, label=label,**kwargs)
     # 繪製散點圖
     def scatter(self, x, y, color='fg', size=3, marker='o', linewidth=None, label=getSCATTERNO(), linestyle='-', **kwargs):
         self.ax[self.row,self.col].scatter(x, y, color=colorlist(color), s=size, marker=marker, linewidth=linewidth, label=label, linestyle=linestyle, **kwargs)
+    # 繪製polar圖
+    def polar(self, theta, r, color='fg', linewidth=2, linestyle='-', **kwargs):
+        self.ax[self.row,self.col].polar(theta, r, color=colorlist(color), linewidth=linewidth, linestyle=linestyle, **kwargs)
+    
+    
     # 繪製等值線
     def contour(self, x, y, z, colors='fg', levels=10, linewidths=2, clabel=True, fontsize=12*fontscale, color='fg', **kwargs):
         CS = self.ax[self.row,self.col].contour(x, y, z, colors=colorlist(colors), levels=levels, linewidths=linewidths, **kwargs)
         if clabel == True:
             CL = CS.clabel(fontsize=fontsize, colors=colorlist(color), inline=True)
     # 繪製等值線填色圖
     def contourf(self, x, y, z, levels=10, cmap='2', contour=True, clabel=True,linewidths=1.5, color='fg', **kwargs):
```

### Comparing `pymeili-0.1.2/pymeili.egg-info/PKG-INFO` & `pymeili-0.1.3/pymeili.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeili
-Version: 0.1.2
+Version: 0.1.3
 Summary: a module to beautify your python plot.
 Home-page: 
 Author: VVVictorZhou
 Author-email: vichouro@gmail.com
 License: MIT
 Keywords: beautify
 Classifier: Development Status :: 4 - Beta
@@ -13,21 +13,25 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 
 pymeili is a module to beautify your python plot with more simple way.
 
 【IMPORTANT】
 Before using this module, you need to install font-packages: https://dwl.freefontsfamily.com/download/futura/; moving the font file to installed module folder(e.g. C:\Users\Username\AppData\Local\Programs\Python\Python311\Lib\site-packages\pymeili).
+For more information and instruction, please go to https://github.com/VVVICTORZHOU/resources.git.
+
 
 Install guide: (run on your powershell or cmd)
 > pip install pymeili
 
 Update guide: (run on your powershell or cmd)
 > pip install --upgrade pymeili
 
+
+
 Change Log
 ==========
 
 0.0.1 (25/07/2023)
 - First Release
 
 0.0.2 (25/07/2023)
@@ -35,9 +39,9 @@
 
 0.0.10 (25/07/2023)
 - Fix Some Problems
 
 0.1.0 (26/07/2023)
 - Add Subplot Function
 
-0.1.2 (26/07/2023)
+0.1.3 (26/07/2023)
 - Fix Some Minor Problems
```

### Comparing `pymeili-0.1.2/setup.py` & `pymeili-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='pymeili',
-    version='0.1.2',
+    version='0.1.3',
     description='a module to beautify your python plot.',
     long_description=open('README.txt',encoding="utf-8").read() + '\n\n' + open('CHANGELOG.txt',encoding="utf-8").read(),
     url='',
     author='VVVictorZhou',
     author_email='vichouro@gmail.com',
     license='MIT',
     classifiers=classifiers,
```


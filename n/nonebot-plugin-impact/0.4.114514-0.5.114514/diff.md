# Comparing `tmp/nonebot_plugin_impact-0.4.114514.tar.gz` & `tmp/nonebot_plugin_impact-0.5.114514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_impact-0.4.114514.tar", last modified: Mon Jul 24 16:39:28 2023, max compression
+gzip compressed data, was "nonebot_plugin_impact-0.5.114514.tar", last modified: Wed Jul 26 18:54:58 2023, max compression
```

## Comparing `nonebot_plugin_impact-0.4.114514.tar` & `nonebot_plugin_impact-0.5.114514.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 16:39:28.868037 nonebot_plugin_impact-0.4.114514/
--rw-rw-rw-   0        0        0     1090 2023-01-30 13:38:17.000000 nonebot_plugin_impact-0.4.114514/LICENSE
--rw-rw-rw-   0        0        0      306 2023-07-24 16:39:28.867535 nonebot_plugin_impact-0.4.114514/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-24 16:39:28.851038 nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact/
--rw-rw-rw-   0        0        0     2093 2023-07-24 16:38:21.000000 nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact/__init__.py
--rw-rw-rw-   0        0        0     9174 2023-07-24 16:37:35.000000 nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact/draw_img.py
-drwxrwxrwx   0        0        0        0 2023-07-24 16:39:28.858536 nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact/fonts/
--rw-rw-rw-   0        0        0  6700204 2015-07-29 19:27:52.000000 nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact/fonts/SIMYOU.TTF
--rw-rw-rw-   0        0        0    20206 2023-07-24 16:35:42.000000 nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact/handle.py
--rw-rw-rw-   0        0        0     2205 2023-07-24 16:35:42.000000 nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact/txt2img.py
--rw-rw-rw-   0        0        0     8628 2023-07-24 16:35:42.000000 nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-24 16:39:28.857039 nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact.egg-info/
--rw-rw-rw-   0        0        0      306 2023-07-24 16:39:28.000000 nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      443 2023-07-24 16:39:28.000000 nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 16:39:28.000000 nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-24 16:39:28.000000 nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-24 16:39:28.000000 nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 16:39:28.868535 nonebot_plugin_impact-0.4.114514/setup.cfg
--rw-rw-rw-   0        0        0      543 2023-07-24 16:39:19.000000 nonebot_plugin_impact-0.4.114514/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:54:58.166345 nonebot_plugin_impact-0.5.114514/
+-rw-rw-rw-   0        0        0     1090 2023-01-30 13:38:17.000000 nonebot_plugin_impact-0.5.114514/LICENSE
+-rw-rw-rw-   0        0        0      306 2023-07-26 18:54:58.165344 nonebot_plugin_impact-0.5.114514/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 18:54:58.093484 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/
+-rw-rw-rw-   0        0        0     2093 2023-07-26 18:53:36.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/__init__.py
+-rw-rw-rw-   0        0        0     9180 2023-07-26 18:53:23.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/draw_img.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:54:58.100484 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/fonts/
+-rw-rw-rw-   0        0        0  6700204 2015-07-29 19:27:52.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/fonts/SIMYOU.TTF
+-rw-rw-rw-   0        0        0    20206 2023-07-26 18:52:03.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/handle.py
+-rw-rw-rw-   0        0        0     2205 2023-07-26 18:52:03.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/txt2img.py
+-rw-rw-rw-   0        0        0     8628 2023-07-26 18:52:03.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:54:58.098985 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact.egg-info/
+-rw-rw-rw-   0        0        0      306 2023-07-26 18:54:57.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2023-07-26 18:54:57.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 18:54:57.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-26 18:54:57.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-26 18:54:57.000000 nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 18:54:58.166844 nonebot_plugin_impact-0.5.114514/setup.cfg
+-rw-rw-rw-   0        0        0      543 2023-07-26 18:54:19.000000 nonebot_plugin_impact-0.5.114514/setup.py
```

### Comparing `nonebot_plugin_impact-0.4.114514/LICENSE` & `nonebot_plugin_impact-0.5.114514/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact/__init__.py` & `nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,11 +85,11 @@
         description="让群友们眼前一黑的nonebot2淫趴插件",
         usage=utils.usage,
         type="application",
         homepage="https://github.com/Special-Week/nonebot_plugin_impact",
         supported_adapters={"~onebot.v11"},
         extra={
             "author": "Special-Week",
-            "version": "0.04.114514",
+            "version": "0.05.114514",
             "priority": 20,
         },
     )
```

### Comparing `nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact/draw_img.py` & `nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/draw_img.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
             while x < x_end:
                 x_dash_end = min(x + dash_length, x_end)
                 draw.line((x, y, x_dash_end, y), fill="black", width=1)
                 x += dash_length + gap_length
 
         for i in range(10):
             draw_dotted_line(1000 - 950 * i / 10)
-        maxnum_scale = int(maxnum_scale / 50) * 20
+        maxnum_scale = int((maxnum_scale / 20 + 1) * 20)
         if maxnum_scale == 0:
             maxnum_scale = 20
 
         for i in range(10):
             draw.text(
                 (450, 1000 - 950 * i / 10 - 10),
                 str(maxnum_scale * i),
```

### Comparing `nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact/fonts/SIMYOU.TTF` & `nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/fonts/SIMYOU.TTF`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact/handle.py` & `nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact/txt2img.py` & `nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/txt2img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.4.114514/nonebot_plugin_impact/utils.py` & `nonebot_plugin_impact-0.5.114514/nonebot_plugin_impact/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_impact-0.4.114514/setup.py` & `nonebot_plugin_impact-0.5.114514/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="nonebot_plugin_impact",
-    version="0.04.114514",
+    version="0.05.114514",
     author="Special-Week",
     author_email="HuaMing27499@gmail.com",
     description="让群友们眼前一黑的nonebot2淫趴插件",
     python_requires=">=3.8.0",
     packages=find_packages(),
     url="https://github.com/Special-Week/nonebot_plugin_impact",
     package_data={"nonebot_plugin_impact": ["fonts/*"]},
```


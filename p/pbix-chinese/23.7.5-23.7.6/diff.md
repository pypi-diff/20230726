# Comparing `tmp/pbix_chinese-23.7.5.tar.gz` & `tmp/pbix_chinese-23.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbix_chinese-23.7.5.tar", last modified: Wed Jul 26 09:26:06 2023, max compression
+gzip compressed data, was "pbix_chinese-23.7.6.tar", last modified: Wed Jul 26 09:51:06 2023, max compression
```

## Comparing `pbix_chinese-23.7.5.tar` & `pbix_chinese-23.7.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 09:26:06.651664 pbix_chinese-23.7.5/
--rw-rw-rw-   0        0        0       99 2023-07-26 09:26:06.650665 pbix_chinese-23.7.5/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-07-17 07:47:27.000000 pbix_chinese-23.7.5/README.txt
--rw-rw-rw-   0        0        0       52 2023-07-15 07:22:48.000000 pbix_chinese-23.7.5/license.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 09:26:06.637673 pbix_chinese-23.7.5/pbix_chinese/
--rw-rw-rw-   0        0        0       51 2023-07-17 07:53:45.000000 pbix_chinese-23.7.5/pbix_chinese/__init__.py
--rw-rw-rw-   0        0        0     1989 2023-07-26 09:22:11.000000 pbix_chinese-23.7.5/pbix_chinese/pbix_refresher.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:26:06.647668 pbix_chinese-23.7.5/pbix_chinese.egg-info/
--rw-rw-rw-   0        0        0       99 2023-07-26 09:26:06.000000 pbix_chinese-23.7.5/pbix_chinese.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-07-26 09:26:06.000000 pbix_chinese-23.7.5/pbix_chinese.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 09:26:06.000000 pbix_chinese-23.7.5/pbix_chinese.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-26 09:26:06.000000 pbix_chinese-23.7.5/pbix_chinese.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 09:26:06.651664 pbix_chinese-23.7.5/setup.cfg
--rw-rw-rw-   0        0        0      221 2023-07-26 09:25:55.000000 pbix_chinese-23.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:51:06.456068 pbix_chinese-23.7.6/
+-rw-rw-rw-   0        0        0       99 2023-07-26 09:51:06.455068 pbix_chinese-23.7.6/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-07-17 07:47:27.000000 pbix_chinese-23.7.6/README.txt
+-rw-rw-rw-   0        0        0       52 2023-07-15 07:22:48.000000 pbix_chinese-23.7.6/license.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 09:51:06.439078 pbix_chinese-23.7.6/pbix_chinese/
+-rw-rw-rw-   0        0        0       51 2023-07-17 07:53:45.000000 pbix_chinese-23.7.6/pbix_chinese/__init__.py
+-rw-rw-rw-   0        0        0     1931 2023-07-26 09:50:13.000000 pbix_chinese-23.7.6/pbix_chinese/pbix_refresher.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:51:06.451070 pbix_chinese-23.7.6/pbix_chinese.egg-info/
+-rw-rw-rw-   0        0        0       99 2023-07-26 09:51:06.000000 pbix_chinese-23.7.6/pbix_chinese.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-07-26 09:51:06.000000 pbix_chinese-23.7.6/pbix_chinese.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 09:51:06.000000 pbix_chinese-23.7.6/pbix_chinese.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-26 09:51:06.000000 pbix_chinese-23.7.6/pbix_chinese.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 09:51:06.456068 pbix_chinese-23.7.6/setup.cfg
+-rw-rw-rw-   0        0        0      221 2023-07-26 09:50:36.000000 pbix_chinese-23.7.6/setup.py
```

### Comparing `pbix_chinese-23.7.5/pbix_chinese/pbix_refresher.py` & `pbix_chinese-23.7.6/pbix_chinese/pbix_refresher.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,27 +38,24 @@
     # print(get_time(), "启动Powerbi")
     os.system('start "" "' + file_path + '"')
     time.sleep(wait)
 
     # 连接power bi
     app = Application(backend='uia').connect(path=procname)
     win = app.window(title_re='.*Power BI Desktop')
-    win.wait("enabled", timeout=60)
+    win.wait("enabled", timeout=15)
     win.set_focus()
-    time.sleep(30)
     # win['主页'].click_input()
     # win['刷新'].wait("enabled", timeout=60)
     # win.set_focus()
     win['刷新'].click_input()
-    time.sleep(2)
     win.wait("enabled", timeout=re_timeout)
 
     win.type_keys("^s")
-    time.sleep(2)
-    win.wait("enabled", timeout=30)
+    win.wait("enabled", timeout=15)
     win.close()
     # print(get_time(), '已保存')
 
     for proc in psutil.process_iter():
         if proc.name() == procname:
             proc.kill()
```


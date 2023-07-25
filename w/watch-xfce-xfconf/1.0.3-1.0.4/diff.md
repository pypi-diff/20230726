# Comparing `tmp/watch-xfce-xfconf-1.0.3.tar.gz` & `tmp/watch-xfce-xfconf-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watch-xfce-xfconf-1.0.3.tar", last modified: Mon Oct 24 22:33:18 2022, max compression
+gzip compressed data, was "watch-xfce-xfconf-1.0.4.tar", last modified: Tue Jul 25 22:01:11 2023, max compression
```

## Comparing `watch-xfce-xfconf-1.0.3.tar` & `watch-xfce-xfconf-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2022-10-24 22:33:18.881383 watch-xfce-xfconf-1.0.3/
--rw-r--r--   0 work      (1000) work      (1000)     1064 2022-04-14 15:35:22.000000 watch-xfce-xfconf-1.0.3/LICENSE
--rw-r--r--   0 work      (1000) work      (1000)     2473 2022-10-24 22:33:18.881383 watch-xfce-xfconf-1.0.3/PKG-INFO
--rw-r--r--   0 work      (1000) work      (1000)     1343 2022-04-25 14:02:11.000000 watch-xfce-xfconf-1.0.3/README.md
--rw-r--r--   0 work      (1000) work      (1000)       38 2022-10-24 22:33:18.881383 watch-xfce-xfconf-1.0.3/setup.cfg
--rwxr-xr-x   0 work      (1000) work      (1000)     1710 2022-10-24 22:27:29.000000 watch-xfce-xfconf-1.0.3/setup.py
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2022-10-24 22:33:18.881383 watch-xfce-xfconf-1.0.3/watch_xfce_xfconf/
--rw-r--r--   0 work      (1000) work      (1000)     2435 2022-04-25 14:02:11.000000 watch-xfce-xfconf-1.0.3/watch_xfce_xfconf/__init__.py
--rw-r--r--   0 work      (1000) work      (1000)     7784 2022-10-24 22:21:38.000000 watch-xfce-xfconf-1.0.3/watch_xfce_xfconf/xfconf.py
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2022-10-24 22:33:18.881383 watch-xfce-xfconf-1.0.3/watch_xfce_xfconf.egg-info/
--rw-r--r--   0 work      (1000) work      (1000)     2473 2022-10-24 22:33:18.000000 watch-xfce-xfconf-1.0.3/watch_xfce_xfconf.egg-info/PKG-INFO
--rw-r--r--   0 work      (1000) work      (1000)      332 2022-10-24 22:33:18.000000 watch-xfce-xfconf-1.0.3/watch_xfce_xfconf.egg-info/SOURCES.txt
--rw-r--r--   0 work      (1000) work      (1000)        1 2022-10-24 22:33:18.000000 watch-xfce-xfconf-1.0.3/watch_xfce_xfconf.egg-info/dependency_links.txt
--rw-r--r--   0 work      (1000) work      (1000)       83 2022-10-24 22:33:18.000000 watch-xfce-xfconf-1.0.3/watch_xfce_xfconf.egg-info/entry_points.txt
--rw-r--r--   0 work      (1000) work      (1000)       17 2022-10-24 22:33:18.000000 watch-xfce-xfconf-1.0.3/watch_xfce_xfconf.egg-info/requires.txt
--rw-r--r--   0 work      (1000) work      (1000)       18 2022-10-24 22:33:18.000000 watch-xfce-xfconf-1.0.3/watch_xfce_xfconf.egg-info/top_level.txt
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-07-25 22:01:11.788397 watch-xfce-xfconf-1.0.4/
+-rw-r--r--   0 work      (1000) work      (1000)     2035 2022-04-14 15:35:22.000000 watch-xfce-xfconf-1.0.4/.gitignore
+-rw-r--r--   0 work      (1000) work      (1000)     1064 2022-04-14 15:35:22.000000 watch-xfce-xfconf-1.0.4/LICENSE
+-rw-r--r--   0 work      (1000) work      (1000)     3645 2023-07-25 22:01:11.788397 watch-xfce-xfconf-1.0.4/PKG-INFO
+-rw-r--r--   0 work      (1000) work      (1000)     2515 2023-07-25 21:59:20.000000 watch-xfce-xfconf-1.0.4/README.md
+-rw-r--r--   0 work      (1000) work      (1000)       12 2023-07-25 21:59:20.000000 watch-xfce-xfconf-1.0.4/requirements.txt
+-rw-r--r--   0 work      (1000) work      (1000)       38 2023-07-25 22:01:11.788397 watch-xfce-xfconf-1.0.4/setup.cfg
+-rwxr-xr-x   0 work      (1000) work      (1000)     1702 2023-07-25 21:59:20.000000 watch-xfce-xfconf-1.0.4/setup.py
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-07-25 22:01:11.788397 watch-xfce-xfconf-1.0.4/watch_xfce_xfconf/
+-rw-r--r--   0 work      (1000) work      (1000)     2435 2022-04-25 14:02:11.000000 watch-xfce-xfconf-1.0.4/watch_xfce_xfconf/__init__.py
+-rw-r--r--   0 work      (1000) work      (1000)     7784 2022-10-24 22:21:38.000000 watch-xfce-xfconf-1.0.4/watch_xfce_xfconf/xfconf.py
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-07-25 22:01:11.788397 watch-xfce-xfconf-1.0.4/watch_xfce_xfconf.egg-info/
+-rw-r--r--   0 work      (1000) work      (1000)     3645 2023-07-25 22:01:11.000000 watch-xfce-xfconf-1.0.4/watch_xfce_xfconf.egg-info/PKG-INFO
+-rw-r--r--   0 work      (1000) work      (1000)      360 2023-07-25 22:01:11.000000 watch-xfce-xfconf-1.0.4/watch_xfce_xfconf.egg-info/SOURCES.txt
+-rw-r--r--   0 work      (1000) work      (1000)        1 2023-07-25 22:01:11.000000 watch-xfce-xfconf-1.0.4/watch_xfce_xfconf.egg-info/dependency_links.txt
+-rw-r--r--   0 work      (1000) work      (1000)       83 2023-07-25 22:01:11.000000 watch-xfce-xfconf-1.0.4/watch_xfce_xfconf.egg-info/entry_points.txt
+-rw-r--r--   0 work      (1000) work      (1000)       12 2023-07-25 22:01:11.000000 watch-xfce-xfconf-1.0.4/watch_xfce_xfconf.egg-info/requires.txt
+-rw-r--r--   0 work      (1000) work      (1000)       18 2023-07-25 22:01:11.000000 watch-xfce-xfconf-1.0.4/watch_xfce_xfconf.egg-info/top_level.txt
```

### Comparing `watch-xfce-xfconf-1.0.3/LICENSE` & `watch-xfce-xfconf-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `watch-xfce-xfconf-1.0.3/setup.py` & `watch-xfce-xfconf-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 CURRENT_DIRECTORY = Path(__file__).parent.resolve()
 LONG_DESCRIPTION = \
     (CURRENT_DIRECTORY / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="watch-xfce-xfconf",
 
-    version="1.0.3",
+    version="1.0.4",
     packages=find_packages(),
 
     description=("A command-line tool that can help you to configure XFCE 4 "
                  "programmatically"),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/jamescherti/watch-xfce-xfconf",
     author="James Cherti",
 
     python_requires=">=3.6, <4",
-    install_requires=['mypy', 'psutil', 'lxml'],
+    install_requires=['psutil', 'lxml'],
 
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: End Users/Desktop",
         "License :: OSI Approved :: MIT License",
         "Environment :: Console",
         "Environment :: X11 Applications",
```

### Comparing `watch-xfce-xfconf-1.0.3/watch_xfce_xfconf/__init__.py` & `watch-xfce-xfconf-1.0.4/watch_xfce_xfconf/__init__.py`

 * *Files identical despite different names*

### Comparing `watch-xfce-xfconf-1.0.3/watch_xfce_xfconf/xfconf.py` & `watch-xfce-xfconf-1.0.4/watch_xfce_xfconf/xfconf.py`

 * *Files identical despite different names*


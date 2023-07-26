# Comparing `tmp/deploymenthub-1.8.tar.gz` & `tmp/deploymenthub-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deploymenthub-1.8.tar", last modified: Tue Jul 25 06:42:18 2023, max compression
+gzip compressed data, was "deploymenthub-1.9.tar", last modified: Wed Jul 26 07:22:08 2023, max compression
```

## Comparing `deploymenthub-1.8.tar` & `deploymenthub-1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-25 06:42:18.127630 deploymenthub-1.8/
--rw-r--r--   0 jaredwines   (501) staff       (20)     1050 2023-07-25 04:40:15.000000 deploymenthub-1.8/LICENSE.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-25 06:42:18.127524 deploymenthub-1.8/PKG-INFO
--rw-r--r--   0 jaredwines   (501) staff       (20)      124 2023-07-25 04:40:15.000000 deploymenthub-1.8/README.md
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-25 06:42:18.126843 deploymenthub-1.8/bin/
--rw-r--r--   0 jaredwines   (501) staff       (20)     1183 2023-07-25 06:41:24.000000 deploymenthub-1.8/bin/deploymenthub
-drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-25 06:42:18.127350 deploymenthub-1.8/deploymenthub.egg-info/
--rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-25 06:42:18.000000 deploymenthub-1.8/deploymenthub.egg-info/PKG-INFO
--rw-r--r--   0 jaredwines   (501) staff       (20)      196 2023-07-25 06:42:18.000000 deploymenthub-1.8/deploymenthub.egg-info/SOURCES.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-25 06:42:18.000000 deploymenthub-1.8/deploymenthub.egg-info/dependency_links.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-25 06:42:18.000000 deploymenthub-1.8/deploymenthub.egg-info/top_level.txt
--rw-r--r--   0 jaredwines   (501) staff       (20)       38 2023-07-25 06:42:18.127670 deploymenthub-1.8/setup.cfg
--rw-r--r--   0 jaredwines   (501) staff       (20)      683 2023-07-25 06:41:24.000000 deploymenthub-1.8/setup.py
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-26 07:22:08.747251 deploymenthub-1.9/
+-rw-r--r--   0 jaredwines   (501) staff       (20)     1050 2023-07-25 04:40:15.000000 deploymenthub-1.9/LICENSE.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-26 07:22:08.747111 deploymenthub-1.9/PKG-INFO
+-rw-r--r--   0 jaredwines   (501) staff       (20)      124 2023-07-25 04:40:15.000000 deploymenthub-1.9/README.md
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-26 07:22:08.746334 deploymenthub-1.9/bin/
+-rw-r--r--   0 jaredwines   (501) staff       (20)     1203 2023-07-26 07:20:44.000000 deploymenthub-1.9/bin/deploymenthub
+drwxr-xr-x   0 jaredwines   (501) staff       (20)        0 2023-07-26 07:22:08.746856 deploymenthub-1.9/deploymenthub.egg-info/
+-rw-r--r--   0 jaredwines   (501) staff       (20)      433 2023-07-26 07:22:08.000000 deploymenthub-1.9/deploymenthub.egg-info/PKG-INFO
+-rw-r--r--   0 jaredwines   (501) staff       (20)      196 2023-07-26 07:22:08.000000 deploymenthub-1.9/deploymenthub.egg-info/SOURCES.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-26 07:22:08.000000 deploymenthub-1.9/deploymenthub.egg-info/dependency_links.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)        1 2023-07-26 07:22:08.000000 deploymenthub-1.9/deploymenthub.egg-info/top_level.txt
+-rw-r--r--   0 jaredwines   (501) staff       (20)       38 2023-07-26 07:22:08.747293 deploymenthub-1.9/setup.cfg
+-rw-r--r--   0 jaredwines   (501) staff       (20)      683 2023-07-26 07:21:56.000000 deploymenthub-1.9/setup.py
```

### Comparing `deploymenthub-1.8/LICENSE.txt` & `deploymenthub-1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deploymenthub-1.8/bin/deploymenthub` & `deploymenthub-1.9/bin/deploymenthub`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     args = parser.parse_args()
 
     project = args.project
     action = args.action
     branch = args.branch
     url = "http://192.168.0.216:5000"
 
-    list_of_projects = ['jaredwines', 'home-assistant', 'deployment-hub', 'alohamillworks', 'coastalteardrops', 'homebridge']
+    list_of_projects = ['jaredwines', 'home-assistant', 'deployment-hub', 'alohamillworks', 'coastalteardrops', 'homebridge','deployment-hub-ui']
 
     if project in list_of_projects:
         if branch is None:
             command = ('curl ' + url + '/' + project + '/' + action + '/')
         else:
             command = ('curl ' + url + '/' + project + '/' + action + '/' + branch + '/')
```

### Comparing `deploymenthub-1.8/setup.py` & `deploymenthub-1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="deploymenthub",
-    version=1.8,
+    version=1.9,
     description='A CLI client for deployment-hub server.',
     license='MIT',
     author='Jared Wines',
     author_email='contact@jaredwines.com',
     url='https://github.com/jaredwines/deployment-hub-cli-client',
     packages=find_packages(exclude=['tests']),
     scripts=['bin/deploymenthub'],
```


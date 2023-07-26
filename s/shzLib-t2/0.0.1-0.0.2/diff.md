# Comparing `tmp/shzLib_t2-0.0.1.tar.gz` & `tmp/shzLib_t2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shzLib_t2-0.0.1.tar", last modified: Wed Jul 26 16:04:48 2023, max compression
+gzip compressed data, was "shzLib_t2-0.0.2.tar", last modified: Wed Jul 26 16:06:54 2023, max compression
```

## Comparing `shzLib_t2-0.0.1.tar` & `shzLib_t2-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-26 16:04:48.612936 shzLib_t2-0.0.1/
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      271 2023-07-26 16:04:48.611880 shzLib_t2-0.0.1/PKG-INFO
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-26 15:52:48.000000 shzLib_t2-0.0.1/README.md
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       38 2023-07-26 16:04:48.613061 shzLib_t2-0.0.1/setup.cfg
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      543 2023-07-26 16:04:26.000000 shzLib_t2-0.0.1/setup.py
-drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-26 16:04:48.608836 shzLib_t2-0.0.1/shzLib_t2/
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-26 16:03:23.000000 shzLib_t2-0.0.1/shzLib_t2/__init__.py
-drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-26 16:04:48.611212 shzLib_t2-0.0.1/shzLib_t2.egg-info/
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      271 2023-07-26 16:04:48.000000 shzLib_t2-0.0.1/shzLib_t2.egg-info/PKG-INFO
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      204 2023-07-26 16:04:48.000000 shzLib_t2-0.0.1/shzLib_t2.egg-info/SOURCES.txt
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        1 2023-07-26 16:04:48.000000 shzLib_t2-0.0.1/shzLib_t2.egg-info/dependency_links.txt
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       28 2023-07-26 16:04:48.000000 shzLib_t2-0.0.1/shzLib_t2.egg-info/requires.txt
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       10 2023-07-26 16:04:48.000000 shzLib_t2-0.0.1/shzLib_t2.egg-info/top_level.txt
+drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-26 16:06:54.776846 shzLib_t2-0.0.2/
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      271 2023-07-26 16:06:54.776508 shzLib_t2-0.0.2/PKG-INFO
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-26 15:52:48.000000 shzLib_t2-0.0.2/README.md
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       38 2023-07-26 16:06:54.776951 shzLib_t2-0.0.2/setup.cfg
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      543 2023-07-26 16:06:45.000000 shzLib_t2-0.0.2/setup.py
+drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-26 16:06:54.775883 shzLib_t2-0.0.2/shzLib_t2.egg-info/
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      271 2023-07-26 16:06:54.000000 shzLib_t2-0.0.2/shzLib_t2.egg-info/PKG-INFO
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      182 2023-07-26 16:06:54.000000 shzLib_t2-0.0.2/shzLib_t2.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        1 2023-07-26 16:06:54.000000 shzLib_t2-0.0.2/shzLib_t2.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       28 2023-07-26 16:06:54.000000 shzLib_t2-0.0.2/shzLib_t2.egg-info/requires.txt
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       10 2023-07-26 16:06:54.000000 shzLib_t2-0.0.2/shzLib_t2.egg-info/top_level.txt
```

### Comparing `shzLib_t2-0.0.1/setup.py` & `shzLib_t2-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 project_name = 'shzLib_t2'
 
 setup(name=project_name,
-    version='0.0.1',
+    version='0.0.2',
     license='MIT License',
     author='Eliseu Brito',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='eliseubrito776@gmail.com',
     keywords='shz tools shzlib',
     description=u'Personal support tools in the development of varied projects',
```


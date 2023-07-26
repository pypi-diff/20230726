# Comparing `tmp/ai-supporter-0.0.2.tar.gz` & `tmp/ai-supporter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-supporter-0.0.2.tar", last modified: Wed Jun  7 03:15:14 2023, max compression
+gzip compressed data, was "ai-supporter-0.0.3.tar", last modified: Wed Jul 26 11:29:52 2023, max compression
```

## Comparing `ai-supporter-0.0.2.tar` & `ai-supporter-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 03:15:14.170587 ai-supporter-0.0.2/
--rw-r--r--   0 root         (0) root         (0)      338 2023-06-07 03:15:14.170587 ai-supporter-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       92 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 03:15:14.169587 ai-supporter-0.0.2/ai_supporter/
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/ai_supporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/ai_supporter/tts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 03:15:14.170587 ai-supporter-0.0.2/ai_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)      338 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/ai_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      277 2023-06-07 03:15:14.000000 ai-supporter-0.0.2/ai_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/ai_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/ai_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/ai_supporter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/ai_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 03:15:14.171587 ai-supporter-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      588 2023-06-07 03:15:13.000000 ai-supporter-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:29:52.884079 ai-supporter-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)      517 2023-07-26 11:29:52.884079 ai-supporter-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      271 2023-07-26 11:29:52.000000 ai-supporter-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:29:52.882079 ai-supporter-0.0.3/ai_supporter/
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-26 11:29:52.000000 ai-supporter-0.0.3/ai_supporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-07-26 11:29:52.000000 ai-supporter-0.0.3/ai_supporter/tts.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-26 11:29:52.000000 ai-supporter-0.0.3/ai_supporter/tts_old.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:29:52.884079 ai-supporter-0.0.3/ai_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      517 2023-07-26 11:29:52.000000 ai-supporter-0.0.3/ai_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      301 2023-07-26 11:29:52.000000 ai-supporter-0.0.3/ai_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 11:29:52.000000 ai-supporter-0.0.3/ai_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 11:29:52.000000 ai-supporter-0.0.3/ai_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-26 11:29:52.000000 ai-supporter-0.0.3/ai_supporter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-26 11:29:52.000000 ai-supporter-0.0.3/ai_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 11:29:52.884079 ai-supporter-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-26 11:29:52.000000 ai-supporter-0.0.3/setup.py
```

### Comparing `ai-supporter-0.0.2/ai_supporter/tts.py` & `ai-supporter-0.0.3/ai_supporter/tts_old.py`

 * *Files identical despite different names*

### Comparing `ai-supporter-0.0.2/setup.py` & `ai-supporter-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='ai-supporter',
-	version='0.0.2',
+	version='0.0.3',
 	description='Ai supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/ai-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```


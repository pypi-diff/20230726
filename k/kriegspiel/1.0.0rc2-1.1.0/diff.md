# Comparing `tmp/kriegspiel-1.0.0rc2.tar.gz` & `tmp/kriegspiel-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kriegspiel-1.0.0rc2.tar", last modified: Sun Dec 17 10:35:16 2017, max compression
+gzip compressed data, was "kriegspiel-1.1.0.tar", last modified: Wed Jul 26 03:20:06 2023, max compression
```

## Comparing `kriegspiel-1.0.0rc2.tar` & `kriegspiel-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxrwxr-x   0 olive     (1000) olive     (1000)        0 2017-12-17 10:35:16.000000 kriegspiel-1.0.0rc2/
--rw-rw-r--   0 olive     (1000) olive     (1000)     1821 2017-12-17 10:35:16.000000 kriegspiel-1.0.0rc2/PKG-INFO
-drwxrwxr-x   0 olive     (1000) olive     (1000)        0 2017-12-17 10:35:16.000000 kriegspiel-1.0.0rc2/kriegspiel.egg-info/
--rw-rw-r--   0 olive     (1000) olive     (1000)     1821 2017-12-17 10:35:16.000000 kriegspiel-1.0.0rc2/kriegspiel.egg-info/PKG-INFO
--rw-rw-r--   0 olive     (1000) olive     (1000)      252 2017-12-17 10:35:16.000000 kriegspiel-1.0.0rc2/kriegspiel.egg-info/SOURCES.txt
--rw-rw-r--   0 olive     (1000) olive     (1000)       28 2017-12-17 10:35:16.000000 kriegspiel-1.0.0rc2/kriegspiel.egg-info/requires.txt
--rw-rw-r--   0 olive     (1000) olive     (1000)       11 2017-12-17 10:35:16.000000 kriegspiel-1.0.0rc2/kriegspiel.egg-info/top_level.txt
--rw-rw-r--   0 olive     (1000) olive     (1000)        1 2017-12-17 10:35:16.000000 kriegspiel-1.0.0rc2/kriegspiel.egg-info/dependency_links.txt
--rw-rw-r--   0 olive     (1000) olive     (1000)      274 2017-12-17 10:35:16.000000 kriegspiel-1.0.0rc2/setup.cfg
-drwxrwxr-x   0 olive     (1000) olive     (1000)        0 2017-12-17 10:35:16.000000 kriegspiel-1.0.0rc2/kriegspiel/
--rw-rw-r--   0 olive     (1000) olive     (1000)     5687 2017-12-17 10:31:49.000000 kriegspiel-1.0.0rc2/kriegspiel/move.py
--rw-rw-r--   0 olive     (1000) olive     (1000)    11279 2017-12-17 10:31:49.000000 kriegspiel-1.0.0rc2/kriegspiel/berkeley.py
--rw-rw-r--   0 olive     (1000) olive     (1000)      124 2017-12-17 10:31:49.000000 kriegspiel-1.0.0rc2/kriegspiel/__init__.py
--rw-rw-r--   0 olive     (1000) olive     (1000)     3730 2017-12-17 10:34:25.000000 kriegspiel-1.0.0rc2/setup.py
+drwxr-xr-x   0 fil        (501) staff       (20)        0 2023-07-26 03:20:06.335423 kriegspiel-1.1.0/
+-rw-r--r--   0 fil        (501) staff       (20)     1067 2022-02-05 22:22:30.000000 kriegspiel-1.1.0/LICENSE
+-rw-r--r--   0 fil        (501) staff       (20)     1560 2023-07-26 03:20:06.335476 kriegspiel-1.1.0/PKG-INFO
+-rw-r--r--   0 fil        (501) staff       (20)      936 2023-07-23 17:01:30.000000 kriegspiel-1.1.0/README.md
+drwxr-xr-x   0 fil        (501) staff       (20)        0 2023-07-26 03:20:06.333923 kriegspiel-1.1.0/kriegspiel/
+-rw-r--r--   0 fil        (501) staff       (20)      121 2023-07-26 03:18:38.000000 kriegspiel-1.1.0/kriegspiel/__init__.py
+-rw-r--r--   0 fil        (501) staff       (20)    14642 2023-07-26 03:11:02.000000 kriegspiel-1.1.0/kriegspiel/berkeley.py
+-rw-r--r--   0 fil        (501) staff       (20)    10639 2023-07-26 03:11:02.000000 kriegspiel-1.1.0/kriegspiel/move.py
+drwxr-xr-x   0 fil        (501) staff       (20)        0 2023-07-26 03:20:06.334632 kriegspiel-1.1.0/kriegspiel.egg-info/
+-rw-r--r--   0 fil        (501) staff       (20)     1560 2023-07-26 03:20:06.000000 kriegspiel-1.1.0/kriegspiel.egg-info/PKG-INFO
+-rw-r--r--   0 fil        (501) staff       (20)      312 2023-07-26 03:20:06.000000 kriegspiel-1.1.0/kriegspiel.egg-info/SOURCES.txt
+-rw-r--r--   0 fil        (501) staff       (20)        1 2023-07-26 03:20:06.000000 kriegspiel-1.1.0/kriegspiel.egg-info/dependency_links.txt
+-rw-r--r--   0 fil        (501) staff       (20)       28 2023-07-26 03:20:06.000000 kriegspiel-1.1.0/kriegspiel.egg-info/requires.txt
+-rw-r--r--   0 fil        (501) staff       (20)       11 2023-07-26 03:20:06.000000 kriegspiel-1.1.0/kriegspiel.egg-info/top_level.txt
+-rw-r--r--   0 fil        (501) staff       (20)      253 2023-07-26 03:20:06.335680 kriegspiel-1.1.0/setup.cfg
+-rw-r--r--   0 fil        (501) staff       (20)     3730 2022-02-05 22:22:30.000000 kriegspiel-1.1.0/setup.py
+drwxr-xr-x   0 fil        (501) staff       (20)        0 2023-07-26 03:20:06.335202 kriegspiel-1.1.0/tests/
+-rw-r--r--   0 fil        (501) staff       (20)    36433 2023-07-26 03:10:24.000000 kriegspiel-1.1.0/tests/test_berkeley.py
+-rw-r--r--   0 fil        (501) staff       (20)     4854 2023-07-26 03:10:24.000000 kriegspiel-1.1.0/tests/test_move.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kriegspiel-1.0.0rc2/setup.py` & `kriegspiel-1.1.0/setup.py`

 * *Files identical despite different names*


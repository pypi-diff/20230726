# Comparing `tmp/mdformat_mkdocs-1.0.4rc1.tar.gz` & `tmp/mdformat_mkdocs-1.0.4rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdformat_mkdocs-1.0.4rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mdformat_mkdocs-1.0.4rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mdformat_mkdocs-1.0.4rc1.tar` & `mdformat_mkdocs-1.0.4rc2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1819 2023-04-06 01:58:46.525588 mdformat_mkdocs-1.0.4rc1/.gitignore
--rw-r--r--   0        0        0     1756 2023-06-27 11:21:14.928646 mdformat_mkdocs-1.0.4rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      571 2023-07-18 22:26:29.357397 mdformat_mkdocs-1.0.4rc1/.pre-commit-test.yaml
--rw-r--r--   0        0        0       33 2023-04-06 01:58:46.526052 mdformat_mkdocs-1.0.4rc1/.tool-versions
--rw-r--r--   0        0        0      979 2023-07-23 23:07:19.274542 mdformat_mkdocs-1.0.4rc1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1073 2023-04-06 01:58:46.526311 mdformat_mkdocs-1.0.4rc1/LICENSE
--rw-r--r--   0        0        0     3265 2023-07-23 23:07:19.381070 mdformat_mkdocs-1.0.4rc1/README.md
--rw-r--r--   0        0        0      175 2023-07-23 23:14:30.380833 mdformat_mkdocs-1.0.4rc1/mdformat_mkdocs/__init__.py
--rw-r--r--   0        0        0     3925 2023-07-23 23:03:42.317613 mdformat_mkdocs-1.0.4rc1/mdformat_mkdocs/plugin.py
--rw-r--r--   0        0        0      402 2023-07-23 23:07:19.385206 mdformat_mkdocs-1.0.4rc1/mkdocs-demo/README.md
--rw-r--r--   0        0        0     1030 2023-07-23 23:06:49.565898 mdformat_mkdocs-1.0.4rc1/mkdocs-demo/docs/README.md
--rw-r--r--   0        0        0    78687 2023-06-27 11:17:33.074820 mdformat_mkdocs-1.0.4rc1/mkdocs-demo/mkdcs-demo-screenshot.png
--rw-r--r--   0        0        0       42 2023-06-27 11:14:04.088218 mdformat_mkdocs-1.0.4rc1/mkdocs-demo/mkdocs.yml
--rw-r--r--   0        0        0        0 2023-06-27 11:10:00.809267 mdformat_mkdocs-1.0.4rc1/mkdocs-demo/mkdocs_demo/__init__.py
--rw-r--r--   0        0        0    24503 2023-06-27 11:08:15.516527 mdformat_mkdocs-1.0.4rc1/mkdocs-demo/poetry.lock
--rw-r--r--   0        0        0      372 2023-06-27 11:12:24.831270 mdformat_mkdocs-1.0.4rc1/mkdocs-demo/pyproject.toml
--rw-r--r--   0        0        0     1630 2023-06-27 23:43:24.286403 mdformat_mkdocs-1.0.4rc1/pyproject.toml
--rw-r--r--   0        0        0      789 2023-04-06 02:58:30.440638 mdformat_mkdocs-1.0.4rc1/tox.ini
--rw-r--r--   0        0        0     4688 1970-01-01 00:00:00.000000 mdformat_mkdocs-1.0.4rc1/PKG-INFO
+-rw-r--r--   0        0        0     1819 2023-04-06 01:58:46.525588 mdformat_mkdocs-1.0.4rc2/.gitignore
+-rw-r--r--   0        0        0     1756 2023-06-27 11:21:14.928646 mdformat_mkdocs-1.0.4rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      571 2023-07-23 23:55:55.891998 mdformat_mkdocs-1.0.4rc2/.pre-commit-test.yaml
+-rw-r--r--   0        0        0       33 2023-04-06 01:58:46.526052 mdformat_mkdocs-1.0.4rc2/.tool-versions
+-rw-r--r--   0        0        0     1104 2023-07-26 12:52:58.256221 mdformat_mkdocs-1.0.4rc2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1073 2023-04-06 01:58:46.526311 mdformat_mkdocs-1.0.4rc2/LICENSE
+-rw-r--r--   0        0        0     3265 2023-07-26 12:52:58.363552 mdformat_mkdocs-1.0.4rc2/README.md
+-rw-r--r--   0        0        0      175 2023-07-26 12:56:49.942453 mdformat_mkdocs-1.0.4rc2/mdformat_mkdocs/__init__.py
+-rw-r--r--   0        0        0     6305 2023-07-26 12:56:49.942938 mdformat_mkdocs-1.0.4rc2/mdformat_mkdocs/plugin.py
+-rw-r--r--   0        0        0      402 2023-07-26 12:52:58.367714 mdformat_mkdocs-1.0.4rc2/mkdocs-demo/README.md
+-rw-r--r--   0        0        0     1030 2023-07-26 12:52:45.343554 mdformat_mkdocs-1.0.4rc2/mkdocs-demo/docs/README.md
+-rw-r--r--   0        0        0    78687 2023-06-27 11:17:33.074820 mdformat_mkdocs-1.0.4rc2/mkdocs-demo/mkdcs-demo-screenshot.png
+-rw-r--r--   0        0        0       42 2023-06-27 11:14:04.088218 mdformat_mkdocs-1.0.4rc2/mkdocs-demo/mkdocs.yml
+-rw-r--r--   0        0        0        0 2023-06-27 11:10:00.809267 mdformat_mkdocs-1.0.4rc2/mkdocs-demo/mkdocs_demo/__init__.py
+-rw-r--r--   0        0        0    24503 2023-06-27 11:08:15.516527 mdformat_mkdocs-1.0.4rc2/mkdocs-demo/poetry.lock
+-rw-r--r--   0        0        0      372 2023-06-27 11:12:24.831270 mdformat_mkdocs-1.0.4rc2/mkdocs-demo/pyproject.toml
+-rw-r--r--   0        0        0     1630 2023-06-27 23:43:24.286403 mdformat_mkdocs-1.0.4rc2/pyproject.toml
+-rw-r--r--   0        0        0      789 2023-04-06 02:58:30.440638 mdformat_mkdocs-1.0.4rc2/tox.ini
+-rw-r--r--   0        0        0     4688 1970-01-01 00:00:00.000000 mdformat_mkdocs-1.0.4rc2/PKG-INFO
```

### Comparing `mdformat_mkdocs-1.0.4rc1/.gitignore` & `mdformat_mkdocs-1.0.4rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.4rc1/.pre-commit-config.yaml` & `mdformat_mkdocs-1.0.4rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.4rc1/.pre-commit-test.yaml` & `mdformat_mkdocs-1.0.4rc2/.pre-commit-test.yaml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.4rc1/LICENSE` & `mdformat_mkdocs-1.0.4rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.4rc1/README.md` & `mdformat_mkdocs-1.0.4rc2/README.md`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.4rc1/mkdocs-demo/docs/README.md` & `mdformat_mkdocs-1.0.4rc2/mkdocs-demo/docs/README.md`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.4rc1/mkdocs-demo/mkdcs-demo-screenshot.png` & `mdformat_mkdocs-1.0.4rc2/mkdocs-demo/mkdcs-demo-screenshot.png`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.4rc1/mkdocs-demo/poetry.lock` & `mdformat_mkdocs-1.0.4rc2/mkdocs-demo/poetry.lock`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.4rc1/pyproject.toml` & `mdformat_mkdocs-1.0.4rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.4rc1/tox.ini` & `mdformat_mkdocs-1.0.4rc2/tox.ini`

 * *Files identical despite different names*

### Comparing `mdformat_mkdocs-1.0.4rc1/PKG-INFO` & `mdformat_mkdocs-1.0.4rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdformat_mkdocs
-Version: 1.0.4rc1
+Version: 1.0.4rc2
 Summary: An mdformat plugin for mkdocs.
 Keywords: mdformat,markdown,markdown-it
 Author-email: Kyle King <dev.act.kyle@gmail.com>
 Requires-Python: >=3.7.2
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```


# Comparing `tmp/tvolib-0.2.0.tar.gz` & `tmp/tvolib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvolib-0.2.0.tar", max compression
+gzip compressed data, was "tvolib-0.2.1.tar", max compression
```

## Comparing `tvolib-0.2.0.tar` & `tvolib-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-07-21 18:31:00.565627 tvolib-0.2.0/LICENSE
--rw-r--r--   0        0        0      307 2023-07-25 22:43:23.561333 tvolib-0.2.0/README.md
--rw-r--r--   0        0        0      714 2023-07-25 23:50:05.041765 tvolib-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 17:26:07.254703 tvolib-0.2.0/src/tvolib/__init__.py
--rw-r--r--   0        0        0      219 2023-07-25 19:48:55.445686 tvolib-0.2.0/src/tvolib/mpl_utils/__init__.py
--rw-r--r--   0        0        0     2103 2023-07-25 19:51:46.873557 tvolib-0.2.0/src/tvolib/mpl_utils/_draw.py
--rw-r--r--   0        0        0      526 2023-07-25 19:42:33.293735 tvolib-0.2.0/src/tvolib/mpl_utils/_format.py
--rw-r--r--   0        0        0      898 2023-07-25 19:48:29.873412 tvolib-0.2.0/src/tvolib/mpl_utils/_setup.py
--rw-r--r--   0        0        0    25742 2023-07-21 17:47:40.083899 tvolib-0.2.0/src/tvolib/mpl_utils/data/mpl_utils.mplstyle
--rw-r--r--   0        0        0       83 2023-07-25 23:49:44.174619 tvolib-0.2.0/src/tvolib/numeric/__init__.py
--rw-r--r--   0        0        0     1718 2023-07-25 23:49:09.022374 tvolib-0.2.0/src/tvolib/numeric/interpolate.py
--rw-r--r--   0        0        0     1488 2023-07-25 22:45:58.568398 tvolib-0.2.0/src/tvolib/numeric/moving.py
--rw-r--r--   0        0        0      572 2023-07-25 23:04:48.648666 tvolib-0.2.0/src/tvolib/numeric/timing.py
--rw-r--r--   0        0        0     1201 1970-01-01 00:00:00.000000 tvolib-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-21 18:31:00.565627 tvolib-0.2.1/LICENSE
+-rw-r--r--   0        0        0      307 2023-07-25 22:43:23.561333 tvolib-0.2.1/README.md
+-rw-r--r--   0        0        0      714 2023-07-26 00:06:59.260664 tvolib-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-07-26 00:04:36.796710 tvolib-0.2.1/src/tvolib/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-25 19:48:55.445686 tvolib-0.2.1/src/tvolib/mpl_utils/__init__.py
+-rw-r--r--   0        0        0     2103 2023-07-25 19:51:46.873557 tvolib-0.2.1/src/tvolib/mpl_utils/_draw.py
+-rw-r--r--   0        0        0      526 2023-07-25 19:42:33.293735 tvolib-0.2.1/src/tvolib/mpl_utils/_format.py
+-rw-r--r--   0        0        0      898 2023-07-25 19:48:29.873412 tvolib-0.2.1/src/tvolib/mpl_utils/_setup.py
+-rw-r--r--   0        0        0    25742 2023-07-21 17:47:40.083899 tvolib-0.2.1/src/tvolib/mpl_utils/data/mpl_utils.mplstyle
+-rw-r--r--   0        0        0       83 2023-07-25 23:49:44.174619 tvolib-0.2.1/src/tvolib/numeric/__init__.py
+-rw-r--r--   0        0        0     1724 2023-07-26 00:06:32.551484 tvolib-0.2.1/src/tvolib/numeric/interpolate.py
+-rw-r--r--   0        0        0     1488 2023-07-25 22:45:58.568398 tvolib-0.2.1/src/tvolib/numeric/moving.py
+-rw-r--r--   0        0        0      572 2023-07-25 23:04:48.648666 tvolib-0.2.1/src/tvolib/numeric/timing.py
+-rw-r--r--   0        0        0     1201 1970-01-01 00:00:00.000000 tvolib-0.2.1/PKG-INFO
```

### Comparing `tvolib-0.2.0/LICENSE` & `tvolib-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tvolib-0.2.0/pyproject.toml` & `tvolib-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tvolib"
-version = "0.2.0"
+version = "0.2.1"
 description = "A personal collection of Python and IDL research tools in Space Plasma Physics."
 authors = ["Tien Vo <tien.a.vo@proton.me>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 packages = [
     { include = "tvolib", from = "src" }
 ]
```

### Comparing `tvolib-0.2.0/src/tvolib/mpl_utils/_draw.py` & `tvolib-0.2.1/src/tvolib/mpl_utils/_draw.py`

 * *Files identical despite different names*

### Comparing `tvolib-0.2.0/src/tvolib/mpl_utils/_format.py` & `tvolib-0.2.1/src/tvolib/mpl_utils/_format.py`

 * *Files identical despite different names*

### Comparing `tvolib-0.2.0/src/tvolib/mpl_utils/_setup.py` & `tvolib-0.2.1/src/tvolib/mpl_utils/_setup.py`

 * *Files identical despite different names*

### Comparing `tvolib-0.2.0/src/tvolib/mpl_utils/data/mpl_utils.mplstyle` & `tvolib-0.2.1/src/tvolib/mpl_utils/data/mpl_utils.mplstyle`

 * *Files identical despite different names*

### Comparing `tvolib-0.2.0/src/tvolib/numeric/interpolate.py` & `tvolib-0.2.1/src/tvolib/numeric/interpolate.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         yout = interp1d(x, yin, **interp_kw)(xout)
     elif len(y.shape) == 2:
         yout = np.empty((len(xout), N := y.shape[1]))
         for i in range(N):
             yin = (
                 move_avg(y[:, i], (w,), window=window)
                 if window is not None
-                else y
+                else y[:, i]
             )
             yout[:, i] = interp1d(x, yin, **interp_kw)(xout)
     else:
         raise NotImplementedError("Max dimensionality is 2.")
 
     if isinstance(y, u.Quantity):
         yout *= u.Unit(y.unit)
```

### Comparing `tvolib-0.2.0/src/tvolib/numeric/moving.py` & `tvolib-0.2.1/src/tvolib/numeric/moving.py`

 * *Files identical despite different names*

### Comparing `tvolib-0.2.0/src/tvolib/numeric/timing.py` & `tvolib-0.2.1/src/tvolib/numeric/timing.py`

 * *Files identical despite different names*

### Comparing `tvolib-0.2.0/PKG-INFO` & `tvolib-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvolib
-Version: 0.2.0
+Version: 0.2.1
 Summary: A personal collection of Python and IDL research tools in Space Plasma Physics.
 Home-page: https://github.com/tien-vo/tvolib
 License: GPL-3.0-or-later
 Author: Tien Vo
 Author-email: tien.a.vo@proton.me
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```


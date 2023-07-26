# Comparing `tmp/rastermap-0.9.0.tar.gz` & `tmp/rastermap-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastermap-0.9.0.tar", last modified: Sat Jul 15 12:01:36 2023, max compression
+gzip compressed data, was "rastermap-0.9.1.tar", last modified: Wed Jul 26 11:51:09 2023, max compression
```

## Comparing `rastermap-0.9.0.tar` & `rastermap-0.9.1.tar`

### file list

```diff
@@ -1,59 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:01:36.151928 rastermap-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:01:36.135928 rastermap-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:01:36.139928 rastermap-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-15 12:01:21.000000 rastermap-0.9.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-15 12:01:21.000000 rastermap-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-15 12:01:21.000000 rastermap-0.9.0/.style.yapf
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-15 12:01:21.000000 rastermap-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-15 12:01:36.151928 rastermap-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-07-15 12:01:21.000000 rastermap-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-15 12:01:21.000000 rastermap-0.9.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:01:36.143928 rastermap-0.9.0/paper/
--rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    21082 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig3.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig4.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig5.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig5.py
--rw-r--r--   0 runner    (1001) docker     (123)    12948 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/fig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/other_upsampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/qrdqn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-15 12:01:21.000000 rastermap-0.9.0/paper/splitting.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:01:36.147928 rastermap-0.9.0/rastermap/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:01:36.147928 rastermap-0.9.0/rastermap/gui/
--rw-r--r--   0 runner    (1001) docker     (123)   118393 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/gui/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)    27413 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/gui/guiparts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16916 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/gui/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/gui/menus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/gui/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/gui/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/rastermap.py
--rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-15 12:01:21.000000 rastermap-0.9.0/rastermap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:01:36.147928 rastermap-0.9.0/rastermap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-15 12:01:36.000000 rastermap-0.9.0/rastermap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-15 12:01:36.000000 rastermap-0.9.0/rastermap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:01:36.000000 rastermap-0.9.0/rastermap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-15 12:01:36.000000 rastermap-0.9.0/rastermap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-15 12:01:36.000000 rastermap-0.9.0/rastermap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 12:01:36.151928 rastermap-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-15 12:01:21.000000 rastermap-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:01:36.151928 rastermap-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-15 12:01:21.000000 rastermap-0.9.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-15 12:01:21.000000 rastermap-0.9.0/tests/test_rastermap.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-15 12:01:21.000000 rastermap-0.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.039098 rastermap-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.027097 rastermap-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.031097 rastermap-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-26 11:50:54.000000 rastermap-0.9.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-26 11:50:54.000000 rastermap-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 11:50:54.000000 rastermap-0.9.1/.style.yapf
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-26 11:50:54.000000 rastermap-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-07-26 11:51:09.039098 rastermap-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15587 2023-07-26 11:50:54.000000 rastermap-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-26 11:50:54.000000 rastermap-0.9.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.031097 rastermap-0.9.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-26 11:50:54.000000 rastermap-0.9.1/notebooks/rastermap_largescale.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-07-26 11:50:54.000000 rastermap-0.9.1/notebooks/rastermap_singleneurons.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-07-26 11:50:54.000000 rastermap-0.9.1/notebooks/rastermap_widefield.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-07-26 11:50:54.000000 rastermap-0.9.1/notebooks/rastermap_zebrafish.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    27163 2023-07-26 11:50:54.000000 rastermap-0.9.1/notebooks/tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.035097 rastermap-0.9.1/paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21793 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig3.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/fig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/other_upsampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/qrdqn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17359 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-07-26 11:50:54.000000 rastermap-0.9.1/paper/splitting.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.035097 rastermap-0.9.1/rastermap/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.035097 rastermap-0.9.1/rastermap/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)   118393 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/gui/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27515 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/gui/guiparts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/gui/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/gui/menus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/gui/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/gui/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21955 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/rastermap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-07-26 11:50:54.000000 rastermap-0.9.1/rastermap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.035097 rastermap-0.9.1/rastermap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-07-26 11:51:08.000000 rastermap-0.9.1/rastermap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-26 11:51:08.000000 rastermap-0.9.1/rastermap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:51:08.000000 rastermap-0.9.1/rastermap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-26 11:51:08.000000 rastermap-0.9.1/rastermap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 11:51:08.000000 rastermap-0.9.1/rastermap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 11:51:09.039098 rastermap-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-26 11:50:54.000000 rastermap-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:51:09.039098 rastermap-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 11:50:54.000000 rastermap-0.9.1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-26 11:50:54.000000 rastermap-0.9.1/tests/test_rastermap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-26 11:50:54.000000 rastermap-0.9.1/tox.ini
```

### Comparing `rastermap-0.9.0/.github/workflows/test_and_deploy.yml` & `rastermap-0.9.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/.gitignore` & `rastermap-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/LICENSE` & `rastermap-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/conftest.py` & `rastermap-0.9.1/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     finally:
         f.close()
         if os.path.exists(f.name):
             os.remove(f.name)
 
 @pytest.fixture()
 def test_file():
-    ddir = Path.home().joinpath('.neuropop')
+    ddir = Path.home().joinpath('.rastermap')
     ddir.mkdir(exist_ok=True)
     data_dir = ddir.joinpath('data')
     data_dir.mkdir(exist_ok=True)
     url = "http://www.suite2p.org/static/test_data/neuropop_test_data.npz"
     test_file = str(data_dir.joinpath("neuropop_test_data.npz"))
     if not os.path.exists(test_file):
         download_url_to_file(url, test_file)
```

### Comparing `rastermap-0.9.0/paper/fig1.ipynb` & `rastermap-0.9.1/paper/fig1.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998845464571271%*

 * *Differences: {"'cells'": "{9: {'source': {insert: [(12, '                    time_lag_window=10, "*

 * *            "time_bin=10).fit(spks)   \\n')], delete: [12]}}, 10: {'source': {insert: [(13, "*

 * *            "'                    time_lag_window=10, time_bin=10).fit(spks)   \\n')], delete: "*

 * *            '[13]}}}'}*

```diff
@@ -118,15 +118,15 @@
                 "scores_all = np.zeros((10, 2, 8, 5))\n",
                 "for random_state in range(10):\n",
                 "    print(random_state)\n",
                 "    dat = np.load(os.path.join(root, \"simulations\", f\"sim_{random_state}.npz\"), allow_pickle=True)\n",
                 "    spks = dat[\"spks\"]\n",
                 "    # run rastermap to get PCs\n",
                 "    model = Rastermap(n_clusters=100, n_PCs=200, locality=0.8,\n",
-                "                    time_lag_window=10, time_bin=10).fit(spks, normalize=True, mean_time=True)   \n",
+                "                    time_lag_window=10, time_bin=10).fit(spks)   \n",
                 "    perplexities = []\n",
                 "    j = 0\n",
                 "    for perplexity in [10,30,60,100,200]:\n",
                 "        M = metrics.run_TSNE(model.Usv, perplexities=[perplexity])\n",
                 "        embs_all[random_state, j] = M\n",
                 "        j += 1\n",
                 "        perplexities.append([perplexity, 0])\n",
@@ -162,15 +162,15 @@
                 "scores_all = np.zeros((10, 2, 7, 5))\n",
                 "for random_state in range(10):\n",
                 "    print(random_state)\n",
                 "    dat = np.load(os.path.join(root, \"simulations\", f\"sim_{random_state}.npz\"), allow_pickle=True)\n",
                 "    spks = dat[\"spks\"]\n",
                 "    # run rastermap to get PCs\n",
                 "    model = Rastermap(n_clusters=100, n_PCs=200, locality=0.8,\n",
-                "                    time_lag_window=10, time_bin=10).fit(spks, normalize=True, mean_time=True)   \n",
+                "                    time_lag_window=10, time_bin=10).fit(spks)   \n",
                 "    j = 0\n",
                 "    for nneigh in n_neighbors:\n",
                 "        M = metrics.run_UMAP(model.Usv, n_neighbors=nneigh)\n",
                 "        embs_all[random_state, j] = M\n",
                 "        j += 1\n",
                 "        print(j)\n",
                 "    contamination_scores, triplet_scores = metrics.benchmarks(dat[\"xi_all\"], embs_all[random_state])\n",
```

### Comparing `rastermap-0.9.0/paper/fig1.py` & `rastermap-0.9.1/paper/fig1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
 """
 import matplotlib.pyplot as plt 
 import os
 import numpy as np
 from rastermap.utils import bin1d
+from rastermap.sort import compute_BBt, compute_BBt_mask
 import metrics
 from fig_utils import *
 
 alg_cols = plt.get_cmap("tab20b")(np.linspace(0,1.,20))[::4]
 alg_cols = alg_cols[[1,0,2,3]]
 alg_cols = np.concatenate((np.array([0,0,0,1])[np.newaxis,:],
                            alg_cols), axis=0)
@@ -34,15 +35,15 @@
 
     # plot kmeans illustration
     ax_kmeans_img.imshow(kmeans_img)
     ax_kmeans_img.set_title("k-means\nclustering")
     ax_kmeans_img.axis("off")
 
     # plot example crosscorr
-    c0, c1 = 1, 4
+    c0, c1 = 5, 7
     ax_crosscorr.plot(tshifts, cc_tdelay[c0,c1], color=[0.5,0.5,0.5], zorder=1)
     ax_crosscorr.set_ylabel("corr")
     ax_crosscorr.set_xlabel("time lag ($\delta$t)")
     ax_crosscorr.set_xlim([tshifts.min(), tshifts.max()])
     ax_crosscorr.set_title(f"cross-corr\nclusters {c0}, {c1}")
     ix = cc_tdelay[c0,c1].argmax()
     ax_crosscorr.scatter(tshifts[ix], cc_tdelay[c0,c1,ix], marker="*", lw=0.5, color=[1,0.5,0], s=40, zorder=2)
@@ -79,52 +80,66 @@
             axi.text(0.5,-0.15,"clusters", transform=axi.transAxes, ha="center")
 
     ax = plt.subplot(grid[0,2])
     il = plot_label(ltr, il, ax, transl, fs_title)
     ax.set_title("matching matrix")
     ax.axis("off")
     pos = ax.get_position().bounds
+    xi = np.arange(0, nshow, 1, "float32") / nshow
+    BBt_log = compute_BBt(xi, xi)
+    BBt_log = np.triu(BBt_log)
+    BBt_log /= BBt_log.sum()
+    BBt_travel = compute_BBt_mask(xi, xi)
+    BBt_travel = np.triu(BBt_travel)
+    BBt_travel /= BBt_travel.sum() 
+    vmax = 2e-2
     for i,mat in enumerate([BBt_log, BBt_travel]):
-        axi = fig.add_axes([pos[0]-dx*0.05+i*dx*1, 
-                                    pos[1]+pos[3]*0.3-i*dy*0.3, pos[2]*0.5, pos[3]*0.5])
-        axi.imshow(mat[:nshow,:nshow], vmin=-6, vmax=6, cmap="RdBu_r")
+        axi = fig.add_axes([pos[0]+dx*0.2+i*dx*1, 
+                            pos[1]+pos[3]*0.3, pos[2]*0.5, pos[3]*0.5])
+        axi.imshow(mat[:nshow,:nshow], vmin=-vmax, vmax=vmax, cmap="RdBu_r")
         axi.set_yticks([])
         axi.set_xticks([])
         axi.spines["right"].set_visible(True)
         axi.spines["top"].set_visible(True)
-        axi.set_title(["global", "traveling\nsalesman"][i])
+        axi.set_title(["global", "local"][i])
         if i==0:
-            axi.text(1.2,0.25, "+",transform=axi.transAxes, fontsize=default_font+4)
+            axi.text(1.07,0.5, "+",transform=axi.transAxes, fontsize=default_font+6)
+            axi.text(1.3,0.5, "w",transform=axi.transAxes, fontsize=default_font+2)
+            axi.text(-0.05,0.5, "(1-w)",transform=axi.transAxes, 
+                        fontsize=default_font+2, ha="right")
+        else:
+            axi.text(1.2,0.4, "=",transform=axi.transAxes, fontsize=default_font+6)
 
     ax = plt.subplot(grid[0,3])
-    il = plot_label(ltr, il, ax, transl, fs_title)
-    nn = cc_tdelay.shape[0]
-    cc_tdelay[np.arange(0, nn), np.arange(0, nn)] = 1
-    im=ax.imshow(cc_tdelay[c0:c0+nshow,c0:c0+nshow,10:].max(axis=-1), vmin=-1, vmax=1, cmap="RdBu_r")
-    ax.set_title("asymmetric similarity")
+    pos = ax.get_position().bounds
+    ax.set_position([pos[0]+dx*0.2, pos[1]+pos[3]*0.3, pos[2]*0.5, pos[3]*0.5])
+    im = ax.imshow(BBt_log[:nshow, :nshow]/2 + BBt_travel[:nshow, :nshow]/2, 
+                    vmin=-vmax, vmax=vmax, cmap="RdBu_r")
     ax.set_yticks([])
     ax.set_xticks([])
     ax.spines["right"].set_visible(True)
     ax.spines["top"].set_visible(True)
     posi = ax.get_position().bounds
     #divider = make_axes_locatable(ax)
-    cax = fig.add_axes([posi[0]+posi[2]*1.02, posi[1]+posi[3]*0.75, posi[2]*0.05, posi[3]*0.25])
+    cax = fig.add_axes([posi[0]+posi[2]*1.1, posi[1]+posi[3]*0.6, posi[2]*0.07, posi[3]*0.4])
     plt.colorbar(im, cax)
 
     ax = plt.subplot(grid[0,4])
     il = plot_label(ltr, il, ax, transl, fs_title)
     for i in range(3):
         nshow=20
         du = 0.4
         p = ax.plot(np.linspace(0, len(U_upsampled[c0:c0+nshow*10,i]), 
                                             len(U_nodes[c0:c0+nshow+1,i])), 
-                            U_nodes[c0:c0+nshow+1,i] + du*(2-i), "x", markersize=6, 
+                            U_nodes[c0:c0+nshow+1,i] + du*(2-i) + (i==2)*0.08, "x", 
+                            markersize=6, 
                             color=np.ones(3)*(0.25*i),
                             lw=4)
-        ax.plot(U_upsampled[c0*10:(c0+nshow)*10,i] + du*(2-i), color=p[0].get_color(), lw=1)
+        ax.plot(U_upsampled[c0*10:(c0+nshow)*10,i] + du*(2-i) + (i==2)*0.08, 
+                color=p[0].get_color(), lw=1)
         ax.text(20*10, du*(2-i) + du*0.05 + U_nodes[c0:c0+nshow,i].max(), f"PC {i+1:d}", 
                          color=p[0].get_color(), ha="right")
     ax.set_ylim([-du*0.8,du*2.4])
     ax.axis("off")
     ax.text(0,0.1, "clusters sorted x", transform=ax.transAxes)
     ax.text(0,0., "upsampled nodes -", transform=ax.transAxes)
     ax.text(-0.1,0.5, "weights", rotation=90, transform=ax.transAxes, va="center")
@@ -313,14 +328,15 @@
                     color=alg_cols[k], zorder=0 if k>0 else 5)
     ax.plot(100 * np.array([5./6, 5./6, 5./6, 5./6, 2./3]), color="k", linestyle="--")
     ax.text(0, 85, "chance")
     ax.set_ylabel("% contamination")
     ax.set_xticks(np.arange(0, 5))
     ax.set_xticklabels(mod_names, 
                         rotation=30, ha="right", rotation_mode="anchor")
+    ax.set_ylim([0, 85])
     return il
 
 def _fig1(kmeans_img, xi_all, cc_tdelay, tshifts, BBt_log, BBt_travel, 
         seqcurves0, seqcurves1, tcurves, xresp, 
         U_nodes, U_upsampled, X_embs, cc_embs,cc_embs_max,
         csig, scores_all, embs_all):
     
@@ -424,14 +440,15 @@
     #il = plot_label(ltr, il, ax, transl, fs_title)
     for k in range(len(cs)-1):
         ax.errorbar(np.arange(5), cs[k], cs_sem[k], lw=2, 
                     color=cols[k]   , zorder=0 if k>0 else 5)
     ax.plot(100 * np.array([5./6, 5./6, 5./6, 5./6, 2./3]), color="k", linestyle="--")
     ax.text(0, 85, "chance")
     ax.set_ylabel("% contamination")
+    ax.set_ylim([0, 85])
     ax.set_xticks(np.arange(0, 5))
     ax.set_xticklabels(mod_names, 
                         rotation=30, ha="right", rotation_mode="anchor")
     return il
         
 def suppfig_scores(root, save_figure=True):
     tsne_cols = plt.get_cmap("Greens")(np.linspace(0.4,1,8))
```

### Comparing `rastermap-0.9.0/paper/fig2.ipynb` & `rastermap-0.9.1/paper/fig2.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9718055555555556%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(27, '                    ).fit(spks)\\n'), (31, '### bin "*

 * *            "full data into superneurons\\n'), (33, 'sn = zscore(utils.bin1d(spks[isort], nbin, "*

 * *            "axis=0), axis=1)\\n'), (34, 'np.random.seed(0)\\n'), (35, 'sn_rand = "*

 * *            'zscore(utils.bin1d(spks[np.random.permutation(spks.shape[0])], nbin, axis=0), '*

 * *            "axis=1)\\n'), (36, '\\n'), (37, '# sort in time\\n'), (38, 'model2 = "*

 * *            "Rastermap(n_clusters=100, locality=0.,\\n' […]*

```diff
@@ -81,29 +81,35 @@
                 "\n",
                 "    y_pred_all, ve_all, itest = pred_model.train_model(beh, Vfit, tcam, tneural, delay=-1,\n",
                 "                                                        learning_rate=1e-3, n_iter=400,\n",
                 "                                                    device=device, verbose=True)\n",
                 "    if i==1:\n",
                 "        y_pred_nn = y_pred_all.copy()\n",
                 "\n",
-                "\n",
                 "### run rastermap\n",
                 "model = Rastermap(n_clusters=100, \n",
                 "                    n_PCs=128, \n",
                 "                    locality=0.75,\n",
                 "                    time_lag_window=5,\n",
-                "                    symmetric=False,\n",
-                "                    grid_upsample=10,\n",
-                "                    time_bin=1,\n",
-                "                    bin_size=0).fit(spks, normalize=True, mean_time=True)\n",
+                "                    ).fit(spks)\n",
                 "cc_nodes = model.cc.copy()\n",
                 "isort = model.isort\n",
                 "\n",
-                "### sort and bin data and prediction into superneurons\n",
+                "### bin full data into superneurons\n",
                 "nbin = 200\n",
+                "sn = zscore(utils.bin1d(spks[isort], nbin, axis=0), axis=1)\n",
+                "np.random.seed(0)\n",
+                "sn_rand = zscore(utils.bin1d(spks[np.random.permutation(spks.shape[0])], nbin, axis=0), axis=1)\n",
+                "\n",
+                "# sort in time\n",
+                "model2 = Rastermap(n_clusters=100, locality=0.,\n",
+                "                    n_PCs=128).fit(sn.T)\n",
+                "isort2 = model2.isort\n",
+                "\n",
+                "### bin test data and prediction into superneurons\n",
                 "sn_test = utils.bin1d(spks[isort][:,itest.flatten()], nbin, axis=0)\n",
                 "sn_pred_test = utils.bin1d(U[isort] @ y_pred_nn.T, nbin, axis=0)\n",
                 "sn_pred_test -= sn_test.mean(axis=1, keepdims=True)\n",
                 "sn_pred_test /= sn_test.std(axis=1, keepdims=True)\n",
                 "sn_test = zscore(sn_test, axis=1)\n",
                 "cc_pred = (sn_test * zscore(sn_pred_test, axis=1)).mean(axis=1)\n",
                 "# sort and bin PCs for maxstim estimation\n",
@@ -116,21 +122,23 @@
                 "ms_model = nn_prediction.MaxStimModel(pred_model)\n",
                 "ms_model.requires_grad = False\n",
                 "u = torch.from_numpy(U_sn).to(device)\n",
                 "u.requires_grad = False\n",
                 "xr = ms_model.train_batch(u, n_iter=200, learning_rate=1e-2)\n",
                 "rfs = xr.detach().cpu().numpy()\n",
                 "\n",
+                "\n",
                 "# save results\n",
                 "np.savez(os.path.join(root, \"results\", \"spont_proc.npz\"), sn_test=sn_test, \n",
-                "            sn_pred_test=sn_pred_test, itest=itest,\n",
+                "            sn_pred_test=sn_pred_test, itest=itest, \n",
+                "            sn=sn, sn_rand=sn_rand, isort2=isort2,\n",
                 "            rfs=rfs, isort=isort, cc_nodes=cc_nodes,\n",
                 "            xpos=xpos, ypos=ypos,\n",
                 "            tcam=tcam, tneural=tneural, \n",
-                "            run=run, beh=beh, beh_names=beh_names)"
+                "            run=run, beh=beh, beh_names=beh_names)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### make figure"
@@ -143,14 +151,30 @@
             "outputs": [],
             "source": [
                 "# root path has folder \"results\" with saved results\n",
                 "# will save figures to \"figures\" folder\n",
                 "os.makedirs(os.path.join(root, \"figures/\"), exist_ok=True)\n",
                 "fig2.fig2(root, save_figure=True)"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### make supp fig "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "fig2.suppfig_random(root, save_figure=True)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3.9.16 ('rastermap')",
             "language": "python",
             "name": "python3"
```

### Comparing `rastermap-0.9.0/paper/fig2.py` & `rastermap-0.9.1/paper/fig2.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 import matplotlib.pyplot as plt 
 from matplotlib import patches
 import os
 import numpy as np
 from fig_utils import *
 
-
 def panel_neuron_pos(fig, grid1, il, yratio, xpos0, ypos0, isort, brain_img):
     xpos, ypos = xpos0.copy(), -1*ypos0.copy()
     ylim = np.array([ypos.min(), ypos.max()])
     xlim = np.array([xpos.min(), xpos.max()])
     ylr = np.diff(ylim)[0] / np.diff(xlim)[0]
     
     ax = fig.add_subplot(grid1[:1])
@@ -137,15 +136,15 @@
         ax.set_ylim([0,1.2])
         ax.spines["left"].set_visible(False)
         ax.set_yticks([])
         ax.set_xticks([])
         transl = mtransforms.ScaledTranslation(-15 / 72, 12 / 72, fig.dpi_scale_trans)
         il = plot_label(ltr, il, ax, transl, fs_title)
         if k==0:
-            il+=1
+            il+=2
 
         if k==0:
             ax.text(0.75,0.8,"running speed", transform=ax.transAxes, color=kp_colors[0])
         ax.text(0,1.5,titles[k], transform=ax.transAxes, fontsize="large")
         
         # spk raster
         ax = fig.add_axes([pos[0]+0.02*(k==0), pos[1], pos[2], pos[3]*yh])     
@@ -153,16 +152,17 @@
             ax0 = ax
         xw = pos[2]*0.1
         if k==0:
             cax = fig.add_axes([pos[0]+0.02, pos[1]-pos[3]*0.005, xw, pos[3]*0.01])
         else: 
             cax = None
         plot_raster(ax, sn_test if k==0 else sn_pred_test, 
-                    xmin=xmin, xmax=xmax, vmax=1.5, fs=3.38, label=k==1, 
-                    padding=padding, cax=cax, label_pos="right")    
+                    xmin=xmin, xmax=xmax, vmax=1.5, fs=3.38, 
+                    nper=200, n_neurons=5000, label=k==1, 
+                    padding=padding, padding_x=0.01, cax=cax, label_pos="right")    
         if k==0:
             cax = fig.add_axes([pos[0]+0.02-pos[2]*0.02, pos[1], pos[2]*0.01, pos[3]*yh])
             nn = sn_test.shape[0]
             cols = cmap_emb(np.linspace(0, 1, nn))
             cax.imshow(cols[:,np.newaxis], aspect="auto")
             cax.set_ylim([0, (1+padding)*nn])
             cax.invert_yaxis()
@@ -173,15 +173,16 @@
                 xy0 = (0,ir)
                 xy1 = (xr,ir)
                 con = patches.ConnectionPatch(xyA=xy0, xyB=xy1, coordsA="data", coordsB="data",
                                     axesA=ax0, axesB=ax, color=.5*np.ones(3), lw=0.5)
                 ax.add_artist(con)
     return il
             
-def _fig2(brain_img, face_img, xpos, ypos, isort, cc_nodes,
+def _fig2(brain_img, face_img, xpos, ypos, isort, 
+            isort2, sn, cc_nodes, sn_rand,
             beh, beh_names, tcam, tneural, 
             itest, rfs, run, sn_test, sn_pred_test):
     fig = plt.figure(figsize=(14,7))
     yratio = 14 / 7
     grid = plt.GridSpec(1,9, figure=fig, left=0.02, right=0.98, top=0.94, bottom=0.07, 
                         wspace = 0.35, hspace = 0.3)
 
@@ -198,24 +199,24 @@
     ax = fig.add_subplot(grid[0])
     ax.axis("off")
     grid1 = matplotlib.gridspec.GridSpecFromSubplotSpec(3,1, subplot_spec=ax, 
                                                         wspace=0.2, hspace=0.5)
     ax.remove()
     il = 0
 
-    il+=1
+    il+=2
     il = panels_beh_traces(grid1, il, face_img, beh, beh_names, tcam, tneural, itest, xmin, xmax)
 
-    il-=2
+    il-=3
     il = panel_neuron_pos(fig, grid1, il, yratio, xpos, ypos, isort, brain_img)
     
     il+=2
     il = panels_rfs(grid, il, yh, padding, ipl, rfs, beh_names)
         
-    il-=2
+    il-=3
     il = panels_rasters(fig, grid, il, yh, padding, ipl, sn_test, sn_pred_test, 
                         run, itest, xmin, xmax)
     return fig
 
 def fig2(root, save_figure=True):
     d = np.load(os.path.join(root, "results", "spont_proc.npz"), allow_pickle=True) 
     try:
@@ -228,8 +229,68 @@
     fig = _fig2(brain_img, face_img, **d);
     if save_figure:
         fig.savefig(os.path.join(root, "figures", "fig2.pdf"), dpi=200)
 
             
 
 
+def suppfig_random(root, save_figure=True):
+    d = np.load(os.path.join(root, "results", "spont_proc.npz"), allow_pickle=True) 
+    sn = d["sn"]
+    sn_rand = d["sn_rand"]
+    run = d["run"]
+    itest = d["itest"]
+
+    fig = plt.figure(figsize=(14*0.75,8*0.75))
+
+    grid = plt.GridSpec(1,2, figure=fig, left=0.02, right=0.99, top=0.9, bottom=0.13, 
+                        wspace = 0.15, hspace = 0.3)
+    il = 0
+
+    titles = ["random sorting", 
+            "Rastermap sorting"]
+
+    xmin = 185 
+    xmax = xmin+500
+    padding = 0.015
+    yh = 0.94 # fraction raster vs run
+    xr = xmax - xmin
+
+    for k in range(2):
+        ax = plt.subplot(grid[k])
+        pos = ax.get_position().bounds
+        ax.axis("off")
+        ax.remove()
+
+        # run raster
+        ax = fig.add_axes([pos[0]+0.02*(k==0), pos[1]+pos[3]*(yh+0.01), pos[2], pos[3]*(1-yh-0.01)])     
+        ax.fill_between(np.arange(0, xr), run[itest.flatten()][xmin:xmax], 
+                        color=kp_colors[0])
+        ax.set_xlim([0, 1.008*xr])
+        ax.set_ylim([0,1.2])
+        ax.spines["left"].set_visible(False)
+        ax.set_yticks([])
+        ax.set_xticks([])
+        transl = mtransforms.ScaledTranslation(-15 / 72, 12 / 72, fig.dpi_scale_trans)
+        il = plot_label(ltr, il, ax, transl, fs_title)
+        
+        if k==0:
+            ax.text(0.75,0.8,"running speed", transform=ax.transAxes, color=kp_colors[0])
+        ax.text(0,1.5,titles[k], transform=ax.transAxes, fontsize="large")
+        
+        # spk raster
+        ax = fig.add_axes([pos[0]+0.02*(k==0), pos[1], pos[2], pos[3]*yh])     
+        if k==0:
+            ax0 = ax
+        xw = pos[2]*0.1
+        if k==0:
+            cax = fig.add_axes([pos[0]+0.02, pos[1]-pos[3]*0.005, xw, pos[3]*0.01])
+        else: 
+            cax = None
+        plot_raster(ax, sn_rand[:,itest.flatten()] if k==0 else sn[:, itest.flatten()], 
+                    xmin=xmin, xmax=xmax, vmax=1.5, fs=3.38, label=k==0, 
+                    nper=200, n_neurons=5000,
+                    padding=padding, padding_x=0.01, cax=cax, label_pos="right")    
 
+    
+    if save_figure:
+        fig.savefig(os.path.join(root, "figures", "suppfig_random.pdf"))
```

### Comparing `rastermap-0.9.0/paper/fig3.ipynb` & `rastermap-0.9.1/paper/fig3.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992763157894737%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(1, '                    time_lag_window=10, "*

 * *            "locality=0.75).fit(spks)\\n'), (7, '\\n'), (8, '# sort in time\\n'), (9, 'model2 = "*

 * *            "Rastermap(n_clusters=100, n_splits=0, locality=0.,\\n'), (10, "*

 * *            "'                             n_PCs=200).fit(sn.T)\\n'), (11, 'isort2 = "*

 * *            "model2.isort\\n'), (14, '         sn=sn, xpos=xpos, ypos=ypos, isort=isort, "*

 * *            "isort2=isort2,\\n'), (15, '        cc_nodes=cc_nodes, "*

 * *      […]*

```diff
@@ -56,24 +56,29 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "model = Rastermap(n_clusters=100, n_PCs=200, \n",
-                "                    time_lag_window=10, locality=0.8).fit(spks)\n",
+                "                    time_lag_window=10, locality=0.75).fit(spks)\n",
                 "isort = model.isort \n",
                 "cc_nodes = model.cc\n",
                 "bin_size = 100\n",
                 "sn = zscore(utils.bin1d(spks[isort], bin_size, axis=0), axis=1)\n",
                 "corridor_tuning = tuning_curves_VR(sn, corridor[\"VRpos\"], corridor[\"corridor_starts\"])\n",
                 "\n",
+                "# sort in time\n",
+                "model2 = Rastermap(n_clusters=100, n_splits=0, locality=0.,\n",
+                "                             n_PCs=200).fit(sn.T)\n",
+                "isort2 = model2.isort\n",
+                "\n",
                 "np.savez(os.path.join(root, \"results\", \"corridor_proc.npz\"),\n",
-                "         sn=sn, xpos=xpos, ypos=ypos, isort=isort, cc_nodes=cc_nodes,\n",
-                "         corridor_tuning=corridor_tuning)"
+                "         sn=sn, xpos=xpos, ypos=ypos, isort=isort, isort2=isort2,\n",
+                "        cc_nodes=cc_nodes, corridor_tuning=corridor_tuning)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### make figure"
```

### Comparing `rastermap-0.9.0/paper/fig3.py` & `rastermap-0.9.1/paper/fig3.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
     il = plot_label(ltr, il, ax, transl, fs_title)
     
     cax = grid.figure.add_axes([poss[0]+poss[2]*1.02, poss[1]+poss[3]*0.75, 
                         poss[2]*0.03, poss[3]*0.25])
     plt.colorbar(im, cax)
     return il
 
-def _fig3(brain_img, sn, xpos, ypos, isort, cc_nodes,
+def _fig3(brain_img, sn, xpos, ypos, isort, isort2, cc_nodes,
          corridor_starts, corridor_widths, 
          corridor_tuning, corridor_imgs, VRpos,
          reward_inds, sound_inds, lick_inds, run):
     fig = plt.figure(figsize=(14,7))
     yratio = 14 / 7
     grid = plt.GridSpec(3,5, figure=fig, left=0.02, right=0.98, top=0.98, bottom=0.02, 
                         wspace = 0.3, hspace = 0.15)
@@ -195,16 +195,16 @@
 
     il = panel_cc(grid, il, yratio, cc_nodes)
     
     ax = plt.subplot(grid[:,1:])
     pos = ax.get_position().bounds
     ax.remove()
 
-    xmin = 1000
-    xmax=xmin+500
+    xmin = 1410
+    xmax=xmin+520
 
     nn = sn.shape[0]
     xr = xmax - xmin
     y0 = pos[1]
     x0 = pos[0]
     padding=0.025
     dye = 0.06
@@ -236,15 +236,15 @@
     
     il = panels_tuning(axs, il, padding, corridor_tuning)
 
     return fig
 
 
 def fig3(root, save_figure=True):
-    d = np.load(os.path.join(root, "results", "corridor_proc2.npz"), allow_pickle=True) 
+    d = np.load(os.path.join(root, "results", "corridor_proc.npz"), allow_pickle=True) 
     d2 = np.load(os.path.join(root, "data", "corridor_behavior.npz"), allow_pickle=True) 
     try:
         brain_img = plt.imread(os.path.join(root, "figures", "brain_window_visual.png"))
     except:
         brain_img = np.zeros((50,50))
 
     fig = _fig3(brain_img, **d, **d2)
```

### Comparing `rastermap-0.9.0/paper/fig4.ipynb` & `rastermap-0.9.1/paper/fig4.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995122354497354%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(12, '                  n_PCs=U0.shape[1]).fit(Usv = U0 * "*

 * *            "sv, \\n'), (13, '                                                          Vsv = "*

 * *            "Vsv)\\n'), (20, 'U_sn = utils.bin1d(U0[isort], bin_size=bin_size, axis=0) # bin over "*

 * *            "voxel axis\\n'), (21, 'sn = U_sn @ Vsv_sub.T\\n')], delete: [23, 22, 21, 20, 13, "*

 * *            "12]}}, 6: {'source': {insert: [(5, 'model = Rastermap(n_clusters=100, locality=0.1, "*

 * *            "time_lag_w […]*

```diff
@@ -100,26 +100,24 @@
                 "out = load_widefield_data(data_path)\n",
                 "(U0, sv, Vsv, ypos, xpos, regressors, \n",
                 "    behav_idx, stim_times, reward_times, stim_labels) = out\n",
                 "\n",
                 "\n",
                 "### run rastermap\n",
                 "model = Rastermap(n_clusters=100, locality=0.5, time_lag_window=10,\n",
-                "                  n_PCs=U0.shape[1], grid_upsample=5).fit(Usv = U0 * sv, \n",
-                "                                                          Vsv = Vsv, mean_time=True)\n",
+                "                  n_PCs=U0.shape[1]).fit(Usv = U0 * sv, \n",
+                "                                                          Vsv = Vsv)\n",
                 "\n",
                 "isort = model.isort \n",
                 "cc_nodes = model.cc\n",
                 "Vsv_sub = model.Vsv\n",
                 "\n",
                 "bin_size = 200\n",
-                "n_bins = U0.shape[0]//bin_size\n",
-                "sn = np.zeros((n_bins, Vsv.shape[0]), \"float32\")\n",
-                "for k in range(n_bins):\n",
-                "    sn[k] = U0[isort[k*bin_size : (k+1)*bin_size],:].sum(axis=0) @ Vsv_sub[:,:].T\n",
+                "U_sn = utils.bin1d(U0[isort], bin_size=bin_size, axis=0) # bin over voxel axis\n",
+                "sn = U_sn @ Vsv_sub.T\n",
                 "sn = zscore(sn, axis=1)\n",
                 "\n",
                 "### predict activity from behavior\n",
                 "ve, _, sn_pred, itest = linear_prediction.prediction_wrapper(regressors, sn.T, lam=1e4, delay=0)\n",
                 "sn_pred = sn_pred.T\n",
                 "itest = itest.flatten()\n",
                 "print(ve)\n",
@@ -154,15 +152,15 @@
             "outputs": [],
             "source": [
                 "### folder with \"subject_8\" folder\n",
                 "data_path = os.path.join(root, \"data\")\n",
                 "\n",
                 "spks, F, xyz, stims, swimming, eyepos = load_fish_data(data_path, subject=8)\n",
                 "\n",
-                "model = Rastermap(n_clusters=50, locality=0.75, time_lag_window=5, n_PCs=200).fit(spks)\n",
+                "model = Rastermap(n_clusters=100, locality=0.1, time_lag_window=5, n_PCs=200).fit(spks)\n",
                 "isort = model.isort \n",
                 "cc_nodes = model.cc\n",
                 "sn = zscore(utils.bin1d(zscore(spks[isort], axis=1), bin_size=50, axis=0), axis=1)\n",
                 "\n",
                 "np.savez(os.path.join(root, \"results\", \"fish_proc.npz\"),\n",
                 "         swimming=swimming, eyepos=eyepos, stims=stims, \n",
                 "         sn=sn, xyz=xyz, isort=isort, cc_nodes=cc_nodes)"
```

### Comparing `rastermap-0.9.0/paper/fig4.py` & `rastermap-0.9.1/paper/fig4.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             cax.set_xticks([-0.2,0,0.2])
             cax.set_xticklabels(["-0.2  ", "0", "  0.2"])
             cax.set_xlabel("diff. in \nvar. exp.")
 
     #ax.axis("square")
 
 def panels_hippocampus(fig, grid, il, spks, pyr_cells, speed, loc2d, tcurves, isort,
-                        cc_nodes, xmin=1000, xmax=2000, bin_sec=0.2):
+                        cc_nodes, isort2, xmin=1000, xmax=2000, bin_sec=0.2):
     ax = plt.subplot(grid[0,:3])
     pos = ax.get_position().bounds
     ax.set_position([pos[0], pos[1]+pos[3]*0.1, pos[2], pos[3]*0.9])
     grid1 = matplotlib.gridspec.GridSpecFromSubplotSpec(8,5, subplot_spec=ax, 
                                                             wspace=0.3, hspace=0.1)
     ax.remove()
 
@@ -188,15 +188,15 @@
             ve = ven
         elif j==2:
             X = sn_pred_beh 
             ve = ven_beh
         else:
             X = sn_pred - sn_pred_beh
             ve = ven - ven_beh
-        vmax=2
+        vmax=1.1
         ax = plt.subplot(grid1[j,1:])
         poss = ax.get_position().bounds
         ax.set_position([poss[0], poss[1], poss[2]*0.9, poss[3]])
         poss = ax.get_position().bounds
         cax = fig.add_axes([poss[0]+poss[2]*1.06, poss[1]+0.05*poss[3], 
                             poss[2]*0.02, 0.2*poss[3]])
         plot_raster(ax, X, xmin, xmax, n_neurons=None, fs=30, n_sec=5,
@@ -251,21 +251,24 @@
         cax.axis("off")
         cax.add_patch(patches.Rectangle(xy=(-0.5, 0), width=0.99, height=nn*1, 
                                 fill=False, edgecolor="k", lw=1))
     return il
 
 
 def panels_fish(fig, grid1, il, sn, swimming, eyepos, 
-                stims, xyz, isort, cc_nodes,
-                xmin=5900, xmax=6600):
+                stims, xyz, isort, isort2, cc_nodes):
     nn = sn.shape[0]
     nx = 3
     ny = 6
     nxy = nx * ny
 
+    xi = np.hstack((np.arange(5700, 6500), np.arange(7300,7860)))
+    stims = stims[xi]
+    #xmin=5600, xmax=7900
+
     ax = plt.subplot(grid1[0,:-1])
     pos = ax.get_position().bounds 
     ax.remove()
 
     yh = 0.09*pos[3]
     yh2 = 0.05*pos[3]
     ypad = 0.01*pos[3]
@@ -274,45 +277,45 @@
                         pos[2]-xp, pos[3]-(2*yh+yh2+3*ypad)])
     pos_neural = ax_neural.get_position().bounds
 
     ### eyepos
     ax = fig.add_axes([pos_neural[0], pos[1], pos_neural[2], yh])
     eye_color = [[0,0.95,0], [0,0.5,0.]]
     for i in range(2):
-        ax.plot(eyepos[:,i], color=eye_color[i])
-        ax.text(xmin+130, swimming[xmin:xmax].max()*(0.6- 0.42*i), 
+        ax.plot(eyepos[xi,i], color=eye_color[i])
+        ax.text(320+130*i, eyepos[xi].max()*(0.8), 
                 "left" if i==0 else "right", color=eye_color[i])
-    ax.text(xmin, eyepos[xmin:xmax].max()*0.6,"eye pos.", 
+    ax.text(0, eyepos[xi].max()*0.8, "eye pos.", 
                 color="k")
-    ax.plot([xmin, xmin+60], (-1+eyepos[xmin:xmax].min())*np.ones(2), 
+    ax.plot([0, 60], (-1+eyepos[xi].min())*np.ones(2), 
                 color="k")
-    ax.text(xmin, -5, "30 sec.")
-    ax.set_xlim([xmin,xmax])
+    ax.text(0, -5, "30 sec.")
+    ax.set_xlim([0, len(xi)])
     ax.axis("off")
     
     ### swimming
     swim_color = np.array([[0,1,1,1],
                            [0,0,1,1],
                            [1.0,0.0,0,1],
                            [0.8,1.0,0,1]])
 
     ax = fig.add_axes([pos_neural[0], pos[1] + yh + ypad, 
                         pos_neural[2], yh])
     for i in range(2):
-        ax.plot(swimming[:,i], color=swim_color[i])
-        ax.text(xmin+130, swimming[xmin:xmax].max()*(0.6- 0.42*i), 
+        ax.plot(swimming[xi,i], color=swim_color[i])
+        ax.text(0+320+130*i, swimming[xi].max()*(0.6), 
                 "left" if i==0 else "right", color=swim_color[i])
-    ax.text(xmin, swimming[xmin:xmax].max()*0.6,"swim speed", 
+    ax.text(0, swimming[xi].max()*0.6,"swimming", 
                 color="k")
-    ax.set_ylim([swimming[xmin:xmax].min(), swimming[xmin:xmax].max()])
-    ax.set_xlim([xmin,xmax])
+    ax.set_ylim([swimming[xi].min(), swimming[xi].max()])
+    ax.set_xlim([0, len(xi)])
     ax.axis("off")
 
     ### neuron activity
-    ax_neural.imshow(sn[:,xmin:xmax], vmin=0, vmax=1, 
+    ax_neural.imshow(sn[:, xi], vmin=0, vmax=1, 
                   cmap="gray_r", aspect="auto")
     ax_neural.axis("off")
     ax = fig.add_axes([-pos_neural[2]*0.01+pos_neural[0], pos_neural[1], 
                         0.01*pos_neural[2], pos_neural[3]])
     ax.plot(np.ones(2), [0, 40], 
                 color="k")
     ax.text(-2.5, 0, "2000 neurons", transform=ax.transAxes, rotation=90, ha="left")
@@ -336,75 +339,69 @@
     starts = np.append(np.array([0]), starts)
     starts = np.append(starts, np.array([len(stims)-1]))
     for n in range(len(starts)-1):
         start = starts[n]+1
         stype = stims[start]
         if stype!=3:
             width = starts[n+1] - start
-            if start+width > xmin and start < xmax:
-                width += min(0, start-xmin)
-                start = max(0, start-xmin)
-                width = min(width, xmax - xmin - start)
-                ax_neural.add_patch(
-                        patches.Rectangle(xy=(start, 0), width=width,
-                                  height=nn, facecolor=fcolor[stype], 
-                                  edgecolor=None, alpha=0.15*(stype!=2)))
-
-                if stype==11 or stype==10:
-                    if stype==11:
-                        ax_stim.arrow(start+0.2*width, 0, width*0.75, 0, width=0.04, 
-                                        head_length=10, length_includes_head=True,
-                                        facecolor=fcolor[stype])
-                    else:
-                        ax_stim.arrow(start+width*0.8, 0, -width*0.75, 0, width=0.04, 
-                                        head_length=10, length_includes_head=True,
-                                        facecolor=fcolor[stype], edgecolor=None)
-                    pim = np.zeros((12,12))
-                    pim[1:-1,1:3] = 1
-                    pim[1:-1,5:7] = 1
-                    pim[1:-1,9:11] = 1
-                    ax_stim.imshow(pim, extent=(start, start+width+2, -0.1, 0.1), 
-                                aspect="auto", cmap="gray", vmin=0, vmax=1)
-                elif stype==9 or stype==8:
-                    if stype==9:
-                        ax_stim.arrow(start+width*0.5, -0.06, 0, 0.13*1.2, width=5,
-                                        head_length=0.08, length_includes_head=True,
-                                        facecolor=fcolor[stype])      
-                    else:
-                        ax_stim.arrow(start+width*0.5, 0.08, 0, -0.13*1.2, width=5,
+            width += min(0, start)
+            start = max(0, start)
+            width = min(width, len(xi) - start)
+            ax_neural.add_patch(
+                    patches.Rectangle(xy=(start, 0), width=width,
+                                height=nn, facecolor=fcolor[stype], 
+                                edgecolor=None, alpha=0.15*(stype!=2)))
+
+            if stype==11 or stype==10:
+                if stype==11:
+                    ax_stim.arrow(start+0.2*width, 0, width*0.75, 0, width=0.04, 
+                                    head_length=10, length_includes_head=True,
+                                    facecolor=fcolor[stype], edgecolor='none')
+                else:
+                    ax_stim.arrow(start+width*0.8, 0, -width*0.75, 0, width=0.04, 
+                                    head_length=10, length_includes_head=True,
+                                    facecolor=fcolor[stype], edgecolor='none')
+                pim = np.ones((12,12))
+                ax_stim.imshow(pim, extent=(start, start+width+2, -0.1, 0.1), 
+                            aspect="auto", cmap="gray", vmin=0, vmax=1)
+            elif stype==9 or stype==8:
+                if stype==9:
+                    ax_stim.arrow(start+width*0.5, -0.06, 0, 0.13*1.2, width=8,
                                     head_length=0.08, length_includes_head=True,
-                                    facecolor=fcolor[stype], edgecolor=None)
-                    pim = np.zeros((12,width))
-                    pim[1:3,1:-1] = 1
-                    pim[5:7,1:-1] = 1
-                    pim[9:11,1:-1] = 1
-                    ax_stim.imshow(pim, extent=(start, start+width+2, -0.1, 0.1), 
-                                aspect="auto", cmap="gray", vmin=0, vmax=1)
-                elif stype==1:
-                    pim = np.zeros((12,width))
-                    pim[1:6] = 1
-                    ax_stim.imshow(pim, extent=(start, start+width+1, -0.1, 0.1), 
-                                aspect="auto", cmap="gray", vmin=0, vmax=1)
-                elif stype==0:
-                    pim = np.zeros((12,width))
-                    pim[6:11,:] = 1
-                    ax_stim.imshow(pim, extent=(start, start+width+1, -0.1, 0.1), 
-                                aspect="auto", cmap="gray", vmin=0, vmax=1)
-                elif stype==2:
-                    pim = np.zeros((12,width))
-                    pim[1:-1] = 1
-                    ax_stim.imshow(pim, extent=(start, start+width+2, -0.1, 0.1), 
-                                aspect="auto", cmap="gray", vmin=0, vmax=1)
+                                    facecolor=fcolor[stype], edgecolor='none')      
+                else:
+                    ax_stim.arrow(start+width*0.5, 0.08, 0, -0.13*1.2, width=8,
+                                head_length=0.08, length_includes_head=True,
+                                facecolor=fcolor[stype], edgecolor='none')
+                pim = np.ones((12,width))
+                ax_stim.imshow(pim, extent=(start, start+width+2, -0.1, 0.1), 
+                            aspect="auto", cmap="gray", vmin=0, vmax=1)
+            elif stype==1:
+                pim = np.ones((12,width))
+                ax_stim.text(start+width/2, -0.07, "L", fontsize="small",
+                                ha="center", va="bottom", color=fcolor[stype])
+                ax_stim.imshow(pim, extent=(start, start+width+1, -0.1, 0.1), 
+                            aspect="auto", cmap="gray", vmin=0, vmax=1)
+            elif stype==0:
+                pim = np.ones((12,width))
+                ax_stim.text(start+width/2, -0.07, "R", fontsize="small",
+                                ha="center", va="bottom", color=fcolor[stype])
+                ax_stim.imshow(pim, extent=(start, start+width+1, -0.1, 0.1), 
+                            aspect="auto", cmap="gray", vmin=0, vmax=1)
+            elif stype==2:
+                pim = np.ones((12,width))
+                ax_stim.imshow(pim, extent=(start, start+width+2, -0.1, 0.1), 
+                            aspect="auto", cmap="gray", vmin=0, vmax=1)
 
-    ax_stim.set_xlim([0, xmax - xmin])
+    ax_stim.set_xlim([0, len(xi)])
     ax_stim.axis("off")
 
-    ax_stim.text(0.2, 1.1, "phototactic stimuli", 
-        transform=ax_stim.transAxes, ha="center")
-    ax_stim.text(0.71, 1.1, "optomotor response stimuli", 
+    ax_stim.text(0., 1.1, "phototactic stimuli", 
+        transform=ax_stim.transAxes, ha="left")
+    ax_stim.text(0.55, 1.1, "optomotor response stimuli", 
         transform=ax_stim.transAxes, ha="center")
 
     ### title
     ax_stim.text(0, 2, "zebrafish brainwide recording", 
                     transform=ax_stim.transAxes, fontsize="large")
     transl = mtransforms.ScaledTranslation(-15 / 72, 14/ 72, fig.dpi_scale_trans)
     il = plot_label(ltr, il, ax_stim, transl, fs_title)
@@ -459,30 +456,65 @@
     fig = plt.figure(figsize=(14,10))
     yratio = 14 / 10
     grid = plt.GridSpec(2,5, figure=fig, left=0.02, right=0.98, top=0.96, bottom=0.02, 
                     wspace = 0.2, hspace = 0.08)
     il = 0
 
     try:
-        d = np.load(os.path.join(root, "results", "hippocampus_proc2.npz"))
+        d = np.load(os.path.join(root, "results", "hippocampus_proc.npz"))
         il = panels_hippocampus(fig, grid, il, **d)    
     except:
         print("hippocampus data not processed")
 
     ax = plt.subplot(grid[1,:3])
     grid1 = matplotlib.gridspec.GridSpecFromSubplotSpec(1,4, subplot_spec=ax, 
                                                             wspace=0.3, hspace=0.15)
     ax.remove()
     try:
-        d = np.load(os.path.join(root, "results", "fish_proc2.npz"))
+        d = np.load(os.path.join(root, "results", "fish_proc.npz"))
         il = panels_fish(fig, grid1, il, **d) 
     except:
         print("fish data not processed")
 
     try:
-        d = np.load(os.path.join(root, "results", "widefield_proc2.npz"))
+        d = np.load(os.path.join(root, "results", "widefield_proc.npz"))
         il = panels_widefield(fig, grid, il, **d)
     except:
         print("widefield data not processed")
 
     if save_figure:
-        fig.savefig(os.path.join(root, "figures", "fig4.pdf"), dpi=200)
+        fig.savefig(os.path.join(root, "figures", "fig4.pdf"), dpi=200)
+
+def suppfig_timesort(root, save_figure=True):
+
+    fig = plt.figure(figsize=(14,8))
+    yratio = 14 / 8
+    grid = plt.GridSpec(2,2, figure=fig, left=0.05, right=0.98, top=0.95, bottom=0.06, 
+                    wspace = 0.2, hspace = 0.25)
+    il = 0
+
+    titles = ["spontaneous activity", "virtual reality task", "rat hippocampus, linear track",
+                "fish wholebrain, visual stimuli"]
+    tstr = ["spont", "corridor", "hippocampus", "fish"]
+    transl = mtransforms.ScaledTranslation(-20 / 72, 10/ 72, fig.dpi_scale_trans)
+        
+    for j in range(4):
+        d = np.load(os.path.join(root, "results", f"{tstr[j]}_proc.npz"))
+        ax = plt.subplot(grid[j//2, j%2])
+        il = plot_label(ltr, il, ax, transl, fs_title)
+        if j!=2:
+            isort2 = d["isort2"]
+            sn = d["sn"]
+            sp = sn[:,isort2]
+        else:
+            isort = d["isort"]
+            isort2 = d["isort2"]
+            spks = d["spks"]
+            sp = spks[isort][:,isort2]
+
+        ax.imshow(sp, vmin=0, vmax=1.5, aspect="auto", cmap="gray_r")
+        ax.set_xlabel("time sorted")
+        ax.set_ylabel("superneurons" if j!=2 else "neurons")
+        ax.set_title(titles[j])
+
+    if save_figure:
+        fig.savefig(os.path.join(root, "figures", "suppfig_timesort.pdf"), dpi=200)
```

### Comparing `rastermap-0.9.0/paper/fig5.ipynb` & `rastermap-0.9.1/paper/fig5.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/paper/fig5.py` & `rastermap-0.9.1/paper/fig5.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,21 +27,26 @@
         nn, nt = X_embedding.shape
         emb_layer = d["emb_layer"]
         ex_frames = d["ex_frames"]
         iframes = d["iframes"]
 
         ax = plt.subplot(grid[i0, j0+1:j0+3])
         pos = ax.get_position().bounds
-        ax.imshow(X_embedding, aspect='auto', vmax=2.5, vmin=-0., cmap='gray_r')
+        ax.imshow(X_embedding, aspect='auto', 
+                 vmax=2.5, vmin=-0., 
+                 cmap='gray_r')
+        
         for k in range(4):
             ik = iframes[k]
             ax.plot(ik*np.ones(2), [0, nn], color="b", ls="--")
         ax.spines["left"].set_visible(False)
         ax.set_yticks([])
         ax.set_ylim([0, nn])
+        if env_id=="EnduroNoFrameskip-v4":
+            ax.set_xlim([780, nt])
         ax.invert_yaxis()
         ax.set_xlabel("timepoint in episode")
         if igame==0:
             ax.text(0.28, 1.02, "layers in DQN: ", color="k", 
                     transform=ax.transAxes, ha="right")
             for l, lcol in enumerate(layer_cols):
                 ax.text(0.3+l*0.13, 1.02, layer_names[l], color=lcol, transform=ax.transAxes)
```

### Comparing `rastermap-0.9.0/paper/fig_splitting.py` & `rastermap-0.9.1/paper/fig_splitting.py`

 * *Files 10% similar despite different names*

```diff
@@ -117,23 +117,24 @@
     ax.set_yticks([])
     ax.spines["left"].set_visible(False)
     ax.spines["bottom"].set_visible(False)
 
     return il
 
 def panels_v1stimresp(fig, grid, il, yratio, areas, X_embedding, bin_size,
-                      isort, xpos, ypos, stim_times, run, ex_stim, rfs, g0=1):
+                      isort, xpos, ypos, stim_times, run, ex_stim, 
+                      isort2, x, rfs, g0=1):
     subsample = 5
     xpos_sub = xpos[::subsample]
     ypos_sub = ypos[::subsample]
 
     ax = plt.subplot(grid[g0,0])
     pos = ax.get_position().bounds
     pos_ratio = (ypos.max() - ypos.min()) / (xpos.max() - xpos.min())
-    ax.set_position([pos[0]+0.01, pos[1]-0.04, pos[2]*0.9, pos[2]*0.9*yratio*pos_ratio])    
+    ax.set_position([pos[0]+0.01, pos[1]-0.07, pos[2]*0.9, pos[2]*0.9*yratio*pos_ratio])    
     memb = np.zeros_like(isort)
     memb[isort] = np.arange(0, len(isort))
     memb = memb[::subsample]
     ax.scatter(xpos_sub, -ypos_sub, s=2.5, 
             c=memb, cmap=cmap_emb, alpha=0.15, rasterized=True)
     iarea = [21, 23, 27, 3, 5]
     xw = 10
@@ -176,18 +177,19 @@
         x0, y0 = i*dx, i*dy
         imgs[y0:y0+ly, x0:x0+lx] = ex_stim[nimg-1-i]
     axin.imshow(imgs, cmap="gray", vmin=0, vmax=255)
     axin.text(1, -0.05, "x5000", fontweight="bold", 
             ha="right", va="top", transform=axin.transAxes)
     axin.axis("off")
 
-    ax = plt.subplot(grid[g0,1:4])
     xmin = 5000
     xmax = 5400
     padding_x = 0.005
+    
+    ax = plt.subplot(grid[g0,1:4])
     pos = ax.get_position().bounds
     ax.set_position([pos[0], pos[1]-0.03, pos[2], pos[3]*0.9])    
     axs = fig.add_axes([pos[0], pos[1]-0.03 + pos[3]*1.07, pos[2], pos[3]*0.05])
     axs.text(0, 1.1, "visual stim.", transform=axs.transAxes)
     st = stim_times[np.logical_and(stim_times < xmax, stim_times >= xmin)] - xmin
     axs.plot([0, xmax-xmin], [0, 0], color="k")
     axs.scatter(st, np.zeros(len(st)), color="k", marker=2, rasterized=True)
@@ -213,38 +215,53 @@
     nn = X_embedding.shape[0]
     emb_cols = plt.get_cmap("gist_ncar")(np.linspace(0.05, 0.95, nn))[::-1]
     cax.imshow(emb_cols[:,np.newaxis], aspect="auto")
     cax.set_ylim([0, nn*1.025])
     cax.invert_yaxis()
     cax.axis("off")
 
-    ax = plt.subplot(grid[g0:g0+2, 4])
+    ax = plt.subplot(grid[g0+1,1:4])
+    pos = ax.get_position().bounds
+    ax.set_position([pos[0], pos[1]-0.02, pos[2], pos[3]*0.9])    
+    transl = mtransforms.ScaledTranslation(-15 / 72, 5 / 72, fig.dpi_scale_trans)
+    il = plot_label(ltr, il, ax, transl, fs_title)
+    plot_raster(ax, x[:,isort2][:,::10], xmin=0, xmax=500, vmax=1.5, padding=0.04,
+                padding_x=padding_x, nper=bin_size, n_neurons=5000, xlabel="stim.",
+                label_pos="right", label=True, fs=1, n_sec=20)
+    ax.set_title("responses sorted across stimuli", fontsize="medium")
+
+    ax = plt.subplot(grid[g0:g0+4, 4])
     pos = ax.get_position().bounds
-    ax.set_position([pos[0], pos[1]-0.05, pos[2], pos[3]+0.05])    
-    ny, nx = 28, 8
+    ax.set_position([pos[0], pos[1]-0.07, pos[2], pos[3]+0.05])    
+    ny, nx = 30, 8
     grid1 = matplotlib.gridspec.GridSpecFromSubplotSpec(ny,nx, subplot_spec=ax, 
                                                                 wspace=0.15, hspace=0.1)
     ax.remove()
     dj = nn // (nx*ny)
-    rf_colors = cmap_emb(np.linspace(0, 1, nn))
     vmax = 1e-4
+    rfj = np.linspace(0, nn-1, nx*ny).astype("int")
     for j in range(nx*ny):
         ax = plt.subplot(grid1[j//nx, j%nx])
-        rfi = nn-1-j*dj
+        rfi = rfj[nx*ny - 1 - j]
         ax.imshow(rfs[rfi], vmin = -vmax, vmax = vmax, cmap = 'RdBu_r', rasterized=True)
         if j==0:
-            ax.set_title("receptive fields", fontsize="medium")
-            transl = mtransforms.ScaledTranslation(-15 / 72, 5 / 72, fig.dpi_scale_trans)
+            ax.text(0, 2.5, "superneuron receptive fields", transform=ax.transAxes)
+            transl = mtransforms.ScaledTranslation(-15 / 72, 15 / 72, fig.dpi_scale_trans)
             il = plot_label(ltr, il, ax, transl, fs_title)
         ax.axis('off')
+        if j<2 or j>nx*ny-3:
+            ax.text(0.5, 1.1, f"{nn - rfi}", ha="center", transform=ax.transAxes)
+        elif j==2 or j==nx*ny-3:
+            ax.text(0.5, 1.5, f"...", ha="center", transform=ax.transAxes)
+
 
     return il
 
 def panels_alexnet(fig, grid, il, X_embedding, bin_size, 
-                   isort, ipos, ilayer, iconv, nmax, g0=2):
+                   isort, isort2, ipos, ilayer, iconv, nmax, g0=2):
     
     memb = np.zeros(len(isort))
     memb[isort] = np.arange(len(isort))
     ax = plt.subplot(grid[g0,0])
     transl = mtransforms.ScaledTranslation(-15 / 72, -12 / 72, fig.dpi_scale_trans)
     il = plot_label(ltr, il, ax, transl, fs_title)
     ypre = 0
@@ -260,15 +277,15 @@
         ypre += (yp.max() + 4)
     ax.axis("square")
     ax.axis("off")
     ax.set_title("Alexnet convolutional layer responses", y=0.88)
 
     ax = plt.subplot(grid[g0,1:4])
     xmin = 2200
-    xmax = 2500
+    xmax = 2700
     padding_x = 0.005
     pos = ax.get_position().bounds
     ax.set_position([pos[0], pos[1]-0.01, pos[2], pos[3]*0.9]) 
     pos = ax.get_position().bounds
     cax = fig.add_axes([pos[0]+0.6*pos[2], pos[1]-pos[3]*0.05, 
                         pos[2]*0.06, pos[3]*0.03])
     plot_raster(ax, X_embedding, xmin, xmax, cax=cax, cax_label="left", 
@@ -279,14 +296,26 @@
     cax = fig.add_axes([pos[0]-pos[2]*0.03, pos[1], pos[2]*0.015, pos[3]])
     nn = X_embedding.shape[0]
     emb_cols = plt.get_cmap("gist_ncar")(np.linspace(0.05, 0.95, nn))[::-1]
     cax.imshow(emb_cols[:,np.newaxis], aspect="auto")
     cax.set_ylim([0, nn*1.025])
     cax.invert_yaxis()
     cax.axis("off")
+
+    ax = plt.subplot(grid[g0+1,1:4])
+    pos = ax.get_position().bounds
+    ax.set_position([pos[0], pos[1]-0.0, pos[2], pos[3]*0.9])    
+    transl = mtransforms.ScaledTranslation(-15 / 72, 5 / 72, fig.dpi_scale_trans)
+    il = plot_label(ltr, il, ax, transl, fs_title)
+    plot_raster(ax, X_embedding[:,isort2][:,::10], xmin=0, xmax=500, vmax=1.5, padding=0.04,
+                padding_x=padding_x, nper=bin_size, n_neurons=5000, xlabel="stim.",
+                label_pos="right", label=True, fs=1, n_sec=20)
+    ax.set_title("responses sorted across stimuli", fontsize="medium")
+
+
     return il
 
     
 def fig_all(root, save_figure=True):
     
     fig = plt.figure(figsize=(14,8))
     yratio = 14 / 8
```

### Comparing `rastermap-0.9.0/paper/fig_utils.py` & `rastermap-0.9.1/paper/fig_utils.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/paper/loaders.py` & `rastermap-0.9.1/paper/loaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,14 +201,15 @@
     del dat
     
     # take only high variance neurons (other neurons are noisy)
     good_neurons = F.std(axis=1) > 0.08
     S = S[good_neurons]
     F = F[good_neurons]
     xyz = xyz[good_neurons]
+    xyz[:,0] = -1*xyz[:,0]
 
     return S, F, xyz, stims, swimming, eyepos
 
 def load_widefield_data(root):
     USV = mat73.loadmat(os.path.join(root, "Vc.mat"))
     U = np.array(USV["U"])
     Ly,Lx = U.shape[:-1]
```

### Comparing `rastermap-0.9.0/paper/metrics.py` & `rastermap-0.9.1/paper/metrics.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/paper/other_upsampling.py` & `rastermap-0.9.1/paper/other_upsampling.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/paper/qrdqn.py` & `rastermap-0.9.1/paper/qrdqn.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,18 +152,23 @@
     S = zscore(spks[igood], axis=1)
     rm_model = Rastermap(time_lag_window=10, locality=0.75).fit(S[:,:])
     isort = rm_model.isort
 
     # show last episode
     bin_size = 50
     X_embedding = zscore(utils.bin1d(S[:,-eps_len[-1]:][isort], bin_size, axis=0), axis=1)
-    if env_id=="EnduroNoFrameskip-v4":
-        X_embedding = X_embedding[:,780:]
-        obs = obs[780:]
+    #if env_id=="EnduroNoFrameskip-v4":
+    #    X_embedding = X_embedding[:,780:]
+    #    obs = obs[780:]
     nn, nt = X_embedding.shape
-    iframes = np.linspace(nt*0.1, nt*0.9, 4).astype("int")
+    if env_id=="EnduroNoFrameskip-v4":
+        nt = nt-900
+        iframes = np.linspace(780 + nt*0.1, 780 + nt*0.9, 4).astype("int")
+    else:
+        iframes = np.linspace(nt*0.1, nt*0.9, 4).astype("int")
+    print(iframes)
     emb_layer = mode(ilayer[igood][isort][:nn*bin_size].reshape(-1, bin_size), axis=1, keepdims=False).mode
     ex_frames = obs[iframes]
     print(ex_frames.shape)
     np.savez(os.path.join(root, "simulations/", f"qrdqn_{env_id}_results.npz"),
              X_embedding=X_embedding, emb_layer=emb_layer, 
              ex_frames=ex_frames, iframes=iframes)
```

### Comparing `rastermap-0.9.0/paper/simulations.py` & `rastermap-0.9.1/paper/simulations.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
         model = Rastermap(n_clusters=100, 
                         n_PCs=200, 
                         locality=0.8,
                         time_lag_window=10,
                         symmetric=False,
                         grid_upsample=10,
                         time_bin=10,
-                        bin_size=0).fit(spks, normalize=True, mean_time=True)
+                        bin_size=0).fit(spks)
         embs_all[random_state, 0] = model.embedding
 
         # tsne
         M = metrics.run_TSNE(model.Usv, perplexities=[30])
         embs_all[random_state, 1] = M
 
         # umap
```

### Comparing `rastermap-0.9.0/paper/splitting.ipynb` & `rastermap-0.9.1/paper/splitting.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987743506493507%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(8, '                             n_PCs=400, "*

 * *            "mean_time=False).fit(spks)\\n'), (16, '# compute stimulus responses sresp and average "*

 * *            "over the three repeats\\n'), (32, '\\n'), (33, '# sort stimuli\\n'), (34, 'model2 = "*

 * *            "Rastermap(n_clusters=100, n_splits=0, locality=0.,\\n'), (35, "*

 * *            "'                             n_PCs=400).fit(x.T)\\n'), (36, 'isort2 = "*

 * *            "model2.isort\\n'), (64, '         X_embedding=X_emb […]*

```diff
@@ -93,23 +93,23 @@
                 "stim_filename = os.path.join(root, \"data/\", \"text5k_3x.mat\")\n",
                 "\n",
                 "out = load_visual_data(filename, stim_filename)\n",
                 "spks, istim, stim_times, xpos, ypos, run, ex_stim, img_pca, img_U, Ly, Lx = out\n",
                 "\n",
                 "# run rastermap \n",
                 "model = Rastermap(n_clusters=100, n_splits=3, nc_splits=25, locality=0.,\n",
-                "                             n_PCs=400).fit(spks, normalize=True, mean_time=False)\n",
+                "                             n_PCs=400, mean_time=False).fit(spks)\n",
                 "isort = model.isort\n",
                 "# bin by rastermap\n",
                 "n_neurons = len(isort)\n",
                 "n_bins = 500\n",
                 "bin_size = n_neurons // n_bins\n",
                 "X_embedding = zscore(utils.bin1d(spks[isort], bin_size, axis=0), axis=1)\n",
                 "\n",
-                "# sort sresp into stimuli and average over the three repeats\n",
+                "# compute stimulus responses sresp and average over the three repeats\n",
                 "iss = np.zeros((3,5000), \"int\")\n",
                 "for j in range(5000):\n",
                 "    iss[:,j] = (istim==j).nonzero()[0][:3]\n",
                 "sresp = spks[:, stim_times]\n",
                 "sresp = sresp[:, iss].transpose((1,0,2))\n",
                 "snr_neurons = (zscore(sresp[0], axis=-1) * zscore(sresp[1], axis=-1)).mean(axis=1)\n",
                 "\n",
@@ -118,14 +118,19 @@
                 "n_bins = 500\n",
                 "bin_size = n_neurons // n_bins\n",
                 "x = sresp[:, isort[:(n_neurons // bin_size) * bin_size]]\n",
                 "x = x.reshape(3, -1, bin_size, n_stim).mean(axis=2)\n",
                 "n_bins = x.shape[1]\n",
                 "snr = (zscore(x[0], axis=-1) * zscore(x[1], axis=-1)).mean(axis=-1)\n",
                 "\n",
+                "# sort stimuli\n",
+                "model2 = Rastermap(n_clusters=100, n_splits=0, locality=0.,\n",
+                "                             n_PCs=400).fit(x.T)\n",
+                "isort2 = model2.isort\n",
+                "\n",
                 "# mean over 3 repeats\n",
                 "sresp = sresp.mean(axis=0)\n",
                 "sresp = zscore(sresp, axis=1)\n",
                 "x = x.mean(axis=0)\n",
                 "x = zscore(x, axis=-1)\n",
                 "\n",
                 "# ridge regression from 200 image PCs to 1000 rastermap components\n",
@@ -144,15 +149,16 @@
                 "# evaluate model on test data\n",
                 "rpred = img_pca[itest] @ B\n",
                 "cpred = (zscore(rpred.T, 1) * zscore(x[:,itest], 1)).mean(1)\n",
                 "\n",
                 "print(f\"mean r on test data {cpred.mean()}\")\n",
                 "\n",
                 "np.savez(os.path.join(root, \"results\", \"v1stimresp_proc.npz\"),\n",
-                "         X_embedding=X_embedding, bin_size=bin_size, isort=isort, xpos=xpos, ypos=ypos,\n",
+                "         X_embedding=X_embedding, bin_size=bin_size, isort=isort, isort2=isort2, \n",
+                "         xpos=xpos, ypos=ypos, x=x,\n",
                 "         stim_times=stim_times, run=run, ex_stim=ex_stim, rfs=rfs)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -168,23 +174,28 @@
             "outputs": [],
             "source": [
                 "filename = os.path.join(root, \"data\", \"ann_fvs_Grayscale(224)_TX61_3X.npz\")\n",
                 "sresp, ilayer, ipos, iconv, nmax = load_alexnet_data(filename)\n",
                 "\n",
                 "# run rastermap\n",
                 "model = Rastermap(n_clusters=100, n_splits=3, nc_splits=25, locality=0.,\n",
-                "                             n_PCs=400).fit(sresp, normalize=True, mean_time=False)\n",
+                "                             n_PCs=400, mean_time=False).fit(sresp)\n",
                 "isort = model.isort\n",
                 "\n",
                 "# bin by rastermap\n",
                 "bin_size = 24\n",
                 "X_embedding = zscore(utils.bin1d(sresp[isort], bin_size, axis=0), axis=1)\n",
                 "\n",
+                "# sort stimuli\n",
+                "model2 = Rastermap(n_clusters=100, n_splits=0, locality=0.,\n",
+                "                             n_PCs=400).fit(X_embedding.T)\n",
+                "isort2 = model2.isort\n",
+                "\n",
                 "np.savez(os.path.join(root, \"results\", \"alexnet_proc.npz\"),\n",
-                "         X_embedding=X_embedding, bin_size=bin_size, isort=isort, \n",
+                "         X_embedding=X_embedding, bin_size=bin_size, isort=isort, isort2=isort2,\n",
                 "         ilayer=ilayer, ipos=ipos, iconv=iconv, nmax=nmax)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -213,26 +224,26 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from scipy.io import loadmat\n",
                 "\n",
-                "fig = plt.figure(figsize=(14,16/3))\n",
-                "yratio = 14 / (16/3)\n",
-                "grid = plt.GridSpec(2,5, figure=fig, left=0.01, right=0.99, top=0.94, bottom=0.07, \n",
+                "fig = plt.figure(figsize=(14, 10))\n",
+                "yratio = 14 / 10\n",
+                "grid = plt.GridSpec(4,5, figure=fig, left=0.01, right=0.99, top=0.94, bottom=0.07, \n",
                 "                    wspace = 0.15, hspace = 0.25)\n",
                 "il = 0\n",
                 "areas = loadmat(os.path.join(root, \"figures\", \"ctxOutlines.mat\"), \n",
                 "                squeeze_me=True)[\"coords\"]\n",
                 "d = np.load(os.path.join(root, \"results\", \"v1stimresp_proc.npz\"))\n",
                 "il = fig_splitting.panels_v1stimresp(fig, grid, il, yratio, areas, **d, g0=0)\n",
                 "\n",
                 "d = np.load(os.path.join(root, \"results\", \"alexnet_proc.npz\"))\n",
-                "il = fig_splitting.panels_alexnet(fig, grid, il, **d, g0=1)  \n",
+                "il = fig_splitting.panels_alexnet(fig, grid, il, **d, g0=2)  \n",
                 "\n",
                 "fig.savefig(os.path.join(root, \"figures\", \"suppfig_visual.pdf\"), dpi=200)\n"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `rastermap-0.9.0/rastermap/__main__.py` & `rastermap-0.9.1/rastermap/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""
-Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
-"""
+"""
+Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
+"""
 from scipy.stats import zscore
 import numpy as np
 import argparse
 import os
 from rastermap import Rastermap
 from rastermap.io import load_activity
 
@@ -40,23 +40,23 @@
                 iscell = iscell[:, 0].astype("bool")
             else:
                 iscell = iscell.astype("bool")
             if iscell.size == X.shape[0]:
                 X = X[iscell, :]
                 print("iscell found and used to select neurons")
         
-        if Usv.ndim==3:
+        if Usv is not None and Usv.ndim==3:
             Usv = Usv.reshape(-1, Usv.shape[-1])
         
         model = Rastermap(**ops)
         train_time = np.ones(X.shape[1] if X is not None 
                              else Vsv.shape[0], "bool")
         if X is not None:
             if ("end_time" in ops and ops["end_time"] == -1) or "end_time" not in ops:
-                ops["end_time"] = S.shape[1]
+                ops["end_time"] = X.shape[1]
                 ops["start_time"] = 0
             else:
                 train_time = np.zeros(X.shape[1], "bool")
                 train_time[np.arange(ops["start_time"], ops["end_time"]).astype(int)] = 1
                 X = X[:, train_time]
 
         model.fit(data=X, Usv=Usv, Vsv=Vsv)
```

### Comparing `rastermap-0.9.0/rastermap/cluster.py` & `rastermap-0.9.1/rastermap/cluster.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/rastermap/gui/colormaps.py` & `rastermap-0.9.1/rastermap/gui/colormaps.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/rastermap/gui/gui.py` & `rastermap-0.9.1/rastermap/gui/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -591,36 +591,38 @@
             self.update_status_bar("ERROR: please upload neuron position data")
 
     def plot_scatter(self, x, y, roi_id=None, iplane=0):
         if self.all_neurons_checkBox.isChecked() and roi_id is None:
             colors = colormaps.gist_ncar[np.linspace(
                 0, 254, len(x)).astype("int")][self.sorting]
             brushes = [pg.mkBrush(color=c) for c in colors]
-            self.scatter_plots[iplane][0].setData(x, y, symbol="o", brush=brushes,
+            self.scatter_plots[iplane][0].setData(x, y, symbol="o", size=3,
+                                                  brush=brushes,
                                                   hoverable=True)
             for i in range(1, nclust_max + 1):
                 self.scatter_plots[iplane][i].setData([], [])
         else:
             if roi_id is None:
                 self.scatter_plots[iplane][0].setData(
-                    x, y, symbol="o", brush=pg.mkBrush(color=(180, 180, 180)),
+                    x, y, symbol="o", size=3,
+                    brush=pg.mkBrush(color=(180, 180, 180)),
                     hoverable=True)
                 for roi_id in range(nclust_max):
                     if roi_id < len(self.cluster_rois):
                         selected = self.neurons_selected(self.cluster_slices[roi_id])
                         self.scatter_plots[iplane][roi_id + 1].setData(
-                            x[selected], y[selected], symbol="o",
+                            x[selected], y[selected], symbol="o", size=3,
                             brush=pg.mkBrush(color=self.colors[roi_id][:3]),
                             hoverable=True)
                     else:
                         self.scatter_plots[iplane][roi_id + 1].setData([], [])
             else:
                 selected = self.neurons_selected(self.cluster_slices[roi_id])
                 self.scatter_plots[iplane][roi_id + 1].setData(
-                    x[selected], y[selected], symbol="o",
+                    x[selected], y[selected], symbol="o", size=3,
                     brush=pg.mkBrush(color=self.colors[roi_id][:3]), hoverable=True)
 
 
 def run(filename=None, proc=False):
     # Always start by initializing Qt (only once per application)
     app = QApplication(sys.argv)
     icon_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "logo.png")
```

### Comparing `rastermap-0.9.0/rastermap/gui/guiparts.py` & `rastermap-0.9.1/rastermap/gui/guiparts.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/rastermap/gui/io.py` & `rastermap-0.9.1/rastermap/gui/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,17 +365,17 @@
 
     if user_clusters is not None:
         parent.smooth_bin = user_clusters[0]["binsize"]
         parent.smooth.setText(str(int(parent.smooth_bin)))
 
     parent.embedding = y
     parent.sorting = isort
-    parent.Usv = Usv if parent.Usv is None else parent.Usv
-    parent.Vsv = Vsv if parent.Vsv is None else parent.Vsv
-    parent.sv = sv if parent.sv is None else parent.sv
+    parent.Usv = Usv #if parent.Usv is None else parent.Usv
+    parent.Vsv = Vsv #if parent.Vsv is None else parent.Vsv
+    parent.sv = sv #if parent.sv is None else parent.sv
     parent.ops = ops
     parent.user_clusters = user_clusters
 
     print(f"loaded:  {parent.proc['filename']}")
     _load_iscell_stat(parent)
     _load_sp(parent)
```

### Comparing `rastermap-0.9.0/rastermap/gui/menus.py` & `rastermap-0.9.1/rastermap/gui/menus.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/rastermap/gui/run.py` & `rastermap-0.9.1/rastermap/gui/run.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/rastermap/gui/views.py` & `rastermap-0.9.1/rastermap/gui/views.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/rastermap/io.py` & `rastermap-0.9.1/rastermap/io.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/rastermap/rastermap.py` & `rastermap-0.9.1/rastermap/rastermap.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,38 +9,34 @@
 from .cluster import kmeans, scaled_kmeans, compute_cc_tdelay
 from .sort import traveling_salesman, compute_BBt, matrix_matching
 from .upsample import grid_upsampling
 from .utils import bin1d
 from .svd import SVD
 
 def default_settings():
+    """ default settings for main algorithm settings """
     settings = {}
     settings["n_clusters"] = 100
     settings["n_PCs"] = 200
     settings["time_lag_window"] = 0
     settings["locality"] = 0.0
-    settings["grid_upsample"] = 10
-    settings["smoothness"] = 1
     settings["n_splits"] = 0
-    settings["bin_size"] = 0
     settings["time_bin"] = 0
-    settings["run_scaled_kmeans"] = True
-    settings["symmetric"] = True
-    settings["keep_norm_X"] = False
-    settings["sticky"] = True
+    settings["grid_upsample"] = 10
+    settings["mean_time"] = True
     settings["verbose"] = True
     settings["verbose_sorting"] = False
     return settings
 
 
 def sequence_settings():
     """ good for data with sequences """
     settings = default_settings()
     settings["time_lag_window"] = 10
-    settings["locality"] = 1.0
+    settings["locality"] = 0.75
     return settings
 
 
 def highd_settings():
     """ good for large scale data with high-d features like natural image responses """
     settings = default_settings()
     settings["n_clusters"] = 100
@@ -53,205 +49,259 @@
     info = {}
     info["n_clusters"] = (
         """number of clusters created from data before upsampling and creating embedding \n 
             (any number above 150 will be very slow due to NP-hard sorting problem)"""
     )
     info["n_PCs"] = "number of PCs to use during optimization"
     info["time_lag_window"] = (
-        """number of time points into the future to compute cross-correlation, useful for sequence finding"""
+        """number of time points into the future to compute cross-correlation, 
+            useful for sequence finding"""
     )
     info["locality"] = (
         "how local should the algorithm be -- set to 1.0 for highly local + sequence finding"
     )
     info["grid_upsample"] = "how much to upsample clusters"
-    info["smoothness"] = (
-        "how much to smooth over clusters when upsampling, set to number from 1 to number of clusters"
-    )
     info["n_splits"] = (
         "split, recluster and sort n_splits times (increases local neighborhood preservation); \n (4 with 50 clusters => 800 clusters)"
     )
-    info["bin_size"] = (
-        """binning of data across n_samples to return embedding figure, X_embedding; \n 
-            if 0, then binning based on data size, if 1 then no binning"""
-    )
     info["time_bin"] = (
         """ binning of data in time before PCA is computed """
     )
-    info["run_scaled_kmeans"] = (
-        "run scaled_kmeans as clustering algorithm; if False, run kmeans"
-    )
-    info["symmetric"] = (
-        """if False, use only positive time lag cross-correlations for sorting (only makes a difference if time_lag_window > 0); 
-            \n keep False for sequence finding"""
-    )
-    info["keep_norm_X"] = "keep normalized version of X saved as member of class"
-    info["sticky"] = (
-        """if n_splits>0, sticky=True keeps neurons in same place as initial sorting before splitting; \n 
-            otherwise neurons can move each split (which generally does not work as well)"""
+    info["mean_time"] = (
+        """whether to project out the mean over data samples at each timepoint,
+             usually good to keep on to find structure"""
     )
     info["verbose"] = "whether to output progress during optimization"
     info["verbose_sorting"] = "output progress in travelling salesman"
     return info
 
 
 class Rastermap:
     """Rastermap embedding algorithm
     Rastermap takes the n_PCs (200 default) of the data, and embeds them into
     n_clusters clusters. It then sorts the clusters and upsamples to a grid with 
     grid_upsample * n_clusters nodes. Each data sample is assigned to a node. 
-    The assignment of the samples to nodes is returned.
+    The assignment of the samples to nodes is attribute `embedding`, and the sorting 
+    of the nodes is `isort`.
 
-    data : n_samples x n_features
+    Parameters in order of importance
 
     Parameters
     -----------
     n_clusters : int, optional (default: 100)
         number of clusters created from data before upsampling and creating embedding
-        (any number above 150 will be very slow due to NP-hard sorting problem)
+        (any number above 150 will be slow due to NP-hard sorting problem, max is 200)
     n_PCs : int, optional (default: 200)
         number of PCs to use during optimization
     time_lag_window : int, optional (default: 0)
-        number of time points into the future to compute cross-correlation, useful for sequence finding
+        number of time points into the future to compute cross-correlation, 
+        useful to set to several timepoints for sequence finding
     locality : float, optional (default: 0.0)
-        how local should the algorithm be -- set to 1.0 for highly local + sequence finding
+        how local should the algorithm be -- set to 1.0 for highly local + 
+        sequence finding, and 0.0 for global sorting
     grid_upsample : int, optional (default: 10)
         how much to upsample clusters, if set to 0.0 then no upsampling
-    smoothness : int, optional (default: 1)
-        how much to smooth over clusters when upsampling, number from 1 to number of clusters
+    time_bin : int, optional (default: 0)
+        binning of data in time before PCA is computed, if set to 0 or 1 no binning occurs
+    mean_time : bool, optional (default: True)
+        whether to project out the mean over data samples at each timepoint,
+             usually good to keep on to find structure
     n_splits : int, optional (default: 0)
-        split, recluster and sort n_splits times (increases local neighborhood preservation); 
-        (4 with 50 clusters => 800 clusters)
-    bin_size : int, optional (default: 0)
-        binning of data across n_samples to return embedding figure, X_embedding; 
-        if 0, then binning based on data size, if 1 then no binning
+        split, recluster and sort n_splits times 
+        (increases local neighborhood preservation for high-dim data); 
+        results in (n_clusters * 2**n_splits) clusters
     run_scaled_kmeans : bool, optional (default: True)
         run scaled_kmeans as clustering algorithm; if False, run kmeans
-    symmetric : bool, optional (default: False)
-        if False, use only positive time lag cross-correlations for sorting (only makes a difference if time_lag_window > 0); 
-        keep False for sequence finding
+    verbose : bool (default: True)
+        whether to output progress during optimization
+    verbose_sorting : bool (default: False)
+        output progress in travelling salesman    
     keep_norm_X : bool, optional (default: True)
         keep normalized version of X saved as member of class
+    bin_size : int, optional (default: 0)
+        binning of data across n_samples to return embedding figure, X_embedding; 
+        if 0, then binning based on data size, if 1 then no binning
+    symmetric : bool, optional (default: False)
+        if False, use only positive time lag cross-correlations for sorting 
+        (only makes a difference if time_lag_window > 0); 
+        recommended to keep False for sequence finding
     sticky : bool, optional (default: True)
         if n_splits>0, sticky=True keeps neurons in same place as initial sorting before splitting; 
         otherwise neurons can move each split (which generally does not work as well)
-    verbose : bool (default: True)
-        whether to output progress during optimization
-    verbose_sorting : bool (default: False)
-        output progress in travelling salesman
+    nc_splits : int, optional (default: None)
+        if n_splits > 0, size to split n_clusters into; 
+        if None, nc_splits = min(50, n_clusters // 4)
+    smoothness : int, optional (default: 1)
+        how much to smooth over clusters when upsampling, number from 1 to number of 
+        clusters (recommended to not change, instead use locality to change sorting)
+    
     """
 
     def __init__(self, n_clusters=100, n_PCs=200, time_lag_window=0.0, locality=0.0,
-                 smoothness=1, grid_upsample=10, bin_size=0, 
-                 time_bin=0, sticky=True, n_splits=0, nc_splits=None, circular=False,
-                 run_scaled_kmeans=True, symmetric=False, 
-                 keep_norm_X=True, verbose=True,
-                 verbose_sorting=False):
+                 grid_upsample=10, time_bin=0, normalize=True, mean_time=True, n_splits=0,
+                 run_scaled_kmeans=True, verbose=True, verbose_sorting=False, 
+                 keep_norm_X=True, bin_size=0, symmetric=False, 
+                 sticky=True, nc_splits=None, smoothness=1):
 
-        self.n_PCs = n_PCs
-        self.n_splits = n_splits
         self.n_clusters = n_clusters
-        self.nc_splits = nc_splits
-        self.run_scaled_kmeans = run_scaled_kmeans
-        self.sticky = sticky
-        
+        self.n_PCs = n_PCs
         self.time_lag_window = time_lag_window
-        self.symmetric = symmetric
         self.locality = locality
-        self.circular = circular
-        self.smoothness = smoothness
         self.grid_upsample = grid_upsample
         self.time_bin = time_bin
-        self.bin_size = 0
-        
-        self.keep_norm_X = keep_norm_X
+        self.normalize = normalize
+        self.mean_time = mean_time
+        self.n_splits = n_splits
+        self.run_scaled_kmeans = run_scaled_kmeans
         self.verbose = verbose
         self.verbose_sorting = verbose_sorting
 
+        self.keep_norm_X = keep_norm_X
+        self.bin_size = bin_size                
+        self.symmetric = symmetric
+        self.sticky = sticky
+        self.nc_splits = nc_splits
+        self.smoothness = smoothness
+        
         self.sorting_algorithm = "travelling_salesman"
-        self.quadratic_upsample = False
-        self.gradient_upsample = False  ### NOT IMPLEMENTED
-
-    def fit_transform(self, X, u=None):
-        """Fit X into an embedded space and return that transformed
-        output.
-        Inputs
-        ----------
-        X : array, shape (n_samples, n_features). X contains a sample per row.
+        
+    def fit(self, data=None, Usv=None, Vsv=None, U_nodes=None, itrain=None,
+            compute_X_embedding=False):
+        """ sorts data or singular value decomposition of data by first axis
 
-        Returns
-        -------
-        embedding : array, shape (n_samples, n_components)
-            Embedding of the training data in low-dimensional space.
-        """
-        self.fit(X, u)
-        return self.embedding
+        can use full data matrix, or use singular value decomposition, to reduce RAM 
+        requirements, it is recommended to use float32. see Rastermap class for 
+        parameter information (`Rastermap?`)
+
+        example usage:
+        ```
+        import numpy as np
+        import matplotlib.pyplot as plt
+        from rastermap import Rastermap, utils
+        from scipy.stats import zscore
+
+        # spks is neurons by time
+        spks = np.load("spks.npy").astype("float32")
+        spks = zscore(spks, axis=1)
+
+        # fit rastermap
+        model = Rastermap(n_PCs=200, n_clusters=100, 
+                        locality=0.75, time_lag_window=5).fit(spks)
+        y = model.embedding # neurons x 1
+        isort = model.isort
+
+        # bin over neurons
+        X_embedding = zscore(utils.bin1d(spks, bin_size=25, axis=0), axis=1)
+
+        # plot
+        fig = plt.figure(figsize=(12,5))
+        ax = fig.add_subplot(111)
+        ax.imshow(X_embedding, vmin=0, vmax=1.5, cmap="gray_r", aspect="auto")
+        ```
 
-    def fit(self, data=None, Usv=None, Vsv=None, U_nodes=None, itrain=None,
-            normalize=True, mean_time=True, compute_X_embedding=True, 
-            bin_size=0):
-        """Fit X into an embedded space.
         Inputs
         ----------
-        X : array, shape (n_samples, n_features) - float32 recommended
-        u, v : svd decomposition of X (optional), u should be u*sv
+        data : array, shape (n_samples, n_features) (optional, default None) 
+            this matrix is usually neurons/voxels by time, or None if using decomposition, 
+            e.g. as in widefield imaging
+        Usv : array, shape (n_samples, n_PCs) (optional, default None)
+            singular vectors U times singular values sv
+        Vsv : array, shape (n_features, n_PCs) (optional, default None)
+            singular vectors U times singular values sv
+        U_nodes : array, shape (n_clusters, n_PCs) (optional, default None)
+            cluster centers in PC space, if you have precomputed them
+        itrain : array, shape (n_features,) (optional, default None)
+            fit embedding on timepoints itrain only
 
         Assigns
         ----------
-        embedding : array-like, shape (n_samples, n_components)
-            Stores the embedding vectors.
-        isort : sorting along first dimension of matrix
-        
+        embedding : array, shape (n_samples, 1)
+            embedding of each neuron / voxel
+        isort : sorting along first dimension of input matrix
+            use this to get neuron / voxel sorting
+        igood : array, shape (n_samples, 1)
+            neurons/voxels which had non-zero activity and were used for sorting
+        Usv : array, shape (n_samples, n_PCs) 
+            singular vectors U times singular values sv
+        Vsv : array, shape (n_features, n_PCs)
+            singular vectors U times singular values sv
+        U_nodes : array, shape (n_clusters, n_PCs) 
+            cluster centers in PC space
+        Y_nodes : array, shape (n_clusters, 1) 
+            np.arange(0, n_clusters)
+        X_nodes : array, shape (n_clusters, n_features)
+            cluster activity traces in time
+        cc : array, shape (n_clusters, n_clusters)
+            sorted asymmetric similarity matrix
+        embedding_clust : array, shape (n_samples, 1)
+            assignment of each neuron/voxel to each cluster (before upsampling)
+        X : array, shape (n_samples, n_features)
+            normalized data stored (if keep_norm_X is True)
+        X_embedding : array, shape (n_samples//bin_size, n_features)
+            normalized data binned across samples (if compute_X_embedding is True)
+
         """
         t0 = time.time()
 
         
         # normalize data
         igood = ~np.isnan(data[:,0]) if data is not None else ~np.isnan(Usv[:,0])
         stdx = None
+        normed = False
         if data is not None:
-            if normalize:
+            if self.normalize:
                 if hasattr(self, "X"):
-                    warnings.warn("not renormalizing, using previous normalization")
+                    warnings.warn("not renormalizing / subtracting mean, using previous normalization")
                     X = self.X 
                 else:
-                    print("normalizing data")
+                    print("normalizing data across axis=1")
                     X = data.copy() 
                     if self.time_bin > 1:
                         print(f"binning in time with time_bin = {self.time_bin}")
                         X = bin1d(X, bin_size=self.time_bin, axis=1)
                     X -= X.mean(axis=1)[:,np.newaxis]
                     stdx = X.std(axis=1)
                     X /= stdx[:,np.newaxis]
-                    if mean_time:
-                        X_mean = np.nanmean(X, axis=0, keepdims=True).T
-                        X_mean /= (X_mean**2).sum()**0.5
-                        w_mean = X @ X_mean
-                        X -= w_mean @ X_mean.T
-                    if self.keep_norm_X:
-                        self.X = X
+                    normed = True
             else:
                 if self.time_bin > 1:
                     X = bin1d(data.copy(), bin_size=self.time_bin, axis=1)
                 else:
                     X = data
+            if self.mean_time:
+                if hasattr(self, "X"):
+                    warnings.warn("not renormalizing / subtracting mean, using previous normalization")
+                    X = self.X 
+                else:
+                    print("projecting out mean along axis=0")
+                    X_mean = np.nanmean(X, axis=0, keepdims=True).T
+                    X_mean /= (X_mean**2).sum()**0.5
+                    w_mean = X @ X_mean
+                    X -= w_mean @ X_mean.T
+                    normed = True
+            if self.keep_norm_X and (self.mean_time or self.normalize):
+                self.X = X
         elif hasattr(self, "X"):
             X = self.X
             Vsv_sub = Vsv.copy()
-            if normalize:
-                warnings.warn("not renormalizing, using previous normalization")
+            if self.normalize or self.mean_time:
+                warnings.warn("not renormalizing / subtracting mean, using previous normalization")
         else:
-            if mean_time:
+            if self.mean_time:
                 V_mean = Vsv.mean(axis=1, keepdims=True)
                 V_mean /= (V_mean**2).sum()**0.5
                 self.V_mean = V_mean
                 proj_mean = V_mean @ (V_mean.T @ Vsv)
                 Vsv_sub = Vsv.copy() - proj_mean
+                normed = True
             else:
                 Vsv_sub = Vsv.copy()
             stdx = Usv.std(axis=1) if stdx is None else stdx
+        if normed:
+            print(f"data normalized, {time.time()-t0:0.2f}sec")    
 
         stdx = X.std(axis=1) if stdx is None else stdx
         igood = np.logical_and(igood, stdx > 0)
         n_samples = igood.sum() 
         n_time = data.shape[1] if data is not None else Vsv.shape[0]
         print(f"sorting activity: {n_samples} valid samples by {n_time} timepoints")
         
@@ -263,15 +313,15 @@
                 Usv_valid = SVD(X[igood][:, itrain] if itrain is not None else X, 
                                n_components=self.n_PCs)            
                 Usv = np.nan * np.zeros((len(igood), Usv_valid.shape[1]), "float32")
                 Usv[igood] = Usv_valid
                 self.Usv = Usv
                 self.n_PCs = Usv.shape[1]
                 pc_time = time.time() - tic
-                print(f"n_PCs = {self.n_PCs} computed in {pc_time:0.2f}sec")    
+                print(f"n_PCs = {self.n_PCs} computed, {time.time()-t0:0.2f}sec")    
             elif Usv is not None:
                 self.Usv = Usv
                 pc_time = 0
                 self.n_PCs = self.Usv.shape[1]
         self.sv = np.nansum((self.Usv**2), axis=0)**0.5
         if not hasattr(self, "Vsv"):
             if Vsv is None:
@@ -315,27 +365,27 @@
                 raise ValueError("""cannot rerun if n_splits > 0\n 
                                     need to set model.U_nodes = None first or \n 
                                     reset model = Rastermap(...) """)
         else:
             # run clustering
             self.n_clusters = min(self.Usv.shape[0]//2, self.n_clusters)
             U_nodes, imax = kmeans_func(self.Usv[igood], n_clusters=self.n_clusters)
-            print(f"{U_nodes.shape[0]} clusters computed, time {time.time() - t0:0.2f}")
+            print(f"{U_nodes.shape[0]} clusters computed, time {time.time() - t0:0.2f}sec")
 
         # compute correlation matrix across clusters
         if self.time_lag_window > 0:
             cc = compute_cc_tdelay(self.Vsv / self.sv, U_nodes, 
                                    time_lag_window=self.time_lag_window,
                                    symmetric=self.symmetric)
         else:
             cc = U_nodes @ U_nodes.T
 
         ### ---------------- sorting ----------------------------------------------- ###
         cc, inds = traveling_salesman(cc, verbose=self.verbose_sorting, 
-                                       locality=self.locality, circular=self.circular,
+                                       locality=self.locality,
                                         n_skip=None)[:2]
         U_nodes = U_nodes[inds]
         ineurons = (self.Usv[igood] @ U_nodes.T).argmax(axis=1)
         self.cc = cc
         Y_nodes = np.arange(0, U_nodes.shape[0])[:, np.newaxis]
 
         # split and recluster and sort
@@ -373,27 +423,27 @@
                 n_nodes = U_nodes_new.shape[0]
                 U_nodes = U_nodes_new.copy()
                 ineurons = ineurons_new.copy()
             if not self.sticky:
                 ineurons = (self.Usv[igood] @ U_nodes.T).argmax(axis=1)
             Y_nodes = np.arange(0, U_nodes.shape[0])[:, np.newaxis]
 
-        print(f"clusters sorted, time {time.time() - t0:0.2f}")
+        print(f"clusters sorted, time {time.time() - t0:0.2f}sec")
         
         ### ---------------- upsample ---------------------------------------------- ###
         self.n_clusters = U_nodes.shape[0]
         if self.grid_upsample > 0:
             self.n_X = int(self.n_clusters * max(2, self.grid_upsample))
             n_neighbors = max(min(8, self.n_clusters - 1), self.n_clusters // 5)
             e_neighbor = max(1, min(self.smoothness, n_neighbors - 1))
 
             Y, corr, g, Xrec = grid_upsampling(self.Usv[igood], U_nodes, Y_nodes, n_X=self.n_X,
                                             n_neighbors=n_neighbors,
                                             e_neighbor=e_neighbor)
-            print(f"clusters upsampled, time {time.time() - t0:0.2f}")
+            print(f"clusters upsampled, time {time.time() - t0:0.2f}sec")
         else:
             if len(U_nodes) == n_samples:
                 Y = np.zeros(n_samples, "int")
                 Y[inds] = np.arange(0, n_samples)
             else:
                 Y = np.zeros(n_samples, "int")
                 Y[ineurons.argsort()] = np.arange(0, n_samples)
@@ -406,26 +456,29 @@
         self.U_upsampled = Xrec.copy()
         self.embedding_valid = Y
         self.isort_valid = Y[:, 0].argsort()
 
         # convert cluster centers to time traces (not used in algorithm)
         Vnorm = (self.Vsv**2).sum(axis=1)**0.5
         self.X_nodes = U_nodes @ (self.Vsv / Vnorm[:, np.newaxis]).T
-        if data is not None:
-            self.X_upsampled = Xrec @ self.Vsv.T
+        # upsampled cluster centers in time (these are large so we won't keep them for now)
+        # if data is not None:
+        #     self.X_upsampled = Xrec @ (self.Vsv / Vnorm[:, np.newaxis]).T
         
         self.igood = igood
         self.embedding = np.nan * np.zeros((len(self.igood),1))
         self.embedding[igood] = self.embedding_valid
         self.isort = self.embedding[:,0].argsort()
         
         ### ----------- bin across embedding --------------------------------------- ###
         if data is not None and compute_X_embedding:
             if (bin_size==0 or n_samples < bin_size or 
                 (bin_size == 50 and n_samples < 1000)):
                 bin_size = max(1, n_samples // 500)
             self.X_embedding = zscore(bin1d(X[igood][self.isort], bin_size, axis=0), axis=1)
 
+        print(f"rastermap complete, time {time.time() - t0:0.2f}sec")
+
+        self.runtime = time.time() - t0
         self.pc_time = pc_time
-        self.map_time = time.time() - t0 - pc_time
 
         return self
```

### Comparing `rastermap-0.9.0/rastermap/sort.py` & `rastermap-0.9.1/rastermap/sort.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/rastermap/svd.py` & `rastermap-0.9.1/rastermap/svd.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/rastermap/upsample.py` & `rastermap-0.9.1/rastermap/upsample.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/rastermap.egg-info/SOURCES.txt` & `rastermap-0.9.1/rastermap.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 .style.yapf
 LICENSE
 README.md
 conftest.py
 setup.py
 tox.ini
 .github/workflows/test_and_deploy.yml
+notebooks/rastermap_largescale.ipynb
+notebooks/rastermap_singleneurons.ipynb
+notebooks/rastermap_widefield.ipynb
+notebooks/rastermap_zebrafish.ipynb
+notebooks/tutorial.ipynb
 paper/fig1.ipynb
 paper/fig1.py
 paper/fig2.ipynb
 paper/fig2.py
 paper/fig3.ipynb
 paper/fig3.py
 paper/fig4.ipynb
```

### Comparing `rastermap-0.9.0/setup.py` & `rastermap-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.0/tox.ini` & `rastermap-0.9.1/tox.ini`

 * *Files identical despite different names*


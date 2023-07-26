# Comparing `tmp/fabrictestbed-extensions-1.6.0b7.tar.gz` & `tmp/fabrictestbed-extensions-1.6.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-extensions-1.6.0b7.tar", last modified: Fri Jul 21 15:33:57 2023, max compression
+gzip compressed data, was "fabrictestbed-extensions-1.6.0b8.tar", last modified: Wed Jul 26 18:52:58 2023, max compression
```

## Comparing `fabrictestbed-extensions-1.6.0b7.tar` & `fabrictestbed-extensions-1.6.0b8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1025 2023-07-13 19:11:12.627401 fabrictestbed-extensions-1.6.0b7/.github/workflows/build.yml
--rw-r--r--   0        0        0     1727 2023-07-13 19:11:12.627648 fabrictestbed-extensions-1.6.0b7/.github/workflows/checks.yml
--rw-r--r--   0        0        0     2402 2023-07-13 19:11:12.627776 fabrictestbed-extensions-1.6.0b7/.github/workflows/test.yml
--rw-r--r--   0        0        0     1806 2023-07-13 19:11:12.627899 fabrictestbed-extensions-1.6.0b7/.gitignore
--rw-r--r--   0        0        0      666 2023-07-13 19:11:12.628010 fabrictestbed-extensions-1.6.0b7/.readthedocs.yaml
--rw-r--r--   0        0        0     3134 2023-07-13 19:11:12.628291 fabrictestbed-extensions-1.6.0b7/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2023-07-13 19:11:12.628702 fabrictestbed-extensions-1.6.0b7/LICENSE
--rw-r--r--   0        0        0     4093 2023-07-13 19:11:12.628878 fabrictestbed-extensions-1.6.0b7/README.md
--rw-r--r--   0        0        0      638 2023-07-13 19:11:12.629133 fabrictestbed-extensions-1.6.0b7/docs/Makefile
--rw-r--r--   0        0        0      799 2023-07-13 19:11:12.629318 fabrictestbed-extensions-1.6.0b7/docs/make.bat
--rw-r--r--   0        0        0     1996 2023-07-13 19:11:12.629573 fabrictestbed-extensions-1.6.0b7/docs/source/conf.py
--rw-r--r--   0        0        0     8968 2023-07-13 19:11:12.629746 fabrictestbed-extensions-1.6.0b7/docs/source/fablib.rst
--rw-r--r--   0        0        0     4470 2023-07-13 19:11:12.630094 fabrictestbed-extensions-1.6.0b7/docs/source/index.rst
--rw-r--r--   0        0        0      149 2023-07-21 15:33:44.204786 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/__init__.py
--rw-r--r--   0        0        0        2 2023-07-13 19:11:12.630706 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/editors/__init__.py
--rw-r--r--   0        0        0    18043 2023-07-13 19:11:12.630995 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/editors/abc_topology_editor.py
--rw-r--r--   0        0        0     6203 2023-07-13 19:11:12.631560 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
--rw-r--r--   0        0        0    68406 2023-07-13 19:11:12.631815 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/editors/geo_topology_editor.py
--rw-r--r--   0        0        0        1 2023-07-13 19:11:12.632118 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/__init__.py
--rw-r--r--   0        0        0     4793 2023-07-13 19:11:12.632370 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/abc_fablib.py
--rw-r--r--   0        0        0    21495 2023-07-13 19:11:12.633036 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/component.py
--rw-r--r--   0        0        0    77361 2023-07-13 19:11:12.634055 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/fablib.py
--rw-r--r--   0        0        0     5822 2023-07-13 19:11:12.634355 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/facility_port.py
--rw-r--r--   0        0        0    26310 2023-07-13 19:11:12.634666 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/interface.py
--rw-r--r--   0        0        0    40016 2023-07-13 19:11:12.635187 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/network_service.py
--rw-r--r--   0        0        0    96387 2023-07-13 19:11:12.635705 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/node.py
--rw-r--r--   0        0        0    38529 2023-07-13 19:11:12.636077 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/resources.py
--rw-r--r--   0        0        0    81759 2023-07-13 19:11:12.636971 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/slice.py
--rw-r--r--   0        0        0        2 2023-07-13 19:11:12.637479 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/images/__init__.py
--rw-r--r--   0        0        0   199914 2023-07-13 19:11:12.639231 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/images/fabric_logo.png
--rw-r--r--   0        0        0     1316 2023-07-13 19:11:12.639596 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/images/server.png
--rw-r--r--   0        0        0    62250 2023-07-13 19:11:12.639917 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/images/slice_rack.png
--rw-r--r--   0        0        0        2 2023-07-13 19:11:12.640209 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/utils/__init__.py
--rw-r--r--   0        0        0     3081 2023-07-13 19:11:12.640528 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/utils/abc_utils.py
--rw-r--r--   0        0        0     3304 2023-07-13 19:11:12.640718 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/utils/node.py
--rw-r--r--   0        0        0     8437 2023-07-13 19:11:12.640903 fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/utils/slice.py
--rw-r--r--   0        0        0     1585 2023-07-21 15:33:54.404314 fabrictestbed-extensions-1.6.0b7/pyproject.toml
--rwxr-xr-x   0        0        0      122 2023-07-13 19:11:12.641373 fabrictestbed-extensions-1.6.0b7/sphinx.sh
--rw-r--r--   0        0        0    13331 2023-07-13 19:11:12.641937 fabrictestbed-extensions-1.6.0b7/tests/benchmarks/gpu_tesla_t4_benchmark.py
--rw-r--r--   0        0        0    20582 2023-07-13 19:11:12.642271 fabrictestbed-extensions-1.6.0b7/tests/benchmarks/link_benchmark.py
--rw-r--r--   0        0        0    20886 2023-07-13 19:11:12.642664 fabrictestbed-extensions-1.6.0b7/tests/benchmarks/local_network_benchmark.py
--rw-r--r--   0        0        0    44920 2023-07-13 19:11:12.643280 fabrictestbed-extensions-1.6.0b7/tests/benchmarks/network_benchmark_tests.py
--rw-r--r--   0        0        0    10017 2023-07-13 19:11:12.643622 fabrictestbed-extensions-1.6.0b7/tests/benchmarks/nvme_benchmark.py
--rw-r--r--   0        0        0    14764 2023-07-13 19:11:12.643933 fabrictestbed-extensions-1.6.0b7/tests/integration/abc_test.py
--rw-r--r--   0        0        0    34368 2023-07-13 19:11:12.644201 fabrictestbed-extensions-1.6.0b7/tests/integration/component_tests.py
--rw-r--r--   0        0        0    10205 2023-07-13 19:11:12.644478 fabrictestbed-extensions-1.6.0b7/tests/integration/hello_fabric.py
--rw-r--r--   0        0        0        1 2023-07-13 19:11:12.644724 fabrictestbed-extensions-1.6.0b7/tests/unit/__init__.py
--rw-r--r--   0        0        0       85 2023-07-13 19:11:12.645011 fabrictestbed-extensions-1.6.0b7/tests/unit/data/dummy-token.json
--rw-r--r--   0        0        0     5095 2023-07-13 19:11:12.645235 fabrictestbed-extensions-1.6.0b7/tests/unit/test_basic.py
--rw-r--r--   0        0        0      398 2023-07-13 19:11:12.645487 fabrictestbed-extensions-1.6.0b7/tox.ini
--rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.6.0b7/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-07-13 19:11:12.627401 fabrictestbed-extensions-1.6.0b8/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1727 2023-07-13 19:11:12.627648 fabrictestbed-extensions-1.6.0b8/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     2402 2023-07-13 19:11:12.627776 fabrictestbed-extensions-1.6.0b8/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1839 2023-07-26 18:51:56.402517 fabrictestbed-extensions-1.6.0b8/.gitignore
+-rw-r--r--   0        0        0      666 2023-07-13 19:11:12.628010 fabrictestbed-extensions-1.6.0b8/.readthedocs.yaml
+-rw-r--r--   0        0        0     3918 2023-07-26 18:51:56.402734 fabrictestbed-extensions-1.6.0b8/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2023-07-13 19:11:12.628702 fabrictestbed-extensions-1.6.0b8/LICENSE
+-rw-r--r--   0        0        0     4509 2023-07-26 18:51:56.402940 fabrictestbed-extensions-1.6.0b8/README.md
+-rw-r--r--   0        0        0      638 2023-07-13 19:11:12.629133 fabrictestbed-extensions-1.6.0b8/docs/Makefile
+-rw-r--r--   0        0        0      799 2023-07-13 19:11:12.629318 fabrictestbed-extensions-1.6.0b8/docs/make.bat
+-rw-r--r--   0        0        0     1996 2023-07-13 19:11:12.629573 fabrictestbed-extensions-1.6.0b8/docs/source/conf.py
+-rw-r--r--   0        0        0     9045 2023-07-26 18:51:56.403389 fabrictestbed-extensions-1.6.0b8/docs/source/fablib.rst
+-rw-r--r--   0        0        0     4470 2023-07-13 19:11:12.630094 fabrictestbed-extensions-1.6.0b8/docs/source/index.rst
+-rw-r--r--   0        0        0      149 2023-07-26 18:52:18.640526 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/__init__.py
+-rw-r--r--   0        0        0        2 2023-07-13 19:11:12.630706 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/editors/__init__.py
+-rw-r--r--   0        0        0    18043 2023-07-13 19:11:12.630995 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/editors/abc_topology_editor.py
+-rw-r--r--   0        0        0     6203 2023-07-13 19:11:12.631560 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
+-rw-r--r--   0        0        0    68406 2023-07-13 19:11:12.631815 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/editors/geo_topology_editor.py
+-rw-r--r--   0        0        0        1 2023-07-13 19:11:12.632118 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/__init__.py
+-rw-r--r--   0        0        0    21495 2023-07-13 19:11:12.633036 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/component.py
+-rw-r--r--   0        0        0    78005 2023-07-26 18:51:56.405727 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/fablib.py
+-rw-r--r--   0        0        0     5822 2023-07-13 19:11:12.634355 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/facility_port.py
+-rw-r--r--   0        0        0    26951 2023-07-26 18:51:56.406253 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/interface.py
+-rw-r--r--   0        0        0    40016 2023-07-13 19:11:12.635187 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/network_service.py
+-rw-r--r--   0        0        0    97080 2023-07-26 18:51:56.406552 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/node.py
+-rw-r--r--   0        0        0    38529 2023-07-13 19:11:12.636077 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/resources.py
+-rw-r--r--   0        0        0    82338 2023-07-26 18:51:56.407041 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/slice.py
+-rw-r--r--   0        0        0        2 2023-07-13 19:11:12.637479 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/images/__init__.py
+-rw-r--r--   0        0        0   199914 2023-07-13 19:11:12.639231 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/images/fabric_logo.png
+-rw-r--r--   0        0        0     1316 2023-07-13 19:11:12.639596 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/images/server.png
+-rw-r--r--   0        0        0    62250 2023-07-13 19:11:12.639917 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/images/slice_rack.png
+-rw-r--r--   0        0        0        2 2023-07-13 19:11:12.640209 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/utils/__init__.py
+-rw-r--r--   0        0        0     3081 2023-07-13 19:11:12.640528 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/utils/abc_utils.py
+-rw-r--r--   0        0        0     3304 2023-07-13 19:11:12.640718 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/utils/node.py
+-rw-r--r--   0        0        0     8437 2023-07-13 19:11:12.640903 fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/utils/slice.py
+-rw-r--r--   0        0        0     1875 2023-07-26 18:52:31.086467 fabrictestbed-extensions-1.6.0b8/pyproject.toml
+-rwxr-xr-x   0        0        0      122 2023-07-13 19:11:12.641373 fabrictestbed-extensions-1.6.0b8/sphinx.sh
+-rw-r--r--   0        0        0    13331 2023-07-13 19:11:12.641937 fabrictestbed-extensions-1.6.0b8/tests/benchmarks/gpu_tesla_t4_benchmark.py
+-rw-r--r--   0        0        0    20582 2023-07-13 19:11:12.642271 fabrictestbed-extensions-1.6.0b8/tests/benchmarks/link_benchmark.py
+-rw-r--r--   0        0        0    20886 2023-07-13 19:11:12.642664 fabrictestbed-extensions-1.6.0b8/tests/benchmarks/local_network_benchmark.py
+-rw-r--r--   0        0        0    44920 2023-07-13 19:11:12.643280 fabrictestbed-extensions-1.6.0b8/tests/benchmarks/network_benchmark_tests.py
+-rw-r--r--   0        0        0    10017 2023-07-13 19:11:12.643622 fabrictestbed-extensions-1.6.0b8/tests/benchmarks/nvme_benchmark.py
+-rw-r--r--   0        0        0     6207 2023-07-26 18:51:56.407212 fabrictestbed-extensions-1.6.0b8/tests/integration/L2_reconfig_post_reboot_tests.py
+-rw-r--r--   0        0        0    14764 2023-07-13 19:11:12.643933 fabrictestbed-extensions-1.6.0b8/tests/integration/abc_test.py
+-rw-r--r--   0        0        0    34368 2023-07-13 19:11:12.644201 fabrictestbed-extensions-1.6.0b8/tests/integration/component_tests.py
+-rw-r--r--   0        0        0     2106 2023-07-26 18:51:56.407324 fabrictestbed-extensions-1.6.0b8/tests/integration/test_hello_fabric.py
+-rw-r--r--   0        0        0        1 2023-07-13 19:11:12.644724 fabrictestbed-extensions-1.6.0b8/tests/unit/__init__.py
+-rw-r--r--   0        0        0       85 2023-07-13 19:11:12.645011 fabrictestbed-extensions-1.6.0b8/tests/unit/data/dummy-token.json
+-rw-r--r--   0        0        0     5522 2023-07-26 18:51:56.407569 fabrictestbed-extensions-1.6.0b8/tests/unit/test_basic.py
+-rw-r--r--   0        0        0      397 2023-07-26 18:51:56.407797 fabrictestbed-extensions-1.6.0b8/tox.ini
+-rw-r--r--   0        0        0     5862 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.6.0b8/PKG-INFO
```

### Comparing `fabrictestbed-extensions-1.6.0b7/.github/workflows/build.yml` & `fabrictestbed-extensions-1.6.0b8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/.github/workflows/checks.yml` & `fabrictestbed-extensions-1.6.0b8/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/.github/workflows/test.yml` & `fabrictestbed-extensions-1.6.0b8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/.gitignore` & `fabrictestbed-extensions-1.6.0b8/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -124,7 +124,10 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 .idea/
+
+# Created by tox.
+/_trial_temp/
```

### Comparing `fabrictestbed-extensions-1.6.0b7/.readthedocs.yaml` & `fabrictestbed-extensions-1.6.0b8/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/LICENSE` & `fabrictestbed-extensions-1.6.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/README.md` & `fabrictestbed-extensions-1.6.0b8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -58,23 +58,41 @@
 ## Contributing to FABlib
 
 Contributions to FABlib are made with GitHub Pull Requests. When you
 submit a pull request, some tests will run against it:
 
 - Code formatting will be checked using [black] and [isort].  Be sure
   that your code is formatted with these tools.
-- CHANGELOG.md will be checked for updates.
-- Packages will be built.
 - Unit tests will be run.
+- Packages will be built.
+- CHANGELOG.md will be checked for updates.
 
-You can run tests in your environment, like so, using [pytest]:
+
+## Testing FABlib
+
+FABlib currently has a modest set of unit and integration tests, under
+the top-level `tests` directory.  Unit tests can be run like so, using
+[tox]:
 
 ```console
 $ pip install -e .[test]
-$ pytest
+$ tox
+```
+
+Integration tests can be run like so:
+
+```console
+$ tox -e integration
+```
+
+Tox attempts to run tests in an isolated virtual environment.  If you
+want to run some tests directly using [pytest], that is possible too:
+
+```
+$ pytest -s tests/integration/test_hello_fabric.py
 ```
 
 ## Packaging FABlib
 
 FABlib uses [flit] as the build backend.  To build source and wheel
 packages, do this:
 
@@ -133,10 +151,11 @@
 [fablib-api-rtd]: https://fabric-fablib.readthedocs.io/en/latest/
 [fablib-api-old]: https://learn.fabric-testbed.net/docs/fablib/fablib.html
 
 [flit]: https://flit.pypa.io/en/stable/
 [package uploads]: https://flit.pypa.io/en/latest/upload.html
 
 [build]: https://pypi.org/project/build/
+[tox]: https://pypi.org/project/tox/
 [pytest]: https://pypi.org/project/pytest/
 [black]: https://pypi.org/project/black/
 [isort]: https://pypi.org/project/isort/
```

### Comparing `fabrictestbed-extensions-1.6.0b7/docs/Makefile` & `fabrictestbed-extensions-1.6.0b8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/docs/make.bat` & `fabrictestbed-extensions-1.6.0b8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/docs/source/conf.py` & `fabrictestbed-extensions-1.6.0b8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/docs/source/fablib.rst` & `fabrictestbed-extensions-1.6.0b8/docs/source/fablib.rst`

 * *Files 1% similar despite different names*

```diff
@@ -335,14 +335,16 @@
 
  .. automethod:: ping_test
 
  .. automethod:: get_storage
 
  .. automethod:: add_storage
 
+ .. automethod:: un_manage_interface
+
 
 .. automodule:: component
 
 ``Component``
 ----------------------------
 
 .. autoclass:: component.Component
@@ -451,14 +453,16 @@
 
   .. automethod::  get_ip_addr
 
   .. automethod::  get_ips
 
   .. automethod:: get_numa_node
 
+  .. automethod:: un_manage_interface
+
 .. automodule:: network_service
 
 
 ``NetworkService``
 ------------------------------------
 
 .. autoclass:: network_service.NetworkService
```

### Comparing `fabrictestbed-extensions-1.6.0b7/docs/source/index.rst` & `fabrictestbed-extensions-1.6.0b8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/editors/abc_topology_editor.py` & `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/editors/abc_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/editors/cytoscape_topology_editor.py` & `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/editors/cytoscape_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/editors/geo_topology_editor.py` & `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/editors/geo_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/component.py` & `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/component.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/fablib.py` & `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/fablib.py`

 * *Files 1% similar despite different names*

```diff
@@ -992,24 +992,28 @@
         :rtype: list[str]
         """
         return [
             "default_centos8_stream",
             "default_centos9_stream",
             "default_centos_7",
             "default_centos_8",
-            "default_cirros",
             "default_debian_10",
+            "default_debian_11",
             "default_fedora_35",
-            "default_freebsd_13_zfs",
-            "default_openbsd_7",
             "default_rocky_8",
+            "default_rocky_9",
             "default_ubuntu_18",
             "default_ubuntu_20",
             "default_ubuntu_21",
             "default_ubuntu_22",
+            "default_fedora_36",
+            "default_fedora_37",
+            "docker_rocky_8",
+            "docker_ubuntu_20",
+            "docker_ubuntu_22",
         ]
 
     def get_site_names(self) -> List[str]:
         """
         Gets a list of all available site names.
 
         :return: list of site names as strings
@@ -1590,14 +1594,24 @@
         Gets the FABRIC Bastion key filename.
 
         :return: FABRIC Bastion key filename
         :rtype: String
         """
         return self.bastion_key_filename
 
+    def get_bastion_key(self) -> str:
+        """
+        Reads the FABRIC Bastion private key file and returns the key.
+
+        :return: FABRIC Bastion key string
+        :rtype: String
+        """
+        with open(self.bastion_key_filename, "r", encoding="utf-8") as f:
+            return f.read()
+
     def get_bastion_public_addr(self) -> str:
         """
         Gets the FABRIC Bastion host address.
 
         :return: Bastion host public address
         :rtype: String
         """
@@ -1924,15 +1938,20 @@
                 raise Exception(f"More than 1 slice found with slice_id: {slice_id}")
         elif name:
             # if getting by name then only consider active slices
             slices = self.get_slices(
                 excludes=[SliceState.Dead, SliceState.Closing], slice_name=name
             )
 
-            return slices[0]
+            if len(slices) > 0:
+                return slices[0]
+            else:
+                raise Exception(
+                    f'Unable to find slice "{name}" for this project. Check slice name spelling and project id.'
+                )
         else:
             raise Exception(
                 "get_slice requires slice name (name) or slice id (slice_id)"
             )
 
     def delete_slice(self, slice_name: str = None):
         """
```

### Comparing `fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/facility_port.py` & `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/facility_port.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/interface.py` & `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,21 @@
     from fabrictestbed_extensions.fablib.component import Component
 
 from fabrictestbed.slice_editor import UserData
 from fim.user.interface import Interface as FimInterface
 
 
 class Interface:
+    CONFIGURED = "configured"
+    MODE = "mode"
+    AUTO = "auto"
+    MANUAL = "manual"
+    ADDR = "addr"
+    CONFIG = "config"
+
     def __init__(self, component: Component = None, fim_interface: FimInterface = None):
         """
         Constructor. Sets keyword arguments as instance fields.
 
         :param component: the component to set on this interface
         :type component: Component
         :param fim_interface: the FABRIC information model interface to set on this fablib interface
@@ -461,14 +468,25 @@
         """
         Toggle the dev down then up.
 
         """
         self.get_node().ip_link_down(None, self)
         self.get_node().ip_link_up(None, self)
 
+    def un_manage_interface(self):
+        """
+        Mark an interface unmanaged by Network Manager;
+        This is needed to be run on rocky* images to avoid the
+        network configuration from being overwritten by NetworkManager
+        """
+        if self.get_network() is None:
+            return
+
+        self.get_node().un_manage_interface(self)
+
     def set_vlan(self, vlan: Any = None):
         """
         Set the VLAN on the FABRIC request.
 
         :param addr: vlan
         :type addr: String or int
         """
@@ -781,94 +799,98 @@
         network.add_interface(self)
 
         return self
 
     def set_ip_addr(self, addr: ipaddress = None, mode: str = None):
         fablib_data = self.get_fablib_data()
         if mode:
-            fablib_data["mode"] = str(mode)
+            fablib_data[self.MODE] = str(mode)
 
-        mode = fablib_data["mode"]
+        mode = fablib_data[self.MODE]
         if addr:
-            fablib_data["addr"] = str(self.get_network().allocate_ip(addr))
-        elif mode == "auto":
+            fablib_data[self.ADDR] = str(self.get_network().allocate_ip(addr))
+        elif mode == self.AUTO:
             if self.get_network():
-                fablib_data["addr"] = str(self.get_network().allocate_ip())
+                fablib_data[self.ADDR] = str(self.get_network().allocate_ip())
         self.set_fablib_data(fablib_data)
 
         return self
 
     def get_ip_addr(self):
         fablib_data = self.get_fablib_data()
-        if "addr" in fablib_data:
+        if self.ADDR in fablib_data:
             try:
-                addr = ipaddress.ip_address(fablib_data["addr"])
+                addr = ipaddress.ip_address(fablib_data[self.ADDR])
             except:
-                addr = fablib_data["addr"]
+                addr = fablib_data[self.ADDR]
             return addr
         else:
             # get_ip_addr_ssh()
             if self.get_mac() is None:
                 return None
             return self.get_ip_addr_ssh()
 
     def set_mode(self, mode: str = "config"):
         fablib_data = self.get_fablib_data()
-        fablib_data["mode"] = mode
+        fablib_data[self.MODE] = mode
         self.set_fablib_data(fablib_data)
 
         return self
 
     def get_mode(self):
         fablib_data = self.get_fablib_data()
-        if "mode" not in fablib_data:
-            self.set_mode("config")
+        if self.MODE not in fablib_data:
+            self.set_mode(self.CONFIG)
             fablib_data = self.get_fablib_data()
 
-        return fablib_data["mode"]
+        return fablib_data[self.MODE]
+
+    def is_configured(self):
+        fablib_data = self.get_fablib_data()
+        is_configured = fablib_data.get(self.CONFIGURED)
+        if is_configured is None or not bool(is_configured):
+            return False
+
+        return True
 
     def config(self):
         network = self.get_network()
         if not network:
             logging.info(
                 f"interface {self.get_name()} not connected to network, skipping config."
             )
             return
 
         fablib_data = self.get_fablib_data()
-        if "configured" in fablib_data and bool(fablib_data["configured"]):
-            logging.debug(
-                f"interface {self.get_name()} already configured, skipping config."
-            )
-            return
+        addr = None
+        if self.is_configured():
+            addr = fablib_data.get(self.ADDR)
         else:
-            logging.debug(f"interface {self.get_name()} not configured, configuring.")
-
-        fablib_data["configured"] = str(True)
-        self.set_fablib_data(fablib_data)
+            fablib_data[self.CONFIGURED] = str(True)
+            self.set_fablib_data(fablib_data)
 
-        if "mode" in fablib_data:
-            mode = fablib_data["mode"]
+        if self.MODE in fablib_data:
+            mode = fablib_data[self.MODE]
         else:
-            mode = "manual"
-
-        if mode == "auto":
-            fablib_data["addr"] = str(self.get_network().allocate_ip())
-            addr = fablib_data["addr"]
+            mode = self.MANUAL
 
+        if mode == self.AUTO and addr is None:
+            fablib_data[self.ADDR] = str(self.get_network().allocate_ip())
+            # addr = fablib_data[self.ADDR]
             # print(f"auto allocated addr: {addr}")
 
             self.set_fablib_data(fablib_data)
 
-        if mode == "config" or mode == "auto":
+        if mode == self.CONFIG or mode == self.AUTO:
             subnet = self.get_network().get_subnet()
-            if "addr" in fablib_data:
-                addr = fablib_data["addr"]
-                if addr and subnet:
-                    self.ip_addr_add(addr=addr, subnet=ipaddress.ip_network(subnet))
+            addr = fablib_data.get(self.ADDR)
+            if addr and subnet:
+                self.un_manage_interface()
+                self.ip_link_up()
+                self.ip_addr_add(addr=addr, subnet=ipaddress.ip_network(subnet))
         else:
             # manual mode... do nothing
             pass
 
     def add_mirror(self, port_name: str, name: str = "mirror"):
         self.get_slice().get_fim_topology().add_port_mirror_service(
             name=name,
```

### Comparing `fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/network_service.py` & `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/network_service.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/node.py` & `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -2162,14 +2162,34 @@
                 f"{ip_command} addr del {addr}/{subnet.prefixlen} dev {interface.get_device_name()} ",
                 quiet=True,
             )
         except Exception as e:
             logging.warning(f"Failed to del addr: {e}")
             raise e
 
+    def un_manage_interface(self, interface: Interface):
+        """
+        Mark an interface unmanaged by Network Manager;
+        This is needed to be run on rocky* images to avoid the
+        network configuration from being overwritten by NetworkManager
+        :param interface: the FABlib interface.
+        :type interface: Interface
+        """
+
+        if interface is None:
+            return
+
+        try:
+            self.execute(
+                f"sudo nmcli dev set {interface.get_physical_os_interface_name()} managed no",
+                quiet=True,
+            )
+        except Exception as e:
+            logging.warning(f"Failed to mark interface as unmanaged: {e}")
+
     def ip_link_up(self, subnet: Union[IPv4Network, IPv6Network], interface: Interface):
         """
         Bring up a link on an interface on the node.
         :param subnet: subnet.
         :type subnet: IPv4Network or IPv6Network
         :param interface: the FABlib interface.
         :type interface: Interface
@@ -2197,15 +2217,15 @@
                 ip_command = "sudo ip"
         except Exception as e:
             logging.warning(f"Failed to down link: {e}")
             return
 
         try:
             self.execute(
-                f"{ip_command} link set dev {interface.get_physical_os_interface()} up",
+                f"{ip_command} link set dev {interface.get_physical_os_interface_name()} up",
                 quiet=True,
             )
         except Exception as e:
             logging.warning(f"Failed to up link: {e}")
             raise e
 
         try:
```

### Comparing `fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/resources.py` & `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/resources.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/fablib/slice.py` & `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/fablib/slice.py`

 * *Files 1% similar despite different names*

```diff
@@ -705,14 +705,24 @@
         :rtype: String
         """
         if "slice_public_key_file" in self.slice_key.keys():
             return self.slice_key["slice_public_key_file"]
         else:
             return None
 
+    def get_slice_public_key(self) -> str:
+        """
+        Gets the string representing the slice public key.
+
+        :return: public key
+        :rtype: String
+        """
+        with open(self.get_slice_public_key_file(), "r", encoding="utf-8") as f:
+            return f.read()
+
     def get_slice_private_key_file(self) -> str:
         """
         Gets the path to the slice private key file.
 
         Important! Slice key management is underdevelopment and this
         functionality will likely change going forward.
 
@@ -720,14 +730,24 @@
         :rtype: String
         """
         if "slice_private_key_file" in self.slice_key.keys():
             return self.slice_key["slice_private_key_file"]
         else:
             return None
 
+    def get_slice_private_key(self) -> str:
+        """
+        Gets the string representing the slice private key.
+
+        :return: public key
+        :rtype: String
+        """
+        with open(self.get_slice_private_key_file(), "r", encoding="utf-8") as f:
+            return f.read()
+
     def is_dead_or_closing(self):
         if self.get_state() in ["Closing", "Dead"]:
             return True
         else:
             return False
 
     def isStable(self) -> bool:
@@ -1667,15 +1687,15 @@
         for net in self.get_networks():
             if net.get_type() in ["FABNetv4", "FABNetv6", "FABNetv4Ext", "FABNetv6Ext"]:
                 try:
                     if (
                         not type(net.get_subnet())
                         in [ipaddress.IPv4Network, ipaddress.IPv6Network]
                         or not type(net.get_gateway())
-                        in [ipaddress.IPv4Address, ipaddress.IPv46ddress]
+                        in [ipaddress.IPv4Address, ipaddress.IPv6Address]
                         or net.get_available_ips() == None
                     ):
                         logging.warning(
                             f"slice not ready: net {net.get_name()}, subnet: {net.get_subnet()}, available_ips: {net.get_available_ips()}"
                         )
 
                         return False
```

### Comparing `fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/images/fabric_logo.png` & `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/images/fabric_logo.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/images/server.png` & `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/images/server.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/images/slice_rack.png` & `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/images/slice_rack.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/utils/abc_utils.py` & `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/utils/abc_utils.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/utils/node.py` & `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/utils/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/fabrictestbed_extensions/utils/slice.py` & `fabrictestbed-extensions-1.6.0b8/fabrictestbed_extensions/utils/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/pyproject.toml` & `fabrictestbed-extensions-1.6.0b8/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 requires-python = ">=3.9"
 dependencies = [
     "ipycytoscape",
     "ipywidgets",
     "ipyleaflet",
     "ipycytoscape",
     "tabulate",
-    "fabrictestbed==1.6.0b6",
+    "fabrictestbed==1.6.0b7",
     "paramiko",
     "jinja2>=3.0.0",
     "pandas",
     "numpy",
     "ipython>=8.12.0"
     ]
 
@@ -42,21 +42,32 @@
 ChangeLog = "https://github.com/fabric-testbed/fabrictestbed-extensions/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 doc = ["sphinx", "furo"]
 test = [
     "black==23.*",
     "isort==5.*",
+    "tox==4.*",
     "pytest",
     "coverage[toml]"
     ]
 
 [tool.coverage.run]
 branch = true
 omit = [ "fabrictestbed_extensions/tests/*" ]
 
 [tool.black]
 src_paths = ["fabrictestbed_extensions", "docs/source/conf.py", "tests"]
 
 [tool.isort]
 profile = "black"
 src_paths = ["fabrictestbed_extensions", "docs/source/conf.py", "tests"]
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+addopts = "-ra -q"
+# By default, run only unit tests when pytest is invoked.  Integration
+# tests will require some manual setup (namely token acquisition), and
+# thus we can't run them on CI.
+testpaths = [
+    "tests/unit/",
+]
```

### Comparing `fabrictestbed-extensions-1.6.0b7/tests/benchmarks/gpu_tesla_t4_benchmark.py` & `fabrictestbed-extensions-1.6.0b8/tests/benchmarks/gpu_tesla_t4_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/tests/benchmarks/link_benchmark.py` & `fabrictestbed-extensions-1.6.0b8/tests/benchmarks/link_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/tests/benchmarks/local_network_benchmark.py` & `fabrictestbed-extensions-1.6.0b8/tests/benchmarks/local_network_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/tests/benchmarks/network_benchmark_tests.py` & `fabrictestbed-extensions-1.6.0b8/tests/benchmarks/network_benchmark_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/tests/benchmarks/nvme_benchmark.py` & `fabrictestbed-extensions-1.6.0b8/tests/benchmarks/nvme_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/tests/integration/abc_test.py` & `fabrictestbed-extensions-1.6.0b8/tests/integration/abc_test.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/tests/integration/component_tests.py` & `fabrictestbed-extensions-1.6.0b8/tests/integration/component_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.6.0b7/tests/unit/test_basic.py` & `fabrictestbed-extensions-1.6.0b8/tests/unit/test_basic.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,69 +26,71 @@
         FablibManager.FABRIC_BASTION_KEY_LOCATION,
     ]
 
     def setUp(self):
         # Run each test with an empty environment.
         os.environ.clear()
 
+        # Create an empty configuration file, so that we will be
+        # really testing with a clean slate.  Creating the
+        # configuration file in read-only mode should ensure that it
+        # will remain empty.
+        self.rcfile = tempfile.NamedTemporaryFile(mode="r")
+        self.rcfile.flush()
+
+    def tearDown(self):
+        self.rcfile.close()
+
     def test_fablib_manager_no_env_vars(self):
         # Test with no required env vars set.
-        with self.assertRaises(AttributeError):
-            FablibManager()
+        self.assertRaises(AttributeError, FablibManager, fabric_rc=self.rcfile.name)
 
     def test_fablib_manager_one_env_var(self):
         # Test with some required env vars set.
         for var in self.required_env_vars:
-            with self.assertRaises(AttributeError):
-                os.environ[var] = "dummy"
-                FablibManager()
+            os.environ[var] = "dummy"
+            self.assertRaises(AttributeError, FablibManager, fabric_rc=self.rcfile.name)
 
     def test_fablib_manager_all_env_vars(self):
         # Test with all required configuration except
         # FABRIC_TOKEN_LOCATION.
         for var in self.required_env_vars:
             os.environ[var] = "dummy"
 
-        with self.assertRaises(AttributeError):
-            FablibManager()
+        self.assertRaises(AttributeError, FablibManager, fabric_rc=self.rcfile.name)
 
     def test_fablib_manager_test_only_cm_host(self):
-        with self.assertRaises(AttributeError):
-            os.environ[Constants.FABRIC_CREDMGR_HOST] = "dummy"
-            FablibManager()
+        os.environ[Constants.FABRIC_CREDMGR_HOST] = "dummy"
+        self.assertRaises(AttributeError, FablibManager, fabric_rc=self.rcfile.name)
 
     def test_fablib_manager_test_only_orchestrator_host(self):
-        with self.assertRaises(AttributeError):
-            os.environ[Constants.FABRIC_ORCHESTRATOR_HOST] = "dummy"
-            FablibManager()
+        os.environ[Constants.FABRIC_ORCHESTRATOR_HOST] = "dummy"
+        self.assertRaises(AttributeError, FablibManager, fabric_rc=self.rcfile.name)
 
     def test_fablib_manager_test_only_project_id(self):
-        with self.assertRaises(AttributeError):
-            os.environ[Constants.FABRIC_PROJECT_ID] = "dummy"
-            FablibManager()
+        os.environ[Constants.FABRIC_PROJECT_ID] = "dummy"
+        self.assertRaises(AttributeError, FablibManager, fabric_rc=self.rcfile.name)
 
     def test_fablib_manager_test_only_token_location(self):
-        with self.assertRaises(AttributeError):
-            os.environ[Constants.FABRIC_TOKEN_LOCATION] = "dummy"
-            FablibManager()
+        os.environ[Constants.FABRIC_TOKEN_LOCATION] = "dummy"
+        self.assertRaises(AttributeError, FablibManager, fabric_rc=self.rcfile.name)
 
     def test_fablib_manager_test_with_no_token_file(self):
         # Should fail when token location is not a valid path.
 
         # set all required env vars.
         for var in self.required_env_vars:
             os.environ[var] = "dummy"
 
         os.environ[Constants.FABRIC_TOKEN_LOCATION] = "dummy"
 
         # FablibManager() without a valid token or token location
         # should raise a "ValueError: Invalid value for
         # `refresh_token`, must not be `None`"
-        with self.assertRaises(ValueError):
-            FablibManager()
+        self.assertRaises(ValueError, FablibManager, fabric_rc=self.rcfile.name)
 
     def test_fablib_manager_test_with_dummy_token(self):
         # TODO: That FablibManager() calls build_slice_manager()
         # complicates writing a test for it.  It eventually makes a
         # network call to credential manager API, but it is not right
         # for a unit test to do such a thing.  We could probably
         # somehow mock a CM here?
@@ -96,19 +98,18 @@
         # set all required env vars.
         for var in self.required_env_vars:
             os.environ[var] = "dummy"
 
         # '.invalid' is an invalid host per RFC 6761, so this test
         # must fail without ever making a successful network call.
         os.environ[Constants.FABRIC_CREDMGR_HOST] = ".invalid"
-        path = os.path.join(os.path.dirname(__file__), "dummy-token.json")
-        os.environ[Constants.FABRIC_TOKEN_LOCATION] = path
+        path = pathlib.Path(__file__).parent / "data" / "dummy-token.json"
+        os.environ[Constants.FABRIC_TOKEN_LOCATION] = f"{path}"
 
-        with self.assertRaises(Exception):
-            FablibManager()
+        self.assertRaises(ValueError, FablibManager, fabric_rc=self.rcfile.name)
 
     def test_fablib_manager_with_empty_config(self):
         # Check that an empty configuration file will cause
         # FablibManager to raise an error.
         rcfile = tempfile.NamedTemporaryFile()
         rcfile.flush()
```

### Comparing `fabrictestbed-extensions-1.6.0b7/PKG-INFO` & `fabrictestbed-extensions-1.6.0b8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-extensions
-Version: 1.6.0b7
+Version: 1.6.0b8
 Summary: FABRIC Python Client Library and CLI Extensions
 Author-email: Paul Ruth <pruth@renci.org>, Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: ipycytoscape
 Requires-Dist: ipywidgets
 Requires-Dist: ipyleaflet
 Requires-Dist: ipycytoscape
 Requires-Dist: tabulate
-Requires-Dist: fabrictestbed==1.6.0b6
+Requires-Dist: fabrictestbed==1.6.0b7
 Requires-Dist: paramiko
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: ipython>=8.12.0
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: furo ; extra == "doc"
 Requires-Dist: black==23.* ; extra == "test"
 Requires-Dist: isort==5.* ; extra == "test"
+Requires-Dist: tox==4.* ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: coverage[toml] ; extra == "test"
 Project-URL: ChangeLog, https://github.com/fabric-testbed/fabrictestbed-extensions/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://fabric-fablib.readthedocs.io/
 Project-URL: Homepage, https://fabric-testbed.net/
 Project-URL: Sources, https://github.com/fabric-testbed/fabrictestbed-extensions
 Provides-Extra: doc
@@ -92,23 +93,41 @@
 ## Contributing to FABlib
 
 Contributions to FABlib are made with GitHub Pull Requests. When you
 submit a pull request, some tests will run against it:
 
 - Code formatting will be checked using [black] and [isort].  Be sure
   that your code is formatted with these tools.
-- CHANGELOG.md will be checked for updates.
-- Packages will be built.
 - Unit tests will be run.
+- Packages will be built.
+- CHANGELOG.md will be checked for updates.
 
-You can run tests in your environment, like so, using [pytest]:
+
+## Testing FABlib
+
+FABlib currently has a modest set of unit and integration tests, under
+the top-level `tests` directory.  Unit tests can be run like so, using
+[tox]:
 
 ```console
 $ pip install -e .[test]
-$ pytest
+$ tox
+```
+
+Integration tests can be run like so:
+
+```console
+$ tox -e integration
+```
+
+Tox attempts to run tests in an isolated virtual environment.  If you
+want to run some tests directly using [pytest], that is possible too:
+
+```
+$ pytest -s tests/integration/test_hello_fabric.py
 ```
 
 ## Packaging FABlib
 
 FABlib uses [flit] as the build backend.  To build source and wheel
 packages, do this:
 
@@ -167,11 +186,12 @@
 [fablib-api-rtd]: https://fabric-fablib.readthedocs.io/en/latest/
 [fablib-api-old]: https://learn.fabric-testbed.net/docs/fablib/fablib.html
 
 [flit]: https://flit.pypa.io/en/stable/
 [package uploads]: https://flit.pypa.io/en/latest/upload.html
 
 [build]: https://pypi.org/project/build/
+[tox]: https://pypi.org/project/tox/
 [pytest]: https://pypi.org/project/pytest/
 [black]: https://pypi.org/project/black/
 [isort]: https://pypi.org/project/isort/
```


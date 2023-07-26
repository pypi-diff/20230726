# Comparing `tmp/fastsweep-0.1.2.tar.gz` & `tmp/fastsweep-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastsweep-0.1.2.tar", last modified: Thu May 11 18:05:18 2023, max compression
+gzip compressed data, was "fastsweep-0.1.3.tar", last modified: Wed Jul 26 20:21:53 2023, max compression
```

## Comparing `fastsweep-0.1.2.tar` & `fastsweep-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.428388 fastsweep-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-11 18:05:06.000000 fastsweep-0.1.2/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.424388 fastsweep-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.424388 fastsweep-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-11 18:05:06.000000 fastsweep-0.1.2/.github/workflows/macOS_arm64_toolchain.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     2493 2023-05-11 18:05:06.000000 fastsweep-0.1.2/.github/workflows/tag_wheel_manylinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-11 18:05:06.000000 fastsweep-0.1.2/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-11 18:05:06.000000 fastsweep-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:06.000000 fastsweep-0.1.2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-11 18:05:06.000000 fastsweep-0.1.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-11 18:05:06.000000 fastsweep-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-05-11 18:05:18.428388 fastsweep-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-11 18:05:06.000000 fastsweep-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.424388 fastsweep-0.1.2/cmake-defaults/
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-05-11 18:05:06.000000 fastsweep-0.1.2/cmake-defaults/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.428388 fastsweep-0.1.2/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-11 18:05:06.000000 fastsweep-0.1.2/kernels/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-11 18:05:06.000000 fastsweep-0.1.2/kernels/cuda_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    30671 2023-05-11 18:05:06.000000 fastsweep-0.1.2/kernels/cuda_kernels.h
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-05-11 18:05:06.000000 fastsweep-0.1.2/kernels/cuda_kernels.ptx
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-11 18:05:06.000000 fastsweep-0.1.2/kernels/vec.h
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-11 18:05:06.000000 fastsweep-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.428388 fastsweep-0.1.2/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-11 18:05:06.000000 fastsweep-0.1.2/python/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-05-11 18:05:06.000000 fastsweep-0.1.2/python/pure_python_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    39945 2023-05-11 18:05:06.000000 fastsweep-0.1.2/redistancing.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:05:18.428388 fastsweep-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-11 18:05:06.000000 fastsweep-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.428388 fastsweep-0.1.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-11 18:05:06.000000 fastsweep-0.1.2/src/cuda_helpers.h
--rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-05-11 18:05:06.000000 fastsweep-0.1.2/src/distance_marcher.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-11 18:05:06.000000 fastsweep-0.1.2/src/distance_marcher.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.428388 fastsweep-0.1.2/src/fastsweep/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-11 18:05:06.000000 fastsweep-0.1.2/src/fastsweep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.428388 fastsweep-0.1.2/src/fastsweep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-05-11 18:05:18.000000 fastsweep-0.1.2/src/fastsweep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-11 18:05:18.000000 fastsweep-0.1.2/src/fastsweep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:05:18.000000 fastsweep-0.1.2/src/fastsweep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 18:05:18.000000 fastsweep-0.1.2/src/fastsweep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 18:05:18.000000 fastsweep-0.1.2/src/fastsweep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-11 18:05:06.000000 fastsweep-0.1.2/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:05:18.428388 fastsweep-0.1.2/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-11 18:05:06.000000 fastsweep-0.1.2/src/tests/test_redistancing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:21:53.263479 fastsweep-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-26 20:21:42.000000 fastsweep-0.1.3/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:21:53.251479 fastsweep-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:21:53.255479 fastsweep-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-26 20:21:42.000000 fastsweep-0.1.3/.github/workflows/macOS_arm64_toolchain.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2493 2023-07-26 20:21:42.000000 fastsweep-0.1.3/.github/workflows/tag_wheel_manylinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-26 20:21:42.000000 fastsweep-0.1.3/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-26 20:21:42.000000 fastsweep-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:21:42.000000 fastsweep-0.1.3/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-26 20:21:42.000000 fastsweep-0.1.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-26 20:21:42.000000 fastsweep-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-26 20:21:53.263479 fastsweep-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-26 20:21:42.000000 fastsweep-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:21:53.255479 fastsweep-0.1.3/cmake-defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-07-26 20:21:42.000000 fastsweep-0.1.3/cmake-defaults/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:21:53.259479 fastsweep-0.1.3/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-26 20:21:42.000000 fastsweep-0.1.3/kernels/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-26 20:21:42.000000 fastsweep-0.1.3/kernels/cuda_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    30671 2023-07-26 20:21:42.000000 fastsweep-0.1.3/kernels/cuda_kernels.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-26 20:21:42.000000 fastsweep-0.1.3/kernels/cuda_kernels.ptx
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-26 20:21:42.000000 fastsweep-0.1.3/kernels/vec.h
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-26 20:21:42.000000 fastsweep-0.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:21:53.259479 fastsweep-0.1.3/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-26 20:21:42.000000 fastsweep-0.1.3/python/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-07-26 20:21:42.000000 fastsweep-0.1.3/python/pure_python_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39945 2023-07-26 20:21:42.000000 fastsweep-0.1.3/redistancing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 20:21:53.263479 fastsweep-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-26 20:21:42.000000 fastsweep-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:21:53.259479 fastsweep-0.1.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-26 20:21:42.000000 fastsweep-0.1.3/src/cuda_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-07-26 20:21:42.000000 fastsweep-0.1.3/src/distance_marcher.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-26 20:21:42.000000 fastsweep-0.1.3/src/distance_marcher.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:21:53.259479 fastsweep-0.1.3/src/fastsweep/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-26 20:21:42.000000 fastsweep-0.1.3/src/fastsweep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:21:53.263479 fastsweep-0.1.3/src/fastsweep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-26 20:21:53.000000 fastsweep-0.1.3/src/fastsweep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-26 20:21:53.000000 fastsweep-0.1.3/src/fastsweep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:21:53.000000 fastsweep-0.1.3/src/fastsweep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 20:21:53.000000 fastsweep-0.1.3/src/fastsweep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 20:21:53.000000 fastsweep-0.1.3/src/fastsweep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-26 20:21:42.000000 fastsweep-0.1.3/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:21:53.263479 fastsweep-0.1.3/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-26 20:21:42.000000 fastsweep-0.1.3/src/tests/test_redistancing.py
```

### Comparing `fastsweep-0.1.2/.clang-format` & `fastsweep-0.1.3/.clang-format`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.2/.github/workflows/tag_wheel_manylinux.py` & `fastsweep-0.1.3/.github/workflows/tag_wheel_manylinux.py`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.2/.github/workflows/wheels.yml` & `fastsweep-0.1.3/.github/workflows/wheels.yml`

 * *Files 2% similar despite different names*

```diff
@@ -60,25 +60,25 @@
     - uses: actions/checkout@v3
       with:
         submodules: recursive
 
     - uses: actions/setup-python@v4
       name: Install Python
       with:
-        python-version: '3.8'
+        python-version: '3.10'
 
     - name: Prepare compiler environment for Windows
       if: runner.os == 'Windows'
       uses: ilammy/msvc-dev-cmd@v1
       with:
         arch: x64
 
     - name: Install cibuildwheel
       run: |
-        python -m pip install cibuildwheel==2.8.1
+        python -m pip install cibuildwheel==2.11.2
 
     - name: Prepare cibuildwheel environment for macOS
       if: runner.os == 'macOS'
       run: |
         [[ "arm64" == "${{ matrix.cibw-arch }}" ]] && \
         echo "FASTSWEEP_CMAKE_TOOLCHAIN_FILE=$(pwd)/.github/workflows/macOS_arm64_toolchain.cmake" >> $GITHUB_ENV && \
         echo "CIBW_BEFORE_BUILD_MACOS=\
```

### Comparing `fastsweep-0.1.2/.gitignore` & `fastsweep-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.2/CMakeLists.txt` & `fastsweep-0.1.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.2/LICENSE` & `fastsweep-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.2/PKG-INFO` & `fastsweep-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastsweep
-Version: 0.1.2
+Version: 0.1.3
 Summary: Eikonal solver using parallel fast sweeping
 Home-page: https://github.com/rgl-epfl/fastsweep
 Author: Delio Vicini
 Author-email: delio.vicini@gmail.com
 License: BSD
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `fastsweep-0.1.2/README.md` & `fastsweep-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.2/cmake-defaults/CMakeLists.txt` & `fastsweep-0.1.3/cmake-defaults/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.2/kernels/cuda_kernels.cu` & `fastsweep-0.1.3/kernels/cuda_kernels.cu`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.2/kernels/cuda_kernels.h` & `fastsweep-0.1.3/kernels/cuda_kernels.h`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.2/kernels/cuda_kernels.ptx` & `fastsweep-0.1.3/kernels/cuda_kernels.ptx`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.2/pyproject.toml` & `fastsweep-0.1.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 [build-system]
 requires = ["setuptools", "wheel", "scikit-build", "cmake", "ninja", "pybind11", "drjit>=0.4.2"]
 
 build-backend = "setuptools.build_meta"
 
-[tool.isort]
-profile = "black"
-
-[tool.pytest.ini_options]
-norecursedirs = [ "ext" ]
-
 [tool.cibuildwheel]
 test-command = "python -c \"import fastsweep\""
 test-requires =  "pytest numpy drjit"
-skip = "*-musllinux* pp* cp36-* cp37-* cp311-* *-win32 *_i686 cp38-macosx_arm64"
+skip = "*-musllinux* pp* cp36-* cp37-* *-win32 *_i686 cp38-macosx_arm64"
 
 [tool.cibuildwheel.linux]
 repair-wheel-command = "python3 .github/workflows/tag_wheel_manylinux.py {wheel} {dest_dir}"
 archs = "auto64"
 
 [tool.cibuildwheel.windows]
 archs = "auto64"
```

### Comparing `fastsweep-0.1.2/python/example.py` & `fastsweep-0.1.3/python/example.py`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.2/python/pure_python_impl.py` & `fastsweep-0.1.3/python/pure_python_impl.py`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.2/redistancing.svg` & `fastsweep-0.1.3/redistancing.svg`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.2/setup.py` & `fastsweep-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 fastsweep_cmake_toolchain_file = os.environ.get("FASTSWEEP_CMAKE_TOOLCHAIN_FILE", "")
 fastsweep_drjit_cmake_dir = os.environ.get("FASTSWEEP_DRJIT_CMAKE_DIR", "")
 
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 
 setup(
     name="fastsweep",
     version=VERSION,
     description="Eikonal solver using parallel fast sweeping",
     author="Delio Vicini",
     author_email="delio.vicini@gmail.com",
```

### Comparing `fastsweep-0.1.2/src/cuda_helpers.h` & `fastsweep-0.1.3/src/cuda_helpers.h`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.2/src/distance_marcher.cpp` & `fastsweep-0.1.3/src/distance_marcher.cpp`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.2/src/fastsweep.egg-info/PKG-INFO` & `fastsweep-0.1.3/src/fastsweep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastsweep
-Version: 0.1.2
+Version: 0.1.3
 Summary: Eikonal solver using parallel fast sweeping
 Home-page: https://github.com/rgl-epfl/fastsweep
 Author: Delio Vicini
 Author-email: delio.vicini@gmail.com
 License: BSD
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `fastsweep-0.1.2/src/fastsweep.egg-info/SOURCES.txt` & `fastsweep-0.1.3/src/fastsweep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.2/src/main.cpp` & `fastsweep-0.1.3/src/main.cpp`

 * *Files identical despite different names*

### Comparing `fastsweep-0.1.2/src/tests/test_redistancing.py` & `fastsweep-0.1.3/src/tests/test_redistancing.py`

 * *Files identical despite different names*


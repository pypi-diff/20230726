# Comparing `tmp/psr-graf-1.0.0.tar.gz` & `tmp/psr-graf-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psr-graf-1.0.0.tar", last modified: Wed Jul 26 17:50:20 2023, max compression
+gzip compressed data, was "psr-graf-1.0.1.tar", last modified: Wed Jul 26 18:20:59 2023, max compression
```

## Comparing `psr-graf-1.0.0.tar` & `psr-graf-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 17:50:00.547495 psr-graf-1.0.0/
--rw-rw-rw-   0        0        0     3413 2023-07-26 17:50:20.687734 psr-graf-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2975 2023-07-26 17:15:18.000000 psr-graf-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 17:50:00.534876 psr-graf-1.0.0/psr/
-drwxrwxrwx   0        0        0        0 2023-07-26 17:50:00.536912 psr-graf-1.0.0/psr/graf/
--rw-rw-rw-   0        0        0       21 2023-07-26 17:15:18.000000 psr-graf-1.0.0/psr/graf/__init__.py
--rw-rw-rw-   0        0        0    11178 2023-07-26 17:38:30.000000 psr-graf-1.0.0/psr/graf/graf.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:50:20.687734 psr-graf-1.0.0/psr_graf.egg-info/
--rw-rw-rw-   0        0        0     3413 2023-07-26 17:50:20.000000 psr-graf-1.0.0/psr_graf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-07-26 17:50:20.000000 psr-graf-1.0.0/psr_graf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 17:50:20.000000 psr-graf-1.0.0/psr_graf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-26 17:50:20.000000 psr-graf-1.0.0/psr_graf.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0        4 2023-07-26 17:50:20.000000 psr-graf-1.0.0/psr_graf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 17:50:20.690226 psr-graf-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 18:20:59.535678 psr-graf-1.0.1/
+-rw-rw-rw-   0        0        0     4004 2023-07-26 18:20:59.534679 psr-graf-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3566 2023-07-26 18:15:41.000000 psr-graf-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 18:20:59.525996 psr-graf-1.0.1/psr/
+drwxrwxrwx   0        0        0        0 2023-07-26 18:20:59.528672 psr-graf-1.0.1/psr/graf/
+-rw-rw-rw-   0        0        0       21 2023-07-26 17:15:18.000000 psr-graf-1.0.1/psr/graf/__init__.py
+-rw-rw-rw-   0        0        0    11178 2023-07-26 18:17:45.000000 psr-graf-1.0.1/psr/graf/graf.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:20:59.534679 psr-graf-1.0.1/psr_graf.egg-info/
+-rw-rw-rw-   0        0        0     4004 2023-07-26 18:20:59.000000 psr-graf-1.0.1/psr_graf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-26 18:20:59.000000 psr-graf-1.0.1/psr_graf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 18:20:59.000000 psr-graf-1.0.1/psr_graf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-26 18:20:59.000000 psr-graf-1.0.1/psr_graf.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0        4 2023-07-26 18:20:59.000000 psr-graf-1.0.1/psr_graf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 18:20:59.535678 psr-graf-1.0.1/setup.cfg
```

### Comparing `psr-graf-1.0.0/PKG-INFO` & `psr-graf-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-Metadata-Version: 2.1
-Name: psr-graf
-Version: 1.0.0
-Summary: Utility module to read PSR Sddp's hdr/bin result file pairs.
-Home-page: https://github.com/psrenergy/pygraf
-Author: PSR
-Author-email: d.parrini@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 PyGraf
 ======
 
 
 Utility module to read Sddp hdr/bin result file pairs. Some examples to convert it to popular formats are available.
 
 
+Installing
+----------
+
+Install the latest version from [PyPI](https://pypi.org/)
+
+```
+pip install psr-graf
+```
+
+Or download this repository contents.
+
+
 Usage
 -----
 
 Start by importing `psr.graf` module. It's possible to read data directly using `open_bin` function or `load_as_dataframe` function if `pandas` package is available.
 
 
 The example below shows how to load data directly into a `pandas.DataFrame` and prints the first 5 lines of data.
@@ -76,50 +75,57 @@
 Data at stage 2, scenario 10, block 1: (7.440000057220459, 0.7440000176429749, 0.3680693209171295)
 ```
 
 
 Usage Samples
 -------------
 
-### [`dataframes_sample.py`](dataframes_sample.py)
+### [`dataframes_sample.py`](https://github.com/psrenergy/pygraf/blob/main/dataframes_sample.py)
 
 Shows how to read data into `pandas.DataFrame`s.
 
 Requires `pandas` package installed.
 
 
-### [`matplotlib_sample.py`](matplotlib_sample.py)
+### [`matplotlib_sample.py`](https://github.com/psrenergy/pygraf/blob/main/matplotlib_sample.py)
 
 Shows how to read data and plot data from hdr/bin file pairs.
 
-![](docs/matplotlib_sample_plot.png)
+![](https://github.com/psrenergy/pygraf/blob/main/docs/matplotlib_sample_plot.png)
 
 Requires `matplotlib` package installed.
 
 
 
-### [`csv_sample.py`](csv_sample.py)
+### [`csv_sample.py`](https://github.com/psrenergy/pygraf/blob/main/csv_sample.py)
 
 Shows how to convert from hdr/bin file pairs to csv using `psr.graf` module.
 
 This script can also be called from command line:
 
 ```bat
 python csv_sample.py input_file.hdr output_file.csv
 ```
 
 Where `output_file.csv` is optional.
 
 
-### [`parquet_sample.py`](parquet_sample.py)
+### [`parquet_sample.py`](https://github.com/psrenergy/pygraf/blob/main/parquet_sample.py)
 
 Shows how to convert from hdr/bin file pairs to Apache Parquet format.
 
 Requires `pyarrow` package installed.
 
 This script can also be called from command line:
 
 ```bat
 python parquet_sample.py input_file.hdr output_file.parquet
 ```
 
 Where `output_file.parquet` is optional.
+
+
+Issues and Support
+------------------
+
+Check PyGraf's [GitHub repository](https://github.com/psrenergy/pygraf/) and [issues page](https://github.com/psrenergy/pygraf/issues) for support.
+
```

### Comparing `psr-graf-1.0.0/psr/graf/graf.py` & `psr-graf-1.0.1/psr/graf/graf.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 _IS_PY2 = sys.version_info.major == 2
 
 if not _IS_PY2:
     from typing import Union
 
 
-_VERSION = "1.0.0"
+_VERSION = "1.0.1"
 
 # Number of bytes in a word (int32, float, ...)
 _WORD = 4
 
 
 # Check whether pandas' dataframe is available.
 _HAS_PANDAS = False
```

### Comparing `psr-graf-1.0.0/psr_graf.egg-info/PKG-INFO` & `psr-graf-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psr-graf
-Version: 1.0.0
+Version: 1.0.1
 Summary: Utility module to read PSR Sddp's hdr/bin result file pairs.
 Home-page: https://github.com/psrenergy/pygraf
 Author: PSR
 Author-email: d.parrini@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,26 @@
 PyGraf
 ======
 
 
 Utility module to read Sddp hdr/bin result file pairs. Some examples to convert it to popular formats are available.
 
 
+Installing
+----------
+
+Install the latest version from [PyPI](https://pypi.org/)
+
+```
+pip install psr-graf
+```
+
+Or download this repository contents.
+
+
 Usage
 -----
 
 Start by importing `psr.graf` module. It's possible to read data directly using `open_bin` function or `load_as_dataframe` function if `pandas` package is available.
 
 
 The example below shows how to load data directly into a `pandas.DataFrame` and prints the first 5 lines of data.
@@ -76,50 +88,57 @@
 Data at stage 2, scenario 10, block 1: (7.440000057220459, 0.7440000176429749, 0.3680693209171295)
 ```
 
 
 Usage Samples
 -------------
 
-### [`dataframes_sample.py`](dataframes_sample.py)
+### [`dataframes_sample.py`](https://github.com/psrenergy/pygraf/blob/main/dataframes_sample.py)
 
 Shows how to read data into `pandas.DataFrame`s.
 
 Requires `pandas` package installed.
 
 
-### [`matplotlib_sample.py`](matplotlib_sample.py)
+### [`matplotlib_sample.py`](https://github.com/psrenergy/pygraf/blob/main/matplotlib_sample.py)
 
 Shows how to read data and plot data from hdr/bin file pairs.
 
-![](docs/matplotlib_sample_plot.png)
+![](https://github.com/psrenergy/pygraf/blob/main/docs/matplotlib_sample_plot.png)
 
 Requires `matplotlib` package installed.
 
 
 
-### [`csv_sample.py`](csv_sample.py)
+### [`csv_sample.py`](https://github.com/psrenergy/pygraf/blob/main/csv_sample.py)
 
 Shows how to convert from hdr/bin file pairs to csv using `psr.graf` module.
 
 This script can also be called from command line:
 
 ```bat
 python csv_sample.py input_file.hdr output_file.csv
 ```
 
 Where `output_file.csv` is optional.
 
 
-### [`parquet_sample.py`](parquet_sample.py)
+### [`parquet_sample.py`](https://github.com/psrenergy/pygraf/blob/main/parquet_sample.py)
 
 Shows how to convert from hdr/bin file pairs to Apache Parquet format.
 
 Requires `pyarrow` package installed.
 
 This script can also be called from command line:
 
 ```bat
 python parquet_sample.py input_file.hdr output_file.parquet
 ```
 
 Where `output_file.parquet` is optional.
+
+
+Issues and Support
+------------------
+
+Check PyGraf's [GitHub repository](https://github.com/psrenergy/pygraf/) and [issues page](https://github.com/psrenergy/pygraf/issues) for support.
+
```


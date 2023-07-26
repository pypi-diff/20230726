# Comparing `tmp/henhoe2vec-1.0.2.tar.gz` & `tmp/henhoe2vec-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henhoe2vec-1.0.2.tar", last modified: Fri Jul 21 07:56:44 2023, max compression
+gzip compressed data, was "henhoe2vec-1.0.3.tar", last modified: Wed Jul 26 13:10:29 2023, max compression
```

## Comparing `henhoe2vec-1.0.2.tar` & `henhoe2vec-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-07-21 07:56:44.240456 henhoe2vec-1.0.2/
--rw-r--r--   0 bob        (501) staff       (20)     1071 2023-06-08 16:39:49.000000 henhoe2vec-1.0.2/LICENSE.txt
--rw-r--r--   0 bob        (501) staff       (20)     7136 2023-07-21 07:56:44.240249 henhoe2vec-1.0.2/PKG-INFO
--rw-r--r--   0 bob        (501) staff       (20)     4985 2023-06-20 13:30:29.000000 henhoe2vec-1.0.2/README.md
--rw-r--r--   0 bob        (501) staff       (20)     1199 2023-07-21 07:56:37.000000 henhoe2vec-1.0.2/pyproject.toml
--rw-r--r--   0 bob        (501) staff       (20)       38 2023-07-21 07:56:44.240519 henhoe2vec-1.0.2/setup.cfg
--rw-r--r--   0 bob        (501) staff       (20)       38 2023-06-13 07:41:13.000000 henhoe2vec-1.0.2/setup.py
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-07-21 07:56:44.234847 henhoe2vec-1.0.2/src/
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-07-21 07:56:44.237406 henhoe2vec-1.0.2/src/henhoe2vec/
--rw-r--r--   0 bob        (501) staff       (20)       78 2023-07-21 07:52:37.000000 henhoe2vec-1.0.2/src/henhoe2vec/__init__.py
--rw-r--r--   0 bob        (501) staff       (20)       37 2023-07-21 07:52:37.000000 henhoe2vec-1.0.2/src/henhoe2vec/__main__.py
--rw-r--r--   0 bob        (501) staff       (20)     2188 2023-06-10 19:24:50.000000 henhoe2vec-1.0.2/src/henhoe2vec/alias_sampling.py
--rw-r--r--   0 bob        (501) staff       (20)     2109 2023-06-20 13:32:52.000000 henhoe2vec-1.0.2/src/henhoe2vec/embeddings.py
--rw-r--r--   0 bob        (501) staff       (20)    10540 2023-07-21 07:37:30.000000 henhoe2vec-1.0.2/src/henhoe2vec/henhoe2vec.py
--rw-r--r--   0 bob        (501) staff       (20)    12288 2023-06-10 22:17:49.000000 henhoe2vec-1.0.2/src/henhoe2vec/henhoe2vec_walks.py
--rw-r--r--   0 bob        (501) staff       (20)      573 2023-06-10 21:52:42.000000 henhoe2vec-1.0.2/src/henhoe2vec/napkin.py
--rw-r--r--   0 bob        (501) staff       (20)     5314 2023-07-02 16:12:23.000000 henhoe2vec-1.0.2/src/henhoe2vec/utils.py
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-07-21 07:56:44.238544 henhoe2vec-1.0.2/src/henhoe2vec.egg-info/
--rw-r--r--   0 bob        (501) staff       (20)     7136 2023-07-21 07:56:44.000000 henhoe2vec-1.0.2/src/henhoe2vec.egg-info/PKG-INFO
--rw-r--r--   0 bob        (501) staff       (20)      593 2023-07-21 07:56:44.000000 henhoe2vec-1.0.2/src/henhoe2vec.egg-info/SOURCES.txt
--rw-r--r--   0 bob        (501) staff       (20)        1 2023-07-21 07:56:44.000000 henhoe2vec-1.0.2/src/henhoe2vec.egg-info/dependency_links.txt
--rw-r--r--   0 bob        (501) staff       (20)       76 2023-07-21 07:56:44.000000 henhoe2vec-1.0.2/src/henhoe2vec.egg-info/requires.txt
--rw-r--r--   0 bob        (501) staff       (20)       11 2023-07-21 07:56:44.000000 henhoe2vec-1.0.2/src/henhoe2vec.egg-info/top_level.txt
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-07-21 07:56:44.239685 henhoe2vec-1.0.2/tests/
--rw-r--r--   0 bob        (501) staff       (20)     1095 2023-06-10 22:18:24.000000 henhoe2vec-1.0.2/tests/test_alias_sampling.py
--rw-r--r--   0 bob        (501) staff       (20)      764 2023-06-10 22:18:24.000000 henhoe2vec-1.0.2/tests/test_embeddings.py
--rw-r--r--   0 bob        (501) staff       (20)     2171 2023-06-14 09:26:45.000000 henhoe2vec-1.0.2/tests/test_henhoe2vec.py
--rw-r--r--   0 bob        (501) staff       (20)     3913 2023-06-10 22:18:24.000000 henhoe2vec-1.0.2/tests/test_henhoe2vec_walks.py
--rw-r--r--   0 bob        (501) staff       (20)     4215 2023-06-17 08:08:24.000000 henhoe2vec-1.0.2/tests/test_utils.py
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-07-26 13:10:29.726532 henhoe2vec-1.0.3/
+-rw-r--r--   0 bob        (501) staff       (20)     1071 2023-06-08 16:39:49.000000 henhoe2vec-1.0.3/LICENSE.txt
+-rw-r--r--   0 bob        (501) staff       (20)     7114 2023-07-26 13:10:29.726379 henhoe2vec-1.0.3/PKG-INFO
+-rw-r--r--   0 bob        (501) staff       (20)     4963 2023-07-21 07:57:11.000000 henhoe2vec-1.0.3/README.md
+-rw-r--r--   0 bob        (501) staff       (20)     1199 2023-07-26 13:10:10.000000 henhoe2vec-1.0.3/pyproject.toml
+-rw-r--r--   0 bob        (501) staff       (20)       38 2023-07-26 13:10:29.726575 henhoe2vec-1.0.3/setup.cfg
+-rw-r--r--   0 bob        (501) staff       (20)       38 2023-06-13 07:41:13.000000 henhoe2vec-1.0.3/setup.py
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-07-26 13:10:29.721975 henhoe2vec-1.0.3/src/
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-07-26 13:10:29.724313 henhoe2vec-1.0.3/src/henhoe2vec/
+-rw-r--r--   0 bob        (501) staff       (20)       78 2023-07-21 07:52:37.000000 henhoe2vec-1.0.3/src/henhoe2vec/__init__.py
+-rw-r--r--   0 bob        (501) staff       (20)       37 2023-07-21 07:52:37.000000 henhoe2vec-1.0.3/src/henhoe2vec/__main__.py
+-rw-r--r--   0 bob        (501) staff       (20)     2188 2023-06-10 19:24:50.000000 henhoe2vec-1.0.3/src/henhoe2vec/alias_sampling.py
+-rw-r--r--   0 bob        (501) staff       (20)     2109 2023-06-20 13:32:52.000000 henhoe2vec-1.0.3/src/henhoe2vec/embeddings.py
+-rw-r--r--   0 bob        (501) staff       (20)    10540 2023-07-21 07:37:30.000000 henhoe2vec-1.0.3/src/henhoe2vec/henhoe2vec.py
+-rw-r--r--   0 bob        (501) staff       (20)    12337 2023-07-26 13:06:49.000000 henhoe2vec-1.0.3/src/henhoe2vec/henhoe2vec_walks.py
+-rw-r--r--   0 bob        (501) staff       (20)      573 2023-06-10 21:52:42.000000 henhoe2vec-1.0.3/src/henhoe2vec/napkin.py
+-rw-r--r--   0 bob        (501) staff       (20)     5314 2023-07-02 16:12:23.000000 henhoe2vec-1.0.3/src/henhoe2vec/utils.py
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-07-26 13:10:29.725276 henhoe2vec-1.0.3/src/henhoe2vec.egg-info/
+-rw-r--r--   0 bob        (501) staff       (20)     7114 2023-07-26 13:10:29.000000 henhoe2vec-1.0.3/src/henhoe2vec.egg-info/PKG-INFO
+-rw-r--r--   0 bob        (501) staff       (20)      593 2023-07-26 13:10:29.000000 henhoe2vec-1.0.3/src/henhoe2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 bob        (501) staff       (20)        1 2023-07-26 13:10:29.000000 henhoe2vec-1.0.3/src/henhoe2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 bob        (501) staff       (20)       76 2023-07-26 13:10:29.000000 henhoe2vec-1.0.3/src/henhoe2vec.egg-info/requires.txt
+-rw-r--r--   0 bob        (501) staff       (20)       11 2023-07-26 13:10:29.000000 henhoe2vec-1.0.3/src/henhoe2vec.egg-info/top_level.txt
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-07-26 13:10:29.726160 henhoe2vec-1.0.3/tests/
+-rw-r--r--   0 bob        (501) staff       (20)     1095 2023-06-10 22:18:24.000000 henhoe2vec-1.0.3/tests/test_alias_sampling.py
+-rw-r--r--   0 bob        (501) staff       (20)      764 2023-06-10 22:18:24.000000 henhoe2vec-1.0.3/tests/test_embeddings.py
+-rw-r--r--   0 bob        (501) staff       (20)     2171 2023-06-14 09:26:45.000000 henhoe2vec-1.0.3/tests/test_henhoe2vec.py
+-rw-r--r--   0 bob        (501) staff       (20)     3913 2023-06-10 22:18:24.000000 henhoe2vec-1.0.3/tests/test_henhoe2vec_walks.py
+-rw-r--r--   0 bob        (501) staff       (20)     4215 2023-06-17 08:08:24.000000 henhoe2vec-1.0.3/tests/test_utils.py
```

### Comparing `henhoe2vec-1.0.2/LICENSE.txt` & `henhoe2vec-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.2/PKG-INFO` & `henhoe2vec-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henhoe2vec
-Version: 1.0.2
+Version: 1.0.3
 Summary: Implementation of the HeNHoE-2vec algorithm by Valentini et al. (2021).
 Author-email: Robert Giesler <robert.giesler@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Robert Giesler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -82,34 +82,34 @@
 ### As a Python Script
 To run HeNHoE-2vec as a script, clone this repository using
 ```
 $ git clone git@github.com:Bertr0/HeNHoE-2vec.git
 ```
 , install the requirements found in `requirements.txt` and run the following command from the root of the repository:
 ```
-$ python3 -m src.henhoe2vec.henhoe2vec --input <input_path> --output_dir <output_dir_path>
+$ python3 -m src.henhoe2vec --input <input_path> --output_dir <output_dir_path>
 ```
 
 This will generate node embeddings for the nodes of the network specified by the multilayer edge list saved at `<input_path>` and saves the embedding files in `<output_dir>`.
 
-Run `python3 -m src.henhoe2vec.henhoe2vec --help` from the root of the repository to show an overview of all arguments taken by the script. The following table also shows an overview of all arguments:
+Run `python3 -m src.henhoe2vec --help` from the root of the repository to show an overview of all arguments taken by the script. The following table also shows an overview of all arguments:
 
 #### Script Arguments
 | Argument | Type | Description | Default Value |
 | -------- | ---- | ----------- | ------------- |
 | `--input` | str | Path to the multilayer edge list of the network to be embedded (csv file with no index). | - |
 | `--sep` | str | Delimiter of the input csv edge list. | "\t" |
 | `--header` | store_true | Pass this argument if the input csv edge list has a header. | - |
-| `--output-name` | str | Name of the output .csv file (without suffix). | "embeddings" |
-| `--is-directed` | store_true | Pass this argument if the network is directed. | - |
-| `--edges-are-distances` | store_true | Pass this argument if edge weights indicate distance between nodes (opposed to weight/similarity). | - |
+| `--output_name` | str | Name of the output .csv file (without suffix). | "embeddings" |
+| `--is_directed` | store_true | Pass this argument if the network is directed. | - |
+| `--edges_are_distances` | store_true | Pass this argument if edge weights indicate distance between nodes (opposed to weight/similarity). | - |
 | `--output_dir` | str | Path of the output directory where the embedding files will be saved. | - |
 | `--dimensions` | int | The dimensionality of the embeddings. | 128 |
-| `--walk-length` | int | Length of each random walk. | 20 |
-| `--num-walks` | int | Number of random walks to simulate for each node. | 10 |
+| `--walk_length` | int | Length of each random walk. | 20 |
+| `--num_walks` | int | Number of random walks to simulate for each node. | 10 |
 | `--p` | float | Return parameter `p` from the node2vec algorithm. | 1.0 |
 | `--q` | float | In-out parameter `q` from the node2vec algorithm. | 0.5 |
 | `--s` | float | Default switching parameter for layer pairs which are not specified in the `--s-dict` argument. | 1.0 |
-| `--s-dict` | list | Switching parameters for specific layer pairs in a dict-like manner. Pass the names of layer pairs followed by their switching parameters, separated by white spaces. E.g., if the switching parameter from `layer1` to `layer2` is `0.5` and the switching parameter from `layer2` to `layer1` is `0.7`, you would pass `layer1 layer2 0.5 layer2 layer1 0.7`. Note that layer pairs are directed. For all layer pairs which are not specified here, the default parameter `--s` is adopted. | empty list |
-| `--window-size` | int | Context size for the word2vec optimization. | 10 |
+| `--s_dict` | list | Switching parameters for specific layer pairs in a dict-like manner. Pass the names of layer pairs followed by their switching parameters, separated by white spaces. E.g., if the switching parameter from `layer1` to `layer2` is `0.5` and the switching parameter from `layer2` to `layer1` is `0.7`, you would pass `layer1 layer2 0.5 layer2 layer1 0.7`. Note that layer pairs are directed. For all layer pairs which are not specified here, the default parameter `--s` is adopted. | empty list |
+| `--window_size` | int | Context size for the word2vec optimization. | 10 |
 | `--epochs` | int | Number of epochs in SGD. | 1 |
 | `--workers` | int | Number of parallel workers (threads). | 8 |
```

### Comparing `henhoe2vec-1.0.2/README.md` & `henhoe2vec-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -41,34 +41,34 @@
 ### As a Python Script
 To run HeNHoE-2vec as a script, clone this repository using
 ```
 $ git clone git@github.com:Bertr0/HeNHoE-2vec.git
 ```
 , install the requirements found in `requirements.txt` and run the following command from the root of the repository:
 ```
-$ python3 -m src.henhoe2vec.henhoe2vec --input <input_path> --output_dir <output_dir_path>
+$ python3 -m src.henhoe2vec --input <input_path> --output_dir <output_dir_path>
 ```
 
 This will generate node embeddings for the nodes of the network specified by the multilayer edge list saved at `<input_path>` and saves the embedding files in `<output_dir>`.
 
-Run `python3 -m src.henhoe2vec.henhoe2vec --help` from the root of the repository to show an overview of all arguments taken by the script. The following table also shows an overview of all arguments:
+Run `python3 -m src.henhoe2vec --help` from the root of the repository to show an overview of all arguments taken by the script. The following table also shows an overview of all arguments:
 
 #### Script Arguments
 | Argument | Type | Description | Default Value |
 | -------- | ---- | ----------- | ------------- |
 | `--input` | str | Path to the multilayer edge list of the network to be embedded (csv file with no index). | - |
 | `--sep` | str | Delimiter of the input csv edge list. | "\t" |
 | `--header` | store_true | Pass this argument if the input csv edge list has a header. | - |
-| `--output-name` | str | Name of the output .csv file (without suffix). | "embeddings" |
-| `--is-directed` | store_true | Pass this argument if the network is directed. | - |
-| `--edges-are-distances` | store_true | Pass this argument if edge weights indicate distance between nodes (opposed to weight/similarity). | - |
+| `--output_name` | str | Name of the output .csv file (without suffix). | "embeddings" |
+| `--is_directed` | store_true | Pass this argument if the network is directed. | - |
+| `--edges_are_distances` | store_true | Pass this argument if edge weights indicate distance between nodes (opposed to weight/similarity). | - |
 | `--output_dir` | str | Path of the output directory where the embedding files will be saved. | - |
 | `--dimensions` | int | The dimensionality of the embeddings. | 128 |
-| `--walk-length` | int | Length of each random walk. | 20 |
-| `--num-walks` | int | Number of random walks to simulate for each node. | 10 |
+| `--walk_length` | int | Length of each random walk. | 20 |
+| `--num_walks` | int | Number of random walks to simulate for each node. | 10 |
 | `--p` | float | Return parameter `p` from the node2vec algorithm. | 1.0 |
 | `--q` | float | In-out parameter `q` from the node2vec algorithm. | 0.5 |
 | `--s` | float | Default switching parameter for layer pairs which are not specified in the `--s-dict` argument. | 1.0 |
-| `--s-dict` | list | Switching parameters for specific layer pairs in a dict-like manner. Pass the names of layer pairs followed by their switching parameters, separated by white spaces. E.g., if the switching parameter from `layer1` to `layer2` is `0.5` and the switching parameter from `layer2` to `layer1` is `0.7`, you would pass `layer1 layer2 0.5 layer2 layer1 0.7`. Note that layer pairs are directed. For all layer pairs which are not specified here, the default parameter `--s` is adopted. | empty list |
-| `--window-size` | int | Context size for the word2vec optimization. | 10 |
+| `--s_dict` | list | Switching parameters for specific layer pairs in a dict-like manner. Pass the names of layer pairs followed by their switching parameters, separated by white spaces. E.g., if the switching parameter from `layer1` to `layer2` is `0.5` and the switching parameter from `layer2` to `layer1` is `0.7`, you would pass `layer1 layer2 0.5 layer2 layer1 0.7`. Note that layer pairs are directed. For all layer pairs which are not specified here, the default parameter `--s` is adopted. | empty list |
+| `--window_size` | int | Context size for the word2vec optimization. | 10 |
 | `--epochs` | int | Number of epochs in SGD. | 1 |
 | `--workers` | int | Number of parallel workers (threads). | 8 |
```

### Comparing `henhoe2vec-1.0.2/pyproject.toml` & `henhoe2vec-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "henhoe2vec"
-version = "1.0.2"
+version = "1.0.3"
 description = "Implementation of the HeNHoE-2vec algorithm by Valentini et al. (2021)."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "Robert Giesler", email = "robert.giesler@rwth-aachen.de"}
 ]
```

### Comparing `henhoe2vec-1.0.2/src/henhoe2vec/alias_sampling.py` & `henhoe2vec-1.0.3/src/henhoe2vec/alias_sampling.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.2/src/henhoe2vec/embeddings.py` & `henhoe2vec-1.0.3/src/henhoe2vec/embeddings.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.2/src/henhoe2vec/henhoe2vec.py` & `henhoe2vec-1.0.3/src/henhoe2vec/henhoe2vec.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.2/src/henhoe2vec/henhoe2vec_walks.py` & `henhoe2vec-1.0.3/src/henhoe2vec/henhoe2vec_walks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import random
+import numpy as np
 
 # from alias_sampling import alias_setup, alias_draw
 from .alias_sampling import alias_setup, alias_draw
 
 
 class HenHoe2vec:
     """
@@ -75,15 +76,15 @@
         # Form: {node : (J, q)}
         self.transition_probs_nodes = {}
         # Transition probability distribution to neighbors of each node based on edge
         # weights, p, q, and switching parameters. Used for all other steps of the walk.
         # Form: {(node1, node2) : (J, q)}
         self.transition_probs_edges = {}
 
-        if type(s) in [float, int]:
+        if type(s) in [float, int] or isinstance(s, np.floating):
             self.s = {"default": s}
         elif type(s) == dict:
             self.s = s
         else:
             raise TypeError(
                 f"[ERROR] Invalid type for argument s. Should be float or dict but"
                 f" is {type(s)}."
```

### Comparing `henhoe2vec-1.0.2/src/henhoe2vec/napkin.py` & `henhoe2vec-1.0.3/src/henhoe2vec/napkin.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.2/src/henhoe2vec/utils.py` & `henhoe2vec-1.0.3/src/henhoe2vec/utils.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.2/src/henhoe2vec.egg-info/PKG-INFO` & `henhoe2vec-1.0.3/src/henhoe2vec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henhoe2vec
-Version: 1.0.2
+Version: 1.0.3
 Summary: Implementation of the HeNHoE-2vec algorithm by Valentini et al. (2021).
 Author-email: Robert Giesler <robert.giesler@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Robert Giesler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -82,34 +82,34 @@
 ### As a Python Script
 To run HeNHoE-2vec as a script, clone this repository using
 ```
 $ git clone git@github.com:Bertr0/HeNHoE-2vec.git
 ```
 , install the requirements found in `requirements.txt` and run the following command from the root of the repository:
 ```
-$ python3 -m src.henhoe2vec.henhoe2vec --input <input_path> --output_dir <output_dir_path>
+$ python3 -m src.henhoe2vec --input <input_path> --output_dir <output_dir_path>
 ```
 
 This will generate node embeddings for the nodes of the network specified by the multilayer edge list saved at `<input_path>` and saves the embedding files in `<output_dir>`.
 
-Run `python3 -m src.henhoe2vec.henhoe2vec --help` from the root of the repository to show an overview of all arguments taken by the script. The following table also shows an overview of all arguments:
+Run `python3 -m src.henhoe2vec --help` from the root of the repository to show an overview of all arguments taken by the script. The following table also shows an overview of all arguments:
 
 #### Script Arguments
 | Argument | Type | Description | Default Value |
 | -------- | ---- | ----------- | ------------- |
 | `--input` | str | Path to the multilayer edge list of the network to be embedded (csv file with no index). | - |
 | `--sep` | str | Delimiter of the input csv edge list. | "\t" |
 | `--header` | store_true | Pass this argument if the input csv edge list has a header. | - |
-| `--output-name` | str | Name of the output .csv file (without suffix). | "embeddings" |
-| `--is-directed` | store_true | Pass this argument if the network is directed. | - |
-| `--edges-are-distances` | store_true | Pass this argument if edge weights indicate distance between nodes (opposed to weight/similarity). | - |
+| `--output_name` | str | Name of the output .csv file (without suffix). | "embeddings" |
+| `--is_directed` | store_true | Pass this argument if the network is directed. | - |
+| `--edges_are_distances` | store_true | Pass this argument if edge weights indicate distance between nodes (opposed to weight/similarity). | - |
 | `--output_dir` | str | Path of the output directory where the embedding files will be saved. | - |
 | `--dimensions` | int | The dimensionality of the embeddings. | 128 |
-| `--walk-length` | int | Length of each random walk. | 20 |
-| `--num-walks` | int | Number of random walks to simulate for each node. | 10 |
+| `--walk_length` | int | Length of each random walk. | 20 |
+| `--num_walks` | int | Number of random walks to simulate for each node. | 10 |
 | `--p` | float | Return parameter `p` from the node2vec algorithm. | 1.0 |
 | `--q` | float | In-out parameter `q` from the node2vec algorithm. | 0.5 |
 | `--s` | float | Default switching parameter for layer pairs which are not specified in the `--s-dict` argument. | 1.0 |
-| `--s-dict` | list | Switching parameters for specific layer pairs in a dict-like manner. Pass the names of layer pairs followed by their switching parameters, separated by white spaces. E.g., if the switching parameter from `layer1` to `layer2` is `0.5` and the switching parameter from `layer2` to `layer1` is `0.7`, you would pass `layer1 layer2 0.5 layer2 layer1 0.7`. Note that layer pairs are directed. For all layer pairs which are not specified here, the default parameter `--s` is adopted. | empty list |
-| `--window-size` | int | Context size for the word2vec optimization. | 10 |
+| `--s_dict` | list | Switching parameters for specific layer pairs in a dict-like manner. Pass the names of layer pairs followed by their switching parameters, separated by white spaces. E.g., if the switching parameter from `layer1` to `layer2` is `0.5` and the switching parameter from `layer2` to `layer1` is `0.7`, you would pass `layer1 layer2 0.5 layer2 layer1 0.7`. Note that layer pairs are directed. For all layer pairs which are not specified here, the default parameter `--s` is adopted. | empty list |
+| `--window_size` | int | Context size for the word2vec optimization. | 10 |
 | `--epochs` | int | Number of epochs in SGD. | 1 |
 | `--workers` | int | Number of parallel workers (threads). | 8 |
```

### Comparing `henhoe2vec-1.0.2/src/henhoe2vec.egg-info/SOURCES.txt` & `henhoe2vec-1.0.3/src/henhoe2vec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.2/tests/test_alias_sampling.py` & `henhoe2vec-1.0.3/tests/test_alias_sampling.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.2/tests/test_embeddings.py` & `henhoe2vec-1.0.3/tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.2/tests/test_henhoe2vec.py` & `henhoe2vec-1.0.3/tests/test_henhoe2vec.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.2/tests/test_henhoe2vec_walks.py` & `henhoe2vec-1.0.3/tests/test_henhoe2vec_walks.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.2/tests/test_utils.py` & `henhoe2vec-1.0.3/tests/test_utils.py`

 * *Files identical despite different names*


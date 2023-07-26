# Comparing `tmp/hypod-0.0.1.tar.gz` & `tmp/hypod-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypod-0.0.1.tar", last modified: Sat May  6 00:20:12 2023, max compression
+gzip compressed data, was "hypod-0.0.2.tar", last modified: Wed Jul 26 05:29:36 2023, max compression
```

## Comparing `hypod-0.0.1.tar` & `hypod-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jiseobkim   (501) staff       (20)        0 2023-05-06 00:20:12.076052 hypod-0.0.1/
--rw-r--r--   0 jiseobkim   (501) staff       (20)     1066 2023-05-06 00:13:01.000000 hypod-0.0.1/LICENSE
--rw-r--r--   0 jiseobkim   (501) staff       (20)     8277 2023-05-06 00:20:12.075853 hypod-0.0.1/PKG-INFO
--rw-r--r--   0 jiseobkim   (501) staff       (20)     6539 2023-05-06 00:13:01.000000 hypod-0.0.1/README.md
-drwxr-xr-x   0 jiseobkim   (501) staff       (20)        0 2023-05-06 00:20:12.074859 hypod-0.0.1/hypod/
--rw-r--r--   0 jiseobkim   (501) staff       (20)      117 2023-05-06 00:13:01.000000 hypod-0.0.1/hypod/__init__.py
--rw-r--r--   0 jiseobkim   (501) staff       (20)       22 2023-05-06 00:13:01.000000 hypod-0.0.1/hypod/_version.py
--rw-r--r--   0 jiseobkim   (501) staff       (20)     9177 2023-05-06 00:13:01.000000 hypod-0.0.1/hypod/decor.py
--rw-r--r--   0 jiseobkim   (501) staff       (20)     3908 2023-05-06 00:13:01.000000 hypod-0.0.1/hypod/main.py
--rw-r--r--   0 jiseobkim   (501) staff       (20)     1138 2023-05-06 00:13:01.000000 hypod-0.0.1/hypod/parser.py
-drwxr-xr-x   0 jiseobkim   (501) staff       (20)        0 2023-05-06 00:20:12.075617 hypod-0.0.1/hypod.egg-info/
--rw-r--r--   0 jiseobkim   (501) staff       (20)     8277 2023-05-06 00:20:12.000000 hypod-0.0.1/hypod.egg-info/PKG-INFO
--rw-r--r--   0 jiseobkim   (501) staff       (20)      274 2023-05-06 00:20:12.000000 hypod-0.0.1/hypod.egg-info/SOURCES.txt
--rw-r--r--   0 jiseobkim   (501) staff       (20)        1 2023-05-06 00:20:12.000000 hypod-0.0.1/hypod.egg-info/dependency_links.txt
--rw-r--r--   0 jiseobkim   (501) staff       (20)       22 2023-05-06 00:20:12.000000 hypod-0.0.1/hypod.egg-info/requires.txt
--rw-r--r--   0 jiseobkim   (501) staff       (20)        6 2023-05-06 00:20:12.000000 hypod-0.0.1/hypod.egg-info/top_level.txt
--rw-r--r--   0 jiseobkim   (501) staff       (20)      760 2023-05-06 00:13:01.000000 hypod-0.0.1/pyproject.toml
--rw-r--r--   0 jiseobkim   (501) staff       (20)       22 2023-05-06 00:13:01.000000 hypod-0.0.1/requirements.txt
--rw-r--r--   0 jiseobkim   (501) staff       (20)       38 2023-05-06 00:20:12.076110 hypod-0.0.1/setup.cfg
+drwxr-xr-x   0 jiseobkim   (501) staff       (20)        0 2023-07-26 05:29:36.324014 hypod-0.0.2/
+-rw-r--r--   0 jiseobkim   (501) staff       (20)     1066 2023-05-06 00:13:01.000000 hypod-0.0.2/LICENSE
+-rw-r--r--   0 jiseobkim   (501) staff       (20)     8813 2023-07-26 05:29:36.323718 hypod-0.0.2/PKG-INFO
+-rw-r--r--   0 jiseobkim   (501) staff       (20)     7075 2023-05-06 03:23:44.000000 hypod-0.0.2/README.md
+drwxr-xr-x   0 jiseobkim   (501) staff       (20)        0 2023-07-26 05:29:36.319923 hypod-0.0.2/hypod/
+-rw-r--r--   0 jiseobkim   (501) staff       (20)      117 2023-05-06 00:13:01.000000 hypod-0.0.2/hypod/__init__.py
+-rw-r--r--   0 jiseobkim   (501) staff       (20)       22 2023-07-26 05:26:00.000000 hypod-0.0.2/hypod/_version.py
+-rw-r--r--   0 jiseobkim   (501) staff       (20)     9688 2023-07-26 05:19:59.000000 hypod-0.0.2/hypod/decor.py
+-rw-r--r--   0 jiseobkim   (501) staff       (20)     3908 2023-05-06 00:13:01.000000 hypod-0.0.2/hypod/main.py
+-rw-r--r--   0 jiseobkim   (501) staff       (20)     1138 2023-05-06 00:13:01.000000 hypod-0.0.2/hypod/parser.py
+drwxr-xr-x   0 jiseobkim   (501) staff       (20)        0 2023-07-26 05:29:36.321406 hypod-0.0.2/hypod.egg-info/
+-rw-r--r--   0 jiseobkim   (501) staff       (20)     8813 2023-07-26 05:29:36.000000 hypod-0.0.2/hypod.egg-info/PKG-INFO
+-rw-r--r--   0 jiseobkim   (501) staff       (20)      274 2023-07-26 05:29:36.000000 hypod-0.0.2/hypod.egg-info/SOURCES.txt
+-rw-r--r--   0 jiseobkim   (501) staff       (20)        1 2023-07-26 05:29:36.000000 hypod-0.0.2/hypod.egg-info/dependency_links.txt
+-rw-r--r--   0 jiseobkim   (501) staff       (20)       22 2023-07-26 05:29:36.000000 hypod-0.0.2/hypod.egg-info/requires.txt
+-rw-r--r--   0 jiseobkim   (501) staff       (20)        6 2023-07-26 05:29:36.000000 hypod-0.0.2/hypod.egg-info/top_level.txt
+-rw-r--r--   0 jiseobkim   (501) staff       (20)      760 2023-05-06 00:13:01.000000 hypod-0.0.2/pyproject.toml
+-rw-r--r--   0 jiseobkim   (501) staff       (20)       22 2023-05-06 00:13:01.000000 hypod-0.0.2/requirements.txt
+-rw-r--r--   0 jiseobkim   (501) staff       (20)       38 2023-07-26 05:29:36.324097 hypod-0.0.2/setup.cfg
```

### Comparing `hypod-0.0.1/LICENSE` & `hypod-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hypod-0.0.1/PKG-INFO` & `hypod-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypod
-Version: 0.0.1
+Version: 0.0.2
 Summary: Hypod: A dataclass-based hyperparameter managing system
 Author-email: Jiseob Kim <justjest@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jiseob Kim
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,43 +32,43 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hypod: A dataclass-based hyperparameter managing system
 
 ## Overview
-Deep learning models are often composed of multiple networks, where each of the networks is composed of multiple layers, and the class of each layer or its hyperparameters differ by experiments. `Hypod` simplifies managing this complex hierarchy of hyperparameters utilizing the built-in `dataclass`.
+Deep learning models are often composed of multiple networks, where each of the networks is composed of multiple layers, and the class of each layer or its hyperparameters differ by experiments. `Hypod` simplifies managing this complex hierarchy of hyperparameters utilizing the built-in [`dataclass`](https://docs.python.org/3/library/dataclasses.html).
 
-The `dataclass` derives the following benefits.
+`dataclass` derives the following benefits.
 * Defining a group of hyperaparameters is easy with **type annotation** support.
 * Creating it is easy with the auto-defined `__init__`.
 * Many IDE's (e.g., PyCharm, VSCode) support "jump to the definition".
 
 However, difficulties for using it "as-is" in hyperparameter-managing are:
 * Handling nested dataclasses is not so good.
-* Parsing the strings or sys.argv to create a dataclass is not natively supported.
+* Parsing strings or sys.argv to create a dataclass is not natively supported.
 * Switching between multiple child dataclasses using a simple "tag" is cumbersome.
 
 `Hypod` will handle all these difficulties for you with following advantages.
-* Fast, lightweight implementation using the built-in `dataclass` and descriptors
+* Fast, lightweight implementation using the built-in `dataclass` and [descriptors](https://docs.python.org/3/howto/descriptor.html)
 * Minimal dependency
 * Type-checking (based on annotation)
 * Parsing a stringified object or YAML to create the corresponding nested dataclass
 * Ability to auto-make the corresponding module (e.g., layer, network), when defined as an inner class of that module.
 
 ### Comparison with other packages
 * [Hydra](https://github.com/facebookresearch/hydra): Hydra is a popular package with the same purpose. Its _structured config_ mode allows defining a config with `dataclass` as well. However, Hydra converts a config into `DictConfig` object (from another package `omegaconf`) even when it is originally defined with `dataclass`. Thus, all the operations (modifying, getting values, merging) are done with `DictConfig` and this brings the following drawbacks compared to Hypod, which uses `dataclass` object all the time.
   * `DictConfig` is not type annotated.
   * "Go to the definition" in IDE cannot be done with `DictConfig`.
   * Inheritance strcuture of configs cannot be checked.
-  * Complex value interpolation is difficult or impossible to implement. In Hypod `dataclass`, it can be done using built-in `__post_init__()` function (see `examples/advanced_usage.py`).
+  * Complex value interpolation is difficult or impossible to implement. In Hypod `dataclass`, it can be done using built-in [`__post_init__()`](https://docs.python.org/3/library/dataclasses.html#post-init-processing) function (see `examples/advanced_usage.py`).
 
 
 ### Etymology
-Hypod stands for **"A Pot of Hyperparameters, or A Hyperparameters-Pot"**. You can put various Hyperparameters in a Pot and mix them with others as you wish.
+Hypod stands for **"A Pod of Hyperparameters, or A Hyperparameters-Pod"**. You can put various Hyperparameters as a Pod and compose them with other Pods as you wish.
 
 ## Quick start
 ### Install the package
 `pip install hypod`
 
 ### Basic Usage
 
@@ -76,56 +76,56 @@
 from dataclasses import dataclass
 from hypod import hypod
 
 
 @dataclass
 @hypod
 class LayerHP:
-  in_features: int
-  out_features: int
-  init_scale: float = 0.9
+    in_features: int
+    out_features: int
+    init_scale: float = 0.9
 
 
 @dataclass
 @hypod
 class NetworkHP:
-  num_layers: int
-  layer_hp: LayerHP
+    num_layers: int
+    layer_hp: LayerHP
 
 
 if __name__ == "__main__":
-  # Hypod can be created in the same manner as dataclass.
-  net_hp1 = NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32))
-  print(net_hp1)
-  # Hypod can be also created from parsing stringified objects.
-  net_hp2 = NetworkHP(num_layers="3", layer_hp=LayerHP("64", 32))
-  print(net_hp2)
-  # Hypod class itself can be also created from a dictionary.
-  net_hp3 = NetworkHP(num_layers=3, layer_hp=dict(in_features=64, out_features=32))
-  print(net_hp3)
+    # Hypod can be created in the same manner as dataclass.
+    net_hp1 = NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32))
+    print(net_hp1)
+    # Hypod can be also created from parsing stringified objects.
+    net_hp2 = NetworkHP(num_layers="3", layer_hp=LayerHP("64", 32))
+    print(net_hp2)
+    # Hypod class itself can be also created from a dictionary.
+    net_hp3 = NetworkHP(num_layers=3, layer_hp=dict(in_features=64, out_features=32))
+    print(net_hp3)
 
 ```
 
 ### Command-line Usage
 With the Hypod classes defined the same as above, define the main function as follows.
 
 ```python
 # main.py
 from hypod import hypod_main
 
 
 @hypod_main()  # parses sys.argv to construct the hypod in the first argument, `net_hp`
 def main(net_hp: NetworkHP):
-  print(net_hp)
+    print(net_hp)
 
 
 if __name__ == "__main__":
-  main()
+    main()
 ```
-Then, in the command-line type as follows to obtain the same results as before.
+Then, on the command-line, type as follows to obtain the same results as before.
 `python main.py num_layers=3 layer_hp.in_features=64 layer_hp.out_features=32`
 
 
 ### Inheritance
 Hypod can be subclassed with a **tag**.
 
 ```python
@@ -133,72 +133,72 @@
 
 from hypod import hypod
 
 
 @dataclass
 @hypod
 class Data:
-  path: str
-  batch_size: int = 4
+    path: str
+    batch_size: int = 4
 
 
 @dataclass
 @hypod
 class FFHQData(Data, tag="ffhq"):
-  path: str = "/path/to/FFHQ"
-  meta: str = "Flicker-Faces HQ Data, containing 70k images"
+    path: str = "/path/to/FFHQ"
+    meta: str = "Flicker-Faces HQ Data, containing 70k images"
 
 
 @dataclass
 @hypod
 class FFHQDataLargeBatch(FFHQData, tag="ffhq_lg"):
-  batch_size: int = 16
+    batch_size: int = 16
 
 
 @dataclass
 @hypod
 class Model:
-  data: Data
-  net: NetworkHP
+    data: Data
+    net: NetworkHP
 
 
 if __name__ == "__main__":
-  model_with_ffhq = Model(
-    data="ffhq", net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
-  )
-  print(model_with_ffhq)
-
-  model_with_ffhq_lg = Model(
-    data=dict(_tag="ffhq_lg"),  # Also can be created from dict with "_tag" key.
-    net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
-  )
-  print(model_with_ffhq_lg)
-
-  model_with_cifar10 = Model(
-    data=dict(path="/path/to/cifar10"),
-    net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
-  )
-  print(model_with_cifar10)
+    model_with_ffhq = Model(
+        data="ffhq", net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
+    )
+    print(model_with_ffhq)
+
+    model_with_ffhq_lg = Model(
+        data=dict(_tag="ffhq_lg"),  # Also can be created from dict with "_tag" key.
+        net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
+    )
+    print(model_with_ffhq_lg)
+
+    model_with_cifar10 = Model(
+        data=dict(path="/path/to/cifar10"),
+        net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
+    )
+    print(model_with_cifar10)
 ```
 
 ### Command-line Usage with Inheritance
 With the Hypod classes defined the same as above, define the main function as follows.
 
 ```python
 # main.py
 from hypod import hypod_main
 
 
-@hypod_main()  # parses sys.argv to construct the hypod in the first argument, `net_hp`
+@hypod_main()  # parses sys.argv to construct the hypod in the first argument, `model`
 def main(model: Model):
-  print(model)
+    print(model)
 
 
 if __name__ == "__main__":
-  main()
+    main()
 ```
 Then, in the command-line type as follows to obtain the same results as before.
 `python main.py model.data=ffhq model.net.num_layers=3 model.net.layer_hp.in_features=64 model.net.layer_hp.out_features=32`
 I.e., tag can be fed in the CLI as the root argument.
 
 ### Advanced Usage (Value Interpolation)
 * Please refer to `advanced_usage.py` in the `examples` directory.
@@ -212,10 +212,10 @@
 * (Q) Is `typing.Union` supported? 
   * (A) Yes. But when it is a union of `str` or `dict`, there are ambiguities in parsing the stringified objects. A warning or an error will be raised in this case.
 * (Q) Does tag-based creation still work when `typing.Union` is used?
   * (A) Yes. The tag search will be done over all the types in the union.
 * (Q) Are `typing.List` or other generic types supported?
   * (A) Yes.
 * (Q) How can I use value interpolation?
-  * (A) `dataclass` provides `__post_init__()` function where you can define a .
+  * (A) `dataclass` provides [`__post_init__()`](https://docs.python.org/3/library/dataclasses.html#post-init-processing) function where you can define interpolation rules in *Python*. E.g., if you want to make a hyperparameter `a` that has to be twice the value of `b` in some Hypod, write `self.a = 2 * self.b` in `__post_init__()` of that Hypod.
 * (Q) Why not using `typing.dataclass_transform()` in implementing Hypod?
   * (A) Because requirement of Python>=3.11 is too strict for now.
```

### Comparing `hypod-0.0.1/README.md` & `hypod-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # Hypod: A dataclass-based hyperparameter managing system
 
 ## Overview
-Deep learning models are often composed of multiple networks, where each of the networks is composed of multiple layers, and the class of each layer or its hyperparameters differ by experiments. `Hypod` simplifies managing this complex hierarchy of hyperparameters utilizing the built-in `dataclass`.
+Deep learning models are often composed of multiple networks, where each of the networks is composed of multiple layers, and the class of each layer or its hyperparameters differ by experiments. `Hypod` simplifies managing this complex hierarchy of hyperparameters utilizing the built-in [`dataclass`](https://docs.python.org/3/library/dataclasses.html).
 
-The `dataclass` derives the following benefits.
+`dataclass` derives the following benefits.
 * Defining a group of hyperaparameters is easy with **type annotation** support.
 * Creating it is easy with the auto-defined `__init__`.
 * Many IDE's (e.g., PyCharm, VSCode) support "jump to the definition".
 
 However, difficulties for using it "as-is" in hyperparameter-managing are:
 * Handling nested dataclasses is not so good.
-* Parsing the strings or sys.argv to create a dataclass is not natively supported.
+* Parsing strings or sys.argv to create a dataclass is not natively supported.
 * Switching between multiple child dataclasses using a simple "tag" is cumbersome.
 
 `Hypod` will handle all these difficulties for you with following advantages.
-* Fast, lightweight implementation using the built-in `dataclass` and descriptors
+* Fast, lightweight implementation using the built-in `dataclass` and [descriptors](https://docs.python.org/3/howto/descriptor.html)
 * Minimal dependency
 * Type-checking (based on annotation)
 * Parsing a stringified object or YAML to create the corresponding nested dataclass
 * Ability to auto-make the corresponding module (e.g., layer, network), when defined as an inner class of that module.
 
 ### Comparison with other packages
 * [Hydra](https://github.com/facebookresearch/hydra): Hydra is a popular package with the same purpose. Its _structured config_ mode allows defining a config with `dataclass` as well. However, Hydra converts a config into `DictConfig` object (from another package `omegaconf`) even when it is originally defined with `dataclass`. Thus, all the operations (modifying, getting values, merging) are done with `DictConfig` and this brings the following drawbacks compared to Hypod, which uses `dataclass` object all the time.
   * `DictConfig` is not type annotated.
   * "Go to the definition" in IDE cannot be done with `DictConfig`.
   * Inheritance strcuture of configs cannot be checked.
-  * Complex value interpolation is difficult or impossible to implement. In Hypod `dataclass`, it can be done using built-in `__post_init__()` function (see `examples/advanced_usage.py`).
+  * Complex value interpolation is difficult or impossible to implement. In Hypod `dataclass`, it can be done using built-in [`__post_init__()`](https://docs.python.org/3/library/dataclasses.html#post-init-processing) function (see `examples/advanced_usage.py`).
 
 
 ### Etymology
-Hypod stands for **"A Pot of Hyperparameters, or A Hyperparameters-Pot"**. You can put various Hyperparameters in a Pot and mix them with others as you wish.
+Hypod stands for **"A Pod of Hyperparameters, or A Hyperparameters-Pod"**. You can put various Hyperparameters as a Pod and compose them with other Pods as you wish.
 
 ## Quick start
 ### Install the package
 `pip install hypod`
 
 ### Basic Usage
 
@@ -41,56 +41,56 @@
 from dataclasses import dataclass
 from hypod import hypod
 
 
 @dataclass
 @hypod
 class LayerHP:
-  in_features: int
-  out_features: int
-  init_scale: float = 0.9
+    in_features: int
+    out_features: int
+    init_scale: float = 0.9
 
 
 @dataclass
 @hypod
 class NetworkHP:
-  num_layers: int
-  layer_hp: LayerHP
+    num_layers: int
+    layer_hp: LayerHP
 
 
 if __name__ == "__main__":
-  # Hypod can be created in the same manner as dataclass.
-  net_hp1 = NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32))
-  print(net_hp1)
-  # Hypod can be also created from parsing stringified objects.
-  net_hp2 = NetworkHP(num_layers="3", layer_hp=LayerHP("64", 32))
-  print(net_hp2)
-  # Hypod class itself can be also created from a dictionary.
-  net_hp3 = NetworkHP(num_layers=3, layer_hp=dict(in_features=64, out_features=32))
-  print(net_hp3)
+    # Hypod can be created in the same manner as dataclass.
+    net_hp1 = NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32))
+    print(net_hp1)
+    # Hypod can be also created from parsing stringified objects.
+    net_hp2 = NetworkHP(num_layers="3", layer_hp=LayerHP("64", 32))
+    print(net_hp2)
+    # Hypod class itself can be also created from a dictionary.
+    net_hp3 = NetworkHP(num_layers=3, layer_hp=dict(in_features=64, out_features=32))
+    print(net_hp3)
 
 ```
 
 ### Command-line Usage
 With the Hypod classes defined the same as above, define the main function as follows.
 
 ```python
 # main.py
 from hypod import hypod_main
 
 
 @hypod_main()  # parses sys.argv to construct the hypod in the first argument, `net_hp`
 def main(net_hp: NetworkHP):
-  print(net_hp)
+    print(net_hp)
 
 
 if __name__ == "__main__":
-  main()
+    main()
 ```
-Then, in the command-line type as follows to obtain the same results as before.
+Then, on the command-line, type as follows to obtain the same results as before.
 `python main.py num_layers=3 layer_hp.in_features=64 layer_hp.out_features=32`
 
 
 ### Inheritance
 Hypod can be subclassed with a **tag**.
 
 ```python
@@ -98,72 +98,72 @@
 
 from hypod import hypod
 
 
 @dataclass
 @hypod
 class Data:
-  path: str
-  batch_size: int = 4
+    path: str
+    batch_size: int = 4
 
 
 @dataclass
 @hypod
 class FFHQData(Data, tag="ffhq"):
-  path: str = "/path/to/FFHQ"
-  meta: str = "Flicker-Faces HQ Data, containing 70k images"
+    path: str = "/path/to/FFHQ"
+    meta: str = "Flicker-Faces HQ Data, containing 70k images"
 
 
 @dataclass
 @hypod
 class FFHQDataLargeBatch(FFHQData, tag="ffhq_lg"):
-  batch_size: int = 16
+    batch_size: int = 16
 
 
 @dataclass
 @hypod
 class Model:
-  data: Data
-  net: NetworkHP
+    data: Data
+    net: NetworkHP
 
 
 if __name__ == "__main__":
-  model_with_ffhq = Model(
-    data="ffhq", net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
-  )
-  print(model_with_ffhq)
-
-  model_with_ffhq_lg = Model(
-    data=dict(_tag="ffhq_lg"),  # Also can be created from dict with "_tag" key.
-    net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
-  )
-  print(model_with_ffhq_lg)
-
-  model_with_cifar10 = Model(
-    data=dict(path="/path/to/cifar10"),
-    net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
-  )
-  print(model_with_cifar10)
+    model_with_ffhq = Model(
+        data="ffhq", net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
+    )
+    print(model_with_ffhq)
+
+    model_with_ffhq_lg = Model(
+        data=dict(_tag="ffhq_lg"),  # Also can be created from dict with "_tag" key.
+        net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
+    )
+    print(model_with_ffhq_lg)
+
+    model_with_cifar10 = Model(
+        data=dict(path="/path/to/cifar10"),
+        net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
+    )
+    print(model_with_cifar10)
 ```
 
 ### Command-line Usage with Inheritance
 With the Hypod classes defined the same as above, define the main function as follows.
 
 ```python
 # main.py
 from hypod import hypod_main
 
 
-@hypod_main()  # parses sys.argv to construct the hypod in the first argument, `net_hp`
+@hypod_main()  # parses sys.argv to construct the hypod in the first argument, `model`
 def main(model: Model):
-  print(model)
+    print(model)
 
 
 if __name__ == "__main__":
-  main()
+    main()
 ```
 Then, in the command-line type as follows to obtain the same results as before.
 `python main.py model.data=ffhq model.net.num_layers=3 model.net.layer_hp.in_features=64 model.net.layer_hp.out_features=32`
 I.e., tag can be fed in the CLI as the root argument.
 
 ### Advanced Usage (Value Interpolation)
 * Please refer to `advanced_usage.py` in the `examples` directory.
@@ -177,10 +177,10 @@
 * (Q) Is `typing.Union` supported? 
   * (A) Yes. But when it is a union of `str` or `dict`, there are ambiguities in parsing the stringified objects. A warning or an error will be raised in this case.
 * (Q) Does tag-based creation still work when `typing.Union` is used?
   * (A) Yes. The tag search will be done over all the types in the union.
 * (Q) Are `typing.List` or other generic types supported?
   * (A) Yes.
 * (Q) How can I use value interpolation?
-  * (A) `dataclass` provides `__post_init__()` function where you can define a .
+  * (A) `dataclass` provides [`__post_init__()`](https://docs.python.org/3/library/dataclasses.html#post-init-processing) function where you can define interpolation rules in *Python*. E.g., if you want to make a hyperparameter `a` that has to be twice the value of `b` in some Hypod, write `self.a = 2 * self.b` in `__post_init__()` of that Hypod.
 * (Q) Why not using `typing.dataclass_transform()` in implementing Hypod?
   * (A) Because requirement of Python>=3.11 is too strict for now.
```

### Comparing `hypod-0.0.1/hypod/decor.py` & `hypod-0.0.2/hypod/decor.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,39 +55,39 @@
                     if not len(_intersects) == 0:
                         raise ValueError(
                             f"The type {datacls} has duplicate tags: {_intersects}"
                         )
                     _keys.update(_new_keys)
             # Warn if datacls is Union[dict, Hypod]
             if dict in get_args(datacls):
-                warnings.warn(
+                raise ValueError(
                     "Hypod class can be constructed from dict, "
-                    "and thus making a Union with dict is not a good idea. "
-                    "Here, if a dict value is given without '_tag' key,"
-                    "it will be considered as plain 'dict'."
+                    "and thus making a Union with dict is prohibited. "
                 )
         self._datacls = datacls
         self._objcls = objcls
 
     @property
     def name(self):
         return self._name[1:]
 
     @property
     def default(self):
         if isinstance(self._default, Field):
+            if (self._default.default is MISSING) == (
+                self._default.default_factory is MISSING
+            ):
+                raise ValueError(
+                    "Only one of 'default' or 'default_factory' should be defined."
+                )
+
             if self._default.default is not MISSING:
                 default_val = self._default.default
             if self._default.default_factory is not MISSING:
-                assert (
-                    self._default.default is MISSING
-                ), "Only one of 'default' or 'default_factory' should be defined."
                 default_val = self._default.default_factory()
-            else:
-                default_val = MISSING
         else:
             default_val = self._default
         return default_val
 
     def _check_if_MISSING(self, val):
         if val is MISSING:
             raise ValueError(
@@ -120,40 +120,56 @@
 
         # Handle Hypod objects
         if isinstance(val, dict):
             if is_hypod(self._datacls):
                 if "_tag" in val:  # class hint is given by _tag
                     cls = self._datacls._subclasses[val["_tag"]]
                     val.pop("_tag")
-                else:  # no class hint; use the annotated class
-                    cls = self._datacls
-                if self.update_if_hypod and self.default is not MISSING:
+                else:  # no class hint
+                    if self.default is not MISSING:  # use the class of default
+                        cls = type(self.default)
+                    else:
+                        cls = self._datacls
+
+                if (
+                    self.update_if_hypod
+                    and self.default is not MISSING
+                    and cls is type(self.default)
+                ):
                     val = replace(self.default, **val)
                 else:
                     val = cls(**val)
+
             elif is_union_of_hypod(self._datacls):
                 if "_tag" in val:
                     # merge _subclasses dicts
                     _all_subclasses = {
                         k: v
                         for _datacls in get_args(self._datacls)
                         if is_hypod(_datacls)
                         for k, v in _datacls._subclasses.items()
                     }
                     cls = _all_subclasses[val["_tag"]]
                     val.pop("_tag")
-                elif dict in get_args(self._datacls):
-                    cls = dict
-                else:
-                    raise ValueError(
-                        "A dict is given to construct a Hypod without a _tag key. "
-                        "Since the attribute type annotation is Union, "
-                        "its class cannot be determined."
-                    )
-                if self.update_if_hypod and self.default is not MISSING:
+                else:  # no class hint
+                    if self.default is not MISSING:  # use the class of default
+                        cls = type(self.default)
+                    else:
+                        raise ValueError(
+                            f"A dict is given to construct Hypod field '{self.name}' "
+                            "without a _tag key, while no default value has been set. "
+                            "Since the attribute type annotation is Union "
+                            f"'{self._datacls}', "
+                            "its class cannot be determined."
+                        )
+                if (
+                    self.update_if_hypod
+                    and self.default is not MISSING
+                    and cls is type(self.default)
+                ):
                     val = replace(self.default, **val)
                 else:
                     val = cls(**val)
 
         # Check type and set value
         self._check_type(val)
         setattr(obj, self._name, val)
```

### Comparing `hypod-0.0.1/hypod/main.py` & `hypod-0.0.2/hypod/main.py`

 * *Files identical despite different names*

### Comparing `hypod-0.0.1/hypod/parser.py` & `hypod-0.0.2/hypod/parser.py`

 * *Files identical despite different names*

### Comparing `hypod-0.0.1/hypod.egg-info/PKG-INFO` & `hypod-0.0.2/hypod.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypod
-Version: 0.0.1
+Version: 0.0.2
 Summary: Hypod: A dataclass-based hyperparameter managing system
 Author-email: Jiseob Kim <justjest@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jiseob Kim
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,43 +32,43 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hypod: A dataclass-based hyperparameter managing system
 
 ## Overview
-Deep learning models are often composed of multiple networks, where each of the networks is composed of multiple layers, and the class of each layer or its hyperparameters differ by experiments. `Hypod` simplifies managing this complex hierarchy of hyperparameters utilizing the built-in `dataclass`.
+Deep learning models are often composed of multiple networks, where each of the networks is composed of multiple layers, and the class of each layer or its hyperparameters differ by experiments. `Hypod` simplifies managing this complex hierarchy of hyperparameters utilizing the built-in [`dataclass`](https://docs.python.org/3/library/dataclasses.html).
 
-The `dataclass` derives the following benefits.
+`dataclass` derives the following benefits.
 * Defining a group of hyperaparameters is easy with **type annotation** support.
 * Creating it is easy with the auto-defined `__init__`.
 * Many IDE's (e.g., PyCharm, VSCode) support "jump to the definition".
 
 However, difficulties for using it "as-is" in hyperparameter-managing are:
 * Handling nested dataclasses is not so good.
-* Parsing the strings or sys.argv to create a dataclass is not natively supported.
+* Parsing strings or sys.argv to create a dataclass is not natively supported.
 * Switching between multiple child dataclasses using a simple "tag" is cumbersome.
 
 `Hypod` will handle all these difficulties for you with following advantages.
-* Fast, lightweight implementation using the built-in `dataclass` and descriptors
+* Fast, lightweight implementation using the built-in `dataclass` and [descriptors](https://docs.python.org/3/howto/descriptor.html)
 * Minimal dependency
 * Type-checking (based on annotation)
 * Parsing a stringified object or YAML to create the corresponding nested dataclass
 * Ability to auto-make the corresponding module (e.g., layer, network), when defined as an inner class of that module.
 
 ### Comparison with other packages
 * [Hydra](https://github.com/facebookresearch/hydra): Hydra is a popular package with the same purpose. Its _structured config_ mode allows defining a config with `dataclass` as well. However, Hydra converts a config into `DictConfig` object (from another package `omegaconf`) even when it is originally defined with `dataclass`. Thus, all the operations (modifying, getting values, merging) are done with `DictConfig` and this brings the following drawbacks compared to Hypod, which uses `dataclass` object all the time.
   * `DictConfig` is not type annotated.
   * "Go to the definition" in IDE cannot be done with `DictConfig`.
   * Inheritance strcuture of configs cannot be checked.
-  * Complex value interpolation is difficult or impossible to implement. In Hypod `dataclass`, it can be done using built-in `__post_init__()` function (see `examples/advanced_usage.py`).
+  * Complex value interpolation is difficult or impossible to implement. In Hypod `dataclass`, it can be done using built-in [`__post_init__()`](https://docs.python.org/3/library/dataclasses.html#post-init-processing) function (see `examples/advanced_usage.py`).
 
 
 ### Etymology
-Hypod stands for **"A Pot of Hyperparameters, or A Hyperparameters-Pot"**. You can put various Hyperparameters in a Pot and mix them with others as you wish.
+Hypod stands for **"A Pod of Hyperparameters, or A Hyperparameters-Pod"**. You can put various Hyperparameters as a Pod and compose them with other Pods as you wish.
 
 ## Quick start
 ### Install the package
 `pip install hypod`
 
 ### Basic Usage
 
@@ -76,56 +76,56 @@
 from dataclasses import dataclass
 from hypod import hypod
 
 
 @dataclass
 @hypod
 class LayerHP:
-  in_features: int
-  out_features: int
-  init_scale: float = 0.9
+    in_features: int
+    out_features: int
+    init_scale: float = 0.9
 
 
 @dataclass
 @hypod
 class NetworkHP:
-  num_layers: int
-  layer_hp: LayerHP
+    num_layers: int
+    layer_hp: LayerHP
 
 
 if __name__ == "__main__":
-  # Hypod can be created in the same manner as dataclass.
-  net_hp1 = NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32))
-  print(net_hp1)
-  # Hypod can be also created from parsing stringified objects.
-  net_hp2 = NetworkHP(num_layers="3", layer_hp=LayerHP("64", 32))
-  print(net_hp2)
-  # Hypod class itself can be also created from a dictionary.
-  net_hp3 = NetworkHP(num_layers=3, layer_hp=dict(in_features=64, out_features=32))
-  print(net_hp3)
+    # Hypod can be created in the same manner as dataclass.
+    net_hp1 = NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32))
+    print(net_hp1)
+    # Hypod can be also created from parsing stringified objects.
+    net_hp2 = NetworkHP(num_layers="3", layer_hp=LayerHP("64", 32))
+    print(net_hp2)
+    # Hypod class itself can be also created from a dictionary.
+    net_hp3 = NetworkHP(num_layers=3, layer_hp=dict(in_features=64, out_features=32))
+    print(net_hp3)
 
 ```
 
 ### Command-line Usage
 With the Hypod classes defined the same as above, define the main function as follows.
 
 ```python
 # main.py
 from hypod import hypod_main
 
 
 @hypod_main()  # parses sys.argv to construct the hypod in the first argument, `net_hp`
 def main(net_hp: NetworkHP):
-  print(net_hp)
+    print(net_hp)
 
 
 if __name__ == "__main__":
-  main()
+    main()
 ```
-Then, in the command-line type as follows to obtain the same results as before.
+Then, on the command-line, type as follows to obtain the same results as before.
 `python main.py num_layers=3 layer_hp.in_features=64 layer_hp.out_features=32`
 
 
 ### Inheritance
 Hypod can be subclassed with a **tag**.
 
 ```python
@@ -133,72 +133,72 @@
 
 from hypod import hypod
 
 
 @dataclass
 @hypod
 class Data:
-  path: str
-  batch_size: int = 4
+    path: str
+    batch_size: int = 4
 
 
 @dataclass
 @hypod
 class FFHQData(Data, tag="ffhq"):
-  path: str = "/path/to/FFHQ"
-  meta: str = "Flicker-Faces HQ Data, containing 70k images"
+    path: str = "/path/to/FFHQ"
+    meta: str = "Flicker-Faces HQ Data, containing 70k images"
 
 
 @dataclass
 @hypod
 class FFHQDataLargeBatch(FFHQData, tag="ffhq_lg"):
-  batch_size: int = 16
+    batch_size: int = 16
 
 
 @dataclass
 @hypod
 class Model:
-  data: Data
-  net: NetworkHP
+    data: Data
+    net: NetworkHP
 
 
 if __name__ == "__main__":
-  model_with_ffhq = Model(
-    data="ffhq", net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
-  )
-  print(model_with_ffhq)
-
-  model_with_ffhq_lg = Model(
-    data=dict(_tag="ffhq_lg"),  # Also can be created from dict with "_tag" key.
-    net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
-  )
-  print(model_with_ffhq_lg)
-
-  model_with_cifar10 = Model(
-    data=dict(path="/path/to/cifar10"),
-    net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
-  )
-  print(model_with_cifar10)
+    model_with_ffhq = Model(
+        data="ffhq", net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
+    )
+    print(model_with_ffhq)
+
+    model_with_ffhq_lg = Model(
+        data=dict(_tag="ffhq_lg"),  # Also can be created from dict with "_tag" key.
+        net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
+    )
+    print(model_with_ffhq_lg)
+
+    model_with_cifar10 = Model(
+        data=dict(path="/path/to/cifar10"),
+        net=NetworkHP(num_layers=3, layer_hp=LayerHP(64, 32)),
+    )
+    print(model_with_cifar10)
 ```
 
 ### Command-line Usage with Inheritance
 With the Hypod classes defined the same as above, define the main function as follows.
 
 ```python
 # main.py
 from hypod import hypod_main
 
 
-@hypod_main()  # parses sys.argv to construct the hypod in the first argument, `net_hp`
+@hypod_main()  # parses sys.argv to construct the hypod in the first argument, `model`
 def main(model: Model):
-  print(model)
+    print(model)
 
 
 if __name__ == "__main__":
-  main()
+    main()
 ```
 Then, in the command-line type as follows to obtain the same results as before.
 `python main.py model.data=ffhq model.net.num_layers=3 model.net.layer_hp.in_features=64 model.net.layer_hp.out_features=32`
 I.e., tag can be fed in the CLI as the root argument.
 
 ### Advanced Usage (Value Interpolation)
 * Please refer to `advanced_usage.py` in the `examples` directory.
@@ -212,10 +212,10 @@
 * (Q) Is `typing.Union` supported? 
   * (A) Yes. But when it is a union of `str` or `dict`, there are ambiguities in parsing the stringified objects. A warning or an error will be raised in this case.
 * (Q) Does tag-based creation still work when `typing.Union` is used?
   * (A) Yes. The tag search will be done over all the types in the union.
 * (Q) Are `typing.List` or other generic types supported?
   * (A) Yes.
 * (Q) How can I use value interpolation?
-  * (A) `dataclass` provides `__post_init__()` function where you can define a .
+  * (A) `dataclass` provides [`__post_init__()`](https://docs.python.org/3/library/dataclasses.html#post-init-processing) function where you can define interpolation rules in *Python*. E.g., if you want to make a hyperparameter `a` that has to be twice the value of `b` in some Hypod, write `self.a = 2 * self.b` in `__post_init__()` of that Hypod.
 * (Q) Why not using `typing.dataclass_transform()` in implementing Hypod?
   * (A) Because requirement of Python>=3.11 is too strict for now.
```

### Comparing `hypod-0.0.1/pyproject.toml` & `hypod-0.0.2/pyproject.toml`

 * *Files identical despite different names*


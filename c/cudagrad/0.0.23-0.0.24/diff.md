# Comparing `tmp/cudagrad-0.0.23.tar.gz` & `tmp/cudagrad-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudagrad-0.0.23.tar", last modified: Mon Jul 24 23:48:40 2023, max compression
+gzip compressed data, was "cudagrad-0.0.24.tar", last modified: Wed Jul 26 04:07:25 2023, max compression
```

## Comparing `cudagrad-0.0.23.tar` & `cudagrad-0.0.24.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 23:48:40.841282 cudagrad-0.0.23/
--rw-r--r--   0 ryan       (501) staff       (20)       44 2023-07-18 06:47:23.000000 cudagrad-0.0.23/MANIFEST.in
--rw-r--r--   0 ryan       (501) staff       (20)     3619 2023-07-24 23:48:40.841146 cudagrad-0.0.23/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     3117 2023-07-19 01:34:52.000000 cudagrad-0.0.23/README.md
--rw-r--r--   0 ryan       (501) staff       (20)      724 2023-07-24 23:47:25.000000 cudagrad-0.0.23/pyproject.toml
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-24 23:48:40.841332 cudagrad-0.0.23/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     1592 2023-07-18 02:40:23.000000 cudagrad-0.0.23/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 23:48:40.839745 cudagrad-0.0.23/src/
--rw-r--r--   0 ryan       (501) staff       (20)     3857 2023-07-24 23:43:55.000000 cudagrad-0.0.23/src/bindings.cpp
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 23:48:40.840749 cudagrad-0.0.23/src/cudagrad.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3619 2023-07-24 23:48:40.000000 cudagrad-0.0.23/src/cudagrad.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      318 2023-07-24 23:48:40.000000 cudagrad-0.0.23/src/cudagrad.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-24 23:48:40.000000 cudagrad-0.0.23/src/cudagrad.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-18 02:46:33.000000 cudagrad-0.0.23/src/cudagrad.egg-info/not-zip-safe
--rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-24 23:48:40.000000 cudagrad-0.0.23/src/cudagrad.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-24 23:48:40.000000 cudagrad-0.0.23/src/cudagrad.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)    23588 2023-07-24 23:47:23.000000 cudagrad-0.0.23/src/cudagrad.hpp
--rw-r--r--   0 ryan       (501) staff       (20)      171 2023-07-18 06:46:23.000000 cudagrad-0.0.23/src/ops.cu
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-24 23:48:40.840868 cudagrad-0.0.23/tests/
--rw-r--r--   0 ryan       (501) staff       (20)     1050 2023-07-19 01:21:03.000000 cudagrad-0.0.23/tests/test.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-26 04:07:25.248241 cudagrad-0.0.24/
+-rw-r--r--   0 ryan       (501) staff       (20)       44 2023-07-18 06:47:23.000000 cudagrad-0.0.24/MANIFEST.in
+-rw-r--r--   0 ryan       (501) staff       (20)     3672 2023-07-26 04:07:25.248117 cudagrad-0.0.24/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     3170 2023-07-25 01:40:28.000000 cudagrad-0.0.24/README.md
+-rw-r--r--   0 ryan       (501) staff       (20)      724 2023-07-26 04:07:05.000000 cudagrad-0.0.24/pyproject.toml
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-26 04:07:25.248288 cudagrad-0.0.24/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     1592 2023-07-18 02:40:23.000000 cudagrad-0.0.24/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-26 04:07:25.246577 cudagrad-0.0.24/src/
+-rw-r--r--   0 ryan       (501) staff       (20)     2903 2023-07-26 04:06:37.000000 cudagrad-0.0.24/src/bindings.cpp
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-26 04:07:25.247690 cudagrad-0.0.24/src/cudagrad.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3672 2023-07-26 04:07:25.000000 cudagrad-0.0.24/src/cudagrad.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      318 2023-07-26 04:07:25.000000 cudagrad-0.0.24/src/cudagrad.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-26 04:07:25.000000 cudagrad-0.0.24/src/cudagrad.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-18 02:46:33.000000 cudagrad-0.0.24/src/cudagrad.egg-info/not-zip-safe
+-rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-26 04:07:25.000000 cudagrad-0.0.24/src/cudagrad.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-26 04:07:25.000000 cudagrad-0.0.24/src/cudagrad.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)    20539 2023-07-26 00:22:18.000000 cudagrad-0.0.24/src/cudagrad.hpp
+-rw-r--r--   0 ryan       (501) staff       (20)      263 2023-07-26 03:31:20.000000 cudagrad-0.0.24/src/ops.cu
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-26 04:07:25.247835 cudagrad-0.0.24/tests/
+-rw-r--r--   0 ryan       (501) staff       (20)     1050 2023-07-19 01:21:03.000000 cudagrad-0.0.24/tests/test.py
```

### Comparing `cudagrad-0.0.23/PKG-INFO` & `cudagrad-0.0.24/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.23
+Version: 0.0.24
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <moorethreads@hey.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
 # cudagrad
 
 A small autograd engine
 
-![](parallel_1_20.png)
+Work In Progress! TODO: CUDA operation integration and release on PyPI 🙃
 
 ## Example
 
 ```cpp
 // c++ -std=c++11 -I./src examples/example.cpp && ./a.out
 #include "cudagrad.hpp"
 int main() {
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cudagrad-0.0.23/README.md` & `cudagrad-0.0.24/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # cudagrad
 
 A small autograd engine
 
-![](parallel_1_20.png)
+Work In Progress! TODO: CUDA operation integration and release on PyPI 🙃
 
 ## Example
 
 ```cpp
 // c++ -std=c++11 -I./src examples/example.cpp && ./a.out
 #include "cudagrad.hpp"
 int main() {
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cudagrad-0.0.23/pyproject.toml` & `cudagrad-0.0.24/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=40.8.0", "wheel", "pybind11>=2.10.1", "toml",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cudagrad"
-version = "0.0.23"
+version = "0.0.24"
 description = "A small autograd engine"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "Operating System :: OS Independent",]
 dependencies = [ "micrograd",]
 [[project.authors]]
 name = "Ryan Moore"
```

### Comparing `cudagrad-0.0.23/setup.py` & `cudagrad-0.0.24/setup.py`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.23/src/bindings.cpp` & `cudagrad-0.0.24/src/bindings.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,37 @@
+// If the implementation is easy to explain, it may be a good idea.
+//
+// Tim Peters
+
 #include <sstream>
 #include "cudagrad.hpp"
 
 #include <pybind11/stl.h>
 #include <pybind11/pybind11.h>
 
 #define STRINGIFY(x) #x
 #define MACRO_STRINGIFY(x) STRINGIFY(x)
 
-int add(int i, int j) {
-    return i + j;
-}
-
 namespace py = pybind11;
 
 PYBIND11_MODULE(cudagrad, m) {
     m.doc() = R"pbdoc(
         Pybind11 example plugin
         -----------------------
 
         .. currentmodule:: cudagrad
 
         .. autosummary::
            :toctree: _generate
 
-           add
-           subtract
+        hello
+        tensor
+        Tensor
     )pbdoc";
 
-    m.def("add", &add, R"pbdoc(
-        Add two numbers
-
-        Some other explanation about the add function.
-    )pbdoc");
-
-    m.def("subtract", [](int i, int j) { return i - j; }, R"pbdoc(
-        Subtract two numbers
-
-        Some other explanation about the subtract function.
-    )pbdoc");
-
-    m.def("foo", &cg::foo, R"pbdoc(
-        Add one
-
-        Why is this here?
-    )pbdoc");
-
     m.def("hello", &cg::hello, R"pbdoc(
         Can has CUDA?
 
         Hello!
     )pbdoc");
 
     m.def("tensor", [](std::vector<int> sizes, std::vector<float> values) {
@@ -87,27 +70,13 @@
         })
         .def("__repr__", [](std::shared_ptr<cg::Tensor> t) {
             std::ostringstream os;
             os << t;
             return os.str();
         });
 
-    // // Add the stream output operator if you want to print your Tensor object in Python.
-    // py::class_<std::ostream>(m, "ostream")
-    //     .def(py::self_ns::str(py::self_ns::self))
-    //     .def(py::self_ns::repr(py::self_ns::self));
-
-    // m.def("__lshift__", [](std::ostream &os, const std::shared_ptr<cg::Tensor> &t) -> std::ostream& {
-    //     os << t; return os;
-    // }, py::is_operator());
-
-    // m.def("tensor", [](std::vector<int> size, std::vector<float> data) {
-    //     return cg::tensor(size, data);
-    // }, R"pbdoc(Magic tensor)pbdoc", py::arg("sizes"), py::arg("values"));
-
-
 #ifdef VERSION_INFO
     m.attr("__version__") = MACRO_STRINGIFY(VERSION_INFO);
 #else
     m.attr("__version__") = "dev";
 #endif
 }
```

### Comparing `cudagrad-0.0.23/src/cudagrad.egg-info/PKG-INFO` & `cudagrad-0.0.24/src/cudagrad.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.23
+Version: 0.0.24
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <moorethreads@hey.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
 # cudagrad
 
 A small autograd engine
 
-![](parallel_1_20.png)
+Work In Progress! TODO: CUDA operation integration and release on PyPI 🙃
 
 ## Example
 
 ```cpp
 // c++ -std=c++11 -I./src examples/example.cpp && ./a.out
 #include "cudagrad.hpp"
 int main() {
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cudagrad-0.0.23/src/cudagrad.hpp` & `cudagrad-0.0.24/src/cudagrad.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 //
 // "If you remember just one thing out of this course, it should be this – two
 // pieces of advice. The first piece of advice is whenever you can, use vector.
 // The second piece of advice is if you cannot, find a way how you can. This is
 // to avoid any data structures except arrays... Vector is an array, right. Sort
 // of, you say, 'Well... Aren't there exceptions?' – Yes, not for you!"
 //
-// — Alexander Stepanov
+// Alexander Stepanov
 
 #ifndef SRC_CUDAGRAD_HPP_
 #define SRC_CUDAGRAD_HPP_
 
 #include <algorithm>
 #include <cassert>
 #include <functional>
@@ -605,32 +605,14 @@
 using t = std::shared_ptr<Tensor>;
 
 namespace nn {
 
 // TODO(yrom1): nonlinearity of Neuron need to pass and drill down from MLP
 //              static_cast<bool>(vec_.size() - 1) something liek this for MLP
 
-/*
-class Neuron(Module):
-    def __init__(self, nin: int, nonlin: bool = True):
-        self.w = [Value(random.uniform(-1, 1)) for _ in range(nin)]
-        self.b = Value(0)
-        self.nonlin = nonlin
-
-    def __call__(self, x: Union[List[float], List[Value]]) -> Value:
-        act = sum((wi * xi for wi, xi in zip(self.w, x)), self.b)
-        return act.relu() if self.nonlin else act
-
-    def parameters(self) -> List[Value]:
-        return self.w + [self.b]
-
-    def __repr__(self) -> str:
-        return f"{'ReLU' if self.nonlin else 'Linear'}Neuron({len(self.w)})"
-*/
-
 // keep it simple to start
 class Neuron {
  public:
   std::vector<std::shared_ptr<Tensor>> weights_;
   std::shared_ptr<Tensor> bias_;
   float rate_;
 
@@ -672,114 +654,12 @@
     bias_.get()->data_[0] =
         bias_.get()->data_[0] + ((-rate_) * bias_.get()->grad_[0]);
     // std::cout << "bias after: " << bias_.get()->data_[0] << std::endl;
   }
   // TODO(yrom1) parameters, how do i make this like std iterator?
 };
 
-/*
-class Layer(Module):
-
-    def __init__(self, nin, nout, **kwargs):
-        self.neurons = [Neuron(nin, **kwargs) for _ in range(nout)]
-
-    def __call__(self, x):
-        out = [n(x) for n in self.neurons]
-        return out[0] if len(out) == 1 else out
-
-    def parameters(self):
-        return [p for n in self.neurons for p in n.parameters()]
-
-    def __repr__(self):
-        return f"Layer of [{', '.join(str(n) for n in self.neurons)}]"
-*/
-
-struct Layer {
-  int nin_;
-  int nout_;
-  float rate_;
-  std::vector<Neuron> neurons_;
-  Layer(int nin, int nout, float rate) : nin_(nin), nout_(nout), rate_(rate) {
-    for (int i = 0; i < nout_; ++i) {
-      neurons_.push_back(Neuron(nin_, rate_));
-    }
-    assert(neurons_.size() == nout_);
-  }
-
-  std::vector<std::shared_ptr<Tensor>> operator()(
-      std::vector<std::shared_ptr<Tensor>> x) {
-    std::vector<std::shared_ptr<Tensor>> ans;
-    for (auto &neuron : neurons_) {
-      ans.push_back(neuron(x));
-    }
-    return ans;
-  }
-
-  void train() {
-    for (auto &neuron : neurons_) {
-      neuron.train();
-    }
-  }
-};
-
-/*
-class MLP(Module):
-
-    def __init__(self, nin, nouts):
-        sz = [nin] + nouts
-        self.layers = [Layer(sz[i], sz[i+1], nonlin=i!=len(nouts)-1) for i in
-range(len(nouts))]
-
-    def __call__(self, x):
-        for layer in self.layers:
-            x = layer(x)
-        return x
-
-    def parameters(self):
-        return [p for layer in self.layers for p in layer.parameters()]
-
-    def __repr__(self):
-        return f"MLP of [{', '.join(str(layer) for layer in self.layers)}]"
-*/
-
-struct MLP {
-  int nin_;
-  std::vector<int> nouts_;
-  float rate_;
-  std::vector<int> sz_;
-  std::vector<Layer> layers_;
-  MLP(int nin, std::vector<int> nouts, float rate)
-      : nin_(nin), nouts_(nouts), rate_(rate) {
-    sz_.push_back(nin);
-    for (auto &x : nouts_) {  // TODO(yrom1) extend c++?
-      sz_.push_back(x);
-    }
-
-    for (int i = 0; i < nouts_.size(); ++i) {
-      layers_.push_back(
-          Layer(sz_[i], sz_[i + 1], rate_));  // len(sz) == len(nouts_) + 1
-    }
-  }
-
-  std::vector<std::shared_ptr<Tensor>> operator()(
-      std::vector<std::shared_ptr<Tensor>> x) {
-    // because we didnt make things not a vector aribtarily in Layer this is
-    // easy
-    std::vector<std::shared_ptr<Tensor>> ans = x;
-    for (auto &layer : layers_) {
-      ans = layer(ans);
-    }
-    return ans;
-  }
-
-  void train() {
-    for (auto &layer : layers_) {
-      layer.train();
-    }
-  }
-};
-
 }  // namespace nn
 
 }  // namespace cg
 
 #endif  // SRC_CUDAGRAD_HPP_
```

### Comparing `cudagrad-0.0.23/tests/test.py` & `cudagrad-0.0.24/tests/test.py`

 * *Files identical despite different names*


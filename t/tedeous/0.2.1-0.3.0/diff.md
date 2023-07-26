# Comparing `tmp/tedeous-0.2.1.tar.gz` & `tmp/tedeous-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tedeous-0.2.1.tar", last modified: Thu Jul  6 13:22:11 2023, max compression
+gzip compressed data, was "tedeous-0.3.0.tar", last modified: Wed Jul 26 10:35:39 2023, max compression
```

## Comparing `tedeous-0.2.1.tar` & `tedeous-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:11.774417 tedeous-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-06 13:22:06.000000 tedeous-0.2.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-06 13:22:11.774417 tedeous-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-06 13:22:06.000000 tedeous-0.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 13:22:11.774417 tedeous-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-06 13:22:06.000000 tedeous-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:11.770417 tedeous-0.2.1/tedeous/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16374 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/derivative.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/finite_diffs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24639 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/input_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/points_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:11.770417 tedeous-0.2.1/tedeous.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-06 13:22:11.000000 tedeous-0.2.1/tedeous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-06 13:22:11.000000 tedeous-0.2.1/tedeous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:22:11.000000 tedeous-0.2.1/tedeous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 13:22:11.000000 tedeous-0.2.1/tedeous.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:35:39.254169 tedeous-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-26 10:35:32.000000 tedeous-0.3.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-26 10:35:39.254169 tedeous-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-26 10:35:32.000000 tedeous-0.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 10:35:39.254169 tedeous-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-26 10:35:32.000000 tedeous-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:35:39.254169 tedeous-0.3.0/tedeous/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/derivative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10749 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/finite_diffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25476 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/input_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/points_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17556 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-26 10:35:32.000000 tedeous-0.3.0/tedeous/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:35:39.254169 tedeous-0.3.0/tedeous.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-26 10:35:39.000000 tedeous-0.3.0/tedeous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-26 10:35:39.000000 tedeous-0.3.0/tedeous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 10:35:39.000000 tedeous-0.3.0/tedeous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 10:35:39.000000 tedeous-0.3.0/tedeous.egg-info/top_level.txt
```

### Comparing `tedeous-0.2.1/LICENCE` & `tedeous-0.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `tedeous-0.2.1/PKG-INFO` & `tedeous-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tedeous
-Version: 0.2.1
+Version: 0.3.0
 Summary: TEDEouS - Torch Exhaustive Differential Equations Solver. Differential equation solver, based on pytorch library
 Author: Alexander Hvatov
 Author-email: itmo.nss.team@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tedeous-0.2.1/README.rst` & `tedeous-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `tedeous-0.2.1/setup.py` & `tedeous-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 def get_requirements():
     requirements = extract_requirements('requirements.txt')
     return requirements
 
 setup(
     name = 'tedeous',
-    version= '0.2.1' ,
+    version= '0.3.0' ,
     description = 'TEDEouS - Torch Exhaustive Differential Equations Solver. Differential equation solver, based on pytorch library',
     long_description = 'Combine power of pytorch, numerical methods and math overall to conquer and solve ALL {O,P}DEs. There are some examples to provide a little insight to an operator form',
     author = 'Alexander Hvatov',
     author_email = 'itmo.nss.team@gmail.com', # add email
     classifiers = [      
               'Development Status :: 3 - Alpha',
               'Programming Language :: Python :: 3',
```

### Comparing `tedeous-0.2.1/tedeous/cache.py` & `tedeous-0.3.0/tedeous/cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 import glob
 import numpy as np
 
 from copy import deepcopy
 from typing import Union, Tuple, Any
 
-from tedeous.metrics import Solution
+from tedeous.solution import Solution
 from tedeous.input_preprocessing import Equation, EquationMixin
 from tedeous.device import device_type
 
 
 def count_output(model):
     modules, output_layer = list(model.modules()), None
     for layer in reversed(modules):
@@ -33,27 +33,50 @@
         if type(m) == torch.nn.Linear or type(m) == torch.nn.Conv2d:
             m.weight.data = m.weight.data + \
                             (2 * torch.randn(m.weight.size()) - 1) * eps
             m.bias.data = m.bias.data + (2 * torch.randn(m.bias.size()) - 1) * eps
 
     return randomize_params
 
+def remove_all_files(folder):
+    for filename in os.listdir(folder):
+        file_path = os.path.join(folder, filename)
+        try:
+            if os.path.isfile(file_path) or os.path.islink(file_path):
+                os.unlink(file_path)
+            elif os.path.isdir(file_path):
+                shutil.rmtree(file_path)
+        except Exception as e:
+            print('Failed to delete %s. Reason: %s' % (file_path, e))
 
 class Model_prepare():
     """
     Prepares initial model. Serves for computing acceleration.\n
     Saves the trained model to the cache, and subsequently it is possible to use pre-trained model (if \\\
     it saved and if the new model is structurally similar) to sped up computing.\n
     If there isn't pre-trained model in cache, the training process will start from the beginning.
     """
-    def __init__(self, grid, equal_cls, model, mode):
+    def __init__(self, grid, equal_cls, model, mode, weak_form):
         self.grid = grid
         self.equal_cls = equal_cls
         self.model = model
         self.mode = mode
+        self.weak_form = weak_form
+        self.cache_dir=os.path.normpath((os.path.join(os.path.dirname( __file__ ), '..','cache')))
+
+    def change_cache_dir(self,string):
+        self.cache_dir=string
+        return None
+
+    def clear_cache_dir(self,directory=None):
+        if directory==None:
+            remove_all_files(self.cache_dir)
+        else:
+            remove_all_files(directory)
+        return None
 
     @staticmethod
     def cache_files(files, nmodels):
 
         # at some point we may want to reduce the number of models that are
         # checked for the best in the cache
         if nmodels == None:
@@ -104,37 +127,38 @@
             init_model[0]
         except:
             init_model = init_model.model
         
         return init_model, model
         
 
-    def cache_lookup(self, lambda_bound: float = 0.001, weak_form: None = None, cache_dir: str = '../cache/',
+    def cache_lookup(self, lambda_operator: float = 1., lambda_bound: float = 0.001,
                 nmodels: Union[int, None] = None, save_graph: bool = False, cache_verbose: bool = False) -> Tuple[dict, torch.Tensor]:
         """
         Looking for a saved cache.
         Args:
             lambda_bound: an arbitrary chosen constant, influence only convergence speed.
             save_graph: boolean constant, responsible for saving the computational graph.
             cache_dir: directory where saved cache in.
             nmodels: maximal number of models that are looked before optimization
             cache_verbose: more detailed info about models in cache.
         Returns:
             * **best_checkpoint** -- best model with optimizator state.\n
             * **min_loss** -- minimum error in pre-trained error.
         """
-        files = glob.glob(cache_dir + '*.tar')
+        files = glob.glob(self.cache_dir + '\*.tar')
         if len(files) == 0:
             best_checkpoint = None
             min_loss = np.inf
             return best_checkpoint, min_loss
 
         cache_n = self.cache_files(files, nmodels)
 
         min_loss = np.inf
+        min_norm_loss =np.inf
         best_checkpoint = {}
 
         device = device_type()
 
         for i in cache_n:
             file = files[i]
             checkpoint = torch.load(file)
@@ -147,52 +171,62 @@
             if cache_model[0].in_features != solver_model[0].in_features:
                 continue
             try:
                 if count_output(model) != count_output(self.model):
                     continue
             except Exception:
                 continue
+
             model = model.to(device)
-            loss = Solution(self.grid, self.equal_cls, model, self.mode). \
-                loss_evaluation(lambda_bound=lambda_bound, weak_form=weak_form, save_graph=save_graph)
+            loss, loss_normalized = Solution(self.grid, self.equal_cls,
+                                      model, self.mode, self.weak_form,
+                                      lambda_operator, lambda_bound).evaluate(save_graph=save_graph)
+
             if loss < min_loss:
                 min_loss = loss
+                min_norm_loss=loss_normalized
                 best_checkpoint['model'] = model
                 best_checkpoint['model_state_dict'] = model.state_dict()
                 best_checkpoint['optimizer_state_dict'] = \
                     checkpoint['optimizer_state_dict']
                 if cache_verbose:
-                    print('best_model_num={} , loss={}'.format(i, loss))
+                    print('best_model_num={} , normalized_loss={}'.format(i, min_norm_loss))
         if best_checkpoint == {}:
             best_checkpoint = None
             min_loss = np.inf
-        return best_checkpoint, min_loss
+        return best_checkpoint, min_norm_loss
 
-    def save_model(self, prep_model: Any, state: dict, optimizer_state: dict,
-                   cache_dir='../cache/', name: Union[str, None] = None):
+    def save_model(self, prep_model: Any, state: dict, optimizer_state: dict, name: Union[str, None] = None):
         """
         Saved model in a cache (uses for 'NN' and 'autograd' methods).
         Args:
             prep_model: model to save.
             state: a dict holding current model state (i.e., dictionary that maps each layer to its parameter tensor).
             optimizer_state: a dict holding current optimization state (i.e., values, hyperparameters).
             cache_dir: directory where saved cache in.
             name: name for a model.
         """
         if name == None:
             name = str(datetime.datetime.now().timestamp())
-        if os.path.isdir(cache_dir):
+        if not(os.path.isdir(self.cache_dir)):
+            os.mkdir(self.cache_dir)
+
+        try:
             torch.save({'model': prep_model.to('cpu'), 'model_state_dict': state,
-                        'optimizer_state_dict': optimizer_state}, cache_dir + name + '.tar')
-        else:
-            os.mkdir(cache_dir)
+                        'optimizer_state_dict': optimizer_state}, self.cache_dir+'\\' + name + '.tar')
+        except RuntimeError:
             torch.save({'model': prep_model.to('cpu'), 'model_state_dict': state,
-                        'optimizer_state_dict': optimizer_state}, cache_dir + name + '.tar')
+                        'optimizer_state_dict': optimizer_state}, self.cache_dir+'\\' + name + '.tar',_use_new_zipfile_serialization=False) #cyrrilic in path
+        else:
+            print('Cannot save model in cache')
+
+            
+            
 
-    def save_model_mat(self, cache_dir: str ='../cache/', name: None = None, cache_model: None = None):
+    def save_model_mat(self, name: None = None, cache_model: None = None):
         """
         Saved model in a cache (uses for 'mat' method).
 
         Args:
             cache_dir: a directory where saved cache in.
             name: name for a model
             cache_model: model to save
@@ -211,15 +245,15 @@
         loss = np.inf
         t = 0
         while loss > 1e-5 and t < 1e5:
             loss = optimizer.step(closure)
             t += 1
 
         self.save_model(cache_model, cache_model.state_dict(),
-                        optimizer.state_dict(), cache_dir=cache_dir, name=name)
+                        optimizer.state_dict(), cache_dir=self.cache_dir, name=name)
 
     def scheme_interp(self, trained_model: Any, cache_verbose: bool = False) -> Tuple[Any, dict]:
         """
         Smth
 
         Args:
             trained_model: smth
@@ -286,60 +320,57 @@
             cache_model = cache_checkpoint['model']
             cache_model.load_state_dict(cache_checkpoint['model_state_dict'])
             cache_model.eval()
             self.model, optimizer_state = self.scheme_interp(
                 cache_model, cache_verbose=cache_verbose)
         return self.model, optimizer_state
 
-    def cache_nn(self, cache_dir: str, nmodels: Union[int, None], lambda_bound: float,
+    def cache_nn(self, cache_dir: str, nmodels: Union[int, None], lambda_operator: float, lambda_bound: float,
               cache_verbose: bool,model_randomize_parameter: Union[float, None],
-              cache_model: torch.nn.Sequential, weak_form: None = None):
+              cache_model: torch.nn.Sequential, ):
         """
        Restores the model from the cache and uses it for retraining.
        Args:
            cache_dir: a directory where saved cache in.
            nmodels: smth
            lambda_bound: an arbitrary chosen constant, influence only convergence speed.
            cache_verbose: more detailed info about models in cache.
            model_randomize_parameter:  Creates a random model parameters (weights, biases) multiplied with a given
                                        randomize parameter.
            cache_model: cached model
-           weak_form: weak form of differential equation
        Returns:
            * **model** -- NN.\n
            * **min_loss** -- min loss as is.
        """
         r = create_random_fn(model_randomize_parameter)
-        cache_checkpoint, min_loss = self.cache_lookup(cache_dir=cache_dir,
-                                                       nmodels=nmodels,
+        cache_checkpoint, min_loss = self.cache_lookup(nmodels=nmodels,
                                                        cache_verbose=cache_verbose,
-                                                       lambda_bound=lambda_bound,
-                                                       weak_form=weak_form)
+                                                       lambda_operator= lambda_operator,
+                                                       lambda_bound=lambda_bound)
         
         self.model, optimizer_state = self.cache_retrain(cache_checkpoint,
                                                          cache_verbose=cache_verbose)
 
         self.model.apply(r)
 
         return self.model, min_loss
 
-    def cache_mat(self, cache_dir: str, nmodels: Union[int, None], lambda_bound: float,
+    def cache_mat(self, nmodels: Union[int, None],lambda_operator: float, lambda_bound: float,
               cache_verbose: bool,model_randomize_parameter: Union[float, None],
-              cache_model: torch.nn.Sequential, weak_form: None = None):
+              cache_model: torch.nn.Sequential):
         """
        Restores the model from the cache and uses it for retraining.
        Args:
            cache_dir: a directory where saved cache in.
            nmodels: smth
            lambda_bound: an arbitrary chosen constant, influence only convergence speed.
            cache_verbose: more detailed info about models in cache.
            model_randomize_parameter:  Creates a random model parameters (weights, biases) multiplied with a given
                                        randomize parameter.
            cache_model: cached model
-           weak_form: weak form of differential equation
        Returns:
            * **model** -- mat.\n
            * **min_loss** -- min loss as is.
        """
 
         NN_grid, cache_model = self.grid_model_mat(cache_model)
         operator = deepcopy(self.equal_cls.operator)
@@ -349,17 +380,17 @@
             if type(term['coeff']) == torch.Tensor:
                 term['coeff'] = term['coeff'].reshape(-1)
             elif callable(term['coeff']):
                 print("Warning: coefficient is callable,\
                                 it may lead to wrong cache item choice")
         r = create_random_fn(model_randomize_parameter)
         eq = Equation(NN_grid, operator, bconds).set_strategy('NN')
-        model_cls = Model_prepare(NN_grid, eq, cache_model, 'NN')
+        model_cls = Model_prepare(NN_grid, eq, cache_model, 'NN', self.weak_form)
         cache_checkpoint, min_loss = model_cls.cache_lookup(
-            cache_dir=cache_dir,
+            cache_dir=self.cache_dir,
             nmodels=nmodels,
             cache_verbose=cache_verbose,
             lambda_bound=lambda_bound)
         prepared_model, optimizer_state = model_cls.cache_retrain(
             cache_checkpoint,
             cache_verbose=cache_verbose)
 
@@ -368,39 +399,40 @@
         if len(self.grid.shape) == 2:
             self.model = prepared_model(NN_grid).reshape(
                 self.grid.shape).detach()
         else:
             self.model = prepared_model(NN_grid).reshape(
                 self.grid[0].shape).detach()
 
-        min_loss = Solution(self.grid, self.equal_cls, self.model, self.mode). \
-            loss_evaluation(lambda_bound=lambda_bound)
+        min_loss, _ = Solution(self.grid, self.equal_cls,
+                                      self.model, self.mode, self.weak_form,
+                                      lambda_operator, lambda_bound).evaluate()
 
         return self.model, min_loss
 
-    def cache(self, cache_dir: str, nmodels: Union[int, None], lambda_bound: float,
+    def cache(self, nmodels: Union[int, None],lambda_operator, lambda_bound: float,
               cache_verbose: bool,model_randomize_parameter: Union[float, None],
-              cache_model: torch.nn.Sequential, weak_form: None = None):
+              cache_model: torch.nn.Sequential, ):
         """
         Restores the model from the cache and uses it for retraining.
         Args:
             cache_dir: a directory where saved cache in.
-            nmodels: smth
+            nmodels: number cached models.
             lambda_bound: an arbitrary chosen constant, influence only convergence speed.
             cache_verbose: more detailed info about models in cache.
             model_randomize_parameter:  Creates a random model parameters (weights, biases) multiplied with a given
                                         randomize parameter.
             cache_model: cached model
-            weak_form: weak form of differential equation
+
         Returns:
             cache.cache_nn or cache.cache_mat
         """
 
         if self.mode != 'mat':
-            return self.cache_nn(cache_dir, nmodels, lambda_bound,
+            return self.cache_nn(self.cache_dir, nmodels,lambda_operator, lambda_bound,
                                  cache_verbose, model_randomize_parameter,
-                                 cache_model, weak_form)
+                                 cache_model)
         elif self.mode == 'mat':
-            return self.cache_mat(cache_dir, nmodels, lambda_bound,
+            return self.cache_mat(self.cache_dir, nmodels, lambda_operator, lambda_bound,
                                   cache_verbose, model_randomize_parameter,
-                                  cache_model, weak_form)
+                                  cache_model)
```

### Comparing `tedeous-0.2.1/tedeous/config.py` & `tedeous-0.3.0/tedeous/config.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.2.1/tedeous/derivative.py` & `tedeous-0.3.0/tedeous/derivative.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,16 +150,16 @@
 
     @staticmethod
     def derivative(u_tensor: torch.Tensor, h_tensor: torch.Tensor, axis: int,
                    scheme_order: int = 1, boundary_order: int = 1) -> torch.Tensor:
         """
         Computing derivative for 'matrix' method.
         Args:
-            u_tensor: smth.
-            h_tensor: smth.
+            u_tensor: function computed on a grid (n \times m matrix or multi-dimensional tensor with dim=D)
+            h_tensor: computational grid with shape (u_tensor.shape, D) result of solver.grid_format_prepare(coord_list,mode='mat'), where coord list is a list in format [x,t] or [x1,x2,x3,...]
             axis: axis along which the derivative is calculated.
             scheme_order: accuracy inner order for finite difference. Default = 1
             boundary_order: accuracy boundary order for finite difference. Default = 2
         Returns:
             computed derivative.
         """
         if (u_tensor.shape[0]==1):
```

### Comparing `tedeous-0.2.1/tedeous/device.py` & `tedeous-0.3.0/tedeous/device.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.2.1/tedeous/finite_diffs.py` & `tedeous-0.3.0/tedeous/finite_diffs.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.2.1/tedeous/input_preprocessing.py` & `tedeous-0.3.0/tedeous/input_preprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,48 @@
 import torch
 import numpy as np
 from copy import deepcopy
-from typing import Union
+from typing import Union, Tuple
 
 from tedeous.points_type import Points_type
 from tedeous.finite_diffs import Finite_diffs
 from tedeous.device import check_device
 
+def lambda_prepare(val: dict, lambda_: Union[int, list, dict]) -> dict :
+    """
+    Prepares lambdas for corresponding equation or bcond type.
+
+    Args:
+        val:
+        lambda_bound:
+
+    Returns:
+        dict with lambdas.
 
+    """
+    lambdas = {}
+    for i, key_name in enumerate(val):
+        if type(lambda_) is int:
+            lambdas[key_name] = lambda_
+        elif type(lambda_) is list:
+            lambdas[key_name] = lambda_[i]
+        else:
+            return lambda_
+    return lambdas
+
+def op_lambda_prepare(op, lambda_op):
+    lambdas = {}
+    for i, bcs_type in enumerate(op):
+        if type(lambda_op) is int:
+            lambdas[f'eq_{i+1}'] = lambda_op
+        elif type(lambda_op) is list:
+            lambdas[f'eq_{i+1}'] = lambda_op[i]
+        else:
+            return lambda_op
+    return lambdas
 class Boundary():
     """
     Сlass for bringing all boundary conditions to a similar form.
     """
     def __init__(self, bconds: list):
         """
         Args:
@@ -137,15 +168,15 @@
             bnd = {}
             bnd['bnd'], bnd['bop'], bnd['bval'], bnd['var'], \
             bnd['type'] = self.bnd_choose(bcond)
             unified_bnd.append(bnd)
         return unified_bnd
 
 
-class EquationMixin():
+class EquationMixin:
     """
     Auxiliary class. This one contains some methods that uses in other classes.
     """
 
     @staticmethod
     def equation_unify(equation: dict) -> dict:
         """
@@ -199,15 +230,15 @@
                 min_pos = pos
             pos += 1
         return min_pos
 
     @staticmethod
     def convert_to_double(bnd: Union[list, np.array]) -> float:
         """
-        Coverts points to double type.
+        Converts points to double type.
 
         Args:
             bnd: array or list of arrays
                 points that should be converted
         Returns:
             bnd with double type.
         """
@@ -246,14 +277,15 @@
             pos_list.append(pos)
         return pos_list
 
     @staticmethod
     def bndpos(grid: torch.Tensor, bnd: torch.Tensor) -> Union[list, int]:
         """
         Returns the position of the boundary points on the grid.
+
         Args:
             grid:  grid for coefficient in form of torch.Tensor mapping.
             bnd: boundary conditions.
         Returns:
             list of positions of the boundary points on the grid.
         """
 
@@ -271,14 +303,15 @@
     form. Then it will be used for determine solution by 'NN' method.
     """
 
     def __init__(self, grid: torch.Tensor, operator:  Union[dict, list], bconds, h: float = 0.001,
                  inner_order: str = '1', boundary_order: str = '2'):
         """
         Prepares equation, boundary conditions for NN method.
+
         Args:
             grid:  array of a n-D points.
             operator:  equation.
             bconds: boundary conditions.
             h: discretizing parameter in finite difference method (i.e., grid resolution for scheme).
             inner_order: accuracy inner order for finite difference. Default = 1
             boundary_order: accuracy boundary order for finite difference. Default = 2
```

### Comparing `tedeous-0.2.1/tedeous/models.py` & `tedeous-0.3.0/tedeous/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,101 +3,125 @@
 import torch.nn.functional as F
 import numpy as np
 
 
 class Fourier_embedding(nn.Module):
     """
     Class for Fourier features generation.
+
     Args:
         L: list[float or None], sin(w*x)/cos(w*X) frequencie parameter, w = 2*pi/L
         M: list[float or None], number of (sin, cos) pairs in result embedding
         ones: bool, enter or not ones vector in result embedding.
-    Example:
+
+    Examples:
         u(t,x) if user wants to create 5 Fourier features in 'x' direction with L=5:
-        L=[None, 5], M=[None, 5].
+            L=[None, 5], M=[None, 5].
     """
+
     def __init__(self, L=[1], M=[1], ones=False):
         super().__init__()
         self.M = M
         self.L = L
         self.idx = [i for i in range(len(self.M)) if self.M[i] is None]
         self.ones = ones
         self.in_features = len(M)
-        not_none = sum([i for i in M if i is not None]) 
+        not_none = sum([i for i in M if i is not None])
         is_none = self.M.count(None)
         if is_none == 0:
-            self.out_features = not_none*2 + 1
+            self.out_features = not_none * 2 + self.in_features
         else:
-            self.out_features = not_none*2 + is_none
+            self.out_features = not_none * 2 + is_none
         if ones is not False:
             self.out_features += 1
 
-    def forward(self, grid):
+    def forward(self, grid: torch.Tensor) -> torch.Tensor:
         """
         Forward method for Fourier features generation.
+
         Args:
-            grid: torch.Tensor, calculation domain.
+            grid: calculation domain.
         Returns:
-            out: torch.Tensor, embedding with Fourier features.
+            out: embedding with Fourier features.
         """
         if self.idx == []:
             out = grid
         else:
-            out = grid[:,self.idx]
-        
+            out = grid[:, self.idx]
+
         for i in range(len(self.M)):
             if self.M[i] is not None:
                 Mi = self.M[i]
                 Li = self.L[i]
                 w = 2.0 * np.pi / Li
-                k = torch.arange(1, Mi+1).reshape(-1,1).float()
-                x = grid[:,i].reshape(1,-1)
-                x = (k@x).T
-                embed_cos = torch.cos(w*x)
-                embed_sin = torch.sin(w*x)
+                k = torch.arange(1, Mi + 1).reshape(-1, 1).float()
+                x = grid[:, i].reshape(1, -1)
+                x = (k @ x).T
+                embed_cos = torch.cos(w * x)
+                embed_sin = torch.sin(w * x)
                 out = torch.hstack((out, embed_cos, embed_sin))
-        
+
         if self.ones is not False:
-            out = torch.hstack((out, torch.ones_like(out[:,0:1])))
+            out = torch.hstack((out, torch.ones_like(out[:, 0:1])))
 
         return out
 
 
-class Modified_MLP(nn.Module):
+class FourierNN(nn.Module):
     """
-    class for realizing neural network with Fourier features
+    Class for realizing neural network with Fourier features
     and skip connection.
+
     Args:
-        L: list[float or None], sin(w*x)/cos(w*X) frequencie parameter, w = 2*pi/L.
+        L: list[float or None], sin(w*x)/cos(w*X) frequency parameter, w = 2*pi/L.
         M: list[float or None], number of (sin, cos) pairs in result embedding.
         activation: nn.Module object, activation function.
         ones: bool, enter or not ones vector in result embedding.
     """
-    def __init__(self, layers=[100,100,100,1], L=[1], M=[1],
+
+    def __init__(self, layers=[100, 100, 100, 1], L=[1], M=[1],
                  activation=nn.Tanh(), ones=False):
-        super(Modified_MLP, self).__init__()
+        """
+            Class for realizing neural network with Fourier features
+            and skip connection.
+
+            Args:
+                L: list[float or None], sin(w*x)/cos(w*X) frequency parameter, w = 2*pi/L.
+                M: list[float or None], number of (sin, cos) pairs in result embedding.
+                activation: nn.Module object, activation function.
+                ones: bool, enter or not ones vector in result embedding.
+            """
+        super(FourierNN, self).__init__()
         self.L = L
         self.M = M
         FFL = Fourier_embedding(L=L, M=M, ones=ones)
 
         layers = [FFL.out_features] + layers
 
         self.linear_u = nn.Linear(layers[0], layers[1])
         self.linear_v = nn.Linear(layers[0], layers[1])
 
         self.activation = activation
         self.model = nn.ModuleList([FFL])
-        for i in range(len(layers)-1):
-            self.model.append(nn.Linear(layers[i], layers[i+1]))
+        for i in range(len(layers) - 1):
+            self.model.append(nn.Linear(layers[i], layers[i + 1]))
 
+    def forward(self, grid: torch.Tensor) -> torch.Tensor:
+        """
+        Forward pass for neural network.
 
-    def forward(self, grid):
+        Args:
+            grid: calculation domain.
+        Returns:
+            predicted values.
+
+        """
         input = self.model[0](grid)
         V = self.activation(self.linear_v(input))
         U = self.activation(self.linear_u(input))
         for layer in self.model[1:-1]:
             output = self.activation(layer(input))
             input = output * U + (1 - output) * V
 
         output = self.model[-1](input)
 
-        return output
+        return output
```

### Comparing `tedeous-0.2.1/tedeous/points_type.py` & `tedeous-0.3.0/tedeous/points_type.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.2.1/tedeous/solver.py` & `tedeous-0.3.0/tedeous/solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+from filecmp import clear_cache
 import torch
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib import cm
 import os
 import datetime
 from typing import Union
 from torch.optim.lr_scheduler import ExponentialLR
 
 from tedeous.cache import *
 from tedeous.device import check_device, device_type
-from tedeous.metrics import Solution
+from tedeous.solution import Solution
 import tedeous.input_preprocessing
 
 
 def grid_format_prepare(coord_list, mode='NN') -> torch.Tensor:
     """
     Prepares grid to a general form. Further, formatted grid can be processed
     by Points_type.point_typization for 'NN' and 'autograd' methods.
@@ -35,57 +36,65 @@
         else:
             coord_list_tensor = []
             for item in coord_list:
                 if isinstance(item, (np.ndarray)):
                     coord_list_tensor.append(torch.from_numpy(item).to(device))
                 else:
                     coord_list_tensor.append(item.to(device))
-            grid=torch.cartesian_prod(*coord_list_tensor)
-    elif mode=='mat':
+            grid = torch.cartesian_prod(*coord_list_tensor)
+    elif mode == 'mat':
         grid = np.meshgrid(*coord_list)
         grid = torch.tensor(np.array(grid)).to(device)
     return grid
 
 
 class Plots():
-    def __init__(self, model, grid, mode):
+    def __init__(self, model, grid, mode, tol = 0):
         self.model = model
         self.grid = grid
         self.mode = mode
+        self.tol = tol
 
     def print_nn(self, title: str):
         """
         Solution plot for NN method.
 
         Args:
             title: title
         """
         try:
             nvars_model = self.model[-1].out_features
         except:
             nvars_model = self.model.model[-1].out_features
 
         nparams = self.grid.shape[1]
-        fig = plt.figure(figsize=(15,8))
+        fig = plt.figure(figsize=(15, 8))
         for i in range(nvars_model):
             if nparams == 1:
-                ax1 = fig.add_subplot(1,nvars_model,i+1)
+                ax1 = fig.add_subplot(1, nvars_model, i + 1)
                 if title != None:
-                    ax1.set_title(title+' variable {}'.format(i))
+                    ax1.set_title(title + ' variable {}'.format(i))
                 ax1.scatter(self.grid.detach().cpu().numpy().reshape(-1),
-                            self.model(self.grid)[:,i].detach().cpu().numpy())
-                
+                            self.model(self.grid)[:, i].detach().cpu().numpy())
+
             else:
-                ax1 = fig.add_subplot(1, nvars_model, i+1, projection='3d')
+                ax1 = fig.add_subplot(1, nvars_model, i + 1, projection='3d')
                 if title != None:
-                    ax1.set_title(title+' variable {}'.format(i))
-                ax1.plot_trisurf(self.grid[:, 0].detach().cpu().numpy(), 
-                            self.grid[:, 1].detach().cpu().numpy(),
-                            self.model(self.grid)[:,i].detach().cpu().numpy(),
-                            cmap=cm.jet, linewidth=0.2, alpha=1)
+                    ax1.set_title(title + ' variable {}'.format(i))
+
+                if self.tol != 0:
+                    ax1.plot_trisurf(self.grid[:, 1].detach().cpu().numpy(),
+                                     self.grid[:, 0].detach().cpu().numpy(),
+                                     self.model(self.grid)[:, i].detach().cpu().numpy(),
+                                     cmap=cm.jet, linewidth=0.2, alpha=1)
+                else:
+                    ax1.plot_trisurf(self.grid[:, 0].detach().cpu().numpy(),
+                                     self.grid[:, 1].detach().cpu().numpy(),
+                                     self.model(self.grid)[:, i].detach().cpu().numpy(),
+                                     cmap=cm.jet, linewidth=0.2, alpha=1)
                 ax1.set_xlabel("x1")
                 ax1.set_ylabel("x2")
 
     def print_mat(self, title):
         """
         Solution plot for mat method.
 
@@ -96,15 +105,15 @@
         if nparams == 1:
             fig = plt.figure()
             plt.scatter(self.grid.cpu().reshape(-1),
                         self.model.detach().cpu().numpy().reshape(-1))
         elif nparams == 2:
             fig = plt.figure()
             ax = fig.add_subplot(111, projection='3d')
-            if title!=None:
+            if title != None:
                 ax.set_title(title)
             ax.plot_trisurf(self.grid[0].cpu().reshape(-1),
                             self.grid[1].cpu().reshape(-1),
                             self.model.reshape(-1).detach().cpu().numpy(),
                             cmap=cm.jet, linewidth=0.2, alpha=1)
             ax.set_xlabel("x1")
             ax.set_ylabel("x2")
@@ -114,28 +123,28 @@
         Path for save figures.
 
         Args:
             save_dir: directory where saves in
         """
         if save_dir == None:
             try:
-                img_dir = os.path.join(os.path.dirname( __file__ ), 'img')
+                img_dir = os.path.join(os.path.dirname(__file__), 'img')
             except:
                 current_dir = globals()['_dh'][0]
                 img_dir = os.path.join(os.path.dirname(current_dir), 'img')
-            
+
             if not (os.path.isdir(img_dir)):
                 os.mkdir(img_dir)
-            directory = os.path.abspath(os.path.join(img_dir, 
-                            str(datetime.datetime.now().timestamp())+'.png'))
+            directory = os.path.abspath(os.path.join(img_dir,
+                                                     str(datetime.datetime.now().timestamp()) + '.png'))
         else:
             if not (os.path.isdir(save_dir)):
                 os.mkdir(save_dir)
             directory = os.path.join(save_dir,
-                            str(datetime.datetime.now().timestamp())+'.png')
+                                     str(datetime.datetime.now().timestamp()) + '.png')
         return directory
 
     def solution_print(self, title=None, solution_print=False,
                        solution_save=False, save_dir=None):
 
         directory = self.dir_path(save_dir)
 
@@ -150,249 +159,258 @@
         plt.close()
 
 
 class Solver():
     """
     High-level interface for solving equations.
     """
+
     def __init__(self, grid: torch.Tensor, equal_cls,
                  model: Any, mode: str, weak_form: Union[None, list] = None):
         """
         High-level interface for solving equations.
+
         Args:
             grid: array of a n-D points.
             equal_cls: object from input_preprocessing (see input_preprocessing.Equation).
             model: neural network.
             mode: calculation method. (i.e., "NN", "autograd", "mat").
             weak_form: list of basis functions.
         """
         self.grid = check_device(grid)
         self.equal_cls = equal_cls
         self.model = model
         self.mode = mode
         self.weak_form = weak_form
 
-    def optimizer_choice(self, optimizer: str, learning_rate: float)-> \
+    def optimizer_choice(self, optimizer: str, learning_rate: float) -> \
             Union[torch.optim.Adam, torch.optim.SGD, torch.optim.LBFGS]:
         """
         Setting optimizer.
 
         Args:
            optimizer: optimizer choice (Adam, SGD, LBFGS).
            learning_rate: determines the step size at each iteration while moving toward a minimum of a loss function.
         Returns:
            torch.optimizer object as is.
         """
-        if optimizer=='Adam':
+        if optimizer == 'Adam':
             torch_optim = torch.optim.Adam
-        elif optimizer=='SGD':
+        elif optimizer == 'SGD':
             torch_optim = torch.optim.SGD
-        elif optimizer=='LBFGS':
+        elif optimizer == 'LBFGS':
             torch_optim = torch.optim.LBFGS
         else:
             print('Wrong optimizer chosen, optimization was not performed')
             return self.model
 
-        if self.mode =='NN' or self.mode == 'autograd':
+        if self.mode == 'NN' or self.mode == 'autograd':
             optimizer = torch_optim(self.model.parameters(), lr=learning_rate)
-        elif self.mode =='mat':
+        elif self.mode == 'mat':
             optimizer = torch_optim([self.model.requires_grad_()], lr=learning_rate)
-       
-        return optimizer
 
+        return optimizer
 
-    def solve(self, lambda_bound: Union[int, float] = 10,
-              verbose: bool = False, learning_rate: float = 1e-4, gamma=None, lr_change=1000,
+    def solve(self,lambda_operator: Union[float, list] = 1,lambda_bound: Union[float, list] = 10,
+              lambda_update: bool = False, second_order_interactions: bool = True, sampling_N: int = 1, verbose: int = 0,
+              learning_rate: float = 1e-4, gamma=None, lr_decay=1000,
               eps: float = 1e-5, tmin: int = 1000, tmax: float = 1e5,
               nmodels: Union[int, None] = None, name: Union[str, None] = None,
               abs_loss: Union[None, float] = None, use_cache: bool = True,
               cache_dir: str = '../cache/', cache_verbose: bool = False,
               save_always: bool = False, print_every: Union[int, None] = 100,
               cache_model: Union[torch.nn.Sequential, None] = None,
               patience: int = 5, loss_oscillation_window: int = 100,
-              no_improvement_patience: int = 1000,  model_randomize_parameter: Union[int, float] = 0,
+              no_improvement_patience: int = 1000, model_randomize_parameter: Union[int, float] = 0,
               optimizer_mode: str = 'Adam', step_plot_print: Union[bool, int] = False,
-              step_plot_save: Union[bool, int] = False, image_save_dir: Union[str, None] = None, tol:float=0) -> Any:
+              step_plot_save: Union[bool, int] = False, image_save_dir: Union[str, None] = None, tol: float = 0,clear_cache: bool =False) -> Any:
         """
         High-level interface for solving equations.
 
         Args:
-            lambda_bound: an arbitrary chosen constant, influence only convergence speed.
+            lambda_operator: coeff for operator part in loss.
+            lambda_bound: coeff for boundary part in loss.
+            lambda_update: enable lambda update.
             verbose: detailed info about training process.
             learning_rate: determines the step size at each iteration while moving toward a minimum of a loss function.
             gamma: multiplicative factor of learning rate decay.
-            lr_change: the number of epochs after which the learning_rate change occurs
+            lr_decay: decays the learning rate of each parameter group by gamma every epoch.
             eps: arbitrarily small number that uses for loss comparison criterion.
             tmax: maximum execution time.
-            nmodels: smth
+            nmodels: number cached models
             name: model name if saved.
             abs_loss: absolute loss.
             use_cache: as is.
             cache_dir: directory where saved cache in.
             cache_verbose: detailed info about models in cache.
-            save_always: smth
+            save_always: saves trained model even if the cache is False.
             print_every: prints the state of each given iteration to the command line.
             cache_model: model that uses in cache
             patience:if the loss is less than a certain value, then the counter increases when it reaches the given patience, the calculation stops.
             loss_oscillation_window: smth
             no_improvement_patience: smth
             model_randomize_parameter: creates a random model parameters (weights, biases) multiplied with a given randomize parameter.
             optimizer_mode: optimizer choice (Adam, SGD, LBFGS).
             step_plot_print: draws a figure through each given step.
             step_plot_save: saves a figure through each given step.
             image_save_dir: a directory where saved figure in.
-            tol: float constant, influences on error penalty in casual_loss algorithm. 
+            tol: float constant, influences on error penalty in casual_loss algorithm.
 
         Returns:
             model.
         """
-        
-
         Cache_class = Model_prepare(self.grid, self.equal_cls,
-                                                        self.model, self.mode)
+                                    self.model, self.mode, self.weak_form)
 
-        # prepare input data to uniform format 
+        #Cache_class.change_cache_dir(cache_dir)
+
+        # prepare input data to uniform format
         r = create_random_fn(model_randomize_parameter)
 
+        if clear_cache:
+            Cache_class.clear_cache_dir()
 
         #  use cache if needed
         if use_cache:
-            self.model, min_loss = Cache_class.cache(cache_dir, nmodels,
+            self.model, min_loss = Cache_class.cache(nmodels,
+                                                     lambda_operator,
                                                      lambda_bound,
                                                      cache_verbose,
                                                      model_randomize_parameter,
                                                      cache_model,
-                                                     weak_form=self.weak_form)
-            
+                                                    )
+
             Solution_class = Solution(self.grid, self.equal_cls,
-                                      self.model, self.mode)
+                                      self.model, self.mode, self.weak_form,
+                                      lambda_operator, lambda_bound)
         else:
             Solution_class = Solution(self.grid, self.equal_cls,
-                                      self.model, self.mode)
-            min_loss = Solution_class.loss_evaluation(lambda_bound=lambda_bound,
-                                                      weak_form=self.weak_form,
-                                                      tol=tol)
-        
-        self.plot = Plots(self.model, self.grid, self.mode)
+                                      self.model, self.mode, self.weak_form,
+                                      lambda_operator, lambda_bound)
+
+            _ , min_loss = Solution_class.evaluate()
+
+        self.plot = Plots(self.model, self.grid, self.mode, tol)
 
         optimizer = self.optimizer_choice(optimizer_mode, learning_rate)
+
         if gamma != None:
             scheduler = ExponentialLR(optimizer, gamma=gamma)
 
         # standard NN stuff
         if verbose:
             print('[{}] initial (min) loss is {}'.format(
                 datetime.datetime.now(), min_loss))
-    
+
         t = 0
-    
+
         last_loss = np.zeros(loss_oscillation_window) + float(min_loss)
         line = np.polyfit(range(loss_oscillation_window), last_loss, 1)
 
         def closure():
             nonlocal cur_loss
             optimizer.zero_grad()
-            loss = Solution_class.loss_evaluation(
-                lambda_bound = lambda_bound, weak_form=self.weak_form,
-                                                            tol=tol)
+            loss, loss_normalized = Solution_class.evaluate(second_order_interactions=second_order_interactions,
+                                           sampling_N=sampling_N,
+                                           lambda_update=lambda_update,
+                                           tol=tol)
+
             loss.backward()
-            cur_loss = loss.item()
+            cur_loss = loss_normalized.item()
             return loss
 
         stop_dings = 0
         t_imp_start = 0
         # to stop train proceduce we fit the line in the loss data
         # if line is flat enough "patience" times, we stop the procedure
         cur_loss = min_loss
         while stop_dings <= patience:
             optimizer.step(closure)
-
             if cur_loss != cur_loss:
                 print(f'Loss is equal to NaN, something went wrong (LBFGS+high'
-                 f'leraning rate and pytorch<1.12 could be the problem)')
+                      f'learning rate and pytorch<1.12 could be the problem)')
                 break
 
-            last_loss[(t-1)%loss_oscillation_window] = cur_loss
+            last_loss[(t - 1) % loss_oscillation_window] = cur_loss
 
-        
             if cur_loss < min_loss:
                 min_loss = cur_loss
                 t_imp_start = t
 
             if verbose:
-                info_string='Step = {} loss = {:.6f} normalized loss line= {:.6f}x+{:.6f}. There was {} stop dings already.'.format(
-                                                                        t, cur_loss, line[0]/cur_loss, line[1]/cur_loss, stop_dings+1)
-
-            if gamma != None and t % lr_change == 0:
-                 scheduler.step()
+                info_string = 'Step = {} loss = {:.6f} normalized loss line= {:.6f}x+{:.6f}. There was {} stop dings already.'.format(
+                    t, cur_loss, line[0] / cur_loss, line[1] / cur_loss, stop_dings + 1)
 
+            if gamma != None and t % lr_decay == 0:
+                scheduler.step()
 
-            if t%loss_oscillation_window == 0:
+            if t % loss_oscillation_window == 0:
                 line = np.polyfit(range(loss_oscillation_window), last_loss, 1)
-                if abs(line[0]/cur_loss) < eps and t > 0:
+                if abs(line[0] / cur_loss) < eps and t > 0:
                     stop_dings += 1
-                    if self.mode =='NN' or self.mode =='autograd':
+                    if self.mode == 'NN' or self.mode == 'autograd':
                         self.model.apply(r)
                     if verbose:
                         print('[{}] Oscillation near the same loss'.format(
                             datetime.datetime.now()))
                         print(info_string)
                         if step_plot_print or step_plot_save:
                             self.plot.solution_print(title='Iteration = ' + str(t),
-                                                solution_print=step_plot_print,
-                                                solution_save=step_plot_save,
-                                                save_dir=image_save_dir)
+                                                     solution_print=step_plot_print,
+                                                     solution_save=step_plot_save,
+                                                     save_dir=image_save_dir)
 
-            if (t-t_imp_start) == no_improvement_patience:
+            if (t - t_imp_start) == no_improvement_patience:
                 if verbose:
                     print('[{}] No improvement in {} steps'.format(
-                        datetime.datetime.now(),no_improvement_patience))
+                        datetime.datetime.now(), no_improvement_patience))
                     print(info_string)
                     if step_plot_print or step_plot_save:
                         self.plot.solution_print(title='Iteration = ' + str(t),
-                                                solution_print=step_plot_print,
-                                                solution_save=step_plot_save,
-                                                save_dir=image_save_dir)
+                                                 solution_print=step_plot_print,
+                                                 solution_save=step_plot_save,
+                                                 save_dir=image_save_dir)
                 t_imp_start = t
                 stop_dings += 1
                 if self.mode == 'NN' or self.mode == 'autograd':
-                        self.model.apply(r)
-
+                    self.model.apply(r)
 
             if abs_loss != None and cur_loss < abs_loss:
                 if verbose:
                     print('[{}] Absolute value of loss is lower than threshold'.format(datetime.datetime.now()))
                     print(info_string)
                     if step_plot_print or step_plot_save:
                         self.plot.solution_print(title='Iteration = ' + str(t),
-                                                solution_print=step_plot_print,
-                                                solution_save=step_plot_save,
-                                                save_dir=image_save_dir)
+                                                 solution_print=step_plot_print,
+                                                 solution_save=step_plot_save,
+                                                 save_dir=image_save_dir)
                 stop_dings += 1
-
-
+            # print('t',t)
             if print_every != None and (t % print_every == 0) and verbose:
                 print('[{}] Print every {} step'.format(
-                    datetime.datetime.now(),print_every))
+                    datetime.datetime.now(), print_every))
                 print(info_string)
+
+                # print('loss', closure().item(), 'loss_norm', cur_loss)
                 if step_plot_print or step_plot_save:
                     self.plot.solution_print(title='Iteration = ' + str(t),
-                                                solution_print=step_plot_print,
-                                                solution_save=step_plot_save,
-                                                save_dir=image_save_dir)
+                                             solution_print=step_plot_print,
+                                             solution_save=step_plot_save,
+                                             save_dir=image_save_dir)
+
             t += 1
             if t > tmax:
                 break
         if save_always:
             if self.mode == 'mat':
-                Cache_class.save_model_mat(cache_dir=cache_dir, name=name)
+                Cache_class.save_model_mat(name=name)
             else:
                 Cache_class.save_model(self.model, self.model.state_dict(),
-                                optimizer.state_dict(), cache_dir=cache_dir,
-                                name=name)
+                                       optimizer.state_dict(),
+                                       name=name)
         return self.model
```

### Comparing `tedeous-0.2.1/tedeous.egg-info/PKG-INFO` & `tedeous-0.3.0/tedeous.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tedeous
-Version: 0.2.1
+Version: 0.3.0
 Summary: TEDEouS - Torch Exhaustive Differential Equations Solver. Differential equation solver, based on pytorch library
 Author: Alexander Hvatov
 Author-email: itmo.nss.team@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


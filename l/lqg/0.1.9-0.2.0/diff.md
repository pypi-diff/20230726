# Comparing `tmp/lqg-0.1.9.tar.gz` & `tmp/lqg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lqg-0.1.9.tar", last modified: Mon Jun 19 15:09:48 2023, max compression
+gzip compressed data, was "lqg-0.2.0.tar", max compression
```

## Comparing `lqg-0.1.9.tar` & `lqg-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,28 @@
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-06-19 15:09:48.101289 lqg-0.1.9/
--rw-r--r--   0 dominik   (1000) dominik   (1000)    34523 2023-04-27 11:26:54.000000 lqg-0.1.9/LICENSE
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2876 2023-06-19 15:09:48.101289 lqg-0.1.9/PKG-INFO
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2384 2023-06-19 15:07:19.000000 lqg-0.1.9/README.md
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-06-19 15:09:48.097955 lqg-0.1.9/lqg/
--rw-r--r--   0 dominik   (1000) dominik   (1000)       49 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/__init__.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2028 2023-04-27 11:26:54.000000 lqg-0.1.9/lqg/ccg.py
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-06-19 15:09:48.101289 lqg-0.1.9/lqg/infer/
--rw-r--r--   0 dominik   (1000) dominik   (1000)      121 2023-04-27 11:26:54.000000 lqg-0.1.9/lqg/infer/__init__.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     1758 2023-04-27 11:26:54.000000 lqg-0.1.9/lqg/infer/map.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     1557 2023-04-27 11:26:54.000000 lqg-0.1.9/lqg/infer/mle.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     3721 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/infer/models.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2158 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/infer/prior.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     1542 2023-04-27 11:26:54.000000 lqg-0.1.9/lqg/infer/utils.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2968 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/io.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     4456 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/kalman.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     6971 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/model.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     7607 2023-04-27 11:26:54.000000 lqg-0.1.9/lqg/optim.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     1644 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/riccati.py
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-06-19 15:09:48.101289 lqg-0.1.9/lqg/tracking/
--rw-r--r--   0 dominik   (1000) dominik   (1000)      587 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/tracking/__init__.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     4955 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/tracking/basic.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)    11395 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/tracking/eye.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)      698 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/tracking/kf.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     5517 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/tracking/subjective.py
--rw-r--r--   0 dominik   (1000) dominik   (1000)     3096 2023-06-19 15:07:19.000000 lqg-0.1.9/lqg/tracking/three_dims.py
-drwxr-xr-x   0 dominik   (1000) dominik   (1000)        0 2023-06-19 15:09:48.101289 lqg-0.1.9/lqg.egg-info/
--rw-r--r--   0 dominik   (1000) dominik   (1000)     2876 2023-06-19 15:09:48.000000 lqg-0.1.9/lqg.egg-info/PKG-INFO
--rw-r--r--   0 dominik   (1000) dominik   (1000)      506 2023-06-19 15:09:48.000000 lqg-0.1.9/lqg.egg-info/SOURCES.txt
--rw-r--r--   0 dominik   (1000) dominik   (1000)        1 2023-06-19 15:09:48.000000 lqg-0.1.9/lqg.egg-info/dependency_links.txt
--rw-r--r--   0 dominik   (1000) dominik   (1000)      104 2023-06-19 15:09:48.000000 lqg-0.1.9/lqg.egg-info/requires.txt
--rw-r--r--   0 dominik   (1000) dominik   (1000)        4 2023-06-19 15:09:48.000000 lqg-0.1.9/lqg.egg-info/top_level.txt
--rw-r--r--   0 dominik   (1000) dominik   (1000)       38 2023-06-19 15:09:48.101289 lqg-0.1.9/setup.cfg
--rw-r--r--   0 dominik   (1000) dominik   (1000)      919 2023-06-19 15:09:42.000000 lqg-0.1.9/setup.py
+-rw-r--r--   0        0        0    34523 2023-04-27 11:26:54.134688 lqg-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2675 2023-07-26 10:09:43.575186 lqg-0.2.0/README.md
+-rw-r--r--   0        0        0      127 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/belief/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/belief/kf.py
+-rw-r--r--   0        0        0     2028 2023-04-27 11:26:54.148021 lqg-0.2.0/lqg/ccg.py
+-rw-r--r--   0        0        0        0 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/control/__init__.py
+-rw-r--r--   0        0        0     1243 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/control/glqr.py
+-rw-r--r--   0        0        0     1078 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/control/lqr.py
+-rw-r--r--   0        0        0     7298 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/glqg.py
+-rw-r--r--   0        0        0      121 2023-04-27 11:26:54.148021 lqg-0.2.0/lqg/infer/__init__.py
+-rw-r--r--   0        0        0     1758 2023-04-27 11:26:54.148021 lqg-0.2.0/lqg/infer/map.py
+-rw-r--r--   0        0        0     1732 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/infer/mle.py
+-rw-r--r--   0        0        0     2051 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/infer/models.py
+-rw-r--r--   0        0        0     1764 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/infer/prior.py
+-rw-r--r--   0        0        0     1908 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/infer/utils.py
+-rw-r--r--   0        0        0     3014 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/io.py
+-rw-r--r--   0        0        0     7846 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/lqg.py
+-rw-r--r--   0        0        0     7607 2023-04-27 11:26:54.148021 lqg-0.2.0/lqg/optim.py
+-rw-r--r--   0        0        0     1904 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/spec.py
+-rw-r--r--   0        0        0      178 2023-07-25 14:39:35.745375 lqg-0.2.0/lqg/tracking/__init__.py
+-rw-r--r--   0        0        0     1837 2023-07-25 14:39:35.748708 lqg-0.2.0/lqg/tracking/basic.py
+-rw-r--r--   0        0        0     2094 2023-07-25 14:39:35.748708 lqg-0.2.0/lqg/tracking/delay.py
+-rw-r--r--   0        0        0     2824 2023-07-25 14:39:35.748708 lqg-0.2.0/lqg/tracking/signal_dependent.py
+-rw-r--r--   0        0        0     1068 2023-07-25 14:39:35.748708 lqg-0.2.0/lqg/tracking/subjective.py
+-rw-r--r--   0        0        0     1724 2023-07-25 14:39:35.748708 lqg-0.2.0/lqg/utils.py
+-rw-r--r--   0        0        0      554 2023-07-25 14:39:35.755375 lqg-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 lqg-0.2.0/PKG-INFO
```

### Comparing `lqg-0.1.9/LICENSE` & `lqg-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lqg-0.1.9/PKG-INFO` & `lqg-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: lqg
-Version: 0.1.9
-Summary: (Inverse) optimal control for linear quadratic Gaussian systems
-Home-page: https://github.com/dominikstrb/lqg
-Author: Dominik Straub
-Author-email: dominik.straub@tu-darmstadt.de
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Inverse optimal control for continuous psychophysics
 
 ![Experimenter-actor-loop](https://raw.githubusercontent.com/RothkopfLab/lqg/main/docs/source/_static/experimenter-actor-loop.png)
 
 
 This repository contains the official [JAX](https://github.com/google/jax) implementation of the inverse optimal control method presented in the paper:
 
@@ -24,28 +10,33 @@
 ## Installation
 The package can be installed via `pip`
 
 ```bash
 python -m pip install lqg
 ```
 
-although I recommend cloning the repository to get the most recent version and installing locally with a virtual environment
+Since publication of our [eLife paper](https://elifesciences.org/articles/76635), I have substantially updated the package. If you want to use the package as described in the paper, please install an older version `<0.20`:
+
+```bash
+python -m pip install lqg==0.1.9
+```
+
+If you want the latest development version, I recommend cloning the repository and installing locally in a virtual environment: 
 
 ```bash
+git clone git@github.com:dominikstrb/lqg.git
+cd lqg
 python -m venv env
 source env/bin/activate
 python -m pip install -e .
 ```
 
 ## Usage examples
 - `main.py` shows how to simulate data and infer parameters using the LQG model of the tracking task.
-
-- [`notebooks/01-HowTo.ipynb`](https://github.com/RothkopfLab/lqg/blob/main/notebooks/01-HowTo.ipynb) explains the model and its parameters in more detail, including the extension to subjective internal models.
-
-- [`notebooks/02-Data.ipynb`](https://github.com/RothkopfLab/lqg/blob/main/notebooks/02-Data.ipynb) fits the ideal observer and bounded actor model to the [data](https://github.com/kbonnen/BonnenEtAl2015_KalmanFilterCode) from [Bonnen et al. (2015)](https://jov.arvojournals.org/article.aspx?articleid=2301260) to reproduce Fig. 4A from our paper.
+- [`notebooks/Tutorial.ipynb`](https://github.com/RothkopfLab/lqg/blob/main/notebooks/01-HowTo.ipynb) explains the model and its parameters in more detail, including the extension to subjective internal models (based on [my tutorial at CCN 2022](https://www.youtube.com/watch?v=3DbO9n6_mNE))
 
 ## Citation
 If you use our method or code in your research, please cite our paper:
 
 ```
 @article{straub2022putting,
   title={Putting perception into action with inverse optimal control for continuous psychophysics},
@@ -54,9 +45,13 @@
   volume={11},
   pages={e76635},
   year={2022},
   publisher={eLife Sciences Publications Limited}
 }
 ```
 
-## Signal-dependent noise
+## Extensions
+### Signal-dependent noise
 This implementation supports the basic LQG framework. For the extension to signal-dependent noise [(Todorov, 2005)](https://direct.mit.edu/neco/article-abstract/17/5/1084/6949/Stochastic-Optimal-Control-and-Estimation-Methods), please see [our NeurIPS 2021 paper](https://proceedings.neurips.cc/paper/2021/hash/4e55139e019a58e0084f194f758ffdea-Abstract.html) and [its implementation](https://github.com/RothkopfLab/inverse-optimal-control).
+
+### Non-linear dynamics
+We are currently working on extending this approach to non-linear dynamics and non-quadratic costs. Please check out our [preprint](https://arxiv.org/abs/2303.16698). Code will be released soon.
```

### Comparing `lqg-0.1.9/lqg/ccg.py` & `lqg-0.2.0/lqg/ccg.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.9/lqg/infer/map.py` & `lqg-0.2.0/lqg/infer/map.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.9/lqg/infer/mle.py` & `lqg-0.2.0/lqg/infer/mle.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import jax.numpy as jnp
 from jax import random, lax
 import numpyro
 from numpyro.infer import SVI, Trace_ELBO
 
 from lqg.tracking import BoundedActor
-from lqg.infer.models import lqg_model, common_lqg_model
+from lqg.infer.models import lqg_model
 
 
 def guide(x, model_type, process_noise=None, dt=None, **fixed_params):
     pass
 
 
 def max_likelihood(x, model=BoundedActor, numpyro_fn=lqg_model, process_noise=1., dt=1. / 60, steps=2_000,
                    step_size=0.01, **fixed):
     # optim = numpyro.optim.ClippedAdam(step_size=step_size)
     optim = numpyro.optim.Adam(step_size=step_size)
+    # optim = numpyro.optim.Minimize("BFGS")
 
     # optim = numpyro.optim.Minimize()
     svi = SVI(numpyro_fn, guide, optim, Trace_ELBO(), x=x, model_type=model, process_noise=process_noise, dt=dt,
               **fixed)
     params, state, losses = svi.run(random.PRNGKey(3), steps)
 
     return params, losses
@@ -29,23 +30,24 @@
     import arviz as az
 
     c_true = .5
     motor_noise_true = .25
     sigma_true = 8.
     prop_noise_true = 2.
     lqg = BoundedActor(process_noise=1.,
-                      sigma=sigma_true, motor_noise=motor_noise_true, c=c_true, prop_noise=prop_noise_true)
+                       sigma_target=sigma_true, action_variability=motor_noise_true, action_cost=c_true,
+                       sigma_cursor=prop_noise_true, T=500)
 
-    results = dict(c=[], sigma=[], motor_noise=[], prop_noise=[])
+    results = dict(action_cost=[], sigma_target=[], action_variability=[], sigma_cursor=[])
     for seed in range(1):
-        x = lqg.simulate(n=20, T=500, seed=seed)
+        x = lqg.simulate(rng_key=random.PRNGKey(seed), n=20)
 
-        params, losses = max_likelihood(x, steps=1)
+        params, losses = max_likelihood(x, steps=1_000, action_cost=.5, sigma_cursor=2.)
 
         for key, item in params.items():
             results[key].append(item)
 
-    for key in results.keys():
-        results[key] = jnp.stack(results[key])
+        for key in results.keys():
+            results[key] = jnp.stack(results[key])
 
-    az.plot_pair(results, figsize=(8, 8))
-    plt.show()
+        az.plot_pair(results, figsize=(8, 8))
+        plt.show()
```

### Comparing `lqg-0.1.9/lqg/infer/utils.py` & `lqg-0.2.0/lqg/infer/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import jax.numpy as jnp
 from jax import random, lax
+import numpyro
 from numpyro import optim
-from numpyro.infer import NUTS, MCMC, SVI, Trace_ELBO
+from numpyro.infer import NUTS, MCMC, SVI, Trace_ELBO, init_to_median
 from numpyro.infer.autoguide import AutoBNAFNormal
 from numpyro.infer.reparam import NeuTraReparam
 
-from lqg.infer.models import lifted_model as lqg_model
+from lqg.infer.models import lifted_model as lqg_model, get_model_params
+from lqg.infer import prior
 from lqg.tracking import BoundedActor
 
 
 def infer(x, num_samples, num_warmup, model=BoundedActor, numpyro_fn=lqg_model, process_noise=1., dt=1. / 60,
           method="nuts", progress_bar=True, num_chains=1, seed=0, **fixed):
     if method == "nuts":
         # setup kernel
-        nuts_kernel = NUTS(numpyro_fn)
+        nuts_kernel = NUTS(numpyro_fn, init_strategy=init_to_median)
 
     elif method == "neutra":
         # learn normalizing flow
         guide = AutoBNAFNormal(numpyro_fn)
         svi = SVI(numpyro_fn, guide, optim.Adam(0.003), Trace_ELBO())
         svi_state = svi.init(random.PRNGKey(seed), x, model, process_noise, dt, **fixed)
 
@@ -33,7 +35,12 @@
 
     # run NUTS
     mcmc = MCMC(nuts_kernel, num_samples=num_samples, num_warmup=num_warmup, progress_bar=progress_bar,
                 num_chains=num_chains)
     mcmc.run(random.PRNGKey(seed), x, model, process_noise, dt, **fixed)
 
     return mcmc
+
+
+def sample_from_prior(model_type, seed, prior_dict=prior.default_prior):
+    param_dict = {**numpyro.handlers.seed(prior.sample_params, rng_seed=seed)(prior_dict)}
+    return {k: v for k, v in param_dict.items() if k in get_model_params(model_type).keys()}
```

### Comparing `lqg-0.1.9/lqg/io.py` & `lqg-0.2.0/lqg/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import numpy as np
 import scipy.io as spio
 
 
 # methods for properly reading matlab structs
 # taken from https://stackoverflow.com/a/8832212
 
@@ -37,15 +38,15 @@
         if isinstance(elem, spio.matlab.mio5_params.mat_struct):
             dict[strg] = _todict(elem)
         else:
             dict[strg] = elem
     return dict
 
 
-def load_tracking_data(delay=12, clip=120, subtract_mean=True):
+def load_tracking_data(delay=12, clip=120, subtract_mean=True, data_path="data/"):
     """ Load tracking data from Bonnen et al. (2015)
 
     Args:
         delay: temporal delay between target and response
         clip: clip the first n time steps
         subtract_mean: subtract the mean of both trajectories?
 
@@ -53,15 +54,15 @@
         np.array: data from tracking task
     """
 
     # factor to convert between pixels and acrmin
     arcscale = 1.32
 
     # load matlab file
-    mat = loadmat("../data/data.mat")
+    mat = loadmat(os.path.join(data_path, "data.mat"))
 
     # get target blob widths
     sigma = (mat["sigma"] * arcscale).round()
     sigmas = np.unique(sigma)
 
     # convert to numpy.float32
     target = mat["target"].astype(np.float32)
```

### Comparing `lqg-0.1.9/lqg/model.py` & `lqg-0.2.0/lqg/glqg.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,101 +1,42 @@
-from dataclasses import dataclass
-import jax.numpy as jnp
-import numpyro.distributions as dist
-from jax import vmap, random
+from jax import random, vmap, numpy as jnp
 from jax.lax import scan
 
-from lqg.riccati import kalman_gain, control_law
+from lqg.control import glqr
+from lqg.belief import kf
+from lqg.lqg import System
+from lqg.spec import LQGSpec
+from lqg.utils import quadratic_form_t
 
 
-@dataclass
-class Dynamics:
-    A: jnp.array
-    B: jnp.array
-    C: jnp.array
-    V: jnp.array
-    W: jnp.array
-
-
-@dataclass
-class Actor:
-    A: jnp.array
-    B: jnp.array
-    C: jnp.array
-    V: jnp.array
-    W: jnp.array
-    Q: jnp.array
-    R: jnp.array
-
-    def L(self, T):
-        return control_law(self.A, self.B, self.Q, self.R, T=T)
-
-    def K(self, T):
-        return kalman_gain(self.A, self.C, self.V @ self.V.T, self.W @ self.W.T, T=T)
-
-
-class System:
-    def __init__(self, actor: Actor, dynamics: Dynamics):
-        self.actor = actor
-        self.dynamics = dynamics
-
-    @property
-    def xdim(self):
-        """ State dimensionality
+class SignalDependentNoiseSystem(System):
+    def __init__(self, actor: LQGSpec, dynamics: LQGSpec):
+        super().__init__(actor, dynamics)
 
-        Returns:
-            int: dimensionality of state
-        """
-        return self.dynamics.A.shape[0]
-
-    @property
-    def ydim(self):
-        """ Observation dimensionality
-
-        Returns:
-            int: dimensionality of observation
-        """
-        return self.dynamics.C.shape[0]
-
-    @property
-    def bdim(self):
-        """ Belief dimensionality
-
-        Returns:
-            int: dimensionality of belief
-        """
-        return self.actor.A.shape[0]
-
-    @property
-    def udim(self):
-        """ Action dimensionality
-
-        Returns:
-            int: dimensionality of action
-        """
-        return self.dynamics.B.shape[1]
-
-    def simulate(self, rng_key, n=1, T=100, x0=None, xhat0=None, return_all=False):
+    def simulate(self, rng_key, n=1, x0=None, xhat0=None, Sigma0=None, return_all=False):
         """ Simulate n trials
 
         Args:
             rng_key (jax.random.PRNGKey): random number generator key
             n (int): number of trials
             T (int): number of time steps
             x0 (jnp.array): initial state
             xhat0 (jnp.array): initial belief
             return_all (bool): return estimates, controls and observations as well
 
         Returns:
             jnp.array (T, n, d)
         """
-        L = self.actor.L(T=T)
-        K = self.actor.K(T=T)
 
-        def simulate_trial(rng_key, T=100, x0=None, xhat0=None):
+        Sigma0 = self.actor.V[0] @ self.actor.V[0].T if Sigma0 is None else Sigma0
+
+        gains = glqr.backward(self.actor)
+        K = kf.forward(self.actor, Sigma0=Sigma0)
+
+        def simulate_trial(rng_key, x0=None, xhat0=None):
             """ Simulate a single trial
 
             Args:
                 rng_key (jax.random.PRNGKey): random number generator key
                 T (int): number of time steps
                 x0 (jnp.array): initial state
                 xhat0 (jnp.array): initial belief
@@ -104,116 +45,129 @@
                 jnp.array, jnp.array, jnp.array, jnp.array: x (states), x_hat (estimates), y, u
             """
 
             x0 = jnp.zeros(self.xdim) if x0 is None else x0
             xhat0 = jnp.zeros(self.bdim) if xhat0 is None else xhat0
 
             # generate standard normal noise terms
-            rng_key, subkey = random.split(rng_key)
-            epsilon = random.normal(subkey, shape=(T, self.xdim))
-            rng_key, subkey = random.split(rng_key)
-            eta = random.normal(subkey, shape=(T, self.ydim))
+            key1, key2, key3, key4 = random.split(rng_key, 4)
+            noise_x = random.normal(key1, shape=(self.T, self.dynamics.V.shape[-1]))
+            noise_y = random.normal(key2, shape=(self.T, self.dynamics.W.shape[-1]))
+            noise_Cu = random.normal(key3, (self.T, self.dynamics.Cu.shape[-2],))
+            noise_Cx = random.normal(key4, (self.T, self.dynamics.Cx.shape[-2],))
 
             def loop(carry, t):
                 x, x_hat = carry
 
-                # compute control based on agent's current belief
-                u = - L @ x_hat
-
-                # apply dynamics
-                x = self.dynamics.A @ x + self.dynamics.B @ u + self.dynamics.V @ epsilon[t]
-
                 # generate observation
-                y = self.dynamics.C @ x + self.dynamics.W @ eta[t]
+                y = self.dynamics.F[t] @ x + self.dynamics.W[t] @ noise_y[t]
 
                 # update agent's belief
-                x_pred = self.actor.A @ x_hat + self.actor.B @ u
-                x_hat = x_pred + K @ (y - self.actor.C @ x_pred)
+                x_pred = self.actor.A[t] @ x_hat + self.actor.B[t] @ (gains.L[t] @ x_hat + gains.l[t])
+                x_hat = x_pred + K[t] @ (y - self.actor.F[t] @ x_hat)
+
+                # compute control based on agent's current belief
+                u = gains.L[t] @ x_hat + gains.l[t]
+
+                # apply dynamics
+                x = (self.dynamics.A[t] @ x + self.dynamics.B[t] @ u + self.dynamics.V[t] @ noise_x[t]
+                     + self.dynamics.Cx[t] @ x @ noise_Cx[t] + self.dynamics.Cu[t] @ u @ noise_Cu[t])
 
                 return (x, x_hat), (x, x_hat, y, u)
 
-            _, (x, x_hat, y, u) = scan(loop, (x0, xhat0), jnp.arange(1, T))
+            _, (x, x_hat, y, u) = scan(loop, (x0, xhat0), jnp.arange(self.T))
 
-            return jnp.vstack([x0, x]), jnp.vstack([xhat0, x_hat]), \
-                   jnp.vstack([self.dynamics.C @ x0 + self.dynamics.W @ eta[0], y]), u
+            return (jnp.vstack([x0, x]),
+                    jnp.vstack([xhat0, x_hat]),
+                    jnp.vstack([y, self.dynamics.F[-1] @ x[-1] + self.dynamics.W[-1] @ noise_y[-1]]),
+                    u)
 
         # simulate n trials
-        x, x_hat, y, u = vmap(lambda key: simulate_trial(key, T=T, x0=x0, xhat0=xhat0),
-                              out_axes=1)(random.split(rng_key, num=n))
+        x, x_hat, y, u = vmap(lambda key: simulate_trial(key, x0=x0, xhat0=xhat0))(random.split(rng_key, num=n))
 
         if return_all:
             return x, x_hat, y, u
         else:
             return x
 
-    def conditional_moments(self, x, mu0=None):
+    def conditional_moments(self, x):
         """ Conditional distribution p(x | theta)
 
-                Args:
-                    self: LQG
-                    x: time series of shape T (time steps), n (trials), d (dimensionality)
-
-                Returns:
-                    numpyro.distributions.MultivariateNormal
-                """
-        T, n, d = x.shape
-
-        # compute control and estimator gains
-        L = self.actor.L(T)
-        K = self.actor.K(T)
+        Args:
+            self: LQG
+            x: time series of shape T (time steps), n (trials), d (dimensionality)
 
-        # set up joint dynamical system for state and belief
-        # p(x_t, xhat_t | x_{t-1}, xhat_{t-1})
-        F = jnp.vstack(
-            [jnp.hstack([self.dynamics.A,
-                         -self.dynamics.B @ L]),
-             jnp.hstack([K @ self.dynamics.C @ self.dynamics.A,
-                         self.actor.A - self.actor.B @ L - K @ self.actor.C @ self.actor.A])])
+        Returns:
+            numpyro.distributions.MultivariateNormal
+        """
+        T, obs_dim = x.shape
+        xdim = self.dynamics.A.shape[1]
+        bdim = self.actor.A.shape[1]
 
-        G = jnp.vstack([jnp.hstack([self.dynamics.V, jnp.zeros_like(self.dynamics.C.T)]),
-                        jnp.hstack([K @ self.dynamics.C @ self.dynamics.V, K @ self.dynamics.W])])
+        # compute control and estimator gains
+        gains = glqr.backward(self.actor)
+        K = kf.forward(self.actor, Sigma0=self.actor.V[0] @ self.actor.V[0].T)
 
         # initialize p(x_t, xhat_t | x_{1:t-1})
-        mu = jnp.zeros((n, self.dynamics.A.shape[0] + self.actor.A.shape[0])) if mu0 is None else mu0
-        Sigma = G @ G.T
+        # TODO: initialization should not always be zero for the unobserved dims
+        mu = jnp.hstack([x[0], jnp.zeros(xdim - obs_dim + bdim)])
+        # TODO: is there a smarter way to initialize Sigma?
+        #  For example, with zeros in the covariances, we get problems
+        Sigma = jnp.eye(xdim * 2) * 1e-1
 
-        def f(carry, xt):
+        def scan_fn(carry, t):
             mu, Sigma = carry
 
-            # condition on observed state x_t
-            mu = mu @ F.T + (xt - mu[:, :d]) @ jnp.linalg.inv(Sigma[:d, :d]).T @ (F @ Sigma)[:, :d].T
+            # joint dynamics
+            F = jnp.concatenate([
+                jnp.concatenate([self.dynamics.A[t],
+                                 self.dynamics.B[t] @ gains.L[t]],
+                                axis=-1),
+                jnp.concatenate([K[t] @ self.dynamics.F[t],
+                                 self.actor.A[t] + self.actor.B[t] @ gains.L[t] - K[t] @ self.actor.F[t]],
+                                axis=-1)],
+                axis=-2)
+
+            # joint state-independent noise covariance Cholesky factor
+            G = jnp.concatenate([
+                jnp.concatenate([self.dynamics.V[t],
+                                 jnp.zeros_like(self.dynamics.F[t].T)],
+                                axis=-1),
+                jnp.concatenate([jnp.zeros_like(self.actor.V[t]),
+                                 K[t] @ self.dynamics.W[t]],
+                                axis=-1)],
+                axis=-2)
+
+            # signal-dependent noise matrix
+            M = jnp.concatenate([jnp.concatenate([self.dynamics.Cx[t],
+                                                  self.dynamics.Cu[t] @ gains.L[t]], axis=-1),
+                                 jnp.concatenate([jnp.zeros((self.dynamics.A[t].shape[0],
+                                                             self.dynamics.Cx[t].shape[1],
+                                                             self.dynamics.A[t].shape[0])),
+                                                  jnp.zeros((self.dynamics.A[t].shape[0],
+                                                             self.dynamics.Cu[t].shape[1],
+                                                             self.dynamics.A[t].shape[0]))], axis=-1)],
+                                axis=-3)
+
+            # conditioning: p(xhat_t | x_1:t)
+            Sxh = Sigma[:obs_dim, obs_dim:]
+            Shh = Sigma[obs_dim:, obs_dim:]
+            Sxx = Sigma[:obs_dim, :obs_dim]
+            Shx = Sigma[obs_dim:, :obs_dim]
+            mu_x = mu[:obs_dim]
+            mu_ba = mu[obs_dim:] + Shx @ jnp.linalg.solve(Sxx, x[t] - mu_x)
+            Sigma_ba = Shh - Shx @ jnp.linalg.solve(Sxx, Sxh)
+
+            # updating: p(x_t+1, xhat_t+1 | x_1:t)
+            mu = F[:, :obs_dim] @ x[t] + F[:, obs_dim:] @ mu_ba
+            rsm_xh = Sigma_ba + jnp.outer(mu_ba, mu_ba)
+            TM = quadratic_form_t(M[..., :obs_dim], jnp.outer(x[t], x[t])).sum(axis=0)
+            TMh = quadratic_form_t(M[..., obs_dim:], rsm_xh).sum(axis=0)
+            Sigma = TM + TMh + F[:, obs_dim:] @ Sigma_ba @ F[:, obs_dim:].T + G @ G.T
+
+            # for numerical stability, add small diagonal term
+            Sigma += jnp.eye(Sigma.shape[-1]) * 1e-7  # TODO: can we do this in a more principled way?
 
-            Sigma = F @ Sigma @ F.T + G @ G.T - (F @ Sigma)[:, :d] @ jnp.linalg.inv(Sigma[:d, :d]) @ (Sigma @ F.T)[:d,
-                                                                                                     :]
             return (mu, Sigma), (mu, Sigma)
 
-        _, (mu, Sigma) = scan(f, (mu, Sigma), x)
+        _, (mu, Sigma) = scan(scan_fn, (mu, Sigma), jnp.arange(T - 1))
         return mu, Sigma
-
-    def conditional_distribution(self, x):
-        T, n, d = x.shape
-
-        # compute p(x_{t+1}, xhat_{t+1} | x_{1:t})
-        mu, Sigma = self.conditional_moments(x)
-
-        # marginalize out xhat by using only those entries of mu and Sigma that correspond to x
-        return dist.MultivariateNormal(mu[:, :, :d], Sigma[:, jnp.newaxis, :d, :d])
-
-    def log_likelihood(self, x):
-        # log likelihood of the states at time t+1 given all previous states up to time t
-        return self.conditional_distribution(x[:-1]).log_prob(x[1:])
-
-    def belief_tracking_distribution(self, x):
-        d = self.xdim
-
-        # compute p(x_{t+1}, xhat_{t+1} | x_{1:t})
-        mu, Sigma = self.conditional_moments(x)
-
-        # return those elements of mu and Sigma that correspond to xhat
-        return dist.MultivariateNormal(mu[:, :, d:], Sigma[:, jnp.newaxis, d:, d:])
-
-
-class LQG(System):
-    def __init__(self, A, B, C, V, W, Q, R):
-        dynamics = Dynamics(A, B, C, V, W)
-        actor = Actor(A, B, C, V, W, Q, R)
-        super().__init__(actor=actor, dynamics=dynamics)
```

### Comparing `lqg-0.1.9/lqg/optim.py` & `lqg-0.2.0/lqg/optim.py`

 * *Files identical despite different names*

### Comparing `lqg-0.1.9/lqg.egg-info/PKG-INFO` & `lqg-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: lqg
-Version: 0.1.9
-Summary: (Inverse) optimal control for linear quadratic Gaussian systems
-Home-page: https://github.com/dominikstrb/lqg
+Version: 0.2.0
+Summary: (Inverse) optimal control for linear-quadratic Gaussian systems
+License: AGPL-3.0-only
 Author: Dominik Straub
-Author-email: dominik.straub@tu-darmstadt.de
+Author-email: dominikstrb@mailbox.org
+Requires-Python: >=3.10
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: arviz (>=0.16.1)
+Requires-Dist: jax (>=0.4.13)
+Requires-Dist: matplotlib (>=3.2.2)
+Requires-Dist: numpyro (>=0.12.1)
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Inverse optimal control for continuous psychophysics
 
 ![Experimenter-actor-loop](https://raw.githubusercontent.com/RothkopfLab/lqg/main/docs/source/_static/experimenter-actor-loop.png)
 
 
 This repository contains the official [JAX](https://github.com/google/jax) implementation of the inverse optimal control method presented in the paper:
@@ -24,28 +28,33 @@
 ## Installation
 The package can be installed via `pip`
 
 ```bash
 python -m pip install lqg
 ```
 
-although I recommend cloning the repository to get the most recent version and installing locally with a virtual environment
+Since publication of our [eLife paper](https://elifesciences.org/articles/76635), I have substantially updated the package. If you want to use the package as described in the paper, please install an older version `<0.20`:
 
 ```bash
+python -m pip install lqg==0.1.9
+```
+
+If you want the latest development version, I recommend cloning the repository and installing locally in a virtual environment: 
+
+```bash
+git clone git@github.com:dominikstrb/lqg.git
+cd lqg
 python -m venv env
 source env/bin/activate
 python -m pip install -e .
 ```
 
 ## Usage examples
 - `main.py` shows how to simulate data and infer parameters using the LQG model of the tracking task.
-
-- [`notebooks/01-HowTo.ipynb`](https://github.com/RothkopfLab/lqg/blob/main/notebooks/01-HowTo.ipynb) explains the model and its parameters in more detail, including the extension to subjective internal models.
-
-- [`notebooks/02-Data.ipynb`](https://github.com/RothkopfLab/lqg/blob/main/notebooks/02-Data.ipynb) fits the ideal observer and bounded actor model to the [data](https://github.com/kbonnen/BonnenEtAl2015_KalmanFilterCode) from [Bonnen et al. (2015)](https://jov.arvojournals.org/article.aspx?articleid=2301260) to reproduce Fig. 4A from our paper.
+- [`notebooks/Tutorial.ipynb`](https://github.com/RothkopfLab/lqg/blob/main/notebooks/01-HowTo.ipynb) explains the model and its parameters in more detail, including the extension to subjective internal models (based on [my tutorial at CCN 2022](https://www.youtube.com/watch?v=3DbO9n6_mNE))
 
 ## Citation
 If you use our method or code in your research, please cite our paper:
 
 ```
 @article{straub2022putting,
   title={Putting perception into action with inverse optimal control for continuous psychophysics},
@@ -54,9 +63,13 @@
   volume={11},
   pages={e76635},
   year={2022},
   publisher={eLife Sciences Publications Limited}
 }
 ```
 
-## Signal-dependent noise
+## Extensions
+### Signal-dependent noise
 This implementation supports the basic LQG framework. For the extension to signal-dependent noise [(Todorov, 2005)](https://direct.mit.edu/neco/article-abstract/17/5/1084/6949/Stochastic-Optimal-Control-and-Estimation-Methods), please see [our NeurIPS 2021 paper](https://proceedings.neurips.cc/paper/2021/hash/4e55139e019a58e0084f194f758ffdea-Abstract.html) and [its implementation](https://github.com/RothkopfLab/inverse-optimal-control).
+
+### Non-linear dynamics
+We are currently working on extending this approach to non-linear dynamics and non-quadratic costs. Please check out our [preprint](https://arxiv.org/abs/2303.16698). Code will be released soon.
```


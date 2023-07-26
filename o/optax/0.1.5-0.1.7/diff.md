# Comparing `tmp/optax-0.1.5.tar.gz` & `tmp/optax-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optax-0.1.5.tar", last modified: Thu Apr 20 14:42:18 2023, max compression
+gzip compressed data, was "optax-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `optax-0.1.5.tar` & `optax-0.1.7.tar`

### file list

```diff
@@ -1,88 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.392917 optax-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-20 14:42:04.000000 optax-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-20 14:42:04.000000 optax-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-04-20 14:42:18.392917 optax-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-04-20 14:42:04.000000 optax-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.384917 optax-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-04-20 14:42:04.000000 optax-0.1.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.384917 optax-0.1.5/docs/ext/
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-20 14:42:04.000000 optax-0.1.5/docs/ext/coverage_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.384917 optax-0.1.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-20 14:42:04.000000 optax-0.1.5/examples/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-20 14:42:04.000000 optax-0.1.5/examples/datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-04-20 14:42:04.000000 optax-0.1.5/examples/differentially_private_sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-20 14:42:04.000000 optax-0.1.5/examples/flax_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-20 14:42:04.000000 optax-0.1.5/examples/haiku_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-20 14:42:04.000000 optax-0.1.5/examples/lookahead_mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-20 14:42:04.000000 optax-0.1.5/examples/lookahead_mnist_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-20 14:42:04.000000 optax-0.1.5/examples/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-20 14:42:04.000000 optax-0.1.5/examples/mnist_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.384917 optax-0.1.5/optax/
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-20 14:42:04.000000 optax-0.1.5/optax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.388917 optax-0.1.5/optax/_src/
--rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/alias_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/clipping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/combine_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/constrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/constrain_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/control_variates.py
--rw-r--r--   0 runner    (1001) docker     (123)    21789 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/control_variates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/equivalence_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.388917 optax-0.1.5/optax/_src/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/experimental/complex_valued.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/experimental/complex_valued_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/experimental/extra_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/experimental/extra_args_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/factorized.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/factorized_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/float64_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/linear_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/linear_algebra_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/lookahead.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/lookahead_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22680 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/loss_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/numerics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/numerics_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/privacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/privacy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23336 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    25900 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/schedule_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/second_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/second_order_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/state_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/state_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/stochastic_gradient_estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/stochastic_gradient_estimators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    39085 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/transform_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/update_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21653 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    26244 2023-04-20 14:42:04.000000 optax-0.1.5/optax/_src/wrappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.388917 optax-0.1.5/optax/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-20 14:42:04.000000 optax-0.1.5/optax/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-20 14:42:04.000000 optax-0.1.5/optax/optax_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.384917 optax-0.1.5/optax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-04-20 14:42:18.000000 optax-0.1.5/optax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-20 14:42:18.000000 optax-0.1.5/optax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:42:18.000000 optax-0.1.5/optax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:42:18.000000 optax-0.1.5/optax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-20 14:42:18.000000 optax-0.1.5/optax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 14:42:18.000000 optax-0.1.5/optax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:42:18.388917 optax-0.1.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 14:42:04.000000 optax-0.1.5/requirements/minimum-requirements-dp-accounting.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-20 14:42:04.000000 optax-0.1.5/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-20 14:42:04.000000 optax-0.1.5/requirements/requirements-examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 14:42:04.000000 optax-0.1.5/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-20 14:42:04.000000 optax-0.1.5/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:42:18.392917 optax-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-20 14:42:04.000000 optax-0.1.5/setup.py
+-rw-r--r--   0        0        0    11358 2023-07-26 21:24:25.467386 optax-0.1.7/LICENSE
+-rw-r--r--   0        0        0    11393 2023-07-26 21:24:25.467386 optax-0.1.7/README.md
+-rw-r--r--   0        0        0    13095 2023-07-26 21:24:25.471386 optax-0.1.7/optax/__init__.py
+-rw-r--r--   0        0        0    37367 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/alias.py
+-rw-r--r--   0        0        0     7426 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/alias_test.py
+-rw-r--r--   0        0        0    11453 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/base.py
+-rw-r--r--   0        0        0     6609 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/base_test.py
+-rw-r--r--   0        0        0     7499 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/clipping.py
+-rw-r--r--   0        0        0     3774 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/clipping_test.py
+-rw-r--r--   0        0        0     6636 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/combine.py
+-rw-r--r--   0        0        0     8534 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/combine_test.py
+-rw-r--r--   0        0        0     3242 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/constrain.py
+-rw-r--r--   0        0        0     4200 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/constrain_test.py
+-rw-r--r--   0        0        0     8037 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/contrib/mechanic.py
+-rw-r--r--   0        0        0     7168 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/contrib/mechanic_test.py
+-rw-r--r--   0        0        0    17563 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/control_variates.py
+-rw-r--r--   0        0        0    21789 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/control_variates_test.py
+-rw-r--r--   0        0        0     5954 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/equivalence_test.py
+-rw-r--r--   0        0        0     4101 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/experimental/complex_valued.py
+-rw-r--r--   0        0        0     2870 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/experimental/complex_valued_test.py
+-rw-r--r--   0        0        0     6217 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/experimental/extra_args.py
+-rw-r--r--   0        0        0     2043 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/experimental/extra_args_test.py
+-rw-r--r--   0        0        0     7407 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/factorized.py
+-rw-r--r--   0        0        0     1634 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/factorized_test.py
+-rw-r--r--   0        0        0     3783 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/float64_test.py
+-rw-r--r--   0        0        0     7495 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/linear_algebra.py
+-rw-r--r--   0        0        0     2177 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/linear_algebra_test.py
+-rw-r--r--   0        0        0     7478 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/lookahead.py
+-rw-r--r--   0        0        0     5702 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/lookahead_test.py
+-rw-r--r--   0        0        0    24617 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/loss.py
+-rw-r--r--   0        0        0    22156 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/loss_test.py
+-rw-r--r--   0        0        0     4643 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/numerics.py
+-rw-r--r--   0        0        0     4198 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/numerics_test.py
+-rw-r--r--   0        0        0     2731 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/privacy.py
+-rw-r--r--   0        0        0     4565 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/privacy_test.py
+-rw-r--r--   0        0        0    23336 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/schedule.py
+-rw-r--r--   0        0        0    25900 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/schedule_test.py
+-rw-r--r--   0        0        0     3545 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/second_order.py
+-rw-r--r--   0        0        0     3060 2023-07-26 21:24:25.471386 optax-0.1.7/optax/_src/second_order_test.py
+-rw-r--r--   0        0        0     4162 2023-07-26 21:24:25.475386 optax-0.1.7/optax/_src/state_utils.py
+-rw-r--r--   0        0        0     7741 2023-07-26 21:24:25.475386 optax-0.1.7/optax/_src/state_utils_test.py
+-rw-r--r--   0        0        0    12277 2023-07-26 21:24:25.475386 optax-0.1.7/optax/_src/stochastic_gradient_estimators.py
+-rw-r--r--   0        0        0    13766 2023-07-26 21:24:25.475386 optax-0.1.7/optax/_src/stochastic_gradient_estimators_test.py
+-rw-r--r--   0        0        0     1458 2023-07-26 21:24:25.475386 optax-0.1.7/optax/_src/test_utils.py
+-rw-r--r--   0        0        0    39085 2023-07-26 21:24:25.475386 optax-0.1.7/optax/_src/transform.py
+-rw-r--r--   0        0        0    10403 2023-07-26 21:24:25.475386 optax-0.1.7/optax/_src/transform_test.py
+-rw-r--r--   0        0        0     3692 2023-07-26 21:24:25.475386 optax-0.1.7/optax/_src/update.py
+-rw-r--r--   0        0        0     2874 2023-07-26 21:24:25.475386 optax-0.1.7/optax/_src/update_test.py
+-rw-r--r--   0        0        0     5415 2023-07-26 21:24:25.475386 optax-0.1.7/optax/_src/utils.py
+-rw-r--r--   0        0        0     8290 2023-07-26 21:24:25.475386 optax-0.1.7/optax/_src/utils_test.py
+-rw-r--r--   0        0        0    22980 2023-07-26 21:24:25.475386 optax-0.1.7/optax/_src/wrappers.py
+-rw-r--r--   0        0        0    29183 2023-07-26 21:24:25.475386 optax-0.1.7/optax/_src/wrappers_test.py
+-rw-r--r--   0        0        0      840 2023-07-26 21:24:25.475386 optax-0.1.7/optax/contrib/__init__.py
+-rw-r--r--   0        0        0     1082 2023-07-26 21:24:25.475386 optax-0.1.7/optax/experimental/__init__.py
+-rw-r--r--   0        0        0      986 2023-07-26 21:24:25.475386 optax-0.1.7/optax/optax_test.py
+-rw-r--r--   0        0        0     1909 2023-07-26 21:24:25.475386 optax-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    13834 1970-01-01 00:00:00.000000 optax-0.1.7/PKG-INFO
```

### Comparing `optax-0.1.5/LICENSE` & `optax-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/PKG-INFO` & `optax-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,60 @@
 Metadata-Version: 2.1
 Name: optax
-Version: 0.1.5
+Version: 0.1.7
 Summary: A gradient processing and optimisation library in JAX.
-Home-page: https://github.com/deepmind/optax
-Author: DeepMind
-Author-email: optax-dev@google.com
-License: Apache 2.0
-Keywords: reinforcement-learning python machine learning
-Classifier: Development Status :: 5 - Production/Stable
+Keywords: python,machine learning,reinforcement-learning
+Author-email: DeepMind <optax-dev@google.com>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Science/Research
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Requires-Dist: absl-py>=0.7.1
+Requires-Dist: chex>=0.1.5
+Requires-Dist: jax>=0.1.55
+Requires-Dist: jaxlib>=0.1.37
+Requires-Dist: numpy>=1.18.0
+Requires-Dist: sphinx==4.5.0 ; extra == "docs"
+Requires-Dist: sphinx-book-theme==0.3.3 ; extra == "docs"
+Requires-Dist: sphinxcontrib-katex==0.9.0 ; extra == "docs"
+Requires-Dist: sphinxcontrib-bibtex==2.4.2 ; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints==1.11.1 ; extra == "docs"
+Requires-Dist: IPython==7.16.3 ; extra == "docs"
+Requires-Dist: ipykernel==5.3.4 ; extra == "docs"
+Requires-Dist: pandoc==1.0.2 ; extra == "docs"
+Requires-Dist: myst_nb==0.13.1 ; extra == "docs"
+Requires-Dist: docutils==0.16 ; extra == "docs"
+Requires-Dist: matplotlib==3.5.0 ; extra == "docs"
+Requires-Dist: dm-haiku==0.0.8 ; extra == "docs"
+Requires-Dist: absl-py>=1.0.0 ; extra == "dp-accounting"
+Requires-Dist: attrs>=21.4.0 ; extra == "dp-accounting"
+Requires-Dist: mpmath>=1.2.1 ; extra == "dp-accounting"
+Requires-Dist: numpy>=1.21.4 ; extra == "dp-accounting"
+Requires-Dist: scipy>=1.7.1 ; extra == "dp-accounting"
+Requires-Dist: dm-haiku>=0.0.3 ; extra == "examples"
+Requires-Dist: tensorflow-datasets>=4.2.0 ; extra == "examples"
+Requires-Dist: tensorflow>=2.4.0 ; extra == "examples"
+Requires-Dist: dm-haiku>=0.0.3 ; extra == "test"
+Requires-Dist: dm-tree>=0.1.7 ; extra == "test"
+Requires-Dist: flax==0.5.3 ; extra == "test"
+Project-URL: documentation, https://optax.readthedocs.io/
+Project-URL: homepage, https://github.com/deepmind/optax
+Project-URL: repository, https://github.com/deepmind/optax
+Provides-Extra: docs
+Provides-Extra: dp-accounting
+Provides-Extra: examples
+Provides-Extra: test
 
 # Optax
 
 ![CI status](https://github.com/deepmind/optax/workflows/tests/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/optax/badge/?version=latest)](http://optax.readthedocs.io)
 ![pypi](https://img.shields.io/pypi/v/optax)
 
@@ -103,15 +134,15 @@
 You can continue the quick start in [the Optax quickstart notebook.](https://github.com/deepmind/optax/blob/master/examples/quick_start.ipynb)
 
 
 ## Components
 
 We refer to the [docs](https://optax.readthedocs.io/en/latest/index.html)
 for a detailed list of available Optax components. Here, we highlight
-the main categories of buiilding blocks provided by Optax.
+the main categories of building blocks provided by Optax.
 
 ### Gradient Transformations ([transform.py](https://github.com/deepmind/optax/blob/master/optax/_src/transform.py))
 
 One of the key building blocks of `optax` is a `GradientTransformation`.
 
 Each transformation is defined two functions:
 
@@ -301,7 +332,8 @@
 ## Citing Optax
 
 Optax is part of the [DeepMind JAX Ecosystem], to cite Optax please use
 the [DeepMind JAX Ecosystem citation].
 
 [DeepMind JAX Ecosystem]: https://deepmind.com/blog/article/using-jax-to-accelerate-our-research "DeepMind JAX Ecosystem"
 [DeepMind JAX Ecosystem citation]: https://github.com/deepmind/jax/blob/main/deepmind2020jax.txt "Citation"
+
```

### Comparing `optax-0.1.5/README.md` & `optax-0.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 You can continue the quick start in [the Optax quickstart notebook.](https://github.com/deepmind/optax/blob/master/examples/quick_start.ipynb)
 
 
 ## Components
 
 We refer to the [docs](https://optax.readthedocs.io/en/latest/index.html)
 for a detailed list of available Optax components. Here, we highlight
-the main categories of buiilding blocks provided by Optax.
+the main categories of building blocks provided by Optax.
 
 ### Gradient Transformations ([transform.py](https://github.com/deepmind/optax/blob/master/optax/_src/transform.py))
 
 One of the key building blocks of `optax` is a `GradientTransformation`.
 
 Each transformation is defined two functions:
```

### Comparing `optax-0.1.5/optax/__init__.py` & `optax-0.1.7/optax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Optax: composable gradient processing and optimization, in JAX."""
 
+from optax import contrib
 from optax import experimental
 from optax._src.alias import adabelief
 from optax._src.alias import adafactor
 from optax._src.alias import adagrad
 from optax._src.alias import adam
 from optax._src.alias import adamax
 from optax._src.alias import adamaxw
@@ -183,15 +184,15 @@
 from optax._src.wrappers import MaybeUpdateState
 from optax._src.wrappers import MultiSteps
 from optax._src.wrappers import MultiStepsState
 from optax._src.wrappers import ShouldSkipUpdateFunction
 from optax._src.wrappers import skip_large_updates
 from optax._src.wrappers import skip_not_finite
 
-__version__ = "0.1.5"
+__version__ = "0.1.7"
 
 __all__ = (
     "adabelief",
     "adafactor",
     "adagrad",
     "adam",
     "adamax",
```

### Comparing `optax-0.1.5/optax/_src/alias.py` & `optax-0.1.7/optax/_src/alias.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/alias_test.py` & `optax-0.1.7/optax/_src/alias_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/base.py` & `optax-0.1.7/optax/_src/base.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/base_test.py` & `optax-0.1.7/optax/_src/base_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/clipping.py` & `optax-0.1.7/optax/_src/clipping.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/clipping_test.py` & `optax-0.1.7/optax/_src/clipping_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/combine.py` & `optax-0.1.7/optax/_src/combine.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 class MultiTransformState(NamedTuple):
   inner_states: Mapping[Hashable, base.OptState]
 
 
 def multi_transform(
     transforms: Mapping[Hashable, base.GradientTransformation],
     param_labels: Union[base.PyTree, Callable[[base.PyTree], base.PyTree]]
-) -> base.GradientTransformation:
+) -> base.GradientTransformationExtraArgs:
   """Partitions params and applies a different transformation to each subset.
 
   Below is an example where we apply Adam to the weights and SGD to the biases
   of a 2-layer neural network::
 
     import optax
     import jax
@@ -126,14 +126,20 @@
       parameters/updates (or a function that returns one given the parameters as
       input). The leaves of this PyTree correspond to the keys of the transforms
       (therefore the values at the leaves must be a subset of the keys).
 
   Returns:
     An ``optax.GradientTransformation``.
   """
+
+  transforms = {
+      k: base.with_extra_args_support(v)
+      for k, v in transforms.items()
+  }
+
   def make_mask(labels, group):
     return jax.tree_util.tree_map(lambda label: label == group, labels)
 
   def init_fn(params):
     labels = param_labels(params) if callable(param_labels) else param_labels
 
     label_set = set(jax.tree_util.tree_leaves(labels))
@@ -144,17 +150,17 @@
 
     inner_states = {
         group: wrappers.masked(tx, make_mask(labels, group)).init(params)
         for group, tx in transforms.items()
     }
     return MultiTransformState(inner_states)
 
-  def update_fn(updates, state, params=None):
+  def update_fn(updates, state, params=None, **extra_args):
     labels = param_labels(updates) if callable(param_labels) else param_labels
     new_inner_state = {}
     for group, tx in transforms.items():
       masked_tx = wrappers.masked(tx, make_mask(labels, group))
       updates, new_inner_state[group] = masked_tx.update(
-          updates, state.inner_states[group], params)
+          updates, state.inner_states[group], params, **extra_args)
     return updates, MultiTransformState(new_inner_state)
 
-  return base.GradientTransformation(init_fn, update_fn)
+  return base.GradientTransformationExtraArgs(init_fn, update_fn)
```

### Comparing `optax-0.1.5/optax/_src/combine_test.py` & `optax-0.1.7/optax/_src/combine_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -175,14 +175,52 @@
     chex.assert_trees_all_close(updates, correct_updates)
 
     # Check repeated application, this time with no params.
     correct_updates = correct_update_fn(correct_updates)
     updates, state = update_fn(updates, state)
     chex.assert_trees_all_close(updates, correct_updates)
 
+  def test_extra_args(self):
+
+    class ArgNotEqual1Error(ValueError):
+      """Raised when argument not set as expected."""
+
+    def init(params):
+      return {'mu': params}
+
+    def update_with_arg(updates, state, params=None, *, arg, **extra_args):
+      del params, extra_args
+      if arg != 1:
+        raise ArgNotEqual1Error()
+      return updates, state
+
+    def update_without_arg(updates, state, params=None):
+      del params
+      return updates, state
+
+    opt_no_arg = base.GradientTransformation(init, update_without_arg)
+    opt_extra_arg = base.GradientTransformationExtraArgs(init, update_with_arg)
+
+    opt = combine.multi_transform(
+        {
+            'a': opt_no_arg,
+            'b': opt_extra_arg,
+        },
+        ('a', 'b'),
+    )
+
+    fake_params = ({'u': jnp.array([1])}, {'v': jnp.array([1])})
+    state = opt.init(fake_params)
+
+    with self.assertRaises(TypeError):
+      opt.update(fake_params, state)
+    with self.assertRaises(ArgNotEqual1Error):
+      opt.update(fake_params, state, arg=2, ignored_kwarg='hi')
+    opt.update(fake_params, state, arg=1, ignored_kwarg='hi')
+
   @parameterized.parameters(list, tuple, dict)
   def test_empty(self, container):
     init_fn, update_fn = combine.multi_transform(
         {0: alias.sgd(1.)}, lambda _: 0)
     updates, _ = update_fn(container(), init_fn(container()))
     self.assertEqual(updates, container())
```

### Comparing `optax-0.1.5/optax/_src/constrain.py` & `optax-0.1.7/optax/_src/constrain.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/constrain_test.py` & `optax-0.1.7/optax/_src/constrain_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/control_variates.py` & `optax-0.1.7/optax/_src/control_variates.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/control_variates_test.py` & `optax-0.1.7/optax/_src/control_variates_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/equivalence_test.py` & `optax-0.1.7/optax/_src/equivalence_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/experimental/complex_valued.py` & `optax-0.1.7/optax/_src/experimental/complex_valued.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/experimental/complex_valued_test.py` & `optax-0.1.7/optax/_src/experimental/complex_valued_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/experimental/extra_args.py` & `optax-0.1.7/optax/_src/experimental/extra_args.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/experimental/extra_args_test.py` & `optax-0.1.7/optax/_src/experimental/extra_args_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/factorized.py` & `optax-0.1.7/optax/_src/factorized.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/factorized_test.py` & `optax-0.1.7/optax/_src/factorized_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,12 +39,12 @@
     transform_fn = self.variant(scaler.update)
 
     state = init_fn(params)
     chex.assert_tree_all_finite(state)
 
     updates, state = transform_fn(self.per_step_updates, state, params)
     chex.assert_tree_all_finite((params, updates, state))
-    chex.assert_tree_all_equal_shapes(params, updates)
+    chex.assert_trees_all_equal_shapes(params, updates)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `optax-0.1.5/optax/_src/float64_test.py` & `optax-0.1.7/optax/_src/float64_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/linear_algebra.py` & `optax-0.1.7/optax/_src/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/linear_algebra_test.py` & `optax-0.1.7/optax/_src/linear_algebra_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/lookahead.py` & `optax-0.1.7/optax/_src/lookahead.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/lookahead_test.py` & `optax-0.1.7/optax/_src/lookahead_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/loss.py` & `optax-0.1.7/optax/_src/loss.py`

 * *Files 7% similar despite different names*

```diff
@@ -125,21 +125,19 @@
   Smoothed labels favour small logit gaps, and it has been shown that this can
   provide better model calibration by preventing overconfident predictions.
 
   References:
     [Müller et al, 2019](https://arxiv.org/pdf/1906.02629.pdf)
 
   Args:
-    labels: one hot labels to be smoothed.
-    alpha: the smoothing factor, the greedy category with be assigned
-      probability `(1-alpha) + alpha / num_categories`
+    labels: One hot labels to be smoothed.
+    alpha: The smoothing factor.
 
   Returns:
     a smoothed version of the one hot input labels.
-
   """
   chex.assert_type([labels], float)
   num_categories = labels.shape[-1]
   return (1.0 - alpha) * labels + alpha / num_categories
 
 
 def sigmoid_binary_cross_entropy(logits, labels):
@@ -447,15 +445,15 @@
 
   # last row needs to be updated with the last epsilon transition
   logalpha_phi_last = update_phi_score(logalpha_phi[-1], logalpha_emit[-1])
   logalpha_phi = logalpha_phi.at[-1].set(logalpha_phi_last)
 
   # extract per_seq_loss
   one_hot = jax.nn.one_hot(labellens, num_classes=maxlabellen + 1)  # [B, N+1]
-  per_seq_loss = -jnp.einsum('bn,bn->b', logalpha_phi_last, one_hot)
+  per_seq_loss = -jnp.einsum('bn,bn->b', logalpha_phi_last, one_hot)  # pylint:disable=invalid-unary-operand-type
 
   return per_seq_loss, logalpha_phi, logalpha_emit
 
 
 def ctc_loss(logits: chex.Array,
              logit_paddings: chex.Array,
              labels: chex.Array,
@@ -578,7 +576,52 @@
     predictor_outputs: Outputs of the decision function.
     targets: Target values. Target values should be strictly in the set {-1, 1}.
 
   Returns:
     Binary Hinge Loss.
   """
   return jnp.maximum(0, 1 - predictor_outputs * targets)
+
+
+def poly_loss_cross_entropy(
+    logits: chex.Array, labels: chex.Array, epsilon: float = 2.0
+) -> chex.Array:
+  r"""Computes PolyLoss between logits and labels.
+
+  The PolyLoss is a loss function that decomposes commonly
+  used classification loss functions into a series of weighted
+  polynomial bases. It is inspired by the Taylor expansion of
+  cross-entropy loss and focal loss in the bases of :math:`(1 − P_t)^j`.
+
+  .. math::
+    L_{Poly} = \sum_1^\infty \alpha_j \cdot (1 - P_t)^j \\
+    L_{Poly-N} = (\epsilon_1 + 1) \cdot (1 - P_t) + \ldots + \\
+    (\epsilon_N + \frac{1}{N}) \cdot (1 - P_t)^N +
+    \frac{1}{N + 1} \cdot (1 - P_t)^{N + 1} + \ldots = \\
+    - \log(P_t) + \sum_{j = 1}^N \epsilon_j \cdot (1 - P_t)^j
+
+  This function provides a simplified version of :math:`L_{Poly-N}`
+  with only the coefficient of the first polynomial term being changed.
+
+  References:
+    [Zhaoqi Leng et al, 2022](https://arxiv.org/pdf/2204.12511.pdf)
+
+  Args:
+    logits: Unnormalized log probabilities, with shape `[..., num_classes]`.
+    labels: Valid probability distributions (non-negative, sum to 1), e.g. a
+      one hot encoding specifying the correct class for each input;
+      must have a shape broadcastable to `[..., num_classes]`.
+    epsilon: The coefficient of the first polynomial term.
+      According to the paper, the following values are recommended:
+      - For the ImageNet 2d image classification, epsilon = 2.0.
+      - For the 2d Instance Segmentation and object detection, epsilon = -1.0.
+      - It is also recommended to adjust this value based on the task, e.g. by
+        using grid search.
+
+  Returns:
+    Poly loss between each prediction and the corresponding target
+    distributions, with shape `[...]`.
+  """
+  chex.assert_type([logits, labels], float)
+  one_minus_pt = jnp.sum(labels * (1 - jax.nn.softmax(logits)), axis=-1)
+  cross_entropy = softmax_cross_entropy(logits=logits, labels=labels)
+  return cross_entropy + epsilon * one_minus_pt
```

### Comparing `optax-0.1.5/optax/_src/loss_test.py` & `optax-0.1.7/optax/_src/loss_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -552,9 +552,94 @@
   @chex.all_variants
   def test_batched(self):
     np.testing.assert_allclose(
         self.variant(loss.hinge_loss)(self.ys, self.ts),
         self.correct_result,
         atol=1e-4)
 
+
+class PolyLossTest(parameterized.TestCase):
+
+  def setUp(self):
+    super().setUp()
+    self.logits = np.array([0.14, 1.456, 2.356, -0.124, -2.47])
+    self.labels = np.array([0.1, 0.15, 0.2, 0.25, 0.3])
+
+    self.batched_logits = np.array([[4.0, 2.0, 1.0], [0.0, 5.0, 1.0]])
+    self.batched_labels = np.array([[1.0, 0.0, 0.0], [0.0, 0.8, 0.2]])
+    # all expected values are computed using tf version of `poly1_cross_entropy`
+    # see page 10 here https://arxiv.org/pdf/2204.12511.pdf for more
+
+  @chex.all_variants
+  @parameterized.parameters(
+      dict(eps=2, expected=4.5317),
+      dict(eps=1, expected=3.7153),
+      dict(eps=-1, expected=2.0827),
+      dict(eps=0, expected=2.8990),
+      dict(eps=-0.5, expected=2.4908),
+      dict(eps=1.15, expected=3.8378),
+      dict(eps=1.214, expected=3.8900),
+      dict(eps=5.45, expected=7.3480),
+  )
+  def test_scalar(self, eps, expected):
+    np.testing.assert_allclose(
+        self.variant(loss.poly_loss_cross_entropy)(
+            self.logits, self.labels, eps
+        ),
+        expected,
+        atol=1e-4,
+    )
+
+  @chex.all_variants
+  @parameterized.parameters(
+      dict(eps=2, expected=np.array([0.4823, 1.2567])),
+      dict(eps=1, expected=np.array([0.3261, 1.0407])),
+      dict(eps=0, expected=np.array([0.1698, 0.8247])),
+      dict(eps=-0.5, expected=np.array([0.0917, 0.7168])),
+      dict(eps=1.15, expected=np.array([0.3495, 1.0731])),
+      dict(eps=1.214, expected=np.array([0.3595, 1.0870])),
+      dict(eps=5.45, expected=np.array([1.0211, 2.0018])),
+  )
+  def test_batched(self, eps, expected):
+    np.testing.assert_allclose(
+        self.variant(loss.poly_loss_cross_entropy)(
+            self.batched_logits, self.batched_labels, eps
+        ),
+        expected,
+        atol=1e-4,
+    )
+
+  @chex.all_variants
+  @parameterized.parameters(
+      dict(
+          logits=np.array(
+              [[4.0, 2.0, 1.0], [0.0, 5.0, 1.0], [0.134, 1.234, 3.235]]
+          ),
+          labels=np.array(
+              [[1.0, 0.0, 0.0], [0.0, 0.8, 0.2], [0.34, 0.33, 0.33]]
+          ),
+      ),
+      dict(
+          logits=np.array([[4.0, 2.0, 1.0], [0.0, 5.0, 1.0]]),
+          labels=np.array([[1.0, 0.0, 0.0], [0.0, 0.8, 0.2]]),
+      ),
+      dict(
+          logits=np.array(
+              [[4.0, 2.0, 1.0, 0.134, 1.3515], [0.0, 5.0, 1.0, 0.5215, 5.616]]
+          ),
+          labels=np.array(
+              [[0.5, 0.0, 0.0, 0.0, 0.5], [0.0, 0.12, 0.2, 0.56, 0.12]]
+          ),
+      ),
+      dict(logits=np.array([1.89, 2.39]), labels=np.array([0.34, 0.66])),
+      dict(logits=np.array([0.314]), labels=np.array([1.0])),
+  )
+  def test_equals_to_cross_entropy_when_eps0(self, logits, labels):
+    np.testing.assert_allclose(
+        self.variant(loss.poly_loss_cross_entropy)(logits, labels, epsilon=0.0),
+        self.variant(loss.softmax_cross_entropy)(logits, labels),
+        atol=1e-4,
+    )
+
+
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `optax-0.1.5/optax/_src/numerics.py` & `optax-0.1.7/optax/_src/numerics.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/numerics_test.py` & `optax-0.1.7/optax/_src/numerics_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/privacy.py` & `optax-0.1.7/optax/_src/privacy.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/privacy_test.py` & `optax-0.1.7/optax/_src/privacy_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/schedule.py` & `optax-0.1.7/optax/_src/schedule.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/schedule_test.py` & `optax-0.1.7/optax/_src/schedule_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/second_order.py` & `optax-0.1.7/optax/_src/second_order.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/second_order_test.py` & `optax-0.1.7/optax/_src/second_order_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/state_utils.py` & `optax-0.1.7/optax/_src/state_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         Initable,
     ],
     f: Callable[..., Any],
     state: base.OptState,
     /,
     *rest: Any,
     transform_non_params: Optional[Callable[..., Any]] = None,
+    is_leaf: Optional[Callable[[base.Params], bool]] = None,
 ) -> base.OptState:
   """Apply a callable over all params in the given optimizer state.
 
   This function exists to help construct partition specs over optimizer
   states, in the case that a partition spec is already known for the parameters.
 
   For example, the following will replace all optimizer state parameter trees
@@ -67,14 +68,17 @@
     f: A callable that will be applied for all copies of the parameter tree
       within this optimizer state.
     state: The optimizer state to map over.
     *rest: Additional arguments, having the same shape as the parameter tree,
       that will be passed to f.
     transform_non_params: An optional function that will be called on all
       non-parameter fields within the optimizer state.
+    is_leaf: Passed through to `jax.tree_map`. This makes it possible to ignore
+      parts of the parameter tree e.g. when the gradient transformations modify
+      the shape of the original pytree, such as for ``optax.masked``.
 
   Returns:
     The result of applying the function f on all trees in the optimizer's state
     that have the same shape as the parameter tree, along with the given
     optional extra arguments.
   """
 
@@ -85,15 +89,15 @@
     initable = cast(Initable, initable)  # for pytype checks
     state_with_placeholders = initable.init(placeholder)
   else:
     state_with_placeholders = initable(placeholder)
 
   def map_params(maybe_placeholder_value, value):
     if isinstance(maybe_placeholder_value, _ParamsPlaceholder):
-      return jax.tree_map(f, value, *rest)
+      return jax.tree_map(f, value, *rest, is_leaf=is_leaf)
     elif transform_non_params is not None:
       return transform_non_params(value)
     else:
       return value
 
   return jax.tree_map(
       map_params,
```

### Comparing `optax-0.1.5/optax/_src/state_utils_test.py` & `optax-0.1.7/optax/_src/state_utils_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/stochastic_gradient_estimators.py` & `optax-0.1.7/optax/_src/stochastic_gradient_estimators.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/stochastic_gradient_estimators_test.py` & `optax-0.1.7/optax/_src/stochastic_gradient_estimators_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/test_utils.py` & `optax-0.1.7/optax/_src/test_utils.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/transform.py` & `optax-0.1.7/optax/_src/transform.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/transform_test.py` & `optax-0.1.7/optax/_src/transform_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/update.py` & `optax-0.1.7/optax/_src/update.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/update_test.py` & `optax-0.1.7/optax/_src/update_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/utils.py` & `optax-0.1.7/optax/_src/utils.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/utils_test.py` & `optax-0.1.7/optax/_src/utils_test.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/_src/wrappers.py` & `optax-0.1.7/optax/_src/wrappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 import jax.numpy as jnp
 from jax.tree_util import tree_flatten
 from jax.tree_util import tree_map
 from jax.tree_util import tree_unflatten
 import numpy as np
 from optax._src import base
 from optax._src import numerics
+from optax._src import state_utils
+
 
 Array = jnp.ndarray
 
 
 def flatten(
     inner: base.GradientTransformation
 ) -> base.GradientTransformationExtraArgs:
@@ -469,14 +471,19 @@
 
     mask = jax.tree_util.tree_map(lambda x: x.ndim != 1, params)
     weight_decay = optax.masked(optax.add_decayed_weights(0.001), mask)
 
   For the ``inner`` transform, state will only be stored for the parameters that
   have a mask value of ``True``.
 
+  Note that, when using ``tree_map_params``, it may be required to pass the
+  argument `is_leaf=lambda v: isinstance(v, optax.MaskedNode)`, if the tree
+  map needs to take additional arguments with the same shape as the original
+  input tree.
+
   Args:
     inner: Inner transformation to mask.
     mask: a PyTree with same structure as (or a prefix of) the params PyTree, or
       a Callable that returns such a pytree given the params/updates. The leaves
       should be booleans, ``True`` for leaves/subtrees you want to apply the
       transformation to, and ``False`` for those you want to skip. The mask must
       be static for the gradient transformation to be jit-compilable.
@@ -486,14 +493,29 @@
   """
   inner = base.with_extra_args_support(inner)
 
   def mask_pytree(pytree, mask_tree):
     return tree_map(lambda m, p: p if m else MaskedNode(), mask_tree, pytree)
 
   def init_fn(params):
+    # This is a workaround to make tree_map_params work with masking.
+    # The API of `masked` takes a mask on construction, instead of at init.
+    # This means that this gradient transformation can only work for parameter
+    # trees that match the shape of the mask. Technically this breaks the API
+    # of optax, and this causes tree_map_params to break. This is because
+    # tree_map_params calls init with a placeholder in order to detect copies
+    # of the parameter tree. As a (slightly ugly) workaround, we detect when
+    # the init is being called by tree_map_params, and pass the placeholder
+    # down without masking. This is safe, since tree_map_params does not impose
+    # any particular constraints on the shape of the parameter tree, as long
+    # as tree_map_params is being called on a tree with the correct structure.
+    # See wrappers_test for proof that this works!
+    if isinstance(params, state_utils._ParamsPlaceholder):  # pylint:disable=protected-access
+      return MaskedState(inner_state=inner.init(params))
+
     mask_tree = mask(params) if callable(mask) else mask
     masked_params = mask_pytree(params, mask_tree)
     return MaskedState(inner_state=inner.init(masked_params))
 
   def update_fn(updates, state, params=None, **extra_args):
     mask_tree = mask(updates) if callable(mask) else mask
     masked_updates = mask_pytree(updates, mask_tree)
```

### Comparing `optax-0.1.5/optax/_src/wrappers_test.py` & `optax-0.1.7/optax/_src/wrappers_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Tests for `wrappers.py`."""
 
 import copy
+from typing import cast
 
 from absl.testing import absltest
 from absl.testing import parameterized
-
 import chex
 import haiku as hk
 import jax
 import jax.numpy as jnp
 import numpy as np
 from optax._src import alias
 from optax._src import base
@@ -386,14 +386,115 @@
       params = update.apply_updates(params, updates)
       np.testing.assert_array_equal(params['a'], -jnp.full([], 2.))
 
 
 class MaskedTest(chex.TestCase):
   """Tests for the masked wrapper."""
 
+  def test_tree_map_params(self):
+    params = {
+        'a': {
+            'b': (jnp.zeros((1, 2)), jnp.zeros((2, 2))),
+        },
+        'c': {
+            'd': jnp.zeros((1, 2)),
+            'e': (jnp.zeros((1, 2)), jnp.zeros((1, 2))),
+        },
+    }
+
+    sharding_axes = {
+        'a': {
+            'b': (1, 2),
+        },
+        'c': {
+            'd': 1,
+            'e': (1, 2),
+        },
+    }
+
+    mask = {
+        'a': {
+            'b': (True, False),
+        },
+        'c': {
+            'd': True,
+            'e': (False, True),
+        },
+    }
+
+    expected = {
+        'a': {
+            'b': (jnp.ones((1, 2)), jnp.zeros((2, 2))),
+        },
+        'c': {
+            'd': jnp.ones((1, 2)),
+            'e': (jnp.ones((1, 2)), jnp.ones((1, 2))),
+        },
+    }
+
+    def init_fn(params):
+      return {'count': 1, 'params': params, 'params_copy': params}
+
+    def update_fn(updates, state, params=None):
+      del params
+      return updates, state
+
+    inner = base.GradientTransformation(init_fn, update_fn)
+    masked = wrappers.masked(inner, mask)
+
+    def increment_dim_1(v):
+      return v + 1 if v.shape[0] == 1 else v
+
+    # For this optimizer, tree_map_params should have the same effect on a
+    # masked optimizer state as it does on an unmasked optimizer state.
+    with self.subTest('inner'):
+      state = inner.init(params)
+      result = state_utils.tree_map_params(inner, increment_dim_1, state)
+      chex.assert_trees_all_equal(result, inner.init(expected))
+
+    with self.subTest('masked'):
+      state = masked.init(params)
+      result = state_utils.tree_map_params(masked, increment_dim_1, state)
+      chex.assert_trees_all_equal(result, masked.init(expected))
+
+    with self.subTest('masked_with_extra_args'):
+      # Users wishing to pass additional arguments with the same tree structure
+      # as the original params pytree will need to add the additional `is_leaf`
+      # callable. This makes it possible to ignore the masked parts of the
+      # pytree.
+
+      # Replace all non-masked parameters in the opt-state tree with the
+      # sharding axis values given in the tree above. Everything else is set to
+      # None.
+      new_state = state_utils.tree_map_params(
+          masked,
+          lambda p, axis: None if isinstance(p, wrappers.MaskedNode) else axis,
+          state,
+          sharding_axes,
+          is_leaf=lambda v: isinstance(v, wrappers.MaskedNode),
+          transform_non_params=lambda v: None,
+      )
+
+      sharded_params = {
+          'a': {
+              'b': (1, None),
+          },
+          'c': {
+              'd': 1,
+              'e': (None, 2),
+          },
+      }
+
+      # Required to make pytype happy
+      new_state = cast(wrappers.MaskedState, new_state)
+
+      chex.assert_equal(None, new_state.inner_state['count'])
+      chex.assert_equal(sharded_params, new_state.inner_state['params'])
+      chex.assert_equal(sharded_params, new_state.inner_state['params_copy'])
+
   @chex.all_variants
   @parameterized.named_parameters(
       ('sgd', _build_sgd, False),
       ('stateful_sgd', _build_stateful_sgd, False),
       ('sgd_w_mask_fn', _build_sgd, True),
       ('stateful_sgd_w_mask_fn', _build_stateful_sgd, True),
   )
@@ -412,18 +513,17 @@
           lambda upd, m: -upd if m else upd, updates, mask)
     correct_updates = masked_negate(input_updates)
 
     init_fn, update_fn = wrappers.masked(opt_builder(), mask_arg)
     update_fn = self.variant(update_fn)
     state = self.variant(init_fn)(params)
 
-    # Known issue: masked does not work with arbitrary parameter trees, and
-    # so does not work with tree_map_params.
-    with self.assertRaises(ValueError):
-      state_utils.tree_map_params(init_fn, lambda v: v, state)
+    with self.subTest('tree_map_params'):
+      result = state_utils.tree_map_params(init_fn, lambda v: v, state)
+      chex.assert_tree_all_equal_structs(result, state)
 
     updates, state = update_fn(input_updates, state, params)
     chex.assert_trees_all_close(updates, correct_updates)
 
     # Check repeated application, this time with no params.
     correct_updates = masked_negate(correct_updates)
     updates, state = update_fn(updates, state)
@@ -452,15 +552,15 @@
     state = self.variant(init_fn)(params)
     updates, state = update_fn(input_updates, state, params)
     chex.assert_trees_all_close(updates, correct_updates)
 
     # Check repeated application, this time with no params.
     correct_updates = jax.tree_util.tree_map(
         _masked_sgd_on_updates, mask, correct_updates)
-    updates, state = update_fn(updates, state)
+    updates, _ = update_fn(updates, state)
     chex.assert_trees_all_close(updates, correct_updates)
 
   @chex.all_variants
   def test_update_requires_params(self):
     weight_decay = 0.1
     mask = {'a': True,
             'b': [False, True],
@@ -565,15 +665,15 @@
     mask = {'a': [True, (True, False)], 'b': False}
     tx = wrappers.masked(_build_stateful_sgd(), mask)
     trace = self.variant(tx.init)(params).inner_state[0].trace
     expected_trace = {
         'a': [jnp.zeros(1), (jnp.zeros(2), wrappers.MaskedNode())],
         'b': wrappers.MaskedNode()
     }
-    chex.assert_tree_all_equal_structs(trace, expected_trace)
+    chex.assert_trees_all_equal_structs(trace, expected_trace)
 
   def test_masked_state_is_compatible_with_deepmind_tree(self):
     """Checks that the masked state is compatible with deepmind/tree.
 
     DeepMind's tree library and `jax.tree_util` have slightly different
     behavior: jax treats `None`s as tree nodes without children while
     deepmind/tree treats them as leaves with `None` values. This has led to bugs
```

### Comparing `optax-0.1.5/optax/experimental/__init__.py` & `optax-0.1.7/optax/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `optax-0.1.5/optax/optax_test.py` & `optax-0.1.7/optax/optax_test.py`

 * *Files identical despite different names*


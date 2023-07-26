# Comparing `tmp/sparse-lm-0.5.0.tar.gz` & `tmp/sparse-lm-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparse-lm-0.5.0.tar", last modified: Wed Jul 12 00:23:31 2023, max compression
+gzip compressed data, was "sparse-lm-0.5.1.tar", last modified: Tue Jul 25 23:59:09 2023, max compression
```

## Comparing `sparse-lm-0.5.0.tar` & `sparse-lm-0.5.1.tar`

### file list

```diff
@@ -1,81 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.448223 sparse-lm-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.440223 sparse-lm-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.440223 sparse-lm-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.440223 sparse-lm-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.github/workflows/update-precommit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-12 00:23:31.448223 sparse-lm-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.440223 sparse-lm-0.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.440223 sparse-lm-0.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   235080 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/_static/logo-light.png
--rw-r--r--   0 runner    (1001) docker     (123)   230291 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/sparselm.model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/sparselm.model_selection.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/sparselm.stepwise.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/docs/sparselm.tools.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.444223 sparse-lm-0.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)   153248 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/examples/corr.npy
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/examples/energy.npy
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/examples/plot_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/examples/plot_chull.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/examples/plot_gl_sgl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/examples/plot_sparse_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)   399600 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/examples/structures.json
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 00:23:31.448223 sparse-lm-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.440223 sparse-lm-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.444223 sparse-lm-0.5.0/src/sparse_lm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-12 00:23:31.000000 sparse-lm-0.5.0/src/sparse_lm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-12 00:23:31.000000 sparse-lm-0.5.0/src/sparse_lm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 00:23:31.000000 sparse-lm-0.5.0/src/sparse_lm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-12 00:23:31.000000 sparse-lm-0.5.0/src/sparse_lm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 00:23:31.000000 sparse-lm-0.5.0/src/sparse_lm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.444223 sparse-lm-0.5.0/src/sparselm/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.444223 sparse-lm-0.5.0/src/sparselm/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/_utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.448223 sparse-lm-0.5.0/src/sparselm/model/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33463 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/_adaptive_lasso.py
--rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    31119 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/_lasso.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.448223 sparse-lm-0.5.0/src/sparselm/model/_miqp/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/_miqp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/_miqp/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/_miqp/_best_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/_miqp/_regularized_l0.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model/_ols.py
--rw-r--r--   0 runner    (1001) docker     (123)    33496 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/model_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/stepwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/src/sparselm/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:23:31.448223 sparse-lm-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9808 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/test_lasso.py
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/test_miqp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/test_model_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/test_ols.py
--rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/test_stepwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-12 00:23:21.000000 sparse-lm-0.5.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:59:09.787854 sparse-lm-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:59:09.779854 sparse-lm-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:59:09.779854 sparse-lm-0.5.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:59:09.779854 sparse-lm-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/.github/workflows/update-precommit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-25 23:59:09.787854 sparse-lm-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:59:09.779854 sparse-lm-0.5.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:59:09.783854 sparse-lm-0.5.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   235080 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/docs/_static/logo-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)   230291 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/docs/sparselm.model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/docs/sparselm.model_selection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/docs/sparselm.stepwise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/docs/sparselm.tools.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:59:09.783854 sparse-lm-0.5.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   153248 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/examples/corr.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/examples/energy.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/examples/plot_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/examples/plot_chull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/examples/plot_gl_sgl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/examples/plot_line_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/examples/plot_one_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/examples/plot_sparse_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/examples/plot_stepwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)   399600 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/examples/structures.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 23:59:09.787854 sparse-lm-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:59:09.775854 sparse-lm-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:59:09.783854 sparse-lm-0.5.1/src/sparse_lm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-25 23:59:09.000000 sparse-lm-0.5.1/src/sparse_lm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-25 23:59:09.000000 sparse-lm-0.5.1/src/sparse_lm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 23:59:09.000000 sparse-lm-0.5.1/src/sparse_lm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-25 23:59:09.000000 sparse-lm-0.5.1/src/sparse_lm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 23:59:09.000000 sparse-lm-0.5.1/src/sparse_lm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:59:09.787854 sparse-lm-0.5.1/src/sparselm/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/src/sparselm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:59:09.787854 sparse-lm-0.5.1/src/sparselm/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/src/sparselm/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/src/sparselm/_utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/src/sparselm/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:59:09.787854 sparse-lm-0.5.1/src/sparselm/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/src/sparselm/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33463 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/src/sparselm/model/_adaptive_lasso.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/src/sparselm/model/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31119 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/src/sparselm/model/_lasso.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:59:09.787854 sparse-lm-0.5.1/src/sparselm/model/_miqp/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/src/sparselm/model/_miqp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/src/sparselm/model/_miqp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/src/sparselm/model/_miqp/_best_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/src/sparselm/model/_miqp/_regularized_l0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/src/sparselm/model/_ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33540 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/src/sparselm/model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/src/sparselm/stepwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/src/sparselm/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:59:09.787854 sparse-lm-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9808 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/tests/test_lasso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/tests/test_miqp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/tests/test_model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/tests/test_ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/tests/test_stepwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-25 23:58:59.000000 sparse-lm-0.5.1/tests/test_tools.py
```

### Comparing `sparse-lm-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `sparse-lm-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md` & `sparse-lm-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/.github/pull_request_template.md` & `sparse-lm-0.5.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/.github/workflows/build.yml` & `sparse-lm-0.5.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/.github/workflows/docs.yml` & `sparse-lm-0.5.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/.github/workflows/lint.yml` & `sparse-lm-0.5.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/.github/workflows/test.yml` & `sparse-lm-0.5.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/.github/workflows/update-precommit.yaml` & `sparse-lm-0.5.1/.github/workflows/update-precommit.yaml`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/.gitignore` & `sparse-lm-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/.pre-commit-config.yaml` & `sparse-lm-0.5.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -14,35 +14,35 @@
     - --remove
   - id: end-of-file-fixer
   - id: trailing-whitespace
   - id: check-added-large-files
     args: ['--maxkb=500']
 
 - repo: https://github.com/psf/black
-  rev: 23.3.0
+  rev: 23.7.0
   hooks:
   - id: black
 
 - repo: https://github.com/asottile/blacken-docs
-  rev: 1.14.0
+  rev: 1.15.0
   hooks:
   - id: blacken-docs
     additional_dependencies: [black==23.1.0]
     exclude: README.md
 
 - repo: https://github.com/pycqa/isort
   rev: 5.12.0
   hooks:
   - id: isort
     name: isort (python)
     args:
     - --profile=black
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.8.0
+  rev: v3.9.0
   hooks:
     - id: pyupgrade
       args: [--py38-plus]
 
 - repo: https://github.com/PyCQA/autoflake
   rev: v2.2.0
   hooks:
```

### Comparing `sparse-lm-0.5.0/LICENSE` & `sparse-lm-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/PKG-INFO` & `sparse-lm-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparse-lm
-Version: 0.5.0
+Version: 0.5.1
 Summary: Sparse linear regression models
 Author-email: Luis Barroso-Luque <lbluque@berkeley.edu>
 License: BSD 3-Clause License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `sparse-lm-0.5.0/README.md` & `sparse-lm-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/docs/_static/logo-light.png` & `sparse-lm-0.5.1/docs/_static/logo-light.png`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/docs/_static/logo.png` & `sparse-lm-0.5.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/docs/conf.py` & `sparse-lm-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/docs/contributing.rst` & `sparse-lm-0.5.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/docs/index.rst` & `sparse-lm-0.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/docs/install.rst` & `sparse-lm-0.5.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/examples/corr.npy` & `sparse-lm-0.5.1/examples/corr.npy`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/examples/energy.npy` & `sparse-lm-0.5.1/examples/energy.npy`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/examples/plot_adaptive.py` & `sparse-lm-0.5.1/examples/plot_adaptive.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,25 +75,26 @@
 
 print("Adaptive Lasso performance metrics:")
 print(f"    train r2: {alasso_train['r2']:.3f}")
 print(f"    test r2: {alasso_test['r2']:.3f}")
 print(f"    train rmse: {alasso_train['rmse']:.3f}")
 print(f"    test rmse: {alasso_test['rmse']:.3f}")
 
+# plot model coefficients
+fig, ax = plt.subplots()
+ax.plot(coef, "o", label="True coefficients")
+ax.plot(lasso_cv.best_estimator_.coef_, "o", label="Lasso", alpha=0.5)
+ax.plot(alasso_cv.best_estimator_.coef_, "o", label="Adaptive Lasso", alpha=0.5)
+ax.set_xlabel("covariate index")
+ax.set_ylabel("coefficient value")
+ax.legend()
+fig.show()
+
 # plot predicted values
 fig, ax = plt.subplots()
 ax.plot(y_test, lasso_cv.predict(X_test), "o", label="lasso", alpha=0.5)
 ax.plot(y_test, alasso_cv.predict(X_test), "o", label="adaptive lasso", alpha=0.5)
 ax.plot([y_test.min(), y_test.max()], [y_test.min(), y_test.max()], "k--")
 ax.set_xlabel("true values")
 ax.set_ylabel("predicted values")
 ax.legend()
 fig.show()
-
-# plot model coefficients
-fig, ax = plt.subplots()
-ax.plot(coef, "o", label="True coefficients")
-ax.plot(lasso_cv.best_estimator_.coef_, "o", label="Lasso", alpha=0.5)
-ax.plot(alasso_cv.best_estimator_.coef_, "o", label="Adaptive Lasso", alpha=0.5)
-ax.set_xlabel("covariate index")
-ax.set_ylabel("coefficient value")
-fig.show()
```

### Comparing `sparse-lm-0.5.0/examples/plot_chull.py` & `sparse-lm-0.5.1/examples/plot_chull.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/examples/plot_gl_sgl.py` & `sparse-lm-0.5.1/examples/plot_gl_sgl.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/examples/plot_sparse_signal.py` & `sparse-lm-0.5.1/examples/plot_sparse_signal.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/examples/structures.json` & `sparse-lm-0.5.1/examples/structures.json`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/pyproject.toml` & `sparse-lm-0.5.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [project.optional-dependencies]
 dev = ["pre-commit", "black", "isort", "flake8", "pylint", "pydocstyle", "flake8-pyproject"]
 # Gurobipy needed by mixedL0 tests, pandas needed by sklearn convention checks.
 tests = ["pytest >=7.2.0", "pytest-cov >=4.0.0", "coverage", "pandas", "gurobipy", "pyscipopt"]
-docs = ["sphinx>=5.3", "furo", "m2r2", "sphinx-gallery"]
+docs = ["sphinx>=5.3", "furo", "m2r2", "sphinx-gallery", "matplotlib", "gurobipy", "pymatgen"]
 optional = ["gurobipy"]
 
 # pyproject.toml
 [tool.setuptools_scm]
 
 # linting tools, etc
 [tool.pytest.ini_options]
```

### Comparing `sparse-lm-0.5.0/src/sparse_lm.egg-info/PKG-INFO` & `sparse-lm-0.5.1/src/sparse_lm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparse-lm
-Version: 0.5.0
+Version: 0.5.1
 Summary: Sparse linear regression models
 Author-email: Luis Barroso-Luque <lbluque@berkeley.edu>
 License: BSD 3-Clause License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `sparse-lm-0.5.0/src/sparse_lm.egg-info/SOURCES.txt` & `sparse-lm-0.5.1/src/sparse_lm.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,18 @@
 docs/_static/logo.png
 examples/README.rst
 examples/corr.npy
 examples/energy.npy
 examples/plot_adaptive.py
 examples/plot_chull.py
 examples/plot_gl_sgl.py
+examples/plot_line_search.py
+examples/plot_one_std.py
 examples/plot_sparse_signal.py
+examples/plot_stepwise.py
 examples/structures.json
 src/sparse_lm.egg-info/PKG-INFO
 src/sparse_lm.egg-info/SOURCES.txt
 src/sparse_lm.egg-info/dependency_links.txt
 src/sparse_lm.egg-info/requires.txt
 src/sparse_lm.egg-info/top_level.txt
 src/sparselm/__init__.py
```

### Comparing `sparse-lm-0.5.0/src/sparselm/_utils/validation.py` & `sparse-lm-0.5.1/src/sparselm/_utils/validation.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/src/sparselm/dataset.py` & `sparse-lm-0.5.1/src/sparselm/dataset.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/src/sparselm/model/__init__.py` & `sparse-lm-0.5.1/src/sparselm/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/src/sparselm/model/_adaptive_lasso.py` & `sparse-lm-0.5.1/src/sparselm/model/_adaptive_lasso.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/src/sparselm/model/_base.py` & `sparse-lm-0.5.1/src/sparselm/model/_base.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/src/sparselm/model/_lasso.py` & `sparse-lm-0.5.1/src/sparselm/model/_lasso.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/src/sparselm/model/_miqp/_base.py` & `sparse-lm-0.5.1/src/sparselm/model/_miqp/_base.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/src/sparselm/model/_miqp/_best_subset.py` & `sparse-lm-0.5.1/src/sparselm/model/_miqp/_best_subset.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/src/sparselm/model/_miqp/_regularized_l0.py` & `sparse-lm-0.5.1/src/sparselm/model/_miqp/_regularized_l0.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/src/sparselm/model/_ols.py` & `sparse-lm-0.5.1/src/sparselm/model/_ols.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/src/sparselm/model_selection.py` & `sparse-lm-0.5.1/src/sparselm/model_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,18 +211,17 @@
             for name in param_names:
                 if all(isinstance(val, numbers.Number) for val in results[name]):
                     p = np.array(results[name], dtype=float)
                     if np.all(p > -1e-9):
                         params.append(p)
             params_sum = np.sum(params, axis=0)
             one_std_dists = np.abs(metrics - m + sig)
-            candidates = np.arange(len(metrics))[
-                one_std_dists < (np.min(one_std_dists) + 0.1 * sig)
-            ]
-            best_index = candidates[np.argmax(params_sum[candidates])]
+            # Guarantees that one-std rule always select larger params than max score.
+            candidates = np.arange(len(metrics))[params_sum >= params_sum[opt_index]]
+            best_index = candidates[np.argmin(one_std_dists[candidates])]
             return best_index
 
     # Overwrite original fit method to allow multiple optimal methods.
     def fit(self, X, y=None, *, groups=None, **fit_params):
         """Run fit with all sets of parameters.
 
         Args:
```

### Comparing `sparse-lm-0.5.0/src/sparselm/stepwise.py` & `sparse-lm-0.5.1/src/sparselm/stepwise.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/src/sparselm/tools.py` & `sparse-lm-0.5.1/src/sparselm/tools.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/tests/conftest.py` & `sparse-lm-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/tests/test_common.py` & `sparse-lm-0.5.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/tests/test_dataset.py` & `sparse-lm-0.5.1/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/tests/test_lasso.py` & `sparse-lm-0.5.1/tests/test_lasso.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/tests/test_miqp.py` & `sparse-lm-0.5.1/tests/test_miqp.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/tests/test_ols.py` & `sparse-lm-0.5.1/tests/test_ols.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/tests/test_stepwise.py` & `sparse-lm-0.5.1/tests/test_stepwise.py`

 * *Files identical despite different names*

### Comparing `sparse-lm-0.5.0/tests/test_tools.py` & `sparse-lm-0.5.1/tests/test_tools.py`

 * *Files identical despite different names*


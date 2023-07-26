# Comparing `tmp/felimination-0.1.2.tar.gz` & `tmp/felimination-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felimination-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "felimination-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `felimination-0.1.2.tar` & `felimination-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     2239 2023-07-04 14:32:12.501369 felimination-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-04 14:32:12.501369 felimination-0.1.2/felimination/__init__.py
--rw-r--r--   0        0        0     3863 2023-07-04 14:32:12.501369 felimination-0.1.2/felimination/importance.py
--rw-r--r--   0        0        0    31833 2023-07-04 14:32:12.501369 felimination-0.1.2/felimination/rfe.py
--rw-r--r--   0        0        0     1413 2023-07-04 14:32:12.501369 felimination-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3595 1970-01-01 00:00:00.000000 felimination-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2167 2023-07-26 14:04:29.525784 felimination-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 14:04:29.525784 felimination-0.2.0/felimination/__init__.py
+-rw-r--r--   0        0        0    27093 2023-07-26 14:04:29.525784 felimination-0.2.0/felimination/drift.py
+-rw-r--r--   0        0        0     3863 2023-07-26 14:04:29.525784 felimination-0.2.0/felimination/importance.py
+-rw-r--r--   0        0        0    31512 2023-07-26 14:04:29.525784 felimination-0.2.0/felimination/rfe.py
+-rw-r--r--   0        0        0     1413 2023-07-26 14:04:29.525784 felimination-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 felimination-0.2.0/PKG-INFO
```

### Comparing `felimination-0.1.2/README.md` & `felimination-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+[![pytest](https://github.com/ClaudioSalvatoreArcidiacono/felimination/workflows/Tests/badge.svg)](https://github.com/ClaudioSalvatoreArcidiacono/felimination/actions?query=workflow%3A%22Tests%22)
+[![PyPI](https://img.shields.io/pypi/v/felimination)](#)
+[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://claudiosalvatorearcidiacono.github.io/felimination/)
+
+
 # felimination
 
 This library contains some useful scikit-learn compatible classes for feature selection.
 
-## [Check out documentation here](https://claudiosalvatorearcidiacono.github.io/felimination/)
-
 ## Features
 
 - [Recursive Feature Elimination with Cross Validation using Permutation Importance](reference/RFE.md#felimination.rfe.PermutationImportanceRFECV)
 
 ## Requirements
 
 - Python 3.7+
@@ -21,15 +24,14 @@
 ```
 pip install felimination
 ```
 
 ## Usage
 
 ```python
-
 from felimination.rfe import PermutationImportanceRFECV
 from sklearn.linear_model import LogisticRegression
 from sklearn.datasets import make_classification
 import numpy as np
 
 
 X, y = make_classification(
@@ -37,45 +39,37 @@
     n_features=20,
     n_informative=6,
     n_redundant=10,
     n_clusters_per_class=1,
     random_state=42,
 )
 
-# Add random features at the end, so the first 2 features are
-# relevant and the remaining 8 features are random
-X_with_rand = np.hstack((X, np.random.random(size=(X.shape[0], 8))))
-
 selector = PermutationImportanceRFECV(LogisticRegression(), step=0.3)
 
-selector.fit(X_with_rand, y)
+selector.fit(X, y)
 
 selector.support_
 # array([False, False, False, False, False, False, False, False, False,
-#        False, False, False, False, True, False, False, False, False,
-#        False, False, False, False, False, False, False, False, False,
-#        False])
+#        False, False,  True, False, False, False, False, False, False,
+#        False, False])
 
 selector.ranking_
-# array([10,  3,  9, 10,  8,  9,  7,  7, 10,  6,  8,  2,  8,  1,  9, 10, 10,
-#         4,  5,  6,  9, 10,  9,  8, 10,  9,  7, 10])
-
+# array([9, 3, 8, 9, 7, 8, 5, 6, 9, 6, 8, 1, 9, 7, 8, 9, 9, 2, 4, 7])
 selector.plot()
 ```
 ![example of plot](./docs/assets/example_plot.png)
 
-It looks like `3` is a good number of features, we can set the number of features to select to 3 without need of retraining
+It looks like `5` is a good number of features, we can set the number of features to select to 5 without need of retraining
 
 ```python
-selector.set_n_features_to_select(3)
+selector.set_n_features_to_select(5)
 selector.support_
-# array([False,  True, False, False, False, False, False, False, False,
-#        False, False,  True, False,  True, False, False, False, False,
-#        False, False, False, False, False, False, False, False, False,
-#        False])
+# array([False,  True, False, False, False, False,  True, False, False,
+#        False, False,  True, False, False, False, False, False,  True,
+#         True, False])
 ```
 
 ## License
 
 This project is licensed under the BSD 3-Clause License - see the LICENSE.md file for details
 
 ## Acknowledgments
```

### Comparing `felimination-0.1.2/felimination/importance.py` & `felimination-0.2.0/felimination/importance.py`

 * *Files identical despite different names*

### Comparing `felimination-0.1.2/felimination/rfe.py` & `felimination-0.2.0/felimination/rfe.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,17 +187,15 @@
         - The least important features are pruned.
         - The pruned features are removed from the dataset.
     ```
 
     Parameters
     ----------
     estimator : ``Estimator`` instance
-        A supervised learning estimator with a ``fit`` method that provides
-        information about feature importance either through a ``coef_``
-        attribute or through a ``feature_importances_`` attribute.
+        A supervised learning estimator with a ``fit`` method.
     step : int or float, default=1
         If greater than or equal to 1, then ``step`` corresponds to the
         (integer) number of features to remove at each iteration.
         If within (0.0, 1.0), then ``step`` corresponds to the percentage
         (rounded down) of **remaining** features to remove at each iteration.
         Note that the last iteration may remove fewer than ``step`` features in
         order to reach ``min_features_to_select``.
@@ -359,14 +357,15 @@
         X, y = self._validate_data(
             X,
             y,
             accept_sparse="csc",
             ensure_min_features=2,
             force_all_finite=not tags.get("allow_nan", True),
             multi_output=True,
+            dtype=None,
         )
 
         # Initialization
         cv = check_cv(self.cv, y, classifier=is_classifier(self.estimator))
         scorer = check_scoring(self.estimator, scoring=self.scoring)
         n_features = X.shape[1]
 
@@ -421,43 +420,43 @@
             ]
             cv_importances = [
                 score_importance[2] for score_importance in scores_importances
             ]
             mean_importances = np.mean(np.vstack(cv_importances), axis=0)
             ranks = np.argsort(mean_importances)
 
+            # for sparse case ranks is matrix
+            ranks = np.ravel(ranks)
+
+            if 0.0 < self.step < 1.0:
+                step = int(max(1, self.step * current_number_of_features))
+            else:
+                step = int(self.step)
+
+            # Eliminate the worst features
+            threshold = min(step, current_number_of_features - n_features_to_select)
+
+            support_[features[ranks][:threshold]] = False
+            ranking_[np.logical_not(support_)] += 1
+
             # Update cv scores
             for train_or_test, scores_per_fold in zip(
                 ["train", "test"], [train_scores_per_fold, test_scores_per_fold]
             ):
                 for i, score in enumerate(scores_per_fold):
                     self.cv_results_[f"split{i}_{train_or_test}_score"].append(score)
                 self.cv_results_[f"mean_{train_or_test}_score"].append(
                     np.mean(scores_per_fold)
                 )
                 self.cv_results_[f"std_{train_or_test}_score"].append(
                     np.std(scores_per_fold)
                 )
             self.cv_results_["n_features"].append(current_number_of_features)
 
-            # for sparse case ranks is matrix
-            ranks = np.ravel(ranks)
-
-            if 0.0 < self.step < 1.0:
-                step = int(max(1, self.step * current_number_of_features))
-            else:
-                step = int(self.step)
-
-            # Eliminate the worst features
-            threshold = min(step, current_number_of_features - n_features_to_select)
-
-            support_[features[ranks][:threshold]] = False
-            ranking_[np.logical_not(support_)] += 1
             current_number_of_features = np.sum(support_)
-
         # Set final attributes
 
         # Estimate performances of final model
         features = np.arange(n_features)[support_]
         X_remaining_features = X[:, features]
         cv_scores = cross_validate(
             self.estimator,
@@ -605,17 +604,15 @@
         - The least important features are pruned.
         - The pruned features are removed from the dataset.
     ```
 
     Parameters
     ----------
     estimator : ``Estimator`` instance
-        A supervised learning estimator with a ``fit`` method that provides
-        information about feature importance either through a ``coef_``
-        attribute or through a ``feature_importances_`` attribute.
+        A supervised learning estimator with a ``fit`` method.
     step : int or float, default=1
         If greater than or equal to 1, then ``step`` corresponds to the
         (integer) number of features to remove at each iteration.
         If within (0.0, 1.0), then ``step`` corresponds to the percentage
         (rounded down) of **remaining** features to remove at each iteration.
         Note that the last iteration may remove fewer than ``step`` features in
         order to reach ``min_features_to_select``.
@@ -744,15 +741,14 @@
         n_jobs=None,
         n_repeats=5,
         random_state=None,
         sample_weight=None,
         max_samples=1.0,
     ) -> None:
         self.n_repeats = n_repeats
-        self.random_state = random_state
         self.sample_weight = sample_weight
         self.max_samples = max_samples
         super().__init__(
             estimator,
             step=step,
             n_features_to_select=n_features_to_select,
             cv=cv,
```

### Comparing `felimination-0.1.2/pyproject.toml` & `felimination-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "felimination"
 description = "This library contains some useful scikit-learn compatible classes for feature selection."
-version = "0.1.2"
+version = "0.2.0"
 keywords = ["feature selection", "scikit-learn", "machine learning"]
 authors = [
     { name = "Claudio Salvatore Arcidiacono", email = "author@email.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `felimination-0.1.2/PKG-INFO` & `felimination-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felimination
-Version: 0.1.2
+Version: 0.2.0
 Summary: This library contains some useful scikit-learn compatible classes for feature selection.
 Keywords: feature selection,scikit-learn,machine learning
 Author-email: Claudio Salvatore Arcidiacono <author@email.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,20 +25,23 @@
 Project-URL: Bug Tracker, https://github.com/ClaudioSalvatoreArcidiacono/felimination/issues
 Project-URL: Documentation, https://claudiosalvatorearcidiacono.github.io/felimination/
 Project-URL: Homepage, https://github.com/ClaudioSalvatoreArcidiacono/felimination
 Provides-Extra: build
 Provides-Extra: dev
 Provides-Extra: doc
 
+[![pytest](https://github.com/ClaudioSalvatoreArcidiacono/felimination/workflows/Tests/badge.svg)](https://github.com/ClaudioSalvatoreArcidiacono/felimination/actions?query=workflow%3A%22Tests%22)
+[![PyPI](https://img.shields.io/pypi/v/felimination)](#)
+[![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://claudiosalvatorearcidiacono.github.io/felimination/)
+
+
 # felimination
 
 This library contains some useful scikit-learn compatible classes for feature selection.
 
-## [Check out documentation here](https://claudiosalvatorearcidiacono.github.io/felimination/)
-
 ## Features
 
 - [Recursive Feature Elimination with Cross Validation using Permutation Importance](reference/RFE.md#felimination.rfe.PermutationImportanceRFECV)
 
 ## Requirements
 
 - Python 3.7+
@@ -52,15 +55,14 @@
 ```
 pip install felimination
 ```
 
 ## Usage
 
 ```python
-
 from felimination.rfe import PermutationImportanceRFECV
 from sklearn.linear_model import LogisticRegression
 from sklearn.datasets import make_classification
 import numpy as np
 
 
 X, y = make_classification(
@@ -68,45 +70,37 @@
     n_features=20,
     n_informative=6,
     n_redundant=10,
     n_clusters_per_class=1,
     random_state=42,
 )
 
-# Add random features at the end, so the first 2 features are
-# relevant and the remaining 8 features are random
-X_with_rand = np.hstack((X, np.random.random(size=(X.shape[0], 8))))
-
 selector = PermutationImportanceRFECV(LogisticRegression(), step=0.3)
 
-selector.fit(X_with_rand, y)
+selector.fit(X, y)
 
 selector.support_
 # array([False, False, False, False, False, False, False, False, False,
-#        False, False, False, False, True, False, False, False, False,
-#        False, False, False, False, False, False, False, False, False,
-#        False])
+#        False, False,  True, False, False, False, False, False, False,
+#        False, False])
 
 selector.ranking_
-# array([10,  3,  9, 10,  8,  9,  7,  7, 10,  6,  8,  2,  8,  1,  9, 10, 10,
-#         4,  5,  6,  9, 10,  9,  8, 10,  9,  7, 10])
-
+# array([9, 3, 8, 9, 7, 8, 5, 6, 9, 6, 8, 1, 9, 7, 8, 9, 9, 2, 4, 7])
 selector.plot()
 ```
 ![example of plot](./docs/assets/example_plot.png)
 
-It looks like `3` is a good number of features, we can set the number of features to select to 3 without need of retraining
+It looks like `5` is a good number of features, we can set the number of features to select to 5 without need of retraining
 
 ```python
-selector.set_n_features_to_select(3)
+selector.set_n_features_to_select(5)
 selector.support_
-# array([False,  True, False, False, False, False, False, False, False,
-#        False, False,  True, False,  True, False, False, False, False,
-#        False, False, False, False, False, False, False, False, False,
-#        False])
+# array([False,  True, False, False, False, False,  True, False, False,
+#        False, False,  True, False, False, False, False, False,  True,
+#         True, False])
 ```
 
 ## License
 
 This project is licensed under the BSD 3-Clause License - see the LICENSE.md file for details
 
 ## Acknowledgments
```


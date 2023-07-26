# Comparing `tmp/jianglab-0.6.4.tar.gz` & `tmp/jianglab-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.6.4.tar", last modified: Wed Jul 26 14:46:14 2023, max compression
+gzip compressed data, was "jianglab-0.6.5.tar", last modified: Wed Jul 26 16:20:09 2023, max compression
```

## Comparing `jianglab-0.6.4.tar` & `jianglab-0.6.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-26 14:46:14.860654 jianglab-0.6.4/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-26 14:46:14.860158 jianglab-0.6.4/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.6.4/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-26 14:46:14.855816 jianglab-0.6.4/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.6.4/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    36595 2023-07-26 14:46:03.000000 jianglab-0.6.4/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.6.4/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-26 14:46:14.859307 jianglab-0.6.4/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-26 14:46:14.000000 jianglab-0.6.4/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-26 14:46:14.000000 jianglab-0.6.4/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-26 14:46:14.000000 jianglab-0.6.4/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      119 2023-07-26 14:46:14.000000 jianglab-0.6.4/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-26 14:46:14.000000 jianglab-0.6.4/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-26 14:46:14.860906 jianglab-0.6.4/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1058 2023-07-26 14:46:08.000000 jianglab-0.6.4/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-26 16:20:09.866637 jianglab-0.6.5/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-26 16:20:09.865988 jianglab-0.6.5/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.6.5/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-26 16:20:09.861953 jianglab-0.6.5/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.6.5/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    40704 2023-07-26 16:20:02.000000 jianglab-0.6.5/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.6.5/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-26 16:20:09.865126 jianglab-0.6.5/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-26 16:20:09.000000 jianglab-0.6.5/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-26 16:20:09.000000 jianglab-0.6.5/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-26 16:20:09.000000 jianglab-0.6.5/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      147 2023-07-26 16:20:09.000000 jianglab-0.6.5/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-26 16:20:09.000000 jianglab-0.6.5/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-26 16:20:09.867041 jianglab-0.6.5/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1119 2023-07-26 16:19:25.000000 jianglab-0.6.5/setup.py
```

### Comparing `jianglab-0.6.4/PKG-INFO` & `jianglab-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.6.4
+Version: 0.6.5
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.6.4/README.md` & `jianglab-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.6.4/jianglab/common_functions.py` & `jianglab-0.6.5/jianglab/common_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,29 @@
 import cv2
 import xmltodict
 import matplotlib.animation as animation
 from IPython.display import HTML
 import matplotlib
 from scipy.fftpack import fft, fftfreq
 import seaborn as sns
+import optuna
+import xgboost as xgb
+
+from sklearn.preprocessing import MinMaxScaler, StandardScaler, FunctionTransformer
+from sklearn.metrics import roc_auc_score
+from sklearn.inspection import permutation_importance
+from sklearn.linear_model import LogisticRegression
+from sklearn.inspection import permutation_importance
+from sklearn.ensemble import RandomForestClassifier, VotingClassifier
+from sklearn.model_selection import RepeatedStratifiedKFold, cross_val_score, GridSearchCV
+from sklearn.pipeline import Pipeline, make_pipeline
+from sklearn.compose import ColumnTransformer
+from sklearn.neighbors import KNeighborsClassifier
+
+import warnings
 
 
 
 
 
 def frame_ref_to_onset(frame_ref, first_onset_index = 184, visualize_window = (250_000,350_000), stimulus_interval = 60, on_duration = 30, sampling_rate = 20000,overlay_split_num = 5):
     '''
@@ -869,26 +884,117 @@
         filename_list.sort()
         index = filename_list.index(filename)
         filename_list = filename_list[index-neibour_before:index+neibour_after+1]
         if include_self == False:
             filename_list.remove(filename)
         return [os.path.join(file_dir, f) for f in filename_list]
     
-def plot_correlation_map(df, annot = True, format = ".3f", cmap = "coolwarm", upper_triangle = True):
-	corr = df.corr()
-	if upper_triangle:
-		mask = np.triu(corr)
-	else:
-		mask = None
-	ax, fig = plt.subplots(figsize = (10,5))
-	sns.heatmap(corr, mask = mask, annot = annot, fmt=format, cmap = cmap)
+# explore correlation of features
+def plot_correlation_map(df, annot = True, format = ".3f", cmap = "coolwarm", upper_triangle = True, x_rotation = 0, y_rotation = 0):
+    corr = df.corr()
+    if upper_triangle:
+        mask = np.triu(corr)
+    else:
+        mask = None
+    ax, fig = plt.subplots(figsize = (10,5))
+    sns.heatmap(corr, mask = mask, annot = annot, fmt=format, cmap = cmap)
+    plt.xticks(rotation = x_rotation)
+    plt.yticks(rotation = y_rotation)
+    plt.show()
+
         
 
 # plot kernel density estimation for each variable
-def kde_df(data, grid, figsize=(10,10)):
-    x, y = grid[0], grid[1]
-    fig, axes = plt.subplots(x, y, figsize = figsize)
-    for i, col in enumerate(data.columns):
-        ax = axes[i//y, i%y]
-        sns.kdeplot(data=data[col], ax=ax, fill=None)
-        ax.axvline(data[col].mean(), color='red')
-    fig.suptitle('Density function of each features',y = 0.9, fontsize=10)
+def kde_df(data, grid, figsize=(10,10), fontsize=10):
+	x, y = grid[0], grid[1]
+	fig, axes = plt.subplots(x, y, figsize = figsize)
+	for i, col in enumerate(data.columns):
+		ax = axes[i//y, i%y]
+		sns.kdeplot(data=data[col], ax=ax, fill=None)
+		ax.axvline(data[col].mean(), color='red')
+		fig.suptitle('Density function of each features',y = 0.9, fontsize=fontsize)
+    #plt.show()
+
+def plot_pairplot(data, hue = "target", figsize=(10,10), pallette = "viridis", size = 80):
+    sns.pairplot(data=data, hue =hue, corner=True, plot_kws={'s':size, 'edgecolor':"white", 'linewidth':2.5}, palette=pallette)
+    plt.figure(figsize=(10,10))
+    plt.show()
+
+def xgb_optuna(X, Y,params = {}, n_trials = 2, use_GPU = False):
+    """
+        params = {
+                'verbosity': 0,
+
+                'n_estimators': trial.suggest_int('n_estimators', 50, 1500),
+
+                'learning_rate': trial.suggest_float('learning_rate', 1e-7, 1e-1),
+
+                'max_depth': trial.suggest_int('max_depth', 3, 20),
+
+                'colsample_bytree': trial.suggest_float('colsample_bytree', 0.1, 1.0),
+
+                'alpha': trial.suggest_float('alpha', 1e-5, 1e2),
+
+                'lambda': trial.suggest_float('lambda', 1e-5, 1e2),
+
+                'objective': 'binary:logistic',
+
+                'eval_metric': 'auc',
+
+                'booster':trial.suggest_categorical("booster", ["dart", "gbtree",'gblinear']),
+
+                'min_child_weight': trial.suggest_int('min_child_weight', 0, 5),
+                
+            }
+    """
+
+    #Xgb modeling and optuna selection of hyperparameters
+    optuna.logging.set_verbosity(optuna.logging.WARNING)
+
+    def objective(trial):
+        nonlocal params
+        if params == {}:
+            params = {
+                'verbosity': 0,
+                'n_estimators': trial.suggest_int('n_estimators', 50, 1500),
+                'learning_rate': trial.suggest_float('learning_rate', 1e-7, 1e-1),
+                'max_depth': trial.suggest_int('max_depth', 3, 20),
+                'colsample_bytree': trial.suggest_float('colsample_bytree', 0.1, 1.0),
+                'alpha': trial.suggest_float('alpha', 1e-5, 1e2),
+                'lambda': trial.suggest_float('lambda', 1e-5, 1e2),
+                'objective': 'binary:logistic',
+                'eval_metric': 'auc',
+                'booster':trial.suggest_categorical("booster", ["dart", "gbtree",'gblinear']),
+                'min_child_weight': trial.suggest_int('min_child_weight', 0, 5),
+            }
+        if use_GPU:
+            params['tree_method'] = 'gpu_hist'
+        
+        # n_repeats = 2 bc 10 was too long
+        kf = RepeatedStratifiedKFold(n_splits=10, n_repeats=2, random_state=42)
+        scores = []
+        for train_idx, val_idx in kf.split(X, Y):
+            X_train, X_val = X.iloc[train_idx], X.iloc[val_idx]
+            y_train, y_val = Y.iloc[train_idx], Y.iloc[val_idx]
+            
+            d_train = xgb.DMatrix(X_train, label=y_train)
+            d_val = xgb.DMatrix(X_val, label=y_val)
+            
+            evallist = [(d_val, 'eval')]
+            
+            xgb_model = xgb.train(params, d_train, num_boost_round = 100,
+                            evals = evallist, 
+                            early_stopping_rounds=20, verbose_eval=False)
+
+            y_pred = xgb_model.predict(d_val)
+            score = roc_auc_score(y_val, y_pred)
+            scores.append(score)
+
+        return np.mean(scores)
+
+
+    study = optuna.create_study(direction='maximize')
+
+    #carraying out the optimization
+    study.optimize(objective, n_trials=n_trials)
+    #get the best parameters
+    return study.best_params
```

### Comparing `jianglab-0.6.4/jianglab.egg-info/PKG-INFO` & `jianglab-0.6.5/jianglab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.6.4
+Version: 0.6.5
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.6.4/setup.py` & `jianglab-0.6.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.6.4',
+    version='0.6.5',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
@@ -14,14 +14,17 @@
         "scipy",
         "gspread",
         "oauth2client",
         "xmltodict",
         "opencv-python",
         "ipython",
         "seaborn",
+        "optuna",
+        "xgboost",
+        "scikit-learn",
 
     ],
     author = "Jiang Zheng",
     author_email = "zjiang314@gmail.com",
     description = "A package for Jiang lab",
     url = "https://github.com/jiang-lab-retina/jianglab.git",
     classifiers=[
```


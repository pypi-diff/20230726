# Comparing `tmp/treesimulator-0.1.6.tar.gz` & `tmp/treesimulator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treesimulator-0.1.6.tar", last modified: Fri Jun  9 10:43:30 2023, max compression
+gzip compressed data, was "treesimulator-0.1.7.tar", last modified: Wed Jul 26 16:35:41 2023, max compression
```

## Comparing `treesimulator-0.1.6.tar` & `treesimulator-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-06-09 10:43:30.327995 treesimulator-0.1.6/
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    35823 2022-12-22 13:30:01.000000 treesimulator-0.1.6/LICENSE
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     6340 2023-06-09 10:43:30.327995 treesimulator-0.1.6/PKG-INFO
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     5793 2022-12-22 13:30:01.000000 treesimulator-0.1.6/README.md
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       38 2023-06-09 10:43:30.327995 treesimulator-0.1.6/setup.cfg
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1302 2023-06-09 10:42:39.000000 treesimulator-0.1.6/setup.py
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-06-09 10:43:30.327995 treesimulator-0.1.6/treesimulator/
--rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     1281 2023-05-23 12:45:26.000000 treesimulator-0.1.6/treesimulator/__init__.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    17829 2023-05-23 12:47:02.000000 treesimulator-0.1.6/treesimulator/generator.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    10186 2023-05-23 12:38:06.000000 treesimulator-0.1.6/treesimulator/mtbd_models.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4537 2022-12-22 13:30:02.000000 treesimulator-0.1.6/treesimulator/sequence_generator.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     5459 2023-06-09 10:42:39.000000 treesimulator-0.1.6/treesimulator/simulate_forest.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     3883 2022-12-22 13:30:02.000000 treesimulator-0.1.6/treesimulator/simulate_forest_bd.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4069 2022-12-22 13:30:02.000000 treesimulator-0.1.6/treesimulator/simulate_forest_bdei.py
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4582 2022-12-22 13:30:02.000000 treesimulator-0.1.6/treesimulator/simulate_forest_bdss.py
-drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-06-09 10:43:30.327995 treesimulator-0.1.6/treesimulator.egg-info/
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     6340 2023-06-09 10:43:30.000000 treesimulator-0.1.6/treesimulator.egg-info/PKG-INFO
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)      513 2023-06-09 10:43:30.000000 treesimulator-0.1.6/treesimulator.egg-info/SOURCES.txt
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        1 2023-06-09 10:43:30.000000 treesimulator-0.1.6/treesimulator.egg-info/dependency_links.txt
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)      233 2023-06-09 10:43:30.000000 treesimulator-0.1.6/treesimulator.egg-info/entry_points.txt
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)       15 2023-06-09 10:43:30.000000 treesimulator-0.1.6/treesimulator.egg-info/requires.txt
--rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)       14 2023-06-09 10:43:30.000000 treesimulator-0.1.6/treesimulator.egg-info/top_level.txt
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-07-26 16:35:41.921986 treesimulator-0.1.7/
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    35823 2022-12-22 13:30:01.000000 treesimulator-0.1.7/LICENSE
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     6340 2023-07-26 16:35:41.921986 treesimulator-0.1.7/PKG-INFO
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     5793 2022-12-22 13:30:01.000000 treesimulator-0.1.7/README.md
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       38 2023-07-26 16:35:41.921986 treesimulator-0.1.7/setup.cfg
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1302 2023-07-26 16:34:37.000000 treesimulator-0.1.7/setup.py
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-07-26 16:35:41.917986 treesimulator-0.1.7/treesimulator/
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     1281 2023-05-23 12:45:26.000000 treesimulator-0.1.7/treesimulator/__init__.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    17668 2023-07-26 11:53:02.000000 treesimulator-0.1.7/treesimulator/generator.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    10206 2023-07-17 12:49:05.000000 treesimulator-0.1.7/treesimulator/mtbd_models.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4537 2022-12-22 13:30:02.000000 treesimulator-0.1.7/treesimulator/sequence_generator.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     5459 2023-06-09 10:42:39.000000 treesimulator-0.1.7/treesimulator/simulate_forest.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     3883 2022-12-22 13:30:02.000000 treesimulator-0.1.7/treesimulator/simulate_forest_bd.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4069 2022-12-22 13:30:02.000000 treesimulator-0.1.7/treesimulator/simulate_forest_bdei.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4582 2022-12-22 13:30:02.000000 treesimulator-0.1.7/treesimulator/simulate_forest_bdss.py
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-07-26 16:35:41.921986 treesimulator-0.1.7/treesimulator.egg-info/
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     6340 2023-07-26 16:35:41.000000 treesimulator-0.1.7/treesimulator.egg-info/PKG-INFO
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)      513 2023-07-26 16:35:41.000000 treesimulator-0.1.7/treesimulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)        1 2023-07-26 16:35:41.000000 treesimulator-0.1.7/treesimulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)      233 2023-07-26 16:35:41.000000 treesimulator-0.1.7/treesimulator.egg-info/entry_points.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       15 2023-07-26 16:35:41.000000 treesimulator-0.1.7/treesimulator.egg-info/requires.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       14 2023-07-26 16:35:41.000000 treesimulator-0.1.7/treesimulator.egg-info/top_level.txt
```

### Comparing `treesimulator-0.1.6/LICENSE` & `treesimulator-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.6/PKG-INFO` & `treesimulator-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treesimulator
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simulation of rooted phylogenetic trees under a given Multitype Birth–Death model.
 Home-page: https://github.com/evolbioinfo/treesimulator
 Author: Anna Zhukova
 Author-email: anna.zhukova@pasteur.fr
 Keywords: phylogenetics,tree generator,multitype birth-death model
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `treesimulator-0.1.6/README.md` & `treesimulator-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.6/setup.py` & `treesimulator-0.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
-    version='0.1.6',
+    version='0.1.7',
     description='Simulation of rooted phylogenetic trees under a given Multitype Birth–Death model.',
     author='Anna Zhukova',
     author_email='anna.zhukova@pasteur.fr',
     url='https://github.com/evolbioinfo/treesimulator',
     keywords=['phylogenetics', 'tree generator', 'multitype birth-death model'],
     install_requires=['six', 'ete3', 'numpy'],
     entry_points={
```

### Comparing `treesimulator-0.1.6/treesimulator/__init__.py` & `treesimulator-0.1.7/treesimulator/__init__.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.6/treesimulator/generator.py` & `treesimulator-0.1.7/treesimulator/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     """
     num_states = len(model.states)
     if state_frequencies is None:
         state_frequencies = model.state_frequencies
     root_state = np.random.choice(np.arange(num_states), size=1, p=state_frequencies)[0]
     # evolve till the time is up, following Gillespie
     time = 0
-    infectious_nums = np.zeros(num_states, dtype=np.int)
+    infectious_nums = np.zeros(num_states, dtype=np.int64)
     infectious_nums[root_state] = 1
-    sampled_nums = np.zeros(num_states, dtype=np.int)
+    sampled_nums = np.zeros(num_states, dtype=np.int64)
 
     infectious_state2id = [set() for _ in model.states]
     cur_id = 0, 0
     infectious_state2id[root_state].add(cur_id)
     id2time = {}
     id2parent_id = {}
     sampled_id2state = {}
@@ -142,17 +142,15 @@
                 if np.random.uniform(0, 1, 1)[0] < model.ps[i]:
                     sampled_id2state[removed_id] = model.states[i]
                     sampled_nums[i] += 1
                     # print('\tand sampled')
 
                     # partner notification
                     # if it is not the root
-                    # and not a notified partner him/herself (num_states - 1 is the state of a notified partner)
                     if isinstance(model, PNModel) and np.random.uniform(0, 1, 1)[0] < model.pn \
-                            and i != (num_states - 1) \
                             and removed_id in id2parent_id:
                         parent_id = id2parent_id[removed_id]
                         donor_id = (parent_id[0], parent_id[1] + 1)
                         partner_id = donor_id2recipient_id[parent_id] if removed_id == donor_id else donor_id
                         partner_id = partner_id[0], id2current_id[partner_id[0]]
                         # If the partner is not yet removed, notify them
                         if partner_id not in id2time:
@@ -264,18 +262,18 @@
         time2num[time] = total
     return time2num
 
 
 def random_pop(elements):
     """
     Removes a random element from a list and returns it.
-    :param elements: list of elemetns
+    :param elements: list of elements
     :return: the selected element
     """
-    element = random.sample(elements, 1)[0]
+    element = random.sample(list(elements), 1)[0]
     elements.remove(element)
     return element
 
 
 def generate_forest(model, max_time=np.inf, min_tips=1000, max_sampled=np.inf, keep_nones=False, state_feature=STATE,
                     state_frequencies=None, ltt=False):
     total_n_tips = 0
```

### Comparing `treesimulator-0.1.6/treesimulator/mtbd_models.py` & `treesimulator-0.1.7/treesimulator/mtbd_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
     def __init__(self, states=None,
                  transition_rates=None, transmission_rates=None, removal_rates=None, ps=None, *args, **kwargs):
         super(Model, self).__init__()
         self.__states = np.array(states)
         num_states = len(self.states)
         self.__ps = np.array(ps) if ps is not None else np.ones(num_states, dtype=float)
         self.__transmission_rates = np.array(transmission_rates) if transmission_rates is not None \
-            else np.zeros(shape=(num_states, num_states), dtype=np.float)
+            else np.zeros(shape=(num_states, num_states), dtype=np.float64)
         self.__transition_rates = np.array(transition_rates) if transition_rates is not None \
-            else np.zeros(shape=(num_states, num_states), dtype=np.float)
+            else np.zeros(shape=(num_states, num_states), dtype=np.float64)
         self.__removal_rates = np.array(removal_rates) if removal_rates is not None \
-            else np.zeros(shape=num_states, dtype=np.float)
+            else np.zeros(shape=num_states, dtype=np.float64)
         self.check_rates()
 
     def clone(self):
         return Model(self.states, self.transition_rates, self.transmission_rates, self.removal_rates, self.ps)
 
     @property
     def ps(self):
@@ -126,19 +126,19 @@
     def __init__(self, mu, la, psi, p=0.5, *args, **kwargs):
         """
         :param mu: transition E->I
         :param la: transmission from I to E
         :param psi: removal of I
         :param p: sampling probability of I
         """
-        mus = np.zeros(shape=(2, 2), dtype=np.float)
+        mus = np.zeros(shape=(2, 2), dtype=np.float64)
         mus[0, 1] = mu
-        las = np.zeros(shape=(2, 2), dtype=np.float)
+        las = np.zeros(shape=(2, 2), dtype=np.float64)
         las[1, 0] = la
-        psis = np.zeros(shape=2, dtype=np.float)
+        psis = np.zeros(shape=2, dtype=np.float64)
         psis[1] = psi
 
         Model.__init__(self, states=[EXPOSED, INFECTED],
                        transition_rates=mus, transmission_rates=las, removal_rates=psis, ps=[0, p],
                        *args, **kwargs)
 
     @property
@@ -170,15 +170,15 @@
 
     def __init__(self, la, psi, p=0.5, *args, **kwargs):
         """
         :param la: transmission
         :param psi: removal
         :param p: sampling probability
         """
-        las = la * np.ones(shape=(1, 1), dtype=np.float)
+        las = la * np.ones(shape=(1, 1), dtype=np.float64)
         Model.__init__(self, states=[INFECTED], transmission_rates=las, removal_rates=[psi], ps=[p], *args, **kwargs)
 
     def get_name(self):
         return 'BD'
 
     def get_epidemiological_parameters(self):
         """Converts rate parameters to the epidemiological ones"""
@@ -194,26 +194,26 @@
         :param la_nn: transmission from I to I
         :param la_ns: transmission from I to S
         :param la_sn: transmission from S to I
         :param la_ss: transmission from S to S
         :param psi: removal
         :param p: sampling
         """
-        las = np.zeros(shape=(2, 2), dtype=np.float)
+        las = np.zeros(shape=(2, 2), dtype=np.float64)
         s_ratio = la_ss / la_ns
         n_ratio = la_sn / la_nn
         if np.abs(s_ratio - n_ratio) > 1e-3:
             raise ValueError(
                 'transmission ratio constraint is violated: la_ss / la_ns ({}) must be equal to la_sn / la_nn ({})'
                     .format(s_ratio, n_ratio))
         las[0, 0] = la_nn
         las[0, 1] = la_ns
         las[1, 0] = la_sn
         las[1, 1] = la_ss
-        psis = psi * np.ones(shape=2, dtype=np.float)
+        psis = psi * np.ones(shape=2, dtype=np.float64)
         Model.__init__(self, states=[INFECTED, SUPERSPREADER],
                        transmission_rates=las, removal_rates=psis, ps=[p, p], *args, **kwargs)
 
     @property
     def state_frequencies(self):
         la_ss = self.transmission_rates[1, 1]
         la_sn = self.transmission_rates[1, 0]
@@ -257,15 +257,15 @@
 
     @property
     def partner_removal_rate(self):
         """
         Get partner removal rate
 
         :return partner removal rate
-        :rtype np.float
+        :rtype np.float64
         """
         return self.removal_rates[-1]
 
     def get_name(self):
         return self.model.get_name() + '-PN'
 
     def check_p(self):
```

### Comparing `treesimulator-0.1.6/treesimulator/sequence_generator.py` & `treesimulator-0.1.7/treesimulator/sequence_generator.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.6/treesimulator/simulate_forest.py` & `treesimulator-0.1.7/treesimulator/simulate_forest.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.6/treesimulator/simulate_forest_bd.py` & `treesimulator-0.1.7/treesimulator/simulate_forest_bd.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.6/treesimulator/simulate_forest_bdei.py` & `treesimulator-0.1.7/treesimulator/simulate_forest_bdei.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.6/treesimulator/simulate_forest_bdss.py` & `treesimulator-0.1.7/treesimulator/simulate_forest_bdss.py`

 * *Files identical despite different names*

### Comparing `treesimulator-0.1.6/treesimulator.egg-info/PKG-INFO` & `treesimulator-0.1.7/treesimulator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treesimulator
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simulation of rooted phylogenetic trees under a given Multitype Birth–Death model.
 Home-page: https://github.com/evolbioinfo/treesimulator
 Author: Anna Zhukova
 Author-email: anna.zhukova@pasteur.fr
 Keywords: phylogenetics,tree generator,multitype birth-death model
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `treesimulator-0.1.6/treesimulator.egg-info/SOURCES.txt` & `treesimulator-0.1.7/treesimulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*


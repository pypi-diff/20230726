# Comparing `tmp/circadian-0.0.4.tar.gz` & `tmp/circadian-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circadian-0.0.4.tar", last modified: Tue Feb 14 01:41:22 2023, max compression
+gzip compressed data, was "circadian-1.0.0.tar", last modified: Wed Jul 26 14:13:40 2023, max compression
```

## Comparing `circadian-0.0.4.tar` & `circadian-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 khannay    (501) staff       (20)        0 2023-02-14 01:41:22.804976 circadian-0.0.4/
--rw-rw-r--   0 khannay    (501) staff       (20)    11337 2022-09-05 16:31:43.000000 circadian-0.0.4/LICENSE
--rw-rw-r--   0 khannay    (501) staff       (20)      111 2022-09-05 16:31:43.000000 circadian-0.0.4/MANIFEST.in
--rw-r--r--   0 khannay    (501) staff       (20)     3341 2023-02-14 01:41:22.804834 circadian-0.0.4/PKG-INFO
--rw-r--r--   0 khannay    (501) staff       (20)     2501 2023-02-14 01:35:27.000000 circadian-0.0.4/README.md
-drwxr-xr-x   0 khannay    (501) staff       (20)        0 2023-02-14 01:41:22.803552 circadian-0.0.4/circadian/
--rw-r--r--   0 khannay    (501) staff       (20)       22 2023-02-14 01:41:19.000000 circadian-0.0.4/circadian/__init__.py
--rw-r--r--   0 khannay    (501) staff       (20)    38989 2023-02-14 01:41:19.000000 circadian-0.0.4/circadian/_modidx.py
--rw-r--r--   0 khannay    (501) staff       (20)    14429 2023-02-14 01:41:19.000000 circadian-0.0.4/circadian/cli.py
--rw-r--r--   0 khannay    (501) staff       (20)     7470 2023-02-14 01:41:19.000000 circadian-0.0.4/circadian/lights.py
--rw-r--r--   0 khannay    (501) staff       (20)     2171 2023-02-14 01:41:19.000000 circadian-0.0.4/circadian/metrics.py
--rw-r--r--   0 khannay    (501) staff       (20)    31272 2023-02-14 01:41:19.000000 circadian-0.0.4/circadian/models.py
--rw-r--r--   0 khannay    (501) staff       (20)     1379 2023-02-14 01:41:19.000000 circadian-0.0.4/circadian/phasetools.py
--rw-r--r--   0 khannay    (501) staff       (20)    18144 2023-02-14 01:41:19.000000 circadian-0.0.4/circadian/plots.py
--rw-r--r--   0 khannay    (501) staff       (20)     9452 2023-02-14 01:41:19.000000 circadian-0.0.4/circadian/prc.py
--rw-r--r--   0 khannay    (501) staff       (20)    25529 2023-02-14 01:41:19.000000 circadian-0.0.4/circadian/readers.py
--rw-r--r--   0 khannay    (501) staff       (20)     6677 2023-02-14 01:41:19.000000 circadian-0.0.4/circadian/sleep.py
--rw-r--r--   0 khannay    (501) staff       (20)    10160 2023-02-14 01:41:19.000000 circadian-0.0.4/circadian/utils.py
-drwxr-xr-x   0 khannay    (501) staff       (20)        0 2023-02-14 01:41:22.804627 circadian-0.0.4/circadian.egg-info/
--rw-r--r--   0 khannay    (501) staff       (20)     3341 2023-02-14 01:41:22.000000 circadian-0.0.4/circadian.egg-info/PKG-INFO
--rw-r--r--   0 khannay    (501) staff       (20)      523 2023-02-14 01:41:22.000000 circadian-0.0.4/circadian.egg-info/SOURCES.txt
--rw-r--r--   0 khannay    (501) staff       (20)        1 2023-02-14 01:41:22.000000 circadian-0.0.4/circadian.egg-info/dependency_links.txt
--rw-r--r--   0 khannay    (501) staff       (20)      122 2023-02-14 01:41:22.000000 circadian-0.0.4/circadian.egg-info/entry_points.txt
--rw-r--r--   0 khannay    (501) staff       (20)        1 2023-01-26 01:47:02.000000 circadian-0.0.4/circadian.egg-info/not-zip-safe
--rw-r--r--   0 khannay    (501) staff       (20)       74 2023-02-14 01:41:22.000000 circadian-0.0.4/circadian.egg-info/requires.txt
--rw-r--r--   0 khannay    (501) staff       (20)       10 2023-02-14 01:41:22.000000 circadian-0.0.4/circadian.egg-info/top_level.txt
--rw-r--r--   0 khannay    (501) staff       (20)      998 2023-02-14 01:41:19.000000 circadian-0.0.4/settings.ini
--rw-r--r--   0 khannay    (501) staff       (20)       38 2023-02-14 01:41:22.805022 circadian-0.0.4/setup.cfg
--rw-r--r--   0 khannay    (501) staff       (20)     2641 2023-01-31 03:01:08.000000 circadian-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:13:40.611133 circadian-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-26 14:13:28.000000 circadian-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-26 14:13:28.000000 circadian-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-07-26 14:13:40.611133 circadian-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-26 14:13:28.000000 circadian-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:13:40.611133 circadian-1.0.0/circadian/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37330 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23484 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/lights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42836 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/phasetools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18139 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/prc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25459 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-07-26 14:13:28.000000 circadian-1.0.0/circadian/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:13:40.611133 circadian-1.0.0/circadian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-07-26 14:13:40.000000 circadian-1.0.0/circadian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-26 14:13:40.000000 circadian-1.0.0/circadian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:13:40.000000 circadian-1.0.0/circadian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-26 14:13:40.000000 circadian-1.0.0/circadian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:13:40.000000 circadian-1.0.0/circadian.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 14:13:40.000000 circadian-1.0.0/circadian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 14:13:40.000000 circadian-1.0.0/circadian.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-26 14:13:28.000000 circadian-1.0.0/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:13:40.611133 circadian-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-26 14:13:28.000000 circadian-1.0.0/setup.py
```

### Comparing `circadian-0.0.4/circadian/_modidx.py` & `circadian-1.0.0/circadian/_modidx.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,322 +1,310 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/circadian',
-                'doc_host': 'https://khannay.github.io',
-                'git_url': 'https://github.com/khannay/circadian',
+                'doc_host': 'https://arcascope.github.io/circadian/',
+                'git_url': 'https://github.com/Arcascope/circadian',
                 'lib_path': 'circadian'},
-  'syms': { 'circadian.cli': { 'circadian.cli.main_acto': ('cli.html#main_acto', 'circadian/cli.py'),
-                               'circadian.cli.main_esri': ('cli.html#main_esri', 'circadian/cli.py')},
-            'circadian.lights': { 'circadian.lights.Light': ('lights.html#light', 'circadian/lights.py'),
-                                  'circadian.lights.Light.RegularLight': ('lights.html#light.regularlight', 'circadian/lights.py'),
-                                  'circadian.lights.Light.ShiftWorkLight': ('lights.html#light.shiftworklight', 'circadian/lights.py'),
-                                  'circadian.lights.Light.SlamShift': ('lights.html#light.slamshift', 'circadian/lights.py'),
-                                  'circadian.lights.Light.SocialJetlag': ('lights.html#light.socialjetlag', 'circadian/lights.py'),
-                                  'circadian.lights.Light.__add__': ('lights.html#light.__add__', 'circadian/lights.py'),
-                                  'circadian.lights.Light.__call__': ('lights.html#light.__call__', 'circadian/lights.py'),
-                                  'circadian.lights.Light.__init__': ('lights.html#light.__init__', 'circadian/lights.py'),
-                                  'circadian.lights.Light.end_time': ('lights.html#light.end_time', 'circadian/lights.py'),
-                                  'circadian.lights.Light.plot': ('lights.html#light.plot', 'circadian/lights.py'),
-                                  'circadian.lights.get_pulse': ('lights.html#get_pulse', 'circadian/lights.py'),
-                                  'circadian.lights.make_pulse': ('lights.html#make_pulse', 'circadian/lights.py')},
-            'circadian.metrics': { 'circadian.metrics.esri': ('metrics.html#esri', 'circadian/metrics.py'),
-                                   'circadian.metrics.esri_trajectory': ('metrics.html#esri_trajectory', 'circadian/metrics.py')},
-            'circadian.models': { 'circadian.models.CircadianModel': ('models.html#circadianmodel', 'circadian/models.py'),
-                                  'circadian.models.CircadianModel.__call__': ( 'models.html#circadianmodel.__call__',
+  'syms': { 'circadian.cli': { 'circadian.cli.main_acto': ('api/cli.html#main_acto', 'circadian/cli.py'),
+                               'circadian.cli.main_esri': ('api/cli.html#main_esri', 'circadian/cli.py')},
+            'circadian.lights': { 'circadian.lights.LightSchedule': ('api/lights.html#lightschedule', 'circadian/lights.py'),
+                                  'circadian.lights.LightSchedule.Regular': ( 'api/lights.html#lightschedule.regular',
+                                                                              'circadian/lights.py'),
+                                  'circadian.lights.LightSchedule.ShiftWork': ( 'api/lights.html#lightschedule.shiftwork',
+                                                                                'circadian/lights.py'),
+                                  'circadian.lights.LightSchedule.SlamShift': ( 'api/lights.html#lightschedule.slamshift',
+                                                                                'circadian/lights.py'),
+                                  'circadian.lights.LightSchedule.SocialJetlag': ( 'api/lights.html#lightschedule.socialjetlag',
+                                                                                   'circadian/lights.py'),
+                                  'circadian.lights.LightSchedule.__add__': ( 'api/lights.html#lightschedule.__add__',
+                                                                              'circadian/lights.py'),
+                                  'circadian.lights.LightSchedule.__call__': ( 'api/lights.html#lightschedule.__call__',
+                                                                               'circadian/lights.py'),
+                                  'circadian.lights.LightSchedule.__init__': ( 'api/lights.html#lightschedule.__init__',
+                                                                               'circadian/lights.py'),
+                                  'circadian.lights.LightSchedule.__sub__': ( 'api/lights.html#lightschedule.__sub__',
+                                                                              'circadian/lights.py'),
+                                  'circadian.lights.LightSchedule.concatenate_at': ( 'api/lights.html#lightschedule.concatenate_at',
+                                                                                     'circadian/lights.py'),
+                                  'circadian.lights.LightSchedule.from_pulse': ( 'api/lights.html#lightschedule.from_pulse',
+                                                                                 'circadian/lights.py'),
+                                  'circadian.lights.LightSchedule.plot': ('api/lights.html#lightschedule.plot', 'circadian/lights.py')},
+            'circadian.metrics': { 'circadian.metrics.esri': ('api/metrics.html#esri', 'circadian/metrics.py'),
+                                   'circadian.metrics.esri_trajectory': ('api/metrics.html#esri_trajectory', 'circadian/metrics.py')},
+            'circadian.models': { 'circadian.models.CircadianModel': ('api/models.html#circadianmodel', 'circadian/models.py'),
+                                  'circadian.models.CircadianModel.__call__': ( 'api/models.html#circadianmodel.__call__',
                                                                                 'circadian/models.py'),
-                                  'circadian.models.CircadianModel.__init__': ( 'models.html#circadianmodel.__init__',
+                                  'circadian.models.CircadianModel.__init__': ( 'api/models.html#circadianmodel.__init__',
                                                                                 'circadian/models.py'),
-                                  'circadian.models.CircadianModel._default_params': ( 'models.html#circadianmodel._default_params',
-                                                                                       'circadian/models.py'),
-                                  'circadian.models.CircadianModel.amplitude': ( 'models.html#circadianmodel.amplitude',
-                                                                                 'circadian/models.py'),
-                                  'circadian.models.CircadianModel.cbt': ('models.html#circadianmodel.cbt', 'circadian/models.py'),
-                                  'circadian.models.CircadianModel.default_initial_conditions': ( 'models.html#circadianmodel.default_initial_conditions',
+                                  'circadian.models.CircadianModel._default_initial_condition': ( 'api/models.html#circadianmodel._default_initial_condition',
                                                                                                   'circadian/models.py'),
-                                  'circadian.models.CircadianModel.dlmos': ('models.html#circadianmodel.dlmos', 'circadian/models.py'),
-                                  'circadian.models.CircadianModel.get_parameters': ( 'models.html#circadianmodel.get_parameters',
-                                                                                      'circadian/models.py'),
-                                  'circadian.models.CircadianModel.initial_conditions_loop': ( 'models.html#circadianmodel.initial_conditions_loop',
-                                                                                               'circadian/models.py'),
-                                  'circadian.models.CircadianModel.integrate_model': ( 'models.html#circadianmodel.integrate_model',
+                                  'circadian.models.CircadianModel._default_params': ( 'api/models.html#circadianmodel._default_params',
                                                                                        'circadian/models.py'),
-                                  'circadian.models.CircadianModel.observer': ( 'models.html#circadianmodel.observer',
-                                                                                'circadian/models.py'),
-                                  'circadian.models.CircadianModel.phase': ('models.html#circadianmodel.phase', 'circadian/models.py'),
-                                  'circadian.models.CircadianModel.set_parameters': ( 'models.html#circadianmodel.set_parameters',
-                                                                                      'circadian/models.py'),
-                                  'circadian.models.CircadianModel.step_rk4': ( 'models.html#circadianmodel.step_rk4',
-                                                                                'circadian/models.py'),
-                                  'circadian.models.DynamicalTrajectory': ('models.html#dynamicaltrajectory', 'circadian/models.py'),
-                                  'circadian.models.DynamicalTrajectory.__call__': ( 'models.html#dynamicaltrajectory.__call__',
-                                                                                     'circadian/models.py'),
-                                  'circadian.models.DynamicalTrajectory.__getitem__': ( 'models.html#dynamicaltrajectory.__getitem__',
-                                                                                        'circadian/models.py'),
-                                  'circadian.models.DynamicalTrajectory.__init__': ( 'models.html#dynamicaltrajectory.__init__',
-                                                                                     'circadian/models.py'),
-                                  'circadian.models.DynamicalTrajectory.__len__': ( 'models.html#dynamicaltrajectory.__len__',
-                                                                                    'circadian/models.py'),
-                                  'circadian.models.DynamicalTrajectory.batch_size': ( 'models.html#dynamicaltrajectory.batch_size',
-                                                                                       'circadian/models.py'),
-                                  'circadian.models.DynamicalTrajectory.get_batch': ( 'models.html#dynamicaltrajectory.get_batch',
-                                                                                      'circadian/models.py'),
-                                  'circadian.models.Forger99Model': ('models.html#forger99model', 'circadian/models.py'),
-                                  'circadian.models.Forger99Model.__init__': ('models.html#forger99model.__init__', 'circadian/models.py'),
-                                  'circadian.models.Forger99Model.__repr__': ('models.html#forger99model.__repr__', 'circadian/models.py'),
-                                  'circadian.models.Forger99Model.__str__': ('models.html#forger99model.__str__', 'circadian/models.py'),
-                                  'circadian.models.Forger99Model._default_params': ( 'models.html#forger99model._default_params',
-                                                                                      'circadian/models.py'),
-                                  'circadian.models.Forger99Model.alpha0': ('models.html#forger99model.alpha0', 'circadian/models.py'),
-                                  'circadian.models.Forger99Model.amplitude': ( 'models.html#forger99model.amplitude',
-                                                                                'circadian/models.py'),
-                                  'circadian.models.Forger99Model.cbt': ('models.html#forger99model.cbt', 'circadian/models.py'),
-                                  'circadian.models.Forger99Model.default_initial_conditions': ( 'models.html#forger99model.default_initial_conditions',
-                                                                                                 'circadian/models.py'),
-                                  'circadian.models.Forger99Model.derv': ('models.html#forger99model.derv', 'circadian/models.py'),
-                                  'circadian.models.Forger99Model.dlmos': ('models.html#forger99model.dlmos', 'circadian/models.py'),
-                                  'circadian.models.Forger99Model.get_parameters': ( 'models.html#forger99model.get_parameters',
-                                                                                     'circadian/models.py'),
-                                  'circadian.models.Forger99Model.get_parameters_array': ( 'models.html#forger99model.get_parameters_array',
-                                                                                           'circadian/models.py'),
-                                  'circadian.models.Forger99Model.phase': ('models.html#forger99model.phase', 'circadian/models.py'),
-                                  'circadian.models.Forger99Model.set_parameters': ( 'models.html#forger99model.set_parameters',
-                                                                                     'circadian/models.py'),
-                                  'circadian.models.Hannay19': ('models.html#hannay19', 'circadian/models.py'),
-                                  'circadian.models.Hannay19.CBTObs': ('models.html#hannay19.cbtobs', 'circadian/models.py'),
-                                  'circadian.models.Hannay19.DLMOObs': ('models.html#hannay19.dlmoobs', 'circadian/models.py'),
-                                  'circadian.models.Hannay19.__init__': ('models.html#hannay19.__init__', 'circadian/models.py'),
-                                  'circadian.models.Hannay19._default_params': ( 'models.html#hannay19._default_params',
+                                  'circadian.models.CircadianModel._num_inputs': ( 'api/models.html#circadianmodel._num_inputs',
+                                                                                   'circadian/models.py'),
+                                  'circadian.models.CircadianModel._num_states': ( 'api/models.html#circadianmodel._num_states',
+                                                                                   'circadian/models.py'),
+                                  'circadian.models.CircadianModel.amplitude': ( 'api/models.html#circadianmodel.amplitude',
                                                                                  'circadian/models.py'),
-                                  'circadian.models.Hannay19.alpha0': ('models.html#hannay19.alpha0', 'circadian/models.py'),
-                                  'circadian.models.Hannay19.amplitude': ('models.html#hannay19.amplitude', 'circadian/models.py'),
-                                  'circadian.models.Hannay19.cbt': ('models.html#hannay19.cbt', 'circadian/models.py'),
-                                  'circadian.models.Hannay19.default_initial_conditions': ( 'models.html#hannay19.default_initial_conditions',
+                                  'circadian.models.CircadianModel.cbt': ('api/models.html#circadianmodel.cbt', 'circadian/models.py'),
+                                  'circadian.models.CircadianModel.derv': ('api/models.html#circadianmodel.derv', 'circadian/models.py'),
+                                  'circadian.models.CircadianModel.dlmos': ('api/models.html#circadianmodel.dlmos', 'circadian/models.py'),
+                                  'circadian.models.CircadianModel.equilibrate': ( 'api/models.html#circadianmodel.equilibrate',
+                                                                                   'circadian/models.py'),
+                                  'circadian.models.CircadianModel.get_parameters_array': ( 'api/models.html#circadianmodel.get_parameters_array',
                                                                                             'circadian/models.py'),
-                                  'circadian.models.Hannay19.derv': ('models.html#hannay19.derv', 'circadian/models.py'),
-                                  'circadian.models.Hannay19.dlmos': ('models.html#hannay19.dlmos', 'circadian/models.py'),
-                                  'circadian.models.Hannay19.get_parameters': ( 'models.html#hannay19.get_parameters',
-                                                                                'circadian/models.py'),
-                                  'circadian.models.Hannay19.get_parameters_array': ( 'models.html#hannay19.get_parameters_array',
-                                                                                      'circadian/models.py'),
-                                  'circadian.models.Hannay19.guess_ic': ('models.html#hannay19.guess_ic', 'circadian/models.py'),
-                                  'circadian.models.Hannay19.integrate_observer': ( 'models.html#hannay19.integrate_observer',
-                                                                                    'circadian/models.py'),
-                                  'circadian.models.Hannay19.observer': ('models.html#hannay19.observer', 'circadian/models.py'),
-                                  'circadian.models.Hannay19.phase': ('models.html#hannay19.phase', 'circadian/models.py'),
-                                  'circadian.models.Hannay19.set_parameters': ( 'models.html#hannay19.set_parameters',
+                                  'circadian.models.CircadianModel.initial_condition': ( 'api/models.html#circadianmodel.initial_condition',
+                                                                                         'circadian/models.py'),
+                                  'circadian.models.CircadianModel.integrate': ( 'api/models.html#circadianmodel.integrate',
+                                                                                 'circadian/models.py'),
+                                  'circadian.models.CircadianModel.parameters': ( 'api/models.html#circadianmodel.parameters',
+                                                                                  'circadian/models.py'),
+                                  'circadian.models.CircadianModel.phase': ('api/models.html#circadianmodel.phase', 'circadian/models.py'),
+                                  'circadian.models.CircadianModel.step_rk4': ( 'api/models.html#circadianmodel.step_rk4',
                                                                                 'circadian/models.py'),
-                                  'circadian.models.Hannay19TP': ('models.html#hannay19tp', 'circadian/models.py'),
-                                  'circadian.models.Hannay19TP.CBTObs': ('models.html#hannay19tp.cbtobs', 'circadian/models.py'),
-                                  'circadian.models.Hannay19TP.DLMOObs': ('models.html#hannay19tp.dlmoobs', 'circadian/models.py'),
-                                  'circadian.models.Hannay19TP.__init__': ('models.html#hannay19tp.__init__', 'circadian/models.py'),
-                                  'circadian.models.Hannay19TP._default_params': ( 'models.html#hannay19tp._default_params',
-                                                                                   'circadian/models.py'),
-                                  'circadian.models.Hannay19TP.alpha0': ('models.html#hannay19tp.alpha0', 'circadian/models.py'),
-                                  'circadian.models.Hannay19TP.amplitude': ('models.html#hannay19tp.amplitude', 'circadian/models.py'),
-                                  'circadian.models.Hannay19TP.cbt': ('models.html#hannay19tp.cbt', 'circadian/models.py'),
-                                  'circadian.models.Hannay19TP.default_initial_conditions': ( 'models.html#hannay19tp.default_initial_conditions',
-                                                                                              'circadian/models.py'),
-                                  'circadian.models.Hannay19TP.derv': ('models.html#hannay19tp.derv', 'circadian/models.py'),
-                                  'circadian.models.Hannay19TP.dlmos': ('models.html#hannay19tp.dlmos', 'circadian/models.py'),
-                                  'circadian.models.Hannay19TP.get_parameters': ( 'models.html#hannay19tp.get_parameters',
+                                  'circadian.models.CircadianModel.trajectory': ( 'api/models.html#circadianmodel.trajectory',
                                                                                   'circadian/models.py'),
-                                  'circadian.models.Hannay19TP.get_parameters_array': ( 'models.html#hannay19tp.get_parameters_array',
+                                  'circadian.models.DynamicalTrajectory': ('api/models.html#dynamicaltrajectory', 'circadian/models.py'),
+                                  'circadian.models.DynamicalTrajectory.__call__': ( 'api/models.html#dynamicaltrajectory.__call__',
+                                                                                     'circadian/models.py'),
+                                  'circadian.models.DynamicalTrajectory.__getitem__': ( 'api/models.html#dynamicaltrajectory.__getitem__',
                                                                                         'circadian/models.py'),
-                                  'circadian.models.Hannay19TP.observer': ('models.html#hannay19tp.observer', 'circadian/models.py'),
-                                  'circadian.models.Hannay19TP.phase': ('models.html#hannay19tp.phase', 'circadian/models.py'),
-                                  'circadian.models.Hannay19TP.phase_difference': ( 'models.html#hannay19tp.phase_difference',
-                                                                                    'circadian/models.py'),
-                                  'circadian.models.Hannay19TP.set_parameters': ( 'models.html#hannay19tp.set_parameters',
-                                                                                  'circadian/models.py'),
-                                  'circadian.models.Hilaire2007': ('models.html#hilaire2007', 'circadian/models.py'),
-                                  'circadian.models.Hilaire2007.__init__': ('models.html#hilaire2007.__init__', 'circadian/models.py'),
-                                  'circadian.models.Hilaire2007.__repr__': ('models.html#hilaire2007.__repr__', 'circadian/models.py'),
-                                  'circadian.models.Hilaire2007.__str__': ('models.html#hilaire2007.__str__', 'circadian/models.py'),
-                                  'circadian.models.Hilaire2007._default_params': ( 'models.html#hilaire2007._default_params',
+                                  'circadian.models.DynamicalTrajectory.__init__': ( 'api/models.html#dynamicaltrajectory.__init__',
+                                                                                     'circadian/models.py'),
+                                  'circadian.models.DynamicalTrajectory.__len__': ( 'api/models.html#dynamicaltrajectory.__len__',
                                                                                     'circadian/models.py'),
-                                  'circadian.models.Hilaire2007.alphaNonPhotic': ( 'models.html#hilaire2007.alphanonphotic',
-                                                                                   'circadian/models.py'),
-                                  'circadian.models.Hilaire2007.amplitude': ('models.html#hilaire2007.amplitude', 'circadian/models.py'),
-                                  'circadian.models.Hilaire2007.cbt': ('models.html#hilaire2007.cbt', 'circadian/models.py'),
-                                  'circadian.models.Hilaire2007.default_initial_conditions': ( 'models.html#hilaire2007.default_initial_conditions',
-                                                                                               'circadian/models.py'),
-                                  'circadian.models.Hilaire2007.derv': ('models.html#hilaire2007.derv', 'circadian/models.py'),
-                                  'circadian.models.Hilaire2007.dlmos': ('models.html#hilaire2007.dlmos', 'circadian/models.py'),
-                                  'circadian.models.Hilaire2007.integrate_model': ( 'models.html#hilaire2007.integrate_model',
+                                  'circadian.models.DynamicalTrajectory.__str__': ( 'api/models.html#dynamicaltrajectory.__str__',
                                                                                     'circadian/models.py'),
-                                  'circadian.models.Hilaire2007.phase': ('models.html#hilaire2007.phase', 'circadian/models.py'),
-                                  'circadian.models.Hilaire2007.step_rk4': ('models.html#hilaire2007.step_rk4', 'circadian/models.py'),
-                                  'circadian.models.KronauerJewett': ('models.html#kronauerjewett', 'circadian/models.py'),
-                                  'circadian.models.KronauerJewett.__init__': ( 'models.html#kronauerjewett.__init__',
-                                                                                'circadian/models.py'),
-                                  'circadian.models.KronauerJewett.__repr__': ( 'models.html#kronauerjewett.__repr__',
-                                                                                'circadian/models.py'),
-                                  'circadian.models.KronauerJewett.__str__': ('models.html#kronauerjewett.__str__', 'circadian/models.py'),
-                                  'circadian.models.KronauerJewett._default_params': ( 'models.html#kronauerjewett._default_params',
+                                  'circadian.models.DynamicalTrajectory.get_batch': ( 'api/models.html#dynamicaltrajectory.get_batch',
+                                                                                      'circadian/models.py'),
+                                  'circadian.models.Forger99': ('api/models.html#forger99', 'circadian/models.py'),
+                                  'circadian.models.Forger99.__init__': ('api/models.html#forger99.__init__', 'circadian/models.py'),
+                                  'circadian.models.Forger99.__repr__': ('api/models.html#forger99.__repr__', 'circadian/models.py'),
+                                  'circadian.models.Forger99.__str__': ('api/models.html#forger99.__str__', 'circadian/models.py'),
+                                  'circadian.models.Forger99.amplitude': ('api/models.html#forger99.amplitude', 'circadian/models.py'),
+                                  'circadian.models.Forger99.cbt': ('api/models.html#forger99.cbt', 'circadian/models.py'),
+                                  'circadian.models.Forger99.derv': ('api/models.html#forger99.derv', 'circadian/models.py'),
+                                  'circadian.models.Forger99.dlmos': ('api/models.html#forger99.dlmos', 'circadian/models.py'),
+                                  'circadian.models.Forger99.integrate': ('api/models.html#forger99.integrate', 'circadian/models.py'),
+                                  'circadian.models.Forger99.phase': ('api/models.html#forger99.phase', 'circadian/models.py'),
+                                  'circadian.models.Hannay19': ('api/models.html#hannay19', 'circadian/models.py'),
+                                  'circadian.models.Hannay19.__init__': ('api/models.html#hannay19.__init__', 'circadian/models.py'),
+                                  'circadian.models.Hannay19.__repr__': ('api/models.html#hannay19.__repr__', 'circadian/models.py'),
+                                  'circadian.models.Hannay19.__str__': ('api/models.html#hannay19.__str__', 'circadian/models.py'),
+                                  'circadian.models.Hannay19.amplitude': ('api/models.html#hannay19.amplitude', 'circadian/models.py'),
+                                  'circadian.models.Hannay19.cbt': ('api/models.html#hannay19.cbt', 'circadian/models.py'),
+                                  'circadian.models.Hannay19.derv': ('api/models.html#hannay19.derv', 'circadian/models.py'),
+                                  'circadian.models.Hannay19.dlmos': ('api/models.html#hannay19.dlmos', 'circadian/models.py'),
+                                  'circadian.models.Hannay19.integrate': ('api/models.html#hannay19.integrate', 'circadian/models.py'),
+                                  'circadian.models.Hannay19.phase': ('api/models.html#hannay19.phase', 'circadian/models.py'),
+                                  'circadian.models.Hannay19TP': ('api/models.html#hannay19tp', 'circadian/models.py'),
+                                  'circadian.models.Hannay19TP.__init__': ('api/models.html#hannay19tp.__init__', 'circadian/models.py'),
+                                  'circadian.models.Hannay19TP.__repr__': ('api/models.html#hannay19tp.__repr__', 'circadian/models.py'),
+                                  'circadian.models.Hannay19TP.__str__': ('api/models.html#hannay19tp.__str__', 'circadian/models.py'),
+                                  'circadian.models.Hannay19TP.amplitude': ('api/models.html#hannay19tp.amplitude', 'circadian/models.py'),
+                                  'circadian.models.Hannay19TP.cbt': ('api/models.html#hannay19tp.cbt', 'circadian/models.py'),
+                                  'circadian.models.Hannay19TP.derv': ('api/models.html#hannay19tp.derv', 'circadian/models.py'),
+                                  'circadian.models.Hannay19TP.dlmos': ('api/models.html#hannay19tp.dlmos', 'circadian/models.py'),
+                                  'circadian.models.Hannay19TP.integrate': ('api/models.html#hannay19tp.integrate', 'circadian/models.py'),
+                                  'circadian.models.Hannay19TP.phase': ('api/models.html#hannay19tp.phase', 'circadian/models.py'),
+                                  'circadian.models.Jewett99': ('api/models.html#jewett99', 'circadian/models.py'),
+                                  'circadian.models.Jewett99.__init__': ('api/models.html#jewett99.__init__', 'circadian/models.py'),
+                                  'circadian.models.Jewett99.__repr__': ('api/models.html#jewett99.__repr__', 'circadian/models.py'),
+                                  'circadian.models.Jewett99.__str__': ('api/models.html#jewett99.__str__', 'circadian/models.py'),
+                                  'circadian.models.Jewett99.amplitude': ('api/models.html#jewett99.amplitude', 'circadian/models.py'),
+                                  'circadian.models.Jewett99.cbt': ('api/models.html#jewett99.cbt', 'circadian/models.py'),
+                                  'circadian.models.Jewett99.derv': ('api/models.html#jewett99.derv', 'circadian/models.py'),
+                                  'circadian.models.Jewett99.dlmos': ('api/models.html#jewett99.dlmos', 'circadian/models.py'),
+                                  'circadian.models.Jewett99.integrate': ('api/models.html#jewett99.integrate', 'circadian/models.py'),
+                                  'circadian.models.Jewett99.phase': ('api/models.html#jewett99.phase', 'circadian/models.py'),
+                                  'circadian.models._check_cbtmin_spacing': ( 'api/models.html#_check_cbtmin_spacing',
+                                                                              'circadian/models.py'),
+                                  'circadian.models._get_default_initial_condition': ( 'api/models.html#_get_default_initial_condition',
                                                                                        'circadian/models.py'),
-                                  'circadian.models.KronauerJewett.alphaFunction': ( 'models.html#kronauerjewett.alphafunction',
-                                                                                     'circadian/models.py'),
-                                  'circadian.models.KronauerJewett.amplitude': ( 'models.html#kronauerjewett.amplitude',
-                                                                                 'circadian/models.py'),
-                                  'circadian.models.KronauerJewett.cbt': ('models.html#kronauerjewett.cbt', 'circadian/models.py'),
-                                  'circadian.models.KronauerJewett.default_initial_conditions': ( 'models.html#kronauerjewett.default_initial_conditions',
-                                                                                                  'circadian/models.py'),
-                                  'circadian.models.KronauerJewett.derv': ('models.html#kronauerjewett.derv', 'circadian/models.py'),
-                                  'circadian.models.KronauerJewett.dlmos': ('models.html#kronauerjewett.dlmos', 'circadian/models.py'),
-                                  'circadian.models.KronauerJewett.phase': ('models.html#kronauerjewett.phase', 'circadian/models.py')},
-            'circadian.phasetools': { 'circadian.phasetools.cosinor': ('phasetools.html#cosinor', 'circadian/phasetools.py'),
-                                      'circadian.phasetools.cosinor_goals': ('phasetools.html#cosinor_goals', 'circadian/phasetools.py'),
-                                      'circadian.phasetools.cosinor_phase': ('phasetools.html#cosinor_phase', 'circadian/phasetools.py')},
-            'circadian.plots': { 'circadian.plots.Actogram': ('plots.html#actogram', 'circadian/plots.py'),
-                                 'circadian.plots.Actogram.__init__': ('plots.html#actogram.__init__', 'circadian/plots.py'),
-                                 'circadian.plots.Actogram.addLightSchedule': ( 'plots.html#actogram.addlightschedule',
+                                  'circadian.models._initial_condition_input_checking': ( 'api/models.html#_initial_condition_input_checking',
+                                                                                          'circadian/models.py'),
+                                  'circadian.models._light_input_checking': ( 'api/models.html#_light_input_checking',
+                                                                              'circadian/models.py'),
+                                  'circadian.models._model_input_checking': ( 'api/models.html#_model_input_checking',
+                                                                              'circadian/models.py'),
+                                  'circadian.models._parameter_input_checking': ( 'api/models.html#_parameter_input_checking',
+                                                                                  'circadian/models.py'),
+                                  'circadian.models._positive_int_checking': ( 'api/models.html#_positive_int_checking',
+                                                                               'circadian/models.py'),
+                                  'circadian.models._state_input_checking': ( 'api/models.html#_state_input_checking',
+                                                                              'circadian/models.py'),
+                                  'circadian.models._time_input_checking': ('api/models.html#_time_input_checking', 'circadian/models.py'),
+                                  'circadian.models._wake_input_checking': ('api/models.html#_wake_input_checking', 'circadian/models.py')},
+            'circadian.phasetools': { 'circadian.phasetools.cosinor': ('api/phasetools.html#cosinor', 'circadian/phasetools.py'),
+                                      'circadian.phasetools.cosinor_goals': ( 'api/phasetools.html#cosinor_goals',
+                                                                              'circadian/phasetools.py'),
+                                      'circadian.phasetools.cosinor_phase': ( 'api/phasetools.html#cosinor_phase',
+                                                                              'circadian/phasetools.py')},
+            'circadian.plots': { 'circadian.plots.Actogram': ('api/plots.html#actogram', 'circadian/plots.py'),
+                                 'circadian.plots.Actogram.__init__': ('api/plots.html#actogram.__init__', 'circadian/plots.py'),
+                                 'circadian.plots.Actogram.addLightSchedule': ( 'api/plots.html#actogram.addlightschedule',
                                                                                 'circadian/plots.py'),
-                                 'circadian.plots.Actogram.addRect': ('plots.html#actogram.addrect', 'circadian/plots.py'),
-                                 'circadian.plots.Actogram.getRectangles': ('plots.html#actogram.getrectangles', 'circadian/plots.py'),
-                                 'circadian.plots.Actogram.plot_phasemarker': ( 'plots.html#actogram.plot_phasemarker',
+                                 'circadian.plots.Actogram.addRect': ('api/plots.html#actogram.addrect', 'circadian/plots.py'),
+                                 'circadian.plots.Actogram.getRectangles': ('api/plots.html#actogram.getrectangles', 'circadian/plots.py'),
+                                 'circadian.plots.Actogram.plot_phasemarker': ( 'api/plots.html#actogram.plot_phasemarker',
                                                                                 'circadian/plots.py'),
-                                 'circadian.plots.Actogram.plot_phasetimes': ('plots.html#actogram.plot_phasetimes', 'circadian/plots.py'),
-                                 'circadian.plots.Stroboscopic': ('plots.html#stroboscopic', 'circadian/plots.py'),
-                                 'circadian.plots.Stroboscopic.__init__': ('plots.html#stroboscopic.__init__', 'circadian/plots.py'),
-                                 'circadian.plots.Stroboscopic._make_strobo_plot': ( 'plots.html#stroboscopic._make_strobo_plot',
+                                 'circadian.plots.Actogram.plot_phasetimes': ( 'api/plots.html#actogram.plot_phasetimes',
+                                                                               'circadian/plots.py'),
+                                 'circadian.plots.Stroboscopic': ('api/plots.html#stroboscopic', 'circadian/plots.py'),
+                                 'circadian.plots.Stroboscopic.__init__': ('api/plots.html#stroboscopic.__init__', 'circadian/plots.py'),
+                                 'circadian.plots.Stroboscopic._make_strobo_plot': ( 'api/plots.html#stroboscopic._make_strobo_plot',
                                                                                      'circadian/plots.py'),
-                                 'circadian.plots.Stroboscopic.add_strobo_plot': ( 'plots.html#stroboscopic.add_strobo_plot',
+                                 'circadian.plots.Stroboscopic.add_strobo_plot': ( 'api/plots.html#stroboscopic.add_strobo_plot',
                                                                                    'circadian/plots.py'),
-                                 'circadian.plots.plot_actogram': ('plots.html#plot_actogram', 'circadian/plots.py'),
-                                 'circadian.plots.plot_mae': ('plots.html#plot_mae', 'circadian/plots.py'),
-                                 'circadian.plots.plot_phasetimes': ('plots.html#plot_phasetimes', 'circadian/plots.py'),
-                                 'circadian.plots.plot_torus': ('plots.html#plot_torus', 'circadian/plots.py')},
-            'circadian.prc': { 'circadian.prc.DosageResponseCurve': ('prc.html#dosageresponsecurve', 'circadian/prc.py'),
-                               'circadian.prc.DosageResponseCurve.__init__': ('prc.html#dosageresponsecurve.__init__', 'circadian/prc.py'),
-                               'circadian.prc.DosageResponseCurve.light_dosage': ( 'prc.html#dosageresponsecurve.light_dosage',
+                                 'circadian.plots.plot_actogram': ('api/plots.html#plot_actogram', 'circadian/plots.py'),
+                                 'circadian.plots.plot_mae': ('api/plots.html#plot_mae', 'circadian/plots.py'),
+                                 'circadian.plots.plot_phasetimes': ('api/plots.html#plot_phasetimes', 'circadian/plots.py'),
+                                 'circadian.plots.plot_torus': ('api/plots.html#plot_torus', 'circadian/plots.py')},
+            'circadian.prc': { 'circadian.prc.DosageResponseCurve': ('api/prc.html#dosageresponsecurve', 'circadian/prc.py'),
+                               'circadian.prc.DosageResponseCurve.__init__': ( 'api/prc.html#dosageresponsecurve.__init__',
+                                                                               'circadian/prc.py'),
+                               'circadian.prc.DosageResponseCurve.light_dosage': ( 'api/prc.html#dosageresponsecurve.light_dosage',
                                                                                    'circadian/prc.py'),
-                               'circadian.prc.DosageResponseCurve.light_dosage_day1': ( 'prc.html#dosageresponsecurve.light_dosage_day1',
+                               'circadian.prc.DosageResponseCurve.light_dosage_day1': ( 'api/prc.html#dosageresponsecurve.light_dosage_day1',
                                                                                         'circadian/prc.py'),
-                               'circadian.prc.IntensityResponseCurveLight': ('prc.html#intensityresponsecurvelight', 'circadian/prc.py'),
-                               'circadian.prc.IntensityResponseCurveLight.__init__': ( 'prc.html#intensityresponsecurvelight.__init__',
+                               'circadian.prc.IntensityResponseCurveLight': ( 'api/prc.html#intensityresponsecurvelight',
+                                                                              'circadian/prc.py'),
+                               'circadian.prc.IntensityResponseCurveLight.__init__': ( 'api/prc.html#intensityresponsecurvelight.__init__',
                                                                                        'circadian/prc.py'),
-                               'circadian.prc.IntensityResponseCurveLight.light_intensity': ( 'prc.html#intensityresponsecurvelight.light_intensity',
+                               'circadian.prc.IntensityResponseCurveLight.light_intensity': ( 'api/prc.html#intensityresponsecurvelight.light_intensity',
                                                                                               'circadian/prc.py'),
-                               'circadian.prc.PRCFinder': ('prc.html#prcfinder', 'circadian/prc.py'),
-                               'circadian.prc.PRCFinder.exp_type0': ('prc.html#prcfinder.exp_type0', 'circadian/prc.py'),
-                               'circadian.prc.PRCFinder.prc_type0_point': ('prc.html#prcfinder.prc_type0_point', 'circadian/prc.py'),
-                               'circadian.prc.PRCFinder.type0x': ('prc.html#prcfinder.type0x', 'circadian/prc.py'),
-                               'circadian.prc.PhaseResponseCurveLight': ('prc.html#phaseresponsecurvelight', 'circadian/prc.py'),
-                               'circadian.prc.PhaseResponseCurveLight.__init__': ( 'prc.html#phaseresponsecurvelight.__init__',
+                               'circadian.prc.PRCFinder': ('api/prc.html#prcfinder', 'circadian/prc.py'),
+                               'circadian.prc.PRCFinder.exp_type0': ('api/prc.html#prcfinder.exp_type0', 'circadian/prc.py'),
+                               'circadian.prc.PRCFinder.prc_type0_point': ('api/prc.html#prcfinder.prc_type0_point', 'circadian/prc.py'),
+                               'circadian.prc.PRCFinder.type0x': ('api/prc.html#prcfinder.type0x', 'circadian/prc.py'),
+                               'circadian.prc.PhaseResponseCurveLight': ('api/prc.html#phaseresponsecurvelight', 'circadian/prc.py'),
+                               'circadian.prc.PhaseResponseCurveLight.__init__': ( 'api/prc.html#phaseresponsecurvelight.__init__',
                                                                                    'circadian/prc.py'),
-                               'circadian.prc.PhaseResponseCurveLight.light_amplitude_resetting': ( 'prc.html#phaseresponsecurvelight.light_amplitude_resetting',
+                               'circadian.prc.PhaseResponseCurveLight.light_amplitude_resetting': ( 'api/prc.html#phaseresponsecurvelight.light_amplitude_resetting',
                                                                                                     'circadian/prc.py'),
-                               'circadian.prc.PhaseResponseCurveLight.light_czeiler_type0': ( 'prc.html#phaseresponsecurvelight.light_czeiler_type0',
+                               'circadian.prc.PhaseResponseCurveLight.light_czeiler_type0': ( 'api/prc.html#phaseresponsecurvelight.light_czeiler_type0',
                                                                                               'circadian/prc.py'),
-                               'circadian.prc.PhaseResponseCurveLight.light_hilaire': ( 'prc.html#phaseresponsecurvelight.light_hilaire',
+                               'circadian.prc.PhaseResponseCurveLight.light_hilaire': ( 'api/prc.html#phaseresponsecurvelight.light_hilaire',
                                                                                         'circadian/prc.py'),
-                               'circadian.prc.PhaseResponseCurveLight.light_khalsa': ( 'prc.html#phaseresponsecurvelight.light_khalsa',
+                               'circadian.prc.PhaseResponseCurveLight.light_khalsa': ( 'api/prc.html#phaseresponsecurvelight.light_khalsa',
                                                                                        'circadian/prc.py'),
-                               'circadian.prc.RimmerLightPulseLight': ('prc.html#rimmerlightpulselight', 'circadian/prc.py'),
-                               'circadian.prc.RimmerLightPulseLight.__init__': ( 'prc.html#rimmerlightpulselight.__init__',
+                               'circadian.prc.RimmerLightPulseLight': ('api/prc.html#rimmerlightpulselight', 'circadian/prc.py'),
+                               'circadian.prc.RimmerLightPulseLight.__init__': ( 'api/prc.html#rimmerlightpulselight.__init__',
                                                                                  'circadian/prc.py'),
-                               'circadian.prc.RimmerLightPulseLight.make_pulse_rimmer': ( 'prc.html#rimmerlightpulselight.make_pulse_rimmer',
+                               'circadian.prc.RimmerLightPulseLight.make_pulse_rimmer': ( 'api/prc.html#rimmerlightpulselight.make_pulse_rimmer',
                                                                                           'circadian/prc.py'),
-                               'circadian.prc.RimmerLightPulseLight.pulse_rimmer_start': ( 'prc.html#rimmerlightpulselight.pulse_rimmer_start',
+                               'circadian.prc.RimmerLightPulseLight.pulse_rimmer_start': ( 'api/prc.html#rimmerlightpulselight.pulse_rimmer_start',
                                                                                            'circadian/prc.py'),
-                               'circadian.prc.heaviside': ('prc.html#heaviside', 'circadian/prc.py')},
-            'circadian.readers': { 'circadian.readers.WearableData': ('readers.html#wearabledata', 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.__getitem__': ( 'readers.html#wearabledata.__getitem__',
+                               'circadian.prc.get_pulse': ('api/prc.html#get_pulse', 'circadian/prc.py'),
+                               'circadian.prc.heaviside': ('api/prc.html#heaviside', 'circadian/prc.py'),
+                               'circadian.prc.make_pulse': ('api/prc.html#make_pulse', 'circadian/prc.py')},
+            'circadian.readers': { 'circadian.readers.WearableData': ('api/readers.html#wearabledata', 'circadian/readers.py'),
+                                   'circadian.readers.WearableData.__getitem__': ( 'api/readers.html#wearabledata.__getitem__',
                                                                                    'circadian/readers.py'),
-                                   'circadian.readers.WearableData.__post_init__': ( 'readers.html#wearabledata.__post_init__',
+                                   'circadian.readers.WearableData.__post_init__': ( 'api/readers.html#wearabledata.__post_init__',
                                                                                      'circadian/readers.py'),
-                                   'circadian.readers.WearableData._copy_with_metadata': ( 'readers.html#wearabledata._copy_with_metadata',
+                                   'circadian.readers.WearableData._copy_with_metadata': ( 'api/readers.html#wearabledata._copy_with_metadata',
                                                                                            'circadian/readers.py'),
-                                   'circadian.readers.WearableData.activity': ( 'readers.html#wearabledata.activity',
+                                   'circadian.readers.WearableData.activity': ( 'api/readers.html#wearabledata.activity',
                                                                                 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.aggregate': ( 'readers.html#wearabledata.aggregate',
+                                   'circadian.readers.WearableData.aggregate': ( 'api/readers.html#wearabledata.aggregate',
                                                                                  'circadian/readers.py'),
-                                   'circadian.readers.WearableData.build_sleep_chunks': ( 'readers.html#wearabledata.build_sleep_chunks',
+                                   'circadian.readers.WearableData.build_sleep_chunks': ( 'api/readers.html#wearabledata.build_sleep_chunks',
                                                                                           'circadian/readers.py'),
-                                   'circadian.readers.WearableData.date_bounds': ( 'readers.html#wearabledata.date_bounds',
+                                   'circadian.readers.WearableData.date_bounds': ( 'api/readers.html#wearabledata.date_bounds',
                                                                                    'circadian/readers.py'),
-                                   'circadian.readers.WearableData.datetime': ( 'readers.html#wearabledata.datetime',
+                                   'circadian.readers.WearableData.datetime': ( 'api/readers.html#wearabledata.datetime',
                                                                                 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.fillna': ('readers.html#wearabledata.fillna', 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.filter': ('readers.html#wearabledata.filter', 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.from_json': ( 'readers.html#wearabledata.from_json',
+                                   'circadian.readers.WearableData.fillna': ( 'api/readers.html#wearabledata.fillna',
+                                                                              'circadian/readers.py'),
+                                   'circadian.readers.WearableData.filter': ( 'api/readers.html#wearabledata.filter',
+                                                                              'circadian/readers.py'),
+                                   'circadian.readers.WearableData.from_json': ( 'api/readers.html#wearabledata.from_json',
                                                                                  'circadian/readers.py'),
-                                   'circadian.readers.WearableData.get_date': ( 'readers.html#wearabledata.get_date',
+                                   'circadian.readers.WearableData.get_date': ( 'api/readers.html#wearabledata.get_date',
                                                                                 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.get_timestamp': ( 'readers.html#wearabledata.get_timestamp',
+                                   'circadian.readers.WearableData.get_timestamp': ( 'api/readers.html#wearabledata.get_timestamp',
                                                                                      'circadian/readers.py'),
-                                   'circadian.readers.WearableData.groupby': ('readers.html#wearabledata.groupby', 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.head': ('readers.html#wearabledata.head', 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.heartrate': ( 'readers.html#wearabledata.heartrate',
+                                   'circadian.readers.WearableData.groupby': ( 'api/readers.html#wearabledata.groupby',
+                                                                               'circadian/readers.py'),
+                                   'circadian.readers.WearableData.head': ('api/readers.html#wearabledata.head', 'circadian/readers.py'),
+                                   'circadian.readers.WearableData.heartrate': ( 'api/readers.html#wearabledata.heartrate',
                                                                                  'circadian/readers.py'),
-                                   'circadian.readers.WearableData.join': ('readers.html#wearabledata.join', 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.light_estimate': ( 'readers.html#wearabledata.light_estimate',
+                                   'circadian.readers.WearableData.join': ('api/readers.html#wearabledata.join', 'circadian/readers.py'),
+                                   'circadian.readers.WearableData.light_estimate': ( 'api/readers.html#wearabledata.light_estimate',
                                                                                       'circadian/readers.py'),
-                                   'circadian.readers.WearableData.plot_heartrate': ( 'readers.html#wearabledata.plot_heartrate',
+                                   'circadian.readers.WearableData.plot_heartrate': ( 'api/readers.html#wearabledata.plot_heartrate',
                                                                                       'circadian/readers.py'),
-                                   'circadian.readers.WearableData.plot_hr_steps': ( 'readers.html#wearabledata.plot_hr_steps',
+                                   'circadian.readers.WearableData.plot_hr_steps': ( 'api/readers.html#wearabledata.plot_hr_steps',
                                                                                      'circadian/readers.py'),
-                                   'circadian.readers.WearableData.plot_light_activity': ( 'readers.html#wearabledata.plot_light_activity',
+                                   'circadian.readers.WearableData.plot_light_activity': ( 'api/readers.html#wearabledata.plot_light_activity',
                                                                                            'circadian/readers.py'),
-                                   'circadian.readers.WearableData.scatter_hr_steps': ( 'readers.html#wearabledata.scatter_hr_steps',
+                                   'circadian.readers.WearableData.scatter_hr_steps': ( 'api/readers.html#wearabledata.scatter_hr_steps',
                                                                                         'circadian/readers.py'),
-                                   'circadian.readers.WearableData.steps': ('readers.html#wearabledata.steps', 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.steps_hr_loglinear': ( 'readers.html#wearabledata.steps_hr_loglinear',
+                                   'circadian.readers.WearableData.steps': ('api/readers.html#wearabledata.steps', 'circadian/readers.py'),
+                                   'circadian.readers.WearableData.steps_hr_loglinear': ( 'api/readers.html#wearabledata.steps_hr_loglinear',
                                                                                           'circadian/readers.py'),
-                                   'circadian.readers.WearableData.tail': ('readers.html#wearabledata.tail', 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.time_hour_bounds': ( 'readers.html#wearabledata.time_hour_bounds',
+                                   'circadian.readers.WearableData.tail': ('api/readers.html#wearabledata.tail', 'circadian/readers.py'),
+                                   'circadian.readers.WearableData.time_hour_bounds': ( 'api/readers.html#wearabledata.time_hour_bounds',
                                                                                         'circadian/readers.py'),
-                                   'circadian.readers.WearableData.time_total': ( 'readers.html#wearabledata.time_total',
+                                   'circadian.readers.WearableData.time_total': ( 'api/readers.html#wearabledata.time_total',
                                                                                   'circadian/readers.py'),
-                                   'circadian.readers.WearableData.timestamp': ( 'readers.html#wearabledata.timestamp',
+                                   'circadian.readers.WearableData.timestamp': ( 'api/readers.html#wearabledata.timestamp',
                                                                                  'circadian/readers.py'),
-                                   'circadian.readers.WearableData.to_json': ('readers.html#wearabledata.to_json', 'circadian/readers.py'),
-                                   'circadian.readers.WearableData.trim_by_hour': ( 'readers.html#wearabledata.trim_by_hour',
+                                   'circadian.readers.WearableData.to_json': ( 'api/readers.html#wearabledata.to_json',
+                                                                               'circadian/readers.py'),
+                                   'circadian.readers.WearableData.trim_by_hour': ( 'api/readers.html#wearabledata.trim_by_hour',
                                                                                     'circadian/readers.py'),
-                                   'circadian.readers.WearableData.trim_by_idx': ( 'readers.html#wearabledata.trim_by_idx',
+                                   'circadian.readers.WearableData.trim_by_idx': ( 'api/readers.html#wearabledata.trim_by_idx',
                                                                                    'circadian/readers.py'),
-                                   'circadian.readers.WearableData.trim_by_timestamp': ( 'readers.html#wearabledata.trim_by_timestamp',
+                                   'circadian.readers.WearableData.trim_by_timestamp': ( 'api/readers.html#wearabledata.trim_by_timestamp',
                                                                                          'circadian/readers.py'),
-                                   'circadian.readers.WearableData.utc_to_hrs': ( 'readers.html#wearabledata.utc_to_hrs',
+                                   'circadian.readers.WearableData.utc_to_hrs': ( 'api/readers.html#wearabledata.utc_to_hrs',
                                                                                   'circadian/readers.py'),
-                                   'circadian.readers.WearableData.wake': ('readers.html#wearabledata.wake', 'circadian/readers.py'),
-                                   'circadian.readers.combine_wearable_streams': ( 'readers.html#combine_wearable_streams',
+                                   'circadian.readers.WearableData.wake': ('api/readers.html#wearabledata.wake', 'circadian/readers.py'),
+                                   'circadian.readers.combine_wearable_streams': ( 'api/readers.html#combine_wearable_streams',
                                                                                    'circadian/readers.py'),
-                                   'circadian.readers.read_actiwatch': ('readers.html#read_actiwatch', 'circadian/readers.py'),
-                                   'circadian.readers.read_standard_csv': ('readers.html#read_standard_csv', 'circadian/readers.py'),
-                                   'circadian.readers.read_standard_json': ('readers.html#read_standard_json', 'circadian/readers.py')},
-            'circadian.sleep': { 'circadian.sleep.TwoProcessModel': ('sleep.html#twoprocessmodel', 'circadian/sleep.py'),
-                                 'circadian.sleep.TwoProcessModel.__call__': ('sleep.html#twoprocessmodel.__call__', 'circadian/sleep.py'),
-                                 'circadian.sleep.TwoProcessModel.__init__': ('sleep.html#twoprocessmodel.__init__', 'circadian/sleep.py'),
-                                 'circadian.sleep.TwoProcessModel.check_wake_status': ( 'sleep.html#twoprocessmodel.check_wake_status',
+                                   'circadian.readers.read_actiwatch': ('api/readers.html#read_actiwatch', 'circadian/readers.py'),
+                                   'circadian.readers.read_standard_csv': ('api/readers.html#read_standard_csv', 'circadian/readers.py'),
+                                   'circadian.readers.read_standard_json': ('api/readers.html#read_standard_json', 'circadian/readers.py')},
+            'circadian.sleep': { 'circadian.sleep.TwoProcessModel': ('api/sleep.html#twoprocessmodel', 'circadian/sleep.py'),
+                                 'circadian.sleep.TwoProcessModel.__call__': ( 'api/sleep.html#twoprocessmodel.__call__',
+                                                                               'circadian/sleep.py'),
+                                 'circadian.sleep.TwoProcessModel.__init__': ( 'api/sleep.html#twoprocessmodel.__init__',
+                                                                               'circadian/sleep.py'),
+                                 'circadian.sleep.TwoProcessModel.check_wake_status': ( 'api/sleep.html#twoprocessmodel.check_wake_status',
                                                                                         'circadian/sleep.py'),
-                                 'circadian.sleep.TwoProcessModel.dhomeostat': ( 'sleep.html#twoprocessmodel.dhomeostat',
+                                 'circadian.sleep.TwoProcessModel.dhomeostat': ( 'api/sleep.html#twoprocessmodel.dhomeostat',
                                                                                  'circadian/sleep.py'),
-                                 'circadian.sleep.TwoProcessModel.step_rk4': ('sleep.html#twoprocessmodel.step_rk4', 'circadian/sleep.py'),
-                                 'circadian.sleep.cluster_sleep_periods_scipy': ( 'sleep.html#cluster_sleep_periods_scipy',
+                                 'circadian.sleep.TwoProcessModel.step_rk4': ( 'api/sleep.html#twoprocessmodel.step_rk4',
+                                                                               'circadian/sleep.py'),
+                                 'circadian.sleep.cluster_sleep_periods_scipy': ( 'api/sleep.html#cluster_sleep_periods_scipy',
                                                                                   'circadian/sleep.py'),
-                                 'circadian.sleep.sleep_midpoint': ('sleep.html#sleep_midpoint', 'circadian/sleep.py')},
-            'circadian.utils': { 'circadian.utils.NpEncoder': ('utils.html#npencoder', 'circadian/utils.py'),
-                                 'circadian.utils.NpEncoder.default': ('utils.html#npencoder.default', 'circadian/utils.py'),
-                                 'circadian.utils.abs_hour_diff': ('utils.html#abs_hour_diff', 'circadian/utils.py'),
-                                 'circadian.utils.angle_difference': ('utils.html#angle_difference', 'circadian/utils.py'),
-                                 'circadian.utils.cal_days_diff': ('utils.html#cal_days_diff', 'circadian/utils.py'),
-                                 'circadian.utils.circular_av_clock': ('utils.html#circular_av_clock', 'circadian/utils.py'),
-                                 'circadian.utils.circular_mean': ('utils.html#circular_mean', 'circadian/utils.py'),
-                                 'circadian.utils.circular_scatter': ('utils.html#circular_scatter', 'circadian/utils.py'),
-                                 'circadian.utils.convert_binary': ('utils.html#convert_binary', 'circadian/utils.py'),
-                                 'circadian.utils.cut_phases_12': ('utils.html#cut_phases_12', 'circadian/utils.py'),
-                                 'circadian.utils.interpolateLinear': ('utils.html#interpolatelinear', 'circadian/utils.py'),
-                                 'circadian.utils.interpolateLinearExt': ('utils.html#interpolatelinearext', 'circadian/utils.py'),
-                                 'circadian.utils.parse_dt': ('utils.html#parse_dt', 'circadian/utils.py'),
-                                 'circadian.utils.phase_coherence': ('utils.html#phase_coherence', 'circadian/utils.py'),
-                                 'circadian.utils.phase_coherence_clock': ('utils.html#phase_coherence_clock', 'circadian/utils.py'),
-                                 'circadian.utils.phase_ic_guess': ('utils.html#phase_ic_guess', 'circadian/utils.py'),
-                                 'circadian.utils.redact_dates': ('utils.html#redact_dates', 'circadian/utils.py'),
-                                 'circadian.utils.simple_norm_stepshr_sleep_classifier': ( 'utils.html#simple_norm_stepshr_sleep_classifier',
+                                 'circadian.sleep.sleep_midpoint': ('api/sleep.html#sleep_midpoint', 'circadian/sleep.py')},
+            'circadian.utils': { 'circadian.utils.NpEncoder': ('api/utils.html#npencoder', 'circadian/utils.py'),
+                                 'circadian.utils.NpEncoder.default': ('api/utils.html#npencoder.default', 'circadian/utils.py'),
+                                 'circadian.utils.abs_hour_diff': ('api/utils.html#abs_hour_diff', 'circadian/utils.py'),
+                                 'circadian.utils.amplitude_percent_change': ( 'api/utils.html#amplitude_percent_change',
+                                                                               'circadian/utils.py'),
+                                 'circadian.utils.angle_difference': ('api/utils.html#angle_difference', 'circadian/utils.py'),
+                                 'circadian.utils.cal_days_diff': ('api/utils.html#cal_days_diff', 'circadian/utils.py'),
+                                 'circadian.utils.circular_av_clock': ('api/utils.html#circular_av_clock', 'circadian/utils.py'),
+                                 'circadian.utils.circular_mean': ('api/utils.html#circular_mean', 'circadian/utils.py'),
+                                 'circadian.utils.circular_scatter': ('api/utils.html#circular_scatter', 'circadian/utils.py'),
+                                 'circadian.utils.convert_binary': ('api/utils.html#convert_binary', 'circadian/utils.py'),
+                                 'circadian.utils.cut_phases_12': ('api/utils.html#cut_phases_12', 'circadian/utils.py'),
+                                 'circadian.utils.interpolateLinear': ('api/utils.html#interpolatelinear', 'circadian/utils.py'),
+                                 'circadian.utils.interpolateLinearExt': ('api/utils.html#interpolatelinearext', 'circadian/utils.py'),
+                                 'circadian.utils.parse_dt': ('api/utils.html#parse_dt', 'circadian/utils.py'),
+                                 'circadian.utils.phase_coherence': ('api/utils.html#phase_coherence', 'circadian/utils.py'),
+                                 'circadian.utils.phase_coherence_clock': ('api/utils.html#phase_coherence_clock', 'circadian/utils.py'),
+                                 'circadian.utils.phase_difference': ('api/utils.html#phase_difference', 'circadian/utils.py'),
+                                 'circadian.utils.phase_ic_guess': ('api/utils.html#phase_ic_guess', 'circadian/utils.py'),
+                                 'circadian.utils.redact_dates': ('api/utils.html#redact_dates', 'circadian/utils.py'),
+                                 'circadian.utils.simple_norm_stepshr_sleep_classifier': ( 'api/utils.html#simple_norm_stepshr_sleep_classifier',
                                                                                            'circadian/utils.py'),
-                                 'circadian.utils.split_drop_data': ('utils.html#split_drop_data', 'circadian/utils.py'),
-                                 'circadian.utils.split_missing_data': ('utils.html#split_missing_data', 'circadian/utils.py'),
-                                 'circadian.utils.subtract_clock_times': ('utils.html#subtract_clock_times', 'circadian/utils.py'),
-                                 'circadian.utils.times_to_angle': ('utils.html#times_to_angle', 'circadian/utils.py'),
-                                 'circadian.utils.timezone_mapper': ('utils.html#timezone_mapper', 'circadian/utils.py')}}}
+                                 'circadian.utils.split_drop_data': ('api/utils.html#split_drop_data', 'circadian/utils.py'),
+                                 'circadian.utils.split_missing_data': ('api/utils.html#split_missing_data', 'circadian/utils.py'),
+                                 'circadian.utils.subtract_clock_times': ('api/utils.html#subtract_clock_times', 'circadian/utils.py'),
+                                 'circadian.utils.times_to_angle': ('api/utils.html#times_to_angle', 'circadian/utils.py'),
+                                 'circadian.utils.timezone_mapper': ('api/utils.html#timezone_mapper', 'circadian/utils.py')}}}
```

### Comparing `circadian-0.0.4/circadian/cli.py` & `circadian-1.0.0/circadian/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/09_cli.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/api/09_cli.ipynb.
 
 # %% auto 0
 __all__ = ['mytz', 'main_acto', 'main_esri']
 
-# %% ../nbs/09_cli.ipynb 4
+# %% ../nbs/api/09_cli.ipynb 4
+import sys
 import torch
+import argparse
+import circadian
+import numpy as np
+import pandas as pd
 from torch import jit
+from pathlib import Path
+from pytz import timezone
 from datetime import datetime
-import argparse
+from .metrics import *
+import matplotlib.pyplot as plt
 from .plots import Actogram
 from .models import Hannay19
-from .readers import WearableData, read_standard_csv, read_standard_json
 from .utils import phase_ic_guess
-from .sleep import cluster_sleep_periods_scipy, sleep_midpoint
 from .utils import simple_norm_stepshr_sleep_classifier
-from datetime import datetime
-import matplotlib.pylab as plt
-import numpy as np
-from pytz import timezone
-mytz = timezone('EST')
+from .sleep import cluster_sleep_periods_scipy, sleep_midpoint
+from .readers import WearableData, read_standard_csv, read_standard_json
 
+mytz = timezone('EST')
 
-# %% ../nbs/09_cli.ipynb 5
+# %% ../nbs/api/09_cli.ipynb 6
 def main_acto():
     parser = argparse.ArgumentParser(description="""Make an actogram""")
 
     parser.add_argument('-j', '--json',
                         required=False,
                         action='store',
                         type=str,
@@ -221,38 +225,17 @@
     #     sleep_mid, duration = sleep_midpoint(ts_flat, sleep_clusters)
     #     acto.plot_phasemarker(sleep_mid, error=(
     #         duration/2.0), color="green", alpha=1.0)
     #     print(f"The median sleep duration is {np.median(duration)}")
     #     print(f"The average bedtime is {np.mean(np.fmod(sleep_mid-0.5*duration, 24.0))}")
     #     print(f"The average waketime is {np.mean(np.fmod(sleep_mid,24.0)+0.5*duration)}")
 
-
     plt.show()
 
-
-# %% ../nbs/09_cli.ipynb 6
-import numpy as np
-import matplotlib.pyplot as plt
-import argparse
-from pathlib import Path
-import sys
-import torch
-from torch import jit
-import circadian
-from .readers import WearableData, read_standard_csv, read_standard_json
-from .models import Hannay19
-from .utils import phase_ic_guess
-from .metrics import *
-from .utils import simple_norm_stepshr_sleep_classifier
-import pandas as pd
-from .plots import Actogram
-from pytz import timezone
-
-
-# %% ../nbs/09_cli.ipynb 7
+# %% ../nbs/api/09_cli.ipynb 7
 def main_esri():
     mytz = timezone('EST')
     parser = argparse.ArgumentParser(
         description="""Compute the Entrainment Signal Regularity Index for a data set""")
 
     parser.add_argument("-a", "--actogram",
                         required=False,
@@ -392,10 +375,8 @@
         acto = Actogram(np.hstack(ts),
                         np.hstack(steps),
                         ax=ax1,
                         threshold=args.threshold,
                         opacity=1.0,
                         sigma=[args.sigma, args.sigma])
 
-
         plt.show()
-
```

### Comparing `circadian-0.0.4/circadian/metrics.py` & `circadian-1.0.0/circadian/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,64 +1,58 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/04_metrics.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/api/04_metrics.ipynb.
 
 # %% auto 0
 __all__ = ['esri', 'esri_trajectory']
 
-# %% ../nbs/04_metrics.ipynb 3
+# %% ../nbs/api/04_metrics.ipynb 4
 import numpy as np
 from .models import Hannay19
 from .utils import phase_ic_guess
 from .readers import WearableData
 
-# %% ../nbs/04_metrics.ipynb 4
+# %% ../nbs/api/04_metrics.ipynb 5
 def esri(awObj: WearableData, 
                 gamma: float = 0.0,
                 multiplier: float = 1.0,
                 num_days: float = 4.5):
 
     spmodel = Hannay19({'K': 0.0, 'gamma': gamma})
     psi0 = phase_ic_guess(awObj.time_total[0])
 
     idx = awObj.time_total < awObj.time_total[0]+24*num_days
-    sol = spmodel.integrate_model(
-        awObj.time_total[idx], multiplier*awObj.steps[idx],
-        np.array([0.10, psi0, 0.0])
-    )
-    return sol.ts, sol.states
+    sol = spmodel.integrate(awObj.time_total[idx], 
+                            np.array([0.10, psi0, 0.0]),
+                            multiplier*awObj.steps[idx],) 
+    return sol.time, sol.states
 
-
-
-# %% ../nbs/04_metrics.ipynb 5
+# %% ../nbs/api/04_metrics.ipynb 6
 def esri_trajectory(awObj: WearableData,
-                           gamma: float = 0.0,
-                           multiplier: float = 1.0,
-                           num_days: float = 4.5,
-                           ):
-
+                    gamma: float = 0.0,
+                    multiplier: float = 1.0,
+                    num_days: float = 4.5,
+                    ):
     spmodel = Hannay19({'K': 0.0, 'gamma': gamma})
     compactness_trajectory = []
     time_trajectory = []
     timestamps = []
     timeStart = awObj.time_total[0]
     timestampStart = awObj.timestamp[0]
     while timeStart < awObj.time_total[-1] - 24*num_days:
         try:
             psi0 = phase_ic_guess(timeStart)
             idxStart = (awObj.time_total > timeStart)
             tsFilter = awObj.time_total[idxStart]
             idx = tsFilter < np.array(tsFilter[0])+24*num_days
             stepsFilter = awObj.steps[idxStart]
-            trajectory = spmodel.integrate_model(
-                tsFilter[idx], multiplier*stepsFilter[idx],
-                np.array([0.10, psi0, 0.0])
-            )
+            trajectory = spmodel.integrate(
+                tsFilter[idx], np.array([0.10, psi0, 0.0], 
+                multiplier*stepsFilter[idx]))
             sol = trajectory.states
             if sol[0, -1] > 0.0:
                 compactness_trajectory.append(sol[0, -1])
                 time_trajectory.append(timeStart)
                 timestamps.append(
                     3600.0*(timeStart - awObj.time_total[0]) + timestampStart)
         except:
             print("Error in trajectory")
         timeStart += 1.0
     return time_trajectory, timestamps, compactness_trajectory
-
```

### Comparing `circadian-0.0.4/circadian/phasetools.py` & `circadian-1.0.0/circadian/phasetools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,42 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/08_phasetools.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/api/08_phasetools.ipynb.
 
 # %% auto 0
 __all__ = ['cosinor', 'cosinor_phase', 'cosinor_goals']
 
-# %% ../nbs/08_phasetools.ipynb 2
-import circadian 
-
-
-# %% ../nbs/08_phasetools.ipynb 4
+# %% ../nbs/api/08_phasetools.ipynb 4
+import circadian
 import numpy as np 
-import matplotlib.pyplot as plt
 import scipy as sp 
-from typing import List 
 import numpy.linalg 
+from typing import List 
+import matplotlib.pyplot as plt
 
-# %% ../nbs/08_phasetools.ipynb 9
+# %% ../nbs/api/08_phasetools.ipynb 8
 def cosinor(t: np.array, # time vector
                   y: np.array, # signal vector
                   tau: float # period of cosinor analysis 
                   ) -> float: # phase estimate
     
     omega = 2*np.pi/tau 
     sin_transform = np.sin(omega*t)
     cos_transform = np.cos(omega*t)
     a1 = np.dot(y, sin_transform) / np.dot(sin_transform, sin_transform)
     a2 = np.dot(y, cos_transform) / np.dot(cos_transform, cos_transform)
     return np.array([a1, a2])
 
-
-# %% ../nbs/08_phasetools.ipynb 10
+# %% ../nbs/api/08_phasetools.ipynb 9
 def cosinor_phase(a: np.array) -> float: 
     z = a[1]+ complex(0,1)*a[0]
     return np.angle(z)
 
-# %% ../nbs/08_phasetools.ipynb 13
+# %% ../nbs/api/08_phasetools.ipynb 12
 def cosinor_goals(t, y, tau: float):
     omega = 2*np.pi/tau 
     A = np.stack((np.ones(len(t)), np.sin(omega*t), np.cos(omega*t)), axis=1)
     
     Q,R = np.linalg.qr(A)
     x1 = Q[:,1]
     x2 = Q[:,2] 
     
     z = complex(0,1)*np.dot(x1,y) /np.dot(x1,np.sin(omega*t)) + np.dot(x2,y)/np.dot(x2,np.cos(omega*t))
     return np.array([z.imag, z.real])
-
```

### Comparing `circadian-0.0.4/circadian/plots.py` & `circadian-1.0.0/circadian/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/03_plots.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/api/03_plots.ipynb.
 
 # %% auto 0
 __all__ = ['Actogram', 'plot_mae', 'plot_torus', 'Stroboscopic', 'plot_actogram', 'plot_phasetimes']
 
-# %% ../nbs/03_plots.ipynb 4
-from scipy.ndimage import gaussian_filter1d
-from copy import deepcopy
-import pylab as plt
+# %% ../nbs/api/03_plots.ipynb 4
+import sys
+import matplotlib
 import numpy as np
+import pylab as plt
 from pathlib import Path
-import sys
-from .utils import cut_phases_12
+from copy import deepcopy
 from .models import Hannay19
-from .lights import *
-
-#from circadian.readers import read_standard_json
-import matplotlib as mpl
-
+from .utils import cut_phases_12
+from .lights import LightSchedule
+from scipy.ndimage import gaussian_filter1d
 
-# %% ../nbs/03_plots.ipynb 7
+# %% ../nbs/api/03_plots.ipynb 7
 class Actogram:
     """ 
         Create an Actogram visualisation of the data
     """
-
     def __init__(self,
                  time_total: np.ndarray, # time in hours
                  light_vals: np.ndarray, # light values or proxy should be the same length as time_total
                  second_zeit: np.ndarray = None, # optional second zeitgeber to show on the right side
                  ax=None, # Axis to plot on, if None a new figure is created
                  threshold=10.0, # threshold for light on/off 
                  threshold2=None, # threshold for light on/off for second zeitgeber
@@ -237,17 +233,15 @@
                 xx+24.0, yvals_split[idx], alpha=alpha, *args, **kwargs)
             if error is not None:
                 self.ax.fill_betweenx(
                     yvals_split[idx], xx-error_split[idx], xx+error_split[idx], alpha=alpha_error, *args, **kwargs)
                 self.ax.fill_betweenx(
                     yvals_split[idx], xx-error_split[idx]+24.0, xx+error_split[idx]+24.0, alpha=alpha_error, *args, **kwargs)
 
-
-
-# %% ../nbs/03_plots.ipynb 9
+# %% ../nbs/api/03_plots.ipynb 9
 def plot_mae(dlmo_actual: np.ndarray,  # expected to be in hours
              dlmo_pred: np.ndarray,  # predicted to be in hours
              norm_to: float = None, 
              ax=None,  
              *args, 
              **kwargs):
 
@@ -277,17 +271,15 @@
             ls='--', color='blue', lw=1.0)
     ax.plot(np.arange(-12, 12, 1), np.arange(-12, 12, 1)-1,
             ls='--', color='blue', lw=1.0)
 
     ax.set_ylabel("Model Prediction (hrs)")
     ax.set_xlabel("Experimental DLMO (hrs)")
 
-
-
-# %% ../nbs/03_plots.ipynb 11
+# %% ../nbs/api/03_plots.ipynb 11
 def plot_torus(phase1: np.ndarray, # array of phases  
                phase2: np.ndarray, #array of phases, assumed to be the same length as phase1
                scaled_by: float = None, # should the phases be wrapped, this just applies an fmod to the phases
                ax=None, # axis to plot on, if None, a new figure is created
                *args, # passed to the scatter plot
                **kwargs, # passed to the scatter plot
                ) -> plt.Axes:
@@ -303,29 +295,27 @@
     phase1 = np.arctan2(np.sin(phase1), np.cos(phase1))
     phase2 = np.arctan2(np.sin(phase2), np.cos(phase2))
 
     ax.scatter(phase1, phase2, *args, **kwargs)
     
     return ax
 
-
-# %% ../nbs/03_plots.ipynb 15
+# %% ../nbs/api/03_plots.ipynb 15
 class Stroboscopic:
     """
     This class can be used to make a stroboscopic plot of the entrainment of an oscillator to a sudden shift in schedule
     """
-
     def __init__(self, 
                  ax: plt.Axes, # The axes to plot on
                  ts: np.ndarray, # The time series of the model
-                amplitude: np.ndarray, # The amplitude of the model, assumed to be the same length as ts
-                phase: np.ndarray, # The phase of the model, assumed to be the same length as ts
-                period: float = 24.0, # The time period between stroboscopic arrows
-                *args: tuple, #passed to the quiver plot
-                **kwargs: dict #passed to the quiver plot
+                 amplitude: np.ndarray, # The amplitude of the model, assumed to be the same length as ts
+                 phase: np.ndarray, # The phase of the model, assumed to be the same length as ts
+                 period: float = 24.0, # The time period between stroboscopic arrows
+                 *args: tuple, #passed to the quiver plot
+                 **kwargs: dict #passed to the quiver plot
         ):
         
         self.ts = ts
         self.R = amplitude
         self.phase = phase
         self.period = period
         self.ax = ax
@@ -372,19 +362,19 @@
 
         upper_bound = min(10, len(Xvals))
         for i in range(1, upper_bound + 10):
             self.ax.quiver(Xvals[i - 1], Yvals[i - 1], Xvals[i] - Xvals[i - 1], Yvals[i] - Yvals[i - 1],
                            scale_units='xy', angles='xy', scale=1, color=col)
 
 
-# %% ../nbs/03_plots.ipynb 18
+# %% ../nbs/api/03_plots.ipynb 18
 def plot_actogram(ax: plt.Axes, # plot axes
                   zeitgeber: np.ndarray, # the zeitgeber to display
                   num_day: int = 240, # number of points per day
-                  cmap: mpl.colors.Colormap = mpl.cm.get_cmap('jet'), # the colormap to use
+                  cmap: matplotlib.colors.Colormap = matplotlib.colormaps['jet'], # the colormap to use
                   label_days: int = 7, # the number of days between labels
                   *args, # passed to imshow
                   **kwargs # passed to imshow
                  ) -> plt.Axes:
     
     """Make an actogram plot with color"""
     zeitgeber = np.flip(zeitgeber)
@@ -409,15 +399,15 @@
     ax.set_xticks(np.arange(0, 240, 30))
     xlabels_list = list(range(0, 24, 3))
     ax.set_xticklabels(xlabels_list)
     ax.set_xticks(np.arange(0, 240, 10), minor=True)
     
     ax.invert_yaxis()
 
-# %% ../nbs/03_plots.ipynb 20
+# %% ../nbs/api/03_plots.ipynb 20
 def plot_phasetimes(ax: plt.Axes,
                     times: np.ndarray, 
                     phases: np.ndarray, 
                     error: np.ndarray = None,
                     alpha_error=0.30, 
                     alpha=1.0, 
                     *args,
```

### Comparing `circadian-0.0.4/circadian/prc.py` & `circadian-1.0.0/circadian/prc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_prc.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/api/02_prc.ipynb.
 
 # %% auto 0
-__all__ = ['RimmerLightPulseLight', 'PhaseResponseCurveLight', 'heaviside', 'PRCFinder', 'IntensityResponseCurveLight',
-           'DosageResponseCurve']
-
-# %% ../nbs/02_prc.ipynb 5
-# Need to finish implementing this 
+__all__ = ['RimmerLightPulseLight', 'make_pulse', 'get_pulse', 'PhaseResponseCurveLight', 'heaviside', 'PRCFinder',
+           'IntensityResponseCurveLight', 'DosageResponseCurve']
 
+# %% ../nbs/api/02_prc.ipynb 4
+import numpy as np
+import matplotlib.pyplot as plt
+from .lights import LightSchedule
+from .models import CircadianModel, Hannay19
 
+# %% ../nbs/api/02_prc.ipynb 5
+# TODO: Finish implementing this 
 class RimmerLightPulseLight:
-     
     def __init__(self) -> None:
         pass 
-      
+
     @staticmethod
     def make_pulse_rimmer(t: float, 
                           tstart: float, 
                           tend: float):
         val = 0.0
         steep = 100.0
         trans = 25.0/60.0
@@ -50,20 +53,35 @@
         if ((t < tstart) and (t > tstart-trans)):
             val = 5000.0
             factor = np.floor((t-tstart+trans)*60.0/5.0)
             val += factor*1000.0
 
         return(val)
 
+# %% ../nbs/api/02_prc.ipynb 6
+# TODO: Replace the use of these two functions with LightSchedules
+def make_pulse(t, tstart, tend, steep: float=30.0):
+    return 0.5*np.tanh(steep*(t-tstart))-0.5*np.tanh(steep*(t-tend))
+
+def get_pulse(t: float,
+              t1: float,
+              t2: float,
+              repeat=False,
+              Intensity: float = 150.0):
+
+    if repeat:
+        t = np.fmod(t, 24.0)
+    if t < 0.0:
+        t += 24.0
 
+    light_value = Intensity*make_pulse(t, t1, t2)
+    return np.abs(light_value)
 
-
-# %% ../nbs/02_prc.ipynb 6
+# %% ../nbs/api/02_prc.ipynb 7
 class PhaseResponseCurveLight:
-    
     def __init__(self) -> None:
          pass 
      
     def light_khalsa(t: float, 
                      CR: float):
         # Implement a Khalsa Light Schedule give a parameter for the initial CR length */
 
@@ -112,22 +130,16 @@
             make_pulse(t, CR+8+24.0, CR+24+24.0)
         val += 0.02*make_pulse(t, 0+48.0, CR+48.0)+roomLight * \
             make_pulse(t, CR+8+48.0, CR+24+48.0)
         val += afterLight*make_pulse(t, CR+24+48.0+8.0, CR+24+48.0+1000)
         val += 9850*make_pulse(t, CR+8+8-2.5, CR+8+8+2.5)+9850*make_pulse(t, CR+8+8 -
                                                                         2.5+24.0, CR+8+8+2.5+24.0)+9850*make_pulse(t, CR+8+8-2.5+48.0, CR+8+8+2.5+48.0)
         return(val)
-    
-    
-    
-    
-
 
-
-# %% ../nbs/02_prc.ipynb 7
+# %% ../nbs/api/02_prc.ipynb 8
 def heaviside(x: float) -> float:
     if x < 0:
         return 0
     else:
         return 1
     
 class PRCFinder:
@@ -161,47 +173,41 @@
         Gives a single point from the Type 0 Human protocol. The initial cond
         passed in should already be entrained to a regular routine.
         CRlengths for the model fit were taken to vary in the range (6.0,30.0)
         every 0.05. However, this was just for convience.
         Every data point in this study is actually a diffirent person so the
         parameters should be allowed to vary for each computed point.....
         """
-        
-        CRFinal=30.0
-        tend=72.0+8.0+30.0+CRFinal
-        ts = np.arange(0,tend,0.10)
-        light_vals = np.array([PhaseResponseCurveLight.light_czeiler_type0(t, CRlength) for t in ts])
-        trajectory = model(ts, light_vals, initial_value)
-        CBT = model.cbt(trajectory=trajectory)
-        shift=(CBT[0]-CBT[-1]) % 24.0 #finds a neg number between zero and -24.0
+        CRFinal = 30.0
+        tend = 72.0 + 8.0 + 30.0 + CRFinal
+        time = np.arange(0, tend, 0.10)
+        light_vals = np.array([PhaseResponseCurveLight.light_czeiler_type0(t, CRlength) for t in time])
+        trajectory = model(time, initial_value, light_vals)
+        CBT = model.cbt()
+        shift = (CBT[0] - CBT[-1]) % 24.0 #finds a neg number between zero and -24.0
 
         #now shifts live in the range (-12,12) hours
         if (shift < -12.0):
-            shift+=24.0
+            shift += 24.0
 
         #Now find the phase of the stimulus
-        phase=(CRlength-CBT[0]+12.0+16.0-2.5) % 24.0
+        phase = (CRlength - CBT[0] + 12.0 + 16.0 - 2.5) % 24.0
         return phase,shift
-    
-    
-        
 
-# %% ../nbs/02_prc.ipynb 9
+# %% ../nbs/api/02_prc.ipynb 10
 class IntensityResponseCurveLight:
-    
     def __init__(self) -> None:
          pass
      
     @staticmethod
     def light_intensity(t, Intensity):
         """
         Define the light schedule for the dosage response curve experiments. All light exposures started at phi 6.75 hours
         before Tmin and lasted 6.5 hours of varying intensities
         """
-
         cr_light_level = 10.0  # verified, in the statistics section of the methods
         wake_light_level = 10.0  # verified
         wake_stimulus_light_level = 0.03
         sleep_light_level = 0.03
         stimulus_light_level = Intensity
 
         w = 50.0  # length of the constant routine, should be approx 50 hours, did have 50.0-9.50
@@ -216,26 +222,23 @@
         val += sleep_light_level*make_pulse(t, w+24.0, w+32.0)
         # final cr to assess the phase shift induced
         val += cr_light_level*make_pulse(t, w+32.0, w+32.0+30.0)
 
         # Stimulus should start 5.25 hours after phase zero, so that it is centered 3.5 hours before Tmin
         return(val)
 
-
-
-# %% ../nbs/02_prc.ipynb 10
+# %% ../nbs/api/02_prc.ipynb 11
 class DosageResponseCurve:
     
     def __init__(self) -> None:
          pass
      
     @staticmethod
     def light_dosage(t: float, length: float):
         # Implement the Light Schedule for Chang et al's Dosage Response Curve */
-
         CR1 = 48.0  # approx 50.0
         CR2 = 30.0
         CR_light_level = 1.0
         stimulus_light_level = 10000.0
         wake_light_level = 3.0
 
         val = 0.0
@@ -259,9 +262,7 @@
         s = t % 24.0
         val = 0.0
         if (s < 8.0):
             val = 90.0
         if ((s >= 8.0) and (s <= 16.0)):
             val = 3.0
         return(val)
-
-
```

### Comparing `circadian-0.0.4/circadian/readers.py` & `circadian-1.0.0/circadian/readers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,43 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/05_readers.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/api/05_readers.ipynb.
 
 # %% auto 0
 __all__ = ['EXAMPLE_DATA', 'wearable_schema', 'WearableData', 'combine_wearable_streams', 'read_standard_csv',
            'read_standard_json', 'read_actiwatch']
 
-# %% ../nbs/05_readers.ipynb 4
-from copy import deepcopy
-import datetime
-from datetime import datetime
-import numpy as np
-import pandas as pd
-import pylab as plt
-from dataclasses import dataclass
-from scipy.stats import linregress
-
+# %% ../nbs/api/05_readers.ipynb 4
+import os
 import json
 import gzip
-from typing import List, Tuple, Dict, Union, Optional, Any, Callable, Iterable
-import os
-from .utils import *
-import random
-import difflib
 import glob 
-import os
-from scipy.ndimage import gaussian_filter1d
-from os import read
-pd.options.mode.chained_assignment = None
-
-import glob
-import os
 import random
 import difflib
-from scipy.ndimage import gaussian_filter1d
-
-from  jsonschema import validate
-from fastcore.basics import *
-from .plots import Actogram
 import circadian
+import numpy as np
+import pylab as plt
+import pandas as pd
+from os import read
 from pathlib import Path
+from copy import deepcopy
+from .utils import *
+from datetime import datetime
+from jsonschema import validate
+from dataclasses import dataclass
+from scipy.stats import linregress
+from fastcore.basics import patch_to
+from .plots import Actogram
+from scipy.ndimage import gaussian_filter1d
+from typing import List, Tuple, Dict, Union, Optional, Any, Callable, Iterable
 
-# %% ../nbs/05_readers.ipynb 5
-# path to the data folder
+pd.options.mode.chained_assignment = None
+
+# %% ../nbs/api/05_readers.ipynb 5
 EXAMPLE_DATA = circadian.__path__[0]
 
-# %% ../nbs/05_readers.ipynb 6
+# %% ../nbs/api/05_readers.ipynb 6
 wearable_schema = {
     type: "object",
     "properties": {
             "steps": {
                 "type": "array",
                 "items": { "type": "object", "properties": { 
                     "start": { "type": "number" },
@@ -67,20 +57,18 @@
                 "items": { "type": "object", "properties": { 
                     "timestamp": { "type": "number" },
                     "heartrate": { "type": "number" },
             } } },
     },
     "required": ["steps", "wake", "heartrate"]
 }
-    
 
-# %% ../nbs/05_readers.ipynb 9
+# %% ../nbs/api/05_readers.ipynb 9
 @dataclass
 class WearableData:
-    
     _dataframe: pd.DataFrame # the dataframe that holds the data must have datetime columns plus any other wearable streams from steps, heartrate, wake, light_estimate, activity
     phase_measure: np.ndarray = None
     phase_measure_times: np.ndarray = None
     subject_id: str = "unknown-subject"
     data_id: str = "unknown-data-id"
     meta_data: Dict[str, Any] = None
     
@@ -250,33 +238,32 @@
                 if isinstance(jdict[s], list):
                     setattr(wdata, s, [np.array(jdict[s])])
                 else:
                     setattr(wdata, s, jdict[s])
 
         return wdata
 
-
-# %% ../nbs/05_readers.ipynb 10
-@patch 
+# %% ../nbs/api/05_readers.ipynb 10
+@patch_to(WearableData)
 def steps_hr_loglinear(self: WearableData
                        ) -> Tuple[float, float]:
         """
         Find the log steps to hr linear regression parameters .
         hr=beta*log(steps+1.0)+alpha
         Returns beta,alpha
         """
         x = np.log(np.hstack(self.steps)+1.0)
         y = np.hstack(self.heartrate)
         x = x[y > 0]
         y = y[y > 0]
         slope, intercept, r_value, p_value, std_err = linregress(x, y)
         return slope, intercept
 
-# %% ../nbs/05_readers.ipynb 12
-@patch
+# %% ../nbs/api/05_readers.ipynb 12
+@patch_to(WearableData)
 def plot_heartrate(self: WearableData, 
                    t1=None, 
                    t2=None, 
                    ax: plt.Axes = None,
                    show_plot: bool = True,
                    color: str = 'red', 
                    use_dates: bool = True,
@@ -301,18 +288,17 @@
         ax.set_xlabel('Days')
         ax.set_ylabel('BPM')
         ax.set_title('Heart Rate Data')
         
         if show_plot:
             plt.show()
         return ax
-      
 
-# %% ../nbs/05_readers.ipynb 13
-@patch
+# %% ../nbs/api/05_readers.ipynb 13
+@patch_to(WearableData)
 def scatter_hr_steps(self: WearableData, 
                      take_log: bool = True, # Log transform the data?
                      *args, 
                      **kwargs):
     
         fig = plt.figure()
         ax = plt.gca()
@@ -333,16 +319,16 @@
                        **kwargs)
 
         ax.set_ylabel('BPM')
         ax.set_xlabel('Steps')
         ax.set_title('Heart Rate Data')
         plt.show()
 
-# %% ../nbs/05_readers.ipynb 14
-@patch
+# %% ../nbs/api/05_readers.ipynb 14
+@patch_to(WearableData)
 def plot_hr_steps(self: WearableData, 
                   t1: float = None, 
                   t2: float = None, 
                   *args, 
                   **kwargs):
 
         time_start = t1 if t1 is not None else self.time_total[0]/24.0
@@ -384,16 +370,15 @@
         ax[0].grid()
         ax[1].grid()
         ax[0].set_xlim((time_start, time_end))
         ax[1].set_xlim((time_start, time_end+3.0))
         ax[0].set_ylim((0, 200))
         plt.show()
 
-
-# %% ../nbs/05_readers.ipynb 16
+# %% ../nbs/api/05_readers.ipynb 16
 def combine_wearable_streams(steps: pd.DataFrame,  # dataframe with columns 'start', 'end', 'steps'
                              heartrate: pd.DataFrame,  # dataframe with columns 'timestamp', 'heartrate'
                              wake: pd.DataFrame,  # dataframe with columns 'start', 'end', 'wake'
                              bin_minutes: int = 6,  # bin size in minutes for the resampled combined data
                              subject_id: str = "unknown-subject",
                              data_id: str = "Exporter",
                              sleep_trim: bool = False,  # drop any entries without a sleep-wake entry
@@ -494,17 +479,15 @@
         wake = pd.DataFrame(columns=['start', 'end', 'wake'], dtype=float)
 
     if steps is None:
         raise ValueError("No steps file found, need to at least have that file")
 
     return combine_wearable_streams(steps, heartrate, wake, bin_minutes, subject_id, data_id, sleep_trim, inner_join)
 
-
-
-# %% ../nbs/05_readers.ipynb 17
+# %% ../nbs/api/05_readers.ipynb 17
 def read_standard_json(filepath: str,  # path to json file
                        bin_minutes: int = 6,  # data will be binned to this resolution in minutes
                        subject_id: str = "unknown-subject",  # subject id to be used
                        data_id: str = "Exporter",  # name of the data source
                        # set to true if the file is gzipped, will be autodetected if extension is .gz
                        gzip_opt: bool = False,
                        sleep_trim: bool = False,  # drop any entries without a sleep-wake entry
@@ -520,33 +503,32 @@
     # These could be empty
     wake = pd.DataFrame(rawJson['wake'], columns=["start", "end", "wake"])
     heartrate = pd.DataFrame(rawJson['heartrate'], columns=[
                              "timestamp", "heartrate"])
 
     return combine_wearable_streams(steps, heartrate, wake, bin_minutes, subject_id, data_id, sleep_trim, inner_join)
 
-
-# %% ../nbs/05_readers.ipynb 18
-@patch 
+# %% ../nbs/api/05_readers.ipynb 18
+@patch_to(WearableData)
 def fillna(self: WearableData, 
              column_name: str = "heartrate", # column to fill in the dataframe
              with_value: float = 0.0, # value to fill with
              inplace: bool = False # if true, the WearableData object will be modified in place
              ) -> WearableData:
     
     if inplace:
         self._dataframe[column_name].fillna(with_value, inplace=True)
     else:
         df = self._dataframe.copy()
         filled_column = df[column_name].fillna(with_value)
         df[column_name] = filled_column 
         return self._copy_with_metadata(df)
 
-# %% ../nbs/05_readers.ipynb 34
-@patch 
+# %% ../nbs/api/05_readers.ipynb 34
+@patch_to(WearableData)
 def plot_light_activity(self: WearableData, 
                         show=True, 
                         vlines=None, 
                         *args, **kwargs):
 
         fig = plt.figure()
         gs = fig.add_gridspec(2, hspace=0)
@@ -580,29 +562,28 @@
         ax[0].grid()
         ax[1].grid()
         if show:
             plt.show()
         else:
             return ax
 
-
-# %% ../nbs/05_readers.ipynb 36
+# %% ../nbs/api/05_readers.ipynb 36
 def read_actiwatch(filepath: str, # path to actiwatch csv file
-                        MIN_LIGHT_THRESHOLD=5000, # used to trim off empty data at the beginning and end of the file, must reach this amount of light to be included. Turn this off can setting this to 0 or negative
-                        round_data=True, # round the data to the nearest bin_minutes
-                        bin_minutes=6, # bin the data to this resolution in minutes, only used if round_data is true
-                        dt_format: str = None, # format of the date time string, if None, will be inferred
-                        data_id: str = "Actiwatch", # name of the data source
-                        subject_id: str = "unknown-subject", #subject id to be used
-                        ) -> WearableData:
+                   MIN_LIGHT_THRESHOLD=5000, # used to trim off empty data at the beginning and end of the file, must reach this amount of light to be included. Turn this off can setting this to 0 or negative 
+                   round_data=True, # round the data to the nearest bin_minutes 
+                   bin_minutes=6, # bin the data to this resolution in minutes, only used if round_data is true 
+                   dt_format: str = None, # format of the date time string, if None, will be inferred 
+                   data_id: str = "Actiwatch", # name of the data source 
+                   subject_id: str = "unknown-subject", #subject id to be used
+                   ) -> WearableData:
     
     df = pd.read_csv(filepath, names=['Date', 'Time', 'Activity', 'White Light', 'Sleep/Wake'], header=0) 
     df['datetime'] = df['Date']+" "+df['Time']
     if dt_format is None:
-        df['datetime'] = pd.to_datetime(df.datetime, infer_datetime_format=True)
+        df['datetime'] = pd.to_datetime(df.datetime)
     else:
         df['datetime'] = pd.to_datetime(df.datetime, format=dt_format)
 
     df['UnixTime'] = (
         df['datetime'] - pd.Timestamp("1970-01-01")) // pd.Timedelta('1s')
     
     df.rename(columns={'White Light': 'light_estimate'}, inplace=True)
@@ -637,8 +618,7 @@
     df.activity.fillna(0.0, inplace=True) 
     df.light_estimate.fillna(0.0, inplace=True)
     return WearableData(
         _dataframe = df,
         data_id=data_id,
         subject_id=subject_id
     )
-
```

### Comparing `circadian-0.0.4/circadian/sleep.py` & `circadian-1.0.0/circadian/sleep.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,35 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/06_sleep.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/api/06_sleep.ipynb.
 
 # %% auto 0
 __all__ = ['TwoProcessModel', 'sleep_midpoint', 'cluster_sleep_periods_scipy']
 
-# %% ../nbs/06_sleep.ipynb 2
-from nbdev import show_doc
-
-# %% ../nbs/06_sleep.ipynb 3
-import numpy as np
-import pandas as pd
-import scipy as sp
-from numba import jit
-from scipy import interpolate
-import torch 
+# %% ../nbs/api/06_sleep.ipynb 4
+import copy
 import json
 import pytz
+import torch 
 import datetime
-import copy
-import scipy as sp
-from scipy.integrate import solve_ivp
 from math import *
+import scipy as sp
+import numpy as np
 import pylab as plt
-
-from scipy.optimize import minimize
+import pandas as pd
+from numba import jit
+from scipy import interpolate
+from .plots import *
 from .utils import *
 from .models import * 
 from .lights import *
-from .plots import *
+from scipy.optimize import minimize
+from scipy.integrate import solve_ivp
 
-# %% ../nbs/06_sleep.ipynb 5
+# %% ../nbs/api/06_sleep.ipynb 6
 class TwoProcessModel:
-
+    "Implementation of the two-process model of sleep regulation."
     def __init__(self, steps_wake_threshold: float = 10.0):
         self.steps_wake_threshold = steps_wake_threshold
         self.awake = True
 
     @staticmethod
     def check_wake_status(awake: bool, # current wake status
                           h: float,  # homeostat value
@@ -100,31 +95,30 @@
                  ) -> DynamicalTrajectory:
         sol = np.zeros((len(initial_value), len(ts)))
         current_state = initial_value
         sol[:,0] = current_state
         for idx in range(1,len(ts)):
             current_state = self.step_rk4(current_state, steps[idx], phase[idx])
             sol[:,idx] = current_state
-        return(DynamicalTrajectory(ts, np.array(sol)))
+        return(DynamicalTrajectory(ts, np.array(sol.T)))
 
-# %% ../nbs/06_sleep.ipynb 7
+# %% ../nbs/api/06_sleep.ipynb 8
 def sleep_midpoint(timetotal: np.ndarray, 
                    Wake: np.ndarray, 
                    durations=True):
     """
         Given a wearable data frame with a Wake column which takes 
         the values 0, 1, missing this routine will create a sleep phase 
         column which is based on constant phase accumulation between sleep 
         midpoints. 
 
         The sleep midpoints are found using the criteria than they the median 
         time where 
 
     """
-
     sleep_start = []
     sleep_end = []
     awake = Wake[0] > 0.50
 
     if not awake:
         sleep_start.append(timetotal[1])
 
@@ -148,32 +142,29 @@
         sleep_durations += [s2-s1]
 
     if durations:
         return np.array(sleep_midpoints), np.array(sleep_durations)
     else:
         return np.array(sleep_midpoints)
 
-
-
-# %% ../nbs/06_sleep.ipynb 8
+# %% ../nbs/api/06_sleep.ipynb 9
 def cluster_sleep_periods_scipy(wake_data: np.ndarray, 
                                 epsilon: float,
                                 makeplot: bool = False,
                                 max_sleep_clusters=None, 
                                 min_sleep_clusters=None):
     """
         Given a binary vector wake_data which gives a prediction for the sleep/wake  
         status and a regularization penalty ε this function will create smoothed 
         sleep-wake periods. This helps as preprocessing to remove erroneous short sleep 
         periods (and wake) which may mess up calculations like the sleep midpoint for 
         the day
 
         cluster_sleep_periods(wake_data : np.ndarray, epsilon: float, makeplot: bool=False):
     """
-
     np.nan_to_num(wake_data, 0.50)
 
     def objective(w):
         return sum(w * (1 - wake_data)) + sum((1 - w)*wake_data) + epsilon*sum((w[1:]-w[0:-1])**2)
 
     max_clusters = max_sleep_clusters or len(wake_data)
```

### Comparing `circadian-0.0.4/circadian/utils.py` & `circadian-1.0.0/circadian/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,62 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/07_utils.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/api/07_utils.ipynb.
 
 # %% auto 0
-__all__ = ['NpEncoder', 'simple_norm_stepshr_sleep_classifier', 'phase_ic_guess', 'abs_hour_diff', 'cut_phases_12',
-           'convert_binary', 'cal_days_diff', 'interpolateLinear', 'interpolateLinearExt', 'parse_dt', 'circular_mean',
-           'phase_coherence', 'phase_coherence_clock', 'angle_difference', 'subtract_clock_times', 'circular_av_clock',
-           'circular_scatter', 'times_to_angle', 'timezone_mapper', 'split_missing_data', 'split_drop_data',
-           'redact_dates']
+__all__ = ['phase_difference', 'amplitude_percent_change', 'NpEncoder', 'simple_norm_stepshr_sleep_classifier', 'phase_ic_guess',
+           'abs_hour_diff', 'cut_phases_12', 'convert_binary', 'cal_days_diff', 'interpolateLinear',
+           'interpolateLinearExt', 'parse_dt', 'circular_mean', 'phase_coherence', 'phase_coherence_clock',
+           'angle_difference', 'subtract_clock_times', 'circular_av_clock', 'circular_scatter', 'times_to_angle',
+           'timezone_mapper', 'split_missing_data', 'split_drop_data', 'redact_dates']
 
-# %% ../nbs/07_utils.ipynb 3
-import numpy as np
-import pandas as pd
-import scipy as sp
-from numba import jit
-from scipy import interpolate
-import torch 
+# %% ../nbs/api/07_utils.ipynb 4
+import copy
 import json
 import pytz
+import gzip
+import torch 
 import datetime
-import copy
-import scipy as sp
-from scipy.integrate import solve_ivp
 from math import *
+import scipy as sp
+import numpy as np
 import pylab as plt
-import gzip
+import pandas as pd
+from numba import jit
+from scipy import interpolate
+from scipy.integrate import solve_ivp
 
+# %% ../nbs/api/07_utils.ipynb 5
+def phase_difference(phase_1: float, # phase between [-pi, pi]
+                     phase_2: float # phase between [-pi, pi]
+                     ):
+    "Phase difference (phase_2 - phase_1). Negative values represent clockwise rotations"
+    diff = phase_2 - phase_1
+    normalized_diff = (diff + np.pi) % (2 * np.pi) - np.pi
+    return normalized_diff
+
+# %% ../nbs/api/07_utils.ipynb 7
+def amplitude_percent_change(amplitude_1: float, # amplitude between (0, inf)
+                             amplitude_2: float # amplitude between (0, inf)
+                             ):
+    "Percent change between two amplitudes"
+    return (amplitude_2 - amplitude_1) / amplitude_1 * 100
 
-# %% ../nbs/07_utils.ipynb 4
+# %% ../nbs/api/07_utils.ipynb 9
 class NpEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.floating):
             return float(obj)
         if isinstance(obj, np.ndarray):
             return obj.tolist()
         if isinstance(obj, datetime.datetime):
             return obj.isoformat()
         return super(NpEncoder, self).default(obj)
 
-# %% ../nbs/07_utils.ipynb 5
+# %% ../nbs/api/07_utils.ipynb 10
 pd.options.mode.chained_assignment = None  # default='warn'
 
 def simple_norm_stepshr_sleep_classifier(t):
         t[0,:] = torch.tanh((t[0,:] - 10.0)/ 100.0)
         t[1, torch.nonzero(t[1,:])] = torch.tanh((t[1,torch.nonzero(t[1,:])] - 60.0) / 30.0)
         return t 
 
@@ -129,15 +143,15 @@
 
 
 def parse_dt(date, time):
     strDate = date + ' ' + time
     return pd.to_datetime(strDate, format='%m/%d/%Y %I:%M %p')
 
 
-# %% ../nbs/07_utils.ipynb 7
+# %% ../nbs/api/07_utils.ipynb 12
 def circular_mean(series):
     Z=complex(0,0)
     series=np.array(series)
     for i in range(len(series)):
         Z+=np.exp(series[i]*complex(0,1))
 
     Z=Z/float(len(series))
@@ -203,20 +217,16 @@
     ax.scatter(angles, radii, color=color)
     ax.set_theta_zero_location("N")
     ax.set_theta_direction(-1)
     ax.set_thetagrids(list(range(0,360,45)), list(range(0,24,3)))
     ax.set_rmax(1.2)
     ax.set_rticks([0.0,0.2,0.6,0.8,1.0])
     ax.annotate("", xytext=(0.0,0.0), xy=(circular_mean(angles),phase_coherence(angles)),arrowprops=dict(facecolor=color))
-    
-    
-    
 
-
-# %% ../nbs/07_utils.ipynb 9
+# %% ../nbs/api/07_utils.ipynb 14
 class NpEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.floating):
             return float(obj)
         if isinstance(obj, np.ndarray):
@@ -315,15 +325,15 @@
 
     if len(idx_long) > 0:
         return ([date_time[i] for i in idx_long], [ts_split[idx] for idx in idx_long], [steps_split[i] for i in idx_long],
                 [hr_split[i] for i in idx_long], [wake_split[i] for i in idx_long])
     else:
         return None
 
-# %% ../nbs/07_utils.ipynb 11
+# %% ../nbs/api/07_utils.ipynb 16
 def redact_dates(infile: str, # the input file in json format
                  outfile: str, # the output file in json format with dates redacted, for user privacy
                  gzip_opt: bool = False # if the input file is gzipped, if the extension is .gz, this is set to True
                  ) -> None:
     gzip_opt = gzip_opt if gzip_opt else infile.endswith(".gz")
     fileobj = gzip.open(infile, 'r') if gzip_opt else open(infile, 'r')
     data = json.load(fileobj)
@@ -335,9 +345,7 @@
     for i in range(len(data['heartrate'])):
         data['heartrate'][i]['timestamp'] -= first_time
     for i in range(len(data['wake'])):
         data['wake'][i]['start'] -= first_time
         data['wake'][i]['end'] -= first_time
         
     json.dump(data, open(outfile, 'w'))
-    
-
```

### Comparing `circadian-0.0.4/circadian.egg-info/SOURCES.txt` & `circadian-1.0.0/circadian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circadian-0.0.4/settings.ini` & `circadian-1.0.0/settings.ini`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 [DEFAULT]
 repo = circadian
 lib_name = circadian
-version = 0.0.4
+version = 1.0.0
 min_python = 3.7
 license = apache2
 doc_path = _docs
 lib_path = circadian
 nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
 branch = main
-custom_sidebar = False
-doc_host = https://khannay.github.io
+custom_sidebar = True
+doc_host = https://arcascope.github.io/circadian/
 doc_baseurl = /circadian
-git_url = https://github.com/khannay/circadian
-title = circadian
+git_url = https://github.com/Arcascope/circadian
+title = circadian by Arcascope
 audience = Developers
-author = Kevin Hannay
-author_email = 13168556+khannay@users.noreply.github.com
-copyright = 2023 onwards, Kevin Hannay
+author = Arcascope Inc.
+author_email = support@arcascope.com
+copyright = Arcascope
 description = Tools for the simulation and analysis of circadian rhythms
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
-user = khannay
+user = Arcascope
 requirements = fastcore pandas numpy scipy matplotlib torch numba pytz jsonschema
 console_scripts = acto=circadian.cli:main_acto
 	esri=circadian.cli:main_esri
 black_formatting = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
-clear_all = False
-
+clear_all = False
```

### Comparing `circadian-0.0.4/setup.py` & `circadian-1.0.0/setup.py`

 * *Files identical despite different names*


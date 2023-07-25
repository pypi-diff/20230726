# Comparing `tmp/teneva_bm-0.3.0.tar.gz` & `tmp/teneva_bm-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teneva_bm-0.3.0.tar", last modified: Sat Jul 22 18:08:27 2023, max compression
+gzip compressed data, was "teneva_bm-0.4.0.tar", last modified: Tue Jul 25 22:45:22 2023, max compression
```

## Comparing `teneva_bm-0.3.0.tar` & `teneva_bm-0.4.0.tar`

### file list

```diff
@@ -1,67 +1,75 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.962700 teneva_bm-0.3.0/
--rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.3.0/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       54 2023-04-26 09:54:29.000000 teneva_bm-0.3.0/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)    15443 2023-07-22 18:08:27.962983 teneva_bm-0.3.0/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)    14182 2023-07-22 18:08:03.000000 teneva_bm-0.3.0/README.md
--rw-r--r--   0 andrei     (501) staff       (20)      652 2023-07-17 09:21:50.000000 teneva_bm-0.3.0/demo.py
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-07-22 18:08:27.964205 teneva_bm-0.3.0/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2518 2023-07-16 14:04:06.000000 teneva_bm-0.3.0/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.935247 teneva_bm-0.3.0/teneva_bm/
--rw-r--r--   0 andrei     (501) staff       (20)      187 2023-07-22 18:07:52.000000 teneva_bm-0.3.0/teneva_bm/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)    18025 2023-07-22 17:43:46.000000 teneva_bm-0.3.0/teneva_bm/bm.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.943879 teneva_bm-0.3.0/teneva_bm/func/
--rw-r--r--   0 andrei     (501) staff       (20)      516 2023-07-13 07:42:30.000000 teneva_bm-0.3.0/teneva_bm/func/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     2973 2023-07-17 14:30:03.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_ackley.py
--rw-r--r--   0 andrei     (501) staff       (20)     2444 2023-07-17 14:32:24.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_alpine.py
--rw-r--r--   0 andrei     (501) staff       (20)     2423 2023-07-17 14:32:05.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_dixon.py
--rw-r--r--   0 andrei     (501) staff       (20)     2438 2023-07-17 14:32:52.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_exp.py
--rw-r--r--   0 andrei     (501) staff       (20)     2886 2023-07-17 14:33:30.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_griewank.py
--rw-r--r--   0 andrei     (501) staff       (20)     3008 2023-07-17 14:34:01.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_michalewicz.py
--rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 14:34:28.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_piston.py
--rw-r--r--   0 andrei     (501) staff       (20)     2550 2023-07-17 14:34:49.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_qing.py
--rw-r--r--   0 andrei     (501) staff       (20)     2873 2023-07-17 14:35:06.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_rastrigin.py
--rw-r--r--   0 andrei     (501) staff       (20)     3189 2023-07-17 14:35:23.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_rosenbrock.py
--rw-r--r--   0 andrei     (501) staff       (20)     2171 2023-07-17 14:35:48.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_schaffer.py
--rw-r--r--   0 andrei     (501) staff       (20)     2824 2023-07-17 14:36:05.000000 teneva_bm-0.3.0/teneva_bm/func/bm_func_schwefel.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.945509 teneva_bm-0.3.0/teneva_bm/hs/
--rw-r--r--   0 andrei     (501) staff       (20)       78 2023-07-17 21:02:17.000000 teneva_bm-0.3.0/teneva_bm/hs/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     1624 2023-07-22 16:16:15.000000 teneva_bm-0.3.0/teneva_bm/hs/bm_hs_func001.py
--rw-r--r--   0 andrei     (501) staff       (20)     2120 2023-07-22 17:59:30.000000 teneva_bm-0.3.0/teneva_bm/hs/bm_hs_func006.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.949583 teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/
--rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     2272 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs007.py
--rw-r--r--   0 andrei     (501) staff       (20)     2459 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs008.py
--rw-r--r--   0 andrei     (501) staff       (20)     2318 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs009.py
--rw-r--r--   0 andrei     (501) staff       (20)     2266 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs010.py
--rw-r--r--   0 andrei     (501) staff       (20)     2251 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs011.py
--rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs012.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.954177 teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/
--rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     1937 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py
--rw-r--r--   0 andrei     (501) staff       (20)     1857 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py
--rw-r--r--   0 andrei     (501) staff       (20)     1839 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py
--rw-r--r--   0 andrei     (501) staff       (20)     2197 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py
--rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py
--rw-r--r--   0 andrei     (501) staff       (20)     1929 2023-07-17 20:25:36.000000 teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.955936 teneva_bm-0.3.0/teneva_bm/oc/
--rw-r--r--   0 andrei     (501) staff       (20)       87 2023-07-13 07:42:11.000000 teneva_bm-0.3.0/teneva_bm/oc/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     3326 2023-07-17 18:44:45.000000 teneva_bm-0.3.0/teneva_bm/oc/bm_oc_simple.py
--rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-22 17:35:02.000000 teneva_bm-0.3.0/teneva_bm/oc/bm_oc_simple_constr.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.959602 teneva_bm-0.3.0/teneva_bm/qubo/
--rw-r--r--   0 andrei     (501) staff       (20)      166 2023-07-22 15:44:37.000000 teneva_bm-0.3.0/teneva_bm/qubo/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7130 2023-07-22 16:59:19.000000 teneva_bm-0.3.0/teneva_bm/qubo/bm_qubo_knap_det.py
--rw-r--r--   0 andrei     (501) staff       (20)     1866 2023-07-17 19:22:24.000000 teneva_bm-0.3.0/teneva_bm/qubo/bm_qubo_knap_quad.py
--rw-r--r--   0 andrei     (501) staff       (20)     2662 2023-07-17 15:10:35.000000 teneva_bm-0.3.0/teneva_bm/qubo/bm_qubo_maxcut.py
--rw-r--r--   0 andrei     (501) staff       (20)     2668 2023-07-17 19:22:18.000000 teneva_bm-0.3.0/teneva_bm/qubo/bm_qubo_mvc.py
--rw-r--r--   0 andrei     (501) staff       (20)     3270 2023-07-17 20:15:06.000000 teneva_bm-0.3.0/teneva_bm/teneva_bm_demo.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.962088 teneva_bm-0.3.0/teneva_bm/various/
--rw-r--r--   0 andrei     (501) staff       (20)      105 2023-07-13 07:41:21.000000 teneva_bm-0.3.0/teneva_bm/various/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     6982 2023-07-17 20:05:20.000000 teneva_bm-0.3.0/teneva_bm/various/bm_matmul.py
--rw-r--r--   0 andrei     (501) staff       (20)    11422 2023-07-17 19:32:33.000000 teneva_bm-0.3.0/teneva_bm/various/bm_topopt.py
--rw-r--r--   0 andrei     (501) staff       (20)     1919 2023-07-17 19:22:56.000000 teneva_bm-0.3.0/teneva_bm/various/bm_wall_simple.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-22 18:08:27.937422 teneva_bm-0.3.0/teneva_bm.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)    15443 2023-07-22 18:08:27.000000 teneva_bm-0.3.0/teneva_bm.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     1945 2023-07-22 18:08:27.000000 teneva_bm-0.3.0/teneva_bm.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-22 18:08:27.000000 teneva_bm-0.3.0/teneva_bm.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-22 18:08:27.000000 teneva_bm-0.3.0/teneva_bm.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)       10 2023-07-22 18:08:27.000000 teneva_bm-0.3.0/teneva_bm.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.533345 teneva_bm-0.4.0/
+-rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.4.0/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       54 2023-04-26 09:54:29.000000 teneva_bm-0.4.0/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)    18288 2023-07-25 22:45:22.533554 teneva_bm-0.4.0/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)    17027 2023-07-25 22:44:31.000000 teneva_bm-0.4.0/README.md
+-rw-r--r--   0 andrei     (501) staff       (20)      779 2023-07-24 16:41:37.000000 teneva_bm-0.4.0/demo.py
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-07-25 22:45:22.534178 teneva_bm-0.4.0/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2518 2023-07-16 14:04:06.000000 teneva_bm-0.4.0/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.504854 teneva_bm-0.4.0/teneva_bm/
+-rw-r--r--   0 andrei     (501) staff       (20)      233 2023-07-25 22:44:38.000000 teneva_bm-0.4.0/teneva_bm/__init__.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.509336 teneva_bm-0.4.0/teneva_bm/agent/
+-rw-r--r--   0 andrei     (501) staff       (20)       45 2023-07-25 20:49:49.000000 teneva_bm-0.4.0/teneva_bm/agent/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     4457 2023-07-25 22:27:59.000000 teneva_bm-0.4.0/teneva_bm/agent/agent.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1185 2023-07-25 22:09:12.000000 teneva_bm-0.4.0/teneva_bm/agent/bm_agent_swimmer.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.511345 teneva_bm-0.4.0/teneva_bm/agent_toe/
+-rw-r--r--   0 andrei     (501) staff       (20)       52 2023-07-25 20:50:12.000000 teneva_bm-0.4.0/teneva_bm/agent_toe/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2959 2023-07-25 22:32:56.000000 teneva_bm-0.4.0/teneva_bm/agent_toe/agent_toe.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1277 2023-07-25 22:25:31.000000 teneva_bm-0.4.0/teneva_bm/agent_toe/bm_agent_toe_swimmer.py
+-rw-r--r--   0 andrei     (501) staff       (20)    29490 2023-07-25 21:41:50.000000 teneva_bm-0.4.0/teneva_bm/bm.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.518279 teneva_bm-0.4.0/teneva_bm/func/
+-rw-r--r--   0 andrei     (501) staff       (20)      516 2023-07-13 07:42:30.000000 teneva_bm-0.4.0/teneva_bm/func/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3523 2023-07-25 15:25:46.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_ackley.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2398 2023-07-24 16:50:33.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_alpine.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2457 2023-07-24 16:49:31.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_dixon.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2392 2023-07-24 16:50:42.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_exp.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2840 2023-07-24 16:50:21.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_griewank.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3388 2023-07-24 16:49:54.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_michalewicz.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2402 2023-07-24 16:50:01.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_piston.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2580 2023-07-24 16:50:11.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_qing.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3152 2023-07-24 16:50:59.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_rastrigin.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3244 2023-07-24 16:51:02.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_rosenbrock.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2096 2023-07-24 16:51:10.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_schaffer.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3204 2023-07-24 16:51:17.000000 teneva_bm-0.4.0/teneva_bm/func/bm_func_schwefel.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.520121 teneva_bm-0.4.0/teneva_bm/hs/
+-rw-r--r--   0 andrei     (501) staff       (20)       78 2023-07-17 21:02:17.000000 teneva_bm-0.4.0/teneva_bm/hs/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1624 2023-07-22 16:16:15.000000 teneva_bm-0.4.0/teneva_bm/hs/bm_hs_func001.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2120 2023-07-22 17:59:30.000000 teneva_bm-0.4.0/teneva_bm/hs/bm_hs_func006.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.524315 teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/
+-rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2272 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs007.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2459 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs008.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2318 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs009.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2266 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs010.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2251 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs011.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs012.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.528595 teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/
+-rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1937 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1857 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1839 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2197 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1929 2023-07-17 20:25:36.000000 teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.530101 teneva_bm-0.4.0/teneva_bm/oc/
+-rw-r--r--   0 andrei     (501) staff       (20)       87 2023-07-13 07:42:11.000000 teneva_bm-0.4.0/teneva_bm/oc/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     4185 2023-07-24 12:59:27.000000 teneva_bm-0.4.0/teneva_bm/oc/bm_oc_simple.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-22 17:35:02.000000 teneva_bm-0.4.0/teneva_bm/oc/bm_oc_simple_constr.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.531725 teneva_bm-0.4.0/teneva_bm/qubo/
+-rw-r--r--   0 andrei     (501) staff       (20)      166 2023-07-22 15:44:37.000000 teneva_bm-0.4.0/teneva_bm/qubo/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7130 2023-07-22 16:59:19.000000 teneva_bm-0.4.0/teneva_bm/qubo/bm_qubo_knap_det.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1864 2023-07-25 16:21:14.000000 teneva_bm-0.4.0/teneva_bm/qubo/bm_qubo_knap_quad.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2929 2023-07-25 15:27:50.000000 teneva_bm-0.4.0/teneva_bm/qubo/bm_qubo_maxcut.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2935 2023-07-25 15:26:50.000000 teneva_bm-0.4.0/teneva_bm/qubo/bm_qubo_mvc.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3386 2023-07-24 16:41:38.000000 teneva_bm-0.4.0/teneva_bm/teneva_bm_demo.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.533047 teneva_bm-0.4.0/teneva_bm/various/
+-rw-r--r--   0 andrei     (501) staff       (20)      105 2023-07-13 07:41:21.000000 teneva_bm-0.4.0/teneva_bm/various/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7815 2023-07-24 13:03:33.000000 teneva_bm-0.4.0/teneva_bm/various/bm_matmul.py
+-rw-r--r--   0 andrei     (501) staff       (20)    12451 2023-07-24 13:04:15.000000 teneva_bm-0.4.0/teneva_bm/various/bm_topopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1877 2023-07-24 12:57:04.000000 teneva_bm-0.4.0/teneva_bm/various/bm_wall_simple.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-07-25 22:45:22.507712 teneva_bm-0.4.0/teneva_bm.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)    18288 2023-07-25 22:45:22.000000 teneva_bm-0.4.0/teneva_bm.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     2143 2023-07-25 22:45:22.000000 teneva_bm-0.4.0/teneva_bm.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-07-25 22:45:22.000000 teneva_bm-0.4.0/teneva_bm.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-25 22:45:22.000000 teneva_bm-0.4.0/teneva_bm.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       10 2023-07-25 22:45:22.000000 teneva_bm-0.4.0/teneva_bm.egg-info/top_level.txt
```

### Comparing `teneva_bm-0.3.0/LICENSE.txt` & `teneva_bm-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/PKG-INFO` & `teneva_bm-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,35 @@
-Metadata-Version: 2.1
-Name: teneva_bm
-Version: 0.3.0
-Summary: Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods
-Home-page: https://github.com/AndreiChertkov/teneva_bm
-Author: Andrei Chertkov
-Author-email: andre.chertkov@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
-Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # teneva_bm
 
 
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.3.0".
+> Current version "0.4.0".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.2+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following command:
 
-```bash
-pip install networkx==3.0 qubogen==0.1.1 gekko==1.0.6
-```
+- Collections `func`, `hs` and `various` do not require installation of additional libraries.
+
+- Сollections `oc` and `qubo` require installation of the following libraries:
+    ```bash
+    pip install networkx==3.0 qubogen==0.1.1 gekko==1.0.6
+    ```
+
+- Сollections `agent` and `agent_toe` require a rather complicated installation process of the `mujoco` framework, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
+
+> To run benchmark optimization examples, you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
 
 
 ## Documentation and examples
 
 All benchmarks inherit from the `Bm` base class (`teneva_bm/bm.py`) and are located in the subfolders (collections of benchmarks) of `teneva_bm` folder. The corresponding python files contain a detailed description of the benchmarks, as well as a scripts for a demo run at the end of the files. You can get detailed information on the created benchmark using the `info` class method:
 ```python
 from teneva_bm import *
@@ -58,21 +39,27 @@
 
 You can run demos for all benchmarks at once with the command `python demo.py` from the root folder of the project (you can also specify the name of the benchmark as a script argument to run the demo for only one benchmark, e.g., `python demo.py bm_qubo_knap_det`). You can also use a function from the `teneva_bm` package to run all or only one demo:
 ```python
 from teneva_bm import teneva_bm_demo
 teneva_bm_demo('bm_qubo_knap_det', with_info=True)
 ```
 
-> We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/demo_base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.2`).
+> We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/demo_base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
+
+> We also present some examples [DRAFT!] in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
 
 
 ## Available benchmarks
 
+- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) is assumed. The collection includes the following benchmarks: `BmAgentSwimmer`.
+
+- `agent_toe` - the same as `agent` collection, but with optimization of the discrete Toeplitz policy. The collection includes the following benchmarks: `BmAgentToeSwimmer`.
+
 - `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
-    > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores.
+    > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores. Note also that we apply small random shift of the grid limits for all functions, to make the optimization problem more difficult (because many functions have a minimum at the center point of the domain).
 
 - `hs` (draft!) - the [Hock & Schittkowski](http://apmonitor.com/wiki/index.php/Apps/HockSchittkowski) collection of benchmark functions, containing continuous analytic functions of small dimensions (2-5), some of which have given constraints. The collection includes the following benchmarks: `BmHsFunc001`, `BmHsFunc006`.
 
 - `oc` - a collection of optimal control problems described by ordinary differential equations with discrete binary control variable, some of the problems have explicit restrictions on the elements of the control vector. The collection includes the following benchmarks: `BmOcSimple`, `BmOcSimpleConstr`.
 
 - `qubo` - a collection of quadratic unconstrained binary optimization (QUBO) problems; all benchmarks are discrete and have a mode size equals `2`. The collection includes the following benchmarks: `BmQuboKnapDet`, `BmQuboKnapQuad`, `BmQuboMaxcut`, `BmQuboMvc`.
     > The exact global minimum is known only for `BmQuboKnapDet` benchmark (note that this benchmark supports only dimensions `10`, `20`, `50`, `80` and `100`).
@@ -103,27 +90,31 @@
 - `desc` - the description of the benchmark (string). By default, a detailed description of the benchmark is used, provided in the corresponding python file.
 - `...other arguments...` - some benchmarks have additional optional arguments, which are described in the corresponding python files.
 
 ##### Setting advanced options
 
 Before calling the `bm.prep()` method, you can set a number of additional benchmark options:
 
-- `bm.set_grid_kind(kind)` - by default, we use the Chebyshev grid (`kind = 'cheb'`), but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
+- `bm.set_seed(seed=42)` - with this function we can set a custom random seed. Note that we use `Random Generator` from numpy (i.e., `numpy.random.default_rng(seed)`).
+-
+- `bm.set_grid_kind(kind='cheb')` - by default, we use the Chebyshev grid (`kind = 'cheb'`), but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
+
+- `bm.set_budget(m=None, m_cache=None, is_strict=True)` - optional method to set the computation buget `m`. If the number of requests to the benchmark (from calls to `bm.get` and `bm.get_poi` methods) exceeds the specified budget, then `None` will be returned. If the flag `is_strict` is disabled, then the request for the last batch will be allowed, after which the budget will be exceeded, otherwise this last batch will not be considered. Note that when the budget is exceeded, `None` will be returned both when requesting a single value and a batch of values. Also, in a similar way, you can set a limit on the use of the cache by `m_cache` parameter.
 
 - `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm._c`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned).
 
-- `bm.set_max(i, x, y)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks , which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
+- `bm.set_max(i=None, x=None, y=None)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks , which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
 
-- `bm.set_min(i, x, y)` - the same as in the previous point, but for the global minimum.
+- `bm.set_min(i=None, x=None, y=None)` - the same as in the previous point, but for the global minimum.
 
-- `bm.set_log(True, cond, step, prefix)` - when calling this function with the `True` argument, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step and a string `prefix` for the log.
+- `bm.set_log(with_log=True, cond='min-max', step=1000, prefix='bm', with_min=True, with_max=True)` - when calling this function with the `True` argument `with_log`, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step and a string `prefix` for the log. You can also disable the display of minimum values (`with_min`) or maximum values (`with_max`).
 
-- `bm.set_cache(True)` - when calling this function with the `True` argument, the cache will be used (it is not used by default), that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can specify `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
+- `bm.set_cache(with_cache=True, cache=None, m_max=1.E+8)` - when calling this function with the `True` argument `with_cache`, the cache will be used (it is not used by default), that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can specify `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
 
-- `bm.set_quantization(True)` - an auxiliary option, when set, it is assumed that the requested multi-indices and the points are presented in a quantized representation, that is, each mode of the original grid of the size `2^q`, is converted into `q` virtual modes, having a size `2`.
+- `bm.set_quantization(with_quantization=True)` - an auxiliary option, when set, it is assumed that the requested multi-indices and the points are presented in a quantized representation, that is, each mode of the original grid of the size `2^q`, is converted into `q` virtual modes, having a size `2`.
 
 - `bm.set_opts(...)` - for some benchmarks, this function may be called to set additional benchmark-specific options (please see the description of arguments in the relevant benchmark code file).
 
 ##### Computing benchmark values
 
 Now the benchmark is ready to go, and we can calculate its value in any requested discrete multi-index (a real number will be returned) or a list of its values for any requested batch of discrete multi-indices (1D numpy array of real numbers will be returned):
 ```python
```

### Comparing `teneva_bm-0.3.0/README.md` & `teneva_bm-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,61 @@
+Metadata-Version: 2.1
+Name: teneva_bm
+Version: 0.4.0
+Summary: Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods
+Home-page: https://github.com/AndreiChertkov/teneva_bm
+Author: Andrei Chertkov
+Author-email: andre.chertkov@gmail.com
+License: MIT
+Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
+Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # teneva_bm
 
 
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.3.0".
+> Current version "0.4.0".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.2+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following command:
 
-```bash
-pip install networkx==3.0 qubogen==0.1.1 gekko==1.0.6
-```
+- Collections `func`, `hs` and `various` do not require installation of additional libraries.
+
+- Сollections `oc` and `qubo` require installation of the following libraries:
+    ```bash
+    pip install networkx==3.0 qubogen==0.1.1 gekko==1.0.6
+    ```
+
+- Сollections `agent` and `agent_toe` require a rather complicated installation process of the `mujoco` framework, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
+
+> To run benchmark optimization examples, you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
 
 
 ## Documentation and examples
 
 All benchmarks inherit from the `Bm` base class (`teneva_bm/bm.py`) and are located in the subfolders (collections of benchmarks) of `teneva_bm` folder. The corresponding python files contain a detailed description of the benchmarks, as well as a scripts for a demo run at the end of the files. You can get detailed information on the created benchmark using the `info` class method:
 ```python
 from teneva_bm import *
@@ -32,21 +65,27 @@
 
 You can run demos for all benchmarks at once with the command `python demo.py` from the root folder of the project (you can also specify the name of the benchmark as a script argument to run the demo for only one benchmark, e.g., `python demo.py bm_qubo_knap_det`). You can also use a function from the `teneva_bm` package to run all or only one demo:
 ```python
 from teneva_bm import teneva_bm_demo
 teneva_bm_demo('bm_qubo_knap_det', with_info=True)
 ```
 
-> We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/demo_base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.2`).
+> We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/demo_base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
+
+> We also present some examples [DRAFT!] in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
 
 
 ## Available benchmarks
 
+- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) is assumed. The collection includes the following benchmarks: `BmAgentSwimmer`.
+
+- `agent_toe` - the same as `agent` collection, but with optimization of the discrete Toeplitz policy. The collection includes the following benchmarks: `BmAgentToeSwimmer`.
+
 - `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
-    > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores.
+    > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores. Note also that we apply small random shift of the grid limits for all functions, to make the optimization problem more difficult (because many functions have a minimum at the center point of the domain).
 
 - `hs` (draft!) - the [Hock & Schittkowski](http://apmonitor.com/wiki/index.php/Apps/HockSchittkowski) collection of benchmark functions, containing continuous analytic functions of small dimensions (2-5), some of which have given constraints. The collection includes the following benchmarks: `BmHsFunc001`, `BmHsFunc006`.
 
 - `oc` - a collection of optimal control problems described by ordinary differential equations with discrete binary control variable, some of the problems have explicit restrictions on the elements of the control vector. The collection includes the following benchmarks: `BmOcSimple`, `BmOcSimpleConstr`.
 
 - `qubo` - a collection of quadratic unconstrained binary optimization (QUBO) problems; all benchmarks are discrete and have a mode size equals `2`. The collection includes the following benchmarks: `BmQuboKnapDet`, `BmQuboKnapQuad`, `BmQuboMaxcut`, `BmQuboMvc`.
     > The exact global minimum is known only for `BmQuboKnapDet` benchmark (note that this benchmark supports only dimensions `10`, `20`, `50`, `80` and `100`).
@@ -77,27 +116,31 @@
 - `desc` - the description of the benchmark (string). By default, a detailed description of the benchmark is used, provided in the corresponding python file.
 - `...other arguments...` - some benchmarks have additional optional arguments, which are described in the corresponding python files.
 
 ##### Setting advanced options
 
 Before calling the `bm.prep()` method, you can set a number of additional benchmark options:
 
-- `bm.set_grid_kind(kind)` - by default, we use the Chebyshev grid (`kind = 'cheb'`), but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
+- `bm.set_seed(seed=42)` - with this function we can set a custom random seed. Note that we use `Random Generator` from numpy (i.e., `numpy.random.default_rng(seed)`).
+-
+- `bm.set_grid_kind(kind='cheb')` - by default, we use the Chebyshev grid (`kind = 'cheb'`), but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
+
+- `bm.set_budget(m=None, m_cache=None, is_strict=True)` - optional method to set the computation buget `m`. If the number of requests to the benchmark (from calls to `bm.get` and `bm.get_poi` methods) exceeds the specified budget, then `None` will be returned. If the flag `is_strict` is disabled, then the request for the last batch will be allowed, after which the budget will be exceeded, otherwise this last batch will not be considered. Note that when the budget is exceeded, `None` will be returned both when requesting a single value and a batch of values. Also, in a similar way, you can set a limit on the use of the cache by `m_cache` parameter.
 
 - `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm._c`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned).
 
-- `bm.set_max(i, x, y)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks , which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
+- `bm.set_max(i=None, x=None, y=None)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks , which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
 
-- `bm.set_min(i, x, y)` - the same as in the previous point, but for the global minimum.
+- `bm.set_min(i=None, x=None, y=None)` - the same as in the previous point, but for the global minimum.
 
-- `bm.set_log(True, cond, step, prefix)` - when calling this function with the `True` argument, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step and a string `prefix` for the log.
+- `bm.set_log(with_log=True, cond='min-max', step=1000, prefix='bm', with_min=True, with_max=True)` - when calling this function with the `True` argument `with_log`, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step and a string `prefix` for the log. You can also disable the display of minimum values (`with_min`) or maximum values (`with_max`).
 
-- `bm.set_cache(True)` - when calling this function with the `True` argument, the cache will be used (it is not used by default), that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can specify `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
+- `bm.set_cache(with_cache=True, cache=None, m_max=1.E+8)` - when calling this function with the `True` argument `with_cache`, the cache will be used (it is not used by default), that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can specify `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
 
-- `bm.set_quantization(True)` - an auxiliary option, when set, it is assumed that the requested multi-indices and the points are presented in a quantized representation, that is, each mode of the original grid of the size `2^q`, is converted into `q` virtual modes, having a size `2`.
+- `bm.set_quantization(with_quantization=True)` - an auxiliary option, when set, it is assumed that the requested multi-indices and the points are presented in a quantized representation, that is, each mode of the original grid of the size `2^q`, is converted into `q` virtual modes, having a size `2`.
 
 - `bm.set_opts(...)` - for some benchmarks, this function may be called to set additional benchmark-specific options (please see the description of arguments in the relevant benchmark code file).
 
 ##### Computing benchmark values
 
 Now the benchmark is ready to go, and we can calculate its value in any requested discrete multi-index (a real number will be returned) or a list of its values for any requested batch of discrete multi-indices (1D numpy array of real numbers will be returned):
 ```python
```

### Comparing `teneva_bm-0.3.0/demo.py` & `teneva_bm-0.4.0/demo.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,8 +12,12 @@
 
 
 from teneva_bm import teneva_bm_demo
 
 
 if __name__ == '__main__':
     bm_use = sys.argv[1] if len(sys.argv) > 1 else None
-    teneva_bm_demo(bm_use, with_info=(bm_use is None))
+
+    only_info = (bm_use == 'info')
+    bm_use = None if bm_use and bm_use.lower() == 'info' else bm_use
+
+    teneva_bm_demo(bm_use, with_info=(bm_use is None), all=(not only_info))
```

### Comparing `teneva_bm-0.3.0/setup.py` & `teneva_bm-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/bm.py` & `teneva_bm-0.4.0/teneva_bm/bm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,91 +1,126 @@
 import numpy as np
 import teneva
 from time import perf_counter as tpc
 
 
+from teneva_bm import __version__
+
+
 class Bm:
     def __init__(self, d=None, n=None, name='', desc=''):
         self._init()
 
+        self.set_seed()
+
         self.set_size(d, n)
         self.set_quantization()
-
-        self.set_name(name)
-        self.set_desc(desc)
-
         self.set_constr()
 
-        self.set_min()
-        self.set_max()
-
         self.set_grid()
         self.set_grid_kind()
 
-        self.set_opts()
+        self.set_name(name)
+        self.set_desc(desc)
 
+        self.set_opts()
         self.set_cache()
+        self.set_budget()
+
+        self.set_min()
+        self.set_max()
 
         self.set_log()
 
     def __call__(self, X):
         """Return a value or batch of values for provided x-point."""
         return self.get_poi(X)
 
     def __getitem__(self, I):
         """Return a value or batch of values for provided multi-index."""
         return self.get(I)
 
     @property
+    def a0(self):
+        """Return the lower grid size value if it is constant."""
+        if not self.is_a_equal:
+            raise ValueError('Lower grid size is not constant, can`t get a0')
+        return self.a[0]
+
+    @property
+    def b0(self):
+        """Return the upper grid size value if it is constant."""
+        if not self.is_b_equal:
+            raise ValueError('Upper grid size is not constant, can`t get b0')
+        return self.b[0]
+
+    @property
+    def is_a_equal(self):
+        """Check if all the lower grid sizes are the same."""
+        v = self.list_convert(self.a, 'float')
+        return v is None or isinstance(v, (float,))
+
+    @property
+    def is_b_equal(self):
+        """Check if all the upper grid sizes are the same."""
+        v = self.list_convert(self.b, 'float')
+        return v is None or isinstance(v, (float,))
+
+    @property
     def is_func(self):
         """Check if BM relates to function (i.e., continuous function)."""
         return not self.is_tens
 
     @property
     def is_n_equal(self):
         """Check if all the mode sizes are the same."""
-        if self.n is None:
-            return True
-        return len(set(self.n)) == 1
+        v = self.list_convert(self.n, 'int')
+        return v is None or isinstance(v, (int,))
 
     @property
     def is_n_even(self):
-        """Check if all the mode sizes are even."""
+        """Check if all the mode sizes are even (2, 4, ...)."""
         if self.n is None:
             return True
         for k in self.n:
             if k % 2 == 1:
                 return False
         return True
 
     @property
     def is_n_odd(self):
-        """Check if all the mode sizes are odd."""
+        """Check if all the mode sizes are odd (1, 3, ...)."""
         return not self.is_n_even
 
     @property
     def is_tens(self):
         """Check if BM relates to tensor (i.e., discrete function)."""
         return not self.is_func
 
     @property
     def n0(self):
         """Return the mode size value if it is constant."""
         if not self.is_n_equal:
-            raise ValueError('Mode size is not constant, can not get n0')
+            raise ValueError('Mode size is not constant, can`t get n0')
         return self.n[0]
 
     @property
     def with_constr(self):
-        """Return True if benchmark has a constant."""
+        """Return True if benchmark has a constraint."""
+        return False
+
+    @property
+    def with_cores(self):
+        """Return True if exact TT-cores can be constructed for benchmark."""
         return False
 
     def build_cores(self):
         """Return exact TT-cores for the TT-representation of the tensor."""
         if self.is_tens:
+            # TODO: check why
             msg = 'Construction of the TT-cores does not work for tensors'
             raise ValueError(msg)
 
         I = np.array([teneva.grid_flat(k) for k in self.n], dtype=int).T
         X = teneva.ind_to_poi(I, self.a, self.b, self.n, self.grid_kind)
 
         return self._cores(X)
@@ -94,30 +129,38 @@
         """Generate random (from LHS) train dataset of (index, value)."""
         m = int(m)
         n = [2]*self.quantization*self.d if self.with_quantization else self.n
 
         if m < 1:
             return None, None
 
+        # TODO: add fixed random seed support
         I_trn = teneva.sample_lhs(n, m)
         y_trn = self.get(I_trn, skip_process)
 
+        if y_trn is None:
+            raise ValueError('The specified budget is exceeded')
+
         return I_trn, y_trn
 
     def build_tst(self, m=0, skip_process=True):
         """Generate random (from "choice") test dataset of (index, value)."""
         m = int(m)
         n = [2]*self.quantization*self.d if self.with_quantization else self.n
 
         if m < 1:
             return None, None
 
+        # TODO: add fixed random seed support
         I_tst = np.vstack([np.random.choice(k, m) for k in n]).T
         y_tst = self.get(I_tst, skip_process)
 
+        if y_tst is None:
+            raise ValueError('The specified budget is exceeded')
+
         return I_tst, y_tst
 
     def check(self):
         """Check that benchmark's configuration is valid."""
         if not self.is_prep:
             msg = 'Run "prep" method for BM before call it'
             self.set_err(msg)
@@ -143,72 +186,297 @@
         I, X, is_batch = self._parse_input(I=I)
 
         if self.with_cache:
             m = I.shape[0]
             ind = [k for k in range(m) if tuple(I[k]) not in self.cache]
 
             m_new = len(ind)
-            m_cache = m - m_new
+            dm_cache = m - m_new
+
+            if self.budget_m_cache:
+                if self.budget_is_strict:
+                    if self.m_cache + dm_cache > self.budget_m_cache:
+                        return None
+                else:
+                    if self.m_cache > self.budget_m_cache:
+                        return None
 
             if m_new > 0:
-                y_new = self._compute(X[ind] if self.is_func else I[ind])
+                Z = X[ind] if self.is_func else I[ind]
+                y_new = self._compute(Z, skip_process)
+                if y_new is None:
+                    return None
+
                 for k in range(m_new):
                     self.cache[tuple(I[ind[k]])] = y_new[k]
 
             y = np.array([self.cache[tuple(i)] for i in I])
 
         else:
-            m_cache = 0
+            dm_cache = 0
+
+            Z = X if self.is_func else I
+            y = self._compute(Z, skip_process)
+            if y is None:
+                return None
+
+        return self._process(I, X, y, dm_cache, t, is_batch, skip_process)
+
+    def get_config(self):
+        """Return a dict with configuration of the benchmark."""
+        conf = {
+            'd': self.d,
+            'n': self.list_convert(self.n, 'int'),
+            'seed': self.seed,
+            'name': self.name,
+            'benchmark': self.__class__.__name__,
+            'version': __version__,
+            'is_tens': self.is_tens,
+            'is_func': self.is_func,
+            'with_quantization': self.with_quantization,
+            'with_cache': self.with_cache,
+            'with_constr': self.with_constr,
+            'with_cores': self.with_cores,
+        }
+
+        if self.is_func:
+            conf['a'] = self.list_convert(self.a, 'float')
+            conf['b'] = self.list_convert(self.b, 'float')
+            conf['grid_kind'] = self.grid_kind
+
+        if self.with_constr:
+            conf['constr_penalty'] = self.constr_penalty
+            conf['constr_eps'] = self.constr_eps
+            conf['constr_with_amplitude'] = self.constr_with_amplitude
+
+        if self.budget_m:
+            conf['budget_m'] = self.budget_m
+        if self.budget_m_cache:
+            conf['budget_m_cache'] = self.budget_m_cache
+        if self.budget_m or self.budget_m_cache:
+            conf['budget_is_strict'] = self.budget_is_strict
+
+        if self.i_max_real is not None:
+            conf['i_max_real'] = self.list_convert(self.i_max_real, 'int')
+        if self.x_max_real is not None:
+            conf['x_max_real'] = self.list_convert(self.x_max_real, 'float')
+        if self.y_max_real is not None:
+            conf['y_max_real'] = self.y_max_real
+
+        if self.i_min_real is not None:
+            conf['i_min_real'] = self.list_convert(self.i_min_real, 'int')
+        if self.x_min_real is not None:
+            conf['x_min_real'] = self.list_convert(self.x_min_real, 'float')
+        if self.y_min_real is not None:
+            conf['y_min_real'] = self.y_min_real
+
+        return conf
 
-            y = self._compute(X if self.is_func else I)
+    def get_history(self):
+        """Return a dict with results of requests to the benchmark."""
+        hist = {
+            'm': self.m,
+            'm_cache': self.m_cache,
+            'i_max': self.i_max,
+            'x_max': self.x_max,
+            'y_max': self.y_max,
+            'i_min': self.i_min,
+            'x_min': self.x_min,
+            'y_min': self.y_min,
+            'y_list': self.y_list,
+            'time': self.time,
+            'time_full': tpc() - self.log_t,
+            'err': '; '.join(self.err) if len(self.err) else '',
+        }
 
-        return self._process(I, X, y, m_cache, t, is_batch, skip_process)
+        return hist
 
     def get_poi(self, X, skip_process=False):
         """Return a value or batch of values for provided x-point."""
         t = tpc()
 
         self.check()
 
         I, X, is_batch = self._parse_input(X=X)
 
-        y = self._compute(X)
+        y = self._compute(X, skip_process)
+        if y is None:
+            return None
 
         return self._process(I, X, y, 0, t, is_batch, skip_process)
 
-    def info(self):
+    def info(self, footer=''):
         """Returns a detailed description of the benchmark as text."""
         text = '-' * 78 + '\n' + 'BM: '
         text += self.name + ' ' * max(0, 36-len(self.name)) +  ' | '
-        text += f'DIMS = {self.d:-5d} | <MODE SIZE> = {np.mean(self.n):-6.1f}\n'
+        text += f'DIMS = {self.d:-4d} | '
+        n = np.mean(self.n)
+        text += '<MODE SIZE> = ' + (f'{n:-7.1f}' if n<9999 else f'{n:-7.1e}')
+        text += '\n'
+        text += '-' * 41 + '|             '
+        text += '>           Description'
+        text += '\n'
 
-        if self.y_min_real is not None or self.y_max_real is not None:
-            text += ' ' * 35
-            if self.y_min_real is not None:
-                text += f'y_min = {self.y_min_real:-12.5e} | '
-            if self.y_max_real is not None:
-                text += f'y_max = {self.y_max_real:-12.5e}'
-            text += '\n'
+        text += '.' * 78 + '\n'
+        desc = f'    {self.desc.strip()}'
+        text += desc.replace('            ', '    ')
+        text += '\n'
+        text += '.' * 78 + '\n'
+
+        text += '-' * 41 + '|            '
+        text += '>          Configuration'
+        text += '\n'
 
-        if self.desc:
-            desc = f'  [ {self.desc.strip()} ]'
-            text += '\n' + desc.replace('            ', '    ') # TODO
+        text += 'Package version                          : '
+        v = __version__
+        text += f'{v}\n'
+
+        text += 'Random seed                              : '
+        v = self.seed
+        text += f'{v}\n'
+
+        text += 'Benchmark                                : '
+        v = self.__class__.__name__
+        text += f'{v}\n'
+
+        text += 'Dimension                                : '
+        v = self.d
+        text += f'{v}\n'
+
+        text += 'Mode size                                : '
+        v = self.list_convert(self.n, 'int')
+        text += f'{v}\n'
+
+        if self.is_func:
+            text += 'Lower grid limit                         : '
+            va = self.list_convert(self.a, 'float')
+            if not isinstance(va, (int, float)) and self.d > 3:
+                va = f'[{va[0]:.2f}, {va[1]:.2f}, <...>, {va[-1]:.2f}]'
+            text += f'{va}\n'
+
+            text += 'Upper grid limit                         : '
+            vb = self.list_convert(self.b, 'float')
+            if not isinstance(vb, (int, float)) and self.d > 3:
+                vb = f'[{vb[0]:.2f}, {vb[1]:.2f}, <...>, {vb[-1]:.2f}]'
+            if isinstance(va, (int, float)) and isinstance(vb, (int, float)):
+                if va < 0 and vb > 0:
+                    vb = f'+{vb}'
+            text += f'{vb}\n'
+
+            text += 'Grid kind                                : '
+            v = self.grid_kind
+            text += f'{v}\n'
+
+        text += 'Function kind                            : '
+        v = 'discrete' if self.is_tens else 'continuous'
+        text += f'{v}\n'
+
+        text += 'With quantization                        : '
+        v = 'YES' if self.with_quantization else 'no'
+        text += f'{v}\n'
+
+        text += 'With cache                               : '
+        v = 'YES' if self.with_cache else 'no'
+        text += f'{v}\n'
+
+        text += 'With constraint                          : '
+        v = 'YES' if self.with_constr else 'no'
+        text += f'{v}\n'
+
+        text += 'With TT-cores                            : '
+        v = 'YES' if self.with_cores else 'no'
+        text += f'{v}\n'
+
+        if self.with_constr:
+            text += 'Constraint penalty                       : '
+            v = self.constr_penalty
+            text += f'{v}\n'
+
+            text += 'Constraint epsilon                       : '
+            v = self.constr_eps
+            text += f'{v}\n'
+
+            text += 'Constraint with amplitude                : '
+            v = 'YES' if self.constr_with_amplitude else 'no'
+            text += f'{v}\n'
+
+        if self.budget_m:
+            text += 'Computation budget                       : '
+            v = self.budget_m
+            text += f'{v}\n'
+
+        if self.budget_m_cache:
+            text += 'Computation budget for cache requests    : '
+            v = self.budget_m_cache
+            text += f'{v}\n'
+
+        if self.budget_m or self.budget_m_cache:
+            text += 'Computation budget is strict             : '
+            v = 'YES' if self.budget_is_strict else 'no'
+            text += f'{v}\n'
+
+        if self.i_max_real is not None:
+            text += 'Exact max (multi-index)                  : '
+            v = self.list_convert(self.i_max_real, 'int')
+            if not isinstance(v, (int, float)) and self.d > 3:
+                v = f'[{v[0]}, {v[1]}, <...>, {v[-1]}]'
+            text += f'{v}\n'
+
+        if self.x_max_real is not None:
+            text += 'Exact max (point)                        : '
+            v = self.list_convert(self.x_max_real, 'float')
+            if not isinstance(v, (int, float)) and self.d > 3:
+                v = f'[{v[0]:.2f}, {v[1]:.2f}, <...>, {v[-1]:.2f}]'
+            text += f'{v}\n'
+
+        if self.y_max_real is not None:
+            text += 'Exact max (value)                        : '
+            v = self.y_max_real
+            text += f'{v}\n'
 
-        text += '\n' + '=' * 78 + '\n'
+        if self.i_min_real is not None:
+            text += 'Exact min (multi-index)                  : '
+            v = self.list_convert(self.i_min_real, 'int')
+            if not isinstance(v, (int, float)) and self.d > 3:
+                v = f'[{v[0]}, {v[1]}, <...>, {v[-1]}]'
+            text += f'{v}\n'
+
+        if self.x_min_real is not None:
+            text += 'Exact min (point)                        : '
+            v = self.list_convert(self.x_min_real, 'float')
+            if not isinstance(v, (int, float)) and self.d > 3:
+                v = f'[{v[0]:.2f}, {v[1]:.2f}, <...>, {v[-1]:.2f}]'
+            text += f'{v}\n'
+
+        if self.y_min_real is not None:
+            text += 'Exact min (value)                        : '
+            v = self.y_min_real
+            text += f'{v}\n'
+
+        if footer:
+            text += '-' * 41 + '|             '
+            text += '>               Options'
+            text += '\n'
+            text += footer
+
+        text += '=' * 78 + '\n'
         return text
 
     def info_history(self):
         """Returns an information about the request history (text)."""
         text = ''
 
         text = '-' * 78 + '\n' + 'BM: '
         text += self.name + ' ' * max(0, 36-len(self.name)) +  ' | '
-        text += f'DIMS = {self.d:-5d} | <MODE SIZE> = {np.mean(self.n):-6.1f}\n'
-        text += '-' * 41 + '|              '
-        text += '> History of requests.'
+        text += f'DIMS = {self.d:-4d} | '
+        n = np.mean(self.n)
+        text += '<MODE SIZE> = ' + (f'{n:-7.1f}' if n<9999 else f'{n:-7.1e}')
+        text += '\n'
+        text += '-' * 41 + '|             '
+        text += '>   History of requests'
         text += '\n'
 
         if self.m == 0:
             text += '        ... history is empty ...\n'
             text += '=' * 78 + '\n'
             return text
 
@@ -217,14 +485,20 @@
 
         text += 'Number of cache uses                     : '
         text += f'{self.m_cache:-10.3e}\n'
 
         text += 'Average time of one request (sec)        : '
         text += f'{self.time/self.m:-10.3e}\n'
 
+        text += 'Total requests time (sec)                : '
+        text += f'{self.time:-10.3e}\n'
+
+        text += 'Total work time (sec)                    : '
+        text += f'{tpc() - self.log_t:-10.3e}\n'
+
         if self.y_min is not None and self.y_min_real is not None:
             text += 'Minimum (found / real)                   : '
             text += f'{self.y_min:-10.3e}   / {self.y_min_real:-10.3e}\n'
         elif self.y_min is not None:
             text += 'Minimum (found)                          : '
             text += f'{self.y_min:-10.3e}\n'
 
@@ -238,14 +512,32 @@
         elif self.y_max is not None:
             text += 'Maximum (found)                          : '
             text += f'{self.y_max:-10.3e}\n'
 
         text += '=' * 78 + '\n'
         return text
 
+    def list_convert(self, x, kind='float', eps=1.E-16):
+        """Convert list of equal values to one number and back."""
+        if x is None:
+            return None
+        if kind == 'int':
+            if isinstance(x, (int, float)):
+                return np.array([x]*self.d, dtype=int)
+            return int(x[0]) if len(set(x))==1 else np.asanyarray(x, dtype=int)
+        elif kind == 'float':
+            if isinstance(x, (int, float)):
+                return np.array([x]*self.d, dtype=float)
+            for v in x:
+                if np.abs(v - x[0]) > eps:
+                    return np.asanyarray(x, dtype=float)
+            return float(x[0])
+        else:
+            raise ValueError('Unsupported kind for list conversion')
+
     def log(self, postfix='', out=False):
         self.log_m_last = self.m
         t = tpc() - self.log_t
 
         text = ''
 
         if self.log_prefix:
@@ -254,18 +546,18 @@
         text += f'm {self.m:-7.1e}'
         if self.with_cache:
             text += f' [+ {self.m_cache:-7.1e}]'
         text += ' | '
 
         text += f't {t:-7.1e} | '
 
-        if self.log_with_min:
+        if self.log_with_min and self.y_min is not None:
             text += f'min {self.y_min:-10.3e} | '
 
-        if self.log_with_max:
+        if self.log_with_max and self.y_max is not None:
             text += f'max {self.y_max:-10.3e} | '
 
         if postfix:
             text = text + postfix
 
         if out:
             print(text)
@@ -274,19 +566,26 @@
 
     def prep(self):
         """A function with a specific benchmark preparation code."""
         # Note that when inherited, the function in the child class
         # must starts with the following line:
         self.check_err()
 
-        # and should ends with the following two lines:
+        # and it should ends with the following two lines:
         self.is_prep = True
         return self
 
+    def set_budget(self, m=None, m_cache=None, is_strict=True):
+        """Set computation buget."""
+        self.budget_m = int(m) if m else None
+        self.budget_m_cache = int(m_cache) if m_cache else None
+        self.budget_is_strict = is_strict
+
     def set_cache(self, with_cache=False, cache=None, m_max=1.E+8):
+        """Set cache options."""
         self.with_cache = with_cache
         self.cache = {} if cache is None else cache
         self.cache_m_max = int(m_max) if m_max else None
 
     def set_constr(self, penalty=1.E+42, eps=1.E-16, with_amplitude=True):
         """Set constraint options."""
         self.constr_penalty = penalty
@@ -308,16 +607,16 @@
 
     def set_grid_kind(self, kind='cheb'):
         """Set the kind of the grid ('cheb' or 'uni').
 
         Note:
             In some benchmarks, when setting the exact global optimum, it is
             used that the central multi-index for a grid with an odd number of
-            nodes lies at the origin. When new types of grids appear, this
-            point should be taken into account.
+            nodes lies at the origin. When new types of grids appear, it should
+            be taken into account.
 
         """
         self.grid_kind = kind
 
         if not self.grid_kind in ['uni', 'cheb']:
             msg = f'Invalid kind of the grid (should be "uni" or "cheb")'
             raise ValueError(msg)
@@ -331,15 +630,15 @@
         self.log_prefix = prefix
         self.log_with_min = with_min
         self.log_with_max = with_max
 
         self.log_t = tpc()
 
         if not self.log_cond in ['min', 'max', 'min-max', 'step']:
-            raise ValueError('Invalid "log_cond" argument')
+            raise ValueError(f'Invalid "log_cond" argument "{self.log_cond}"')
 
     def set_max(self, i=None, x=None, y=None):
         """Set exact (real) global maximum (index, point and related value)."""
         self.i_max_real = i
         self.x_max_real = x
         self.y_max_real = y
 
@@ -364,59 +663,79 @@
             self.y_min_real = float(self.y_min_real)
 
     def set_name(self, name=''):
         """Set display name for the problem."""
         self.name = name
 
     def set_opts(self):
-        """Setting options specific to the benchmark."""
+        """Set options specific to the benchmark."""
         return
 
     def set_quantization(self, with_quantization=False):
+        """Set quantization usage."""
         self.with_quantization = with_quantization
 
         if not self.with_quantization:
             self.quantization = None
             return
 
         if not self.is_n_equal:
             msg = 'Quantization now works only if all mode sizes are equal'
             raise NotImplementedError(msg)
 
-        n = self.n[0]
+        n = self.n0
         self.quantization = int(np.log2(n))
         if 2**self.quantization != n:
             msg = 'Invalid mode size for quantization '
             msg += '(it should be a power of two)'
             raise ValueError(msg)
 
+    def set_seed(self, seed=42):
+        self.seed = seed
+        self.rand = np.random.default_rng(self.seed)
+
     def set_size(self, d=None, n=None):
         """Set dimension (d) and sizes for all d-modes (n: int or list)."""
         self.d = None if d is None else int(d)
         self.n = teneva.grid_prep_opt(n, self.d, int)
 
+    def shift_grid(self, scale=25):
+        """Apply random shift for the grid limits."""
+        shift = self.rand.normal(size=self.d) / scale
+        self.a = self.a - (self.b-self.a) * shift
+        self.b = self.b + (self.b-self.a) * shift
+
     def _c(self, x):
         """Function that check constraint for a given point/index."""
-        return self._c_batch(np.array(x).reshape(1, -1))[0]
+        return self._c_batch(x.reshape(1, -1))[0]
 
     def _c_batch(self, X):
         """Function that check constraint for a given batch of poi./indices."""
         return np.array([self._c(x) for x in X])
 
-    def _compute(self, X):
+    def _compute(self, X, skip_process=False):
+        m = self.m
+        m_cur = X.shape[0]
+        m_max = self.budget_m
+
+        if not skip_process and m_max:
+            if (m >= m_max) or (m + m_cur > m_max and self.budget_is_strict):
+                return None
+
         if not self.with_constr:
             return self._f_batch(X)
 
         y = np.ones(X.shape[0]) * self.constr_penalty
+
         c = self._c_batch(X)
-        ind = c < self.constr_eps
+        ind_good = c < self.constr_eps
 
-        y[ind] = self._f_batch(X[ind])
+        y[ind_good] = self._f_batch(X[ind_good])
         if self.constr_with_amplitude:
-            y[~ind] *= c[~ind]
+            y[~ind_good] *= c[~ind_good]
 
         return y
 
     def _cores(self, X):
         """Return the exact TT-cores for the provided points."""
         raise NotImplementedError()
 
@@ -438,15 +757,15 @@
 
     def _cores_mul(self, X):
         """Helper function for the construction of the TT-cores."""
         return [x[None, :, None] for x in X]
 
     def _f(self, x):
         """Function that computes value for a given point/index."""
-        return self._f_batch(np.array(x).reshape(1, -1))[0]
+        return self._f_batch(x.reshape(1, -1))[0]
 
     def _f_batch(self, X):
         """Function that computes values for a given batch of points/indices."""
         return np.array([self._f(x) for x in X])
 
     def _init(self):
         self.err = []
@@ -466,15 +785,14 @@
         self.m = 0
         self.m_cache = 0
         self.time = 0.
 
         self.log_m_last = 0
 
         self.is_prep = False
-        self.with_cores = False
 
     def _log_check(self):
         if not self.with_log:
             return False
 
         if self.log_cond == 'min':
             return self.is_y_min_new
@@ -482,22 +800,22 @@
         if self.log_cond == 'max':
             return self.is_y_max_new
 
         if self.log_cond == 'min-max':
             return self.is_y_min_new or self.is_y_max_new
 
         if self.log_cond == 'step':
-            return self.log_step and self.m - self.log_m_last > self.log_step
+            return self.log_step and self.m - self.log_m_last >= self.log_step
 
     def _parse_input(self, I=None, X=None):
         if I is not None and X is not None:
-            raise ValueError('Invalid case')
+            raise ValueError('Can`t parse input. Invalid case')
 
         if I is None and X is None:
-            raise ValueError('Invalid case')
+            raise ValueError('Can`t parse input. Invalid case')
 
         if X is not None and self.is_tens:
             msg = f'BM "{self.name}" is a tensor. '
             msg += 'Can`t compute it in the point'
             raise ValueError(msg)
 
         if I is not None:
```

### Comparing `teneva_bm-0.3.0/teneva_bm/func/__init__.py` & `teneva_bm-0.4.0/teneva_bm/func/__init__.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/func/bm_func_ackley.py` & `teneva_bm-0.4.0/teneva_bm/func/bm_func_dixon.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,88 +2,66 @@
 import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Analytical Ackley function (continuous).
+    Analytical Dixon function (continuous).
     The dimension and mode size may be any (default are d=50, n=15).
-    Default grid limits are [-32.768, 32.768]; the exact global minimum
-    is known: x = [0, ..., 0], y = 0.
-    See https://www.sfu.ca/~ssurjano/ackley.html for details.
+    Default grid limits are [-10, 10]; the exact global minimum
+    is known: x_i = 2^{(2^i-2) / 2^i} (i = 1, ..., d), y = 0.  Note that
+    this function achieves a global minimum at more than one point.
+    See https://www.sfu.ca/~ssurjano/dixonpr.html for details.
     See also the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
-    ("1. Ackley 1 Function"; Continuous, Differentiable, Non-separable,
-    Scalable, Multimodal).
+    ("48. Dixon & Price Function"; Continuous, Differentiable,
+    Non-Separable, Scalable, Unimodal).
 """
 
 
-class BmFuncAckley(Bm):
-    def __init__(self, d=50, n=15, name='FuncAckley', desc=DESC):
+class BmFuncDixon(Bm):
+    def __init__(self, d=50, n=15, name='FuncDixon', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        self.set_grid(-32.768, +32.768)
-
-        self.set_min(
-            i=np.array((self.n-1)/2, dtype=int) if self.is_n_odd else None,
-            x=[0.]*self.d,
-            y=0.)
+        self.set_grid(-10., +10.)
+        self.shift_grid()
+        
+        x_min = [1.]
+        for _ in range(d-1): # TODO: check this formula one more time:
+            x_min.append(np.sqrt(x_min[-1]/2.))
+        self.set_min(x=np.array(x_min), y=0.)
 
     @property
     def is_func(self):
         return True
 
-    def set_opts(self, a=20., b=0.2, c=2.*np.pi):
-        """Setting options specific to this benchmark.
-
-        Args:
-            a (float): parameter of the function.
-            b (float): parameter of the function.
-            c (float): parameter of the function.
-
-        """
-        self.opt_a = a
-        self.opt_b = b
-        self.opt_c = c
-
     def _f_batch(self, X):
-        y1 = np.sqrt(np.sum(X**2, axis=1) / self.d)
-        y1 = -self.opt_a * np.exp(-self.opt_b * y1)
-
-        y2 = np.sum(np.cos(self.opt_c * X), axis=1)
-        y2 = -np.exp(y2 / self.d)
+        y1 = (X[:, 0] - 1)**2
 
-        y3 = self.opt_a + np.exp(1.)
+        y2 = np.arange(2, self.d+1) * (2. * X[:, 1:]**2 - X[:, :-1])**2
+        y2 = np.sum(y2, axis=1)
 
-        return y1 + y2 + y3
+        return y1 + y2
 
     def _f_pt(self, x):
         """Draft."""
         d = torch.tensor(self.d)
-        par_a = torch.tensor(self.opt_a)
-        par_b = torch.tensor(self.opt_b)
-        par_c = torch.tensor(self.opt_c)
-
-        y1 = torch.sqrt(torch.sum(x**2) / d)
-        y1 = - par_a * torch.exp(-par_b * y1)
-
-        y2 = torch.sum(torch.cos(par_c * x))
-        y2 = - torch.exp(y2 / d)
-
-        y3 = par_a + torch.exp(torch.tensor(1.))
 
-        return y1 + y2 + y3
+        y1 = (x[0] - 1)**2
+        y2 = torch.arange(2, d+1) * (2. * x[1:]**2 - x[:-1])**2
+        y2 = torch.sum(y2)
+        return y1 + y2
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmFuncAckley().prep()
+    bm = BmFuncDixon().prep()
     print(bm.info())
 
     I_trn, y_trn = bm.build_trn(1.E+4)
     print(bm.info_history())
 
     text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
```

### Comparing `teneva_bm-0.3.0/teneva_bm/func/bm_func_alpine.py` & `teneva_bm-0.4.0/teneva_bm/func/bm_func_alpine.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
 
 class BmFuncAlpine(Bm):
     def __init__(self, d=50, n=15, name='FuncAlpine', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(-10., +10.)
+        self.shift_grid()
 
-        self.set_min(
-            i=np.array((self.n-1)/2, dtype=int) if self.is_n_odd else None,
-            x=[0.]*self.d,
-            y=0.)
-
-        self.with_cores = True
+        self.set_min(x=[0.]*self.d, y=0.)
 
     @property
     def is_func(self):
         return True
 
+    @property
+    def with_cores(self):
+        return True
+
     def _cores(self, X):
         return self._cores_add([np.abs(x * (np.sin(x) + 0.1)) for x in X.T])
 
     def _f_batch(self, X):
         return np.sum(np.abs(X * np.sin(X) + 0.1 * X), axis=1)
 
     def _f_pt(self, x):
```

### Comparing `teneva_bm-0.3.0/teneva_bm/func/bm_func_dixon.py` & `teneva_bm-0.4.0/teneva_bm/func/bm_func_schaffer.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,65 +2,55 @@
 import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Analytical Dixon function (continuous).
+    Analytical Schaffer function (continuous).
     The dimension and mode size may be any (default are d=50, n=15).
-    Default grid limits are [-10, 10]; the exact global minimum
-    is known: x_i = 2^{(2^i-2) / 2^i} (i = 1, ..., d), y = 0.  Note that
-    this function achieves a global minimum at more than one point.
-    See https://www.sfu.ca/~ssurjano/dixonpr.html for details.
-    See also the work Momin Jamil, Xin-She Yang. "A literature survey of
+    Default grid limits are [-100, 100]; the exact global minimum
+    is known: x = [0, ..., 0], y = 0.
+    See the work Momin Jamil, Xin-She Yang. "A literature survey of
     benchmark functions for global optimization problems". Journal of
     Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
-    ("48. Dixon & Price Function"; Continuous, Differentiable,
-    Non-Separable, Scalable, Unimodal).
+    ("136. Schaffer F6 Function"; Continuous, Differentiable,
+    Non-Separable, Scalable, Multimodal).
 """
 
 
-class BmFuncDixon(Bm):
-    def __init__(self, d=50, n=15, name='FuncDixon', desc=DESC):
+class BmFuncSchaffer(Bm):
+    def __init__(self, d=50, n=15, name='FuncSchaffer', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        self.set_grid(-10., +10.)
+        self.set_grid(-100., +100.)
+        self.shift_grid()
 
-        x_min = [1.]
-        for _ in range(d-1): # TODO: check this formula one more time:
-            x_min.append(np.sqrt(x_min[-1]/2.))
-        self.set_min(x=np.array(x_min), y=0.)
+        self.set_min(x=[0.]*self.d, y=0.)
 
     @property
     def is_func(self):
         return True
 
     def _f_batch(self, X):
-        y1 = (X[:, 0] - 1)**2
-
-        y2 = np.arange(2, self.d+1) * (2. * X[:, 1:]**2 - X[:, :-1])**2
-        y2 = np.sum(y2, axis=1)
-
-        return y1 + y2
+        Z = X[:, :-1]**2 + X[:, 1:]**2
+        Y = 0.5 + (np.sin(np.sqrt(Z))**2 - 0.5) / (1. + 0.001 * Z)**2
+        return np.sum(Y, axis=1)
 
     def _f_pt(self, x):
         """Draft."""
-        d = torch.tensor(self.d)
-
-        y1 = (x[0] - 1)**2
-        y2 = torch.arange(2, d+1) * (2. * x[1:]**2 - x[:-1])**2
-        y2 = torch.sum(y2)
-        return y1 + y2
+        z = x[:-1]**2 + x[1:]**2
+        y = 0.5 + (torch.sin(torch.sqrt(z))**2 - 0.5) / (1. + 0.001 * z)**2
+        return torch.sum(y)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmFuncDixon().prep()
+    bm = BmFuncSchaffer().prep()
     print(bm.info())
 
     I_trn, y_trn = bm.build_trn(1.E+4)
     print(bm.info_history())
 
     text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
```

### Comparing `teneva_bm-0.3.0/teneva_bm/func/bm_func_exp.py` & `teneva_bm-0.4.0/teneva_bm/func/bm_func_exp.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
 
 class BmFuncExp(Bm):
     def __init__(self, d=50, n=15, name='FuncExp', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(-1., +1.)
+        self.shift_grid()
 
-        self.set_min(
-            i=np.array((self.n-1)/2, dtype=int) if self.is_n_odd else None,
-            x=[0.]*self.d,
-            y=-1.)
-
-        self.with_cores = True
+        self.set_min(x=[0.]*self.d, y=-1.)
 
     @property
     def is_func(self):
         return True
 
+    @property
+    def with_cores(self):
+        return True
+
     def _cores(self, X):
         Y = self._cores_mul([np.exp(-0.5 * x**2) for x in X.T])
         Y[-1] *= -1.
         return Y
 
     def _f_batch(self, X):
         return -np.exp(-0.5 * np.sum(X**2, axis=1))
```

### Comparing `teneva_bm-0.3.0/teneva_bm/func/bm_func_griewank.py` & `teneva_bm-0.4.0/teneva_bm/func/bm_func_griewank.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 
 
 class BmFuncGriewank(Bm):
     def __init__(self, d=50, n=15, name='FuncGriewank', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(-100., +100.)
+        self.shift_grid()
 
-        self.set_min(
-            i=np.array((self.n-1)/2, dtype=int) if self.is_n_odd else None,
-            x=[0.]*self.d,
-            y=0.)
-
-        self.with_cores = True
+        self.set_min(x=[0.]*self.d, y=0.)
 
     @property
     def is_func(self):
         return True
 
+    @property
+    def with_cores(self):
+        return True
+
     def _cores(self, X):
         Y = self._cores_mul([np.cos(x/np.sqrt(i)) for i,x in enumerate(X.T,1)])
         Y[-1] *= -1
         return teneva.add(Y, self._cores_add([x**2 / 4000. for x in X.T], a0=1))
 
     def _f_batch(self, X):
         y1 = np.sum(X**2, axis=1) / 4000
```

### Comparing `teneva_bm-0.3.0/teneva_bm/func/bm_func_michalewicz.py` & `teneva_bm-0.4.0/teneva_bm/func/bm_func_michalewicz.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,28 +22,45 @@
 
 
 class BmFuncMichalewicz(Bm):
     def __init__(self, d=50, n=15, name='FuncMichalewicz', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(0., np.pi)
+        self.shift_grid()
 
         if self.d == 2:
             self.set_min(x=[2.20, 1.57], y=-1.8013)
         if self.d == 5:
             self.set_min(y=-4.687658)
         if self.d == 10:
             self.set_min(y=-9.66015)
 
-        self.with_cores = True
-
     @property
     def is_func(self):
         return True
 
+    @property
+    def with_cores(self):
+        return True
+
+    def get_config(self):
+        conf = super().get_config()
+        conf['opt_m'] = self.opt_m
+        return conf
+
+    def info(self, footer=''):
+        text = ''
+
+        text += 'Param m for Michalewicz function         : '
+        v = self.opt_m
+        text += f'{v:.6f}\n'
+
+        return super().info(text+footer)
+
     def set_opts(self, m=10.):
         """Setting options specific to this benchmark.
 
         Args:
             m (float): parameter of the function.
 
         """
```

### Comparing `teneva_bm-0.3.0/teneva_bm/func/bm_func_piston.py` & `teneva_bm-0.4.0/teneva_bm/func/bm_func_piston.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
         if self.d != 7:
             self.set_err('Dimension should be "7"')
 
         self.set_grid(
             [30., 0.005, 0.002, 1000,  90000, 290, 340],
             [60., 0.020, 0.010, 5000, 110000, 296, 360])
+        self.shift_grid()
 
     @property
     def is_func(self):
         return True
 
     def _f_batch(self, X):
         _M  = X[:, 0]
```

### Comparing `teneva_bm-0.3.0/teneva_bm/func/bm_func_qing.py` & `teneva_bm-0.4.0/teneva_bm/func/bm_func_qing.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,25 +23,26 @@
 
 
 class BmFuncQing(Bm):
     def __init__(self, d=50, n=15, name='FuncQing', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(0., +500.)
+        self.shift_grid()
 
-        self.set_min(
-            x=np.sqrt(np.arange(1, self.d+1)),
-            y=0.)
-
-        self.with_cores = True
+        self.set_min(x=np.sqrt(np.arange(1, self.d+1)), y=0.)
 
     @property
     def is_func(self):
         return True
 
+    @property
+    def with_cores(self):
+        return True
+
     def _cores(self, X):
         return self._cores_add([(x**2 - i)**2 for i, x in enumerate(X.T, 1)])
 
     def _f_batch(self, X):
         return np.sum((X**2 - np.arange(1, self.d+1))**2, axis=1)
 
     def _f_pt(self, x):
```

### Comparing `teneva_bm-0.3.0/teneva_bm/func/bm_func_rastrigin.py` & `teneva_bm-0.4.0/teneva_bm/func/bm_func_rastrigin.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,26 +20,40 @@
 
 
 class BmFuncRastrigin(Bm):
     def __init__(self, d=50, n=15, name='FuncRastrigin', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(-5.12, +5.12)
+        self.shift_grid()
 
-        self.set_min(
-            i=np.array((self.n-1)/2, dtype=int) if self.is_n_odd else None,
-            x=[0.]*self.d,
-            y=0.)
-
-        self.with_cores = True
+        self.set_min(x=[0.]*self.d, y=0.)
 
     @property
     def is_func(self):
         return True
 
+    @property
+    def with_cores(self):
+        return True
+
+    def get_config(self):
+        conf = super().get_config()
+        conf['opt_A'] = self.opt_A
+        return conf
+
+    def info(self, footer=''):
+        text = ''
+
+        text += 'Param A for Rastrigin function           : '
+        v = self.opt_A
+        text += f'{v:.6f}\n'
+
+        return super().info(text+footer)
+
     def set_opts(self, A=10.):
         """Setting options specific to this benchmark.
 
         Args:
             A (float): parameter of the function.
 
         """
```

### Comparing `teneva_bm-0.3.0/teneva_bm/func/bm_func_rosenbrock.py` & `teneva_bm-0.4.0/teneva_bm/func/bm_func_rosenbrock.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,23 +22,26 @@
 
 
 class BmFuncRosenbrock(Bm):
     def __init__(self, d=50, n=15, name='FuncRosenbrock', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(-2.048, +2.048)
+        self.shift_grid()
 
         self.set_min(x=[1.]*self.d, y=0.)
 
-        self.with_cores = True
-
     @property
     def is_func(self):
         return True
 
+    @property
+    def with_cores(self):
+        return True
+
     def _cores(self, X):
         Y = []
         for i, x in enumerate(X.T):
             x2 = x*x
             if i == 0:
                 G = np.zeros([1, len(x), 3])
                 G[0, :, 0] = 1
```

### Comparing `teneva_bm-0.3.0/teneva_bm/func/bm_func_schaffer.py` & `teneva_bm-0.4.0/teneva_bm/various/bm_wall_simple.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,57 +2,47 @@
 import teneva
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Analytical Schaffer function (continuous).
-    The dimension and mode size may be any (default are d=50, n=15).
-    Default grid limits are [-100, 100]; the exact global minimum
-    is known: x = [0, ..., 0], y = 0.
-    See the work Momin Jamil, Xin-She Yang. "A literature survey of
-    benchmark functions for global optimization problems". Journal of
-    Mathematical Modelling and Numerical Optimisation 2013; 4:150-194
-    ("136. Schaffer F6 Function"; Continuous, Differentiable,
-    Non-Separable, Scalable, Multimodal).
+    Simple example of the special discrete function ("wall"), which is
+    difficult to optimize by tensor methods. The exact global minimum
+    is known: i = [0, ..., 0], y = 0. The target function returns "0" if
+    the requested multi-index is optimal; returns a large number ("10 * d")
+    if the requested multi-index matches the optimal one in at least one
+    element; and returns the first element of the multi-index otherwise.
+    The dimension and mode size may be any (default are d=10, n=50).
 """
 
 
-class BmFuncSchaffer(Bm):
-    def __init__(self, d=50, n=15, name='FuncSchaffer', desc=DESC):
+class BmWallSimple(Bm):
+    def __init__(self, d=10, n=50, name='WallSimple', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        self.set_grid(-100., +100.)
-
-        self.set_min(
-            i=np.array((self.n-1)/2, dtype=int) if self.is_n_odd else None,
-            x=[0.]*self.d,
-            y=0.)
+        self.set_min(i=[0]*self.d, y=0.)
 
     @property
-    def is_func(self):
+    def is_tens(self):
         return True
 
-    def _f_batch(self, X):
-        Z = X[:, :-1]**2 + X[:, 1:]**2
-        Y = 0.5 + (np.sin(np.sqrt(Z))**2 - 0.5) / (1. + 0.001 * Z)**2
-        return np.sum(Y, axis=1)
-
-    def _f_pt(self, x):
-        """Draft."""
-        z = x[:-1]**2 + x[1:]**2
-        y = 0.5 + (torch.sin(torch.sqrt(z))**2 - 0.5) / (1. + 0.001 * z)**2
-        return torch.sum(y)
+    def _f(self, i):
+        if len(np.where(i == self.i_min_real)[0]) == self.d:
+            return 0.
+        elif len(np.where(i == self.i_min_real)[0]) > 0:
+            return self.d * 10
+        else:
+            return i[0]
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmFuncSchaffer().prep()
+    bm = BmWallSimple().prep()
     print(bm.info())
 
     I_trn, y_trn = bm.build_trn(1.E+4)
     print(bm.info_history())
 
     text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
@@ -67,10 +57,10 @@
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
     text = 'Value at the minimum (real vs calc)      :  '
     y_real = bm.y_min_real
-    y_calc = bm(bm.x_min_real)
+    y_calc = bm[bm.i_min_real]
     text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.3.0/teneva_bm/func/bm_func_schwefel.py` & `teneva_bm-0.4.0/teneva_bm/func/bm_func_schwefel.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,23 +22,40 @@
 
 
 class BmFuncSchwefel(Bm):
     def __init__(self, d=50, n=15, name='FuncSchwefel', desc=DESC):
         super().__init__(d, n, name, desc)
 
         self.set_grid(-500., +500.)
+        self.shift_grid()
 
         self.set_min(x=[420.9687]*self.d, y=0.)
 
-        self.with_cores = True
-
     @property
     def is_func(self):
         return True
 
+    @property
+    def with_cores(self):
+        return True
+
+    def get_config(self):
+        conf = super().get_config()
+        conf['opt_a'] = self.opt_a
+        return conf
+
+    def info(self, footer=''):
+        text = ''
+
+        text += 'Param a for Schwefel function            : '
+        v = self.opt_a
+        text += f'{v:.6f}\n'
+
+        return super().info(text+footer)
+
     def set_opts(self, a=418.9829):
         """Setting options specific to this benchmark.
 
         Args:
             a (float): parameter of the function.
 
         """
```

### Comparing `teneva_bm-0.3.0/teneva_bm/hs/bm_hs_func001.py` & `teneva_bm-0.4.0/teneva_bm/hs/bm_hs_func001.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/hs/bm_hs_func006.py` & `teneva_bm-0.4.0/teneva_bm/hs/bm_hs_func006.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs007.py` & `teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs007.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs008.py` & `teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs008.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs009.py` & `teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs009.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs010.py` & `teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs010.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs011.py` & `teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs011.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/hs/draft_constrained_functions/bm_hs012.py` & `teneva_bm-0.4.0/teneva_bm/hs/draft_constrained_functions/bm_hs012.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py` & `teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py` & `teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py` & `teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py` & `teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py` & `teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py` & `teneva_bm-0.4.0/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/oc/bm_oc_simple.py` & `teneva_bm-0.4.0/teneva_bm/qubo/bm_qubo_mvc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,110 +1,113 @@
 import numpy as np
 import teneva
 
 
 try:
-    from gekko import GEKKO
-    with_gekko = True
+    import networkx as nx
+    with_networkx = True
 except Exception as e:
-    with_gekko = False
+    with_networkx = False
+
+
+try:
+    import qubogen
+    with_qubogen = True
+except Exception as e:
+    with_qubogen = False
 
 
 from teneva_bm import Bm
 
 
 DESC = """
-    Discrete optimal control (OC) problem with simple 1D ODE "x**3 - i",
-    where "x = x(t)" is a state variable, "x(0) = x_ini" and "i" is a
-    binary control variable. The loss function for the optimal control
-    problem is "0.5 * (x-x_ref)^2", where "x_ref" is a target value, and
-    the maximum time value is "t_max". Note that for some control values
-    the solver (gekko) fails, in this case we return the value "y_err".
-    By default (see parameters of the "set_opts" function), "x_ini = 0.8",
-    "x_ref = 0.7", "t_max = 1" and "y_err = 1.E+50".
+    Quadratic unconstrained binary optimization (QUBO) Minimum Vertex Cover
+    (MVC) problem represented as a discrete function.
     The dimension may be any (default is 50), and the mode size should be 2.
-    The benchmark needs "gekko==1.0.6" library (it is used for ODE solution).
+    The benchmark needs "networkx==3.0" and "qubogen==0.1.1" libraries.
 """
 
 
-class BmOcSimple(Bm):
-    def __init__(self, d=50, n=2, name='OcSimple', desc=DESC):
+class BmQuboMvc(Bm):
+    def __init__(self, d=50, n=2, name='QuboMVC', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        if not self.is_n_equal or self.n[0] != 2:
+        if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
-        if not with_gekko:
-            msg = 'Need "gekko" module. For installation please run '
-            msg += '"pip install gekko==1.0.6"'
+        if not with_networkx:
+            msg = 'Need "networkx" module. For installation please run '
+            msg += '"pip install networkx==3.0"'
+            self.set_err(msg)
+        if not with_qubogen:
+            msg = 'Need "qubogen" module. For installation please run '
+            msg += '"pip install qubogen==0.1.1"'
             self.set_err(msg)
 
     @property
     def is_tens(self):
         return True
 
-    def bm_ode(self, x, i):
-        """Target ordinary differential equation (ODE)."""
-        return x**3 - i
-
-    def bm_obj(self, x, i):
-        """Objective function for ODE solution."""
-        return 0.5 * (x - self.opt_x_ref)**2
+    def get_config(self):
+        conf = super().get_config()
+        conf['opt_prob_con'] = self.opt_prob_con
+        return conf
+
+    def info(self, footer=''):
+        text = ''
+
+        text += 'Param prob_con (connection probability)  : '
+        v = self.opt_prob_con
+        text += f'{v:.6f}\n'
+
+        return super().info(text+footer)
+
+    def prep(self):
+        self.check_err()
+
+        d = self.d
+        p = self.opt_prob_con
+        graph = nx.fast_gnp_random_graph(n=d, p=p, seed=self.seed)
+        edges = np.array(list([list(e) for e in graph.edges]))
+        n_nodes = len(np.unique(np.array(edges).flatten()))
+
+        g = qubogen.Graph(edges=edges, n_nodes=n_nodes)
+        self.bm_Q = qubogen.qubo_mvc(g)
+
+        self.is_prep = True
+        return self
 
-    def set_opts(self, x_ini=0.8, x_ref=0.7, t_max=1., y_err=1.E+50):
+    def set_opts(self, prob_con=0.5):
         """Setting options specific to the benchmark.
 
         Args:
-            x_ini (float): initial condition for the ODE.
-            x_ref (float): target (reference) value for solution of the ODE.
-            t_max (float): upper limit for time variable in the ODE.
-            y_err (float): returned value if GEKKO solver ends with error.
+            prob_con (float): probability of the connection in the graph.
 
         """
-        self.opt_x_ini = x_ini
-        self.opt_x_ref = x_ref
-        self.opt_times = np.linspace(0, t_max, self.d)
-        self.opt_y_err = y_err
-
-    def _f(self, i):
-        solver = GEKKO(remote=False)
-        solver.options.IMODE = 4
-        solver.time = self.opt_times
-
-        x = solver.Var(value=self.opt_x_ini, name='x')
-        c = solver.Param(list(i), name='i')
-        y = solver.Var(value=0.)
-
-        solver.Equation(x.dt() == self.bm_ode(x, c))
-        solver.Equation(y == self.bm_obj(x, c))
-
-        try:
-            solver.solve(disp=False)
-            y = sum(y.VALUE)
-        except Exception as e:
-            y = self.opt_y_err
+        self.opt_prob_con = prob_con
 
-        return y
+    def _f_batch(self, I):
+        return ((I @ self.bm_Q) * I).sum(axis=1)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
 
-    bm = BmOcSimple().prep()
+    bm = BmQuboMvc().prep()
     print(bm.info())
 
-    I_trn, y_trn = bm.build_trn(1.E+2)
+    I_trn, y_trn = bm.build_trn(1.E+4)
     print(bm.info_history())
 
-    text = 'Value at a random multi-index     :  '
+    text = 'Value at a random multi-index            :  '
     i = [np.random.choice(k) for k in bm.n]
     y = bm[i]
     text += f'{y:-10.3e}'
     print(text)
 
-    text = 'Value at 3 random multi-indices   :  '
+    text = 'Value at 3 random multi-indices          :  '
     i1 = [np.random.choice(k) for k in bm.n]
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
```

### Comparing `teneva_bm-0.3.0/teneva_bm/oc/bm_oc_simple_constr.py` & `teneva_bm-0.4.0/teneva_bm/oc/bm_oc_simple_constr.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/qubo/bm_qubo_knap_det.py` & `teneva_bm-0.4.0/teneva_bm/qubo/bm_qubo_knap_det.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.3.0/teneva_bm/qubo/bm_qubo_knap_quad.py` & `teneva_bm-0.4.0/teneva_bm/qubo/bm_qubo_knap_quad.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 """
 
 
 class BmQuboKnapQuad(Bm):
     def __init__(self, d=50, n=2, name='QuboKnapQuad', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        if not self.is_n_equal or self.n[0] != 2:
+        if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
         if not with_qubogen:
             msg = 'Need "qubogen" module. For installation please run '
             msg += '"pip install qubogen==0.1.1"'
             self.set_err(msg)
 
     @property
     def is_tens(self):
         return True
 
     def prep(self):
         self.check_err()
 
-        v = np.diag(np.random.random(self.d)) / 3.
-        a = np.random.random(self.d)
+        v = np.diag(self.rand.random(self.d)) / 3.
+        a = self.rand.random(self.d)
         b = np.mean(a)
         self.bm_Q = qubogen.qubo_qkp(v, a, b)
 
         self.is_prep = True
         return self
 
     def _f_batch(self, I):
```

### Comparing `teneva_bm-0.3.0/teneva_bm/qubo/bm_qubo_maxcut.py` & `teneva_bm-0.4.0/teneva_bm/qubo/bm_qubo_maxcut.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,53 +27,66 @@
 """
 
 
 class BmQuboMaxcut(Bm):
     def __init__(self, d=50, n=2, name='QuboMaxcut', desc=DESC):
         super().__init__(d, n, name, desc)
 
-        if not self.is_n_equal or self.n[0] != 2:
+        if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
         if not with_networkx:
             msg = 'Need "networkx" module. For installation please run '
             msg += '"pip install networkx==3.0"'
             self.set_err(msg)
         if not with_qubogen:
             msg = 'Need "qubogen" module. For installation please run '
             msg += '"pip install qubogen==0.1.1"'
             self.set_err(msg)
 
     @property
     def is_tens(self):
         return True
 
+    def get_config(self):
+        conf = super().get_config()
+        conf['opt_prob_con'] = self.opt_prob_con
+        return conf
+
+    def info(self, footer=''):
+        text = ''
+
+        text += 'Param prob_con (connection probability)  : '
+        v = self.opt_prob_con
+        text += f'{v:.6f}\n'
+
+        return super().info(text+footer)
+
     def prep(self):
         self.check_err()
 
-        graph = nx.fast_gnp_random_graph(n=self.d,
-            p=self.opt_prob_con, seed=self.opt_seed)
+        d = self.d
+        p = self.opt_prob_con
+        graph = nx.fast_gnp_random_graph(n=d, p=p, seed=self.seed)
         edges = np.array(list([list(e) for e in graph.edges]))
         n_nodes = len(np.unique(np.array(edges).flatten()))
 
         g = qubogen.Graph(edges=edges, n_nodes=n_nodes)
         self.bm_Q = qubogen.qubo_max_cut(g)
 
         self.is_prep = True
         return self
 
-    def set_opts(self, prob_con=0.5, seed=42):
+    def set_opts(self, prob_con=0.5):
         """Setting options specific to the benchmark.
 
         Args:
             prob_con (float): probability of the connection in the graph.
-            seed (int): seed for the random graph.
 
         """
         self.opt_prob_con = prob_con
-        self.opt_seed = seed
 
     def _f_batch(self, I):
         return ((I @ self.bm_Q) * I).sum(axis=1)
 
 
 if __name__ == '__main__':
     np.random.seed(42)
```

### Comparing `teneva_bm-0.3.0/teneva_bm/teneva_bm_demo.py` & `teneva_bm-0.4.0/teneva_bm/teneva_bm_demo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 import os
 import re
 import subprocess
 
 
-def teneva_bm_demo(bm_use=None, with_info=True):
+def teneva_bm_demo(bm_use=None, with_info=True, all=False):
     """Demo script for teneva_bm.
 
     Run demo for all existing benchmarks (if "bm_use" is None) or for a
     specific benchmark (if "bm_use" is provided; e.g., "bm_qubo_knap_amba"). If
     the flag "with_info" is set, then the stats for existing collections and
     benchmarks will be also printed. Note that the code for the demo run of
     benchmarks should be at the end of the corresponding benchmark file in the
     section "if __name__ == '__main__':".
 
     """
     bms = {}
     found = False
 
+    if bm_use:
+        all = False
+
     bm_use = _parse_bm_name(bm_use)
 
     for cl in _find_cl_all():
         bms[cl] = _find_bm_all(cl)
         if bm_use in bms[cl]:
             found = True
 
     if with_info:
         _info(bms)
 
+    if not bm_use and not all:
+        return
+
     if bm_use and not found:
         msg = f'Benchmark "{bm_use}" does not exist. '
         msg += 'Can not run demo'
         raise ValueError(msg)
 
     _run_all(bms, bm_use)
 
@@ -38,15 +44,15 @@
 def _find_bm_all(cl):
     """Collect all existing benchmark names for the provided collection name."""
     bms = []
     here = os.path.abspath(os.path.dirname(__file__))
     with open(f'{here}/{cl}/__init__.py', encoding='utf-8') as f:
         lines = f.readlines()
     for l in lines:
-        if 'from .' in l and ' import ' in l and l[0] != '#':
+        if 'from .bm_' in l and ' import ' in l and l[0] != '#':
             bms.append(l.split('from .')[1].split(' import')[0])
     return bms
 
 
 def _find_cl_all():
     """Collect all existing collection names."""
     cls = []
@@ -59,18 +65,19 @@
     return cls
 
 
 def _info(bms):
     """Present the stats for existing collections and benchmarks."""
     text = '\n\n\n' + '-' * 70 + '\n'
     text += '-' * 19 + ' Benchmarks library (teneva_bm) ' + '-' * 19 + '\n'
-    text += '-' * 70 + '\n\n'
+    text += '-' * 70 + '\n'
 
     for cl, bm_list in bms.items():
         count = len(bm_list)
+        text += '\n'
         text += f'--> {cl}' + ' ' * max(0, 10-len(cl))
         text += f': {count:-4d} benchmarks'
         for i in range(count):
             if i == 0 or i % 3 == 0:
                 text += '\n' + ' ' * 14 + '> '
             text += str(bm_list[i])
             if i < count - 1:
```

### Comparing `teneva_bm-0.3.0/teneva_bm/various/bm_matmul.py` & `teneva_bm-0.4.0/teneva_bm/various/bm_matmul.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     best known rank is "23"). The default mode size is "3", which relates to
     a standard matrix multiplication task; in this case, we are looking for a
     decomposition with factor matrix entries "-1, 0, 1". A mode size of "5"
     is also supported, which relates to the possible values "-2, -1, 0, 1, 2".
     If the "only2" flag is set during initialization, then only two factor
     matrices will be constructed, and the third matrix will be restored as a
     solution to the corresponding system of linear equations.
+    The benchmark has also the method "recover", which returns the factor
+    matrices for the given multi-indices.
     For more details, see the work Fawzi, A., et al. "Discovering faster
     matrix multiplication algorithms with reinforcement learning." Nature
     610.7930 (2022): 47-53.
 """
 
 
 class BmMatmul(Bm):
@@ -45,57 +47,83 @@
             E = [-2, -1, 0, 1, 2]
         else:
             E = []
             self.set_err('Invalid mode size. May be only 3 and 5')
 
         if size == 2 and n == 3:
             # Strassen algorithm:
-            self.set_min(i=np.array([
+            i=[
                 2, 1, 2, 1, 2, 0, 1,
                 1, 1, 1, 1, 2, 1, 2,
                 1, 2, 1, 1, 1, 2, 1,
                 2, 2, 1, 2, 1, 1, 0,
 
                 2, 2, 1, 0, 1, 2, 1,
                 1, 1, 2, 1, 1, 2, 1,
                 1, 1, 1, 2, 1, 1, 2,
                 2, 1, 0, 1, 2, 1, 2,
 
                 2, 1, 1, 2, 0, 1, 2,
                 1, 1, 2, 1, 2, 1, 1,
                 1, 2, 1, 2, 1, 1, 1,
-                2, 0, 2, 1, 1, 2, 1], dtype=int),
-                y=0.)
+                2, 0, 2, 1, 1, 2, 1]
+            self.set_min(i=i, y=0.)
 
-        self.T = T_real
-        self.E = E
-        self.size = size
-        self.rank = rank
-        self.only2 = only2
+        self.bm_T = T_real
+        self.bm_E = E
+
+        self.opt_size = size
+        self.opt_rank = rank
+        self.opt_only2 = only2
 
     @property
     def is_tens(self):
         return True
 
+    def get_config(self):
+        conf = super().get_config()
+        conf['opt_size'] = self.opt_size
+        conf['opt_rank'] = self.opt_rank
+        conf['opt_only2'] = self.opt_only2
+        return conf
+
+    def info(self, footer=''):
+        text = ''
+
+        text += 'Param size (sizes of the matrices)       : '
+        v = self.opt_size
+        text += f'{v:.0f}\n'
+
+        text += 'Param rank (search rank for CP-decomp.)  : '
+        v = self.opt_rank
+        text += f'{v:.0f}\n'
+
+        text += 'Param only2 (if True, use 2 CP-factors)  : '
+        v = 'YES' if self.opt_only2 else 'no'
+        text += f'{v}\n'
+
+        return super().info(text+footer)
+
     def prep(self):
         self.check_err()
 
-        self.loss = _loss_build(self.T, self.E, self.rank, self.only2)
+        self.loss = _loss_build(self.bm_T, self.bm_E, self.opt_rank,
+            self.opt_only2)
 
         self.is_prep = True
         return self
 
     def recover(self, i):
-        x = _ind_to_poi(i, self.E)
+        x = _ind_to_poi(i, self.bm_E)
 
-        if self.only2:
-            U, V = _factor_from_poi(x, self.rank, True)
-            W = _factor_recover(U, V, self.T)
+        if self.opt_only2:
+            U, V = _factor_from_poi(x, self.opt_rank, True)
+            W = _factor_recover(U, V, self.bm_T)
         else:
-            U, V, W = _factor_from_poi(x, self.rank, False)
+            U, V, W = _factor_from_poi(x, self.opt_rank, False)
 
         return U, V, W
 
     def _f(self, i):
         return self.loss(i)
 
 
@@ -201,15 +229,15 @@
     i2 = [np.random.choice(k) for k in bm.n]
     i3 = [np.random.choice(k) for k in bm.n]
     I = [i1, i2, i3]
     y = bm[I]
     text += '; '.join([f'{y_cur:-10.3e}' for y_cur in y])
     print(text)
 
-    if bm.size == 2 and bm.n[0] == 3:
+    if bm.opt_size == 2 and bm.n0 == 3:
         text = 'Value at the minimum (real vs calc)      :  '
         y_real = bm.y_min_real
         y_calc = bm[bm.i_min_real]
         text += f'{y_real:-10.3e}       /      {y_calc:-10.3e}'
         print(text)
 
     text = 'Check "only2" case                       :  '
@@ -219,10 +247,10 @@
     text += f'{y:-10.3e}'
     print(text)
 
     text = 'Check "recover" error                    :  '
     bm = BmMatmul(size=2, rank=7).prep()
     U, V, W = bm.recover(bm.i_min_real)
     T_appr = np.einsum('nr,mr,sr->nms', U, V, W)
-    e = np.linalg.norm(T_appr.reshape(-1) - bm.T.reshape(-1))
+    e = np.linalg.norm(T_appr.reshape(-1) - bm.bm_T.reshape(-1))
     text += f'{e:-10.3e}'
     print(text)
```

### Comparing `teneva_bm-0.3.0/teneva_bm/various/bm_topopt.py` & `teneva_bm-0.4.0/teneva_bm/various/bm_topopt.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,35 +16,71 @@
 
 class BmTopopt(Bm):
     def __init__(self, d=None, n=2, name='BmTopopt', desc=DESC, nx=128, ny=32):
         super().__init__(nx*ny, n, name, desc)
 
         if d is not None:
             self.set_err('Dimension number (d) should not be set manually')
-        if not self.is_n_equal or self.n[0] != 2:
+        if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
 
-        self.nx = nx
-        self.ny = ny
+        self.opt_nx = nx
+        self.opt_ny = ny
 
     @property
     def is_tens(self):
         return True
 
+    def get_config(self):
+        conf = super().get_config()
+        conf['opt_nx'] = self.opt_nx
+        conf['opt_ny'] = self.opt_ny
+        conf['opt_k_frac'] = self.opt_k_frac
+        conf['opt_penal'] = self.opt_penal
+        conf['opt_rmin'] = self.opt_rmin
+        return conf
+
+    def info(self, footer=''):
+        text = ''
+
+        text += 'Param nx (grid x-size)                   : '
+        v = self.opt_nx
+        text += f'{v:.0f}\n'
+
+        text += 'Param ny (grid y-size)                   : '
+        v = self.opt_ny
+        text += f'{v:.0f}\n'
+
+        text += 'Param k_frac for Topopt                  : '
+        v = self.opt_k_frac
+        text += f'{v:.6f}\n'
+
+        text += 'Param penal for Topopt                   : '
+        v = self.opt_penal
+        text += f'{v:.6f}\n'
+
+        text += 'Param rmin for Topopt                    : '
+        v = self.opt_rmin
+        text += f'{v:.6f}\n'
+
+        return super().info(text+footer)
+
     def optimize_baseline(self):
-        solver = TopOptLite(self.nx, self.ny, self.opt_penal, self.opt_rmin)
+        solver = TopOptLite(self.opt_nx, self.opt_ny, self.opt_penal,
+            self.opt_rmin)
         solver.init(Emin=1.E-9, Emax=1.0)
         solver.prep()
-        x_ini = self.opt_k_frac * np.ones(self.nx * self.ny, dtype=float)
+        x_ini = self.opt_k_frac * np.ones(self.opt_nx * self.opt_ny,
+            dtype=float)
         x_opt = solver.solve(x_ini)
         return x_opt
 
     def plot(self, x, name='solver', fpath=None):
         fig, ax = plt.subplots(1, 1, figsize=(21, 7))
-        x = x.reshape(self.nx, self.ny).T
+        x = x.reshape(self.opt_nx, self.opt_ny).T
         ax.imshow(x, cmap='gray', interpolation='none')
 
         k_frac_real = np.sum(x) / np.size(x)
 
         title = 'Result for ' + name + '. '
         title += f'Shape: {x.shape[0]} x {x.shape[1]}. '
         title += f'Frac: {k_frac_real:.2f} ({self.opt_k_frac:.2f}). '
@@ -54,15 +90,15 @@
             plt.savefig(fpath, bbox_inches='tight')
         else:
             plt.show()
 
     def prep(self):
         self.check_err()
 
-        self.bm_f = topopt_lite(self.nx, self.ny,
+        self.bm_f = topopt_lite(self.opt_nx, self.opt_ny,
             self.opt_k_frac, self.opt_penal, self.opt_rmin)
 
         self.is_prep = True
         return self
 
     def set_opts(self, k_frac=0.4, penal=3., rmin=5.4):
         """Setting options specific to this benchmark.
```

### Comparing `teneva_bm-0.3.0/teneva_bm.egg-info/PKG-INFO` & `teneva_bm-0.4.0/teneva_bm.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva-bm
-Version: 0.3.0
+Version: 0.4.0
 Summary: Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods
 Home-page: https://github.com/AndreiChertkov/teneva_bm
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
 Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
@@ -30,25 +30,32 @@
 ## Description
 
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
-> Current version "0.3.0".
+> Current version "0.4.0".
 
 The package can be installed via pip: `pip install teneva_bm` (it requires the [Python](https://www.python.org) programming language of the version >= 3.8). It can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and installed by `python setup.py install` command from the root folder of the project.
 
 > Required python packages (see `requirements.txt`) [matplotlib](https://matplotlib.org/) (3.7.0+) and [teneva](https://github.com/AndreiChertkov/teneva) (0.14.2+) will be automatically installed during the installation of the main software product.
 
 Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the following command:
 
-```bash
-pip install networkx==3.0 qubogen==0.1.1 gekko==1.0.6
-```
+- Collections `func`, `hs` and `various` do not require installation of additional libraries.
+
+- Сollections `oc` and `qubo` require installation of the following libraries:
+    ```bash
+    pip install networkx==3.0 qubogen==0.1.1 gekko==1.0.6
+    ```
+
+- Сollections `agent` and `agent_toe` require a rather complicated installation process of the `mujoco` framework, so we have prepared a special python installation script [install_mujoco.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_mujoco.py). Detailed instructions for using the script are presented in the file header.
+
+> To run benchmark optimization examples, you should also install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
 
 
 ## Documentation and examples
 
 All benchmarks inherit from the `Bm` base class (`teneva_bm/bm.py`) and are located in the subfolders (collections of benchmarks) of `teneva_bm` folder. The corresponding python files contain a detailed description of the benchmarks, as well as a scripts for a demo run at the end of the files. You can get detailed information on the created benchmark using the `info` class method:
 ```python
 from teneva_bm import *
@@ -58,21 +65,27 @@
 
 You can run demos for all benchmarks at once with the command `python demo.py` from the root folder of the project (you can also specify the name of the benchmark as a script argument to run the demo for only one benchmark, e.g., `python demo.py bm_qubo_knap_det`). You can also use a function from the `teneva_bm` package to run all or only one demo:
 ```python
 from teneva_bm import teneva_bm_demo
 teneva_bm_demo('bm_qubo_knap_det', with_info=True)
 ```
 
-> We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/demo_base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.2`).
+> We prepare some demo scripts with benchmark optimization examples in the `demo_opti` folder. To run these examples (e.g., `python demo_opti/demo_base.py`), you need to install the [PROTES](https://github.com/anabatsh/PROTES) optimizer (`pip install protes==0.3.3`).
+
+> We also present some examples [DRAFT!] in this [colab notebook](https://colab.research.google.com/drive/1z8LgqEARJziKub2dVB65CHkhcboc-fCH?usp=sharing).
 
 
 ## Available benchmarks
 
+- `agent` - the collection of problems from [gym](https://www.gymlibrary.dev/) framework, including [mujoco agents](https://www.gymlibrary.dev/environments/mujoco/index.html) based on the physics engine [mujoco](https://mujoco.org/) for faciliatating research and development in robotics, biomechanics, graphics and animation. Within the framework of this collection, explicit optimization of the entire set of actions (discrete or continuous) is assumed. The collection includes the following benchmarks: `BmAgentSwimmer`.
+
+- `agent_toe` - the same as `agent` collection, but with optimization of the discrete Toeplitz policy. The collection includes the following benchmarks: `BmAgentToeSwimmer`.
+
 - `func` - a collection of analytic functions of a real multidimensional argument. The collection includes the following benchmarks: `BmFuncAckley`, `BmFuncAlpine`, `BmFuncDixon`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncPiston`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchaffer`, `BmFuncSchwefel`.
-    > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores.
+    > For almost all functions, the exact global minimum ("continuous x point", not multi-index) is known (see `bm.x_min_real` and `bm.y_min_real`). For a number of functions (`BmFuncAlpine`, `BmFuncExp`, `BmFuncGriewank`, `BmFuncMichalewicz`, `BmFuncQing`, `BmFuncRastrigin`, `BmFuncRosenbrock`, `BmFuncSchwefel`), a `bm.build_cores()` method is available that returns an exact representation of the function on the discrete grid used in the benchmark in the tensor train (TT) format as a list of 3D TT-cores. Note also that we apply small random shift of the grid limits for all functions, to make the optimization problem more difficult (because many functions have a minimum at the center point of the domain).
 
 - `hs` (draft!) - the [Hock & Schittkowski](http://apmonitor.com/wiki/index.php/Apps/HockSchittkowski) collection of benchmark functions, containing continuous analytic functions of small dimensions (2-5), some of which have given constraints. The collection includes the following benchmarks: `BmHsFunc001`, `BmHsFunc006`.
 
 - `oc` - a collection of optimal control problems described by ordinary differential equations with discrete binary control variable, some of the problems have explicit restrictions on the elements of the control vector. The collection includes the following benchmarks: `BmOcSimple`, `BmOcSimpleConstr`.
 
 - `qubo` - a collection of quadratic unconstrained binary optimization (QUBO) problems; all benchmarks are discrete and have a mode size equals `2`. The collection includes the following benchmarks: `BmQuboKnapDet`, `BmQuboKnapQuad`, `BmQuboMaxcut`, `BmQuboMvc`.
     > The exact global minimum is known only for `BmQuboKnapDet` benchmark (note that this benchmark supports only dimensions `10`, `20`, `50`, `80` and `100`).
@@ -103,27 +116,31 @@
 - `desc` - the description of the benchmark (string). By default, a detailed description of the benchmark is used, provided in the corresponding python file.
 - `...other arguments...` - some benchmarks have additional optional arguments, which are described in the corresponding python files.
 
 ##### Setting advanced options
 
 Before calling the `bm.prep()` method, you can set a number of additional benchmark options:
 
-- `bm.set_grid_kind(kind)` - by default, we use the Chebyshev grid (`kind = 'cheb'`), but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
+- `bm.set_seed(seed=42)` - with this function we can set a custom random seed. Note that we use `Random Generator` from numpy (i.e., `numpy.random.default_rng(seed)`).
+-
+- `bm.set_grid_kind(kind='cheb')` - by default, we use the Chebyshev grid (`kind = 'cheb'`), but you can alternatively set it manually to use a uniform grid (`kind = 'uni'`).
+
+- `bm.set_budget(m=None, m_cache=None, is_strict=True)` - optional method to set the computation buget `m`. If the number of requests to the benchmark (from calls to `bm.get` and `bm.get_poi` methods) exceeds the specified budget, then `None` will be returned. If the flag `is_strict` is disabled, then the request for the last batch will be allowed, after which the budget will be exceeded, otherwise this last batch will not be considered. Note that when the budget is exceeded, `None` will be returned both when requesting a single value and a batch of values. Also, in a similar way, you can set a limit on the use of the cache by `m_cache` parameter.
 
 - `bm.set_constr(penalty=1.E+42, eps=1.E-16, with_amplitude=True)` - if the benchmark has a constraint, then using this function you can set a `penalty` (for the requested points that do not satisfy the constraint, the value `penalty * constraint_value` will be returned) and a `eps` (threshold value to check that the constraint has been fulfilled). Note that we set the constraints as a function (`bm._c`) that returns the value `constraint_value` (amplitude) of the constraint, and if the constraint is met, then the value must be non-positive, otherwise, the objective function is not calculated and a value proportional to the amplitude of the constraint is returned (if you disable flag `with_amplitude`, then just the value of the penalty will be returned).
 
-- `bm.set_max(i, x, y)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks , which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
+- `bm.set_max(i=None, x=None, y=None)` - if necessary, you can manually set the multi-index, the corresponding continuous point (for benchmarks , which relate to functions of a continuous argument), and the corresponding value for the exact global maximum of the function. The corresponding values will be further available in the benchmark as `bm.i_max_real`, `bm.x_max_real` and `bm.y_max_real` respectively. When the benchmark is initialized, this function is called automatically if the optimum is known.
 
-- `bm.set_min(i, x, y)` - the same as in the previous point, but for the global minimum.
+- `bm.set_min(i=None, x=None, y=None)` - the same as in the previous point, but for the global minimum.
 
-- `bm.set_log(True, cond, step, prefix)` - when calling this function with the `True` argument, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step and a string `prefix` for the log.
+- `bm.set_log(with_log=True, cond='min-max', step=1000, prefix='bm', with_min=True, with_max=True)` - when calling this function with the `True` argument `with_log`, the log will be printed while requests to benchmark. You may set the log codition `cond` (`min`, `max`, `min-max` or `step`; e.g., in the case `min` the log will be presented each time the `min` value is updated), the log step and a string `prefix` for the log. You can also disable the display of minimum values (`with_min`) or maximum values (`with_max`).
 
-- `bm.set_cache(True)` - when calling this function with the `True` argument, the cache will be used (it is not used by default), that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can specify `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
+- `bm.set_cache(with_cache=True, cache=None, m_max=1.E+8)` - when calling this function with the `True` argument `with_cache`, the cache will be used (it is not used by default), that is, all the values requested from the benchmark will be saved and when the same multi-indices are accessed again, the values will be retrieved from the cache instead of explicitly calculating the objective function. Additionally, you can optionally pass as an argument `cache` an already existing cache in the form of a dictionary (the keys are multi-indices in the form of tuples, and the values are the corresponding values of the objective function). We especially note that the cache is only used when querying benchmark values in discrete multi-indices; for requested continuous points, no cache will be used. It is also important to note that no cache will be used for matching multi-indices in the same requested batch of values. Optionally, you can specify `m_max` argument that specifies the maximum cache size. If the size is exceeded, the cache will be cleared and a corresponding warning will be displayed.
 
-- `bm.set_quantization(True)` - an auxiliary option, when set, it is assumed that the requested multi-indices and the points are presented in a quantized representation, that is, each mode of the original grid of the size `2^q`, is converted into `q` virtual modes, having a size `2`.
+- `bm.set_quantization(with_quantization=True)` - an auxiliary option, when set, it is assumed that the requested multi-indices and the points are presented in a quantized representation, that is, each mode of the original grid of the size `2^q`, is converted into `q` virtual modes, having a size `2`.
 
 - `bm.set_opts(...)` - for some benchmarks, this function may be called to set additional benchmark-specific options (please see the description of arguments in the relevant benchmark code file).
 
 ##### Computing benchmark values
 
 Now the benchmark is ready to go, and we can calculate its value in any requested discrete multi-index (a real number will be returned) or a list of its values for any requested batch of discrete multi-indices (1D numpy array of real numbers will be returned):
 ```python
```

### Comparing `teneva_bm-0.3.0/teneva_bm.egg-info/SOURCES.txt` & `teneva_bm-0.4.0/teneva_bm.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 teneva_bm/bm.py
 teneva_bm/teneva_bm_demo.py
 teneva_bm.egg-info/PKG-INFO
 teneva_bm.egg-info/SOURCES.txt
 teneva_bm.egg-info/dependency_links.txt
 teneva_bm.egg-info/requires.txt
 teneva_bm.egg-info/top_level.txt
+teneva_bm/agent/__init__.py
+teneva_bm/agent/agent.py
+teneva_bm/agent/bm_agent_swimmer.py
+teneva_bm/agent_toe/__init__.py
+teneva_bm/agent_toe/agent_toe.py
+teneva_bm/agent_toe/bm_agent_toe_swimmer.py
 teneva_bm/func/__init__.py
 teneva_bm/func/bm_func_ackley.py
 teneva_bm/func/bm_func_alpine.py
 teneva_bm/func/bm_func_dixon.py
 teneva_bm/func/bm_func_exp.py
 teneva_bm/func/bm_func_griewank.py
 teneva_bm/func/bm_func_michalewicz.py
```


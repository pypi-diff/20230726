# Comparing `tmp/Chronix2Grid-1.1.0.tar.gz` & `tmp/Chronix2Grid-1.1.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chronix2Grid-1.1.0.tar", last modified: Tue May 31 10:03:46 2022, max compression
+gzip compressed data, was "Chronix2Grid-1.1.0.post1.tar", last modified: Tue May 31 12:05:07 2022, max compression
```

## Comparing `Chronix2Grid-1.1.0.tar` & `Chronix2Grid-1.1.0.post1.tar`

### file list

```diff
@@ -1,93 +1,110 @@
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.574410 Chronix2Grid-1.1.0/
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.478407 Chronix2Grid-1.1.0/Chronix2Grid.egg-info/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    12299 2022-05-31 10:03:46.000000 Chronix2Grid-1.1.0/Chronix2Grid.egg-info/PKG-INFO
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3120 2022-05-31 10:03:46.000000 Chronix2Grid-1.1.0/Chronix2Grid.egg-info/SOURCES.txt
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)        1 2022-05-31 10:03:46.000000 Chronix2Grid-1.1.0/Chronix2Grid.egg-info/dependency_links.txt
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       64 2022-05-31 10:03:46.000000 Chronix2Grid-1.1.0/Chronix2Grid.egg-info/entry_points.txt
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)        1 2022-03-24 15:16:04.000000 Chronix2Grid-1.1.0/Chronix2Grid.egg-info/not-zip-safe
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      584 2022-05-31 10:03:46.000000 Chronix2Grid-1.1.0/Chronix2Grid.egg-info/requires.txt
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       33 2022-05-31 10:03:46.000000 Chronix2Grid-1.1.0/Chronix2Grid.egg-info/top_level.txt
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    12299 2022-05-31 10:03:46.570409 Chronix2Grid-1.1.0/PKG-INFO
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     9348 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/README.md
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.490407 Chronix2Grid-1.1.0/RenewableGANBackend/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      482 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/RenewableGANBackend/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2405 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/RenewableGANBackend/backend.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3738 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/RenewableGANBackend/config.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6535 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/RenewableGANBackend/gan_utils.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4279 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/RenewableGANBackend/generate_solar_wind_gan.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.506408 Chronix2Grid-1.1.0/chronix2grid/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    17135 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/GeneratorBackend.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)      506 2022-05-31 09:42:27.000000 Chronix2Grid-1.1.0/chronix2grid/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    19055 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/config.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1567 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/constants.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2100 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/default_backend.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.510408 Chronix2Grid-1.1.0/chronix2grid/generation/
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)      483 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/__init__.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.510408 Chronix2Grid-1.1.0/chronix2grid/generation/_dispatch/
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.514408 Chronix2Grid-1.1.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    10610 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/PypsaEconomicDispatch.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.514408 Chronix2Grid-1.1.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      555 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    11389 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/run_economic_dispatch.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    16578 2022-05-25 16:11:55.000000 Chronix2Grid-1.1.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/utils.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      482 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      482 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/_dispatch/__init__.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.522408 Chronix2Grid-1.1.0/chronix2grid/generation/consumption/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2429 2022-05-25 16:11:55.000000 Chronix2Grid-1.1.0/chronix2grid/generation/consumption/ConsumptionGeneratorBackend.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)      595 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/consumption/__init__.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     7421 2022-05-25 16:11:55.000000 Chronix2Grid-1.1.0/chronix2grid/generation/consumption/consumption_utils.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     4132 2022-05-25 16:11:55.000000 Chronix2Grid-1.1.0/chronix2grid/generation/consumption/generate_load.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.534408 Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2940 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/DispatchBackend.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    21824 2022-04-06 06:36:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/EconomicDispatch.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.534408 Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/PypsaDispatchBackend/
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.538408 Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/PypsaDispatchBackend/EDispatch_L2RPN2020/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      610 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/PypsaDispatchBackend/EDispatch_L2RPN2020/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      643 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/PypsaDispatchBackend/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      482 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    10957 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/dispatch_loss_utils.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6236 2022-04-06 06:36:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/generate_dispatch.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3374 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/utils.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     2545 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/generate_chronics.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8974 2022-04-06 06:36:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/generation_utils.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.538408 Chronix2Grid-1.1.0/chronix2grid/generation/hydro/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      483 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/hydro/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3738 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/hydro/make_hydro_guide_curves.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.542409 Chronix2Grid-1.1.0/chronix2grid/generation/loss/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2611 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/loss/LossBackend.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      483 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/loss/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2957 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/loss/generate_loss.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.546409 Chronix2Grid-1.1.0/chronix2grid/generation/renewable/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2422 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/renewable/RenewableBackend.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)      562 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/renewable/__init__.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     8501 2022-04-06 06:36:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/renewable/generate_solar_wind.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     7552 2022-04-06 06:36:58.000000 Chronix2Grid-1.1.0/chronix2grid/generation/renewable/solar_wind_utils.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.550409 Chronix2Grid-1.1.0/chronix2grid/grid2op_utils/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      669 2022-05-25 16:11:55.000000 Chronix2Grid-1.1.0/chronix2grid/grid2op_utils/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     5017 2022-05-25 16:11:55.000000 Chronix2Grid-1.1.0/chronix2grid/grid2op_utils/add_data.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2670 2022-05-25 16:11:55.000000 Chronix2Grid-1.1.0/chronix2grid/grid2op_utils/generate_one_episode.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    53374 2022-05-31 09:36:10.000000 Chronix2Grid-1.1.0/chronix2grid/grid2op_utils/utils.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.550409 Chronix2Grid-1.1.0/chronix2grid/kpi/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    13592 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0/chronix2grid/kpi/Generator_parameter_checker.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0/chronix2grid/kpi/__init__.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.566409 Chronix2Grid-1.1.0/chronix2grid/kpi/deterministic/
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)      483 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0/chronix2grid/kpi/deterministic/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7082 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0/chronix2grid/kpi/deterministic/hydro.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    53164 2022-04-06 06:36:58.000000 Chronix2Grid-1.1.0/chronix2grid/kpi/deterministic/kpis.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2002 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0/chronix2grid/kpi/deterministic/nuclear.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8931 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0/chronix2grid/kpi/deterministic/solar.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7496 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0/chronix2grid/kpi/deterministic/wind.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     8256 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0/chronix2grid/kpi/main.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.566409 Chronix2Grid-1.1.0/chronix2grid/kpi/preprocessing/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)        0 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0/chronix2grid/kpi/preprocessing/__init__.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5141 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0/chronix2grid/kpi/preprocessing/pivot_KPI.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    20751 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0/chronix2grid/kpi/preprocessing/pivot_utils.py
-drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 10:03:46.570409 Chronix2Grid-1.1.0/chronix2grid/kpi/utils/
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)        0 2022-03-17 13:47:09.000000 Chronix2Grid-1.1.0/chronix2grid/kpi/utils/__init__.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1301 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0/chronix2grid/kpi/utils/plot_tools.py
--rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    12735 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0/chronix2grid/main.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     5179 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0/chronix2grid/output_processor.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1138 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0/chronix2grid/seed_manager.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      660 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0/chronix2grid/utils.py
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       38 2022-05-31 10:03:46.574410 Chronix2Grid-1.1.0/setup.cfg
--rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4373 2022-05-31 09:41:44.000000 Chronix2Grid-1.1.0/setup.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:07.053472 Chronix2Grid-1.1.0.post1/
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.949469 Chronix2Grid-1.1.0.post1/Chronix2Grid.egg-info/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    12305 2022-05-31 12:05:06.000000 Chronix2Grid-1.1.0.post1/Chronix2Grid.egg-info/PKG-INFO
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3913 2022-05-31 12:05:06.000000 Chronix2Grid-1.1.0.post1/Chronix2Grid.egg-info/SOURCES.txt
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)        1 2022-05-31 12:05:06.000000 Chronix2Grid-1.1.0.post1/Chronix2Grid.egg-info/dependency_links.txt
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       64 2022-05-31 12:05:06.000000 Chronix2Grid-1.1.0.post1/Chronix2Grid.egg-info/entry_points.txt
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)        1 2022-03-24 15:16:04.000000 Chronix2Grid-1.1.0.post1/Chronix2Grid.egg-info/not-zip-safe
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      584 2022-05-31 12:05:06.000000 Chronix2Grid-1.1.0.post1/Chronix2Grid.egg-info/requires.txt
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       33 2022-05-31 12:05:06.000000 Chronix2Grid-1.1.0.post1/Chronix2Grid.egg-info/top_level.txt
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      272 2022-05-31 11:53:28.000000 Chronix2Grid-1.1.0.post1/MANIFEST.in
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    12305 2022-05-31 12:05:07.053472 Chronix2Grid-1.1.0.post1/PKG-INFO
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     9348 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/README.md
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.957470 Chronix2Grid-1.1.0.post1/RenewableGANBackend/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      482 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/RenewableGANBackend/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2405 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/RenewableGANBackend/backend.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3738 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/RenewableGANBackend/config.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6535 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/RenewableGANBackend/gan_utils.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4279 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/RenewableGANBackend/generate_solar_wind_gan.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.969470 Chronix2Grid-1.1.0.post1/chronix2grid/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    17135 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/GeneratorBackend.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)      512 2022-05-31 11:43:59.000000 Chronix2Grid-1.1.0.post1/chronix2grid/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    19055 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/config.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1567 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/constants.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2100 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/default_backend.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.973470 Chronix2Grid-1.1.0.post1/chronix2grid/generation/
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)      483 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/__init__.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.973470 Chronix2Grid-1.1.0.post1/chronix2grid/generation/_dispatch/
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.973470 Chronix2Grid-1.1.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    10610 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/PypsaEconomicDispatch.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.977470 Chronix2Grid-1.1.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      555 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    11389 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/run_economic_dispatch.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    16578 2022-05-25 16:11:55.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/utils.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      482 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      482 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/_dispatch/__init__.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.981470 Chronix2Grid-1.1.0.post1/chronix2grid/generation/consumption/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2429 2022-05-25 16:11:55.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/consumption/ConsumptionGeneratorBackend.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)      595 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/consumption/__init__.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     7421 2022-05-25 16:11:55.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/consumption/consumption_utils.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     4132 2022-05-25 16:11:55.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/consumption/generate_load.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.985470 Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2940 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/DispatchBackend.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    21824 2022-04-06 06:36:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/EconomicDispatch.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.985470 Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/PypsaDispatchBackend/
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.985470 Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/PypsaDispatchBackend/EDispatch_L2RPN2020/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      610 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/PypsaDispatchBackend/EDispatch_L2RPN2020/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      643 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/PypsaDispatchBackend/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      482 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    10957 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/dispatch_loss_utils.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     6236 2022-04-06 06:36:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/generate_dispatch.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3374 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/utils.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     2545 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/generate_chronics.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8974 2022-04-06 06:36:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/generation_utils.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.989470 Chronix2Grid-1.1.0.post1/chronix2grid/generation/hydro/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      483 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/hydro/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     3738 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/hydro/make_hydro_guide_curves.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.989470 Chronix2Grid-1.1.0.post1/chronix2grid/generation/loss/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2611 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/loss/LossBackend.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      483 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/loss/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2957 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/loss/generate_loss.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.993471 Chronix2Grid-1.1.0.post1/chronix2grid/generation/renewable/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2422 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/renewable/RenewableBackend.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)      562 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/renewable/__init__.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     8501 2022-04-06 06:36:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/renewable/generate_solar_wind.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     7552 2022-04-06 06:36:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/generation/renewable/solar_wind_utils.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.993471 Chronix2Grid-1.1.0.post1/chronix2grid/getting_started/
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)      483 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/getting_started/__init__.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.993471 Chronix2Grid-1.1.0.post1/chronix2grid/getting_started/example/
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)      483 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/getting_started/example/__init__.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.993471 Chronix2Grid-1.1.0.post1/chronix2grid/getting_started/example/input/
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)      483 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/getting_started/example/input/__init__.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:06.993471 Chronix2Grid-1.1.0.post1/chronix2grid/getting_started/example/input/generation/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      556 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/getting_started/example/input/generation/__init__.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:07.037472 Chronix2Grid-1.1.0.post1/chronix2grid/getting_started/example/input/generation/patterns/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      556 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/getting_started/example/input/generation/patterns/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)  4825656 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/getting_started/example/input/generation/patterns/hydro_french.csv
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)  4662662 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/getting_started/example/input/generation/patterns/hydro_raw_2018.csv
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)  5140153 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/getting_started/example/input/generation/patterns/hydro_smooth_2018.csv
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)  8081173 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/getting_started/example/input/generation/patterns/load_weekly_pattern.csv
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)  2108172 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/getting_started/example/input/generation/patterns/loss_pattern.csv
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    70216 2022-04-06 06:33:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/getting_started/example/input/generation/patterns/solar_pattern.npy
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:07.041472 Chronix2Grid-1.1.0.post1/chronix2grid/grid2op_utils/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      669 2022-05-25 16:11:55.000000 Chronix2Grid-1.1.0.post1/chronix2grid/grid2op_utils/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     5017 2022-05-25 16:11:55.000000 Chronix2Grid-1.1.0.post1/chronix2grid/grid2op_utils/add_data.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2670 2022-05-25 16:11:55.000000 Chronix2Grid-1.1.0.post1/chronix2grid/grid2op_utils/generate_one_episode.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    53374 2022-05-31 09:36:10.000000 Chronix2Grid-1.1.0.post1/chronix2grid/grid2op_utils/utils.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:07.041472 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)    13592 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/Generator_parameter_checker.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/__init__.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:07.045472 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/deterministic/
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)      483 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/deterministic/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7082 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/deterministic/hydro.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    53164 2022-04-06 06:36:58.000000 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/deterministic/kpis.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     2002 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/deterministic/nuclear.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     8931 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/deterministic/solar.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     7496 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/deterministic/wind.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     8256 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/main.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:07.049472 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/preprocessing/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)        0 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/preprocessing/__init__.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)     5141 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/preprocessing/pivot_KPI.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    20751 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/preprocessing/pivot_utils.py
+drwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)        0 2022-05-31 12:05:07.049472 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/utils/
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)        0 2022-03-17 13:47:09.000000 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/utils/__init__.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1301 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0.post1/chronix2grid/kpi/utils/plot_tools.py
+-rwxrwxr-x   0 donnotben (1774396215) donnotben (1774396215)    12735 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0.post1/chronix2grid/main.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     5179 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0.post1/chronix2grid/output_processor.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     1138 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0.post1/chronix2grid/seed_manager.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)      660 2022-04-06 06:33:59.000000 Chronix2Grid-1.1.0.post1/chronix2grid/utils.py
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)       38 2022-05-31 12:05:07.053472 Chronix2Grid-1.1.0.post1/setup.cfg
+-rw-rw-r--   0 donnotben (1774396215) donnotben (1774396215)     4379 2022-05-31 11:44:09.000000 Chronix2Grid-1.1.0.post1/setup.py
```

### Comparing `Chronix2Grid-1.1.0/Chronix2Grid.egg-info/PKG-INFO` & `Chronix2Grid-1.1.0.post1/Chronix2Grid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chronix2Grid
-Version: 1.1.0
+Version: 1.1.0.post1
 Summary: A python package to generate "en-masse" chronics for loads and productions (thermal, renewable)
 Home-page: https://github.com/BDonnot/ChroniX2Grid
 Author: Mario Jothy, Nicolas Megel, Vincent Renault, Benjamin Donnot
 Author-email:  mario.jothy@artelys.com
 License: Mozilla Public License 2.0 (MPL 2.0)
 Description: # ChroniX2Grid - The Extensive PowerGrid Time-serie Generator
```

### Comparing `Chronix2Grid-1.1.0/Chronix2Grid.egg-info/requires.txt` & `Chronix2Grid-1.1.0.post1/Chronix2Grid.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/PKG-INFO` & `Chronix2Grid-1.1.0.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chronix2Grid
-Version: 1.1.0
+Version: 1.1.0.post1
 Summary: A python package to generate "en-masse" chronics for loads and productions (thermal, renewable)
 Home-page: https://github.com/BDonnot/ChroniX2Grid
 Author: Mario Jothy, Nicolas Megel, Vincent Renault, Benjamin Donnot
 Author-email:  mario.jothy@artelys.com
 License: Mozilla Public License 2.0 (MPL 2.0)
 Description: # ChroniX2Grid - The Extensive PowerGrid Time-serie Generator
```

### Comparing `Chronix2Grid-1.1.0/README.md` & `Chronix2Grid-1.1.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/RenewableGANBackend/backend.py` & `Chronix2Grid-1.1.0.post1/RenewableGANBackend/backend.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/RenewableGANBackend/config.py` & `Chronix2Grid-1.1.0.post1/RenewableGANBackend/config.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/RenewableGANBackend/gan_utils.py` & `Chronix2Grid-1.1.0.post1/RenewableGANBackend/gan_utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/RenewableGANBackend/generate_solar_wind_gan.py` & `Chronix2Grid-1.1.0.post1/RenewableGANBackend/generate_solar_wind_gan.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/GeneratorBackend.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/GeneratorBackend.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/config.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/config.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/constants.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/constants.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/default_backend.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/default_backend.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/PypsaEconomicDispatch.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/PypsaEconomicDispatch.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/__init__.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/__init__.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/run_economic_dispatch.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/run_economic_dispatch.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/utils.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/_dispatch/_PypsaDispatchBackend/_EDispatch_L2RPN2020/utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/consumption/ConsumptionGeneratorBackend.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/consumption/ConsumptionGeneratorBackend.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/consumption/__init__.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/consumption/__init__.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/consumption/consumption_utils.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/consumption/consumption_utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/consumption/generate_load.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/consumption/generate_load.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/DispatchBackend.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/DispatchBackend.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/EconomicDispatch.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/EconomicDispatch.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/PypsaDispatchBackend/EDispatch_L2RPN2020/__init__.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/PypsaDispatchBackend/EDispatch_L2RPN2020/__init__.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/PypsaDispatchBackend/__init__.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/PypsaDispatchBackend/__init__.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/dispatch_loss_utils.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/dispatch_loss_utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/generate_dispatch.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/generate_dispatch.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/dispatch/utils.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/dispatch/utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/generate_chronics.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/generate_chronics.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/generation_utils.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/generation_utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/hydro/make_hydro_guide_curves.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/hydro/make_hydro_guide_curves.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/loss/LossBackend.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/loss/LossBackend.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/loss/generate_loss.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/loss/generate_loss.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/renewable/RenewableBackend.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/renewable/RenewableBackend.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/renewable/__init__.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/renewable/__init__.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/renewable/generate_solar_wind.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/renewable/generate_solar_wind.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/generation/renewable/solar_wind_utils.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/generation/renewable/solar_wind_utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/grid2op_utils/__init__.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/grid2op_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/grid2op_utils/add_data.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/grid2op_utils/add_data.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/grid2op_utils/generate_one_episode.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/grid2op_utils/generate_one_episode.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/grid2op_utils/utils.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/grid2op_utils/utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/kpi/Generator_parameter_checker.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/kpi/Generator_parameter_checker.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/kpi/deterministic/hydro.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/kpi/deterministic/hydro.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/kpi/deterministic/kpis.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/kpi/deterministic/kpis.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/kpi/deterministic/nuclear.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/kpi/deterministic/nuclear.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/kpi/deterministic/solar.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/kpi/deterministic/solar.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/kpi/deterministic/wind.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/kpi/deterministic/wind.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/kpi/main.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/kpi/main.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/kpi/preprocessing/pivot_KPI.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/kpi/preprocessing/pivot_KPI.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/kpi/preprocessing/pivot_utils.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/kpi/preprocessing/pivot_utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/kpi/utils/plot_tools.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/kpi/utils/plot_tools.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/main.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/main.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/output_processor.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/output_processor.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/seed_manager.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/seed_manager.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/chronix2grid/utils.py` & `Chronix2Grid-1.1.0.post1/chronix2grid/utils.py`

 * *Files identical despite different names*

### Comparing `Chronix2Grid-1.1.0/setup.py` & `Chronix2Grid-1.1.0.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
     
     
 setup(name='Chronix2Grid',
-      version='1.1.0',
+      version='1.1.0.post1',
       description='A python package to generate "en-masse" chronics for loads and productions (thermal, renewable)',
       long_description=long_description,
       long_description_content_type='text/markdown',
       classifiers=[
           'Development Status :: 4 - Beta',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
```


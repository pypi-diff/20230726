# Comparing `tmp/trajectopy-0.3.0.tar.gz` & `tmp/trajectopy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trajectopy-0.3.0.tar", last modified: Tue Jul 25 08:41:41 2023, max compression
+gzip compressed data, was "trajectopy-0.3.1.tar", last modified: Wed Jul 26 08:32:55 2023, max compression
```

## Comparing `trajectopy-0.3.0.tar` & `trajectopy-0.3.1.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.752533 trajectopy-0.3.0/
--rw-rw-rw-   0        0        0    35790 2023-07-17 09:26:39.000000 trajectopy-0.3.0/LICENSE
--rw-rw-rw-   0        0        0    19879 2023-07-25 08:41:41.751531 trajectopy-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    19479 2023-07-25 08:40:03.000000 trajectopy-0.3.0/README.md
--rw-rw-rw-   0        0        0      787 2023-07-25 08:40:25.000000 trajectopy-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-25 08:41:41.752533 trajectopy-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1628 2023-07-19 07:37:04.000000 trajectopy-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.661479 trajectopy-0.3.0/test/
--rw-rw-rw-   0        0        0     7503 2023-07-14 07:41:14.000000 trajectopy-0.3.0/test/test_alignment.py
--rw-rw-rw-   0        0        0     5487 2023-07-25 08:37:59.000000 trajectopy-0.3.0/test/test_comparison.py
--rw-rw-rw-   0        0        0     2347 2023-07-14 07:41:14.000000 trajectopy-0.3.0/test/test_settings.py
--rw-rw-rw-   0        0        0     1372 2023-07-14 07:41:14.000000 trajectopy-0.3.0/test/test_sorting.py
--rw-rw-rw-   0        0        0     6331 2023-07-14 07:41:14.000000 trajectopy-0.3.0/test/test_trajectory.py
--rw-rw-rw-   0        0        0      339 2023-07-14 07:41:14.000000 trajectopy-0.3.0/test/testdata.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.671034 trajectopy-0.3.0/trajectopy/
--rw-rw-rw-   0        0        0    35790 2023-07-18 14:52:08.000000 trajectopy-0.3.0/trajectopy/LICENSE
--rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/__init__.py
--rw-rw-rw-   0        0        0      630 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.692991 trajectopy-0.3.0/trajectopy/alignment/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/alignment/__init__.py
--rw-rw-rw-   0        0        0    39680 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/alignment/alignment.py
--rw-rw-rw-   0        0        0     9340 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/alignment/data.py
--rw-rw-rw-   0        0        0     2421 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/alignment/direct_helmert_transformation.py
--rw-rw-rw-   0        0        0     5354 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/alignment/direct_leverarm.py
--rw-rw-rw-   0        0        0     2181 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/alignment/direct_timeshift.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.694989 trajectopy-0.3.0/trajectopy/alignment/functional_model/
--rw-rw-rw-   0        0        0        0 2023-07-18 14:52:08.000000 trajectopy-0.3.0/trajectopy/alignment/functional_model/__init__.py
--rw-rw-rw-   0        0        0    16031 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/alignment/functional_model/equations.py
--rw-rw-rw-   0        0        0     8022 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/alignment/functional_model/interface.py
--rw-rw-rw-   0        0        0    19324 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/alignment/parameters.py
--rw-rw-rw-   0        0        0     3910 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/alignment/util.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.700534 trajectopy-0.3.0/trajectopy/approximation/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/approximation/__init__.py
--rw-rw-rw-   0        0        0     8005 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/approximation/cubic_approximation.py
--rw-rw-rw-   0        0        0     5795 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/approximation/mls_approximation.py
--rw-rw-rw-   0        0        0     5303 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/approximation/rot_approximation.py
--rw-rw-rw-   0        0        0     6116 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/approximation/trajectory_approximation.py
--rw-rw-rw-   0        0        0     4272 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/approximation/util.py
--rw-rw-rw-   0        0        0     4843 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/approximation/voxelizer.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.702536 trajectopy-0.3.0/trajectopy/evaluation/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/evaluation/__init__.py
--rw-rw-rw-   0        0        0    14911 2023-07-25 08:26:56.000000 trajectopy-0.3.0/trajectopy/evaluation/comparison.py
--rw-rw-rw-   0        0        0     4872 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/evaluation/matching.py
--rw-rw-rw-   0        0        0    29996 2023-07-25 08:30:17.000000 trajectopy-0.3.0/trajectopy/evaluation/trajectory_deviations.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.704534 trajectopy-0.3.0/trajectopy/gui/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/__init__.py
--rw-rw-rw-   0        0        0    14315 2023-07-25 07:49:54.000000 trajectopy-0.3.0/trajectopy/gui/main_window.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.709533 trajectopy-0.3.0/trajectopy/gui/managers/
--rw-rw-rw-   0        0        0        0 2023-07-18 14:52:08.000000 trajectopy-0.3.0/trajectopy/gui/managers/__init__.py
--rw-rw-rw-   0        0        0     4444 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/gui/managers/file_manager.py
--rw-rw-rw-   0        0        0     1730 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/gui/managers/manager.py
--rw-rw-rw-   0        0        0     3677 2023-07-19 15:01:54.000000 trajectopy-0.3.0/trajectopy/gui/managers/plot_manager.py
--rw-rw-rw-   0        0        0     3812 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/managers/session_manager.py
--rw-rw-rw-   0        0        0    31367 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/gui/managers/trajectory_manager.py
--rw-rw-rw-   0        0        0     8040 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/managers/ui_manager.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.714536 trajectopy-0.3.0/trajectopy/gui/models/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/models/__init__.py
--rw-rw-rw-   0        0        0    11907 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/gui/models/entry.py
--rw-rw-rw-   0        0        0     1115 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/models/property_model.py
--rw-rw-rw-   0        0        0     3904 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/models/result_model.py
--rw-rw-rw-   0        0        0      983 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/gui/models/selection.py
--rw-rw-rw-   0        0        0     4030 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/gui/models/table_model.py
--rw-rw-rw-   0        0        0     4837 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/gui/models/trajectory_model.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.722534 trajectopy-0.3.0/trajectopy/gui/requests/
--rw-rw-rw-   0        0        0        0 2023-07-18 14:52:08.000000 trajectopy-0.3.0/trajectopy/gui/requests/__init__.py
--rw-rw-rw-   0        0        0      666 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/requests/file_request.py
--rw-rw-rw-   0        0        0      635 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/requests/plot_requests.py
--rw-rw-rw-   0        0        0      424 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/requests/plot_settings_request.py
--rw-rw-rw-   0        0        0      371 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/requests/property_request.py
--rw-rw-rw-   0        0        0      500 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/gui/requests/request.py
--rw-rw-rw-   0        0        0      565 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/requests/result_model_request.py
--rw-rw-rw-   0        0        0      388 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/requests/session_request.py
--rw-rw-rw-   0        0        0     1029 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/requests/trajectory_manager_request.py
--rw-rw-rw-   0        0        0      593 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/requests/trajectory_model_request.py
--rw-rw-rw-   0        0        0      836 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/requests/ui_request.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.723536 trajectopy-0.3.0/trajectopy/gui/resources/
--rw-rw-rw-   0        0        0   120742 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/resources/full-icon-poppins.png
--rw-rw-rw-   0        0        0    24491 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/resources/icon.png
--rw-rw-rw-   0        0        0     1751 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/util.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.733481 trajectopy-0.3.0/trajectopy/gui/views/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/views/__init__.py
--rw-rw-rw-   0        0        0     3757 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/views/about_window.py
--rw-rw-rw-   0        0        0     9601 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/views/alignment_edit_window.py
--rw-rw-rw-   0        0        0    21480 2023-07-19 07:37:04.000000 trajectopy-0.3.0/trajectopy/gui/views/plot_settings_window.py
--rw-rw-rw-   0        0        0     2483 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/views/progress_window.py
--rw-rw-rw-   0        0        0     4013 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/views/properties_window.py
--rw-rw-rw-   0        0        0     6154 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/views/result_context_menu.py
--rw-rw-rw-   0        0        0     4717 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/gui/views/result_selection_window.py
--rw-rw-rw-   0        0        0     4725 2023-07-19 15:01:54.000000 trajectopy-0.3.0/trajectopy/gui/views/result_table_view.py
--rw-rw-rw-   0        0        0    54090 2023-07-25 08:15:18.000000 trajectopy-0.3.0/trajectopy/gui/views/settings_window.py
--rw-rw-rw-   0        0        0    20852 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/views/trajectory_context_menu.py
--rw-rw-rw-   0        0        0     6744 2023-07-17 09:26:50.000000 trajectopy-0.3.0/trajectopy/gui/views/trajectory_table_view.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.738485 trajectopy-0.3.0/trajectopy/plotting/
--rw-rw-rw-   0        0        0       81 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/plotting/__init__.py
--rw-rw-rw-   0        0        0     2185 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/plotting/alignment_plot.py
--rw-rw-rw-   0        0        0      498 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/plotting/default.mplstyle
--rw-rw-rw-   0        0        0    21537 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/plotting/deviation_plot.py
--rw-rw-rw-   0        0        0     7223 2023-07-19 15:01:54.000000 trajectopy-0.3.0/trajectopy/plotting/plot_tabs.py
--rw-rw-rw-   0        0        0     3911 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/plotting/trajectory_plot.py
--rw-rw-rw-   0        0        0     7826 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/plotting/util.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.743486 trajectopy-0.3.0/trajectopy/settings/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/settings/__init__.py
--rw-rw-rw-   0        0        0     8256 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/settings/alignment_settings.py
--rw-rw-rw-   0        0        0     1558 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/settings/approximation_settings.py
--rw-rw-rw-   0        0        0     5669 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/settings/comparison_settings.py
--rw-rw-rw-   0        0        0     3578 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/settings/core.py
--rw-rw-rw-   0        0        0     1703 2023-07-19 07:37:04.000000 trajectopy-0.3.0/trajectopy/settings/plot_settings.py
--rw-rw-rw-   0        0        0     2433 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/settings/processing_settings.py
--rw-rw-rw-   0        0        0      945 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/settings/sorting_settings.py
--rw-rw-rw-   0        0        0    35120 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/trajectory.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.749531 trajectopy-0.3.0/trajectopy/util/
--rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/util/__init__.py
--rw-rw-rw-   0        0        0    18312 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/util/datahandling.py
--rw-rw-rw-   0        0        0     1490 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/util/definitions.py
--rw-rw-rw-   0        0        0      935 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/util/path.py
--rw-rw-rw-   0        0        0     5389 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/util/printing.py
--rw-rw-rw-   0        0        0    13611 2023-07-25 08:11:16.000000 trajectopy-0.3.0/trajectopy/util/reading.py
--rw-rw-rw-   0        0        0     1956 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/util/rotationset.py
--rw-rw-rw-   0        0        0    16143 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/util/spatialsorter.py
--rw-rw-rw-   0        0        0      973 2023-07-14 07:41:14.000000 trajectopy-0.3.0/trajectopy/util/trajectory_processing_state.py
--rw-rw-rw-   0        0        0        5 2023-07-25 08:33:24.000000 trajectopy-0.3.0/trajectopy/version
-drwxrwxrwx   0        0        0        0 2023-07-25 08:41:41.686987 trajectopy-0.3.0/trajectopy.egg-info/
--rw-rw-rw-   0        0        0    19879 2023-07-25 08:41:41.000000 trajectopy-0.3.0/trajectopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3943 2023-07-25 08:41:41.000000 trajectopy-0.3.0/trajectopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 08:41:41.000000 trajectopy-0.3.0/trajectopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-25 08:41:41.000000 trajectopy-0.3.0/trajectopy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-14 07:43:35.000000 trajectopy-0.3.0/trajectopy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      180 2023-07-25 08:41:41.000000 trajectopy-0.3.0/trajectopy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-25 08:41:41.000000 trajectopy-0.3.0/trajectopy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:32:55.093314 trajectopy-0.3.1/
+-rw-rw-rw-   0        0        0    35790 2023-07-17 09:26:39.000000 trajectopy-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0    19879 2023-07-26 08:32:55.093314 trajectopy-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    19479 2023-07-25 08:44:31.000000 trajectopy-0.3.1/README.md
+-rw-rw-rw-   0        0        0      787 2023-07-26 08:31:55.000000 trajectopy-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 08:32:55.093314 trajectopy-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1628 2023-07-19 07:37:04.000000 trajectopy-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:32:55.008690 trajectopy-0.3.1/test/
+-rw-rw-rw-   0        0        0     7503 2023-07-14 07:41:14.000000 trajectopy-0.3.1/test/test_alignment.py
+-rw-rw-rw-   0        0        0     5487 2023-07-25 08:37:59.000000 trajectopy-0.3.1/test/test_comparison.py
+-rw-rw-rw-   0        0        0     2347 2023-07-14 07:41:14.000000 trajectopy-0.3.1/test/test_settings.py
+-rw-rw-rw-   0        0        0     1372 2023-07-14 07:41:14.000000 trajectopy-0.3.1/test/test_sorting.py
+-rw-rw-rw-   0        0        0     6331 2023-07-14 07:41:14.000000 trajectopy-0.3.1/test/test_trajectory.py
+-rw-rw-rw-   0        0        0      339 2023-07-14 07:41:14.000000 trajectopy-0.3.1/test/testdata.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:32:55.016741 trajectopy-0.3.1/trajectopy/
+-rw-rw-rw-   0        0        0    35790 2023-07-18 14:52:08.000000 trajectopy-0.3.1/trajectopy/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/__init__.py
+-rw-rw-rw-   0        0        0      630 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:32:55.038455 trajectopy-0.3.1/trajectopy/alignment/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/alignment/__init__.py
+-rw-rw-rw-   0        0        0    39680 2023-07-17 09:26:50.000000 trajectopy-0.3.1/trajectopy/alignment/alignment.py
+-rw-rw-rw-   0        0        0     9340 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/alignment/data.py
+-rw-rw-rw-   0        0        0     2421 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/alignment/direct_helmert_transformation.py
+-rw-rw-rw-   0        0        0     5354 2023-07-25 08:11:16.000000 trajectopy-0.3.1/trajectopy/alignment/direct_leverarm.py
+-rw-rw-rw-   0        0        0     2181 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/alignment/direct_timeshift.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:32:55.040452 trajectopy-0.3.1/trajectopy/alignment/functional_model/
+-rw-rw-rw-   0        0        0        0 2023-07-18 14:52:08.000000 trajectopy-0.3.1/trajectopy/alignment/functional_model/__init__.py
+-rw-rw-rw-   0        0        0    16031 2023-07-25 08:11:16.000000 trajectopy-0.3.1/trajectopy/alignment/functional_model/equations.py
+-rw-rw-rw-   0        0        0     8022 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/alignment/functional_model/interface.py
+-rw-rw-rw-   0        0        0    19324 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/alignment/parameters.py
+-rw-rw-rw-   0        0        0     3910 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/alignment/util.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:32:55.045452 trajectopy-0.3.1/trajectopy/approximation/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/approximation/__init__.py
+-rw-rw-rw-   0        0        0     8005 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/approximation/cubic_approximation.py
+-rw-rw-rw-   0        0        0     5795 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/approximation/mls_approximation.py
+-rw-rw-rw-   0        0        0     5303 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/approximation/rot_approximation.py
+-rw-rw-rw-   0        0        0     6116 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/approximation/trajectory_approximation.py
+-rw-rw-rw-   0        0        0     4272 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/approximation/util.py
+-rw-rw-rw-   0        0        0     4843 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/approximation/voxelizer.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:32:55.047453 trajectopy-0.3.1/trajectopy/evaluation/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/evaluation/__init__.py
+-rw-rw-rw-   0        0        0    14911 2023-07-25 08:26:56.000000 trajectopy-0.3.1/trajectopy/evaluation/comparison.py
+-rw-rw-rw-   0        0        0     4872 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/evaluation/matching.py
+-rw-rw-rw-   0        0        0    29996 2023-07-25 08:30:17.000000 trajectopy-0.3.1/trajectopy/evaluation/trajectory_deviations.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:32:55.049308 trajectopy-0.3.1/trajectopy/gui/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/gui/__init__.py
+-rw-rw-rw-   0        0        0    14315 2023-07-25 07:49:54.000000 trajectopy-0.3.1/trajectopy/gui/main_window.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:32:55.054314 trajectopy-0.3.1/trajectopy/gui/managers/
+-rw-rw-rw-   0        0        0        0 2023-07-18 14:52:08.000000 trajectopy-0.3.1/trajectopy/gui/managers/__init__.py
+-rw-rw-rw-   0        0        0     4444 2023-07-25 08:11:16.000000 trajectopy-0.3.1/trajectopy/gui/managers/file_manager.py
+-rw-rw-rw-   0        0        0     1730 2023-07-25 08:11:16.000000 trajectopy-0.3.1/trajectopy/gui/managers/manager.py
+-rw-rw-rw-   0        0        0     3677 2023-07-19 15:01:54.000000 trajectopy-0.3.1/trajectopy/gui/managers/plot_manager.py
+-rw-rw-rw-   0        0        0     3812 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/gui/managers/session_manager.py
+-rw-rw-rw-   0        0        0    31367 2023-07-25 08:11:16.000000 trajectopy-0.3.1/trajectopy/gui/managers/trajectory_manager.py
+-rw-rw-rw-   0        0        0     8040 2023-07-17 09:26:50.000000 trajectopy-0.3.1/trajectopy/gui/managers/ui_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:32:55.059313 trajectopy-0.3.1/trajectopy/gui/models/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/gui/models/__init__.py
+-rw-rw-rw-   0        0        0    11907 2023-07-25 08:11:16.000000 trajectopy-0.3.1/trajectopy/gui/models/entry.py
+-rw-rw-rw-   0        0        0     1115 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/gui/models/property_model.py
+-rw-rw-rw-   0        0        0     3904 2023-07-17 09:26:50.000000 trajectopy-0.3.1/trajectopy/gui/models/result_model.py
+-rw-rw-rw-   0        0        0      983 2023-07-25 08:11:16.000000 trajectopy-0.3.1/trajectopy/gui/models/selection.py
+-rw-rw-rw-   0        0        0     4030 2023-07-25 08:11:16.000000 trajectopy-0.3.1/trajectopy/gui/models/table_model.py
+-rw-rw-rw-   0        0        0     4837 2023-07-25 08:11:16.000000 trajectopy-0.3.1/trajectopy/gui/models/trajectory_model.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:32:55.066315 trajectopy-0.3.1/trajectopy/gui/requests/
+-rw-rw-rw-   0        0        0        0 2023-07-18 14:52:08.000000 trajectopy-0.3.1/trajectopy/gui/requests/__init__.py
+-rw-rw-rw-   0        0        0      666 2023-07-17 09:26:50.000000 trajectopy-0.3.1/trajectopy/gui/requests/file_request.py
+-rw-rw-rw-   0        0        0      635 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/gui/requests/plot_requests.py
+-rw-rw-rw-   0        0        0      424 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/gui/requests/plot_settings_request.py
+-rw-rw-rw-   0        0        0      371 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/gui/requests/property_request.py
+-rw-rw-rw-   0        0        0      500 2023-07-25 08:11:16.000000 trajectopy-0.3.1/trajectopy/gui/requests/request.py
+-rw-rw-rw-   0        0        0      565 2023-07-17 09:26:50.000000 trajectopy-0.3.1/trajectopy/gui/requests/result_model_request.py
+-rw-rw-rw-   0        0        0      388 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/gui/requests/session_request.py
+-rw-rw-rw-   0        0        0     1029 2023-07-17 09:26:50.000000 trajectopy-0.3.1/trajectopy/gui/requests/trajectory_manager_request.py
+-rw-rw-rw-   0        0        0      593 2023-07-17 09:26:50.000000 trajectopy-0.3.1/trajectopy/gui/requests/trajectory_model_request.py
+-rw-rw-rw-   0        0        0      836 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/gui/requests/ui_request.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:32:55.067314 trajectopy-0.3.1/trajectopy/gui/resources/
+-rw-rw-rw-   0        0        0   120742 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/gui/resources/full-icon-poppins.png
+-rw-rw-rw-   0        0        0    24491 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/gui/resources/icon.png
+-rw-rw-rw-   0        0        0     1751 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/gui/util.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:32:55.076316 trajectopy-0.3.1/trajectopy/gui/views/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/gui/views/__init__.py
+-rw-rw-rw-   0        0        0     3757 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/gui/views/about_window.py
+-rw-rw-rw-   0        0        0     9601 2023-07-17 09:26:50.000000 trajectopy-0.3.1/trajectopy/gui/views/alignment_edit_window.py
+-rw-rw-rw-   0        0        0    21480 2023-07-19 07:37:04.000000 trajectopy-0.3.1/trajectopy/gui/views/plot_settings_window.py
+-rw-rw-rw-   0        0        0     2483 2023-07-17 09:26:50.000000 trajectopy-0.3.1/trajectopy/gui/views/progress_window.py
+-rw-rw-rw-   0        0        0     4013 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/gui/views/properties_window.py
+-rw-rw-rw-   0        0        0     6154 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/gui/views/result_context_menu.py
+-rw-rw-rw-   0        0        0     4717 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/gui/views/result_selection_window.py
+-rw-rw-rw-   0        0        0     4725 2023-07-19 15:01:54.000000 trajectopy-0.3.1/trajectopy/gui/views/result_table_view.py
+-rw-rw-rw-   0        0        0    54090 2023-07-25 08:15:18.000000 trajectopy-0.3.1/trajectopy/gui/views/settings_window.py
+-rw-rw-rw-   0        0        0    20852 2023-07-17 09:26:50.000000 trajectopy-0.3.1/trajectopy/gui/views/trajectory_context_menu.py
+-rw-rw-rw-   0        0        0     6744 2023-07-17 09:26:50.000000 trajectopy-0.3.1/trajectopy/gui/views/trajectory_table_view.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:32:55.080313 trajectopy-0.3.1/trajectopy/plotting/
+-rw-rw-rw-   0        0        0       81 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/plotting/__init__.py
+-rw-rw-rw-   0        0        0     2185 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/plotting/alignment_plot.py
+-rw-rw-rw-   0        0        0      498 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/plotting/default.mplstyle
+-rw-rw-rw-   0        0        0    21537 2023-07-25 08:11:16.000000 trajectopy-0.3.1/trajectopy/plotting/deviation_plot.py
+-rw-rw-rw-   0        0        0     7223 2023-07-19 15:01:54.000000 trajectopy-0.3.1/trajectopy/plotting/plot_tabs.py
+-rw-rw-rw-   0        0        0     3911 2023-07-25 08:11:16.000000 trajectopy-0.3.1/trajectopy/plotting/trajectory_plot.py
+-rw-rw-rw-   0        0        0     7826 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/plotting/util.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:32:55.085315 trajectopy-0.3.1/trajectopy/settings/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/settings/__init__.py
+-rw-rw-rw-   0        0        0     8256 2023-07-25 08:11:16.000000 trajectopy-0.3.1/trajectopy/settings/alignment_settings.py
+-rw-rw-rw-   0        0        0     1558 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/settings/approximation_settings.py
+-rw-rw-rw-   0        0        0     5669 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/settings/comparison_settings.py
+-rw-rw-rw-   0        0        0     3578 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/settings/core.py
+-rw-rw-rw-   0        0        0     1703 2023-07-19 07:37:04.000000 trajectopy-0.3.1/trajectopy/settings/plot_settings.py
+-rw-rw-rw-   0        0        0     2433 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/settings/processing_settings.py
+-rw-rw-rw-   0        0        0      945 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/settings/sorting_settings.py
+-rw-rw-rw-   0        0        0    35120 2023-07-25 08:11:16.000000 trajectopy-0.3.1/trajectopy/trajectory.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:32:55.092313 trajectopy-0.3.1/trajectopy/util/
+-rw-rw-rw-   0        0        0        0 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/util/__init__.py
+-rw-rw-rw-   0        0        0    18416 2023-07-26 08:31:37.000000 trajectopy-0.3.1/trajectopy/util/datahandling.py
+-rw-rw-rw-   0        0        0     1490 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/util/definitions.py
+-rw-rw-rw-   0        0        0      935 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/util/path.py
+-rw-rw-rw-   0        0        0     5389 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/util/printing.py
+-rw-rw-rw-   0        0        0    13611 2023-07-25 08:11:16.000000 trajectopy-0.3.1/trajectopy/util/reading.py
+-rw-rw-rw-   0        0        0     1956 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/util/rotationset.py
+-rw-rw-rw-   0        0        0    16143 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/util/spatialsorter.py
+-rw-rw-rw-   0        0        0      973 2023-07-14 07:41:14.000000 trajectopy-0.3.1/trajectopy/util/trajectory_processing_state.py
+-rw-rw-rw-   0        0        0        5 2023-07-26 08:31:52.000000 trajectopy-0.3.1/trajectopy/version
+drwxrwxrwx   0        0        0        0 2023-07-26 08:32:55.033439 trajectopy-0.3.1/trajectopy.egg-info/
+-rw-rw-rw-   0        0        0    19879 2023-07-26 08:32:54.000000 trajectopy-0.3.1/trajectopy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3943 2023-07-26 08:32:54.000000 trajectopy-0.3.1/trajectopy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:32:54.000000 trajectopy-0.3.1/trajectopy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-26 08:32:54.000000 trajectopy-0.3.1/trajectopy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-14 07:43:35.000000 trajectopy-0.3.1/trajectopy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      180 2023-07-26 08:32:54.000000 trajectopy-0.3.1/trajectopy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-26 08:32:54.000000 trajectopy-0.3.1/trajectopy.egg-info/top_level.txt
```

### Comparing `trajectopy-0.3.0/LICENSE` & `trajectopy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/PKG-INFO` & `trajectopy-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trajectopy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Trajectory Evaluation in Python
 Home-page: https://github.com/gereon-t/trajectopy
 Author: Gereon Tombrink
 Author-email: tombrink@igg.uni-bonn.de
 License: GPLv3
 Keywords: trajectory,evaluation,alignment,similarity,leverarm,epsg,robotics
 Requires-Python: >=3.9
@@ -60,15 +60,15 @@
 
 When you start the program, you can import trajectories, for example, from the provided [example data folder](https://github.com/gereon-t/trajectopy/tree/main/example_data). This can be done by dragging the file into the trajectory table or clicking the "Add" button below the table.
 
 To visualize the trajectories, you can select them, right-click and choose "Trajectory 2D" from the "View" menu, or simply press V.
 
 ![](.images/plot.png)
 
-To prepare for the comparison, you need to align the estimated trajectories with the ground truth trajectory. To do this, you can access the settings of each trajectory to be aligned by right-clicking on it and selecting "Settings" or by pressing S. By default, a similarity transformation is configured, assuming observation uncertainties of 1 meter in position and 1 degree in rotation. These default settings are suitable for most quick alignments.
+To prepare for the comparison, you need to align the estimated trajectories with the ground truth trajectory. To do this, you can access the settings of each trajectory to be aligned by right-clicking on it and selecting "Settings" or by pressing S. By default, a rigid-body transformation is configured, assuming observation uncertainties of 1 meter in position and 1 degree in rotation. These default settings are suitable for most quick alignments.
 
 ![](.images/settings.png)
 
 Next, you select the ground truth trajectory as the reference, either through the right-click menu or by pressing R. Finally, you initiate the alignment by selecting "Action," then "Align with Reference," and choosing the "Nearest Temporal" option. This aligns both trajectories based on their timestamps. You will see two new trajectories and two new sets of results. These are the aligned trajectories and the alignment parameters estimated during the process.
 
 Besides "Nearest Temporal" you can also match trajectories using interpolation or nearest-neighbor queries. When aligning trajectories using the interpolation method, positions of the trajectories at non-observed timestamps are interpolated based on the available data points. This can be useful when the timestamps of the two trajectories don't exactly match, and some intermediate positions are required to establish correspondence between them.
```

### Comparing `trajectopy-0.3.0/README.md` & `trajectopy-0.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 When you start the program, you can import trajectories, for example, from the provided [example data folder](https://github.com/gereon-t/trajectopy/tree/main/example_data). This can be done by dragging the file into the trajectory table or clicking the "Add" button below the table.
 
 To visualize the trajectories, you can select them, right-click and choose "Trajectory 2D" from the "View" menu, or simply press V.
 
 ![](.images/plot.png)
 
-To prepare for the comparison, you need to align the estimated trajectories with the ground truth trajectory. To do this, you can access the settings of each trajectory to be aligned by right-clicking on it and selecting "Settings" or by pressing S. By default, a similarity transformation is configured, assuming observation uncertainties of 1 meter in position and 1 degree in rotation. These default settings are suitable for most quick alignments.
+To prepare for the comparison, you need to align the estimated trajectories with the ground truth trajectory. To do this, you can access the settings of each trajectory to be aligned by right-clicking on it and selecting "Settings" or by pressing S. By default, a rigid-body transformation is configured, assuming observation uncertainties of 1 meter in position and 1 degree in rotation. These default settings are suitable for most quick alignments.
 
 ![](.images/settings.png)
 
 Next, you select the ground truth trajectory as the reference, either through the right-click menu or by pressing R. Finally, you initiate the alignment by selecting "Action," then "Align with Reference," and choosing the "Nearest Temporal" option. This aligns both trajectories based on their timestamps. You will see two new trajectories and two new sets of results. These are the aligned trajectories and the alignment parameters estimated during the process.
 
 Besides "Nearest Temporal" you can also match trajectories using interpolation or nearest-neighbor queries. When aligning trajectories using the interpolation method, positions of the trajectories at non-observed timestamps are interpolated based on the available data points. This can be useful when the timestamps of the two trajectories don't exactly match, and some intermediate positions are required to establish correspondence between them.
```

### Comparing `trajectopy-0.3.0/pyproject.toml` & `trajectopy-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trajectopy"
-version = "0.3.0"
+version = "0.3.1"
 description = "Trajectory Evaluation in Python"
 authors = ["Gereon Tombrink <tombrink@igg.uni-bonn.de>"]
 license = "GPLv3"
 keywords = ["trajectory", "evaluation", "alignment", "similarity", "leverarm", "epsg", "robotics"]
 readme = "README.md"
 homepage = "https://github.com/gereon-t/trajectopy"
 repository = "https://github.com/gereon-t/trajectopy.git"
```

### Comparing `trajectopy-0.3.0/setup.py` & `trajectopy-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/test/test_alignment.py` & `trajectopy-0.3.1/test/test_alignment.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/test/test_comparison.py` & `trajectopy-0.3.1/test/test_comparison.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/test/test_settings.py` & `trajectopy-0.3.1/test/test_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/test/test_sorting.py` & `trajectopy-0.3.1/test/test_sorting.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/test/test_trajectory.py` & `trajectopy-0.3.1/test/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/LICENSE` & `trajectopy-0.3.1/trajectopy/LICENSE`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/__main__.py` & `trajectopy-0.3.1/trajectopy/__main__.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/alignment/alignment.py` & `trajectopy-0.3.1/trajectopy/alignment/alignment.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/alignment/data.py` & `trajectopy-0.3.1/trajectopy/alignment/data.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/alignment/direct_helmert_transformation.py` & `trajectopy-0.3.1/trajectopy/alignment/direct_helmert_transformation.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/alignment/direct_leverarm.py` & `trajectopy-0.3.1/trajectopy/alignment/direct_leverarm.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/alignment/direct_timeshift.py` & `trajectopy-0.3.1/trajectopy/alignment/direct_timeshift.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/alignment/functional_model/equations.py` & `trajectopy-0.3.1/trajectopy/alignment/functional_model/equations.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/alignment/functional_model/interface.py` & `trajectopy-0.3.1/trajectopy/alignment/functional_model/interface.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/alignment/parameters.py` & `trajectopy-0.3.1/trajectopy/alignment/parameters.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/alignment/util.py` & `trajectopy-0.3.1/trajectopy/alignment/util.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/approximation/cubic_approximation.py` & `trajectopy-0.3.1/trajectopy/approximation/cubic_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/approximation/mls_approximation.py` & `trajectopy-0.3.1/trajectopy/approximation/mls_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/approximation/rot_approximation.py` & `trajectopy-0.3.1/trajectopy/approximation/rot_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/approximation/trajectory_approximation.py` & `trajectopy-0.3.1/trajectopy/approximation/trajectory_approximation.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/approximation/util.py` & `trajectopy-0.3.1/trajectopy/approximation/util.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/approximation/voxelizer.py` & `trajectopy-0.3.1/trajectopy/approximation/voxelizer.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/evaluation/comparison.py` & `trajectopy-0.3.1/trajectopy/evaluation/comparison.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/evaluation/matching.py` & `trajectopy-0.3.1/trajectopy/evaluation/matching.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/evaluation/trajectory_deviations.py` & `trajectopy-0.3.1/trajectopy/evaluation/trajectory_deviations.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/main_window.py` & `trajectopy-0.3.1/trajectopy/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/managers/file_manager.py` & `trajectopy-0.3.1/trajectopy/gui/managers/file_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/managers/manager.py` & `trajectopy-0.3.1/trajectopy/gui/managers/manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/managers/plot_manager.py` & `trajectopy-0.3.1/trajectopy/gui/managers/plot_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/managers/session_manager.py` & `trajectopy-0.3.1/trajectopy/gui/managers/session_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/managers/trajectory_manager.py` & `trajectopy-0.3.1/trajectopy/gui/managers/trajectory_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/managers/ui_manager.py` & `trajectopy-0.3.1/trajectopy/gui/managers/ui_manager.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/models/entry.py` & `trajectopy-0.3.1/trajectopy/gui/models/entry.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/models/property_model.py` & `trajectopy-0.3.1/trajectopy/gui/models/property_model.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/models/result_model.py` & `trajectopy-0.3.1/trajectopy/gui/models/result_model.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/models/selection.py` & `trajectopy-0.3.1/trajectopy/gui/models/selection.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/models/table_model.py` & `trajectopy-0.3.1/trajectopy/gui/models/table_model.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/models/trajectory_model.py` & `trajectopy-0.3.1/trajectopy/gui/models/trajectory_model.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/requests/file_request.py` & `trajectopy-0.3.1/trajectopy/gui/requests/file_request.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/requests/plot_requests.py` & `trajectopy-0.3.1/trajectopy/gui/requests/plot_requests.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/requests/result_model_request.py` & `trajectopy-0.3.1/trajectopy/gui/requests/result_model_request.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/requests/trajectory_manager_request.py` & `trajectopy-0.3.1/trajectopy/gui/requests/trajectory_manager_request.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/requests/trajectory_model_request.py` & `trajectopy-0.3.1/trajectopy/gui/requests/trajectory_model_request.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/requests/ui_request.py` & `trajectopy-0.3.1/trajectopy/gui/requests/ui_request.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/resources/full-icon-poppins.png` & `trajectopy-0.3.1/trajectopy/gui/resources/full-icon-poppins.png`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/resources/icon.png` & `trajectopy-0.3.1/trajectopy/gui/resources/icon.png`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/util.py` & `trajectopy-0.3.1/trajectopy/gui/util.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/views/about_window.py` & `trajectopy-0.3.1/trajectopy/gui/views/about_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/views/alignment_edit_window.py` & `trajectopy-0.3.1/trajectopy/gui/views/alignment_edit_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/views/plot_settings_window.py` & `trajectopy-0.3.1/trajectopy/gui/views/plot_settings_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/views/progress_window.py` & `trajectopy-0.3.1/trajectopy/gui/views/progress_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/views/properties_window.py` & `trajectopy-0.3.1/trajectopy/gui/views/properties_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/views/result_context_menu.py` & `trajectopy-0.3.1/trajectopy/gui/views/result_context_menu.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/views/result_selection_window.py` & `trajectopy-0.3.1/trajectopy/gui/views/result_selection_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/views/result_table_view.py` & `trajectopy-0.3.1/trajectopy/gui/views/result_table_view.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/views/settings_window.py` & `trajectopy-0.3.1/trajectopy/gui/views/settings_window.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/views/trajectory_context_menu.py` & `trajectopy-0.3.1/trajectopy/gui/views/trajectory_context_menu.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/gui/views/trajectory_table_view.py` & `trajectopy-0.3.1/trajectopy/gui/views/trajectory_table_view.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/plotting/alignment_plot.py` & `trajectopy-0.3.1/trajectopy/plotting/alignment_plot.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/plotting/deviation_plot.py` & `trajectopy-0.3.1/trajectopy/plotting/deviation_plot.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/plotting/plot_tabs.py` & `trajectopy-0.3.1/trajectopy/plotting/plot_tabs.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/plotting/trajectory_plot.py` & `trajectopy-0.3.1/trajectopy/plotting/trajectory_plot.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/plotting/util.py` & `trajectopy-0.3.1/trajectopy/plotting/util.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/settings/alignment_settings.py` & `trajectopy-0.3.1/trajectopy/settings/alignment_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/settings/approximation_settings.py` & `trajectopy-0.3.1/trajectopy/settings/approximation_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/settings/comparison_settings.py` & `trajectopy-0.3.1/trajectopy/settings/comparison_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/settings/core.py` & `trajectopy-0.3.1/trajectopy/settings/core.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/settings/plot_settings.py` & `trajectopy-0.3.1/trajectopy/settings/plot_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/settings/processing_settings.py` & `trajectopy-0.3.1/trajectopy/settings/processing_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/settings/sorting_settings.py` & `trajectopy-0.3.1/trajectopy/settings/sorting_settings.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/trajectory.py` & `trajectopy-0.3.1/trajectopy/trajectory.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/util/datahandling.py` & `trajectopy-0.3.1/trajectopy/util/datahandling.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Trajectopy - Trajectory Evaluation in Python
 
 Gereon Tombrink, 2023
 mail@gtombrink.de
 """
 import logging
 from dataclasses import dataclass
-from typing import Callable, Tuple, Union
+from typing import Any, Callable, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 
 from trajectopy.approximation.util import skew_symmetric_matrix
 
@@ -35,16 +35,16 @@
         populated_grid_cells() -> np.ndarray:
             Returns the x and y coordinates and values of the populated grid cells.
         scaled_grid_cells() -> np.ndarray:
             Returns the x and y coordinates and values of the populated grid cells, scaled by the pixel size.
     """
 
     full_grid: np.ndarray
-    x_bin_locations: list[int]
-    y_bin_locations: list[int]
+    x_bin_locations: np.ndarray
+    y_bin_locations: np.ndarray
     pixel_size: float
 
     @property
     def values(self) -> np.ndarray:
         return self.full_grid[self.x_bin_locations, self.y_bin_locations]
 
     @property
@@ -76,15 +76,15 @@
 
     Args:
         dicts (Tuple[dict]): A tuple of dictionaries to be merged.
 
     Returns:
         dict: A dictionary containing the merged key-value pairs.
     """
-    merged_dict = {}
+    merged_dict: dict[Any, Any] = {}
     for i, d in enumerate(dicts):
         for k, v in d.items():
             if k not in merged_dict:
                 merged_dict[k] = ["-"] * len(dicts)
             merged_dict[k][i] = v
     return merged_dict
 
@@ -220,15 +220,15 @@
         int: The rounded odd integer.
     """
     idx = s % 2 < 1
     s = np.floor(s)
 
     if idx:
         s += 1
-    return s
+    return int(s)
 
 
 def lengths_from_xyz(xyz: np.ndarray) -> np.ndarray:
     """
     Computes the cumulative distance along a path defined by a sequence of
     3D points.
 
@@ -249,15 +249,15 @@
 
     diff = xyz_2 - xyz_1
 
     dists = np.linalg.norm(diff, axis=1)
     return np.r_[0, np.cumsum(dists)]
 
 
-def nearest_point(*, p: np.ndarray, line_pts: list) -> np.ndarray:
+def nearest_point(*, p: np.ndarray, line_pts: list) -> tuple[np.ndarray, float]:
     """
     Finds the nearest point on a 3D line to a given point.
 
     Args:
         p (np.ndarray): The point to find the nearest point to.
         line_pts (list): A list of two points that define the 3D line.
 
@@ -441,15 +441,15 @@
             [
                 [np.cos(gamma), -np.sin(gamma), 0],
                 [np.sin(gamma), np.cos(gamma), 0],
                 [0, 0, 1],
             ]
         )
     else:
-        print("rot_z: Unknown dimension!")
+        raise ValueError("rot_z: Unknown dimension!")
 
 
 def filter_from_limits(tstamps: np.ndarray, gap_limits: np.ndarray) -> np.ndarray:
     """
     Creates a boolean filter which filters tstamps
     according to limits defined in gap_limits
 
@@ -560,16 +560,16 @@
         data (np.ndarray): data values [nx1]
         grid_mp (int, optional): Number of grid bins in megapixels.
                                  Defaults to 12.
 
     Returns:
         np.ndarray: grid with averaged values
     """
-    dx = max(xyz[:, 0]) - min(xyz[:, 0])
-    dy = max(xyz[:, 1]) - min(xyz[:, 1])
+    dx = max(1, max(xyz[:, 0]) - min(xyz[:, 0]))
+    dy = max(1, max(xyz[:, 1]) - min(xyz[:, 1]))
     ratio = dy / dx
 
     px = int(np.sqrt(grid_mp * 1e6 / ratio))
     py = int(ratio * px)
     pixel_size = np.mean([dx / px, dy / py])
 
     grid_x = np.linspace(min(xyz[:, 0]), max(xyz[:, 0]), px)
@@ -585,9 +585,12 @@
     y_bin_locations = grid_df_mean.iloc[:, 1].to_numpy(dtype=int)
     grid_values = grid_df_mean.iloc[:, 2].to_numpy(dtype=float)
 
     full_grid = np.zeros((px, py))
     full_grid[x_bin_locations, y_bin_locations] = grid_values
 
     return Grid(
-        full_grid=full_grid, x_bin_locations=x_bin_locations, y_bin_locations=y_bin_locations, pixel_size=pixel_size
+        full_grid=full_grid,
+        x_bin_locations=x_bin_locations,
+        y_bin_locations=y_bin_locations,
+        pixel_size=float(pixel_size),
     )
```

### Comparing `trajectopy-0.3.0/trajectopy/util/definitions.py` & `trajectopy-0.3.1/trajectopy/util/definitions.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/util/path.py` & `trajectopy-0.3.1/trajectopy/util/path.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/util/printing.py` & `trajectopy-0.3.1/trajectopy/util/printing.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/util/reading.py` & `trajectopy-0.3.1/trajectopy/util/reading.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/util/rotationset.py` & `trajectopy-0.3.1/trajectopy/util/rotationset.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/util/spatialsorter.py` & `trajectopy-0.3.1/trajectopy/util/spatialsorter.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy/util/trajectory_processing_state.py` & `trajectopy-0.3.1/trajectopy/util/trajectory_processing_state.py`

 * *Files identical despite different names*

### Comparing `trajectopy-0.3.0/trajectopy.egg-info/PKG-INFO` & `trajectopy-0.3.1/trajectopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trajectopy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Trajectory Evaluation in Python
 Home-page: https://github.com/gereon-t/trajectopy
 Author: Gereon Tombrink
 Author-email: tombrink@igg.uni-bonn.de
 License: GPLv3
 Keywords: trajectory,evaluation,alignment,similarity,leverarm,epsg,robotics
 Requires-Python: >=3.9
@@ -60,15 +60,15 @@
 
 When you start the program, you can import trajectories, for example, from the provided [example data folder](https://github.com/gereon-t/trajectopy/tree/main/example_data). This can be done by dragging the file into the trajectory table or clicking the "Add" button below the table.
 
 To visualize the trajectories, you can select them, right-click and choose "Trajectory 2D" from the "View" menu, or simply press V.
 
 ![](.images/plot.png)
 
-To prepare for the comparison, you need to align the estimated trajectories with the ground truth trajectory. To do this, you can access the settings of each trajectory to be aligned by right-clicking on it and selecting "Settings" or by pressing S. By default, a similarity transformation is configured, assuming observation uncertainties of 1 meter in position and 1 degree in rotation. These default settings are suitable for most quick alignments.
+To prepare for the comparison, you need to align the estimated trajectories with the ground truth trajectory. To do this, you can access the settings of each trajectory to be aligned by right-clicking on it and selecting "Settings" or by pressing S. By default, a rigid-body transformation is configured, assuming observation uncertainties of 1 meter in position and 1 degree in rotation. These default settings are suitable for most quick alignments.
 
 ![](.images/settings.png)
 
 Next, you select the ground truth trajectory as the reference, either through the right-click menu or by pressing R. Finally, you initiate the alignment by selecting "Action," then "Align with Reference," and choosing the "Nearest Temporal" option. This aligns both trajectories based on their timestamps. You will see two new trajectories and two new sets of results. These are the aligned trajectories and the alignment parameters estimated during the process.
 
 Besides "Nearest Temporal" you can also match trajectories using interpolation or nearest-neighbor queries. When aligning trajectories using the interpolation method, positions of the trajectories at non-observed timestamps are interpolated based on the available data points. This can be useful when the timestamps of the two trajectories don't exactly match, and some intermediate positions are required to establish correspondence between them.
```

### Comparing `trajectopy-0.3.0/trajectopy.egg-info/SOURCES.txt` & `trajectopy-0.3.1/trajectopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*


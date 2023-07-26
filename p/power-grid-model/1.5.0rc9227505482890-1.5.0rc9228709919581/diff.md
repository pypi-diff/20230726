# Comparing `tmp/power-grid-model-1.5.0rc9227505482890.tar.gz` & `tmp/power-grid-model-1.5.0rc9228709919581.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power-grid-model-1.5.0rc9227505482890.tar", last modified: Tue Jul 25 11:18:50 2023, max compression
+gzip compressed data, was "power-grid-model-1.5.0rc9228709919581.tar", last modified: Wed Jul 26 06:28:29 2023, max compression
```

## Comparing `power-grid-model-1.5.0rc9227505482890.tar` & `power-grid-model-1.5.0rc9228709919581.tar`

### file list

```diff
@@ -1,593 +1,593 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.428875 power-grid-model-1.5.0rc9227505482890/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-25 11:18:50.428875 power-grid-model-1.5.0rc9227505482890/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 11:18:04.000000 power-grid-model-1.5.0rc9227505482890/PYPI_VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.368874 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.368874 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.360875 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.372875 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.372875 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.372875 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/
--rw-r--r--   0 runner    (1001) docker     (123)    30276 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.372875 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20689 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.372875 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    53721 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.376875 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    41768 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    21344 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30907 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.376875 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.376875 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.376875 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h
--rw-r--r--   0 runner    (1001) docker     (123)    55882 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.376875 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/src/buffer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    93852 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/src/handle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/src/handle.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/src/meta_data.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/src/model.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/src/options.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/src/options.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 11:18:50.428875 power-grid-model-1.5.0rc9227505482890/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.364874 power-grid-model-1.5.0rc9227505482890/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.376875 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.380874 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/core/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/core/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/core/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/core/index_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/core/power_grid_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/core/power_grid_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/core/power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21661 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.380874 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/validation/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    35027 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/validation/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/validation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29999 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model/validation/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.380874 power-grid-model-1.5.0rc9227505482890/src/power_grid_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-25 11:18:50.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35498 2023-07-25 11:18:50.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:18:50.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-25 11:18:50.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 11:18:50.000000 power-grid-model-1.5.0rc9227505482890/src/power_grid_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.368874 power-grid-model-1.5.0rc9227505482890/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.368874 power-grid-model-1.5.0rc9227505482890/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.364874 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.380874 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.380874 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.384875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.384875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.384875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.388875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-incomplete-input/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.388875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.388875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.388875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-newton/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-newton/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-newton/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-newton/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-newton/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.392875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-i-n-optional/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-i-n-optional/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-i-n-optional/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.392875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/gaia-example/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/gaia-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/gaia-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/gaia-example/gaia_grid.gnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/gaia-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/gaia-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/gaia-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/gaia-example/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.392875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/multi-source-with-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/multi-source-with-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/multi-source-with-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/multi-source-with-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/multi-source-with-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/multi-source-with-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.364874 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.364874 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.364874 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.392875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.392875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.396875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.396875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.396875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.396875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.396875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.400875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.400875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.364874 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.400875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/basic-node/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.400875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.404875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.404875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.404875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.404875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.404875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.408875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.408875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.364874 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.364874 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.408875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.408875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.364874 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.412875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.412875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.412875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/r-state-estimation/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/r-state-estimation/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/r-state-estimation/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/r-state-estimation/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/r-state-estimation/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/r-state-estimation/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/r-state-estimation/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.412875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/three-winding-transformer/
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/three-winding-transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/three-winding-transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/three-winding-transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/three-winding-transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/three-winding-transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/three-winding-transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.416875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-example/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-example/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-example/vision_grid.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-example/vision_grid.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.416875 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-validation-network/
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-validation-network/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-validation-network/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-validation-network/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-validation-network/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-validation-network/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-validation-network/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-validation-network/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-validation-network/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.368874 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.416875 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/single_phase_to_ground/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/single_phase_to_ground/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/single_phase_to_ground/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/single_phase_to_ground/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/single_phase_to_ground/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   243263 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/single_phase_to_ground/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/single_phase_to_ground/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.416875 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/three_phase/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/three_phase/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/three_phase/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/three_phase/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/three_phase/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58928 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/three_phase/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/three_phase/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/three_phase/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/three_phase/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.420875 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   236282 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.420875 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase_to_ground/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase_to_ground/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase_to_ground/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase_to_ground/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase_to_ground/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)   242819 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase_to_ground/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase_to_ground/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.368874 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.420875 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.420875 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr-no-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr-no-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr-no-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr-no-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr-no-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.420875 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.424875 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/dummy-test-sym/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/dummy-test-sym/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/dummy-test-sym/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/dummy-test-sym/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/dummy-test-sym/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/dummy-test-sym/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.424875 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.424875 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/residual-test/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/residual-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/residual-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/residual-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/residual-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/residual-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/residual-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.424875 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/single-line-load/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/single-line-load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/single-line-load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/single-line-load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/single-line-load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/single-line-load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/single-line-load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.424875 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/three_winding_transformer/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.424875 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.428875 power-grid-model-1.5.0rc9227505482890/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/unit/test_0Z_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/unit/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/unit/test_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/unit/test_power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/unit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:18:50.428875 power-grid-model-1.5.0rc9227505482890/tests/unit/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/unit/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/unit/validation/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/unit/validation/test_batch_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/unit/validation/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    29354 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/unit/validation/test_input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/unit/validation/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/unit/validation/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-07-25 11:18:01.000000 power-grid-model-1.5.0rc9227505482890/tests/unit/validation/test_validation_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.550681 power-grid-model-1.5.0rc9228709919581/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-26 06:28:29.550681 power-grid-model-1.5.0rc9228709919581/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-26 06:27:42.000000 power-grid-model-1.5.0rc9228709919581/PYPI_VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.482681 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.482681 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.478681 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.486681 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.486681 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.486681 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)    30276 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.486681 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20689 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.490681 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    53721 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.490681 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41768 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25143 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30907 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.490681 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.490681 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.490681 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    55882 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.490681 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/src/buffer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    93852 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/src/handle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/src/handle.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/src/meta_data.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/src/model.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/src/options.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/src/options.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 06:28:29.550681 power-grid-model-1.5.0rc9228709919581/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.478681 power-grid-model-1.5.0rc9228709919581/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.494681 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.494681 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/core/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/core/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/core/index_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/core/power_grid_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/core/power_grid_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22015 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/core/power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21661 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.494681 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/validation/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35027 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/validation/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/validation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29999 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model/validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.494681 power-grid-model-1.5.0rc9228709919581/src/power_grid_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-26 06:28:29.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35498 2023-07-26 06:28:29.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 06:28:29.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-26 06:28:29.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 06:28:29.000000 power-grid-model-1.5.0rc9228709919581/src/power_grid_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.482681 power-grid-model-1.5.0rc9228709919581/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.482681 power-grid-model-1.5.0rc9228709919581/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.482681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.494681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.494681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.498681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.498681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.498681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.498681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-incomplete-input/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.502681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.502681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.506681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-newton/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-newton/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-newton/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-newton/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-newton/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.506681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-i-n-optional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-i-n-optional/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-i-n-optional/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.506681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/gaia-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/gaia-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/gaia-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/gaia-example/gaia_grid.gnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/gaia-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/gaia-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/gaia-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/gaia-example/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.506681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/multi-source-with-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/multi-source-with-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/multi-source-with-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/multi-source-with-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/multi-source-with-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/multi-source-with-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.482681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.478681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.478681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.506681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.510681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.510681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.510681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.510681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.510681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.514681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.514681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.514681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.482681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.514681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/basic-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.514681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.518681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.518681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.518681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.518681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.522681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.522681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.522681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.482681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.482681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.526681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.526681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.482681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.526681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.530681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.530681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/r-state-estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/r-state-estimation/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/r-state-estimation/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/r-state-estimation/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/r-state-estimation/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/r-state-estimation/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/r-state-estimation/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.530681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/three-winding-transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/three-winding-transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/three-winding-transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/three-winding-transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/three-winding-transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/three-winding-transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/three-winding-transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.530681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-example/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-example/vision_grid.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-example/vision_grid.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.534681 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-validation-network/
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-validation-network/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-validation-network/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-validation-network/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-validation-network/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-validation-network/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-validation-network/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-validation-network/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-validation-network/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.482681 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.534681 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/single_phase_to_ground/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/single_phase_to_ground/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/single_phase_to_ground/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/single_phase_to_ground/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/single_phase_to_ground/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   243263 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/single_phase_to_ground/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/single_phase_to_ground/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.534681 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/three_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/three_phase/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/three_phase/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/three_phase/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/three_phase/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58928 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/three_phase/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/three_phase/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/three_phase/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/three_phase/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.538681 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   236282 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.538681 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase_to_ground/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase_to_ground/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase_to_ground/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase_to_ground/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase_to_ground/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)   242819 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase_to_ground/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase_to_ground/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.482681 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.538681 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.538681 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr-no-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr-no-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr-no-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr-no-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr-no-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.542681 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.542681 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/dummy-test-sym/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/dummy-test-sym/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/dummy-test-sym/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/dummy-test-sym/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/dummy-test-sym/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/dummy-test-sym/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.542681 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.542681 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/residual-test/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/residual-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/residual-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/residual-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/residual-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/residual-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/residual-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.542681 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/single-line-load/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/single-line-load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/single-line-load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/single-line-load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/single-line-load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/single-line-load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/single-line-load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.546681 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/three_winding_transformer/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.546681 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.546681 power-grid-model-1.5.0rc9228709919581/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/unit/test_0Z_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/unit/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/unit/test_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/unit/test_power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/unit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:28:29.550681 power-grid-model-1.5.0rc9228709919581/tests/unit/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/unit/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/unit/validation/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/unit/validation/test_batch_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/unit/validation/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29354 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/unit/validation/test_input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/unit/validation/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/unit/validation/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-07-26 06:27:34.000000 power-grid-model-1.5.0rc9228709919581/tests/unit/validation/test_validation_functions.py
```

### Comparing `power-grid-model-1.5.0rc9227505482890/LICENSE` & `power-grid-model-1.5.0rc9228709919581/LICENSE`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/PKG-INFO` & `power-grid-model-1.5.0rc9228709919581/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9227505482890
+Version: 1.5.0rc9228709919581
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9227505482890/README.md` & `power-grid-model-1.5.0rc9228709919581/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/CMakeLists.txt` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_gen/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -157,21 +157,14 @@
 class UnknownAttributeName : public PowerGridError {
    public:
     explicit UnknownAttributeName(std::string const &attr_name) {
         append_msg("Unknown attribute name!" + attr_name + "\n");
     }
 };
 
-class NoShortCircuit : public PowerGridError {
-   public:
-    NoShortCircuit() {
-        append_msg("No faults present in short circuit calculation!\n");
-    }
-};
-
 class InvalidShortCircuitType : public PowerGridError {
    public:
     explicit InvalidShortCircuitType(FaultType short_circuit_type) {
         append_msg("The short circuit type (" + std::to_string(static_cast<IntS>(short_circuit_type)) +
                    ") is invalid!\n");
     }
     InvalidShortCircuitType(bool sym, FaultType short_circuit_type) {
```

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/state.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/main_core/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -76,129 +76,133 @@
             for (Idx source_number = source_bus_indptr[bus_number]; source_number != source_bus_indptr[bus_number + 1];
                  ++source_number) {
                 ComplexTensor<sym> const y_source = y_bus.math_model_param().source_param[source_number];
                 diagonal_element += y_source;  // add y_source to the diagonal of Ybus
                 u_bus += dot(y_source, ComplexValue<sym>{input.source[source_number] *
                                                          source_voltage_ref});  // rhs += Y_source * U_source * c
             }
-            // add all faults
-            for (Idx fault_number = fault_bus_indptr[bus_number]; fault_number != fault_bus_indptr[bus_number + 1];
-                 ++fault_number) {
-                DoubleComplex const y_fault = input.faults[fault_number].y_fault;
-                if (std::isinf(y_fault.real())) {
-                    assert(std::isinf(y_fault.imag()));
-                    infinite_admittance_fault_counter[bus_number] += 1;
-                    if (fault_type == FaultType::three_phase) {  // three phase fault
-                        for (Idx data_index = y_bus.row_indptr_lu()[bus_number];
-                             data_index != y_bus.row_indptr_lu()[bus_number + 1]; ++data_index) {
-                            Idx const col_data_index = y_bus.lu_transpose_entry()[data_index];
-                            // mat_data[:,bus] = 0
-                            mat_data_[col_data_index] = ComplexTensor<sym>{0};
-                        }
-                        // mat_data[bus,bus] = -1
-                        diagonal_element = ComplexTensor<sym>{-1};
-                        u_bus = ComplexValue<sym>{0};  // update rhs
-                    }
-                    if constexpr (!sym) {
-                        if (fault_type == FaultType::single_phase_to_ground) {
+            // skip if no fault
+            if (!input.faults.empty()) {
+                // add all faults
+                for (Idx fault_number = fault_bus_indptr[bus_number]; fault_number != fault_bus_indptr[bus_number + 1];
+                     ++fault_number) {
+                    DoubleComplex const y_fault = input.faults[fault_number].y_fault;
+                    if (std::isinf(y_fault.real())) {
+                        assert(std::isinf(y_fault.imag()));
+                        infinite_admittance_fault_counter[bus_number] += 1;
+                        if (fault_type == FaultType::three_phase) {  // three phase fault
                             for (Idx data_index = y_bus.row_indptr_lu()[bus_number];
                                  data_index != y_bus.row_indptr_lu()[bus_number + 1]; ++data_index) {
                                 Idx const col_data_index = y_bus.lu_transpose_entry()[data_index];
-                                // mat_data[:,bus][:, phase_1] = 0
-                                mat_data_[col_data_index].col(phase_1) = 0;
+                                // mat_data[:,bus] = 0
+                                mat_data_[col_data_index] = ComplexTensor<sym>{0};
+                            }
+                            // mat_data[bus,bus] = -1
+                            diagonal_element = ComplexTensor<sym>{-1};
+                            u_bus = ComplexValue<sym>{0};  // update rhs
+                        }
+                        if constexpr (!sym) {
+                            if (fault_type == FaultType::single_phase_to_ground) {
+                                for (Idx data_index = y_bus.row_indptr_lu()[bus_number];
+                                     data_index != y_bus.row_indptr_lu()[bus_number + 1]; ++data_index) {
+                                    Idx const col_data_index = y_bus.lu_transpose_entry()[data_index];
+                                    // mat_data[:,bus][:, phase_1] = 0
+                                    mat_data_[col_data_index].col(phase_1) = 0;
+                                }
+                                // mat_data[bus,bus][phase_1, phase_1] = -1
+                                diagonal_element(phase_1, phase_1) = -1;
+                                u_bus(phase_1) = 0;  // update rhs
+                            }
+                            else if (fault_type == FaultType::two_phase) {
+                                for (Idx data_index = y_bus.row_indptr_lu()[bus_number];
+                                     data_index != y_bus.row_indptr_lu()[bus_number + 1]; ++data_index) {
+                                    Idx const col_data_index = y_bus.lu_transpose_entry()[data_index];
+                                    // mat_data[:,bus][:, phase_1] += mat_data[:,bus][:, phase_2]
+                                    // mat_data[:,bus][:, phase_2] = 0
+                                    mat_data_[col_data_index].col(phase_1) += mat_data_[col_data_index].col(phase_2);
+                                    mat_data_[col_data_index].col(phase_2) = 0;
+                                }
+                                // mat_data[bus,bus][phase_1, phase_2] = -1
+                                // mat_data[bus,bus][phase_2, phase_2] = 1
+                                diagonal_element(phase_1, phase_2) = -1;
+                                diagonal_element(phase_2, phase_2) = 1;
+                                // update rhs
+                                u_bus(phase_2) += u_bus(phase_1);
+                                u_bus(phase_1) = 0;
+                            }
+                            else if (fault_type == FaultType::two_phase_to_ground) {
+                                for (Idx data_index = y_bus.row_indptr_lu()[bus_number];
+                                     data_index != y_bus.row_indptr_lu()[bus_number + 1]; ++data_index) {
+                                    Idx const col_data_index = y_bus.lu_transpose_entry()[data_index];
+                                    // mat_data[:,bus][:, phase_1] = 0
+                                    // mat_data[:,bus][:, phase_2] = 0
+                                    mat_data_[col_data_index].col(phase_1) = 0;
+                                    mat_data_[col_data_index].col(phase_2) = 0;
+                                }
+                                // mat_data[bus,bus][phase_1, phase_1] = -1
+                                // mat_data[bus,bus][phase_2, phase_2] = -1
+                                diagonal_element(phase_1, phase_1) = -1;
+                                diagonal_element(phase_2, phase_2) = -1;
+                                // update rhs
+                                u_bus(phase_1) = 0;
+                                u_bus(phase_2) = 0;
+                            }
+                            else {
+                                assert((fault_type == FaultType::three_phase));
+                                continue;
                             }
-                            // mat_data[bus,bus][phase_1, phase_1] = -1
-                            diagonal_element(phase_1, phase_1) = -1;
-                            u_bus(phase_1) = 0;  // update rhs
-                        }
-                        else if (fault_type == FaultType::two_phase) {
-                            for (Idx data_index = y_bus.row_indptr_lu()[bus_number];
-                                 data_index != y_bus.row_indptr_lu()[bus_number + 1]; ++data_index) {
-                                Idx const col_data_index = y_bus.lu_transpose_entry()[data_index];
-                                // mat_data[:,bus][:, phase_1] += mat_data[:,bus][:, phase_2]
-                                // mat_data[:,bus][:, phase_2] = 0
-                                mat_data_[col_data_index].col(phase_1) += mat_data_[col_data_index].col(phase_2);
-                                mat_data_[col_data_index].col(phase_2) = 0;
-                            }
-                            // mat_data[bus,bus][phase_1, phase_2] = -1
-                            // mat_data[bus,bus][phase_2, phase_2] = 1
-                            diagonal_element(phase_1, phase_2) = -1;
-                            diagonal_element(phase_2, phase_2) = 1;
-                            // update rhs
-                            u_bus(phase_2) += u_bus(phase_1);
-                            u_bus(phase_1) = 0;
-                        }
-                        else if (fault_type == FaultType::two_phase_to_ground) {
-                            for (Idx data_index = y_bus.row_indptr_lu()[bus_number];
-                                 data_index != y_bus.row_indptr_lu()[bus_number + 1]; ++data_index) {
-                                Idx const col_data_index = y_bus.lu_transpose_entry()[data_index];
-                                // mat_data[:,bus][:, phase_1] = 0
-                                // mat_data[:,bus][:, phase_2] = 0
-                                mat_data_[col_data_index].col(phase_1) = 0;
-                                mat_data_[col_data_index].col(phase_2) = 0;
-                            }
-                            // mat_data[bus,bus][phase_1, phase_1] = -1
-                            // mat_data[bus,bus][phase_2, phase_2] = -1
-                            diagonal_element(phase_1, phase_1) = -1;
-                            diagonal_element(phase_2, phase_2) = -1;
-                            // update rhs
-                            u_bus(phase_1) = 0;
-                            u_bus(phase_2) = 0;
-                        }
-                        else {
-                            assert((fault_type == FaultType::three_phase));
-                            continue;
-                        }
-                    }
-                    // If there is a fault with infinite admittance, there is no need to add other faults to that bus
-                    break;
-                }
-                else {
-                    assert(!std::isinf(y_fault.imag()));
-                    if (fault_type == FaultType::three_phase) {  // three phase fault
-                        // mat_data[bus,bus] += y_fault
-                        diagonal_element += ComplexTensor<sym>{y_fault};
-                    }
-                    if constexpr (!sym) {
-                        if (fault_type == FaultType::single_phase_to_ground) {
-                            // mat_data[bus,bus][phase_1, phase_1] += y_fault
-                            diagonal_element(phase_1, phase_1) += y_fault;
-                        }
-                        else if (fault_type == FaultType::two_phase) {
-                            // mat_data[bus,bus][phase_1, phase_1] += y_fault
-                            // mat_data[bus,bus][phase_2, phase_2] += y_fault
-                            // mat_data[bus,bus][phase_1, phase_2] -= y_fault
-                            // mat_data[bus,bus][phase_2, phase_1] -= y_fault
-                            diagonal_element(phase_1, phase_1) += y_fault;
-                            diagonal_element(phase_2, phase_2) += y_fault;
-                            diagonal_element(phase_1, phase_2) -= y_fault;
-                            diagonal_element(phase_2, phase_1) -= y_fault;
-                        }
-                        else if (fault_type == FaultType::two_phase_to_ground) {
-                            for (Idx data_index = y_bus.row_indptr_lu()[bus_number];
-                                 data_index != y_bus.row_indptr_lu()[bus_number + 1]; ++data_index) {
-                                Idx const col_data_index = y_bus.lu_transpose_entry()[data_index];
-                                // mat_data[:,bus][:, phase_1] += mat_data[:,bus][:, phase_2]
-                                // mat_data[:,bus][:, phase_2] = 0
-                                mat_data_[col_data_index].col(phase_1) += mat_data_[col_data_index].col(phase_2);
-                                mat_data_[col_data_index].col(phase_2) = 0;
-                            }
-                            // mat_data[bus,bus][phase_1, phase_2] = -1
-                            // mat_data[bus,bus][phase_2, phase_1] += y_fault
-                            // mat_data[bus,bus][phase_2, phase_2] = 1
-                            diagonal_element(phase_1, phase_2) = -1;
-                            diagonal_element(phase_2, phase_2) = 1;
-                            diagonal_element(phase_2, phase_1) += y_fault;
-                            // update rhs
-                            u_bus(phase_2) += u_bus(phase_1);
-                            u_bus(phase_1) = 0;
                         }
-                        else {
-                            assert((fault_type == FaultType::three_phase));
-                            continue;
+                        // If there is a fault with infinite admittance, there is no need to add other faults to that
+                        // bus
+                        break;
+                    }
+                    else {
+                        assert(!std::isinf(y_fault.imag()));
+                        if (fault_type == FaultType::three_phase) {  // three phase fault
+                            // mat_data[bus,bus] += y_fault
+                            diagonal_element += ComplexTensor<sym>{y_fault};
+                        }
+                        if constexpr (!sym) {
+                            if (fault_type == FaultType::single_phase_to_ground) {
+                                // mat_data[bus,bus][phase_1, phase_1] += y_fault
+                                diagonal_element(phase_1, phase_1) += y_fault;
+                            }
+                            else if (fault_type == FaultType::two_phase) {
+                                // mat_data[bus,bus][phase_1, phase_1] += y_fault
+                                // mat_data[bus,bus][phase_2, phase_2] += y_fault
+                                // mat_data[bus,bus][phase_1, phase_2] -= y_fault
+                                // mat_data[bus,bus][phase_2, phase_1] -= y_fault
+                                diagonal_element(phase_1, phase_1) += y_fault;
+                                diagonal_element(phase_2, phase_2) += y_fault;
+                                diagonal_element(phase_1, phase_2) -= y_fault;
+                                diagonal_element(phase_2, phase_1) -= y_fault;
+                            }
+                            else if (fault_type == FaultType::two_phase_to_ground) {
+                                for (Idx data_index = y_bus.row_indptr_lu()[bus_number];
+                                     data_index != y_bus.row_indptr_lu()[bus_number + 1]; ++data_index) {
+                                    Idx const col_data_index = y_bus.lu_transpose_entry()[data_index];
+                                    // mat_data[:,bus][:, phase_1] += mat_data[:,bus][:, phase_2]
+                                    // mat_data[:,bus][:, phase_2] = 0
+                                    mat_data_[col_data_index].col(phase_1) += mat_data_[col_data_index].col(phase_2);
+                                    mat_data_[col_data_index].col(phase_2) = 0;
+                                }
+                                // mat_data[bus,bus][phase_1, phase_2] = -1
+                                // mat_data[bus,bus][phase_2, phase_1] += y_fault
+                                // mat_data[bus,bus][phase_2, phase_2] = 1
+                                diagonal_element(phase_1, phase_2) = -1;
+                                diagonal_element(phase_2, phase_2) = 1;
+                                diagonal_element(phase_2, phase_1) += y_fault;
+                                // update rhs
+                                u_bus(phase_2) += u_bus(phase_1);
+                                u_bus(phase_1) = 0;
+                            }
+                            else {
+                                assert((fault_type == FaultType::three_phase));
+                                continue;
+                            }
                         }
                     }
                 }
             }
         }
 
         // solve matrix
@@ -228,116 +232,155 @@
                           int const phase_1, int const phase_2, double const source_voltage_ref) {
         // loop through all buses
         for (Idx bus_number = 0; bus_number != n_bus_; ++bus_number) {
             ComplexValue<sym> const x_bus_subtotal = output.u_bus[bus_number];
             double const infinite_admittance_fault_counter_bus =
                 static_cast<double>(infinite_admittance_fault_counter[bus_number]);
 
-            for (Idx fault_number = input.fault_bus_indptr[bus_number];
-                 fault_number != input.fault_bus_indptr[bus_number + 1]; ++fault_number) {
-                auto& i_fault = output.fault[fault_number].i_fault;
-                auto& u_bus = output.u_bus[bus_number];
-                DoubleComplex const y_fault = input.faults[fault_number].y_fault;
-
-                if (std::isinf(y_fault.real())) {
-                    assert(std::isinf(y_fault.imag()));
-                    if (fault_type == FaultType::three_phase) {  // three phase fault
-                        i_fault = -1.0 * static_cast<ComplexValue<sym>>(x_bus_subtotal) /
-                                  infinite_admittance_fault_counter_bus;  // injection is
-                                                                          // negative to fault
-                        u_bus = ComplexValue<sym>{0.0};
-                    }
-                    if constexpr (!sym) {
-                        if (fault_type == FaultType::single_phase_to_ground) {
-                            i_fault(phase_1) = -1.0 * x_bus_subtotal[phase_1] / infinite_admittance_fault_counter_bus;
-                            u_bus(phase_1) = 0.0;
-                        }
-                        else if (fault_type == FaultType::two_phase) {
-                            i_fault(phase_1) = -1.0 * x_bus_subtotal[phase_2] / infinite_admittance_fault_counter_bus;
-                            i_fault(phase_2) = -1.0 * i_fault(phase_1);
-                            u_bus(phase_2) = u_bus(phase_1);
-                        }
-                        else if (fault_type == FaultType::two_phase_to_ground) {
-                            i_fault(phase_1) = -1.0 * x_bus_subtotal[phase_1] / infinite_admittance_fault_counter_bus;
-                            i_fault(phase_2) = -1.0 * x_bus_subtotal[phase_2] / infinite_admittance_fault_counter_bus;
-                            u_bus(phase_1) = 0.0;
-                            u_bus(phase_2) = 0.0;
+            if (!input.faults.empty()) {
+                for (Idx fault_number = input.fault_bus_indptr[bus_number];
+                     fault_number != input.fault_bus_indptr[bus_number + 1]; ++fault_number) {
+                    auto& i_fault = output.fault[fault_number].i_fault;
+                    auto& u_bus = output.u_bus[bus_number];
+                    DoubleComplex const y_fault = input.faults[fault_number].y_fault;
+
+                    if (std::isinf(y_fault.real())) {
+                        assert(std::isinf(y_fault.imag()));
+                        if (fault_type == FaultType::three_phase) {  // three phase fault
+                            i_fault = -1.0 * static_cast<ComplexValue<sym>>(x_bus_subtotal) /
+                                      infinite_admittance_fault_counter_bus;  // injection is
+                                                                              // negative to fault
+                            u_bus = ComplexValue<sym>{0.0};
+                        }
+                        if constexpr (!sym) {
+                            if (fault_type == FaultType::single_phase_to_ground) {
+                                i_fault(phase_1) =
+                                    -1.0 * x_bus_subtotal[phase_1] / infinite_admittance_fault_counter_bus;
+                                u_bus(phase_1) = 0.0;
+                            }
+                            else if (fault_type == FaultType::two_phase) {
+                                i_fault(phase_1) =
+                                    -1.0 * x_bus_subtotal[phase_2] / infinite_admittance_fault_counter_bus;
+                                i_fault(phase_2) = -1.0 * i_fault(phase_1);
+                                u_bus(phase_2) = u_bus(phase_1);
+                            }
+                            else if (fault_type == FaultType::two_phase_to_ground) {
+                                i_fault(phase_1) =
+                                    -1.0 * x_bus_subtotal[phase_1] / infinite_admittance_fault_counter_bus;
+                                i_fault(phase_2) =
+                                    -1.0 * x_bus_subtotal[phase_2] / infinite_admittance_fault_counter_bus;
+                                u_bus(phase_1) = 0.0;
+                                u_bus(phase_2) = 0.0;
+                            }
+                            else {
+                                assert((fault_type == FaultType::three_phase));
+                                continue;
+                            }
                         }
-                        else {
-                            assert((fault_type == FaultType::three_phase));
+                    }
+                    else {
+                        assert(!std::isinf(y_fault.imag()));
+                        if (infinite_admittance_fault_counter[bus_number] > 0) {
+                            // ignore fault objects with impedance, when there is a fault with infinite admittance on
+                            // bus
                             continue;
                         }
-                    }
-                }
-                else {
-                    assert(!std::isinf(y_fault.imag()));
-                    if (infinite_admittance_fault_counter[bus_number] > 0) {
-                        // ignore fault objects with impedance, when there is a fault with infinite admittance on bus
-                        continue;
-                    }
-                    if (fault_type == FaultType::three_phase) {  // three phase fault
-                        i_fault = static_cast<ComplexValue<sym>>(y_fault * x_bus_subtotal);
-                    }
-                    if constexpr (!sym) {
-                        if (fault_type == FaultType::single_phase_to_ground) {
-                            i_fault(phase_1) = y_fault * x_bus_subtotal[phase_1];
-                        }
-                        else if (fault_type == FaultType::two_phase) {
-                            i_fault(phase_1) = y_fault * x_bus_subtotal[phase_1] - y_fault * x_bus_subtotal[phase_2];
-                            i_fault(phase_2) = y_fault * x_bus_subtotal[phase_2] - y_fault * x_bus_subtotal[phase_1];
-                        }
-                        else if (fault_type == FaultType::two_phase_to_ground) {
-                            i_fault(phase_1) = -1.0 * x_bus_subtotal[phase_2];
-                            i_fault(phase_2) = -1.0 * i_fault(phase_1) + y_fault * x_bus_subtotal[phase_1];
-                            u_bus(phase_2) = u_bus(phase_1);
+                        if (fault_type == FaultType::three_phase) {  // three phase fault
+                            i_fault = static_cast<ComplexValue<sym>>(y_fault * x_bus_subtotal);
                         }
-                        else {
-                            assert((fault_type == FaultType::three_phase));
-                            continue;
+                        if constexpr (!sym) {
+                            if (fault_type == FaultType::single_phase_to_ground) {
+                                i_fault(phase_1) = y_fault * x_bus_subtotal[phase_1];
+                            }
+                            else if (fault_type == FaultType::two_phase) {
+                                i_fault(phase_1) =
+                                    y_fault * x_bus_subtotal[phase_1] - y_fault * x_bus_subtotal[phase_2];
+                                i_fault(phase_2) =
+                                    y_fault * x_bus_subtotal[phase_2] - y_fault * x_bus_subtotal[phase_1];
+                            }
+                            else if (fault_type == FaultType::two_phase_to_ground) {
+                                i_fault(phase_1) = -1.0 * x_bus_subtotal[phase_2];
+                                i_fault(phase_2) = -1.0 * i_fault(phase_1) + y_fault * x_bus_subtotal[phase_1];
+                                u_bus(phase_2) = u_bus(phase_1);
+                            }
+                            else {
+                                assert((fault_type == FaultType::three_phase));
+                                continue;
+                            }
                         }
                     }
                 }
-            }
 
-            ComplexValue<sym> i_source_bus{};  // if asym, already initialized to zero
-            for (Idx source_number = (*source_bus_indptr_)[bus_number];
-                 source_number != (*source_bus_indptr_)[bus_number + 1]; ++source_number) {
-                ComplexTensor<sym> const y_source = y_bus.math_model_param().source_param[source_number];
-                output.source[source_number].i = dot(
-                    y_source,
-                    (ComplexValue<sym>{input.source[source_number] * source_voltage_ref} - output.u_bus[bus_number]));
-                i_source_bus += output.source[source_number].i;
-            }
-
-            // compensate source current into hard fault
-            for (Idx fault_number = input.fault_bus_indptr[bus_number];
-                 fault_number != input.fault_bus_indptr[bus_number + 1]; ++fault_number) {
-                auto& i_fault = output.fault[fault_number].i_fault;
-                DoubleComplex const y_fault = input.faults[fault_number].y_fault;
-
-                if (std::isinf(y_fault.real())) {
-                    assert(std::isinf(y_fault.imag()));
-                    if (fault_type == FaultType::three_phase) {
-                        i_fault += static_cast<ComplexValue<sym>>(i_source_bus / infinite_admittance_fault_counter_bus);
-                    }
-                    if constexpr (!sym) {
-                        if (fault_type == FaultType::single_phase_to_ground) {
-                            i_fault(phase_1) += i_source_bus[phase_1] / infinite_admittance_fault_counter_bus;
-                        }
-                        else if (fault_type == FaultType::two_phase) {
-                            i_fault(phase_1) -= i_source_bus[phase_1];
-                            i_fault(phase_2) -= i_source_bus[phase_2];
-                        }
-                        else if (fault_type == FaultType::two_phase_to_ground) {
-                            i_fault(phase_1) += i_source_bus[phase_1];
-                            i_fault(phase_2) += i_source_bus[phase_2];
+                ComplexValue<sym> i_source_bus{};     // total source current in to the bus
+                ComplexValue<sym> i_source_inject{};  // total raw source current as a Norton equievalent
+                for (Idx source_number = (*source_bus_indptr_)[bus_number];
+                     source_number != (*source_bus_indptr_)[bus_number + 1]; ++source_number) {
+                    ComplexTensor<sym> const y_source = y_bus.math_model_param().source_param[source_number];
+                    ComplexValue<sym> const i_source_inject_single =
+                        dot(y_source, ComplexValue<sym>{input.source[source_number] * source_voltage_ref});
+                    output.source[source_number].i = i_source_inject_single - dot(y_source, output.u_bus[bus_number]);
+                    i_source_bus += output.source[source_number].i;
+                    i_source_inject += i_source_inject_single;
+                }
+
+                // compensate source current into hard fault
+                // compensate source current into two phase to ground fault with impedance
+                for (Idx fault_number = input.fault_bus_indptr[bus_number];
+                     fault_number != input.fault_bus_indptr[bus_number + 1]; ++fault_number) {
+                    auto& i_fault = output.fault[fault_number].i_fault;
+                    DoubleComplex const y_fault = input.faults[fault_number].y_fault;
+
+                    if (std::isinf(y_fault.real())) {
+                        assert(std::isinf(y_fault.imag()));
+                        if (fault_type == FaultType::three_phase) {
+                            i_fault +=
+                                static_cast<ComplexValue<sym>>(i_source_bus / infinite_admittance_fault_counter_bus);
+                        }
+                        if constexpr (!sym) {
+                            if (fault_type == FaultType::single_phase_to_ground) {
+                                i_fault(phase_1) += i_source_bus[phase_1] / infinite_admittance_fault_counter_bus;
+                            }
+                            else if (fault_type == FaultType::two_phase) {
+                                i_fault(phase_1) += i_source_inject[phase_1] / infinite_admittance_fault_counter_bus;
+                                // i_inj_1 + i_inj_2 = i_ref_1 + i_ref_2
+                                // i_fault_2_p = i_inj_1
+                                //      i_fault_2_p is the i_fault_2 status quo after the first fault loop
+                                // i_inj_2 = - i_inj_1 + i_ref_1 + i_ref_2
+                                // i_fault_2 = i_ref_2 - i_inj_2 = i_ref_2 + i_inj_1 - i_ref_1 - i_ref_2
+                                //           = i_inj_1 - i_ref_1 = i_fault_2_p - i_ref_1
+                                i_fault(phase_2) -= i_source_inject[phase_1] / infinite_admittance_fault_counter_bus;
+                            }
+                            else if (fault_type == FaultType::two_phase_to_ground) {
+                                i_fault(phase_1) += i_source_bus[phase_1];
+                                i_fault(phase_2) += i_source_bus[phase_2];
+                            }
+                            else {
+                                assert((fault_type == FaultType::three_phase));
+                                continue;
+                            }
                         }
-                        else {
-                            assert((fault_type == FaultType::three_phase));
-                            continue;
+                    }
+                    else {
+                        // compensate for 2 phase to ground fault with impedance
+                        assert(!std::isinf(y_fault.imag()));
+                        if constexpr (!sym) {
+                            if ((fault_type == FaultType::two_phase_to_ground) &&
+                                (infinite_admittance_fault_counter_bus == 0.0)) {
+                                double const finite_admittance_fault_counter_bus = static_cast<double>(
+                                    input.fault_bus_indptr[bus_number + 1] - input.fault_bus_indptr[bus_number]);
+                                // i_inj_1 + i_inj_2 = i_ref_1 + i_ref_2 - u_12 * y_fault
+                                // i_fault_2_p = i_inj_1 + u_12 * y_fault
+                                //      i_fault_2_p is the i_fault_2 status quo after the first fault loop
+                                // i_inj_2 = - i_inj_1 + i_ref_1 + i_ref_2 - u_12 * y_fault
+                                // i_fault_2 = i_ref_2 - i_inj_2 = i_ref_2 + i_inj_1 - i_ref_1 - i_ref_2 + u_12 *
+                                // y_fault
+                                //           = i_inj_1 + u_12 * y_fault - i_ref_1 = i_fault_2_p - i_ref_1
+                                i_fault(phase_1) += i_source_inject[phase_1] / finite_admittance_fault_counter_bus;
+                                i_fault(phase_2) -= i_source_inject[phase_1] / finite_admittance_fault_counter_bus;
+                            }
                         }
                     }
                 }
             }
         }
 
         output.branch = y_bus.template calculate_branch_flow<BranchShortCircuitMathOutput<sym>>(output.u_bus);
@@ -393,27 +436,25 @@
         }
 
         const auto& first = faults.front();
         return std::pair{first.fault_type, first.fault_phase};
     }
 
     static void check_input_valid(ShortCircuitInput const& input) {
-        if (input.faults.empty()) {
-            throw NoShortCircuit{};
-        }
-
-        // For one calculation all faults should be of the same type and have the same phase
-        if (!all_fault_type_phase_equal(input.faults)) {
-            throw InvalidShortCircuitPhaseOrType{};
-        }
+        if (!input.faults.empty()) {
+            // For one calculation all faults should be of the same type and have the same phase
+            if (!all_fault_type_phase_equal(input.faults)) {
+                throw InvalidShortCircuitPhaseOrType{};
+            }
 
-        auto const& first = input.faults.front();
-        if (first.fault_type == FaultType::nan || first.fault_phase == FaultPhase::default_value ||
-            first.fault_phase == FaultPhase::nan) {
-            throw InvalidShortCircuitPhaseOrType{};
+            auto const& first = input.faults.front();
+            if (first.fault_type == FaultType::nan || first.fault_phase == FaultPhase::default_value ||
+                first.fault_phase == FaultPhase::nan) {
+                throw InvalidShortCircuitPhaseOrType{};
+            }
         }
     }
 
     static constexpr bool all_fault_type_phase_equal(std::vector<FaultCalcParam> const& vec) {
         if (vec.empty()) {
             return true;
         }
```

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/CMakeLists.txt` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/basics.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/buffer.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/dataset_definitions.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/handle.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/meta_data.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/model.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/power_grid_model_c/options.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/src/buffer.cpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/src/buffer.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/src/dataset_definitions.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/src/handle.cpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/src/handle.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/src/handle.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/src/handle.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/src/meta_data.cpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/src/meta_data.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/src/model.cpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/src/model.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/src/options.cpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/src/options.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/power_grid_model_c/power_grid_model_c/src/options.hpp` & `power-grid-model-1.5.0rc9228709919581/power_grid_model_c/power_grid_model_c/src/options.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/pyproject.toml` & `power-grid-model-1.5.0rc9228709919581/pyproject.toml`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/setup.py` & `power-grid-model-1.5.0rc9228709919581/setup.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model/__init__.py` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model/core/data_handling.py` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model/core/data_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model/core/error_handling.py` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model/core/error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model/core/options.py` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model/core/options.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model/core/power_grid_core.py` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model/core/power_grid_core.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model/core/power_grid_meta.py` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model/core/power_grid_meta.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model/core/power_grid_model.py` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model/core/power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model/data_types.py` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model/data_types.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model/enum.py` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model/enum.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model/utils.py` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model/validation/__init__.py` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model/validation/assertions.py` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model/validation/assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model/validation/errors.py` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model/validation/errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model/validation/rules.py` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model/validation/rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model/validation/utils.py` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model/validation/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model/validation/validation.py` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model/validation/validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model.egg-info/PKG-INFO` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9227505482890
+Version: 1.5.0rc9228709919581
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9227505482890/src/power_grid_model.egg-info/SOURCES.txt` & `power-grid-model-1.5.0rc9228709919581/src/power_grid_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/1os2msr/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-batch-newton/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-batch-newton/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-i-n-optional/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-i-n-optional/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/gaia-example/asym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/gaia-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/gaia-example/gaia_grid.gnf` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/gaia-example/gaia_grid.gnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/gaia-example/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/gaia-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/multi-source-with-angle/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/multi-source-with-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/line/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/line/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/node/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/node/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/node/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/source/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/source/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/source/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/line/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/line/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/node/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/source/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/r-state-estimation/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/r-state-estimation/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/r-state-estimation/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/r-state-estimation/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/three-winding-transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/three-winding-transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/three-winding-transformer/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/three-winding-transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/three-winding-transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/three-winding-transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/three-winding-transformer/update_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/three-winding-transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-example/asym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-example/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-example/vision_grid.vnf` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-example/vision_grid.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-validation-network/asym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-validation-network/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-validation-network/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-validation-network/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-validation-network/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-validation-network/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf` & `power-grid-model-1.5.0rc9228709919581/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/single_phase_to_ground/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/single_phase_to_ground/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/single_phase_to_ground/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/single_phase_to_ground/update_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/single_phase_to_ground/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/three_phase/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/three_phase/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/three_phase/sc_output_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/three_phase/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/three_phase/update_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/three_phase/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase/sc_output_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase/update_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase_to_ground/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase_to_ground/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase_to_ground/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/short_circuit/two_phase_to_ground/update_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/short_circuit/two_phase_to_ground/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr-no-angle/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr-no-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/1os2msr-no-angle/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/1os2msr-no-angle/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/distribution-case/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/distribution-case/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/dummy-test-sym/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/dummy-test-sym/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/dummy-test-sym/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/dummy-test-sym/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/single-line-load/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/single-line-load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/single-line-load/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/single-line-load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/three_winding_transformer/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/three_winding_transformer/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/transmission-case/README.md` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/transmission-case/input.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/data/state_estimation/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9228709919581/tests/data/state_estimation/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/unit/test_0Z_model_validation.py` & `power-grid-model-1.5.0rc9228709919581/tests/unit/test_0Z_model_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/unit/test_error_handling.py` & `power-grid-model-1.5.0rc9228709919581/tests/unit/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/unit/test_meta_data.py` & `power-grid-model-1.5.0rc9228709919581/tests/unit/test_meta_data.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/unit/test_power_grid_model.py` & `power-grid-model-1.5.0rc9228709919581/tests/unit/test_power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/unit/test_utils.py` & `power-grid-model-1.5.0rc9228709919581/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/unit/utils.py` & `power-grid-model-1.5.0rc9228709919581/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/unit/validation/test_assertions.py` & `power-grid-model-1.5.0rc9228709919581/tests/unit/validation/test_assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/unit/validation/test_batch_validation.py` & `power-grid-model-1.5.0rc9228709919581/tests/unit/validation/test_batch_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/unit/validation/test_errors.py` & `power-grid-model-1.5.0rc9228709919581/tests/unit/validation/test_errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/unit/validation/test_input_validation.py` & `power-grid-model-1.5.0rc9228709919581/tests/unit/validation/test_input_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/unit/validation/test_rules.py` & `power-grid-model-1.5.0rc9228709919581/tests/unit/validation/test_rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/unit/validation/test_utils.py` & `power-grid-model-1.5.0rc9228709919581/tests/unit/validation/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9227505482890/tests/unit/validation/test_validation_functions.py` & `power-grid-model-1.5.0rc9228709919581/tests/unit/validation/test_validation_functions.py`

 * *Files identical despite different names*


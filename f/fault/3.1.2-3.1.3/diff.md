# Comparing `tmp/fault-3.1.2.tar.gz` & `tmp/fault-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fault-3.1.2.tar", last modified: Tue May 31 00:11:10 2022, max compression
+gzip compressed data, was "fault-3.1.3.tar", last modified: Wed Jul 26 21:28:12 2023, max compression
```

## Comparing `fault-3.1.2.tar` & `fault-3.1.3.tar`

### file list

```diff
@@ -1,75 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 00:11:10.786690 fault-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1459 2022-05-31 00:02:56.000000 fault-3.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17092 2022-05-31 00:11:10.786690 fault-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13882 2022-05-31 00:02:56.000000 fault-3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 00:11:10.786690 fault-3.1.2/fault/
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-05-31 00:02:56.000000 fault-3.1.2/fault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-05-31 00:02:56.000000 fault-3.1.2/fault/action_generators.py
--rw-r--r--   0 runner    (1001) docker     (121)    12901 2022-05-31 00:02:56.000000 fault-3.1.2/fault/actions.py
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-05-31 00:02:56.000000 fault-3.1.2/fault/array.py
--rw-r--r--   0 runner    (1001) docker     (121)     3626 2022-05-31 00:02:56.000000 fault-3.1.2/fault/assert_immediate.py
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-05-31 00:02:56.000000 fault-3.1.2/fault/assert_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-05-31 00:02:56.000000 fault-3.1.2/fault/circuit_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-05-31 00:02:56.000000 fault-3.1.2/fault/codegen.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-05-31 00:02:56.000000 fault-3.1.2/fault/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-05-31 00:02:56.000000 fault-3.1.2/fault/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4354 2022-05-31 00:02:56.000000 fault-3.1.2/fault/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-05-31 00:02:56.000000 fault-3.1.2/fault/fault_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-05-31 00:02:56.000000 fault-3.1.2/fault/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-05-31 00:02:56.000000 fault-3.1.2/fault/functional_tester.py
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-05-31 00:02:56.000000 fault-3.1.2/fault/infix.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-05-31 00:02:56.000000 fault-3.1.2/fault/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     4962 2022-05-31 00:02:56.000000 fault-3.1.2/fault/magma_simulator_target.py
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-05-31 00:02:56.000000 fault-3.1.2/fault/magma_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-05-31 00:02:56.000000 fault-3.1.2/fault/ms_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-05-31 00:02:56.000000 fault-3.1.2/fault/netlister.py
--rw-r--r--   0 runner    (1001) docker     (121)     8415 2022-05-31 00:02:56.000000 fault-3.1.2/fault/pono_target.py
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-05-31 00:02:56.000000 fault-3.1.2/fault/power_tester.py
--rw-r--r--   0 runner    (1001) docker     (121)     9617 2022-05-31 00:02:56.000000 fault-3.1.2/fault/property.py
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-05-31 00:02:56.000000 fault-3.1.2/fault/pwl.py
--rw-r--r--   0 runner    (1001) docker     (121)     5482 2022-05-31 00:02:56.000000 fault-3.1.2/fault/pysv.py
--rw-r--r--   0 runner    (1001) docker     (121)     9133 2022-05-31 00:02:56.000000 fault-3.1.2/fault/random.py
--rw-r--r--   0 runner    (1001) docker     (121)     4589 2022-05-31 00:02:56.000000 fault-3.1.2/fault/ready_valid.py
--rw-r--r--   0 runner    (1001) docker     (121)     3358 2022-05-31 00:02:56.000000 fault-3.1.2/fault/result_parse.py
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-05-31 00:02:56.000000 fault-3.1.2/fault/select_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     4642 2022-05-31 00:02:56.000000 fault-3.1.2/fault/spice.py
--rw-r--r--   0 runner    (1001) docker     (121)    22933 2022-05-31 00:02:56.000000 fault-3.1.2/fault/spice_target.py
--rw-r--r--   0 runner    (1001) docker     (121)     7204 2022-05-31 00:02:56.000000 fault-3.1.2/fault/subprocess_run.py
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-05-31 00:02:56.000000 fault-3.1.2/fault/sva.py
--rw-r--r--   0 runner    (1001) docker     (121)    47290 2022-05-31 00:02:56.000000 fault-3.1.2/fault/system_verilog_target.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-05-31 00:02:56.000000 fault-3.1.2/fault/target.py
--rw-r--r--   0 runner    (1001) docker     (121)     2401 2022-05-31 00:02:56.000000 fault-3.1.2/fault/test_vector_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5865 2022-05-31 00:02:56.000000 fault-3.1.2/fault/test_vectors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 00:11:10.786690 fault-3.1.2/fault/tester/
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-05-31 00:02:56.000000 fault-3.1.2/fault/tester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11244 2022-05-31 00:02:56.000000 fault-3.1.2/fault/tester/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2048 2022-05-31 00:02:56.000000 fault-3.1.2/fault/tester/control.py
--rw-r--r--   0 runner    (1001) docker     (121)     4322 2022-05-31 00:02:56.000000 fault-3.1.2/fault/tester/interactive_tester.py
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-05-31 00:02:56.000000 fault-3.1.2/fault/tester/sequence_tester.py
--rw-r--r--   0 runner    (1001) docker     (121)    19374 2022-05-31 00:02:56.000000 fault-3.1.2/fault/tester/staged_tester.py
--rw-r--r--   0 runner    (1001) docker     (121)     4035 2022-05-31 00:02:56.000000 fault-3.1.2/fault/tester/symbolic_tester.py
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-05-31 00:02:56.000000 fault-3.1.2/fault/tester/synchronous.py
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-05-31 00:02:56.000000 fault-3.1.2/fault/tester/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3688 2022-05-31 00:02:56.000000 fault-3.1.2/fault/tester_samples.py
--rw-r--r--   0 runner    (1001) docker     (121)     2301 2022-05-31 00:02:56.000000 fault-3.1.2/fault/user_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-05-31 00:02:56.000000 fault-3.1.2/fault/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-05-31 00:02:56.000000 fault-3.1.2/fault/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-05-31 00:02:56.000000 fault-3.1.2/fault/value.py
--rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-05-31 00:02:56.000000 fault-3.1.2/fault/value_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2240 2022-05-31 00:02:56.000000 fault-3.1.2/fault/vector_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)    33459 2022-05-31 00:02:56.000000 fault-3.1.2/fault/verilator_target.py
--rw-r--r--   0 runner    (1001) docker     (121)     2544 2022-05-31 00:02:56.000000 fault-3.1.2/fault/verilator_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12377 2022-05-31 00:02:56.000000 fault-3.1.2/fault/verilog_target.py
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-05-31 00:02:56.000000 fault-3.1.2/fault/verilog_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-05-31 00:02:56.000000 fault-3.1.2/fault/verilogams.py
--rw-r--r--   0 runner    (1001) docker     (121)     5661 2022-05-31 00:02:56.000000 fault-3.1.2/fault/verilogams_target.py
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-05-31 00:02:56.000000 fault-3.1.2/fault/wrapped_internal_port.py
--rw-r--r--   0 runner    (1001) docker     (121)     5896 2022-05-31 00:02:56.000000 fault-3.1.2/fault/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 00:11:10.786690 fault-3.1.2/fault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17092 2022-05-31 00:11:10.000000 fault-3.1.2/fault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-05-31 00:11:10.000000 fault-3.1.2/fault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-31 00:11:10.000000 fault-3.1.2/fault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-05-31 00:11:10.000000 fault-3.1.2/fault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-05-31 00:11:10.000000 fault-3.1.2/fault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-05-31 00:11:10.786690 fault-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-05-31 00:02:56.000000 fault-3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:28:12.030488 fault-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-26 21:15:53.000000 fault-3.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21181 2023-07-26 21:28:12.030488 fault-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17283 2023-07-26 21:15:53.000000 fault-3.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:28:12.022488 fault-3.1.3/fault/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-26 21:15:53.000000 fault-3.1.3/fault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-26 21:15:53.000000 fault-3.1.3/fault/action_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12901 2023-07-26 21:15:53.000000 fault-3.1.3/fault/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-26 21:15:53.000000 fault-3.1.3/fault/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-26 21:15:53.000000 fault-3.1.3/fault/assert_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-26 21:15:53.000000 fault-3.1.3/fault/assert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-26 21:15:53.000000 fault-3.1.3/fault/circuit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-26 21:15:53.000000 fault-3.1.3/fault/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-26 21:15:53.000000 fault-3.1.3/fault/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-26 21:15:53.000000 fault-3.1.3/fault/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-26 21:15:53.000000 fault-3.1.3/fault/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-26 21:15:53.000000 fault-3.1.3/fault/fault_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-26 21:15:53.000000 fault-3.1.3/fault/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-26 21:15:53.000000 fault-3.1.3/fault/functional_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-26 21:15:53.000000 fault-3.1.3/fault/infix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-26 21:15:53.000000 fault-3.1.3/fault/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-26 21:15:53.000000 fault-3.1.3/fault/magma_simulator_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-26 21:15:53.000000 fault-3.1.3/fault/magma_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-26 21:15:53.000000 fault-3.1.3/fault/ms_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-26 21:15:53.000000 fault-3.1.3/fault/netlister.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-07-26 21:15:53.000000 fault-3.1.3/fault/pono_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-26 21:15:53.000000 fault-3.1.3/fault/power_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-07-26 21:15:53.000000 fault-3.1.3/fault/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-26 21:15:53.000000 fault-3.1.3/fault/pwl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-07-26 21:15:53.000000 fault-3.1.3/fault/pysv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-26 21:15:53.000000 fault-3.1.3/fault/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-26 21:15:53.000000 fault-3.1.3/fault/ready_valid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-26 21:15:53.000000 fault-3.1.3/fault/result_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-26 21:15:53.000000 fault-3.1.3/fault/select_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-26 21:15:53.000000 fault-3.1.3/fault/spice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22933 2023-07-26 21:15:53.000000 fault-3.1.3/fault/spice_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-07-26 21:15:53.000000 fault-3.1.3/fault/subprocess_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-26 21:15:53.000000 fault-3.1.3/fault/sva.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47290 2023-07-26 21:15:53.000000 fault-3.1.3/fault/system_verilog_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-26 21:15:53.000000 fault-3.1.3/fault/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-26 21:15:53.000000 fault-3.1.3/fault/test_vector_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-07-26 21:15:53.000000 fault-3.1.3/fault/test_vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:28:12.022488 fault-3.1.3/fault/tester/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-26 21:15:53.000000 fault-3.1.3/fault/tester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-26 21:15:53.000000 fault-3.1.3/fault/tester/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-26 21:15:53.000000 fault-3.1.3/fault/tester/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-07-26 21:15:53.000000 fault-3.1.3/fault/tester/interactive_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-26 21:15:53.000000 fault-3.1.3/fault/tester/sequence_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-07-26 21:15:53.000000 fault-3.1.3/fault/tester/staged_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-26 21:15:53.000000 fault-3.1.3/fault/tester/symbolic_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-26 21:15:53.000000 fault-3.1.3/fault/tester/synchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-26 21:15:53.000000 fault-3.1.3/fault/tester/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-07-26 21:15:53.000000 fault-3.1.3/fault/tester_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-26 21:15:53.000000 fault-3.1.3/fault/user_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-26 21:15:53.000000 fault-3.1.3/fault/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-26 21:15:53.000000 fault-3.1.3/fault/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-26 21:15:53.000000 fault-3.1.3/fault/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-26 21:15:53.000000 fault-3.1.3/fault/value_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-26 21:15:53.000000 fault-3.1.3/fault/vector_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33672 2023-07-26 21:15:53.000000 fault-3.1.3/fault/verilator_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-26 21:15:53.000000 fault-3.1.3/fault/verilator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-07-26 21:15:53.000000 fault-3.1.3/fault/verilog_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-26 21:15:53.000000 fault-3.1.3/fault/verilog_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-26 21:15:53.000000 fault-3.1.3/fault/verilogams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-26 21:15:53.000000 fault-3.1.3/fault/verilogams_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-26 21:15:53.000000 fault-3.1.3/fault/wrapped_internal_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-07-26 21:15:53.000000 fault-3.1.3/fault/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:28:12.022488 fault-3.1.3/fault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21181 2023-07-26 21:28:11.000000 fault-3.1.3/fault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-26 21:28:11.000000 fault-3.1.3/fault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:28:11.000000 fault-3.1.3/fault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 21:28:11.000000 fault-3.1.3/fault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 21:28:11.000000 fault-3.1.3/fault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-26 21:28:12.030488 fault-3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-26 21:15:53.000000 fault-3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:28:12.030488 fault-3.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_assert_immediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_bidir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_constrained_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_def_vlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_env_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_ext_tb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_ext_vlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_fork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_functional_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_get_value_analog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_get_value_digital.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_hi_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_inc_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_include_verilog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_init_cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_inv_tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_kratos_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_magma_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_magma_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_magma_simulator_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_param_vlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_power_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31111 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_pwl_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_pysv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_ready_valid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_real_val.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_select_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_setattr_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_spice_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_spice_port_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_system_verilog_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_test_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_top_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_value_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_vams_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_vector_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_verilator_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_verilog_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-26 21:15:53.000000 fault-3.1.3/tests/test_while_loop.py
```

### Comparing `fault-3.1.2/LICENSE.txt` & `fault-3.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/PKG-INFO` & `fault-3.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fault
-Version: 3.1.2
+Version: 3.1.3
 Summary: A Python package for testing hardware (part of the magma ecosystem)
 Home-page: https://github.com/leonardt/fault
 Author: Leonard Truong
 Author-email: lenny@cs.stanford.edu
 License: BSD License
 Description: # Fault
         ![Linux Test](https://github.com/leonardt/fault/workflows/Linux%20Test/badge.svg)
@@ -361,10 +361,96 @@
         
         or for system verilog
         ```python
         tester.compile("system-verilog", simulator="ncsim")
         tb_file = tester.generate_test_bench("system-verilog")
         ```
         
+        ### Using the ReadyValid Tester
+        Fault provides a `ReadyValidTester` that provides a few convenient features for
+        unit testing `ReadyValid` interfaces with sequences.
+        
+        Consider the following circuit:
+        ```python
+        class Main2(m.Circuit):
+            io = m.IO(I=m.Consumer(m.ReadyValid[m.UInt[8]]),
+                      O=m.Producer(m.ReadyValid[m.UInt[8]]),
+                      inc=m.In(m.UInt[8]),
+                      ) + m.ClockIO()
+            count = m.Register(m.UInt[2])()
+            count.I @= count.O + 1
+            enable = io.I.valid & (count.O == 3) & io.O.ready
+            io.I.ready @= enable
+            io.O.data @= m.Register(m.UInt[8], has_enable=True)()(io.I.data + io.inc,
+                                                                  CE=enable)
+            io.O.valid @= enable
+        ```
+        
+        The output stream `O` is the input stream `I` incremented by the value of `inc`
+        and delayed by 4 cycles.
+        
+        Here's a simple test that provides the input sequence `I` and expected output
+        sequence `O`
+        ```python
+        def test_lifted_ready_valid_sequence_simple():
+            I = [BitVector.random(8) for _ in range(8)] + [0]
+            O = [0] + [i + 2 for i in I[:-1]]
+            tester = f.ReadyValidTester(Main2, {"I": I, "O": O})
+            tester.circuit.inc = 2
+            tester.finish_sequences()
+            tester.compile_and_run("verilator", disp_type="realtime")
+        
+        ```
+        
+        Notice that we provide the sequences as a dictionary mapping port name to
+        sequence in the constructor.  Afterwards, we are free to `poke` values like in a normal tester, in this case provide `2` for `inc` which will satisfy the provided stream.
+        
+        **NOTE:** The user must explicitly use the `tester.circuit` peek/poke
+        interface, or call `tester.poke(tester._circuit, value)` since the user circuit
+        is wrapped internally (cannot call `tester.poke(Main2, value)`).
+        
+        The test finishes by calling `tester.finish_sequences()` which is a convenience
+        API that waits for the provided sequences to finish.
+        
+        Here's a different version of the above test that should fail (changing the `inc` value mid test).
+        ```python
+        
+        
+        def test_lifted_ready_valid_sequence_simple_fail():
+            I = [BitVector.random(8) for _ in range(8)] + [0]
+            O = [0] + [i + 2 for i in I[:-1]]
+            tester = f.ReadyValidTester(Main2, {"I": I, "O": O})
+            tester.circuit.inc = 2
+            # Should work for a few cycles
+            for i in range(9):
+                tester.advance_cycle()
+            # Bad inc should fail
+            tester.circuit.inc = 3
+            tester.finish_sequences()
+            with pytest.raises(AssertionError):
+                tester.compile_and_run("verilator", disp_type="realtime")
+        ```
+        
+        Finally, here's a variant that changes the `inc` value over time to match the expected sequence.
+        ```python
+        def test_lifted_ready_valid_sequence_changing_inc():
+            I = [BitVector.random(8) for _ in range(8)] + [0]
+            O = [0] + [I[i] + ((i + 1) % 2) for i in range(8)]
+            tester = f.ReadyValidTester(Main2, {"I": I, "O": O})
+            # Sequence expects inc to change over time
+            for i in range(8):
+                tester.circuit.inc = i % 2
+                tester.advance_cycle()
+                tester.wait_until_high(tester.circuit.O.ready & tester.circuit.O.valid)
+            # Advance one cycle to finish last handshake
+            tester.advance_cycle()
+            tester.expect_sequences_finished()
+            tester.compile_and_run("verilator", disp_type="realtime")
+        ```
+        
+        **NOTE:** At the end of the test, we call `expect_sequences_finished()` to
+        assert that the sequences have all been processed, otherwise it's possible tha
+        the test could pass without completing the sequences.
+        
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `fault-3.1.2/README.md` & `fault-3.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -352,7 +352,93 @@
 ```
 
 or for system verilog
 ```python
 tester.compile("system-verilog", simulator="ncsim")
 tb_file = tester.generate_test_bench("system-verilog")
 ```
+
+### Using the ReadyValid Tester
+Fault provides a `ReadyValidTester` that provides a few convenient features for
+unit testing `ReadyValid` interfaces with sequences.
+
+Consider the following circuit:
+```python
+class Main2(m.Circuit):
+    io = m.IO(I=m.Consumer(m.ReadyValid[m.UInt[8]]),
+              O=m.Producer(m.ReadyValid[m.UInt[8]]),
+              inc=m.In(m.UInt[8]),
+              ) + m.ClockIO()
+    count = m.Register(m.UInt[2])()
+    count.I @= count.O + 1
+    enable = io.I.valid & (count.O == 3) & io.O.ready
+    io.I.ready @= enable
+    io.O.data @= m.Register(m.UInt[8], has_enable=True)()(io.I.data + io.inc,
+                                                          CE=enable)
+    io.O.valid @= enable
+```
+
+The output stream `O` is the input stream `I` incremented by the value of `inc`
+and delayed by 4 cycles.
+
+Here's a simple test that provides the input sequence `I` and expected output
+sequence `O`
+```python
+def test_lifted_ready_valid_sequence_simple():
+    I = [BitVector.random(8) for _ in range(8)] + [0]
+    O = [0] + [i + 2 for i in I[:-1]]
+    tester = f.ReadyValidTester(Main2, {"I": I, "O": O})
+    tester.circuit.inc = 2
+    tester.finish_sequences()
+    tester.compile_and_run("verilator", disp_type="realtime")
+
+```
+
+Notice that we provide the sequences as a dictionary mapping port name to
+sequence in the constructor.  Afterwards, we are free to `poke` values like in a normal tester, in this case provide `2` for `inc` which will satisfy the provided stream.
+
+**NOTE:** The user must explicitly use the `tester.circuit` peek/poke
+interface, or call `tester.poke(tester._circuit, value)` since the user circuit
+is wrapped internally (cannot call `tester.poke(Main2, value)`).
+
+The test finishes by calling `tester.finish_sequences()` which is a convenience
+API that waits for the provided sequences to finish.
+
+Here's a different version of the above test that should fail (changing the `inc` value mid test).
+```python
+
+
+def test_lifted_ready_valid_sequence_simple_fail():
+    I = [BitVector.random(8) for _ in range(8)] + [0]
+    O = [0] + [i + 2 for i in I[:-1]]
+    tester = f.ReadyValidTester(Main2, {"I": I, "O": O})
+    tester.circuit.inc = 2
+    # Should work for a few cycles
+    for i in range(9):
+        tester.advance_cycle()
+    # Bad inc should fail
+    tester.circuit.inc = 3
+    tester.finish_sequences()
+    with pytest.raises(AssertionError):
+        tester.compile_and_run("verilator", disp_type="realtime")
+```
+
+Finally, here's a variant that changes the `inc` value over time to match the expected sequence.
+```python
+def test_lifted_ready_valid_sequence_changing_inc():
+    I = [BitVector.random(8) for _ in range(8)] + [0]
+    O = [0] + [I[i] + ((i + 1) % 2) for i in range(8)]
+    tester = f.ReadyValidTester(Main2, {"I": I, "O": O})
+    # Sequence expects inc to change over time
+    for i in range(8):
+        tester.circuit.inc = i % 2
+        tester.advance_cycle()
+        tester.wait_until_high(tester.circuit.O.ready & tester.circuit.O.valid)
+    # Advance one cycle to finish last handshake
+    tester.advance_cycle()
+    tester.expect_sequences_finished()
+    tester.compile_and_run("verilator", disp_type="realtime")
+```
+
+**NOTE:** At the end of the test, we call `expect_sequences_finished()` to
+assert that the sequences have all been processed, otherwise it's possible tha
+the test could pass without completing the sequences.
```

### Comparing `fault-3.1.2/fault/__init__.py` & `fault-3.1.3/fault/__init__.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/action_generators.py` & `fault-3.1.3/fault/action_generators.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/actions.py` & `fault-3.1.3/fault/actions.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/array.py` & `fault-3.1.3/fault/array.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/assert_immediate.py` & `fault-3.1.3/fault/assert_immediate.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/assert_utils.py` & `fault-3.1.3/fault/assert_utils.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/circuit_utils.py` & `fault-3.1.3/fault/circuit_utils.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/codegen.py` & `fault-3.1.3/fault/codegen.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/expression.py` & `fault-3.1.3/fault/expression.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/file.py` & `fault-3.1.3/fault/file.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/functional_tester.py` & `fault-3.1.3/fault/functional_tester.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/magma_simulator_target.py` & `fault-3.1.3/fault/magma_simulator_target.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/netlister.py` & `fault-3.1.3/fault/netlister.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/pono_target.py` & `fault-3.1.3/fault/pono_target.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/power_tester.py` & `fault-3.1.3/fault/power_tester.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/property.py` & `fault-3.1.3/fault/property.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/pwl.py` & `fault-3.1.3/fault/pwl.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/pysv.py` & `fault-3.1.3/fault/pysv.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/random.py` & `fault-3.1.3/fault/random.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/ready_valid.py` & `fault-3.1.3/fault/ready_valid.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/result_parse.py` & `fault-3.1.3/fault/result_parse.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/select_path.py` & `fault-3.1.3/fault/select_path.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/spice.py` & `fault-3.1.3/fault/spice.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/spice_target.py` & `fault-3.1.3/fault/spice_target.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/subprocess_run.py` & `fault-3.1.3/fault/subprocess_run.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/system_verilog_target.py` & `fault-3.1.3/fault/system_verilog_target.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/test_vector_generator.py` & `fault-3.1.3/fault/test_vector_generator.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/test_vectors.py` & `fault-3.1.3/fault/test_vectors.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/tester/base.py` & `fault-3.1.3/fault/tester/base.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/tester/control.py` & `fault-3.1.3/fault/tester/control.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/tester/interactive_tester.py` & `fault-3.1.3/fault/tester/interactive_tester.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/tester/sequence_tester.py` & `fault-3.1.3/fault/tester/sequence_tester.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/tester/staged_tester.py` & `fault-3.1.3/fault/tester/staged_tester.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/tester/symbolic_tester.py` & `fault-3.1.3/fault/tester/symbolic_tester.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/tester/synchronous.py` & `fault-3.1.3/fault/tester/synchronous.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/tester_samples.py` & `fault-3.1.3/fault/tester_samples.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/user_cfg.py` & `fault-3.1.3/fault/user_cfg.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/util.py` & `fault-3.1.3/fault/util.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/utils.py` & `fault-3.1.3/fault/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,33 +35,15 @@
     # from the original source, so we have to determine the end ourselves.
     # We do that by gradually shaving extra junk from after the definition.
     lambda_text = source_text[lambda_node.col_offset:]
     lambda_body_text = source_text[lambda_node.body.col_offset:]
     min_length = len('lambda:_')  # shortest possible lambda expression
     while len(lambda_text) > min_length:
         try:
-            # What's annoying is that sometimes the junk even parses,
-            # but results in a *different* lambda. You'd probably have to
-            # be deliberately malicious to exploit it but here's one way:
-            #
-            #     bloop = lambda x: False, lambda x: True
-            #     get_short_lamnda_source(bloop[0])
-            #
-            # Ideally, we'd just keep shaving until we get the same code,
-            # but that most likely won't happen because we can't replicate
-            # the exact closure environment.
-            code = compile(lambda_body_text, '<unused filename>', 'eval')
-
-            # Thus the next best thing is to assume some divergence due
-            # to e.g. LOAD_GLOBAL in original code being LOAD_FAST in
-            # the one compiled above, or vice versa.
-            # But the resulting code should at least be the same *length*
-            # if otherwise the same operations are performed in it.
-            if len(code.co_code) == len(lambda_func.__code__.co_code):
-                # return lambda_text
-                return lambda_body_text
+            compile(lambda_body_text, '<unused filename>', 'eval')
+            return lambda_body_text
         except SyntaxError:
             pass
         lambda_text = lambda_text[:-1]
         lambda_body_text = lambda_body_text[:-1]
 
     return None
```

### Comparing `fault-3.1.2/fault/value_utils.py` & `fault-3.1.3/fault/value_utils.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/vector_builder.py` & `fault-3.1.3/fault/vector_builder.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/verilator_target.py` & `fault-3.1.3/fault/verilator_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,23 @@
 import glob
 import pysv
 
 
 max_bits = 64 if platform.architecture()[0] == "64bit" else 32
 
 
+SYSTEM = platform.system()
+if SYSTEM == "Linux":
+    _LIBRARY_PATH_NAME = "LD_LIBRARY_PATH"
+elif SYSTEM == "Darwin":
+    _LIBRARY_PATH_NAME = "DYLD_LIBRARY_PATH"
+else:
+    raise NotImplementedError(SYSTEM)
+
+
 src_tpl = """\
 #include "math.h"
 {includes}
 
 // Based on https://www.veripool.org/projects/verilator/wiki/Manual-verilator#CONNECTING-TO-C
 vluint64_t main_time = 0;       // Current simulation time
 // This is a 64-bit integer to reduce wrap over issues and
@@ -745,38 +754,36 @@
 
     def run(self, actions, verilator_includes=None, num_tests=0,
             _circuit=None):
 
         self.generate_test_bench(actions, verilator_includes, num_tests,
                                  _circuit)
 
+        lib_path = os.path.abspath(os.path.join(self.directory, "obj_dir"))
+        env = {_LIBRARY_PATH_NAME: os.path.dirname(lib_path)}
         # if use kratos, symbolic link the library to dest folder
         if self.use_kratos:
             from kratos_runtime import get_lib_path
             lib_name = os.path.basename(get_lib_path())
             dst_path = os.path.abspath(os.path.join(self.directory, "obj_dir",
                                                     lib_name))
             if not os.path.isfile(dst_path):
                 os.symlink(get_lib_path(), dst_path)
-            # add ld library path
-            env = {"LD_LIBRARY_PATH": os.path.dirname(dst_path)}
-        else:
-            env = None
 
         # codegen the c++ binding if needed
         if len(self.pysv_funcs) > 0:
             header = os.path.join(self.directory, "pysv.hh")
             pysv.generate_cxx_binding(self.pysv_funcs, filename=header)
             lib_path = pysv.compile_lib(self.pysv_funcs, os.path.join(self.directory, "obj_dir"))
             ld_lib_path = os.path.realpath(os.path.dirname(lib_path))
             if env is None:
                 env = {}
-            if "LD_LIBRARY_PATH" in env:
-                ld_lib_path = env["LD_LIBRARY_PATH"] + ":" + ld_lib_path
-            env["LD_LIBRARY_PATH"] = ld_lib_path
+            if _LIBRARY_PATH_NAME in env:
+                ld_lib_path = env[_LIBRARY_PATH_NAME] + ":" + ld_lib_path
+            env[_LIBRARY_PATH_NAME] = ld_lib_path
 
         # Run makefile created by verilator
         make_cmd = verilator_make_cmd(self.circuit_name)
         subprocess_run(make_cmd, cwd=self.directory, disp_type=self.disp_type)
 
         # create the logs folder if necessary
         logs = Path(self.directory) / "logs"
```

### Comparing `fault-3.1.2/fault/verilator_utils.py` & `fault-3.1.3/fault/verilator_utils.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/verilog_target.py` & `fault-3.1.3/fault/verilog_target.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/verilog_utils.py` & `fault-3.1.3/fault/verilog_utils.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/verilogams.py` & `fault-3.1.3/fault/verilogams.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/verilogams_target.py` & `fault-3.1.3/fault/verilogams_target.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault/wrapper.py` & `fault-3.1.3/fault/wrapper.py`

 * *Files identical despite different names*

### Comparing `fault-3.1.2/fault.egg-info/PKG-INFO` & `fault-3.1.3/fault.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fault
-Version: 3.1.2
+Version: 3.1.3
 Summary: A Python package for testing hardware (part of the magma ecosystem)
 Home-page: https://github.com/leonardt/fault
 Author: Leonard Truong
 Author-email: lenny@cs.stanford.edu
 License: BSD License
 Description: # Fault
         ![Linux Test](https://github.com/leonardt/fault/workflows/Linux%20Test/badge.svg)
@@ -361,10 +361,96 @@
         
         or for system verilog
         ```python
         tester.compile("system-verilog", simulator="ncsim")
         tb_file = tester.generate_test_bench("system-verilog")
         ```
         
+        ### Using the ReadyValid Tester
+        Fault provides a `ReadyValidTester` that provides a few convenient features for
+        unit testing `ReadyValid` interfaces with sequences.
+        
+        Consider the following circuit:
+        ```python
+        class Main2(m.Circuit):
+            io = m.IO(I=m.Consumer(m.ReadyValid[m.UInt[8]]),
+                      O=m.Producer(m.ReadyValid[m.UInt[8]]),
+                      inc=m.In(m.UInt[8]),
+                      ) + m.ClockIO()
+            count = m.Register(m.UInt[2])()
+            count.I @= count.O + 1
+            enable = io.I.valid & (count.O == 3) & io.O.ready
+            io.I.ready @= enable
+            io.O.data @= m.Register(m.UInt[8], has_enable=True)()(io.I.data + io.inc,
+                                                                  CE=enable)
+            io.O.valid @= enable
+        ```
+        
+        The output stream `O` is the input stream `I` incremented by the value of `inc`
+        and delayed by 4 cycles.
+        
+        Here's a simple test that provides the input sequence `I` and expected output
+        sequence `O`
+        ```python
+        def test_lifted_ready_valid_sequence_simple():
+            I = [BitVector.random(8) for _ in range(8)] + [0]
+            O = [0] + [i + 2 for i in I[:-1]]
+            tester = f.ReadyValidTester(Main2, {"I": I, "O": O})
+            tester.circuit.inc = 2
+            tester.finish_sequences()
+            tester.compile_and_run("verilator", disp_type="realtime")
+        
+        ```
+        
+        Notice that we provide the sequences as a dictionary mapping port name to
+        sequence in the constructor.  Afterwards, we are free to `poke` values like in a normal tester, in this case provide `2` for `inc` which will satisfy the provided stream.
+        
+        **NOTE:** The user must explicitly use the `tester.circuit` peek/poke
+        interface, or call `tester.poke(tester._circuit, value)` since the user circuit
+        is wrapped internally (cannot call `tester.poke(Main2, value)`).
+        
+        The test finishes by calling `tester.finish_sequences()` which is a convenience
+        API that waits for the provided sequences to finish.
+        
+        Here's a different version of the above test that should fail (changing the `inc` value mid test).
+        ```python
+        
+        
+        def test_lifted_ready_valid_sequence_simple_fail():
+            I = [BitVector.random(8) for _ in range(8)] + [0]
+            O = [0] + [i + 2 for i in I[:-1]]
+            tester = f.ReadyValidTester(Main2, {"I": I, "O": O})
+            tester.circuit.inc = 2
+            # Should work for a few cycles
+            for i in range(9):
+                tester.advance_cycle()
+            # Bad inc should fail
+            tester.circuit.inc = 3
+            tester.finish_sequences()
+            with pytest.raises(AssertionError):
+                tester.compile_and_run("verilator", disp_type="realtime")
+        ```
+        
+        Finally, here's a variant that changes the `inc` value over time to match the expected sequence.
+        ```python
+        def test_lifted_ready_valid_sequence_changing_inc():
+            I = [BitVector.random(8) for _ in range(8)] + [0]
+            O = [0] + [I[i] + ((i + 1) % 2) for i in range(8)]
+            tester = f.ReadyValidTester(Main2, {"I": I, "O": O})
+            # Sequence expects inc to change over time
+            for i in range(8):
+                tester.circuit.inc = i % 2
+                tester.advance_cycle()
+                tester.wait_until_high(tester.circuit.O.ready & tester.circuit.O.valid)
+            # Advance one cycle to finish last handshake
+            tester.advance_cycle()
+            tester.expect_sequences_finished()
+            tester.compile_and_run("verilator", disp_type="realtime")
+        ```
+        
+        **NOTE:** At the end of the test, we call `expect_sequences_finished()` to
+        assert that the sequences have all been processed, otherwise it's possible tha
+        the test could pass without completing the sequences.
+        
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `fault-3.1.2/setup.py` & `fault-3.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 DESCRIPTION = """\
 A Python package for testing hardware (part of the magma ecosystem)\
 """
 
 setup(
     name='fault',
-    version='3.1.2',
+    version='3.1.3',
     description=DESCRIPTION,
     scripts=[],
     packages=[
         "fault",
         "fault.tester",
     ],
     install_requires=[
```


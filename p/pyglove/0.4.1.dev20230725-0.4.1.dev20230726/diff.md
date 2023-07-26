# Comparing `tmp/pyglove-0.4.1.dev20230725.tar.gz` & `tmp/pyglove-0.4.1.dev20230726.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglove-0.4.1.dev20230725.tar", last modified: Tue Jul 25 08:07:02 2023, max compression
+gzip compressed data, was "pyglove-0.4.1.dev20230726.tar", last modified: Wed Jul 26 08:07:06 2023, max compression
```

## Comparing `pyglove-0.4.1.dev20230725.tar` & `pyglove-0.4.1.dev20230726.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:02.381990 pyglove-0.4.1.dev20230725/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-25 08:07:02.381990 pyglove-0.4.1.dev20230725/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-25 08:07:00.000000 pyglove-0.4.1.dev20230725/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:02.353989 pyglove-0.4.1.dev20230725/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:02.353989 pyglove-0.4.1.dev20230725/pyglove/core/
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:02.353989 pyglove-0.4.1.dev20230725/pyglove/core/detouring/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/detouring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/detouring/class_detour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/detouring/class_detour_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:02.357990 pyglove-0.4.1.dev20230725/pyglove/core/geno/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/deduping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/deduping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/dna_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/dna_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/geno/sweeping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:02.361990 pyglove-0.4.1.dev20230725/pyglove/core/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/derived_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/dynamic_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/dynamic_evaluation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/evolvable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/evolvable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/iter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/object_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/hyper/object_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/logging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:02.361990 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/codegen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/common_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/common_traits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/docstr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/docstr_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/formatting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/hierarchical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/thread_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/thread_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/value_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/object_utils/value_location_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:02.365990 pyglove-0.4.1.dev20230725/pyglove/core/patching/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/patching/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/patching/object_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/patching/pattern_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/patching/pattern_based_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/patching/rule_based.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/patching/rule_based_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:02.369990 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78193 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/boilerplate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/class_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/compounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/compounding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/contextual_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    34189 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    62670 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/flags_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23955 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/functor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29174 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/functor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28899 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    55862 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    36064 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    83881 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/origin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/pure_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/symbolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/symbolic/symbolize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:02.369990 pyglove-0.4.1.dev20230725/pyglove/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/tuning/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/tuning/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/tuning/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/tuning/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/tuning/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/tuning/protocols_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/tuning/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/tuning/sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:02.373990 pyglove-0.4.1.dev20230725/pyglove/core/typing/
--rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/annotation_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/annotation_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/callable_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/callable_ext_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/callable_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/callable_signature_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    49558 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/class_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/class_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/class_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/class_schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/custom_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/key_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/key_specs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/pytype_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/type_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/typed_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/typed_missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    79781 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/value_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)   104603 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/core/typing/value_specs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:02.373990 pyglove-0.4.1.dev20230725/pyglove/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:02.373990 pyglove-0.4.1.dev20230725/pyglove/ext/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/early_stopping/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/early_stopping/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/early_stopping/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/early_stopping/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:02.377990 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/hill_climb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/hill_climb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/mutators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/neat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/neat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/recombinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/recombinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/regularized_evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/selectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/where.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/evolution/where_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:02.377990 pyglove-0.4.1.dev20230725/pyglove/ext/mutfun/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/mutfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/mutfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/mutfun/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/mutfun/basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/mutfun/basic_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:02.377990 pyglove-0.4.1.dev20230725/pyglove/ext/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/scalars/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/scalars/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/scalars/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/scalars/maths_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/scalars/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/scalars/randoms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/scalars/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/pyglove/ext/scalars/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:07:02.353989 pyglove-0.4.1.dev20230725/pyglove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-25 08:07:02.000000 pyglove-0.4.1.dev20230725/pyglove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-07-25 08:07:02.000000 pyglove-0.4.1.dev20230725/pyglove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:07:02.000000 pyglove-0.4.1.dev20230725/pyglove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 08:07:02.000000 pyglove-0.4.1.dev20230725/pyglove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 08:07:02.000000 pyglove-0.4.1.dev20230725/pyglove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 08:07:02.381990 pyglove-0.4.1.dev20230725/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-25 08:06:44.000000 pyglove-0.4.1.dev20230725/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:07:06.708295 pyglove-0.4.1.dev20230726/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-26 08:07:06.708295 pyglove-0.4.1.dev20230726/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-26 08:07:04.000000 pyglove-0.4.1.dev20230726/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:07:06.692294 pyglove-0.4.1.dev20230726/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:07:06.692294 pyglove-0.4.1.dev20230726/pyglove/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:07:06.696294 pyglove-0.4.1.dev20230726/pyglove/core/detouring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/detouring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/detouring/class_detour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/detouring/class_detour_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:07:06.696294 pyglove-0.4.1.dev20230726/pyglove/core/geno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/deduping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/deduping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/dna_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/dna_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/geno/sweeping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:07:06.696294 pyglove-0.4.1.dev20230726/pyglove/core/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/derived_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/dynamic_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/dynamic_evaluation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/evolvable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/evolvable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/iter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/object_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/hyper/object_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/logging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:07:06.700294 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/codegen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/common_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/common_traits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/docstr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/docstr_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/formatting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/hierarchical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/thread_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/thread_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/value_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/object_utils/value_location_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:07:06.700294 pyglove-0.4.1.dev20230726/pyglove/core/patching/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/patching/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/patching/object_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/patching/pattern_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/patching/pattern_based_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/patching/rule_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/patching/rule_based_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:07:06.704295 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78519 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/boilerplate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/class_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/compounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/compounding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/contextual_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35745 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64268 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/flags_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23955 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29174 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/functor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30269 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57466 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36446 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84646 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/origin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/pure_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/symbolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/symbolic/symbolize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:07:06.704295 pyglove-0.4.1.dev20230726/pyglove/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/tuning/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/tuning/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/tuning/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/tuning/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/tuning/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/tuning/protocols_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/tuning/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/tuning/sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:07:06.704295 pyglove-0.4.1.dev20230726/pyglove/core/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/annotation_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/annotation_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/callable_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/callable_ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/callable_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/callable_signature_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49558 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/class_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/class_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/class_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/class_schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/custom_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/key_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/key_specs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/pytype_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/type_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/typed_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/typed_missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79809 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/value_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105460 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/core/typing/value_specs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:07:06.704295 pyglove-0.4.1.dev20230726/pyglove/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:07:06.708295 pyglove-0.4.1.dev20230726/pyglove/ext/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/early_stopping/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/early_stopping/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/early_stopping/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/early_stopping/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:07:06.708295 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/hill_climb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/hill_climb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/mutators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/neat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/neat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/recombinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/recombinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/regularized_evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/selectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/evolution/where_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:07:06.708295 pyglove-0.4.1.dev20230726/pyglove/ext/mutfun/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/mutfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/mutfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/mutfun/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/mutfun/basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/mutfun/basic_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:07:06.708295 pyglove-0.4.1.dev20230726/pyglove/ext/scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/scalars/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/scalars/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/scalars/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/scalars/maths_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/scalars/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/scalars/randoms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/scalars/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/pyglove/ext/scalars/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:07:06.692294 pyglove-0.4.1.dev20230726/pyglove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-26 08:07:06.000000 pyglove-0.4.1.dev20230726/pyglove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-07-26 08:07:06.000000 pyglove-0.4.1.dev20230726/pyglove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 08:07:06.000000 pyglove-0.4.1.dev20230726/pyglove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 08:07:06.000000 pyglove-0.4.1.dev20230726/pyglove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 08:07:06.000000 pyglove-0.4.1.dev20230726/pyglove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 08:07:06.708295 pyglove-0.4.1.dev20230726/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-26 08:06:51.000000 pyglove-0.4.1.dev20230726/setup.py
```

### Comparing `pyglove-0.4.1.dev20230725/LICENSE` & `pyglove-0.4.1.dev20230726/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/PKG-INFO` & `pyglove-0.4.1.dev20230726/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.4.1.dev20230725
+Version: 0.4.1.dev20230726
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.4.1.dev20230725/README.md` & `pyglove-0.4.1.dev20230726/README.md`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/__init__.py` & `pyglove-0.4.1.dev20230726/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/__init__.py` & `pyglove-0.4.1.dev20230726/pyglove/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/detouring/__init__.py` & `pyglove-0.4.1.dev20230726/pyglove/core/detouring/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/detouring/class_detour.py` & `pyglove-0.4.1.dev20230726/pyglove/core/detouring/class_detour.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/detouring/class_detour_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/detouring/class_detour_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/__init__.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/base.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/base_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/categorical.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/categorical_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/custom.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/custom_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/deduping.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/deduping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/deduping_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/deduping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/dna_generator.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/dna_generator.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/dna_generator_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/dna_generator_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/numerical.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/numerical_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/random.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/random.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/random_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/random_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/space.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/space.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/space_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/space_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/sweeping.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/sweeping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/geno/sweeping_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/geno/sweeping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/__init__.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/base.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/categorical.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/categorical_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/custom.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/custom_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/derived.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/derived.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/derived_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/derived_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/dynamic_evaluation.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/dynamic_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/dynamic_evaluation_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/dynamic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/evolvable.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/evolvable.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/evolvable_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/evolvable_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/iter.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/iter.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/iter_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/iter_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/numerical.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/numerical_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/object_template.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/object_template.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/hyper/object_template_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/hyper/object_template_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/logging.py` & `pyglove-0.4.1.dev20230726/pyglove/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/logging_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/logging_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/object_utils/__init__.py` & `pyglove-0.4.1.dev20230726/pyglove/core/object_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/object_utils/codegen.py` & `pyglove-0.4.1.dev20230726/pyglove/core/object_utils/codegen.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/object_utils/codegen_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/object_utils/codegen_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/object_utils/common_traits.py` & `pyglove-0.4.1.dev20230726/pyglove/core/object_utils/common_traits.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/object_utils/common_traits_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/object_utils/common_traits_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/object_utils/docstr_utils.py` & `pyglove-0.4.1.dev20230726/pyglove/core/object_utils/docstr_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/object_utils/docstr_utils_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/object_utils/docstr_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/object_utils/formatting.py` & `pyglove-0.4.1.dev20230726/pyglove/core/object_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/object_utils/formatting_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/object_utils/formatting_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/object_utils/hierarchical.py` & `pyglove-0.4.1.dev20230726/pyglove/core/object_utils/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/object_utils/hierarchical_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/object_utils/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/object_utils/missing.py` & `pyglove-0.4.1.dev20230726/pyglove/core/object_utils/missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/object_utils/missing_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/object_utils/missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/object_utils/thread_local.py` & `pyglove-0.4.1.dev20230726/pyglove/core/object_utils/thread_local.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/object_utils/thread_local_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/object_utils/thread_local_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/object_utils/value_location.py` & `pyglove-0.4.1.dev20230726/pyglove/core/object_utils/value_location.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/object_utils/value_location_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/object_utils/value_location_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/patching/__init__.py` & `pyglove-0.4.1.dev20230726/pyglove/core/patching/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/patching/object_factory.py` & `pyglove-0.4.1.dev20230726/pyglove/core/patching/object_factory.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/patching/object_factory_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/patching/object_factory_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/patching/pattern_based.py` & `pyglove-0.4.1.dev20230726/pyglove/core/patching/pattern_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/patching/pattern_based_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/patching/pattern_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/patching/rule_based.py` & `pyglove-0.4.1.dev20230726/pyglove/core/patching/rule_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/patching/rule_based_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/patching/rule_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/__init__.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/base.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,14 +304,25 @@
     # we want to call make `__setattr__` ready to call before entering
     # other base's `__init__`.
     if init_super:
       super().__init__()
     else:
       object.__init__(self)
 
+  def _init_kwargs(self) -> Dict[str, Any]:
+    kwargs = {}
+    def add_if_nondefault(key, attrname, default):
+      v = getattr(self, attrname)
+      if v != default:
+        kwargs[key] = v
+
+    add_if_nondefault('allow_partial', '_allow_partial', False)
+    add_if_nondefault('sealed', '_sealed', False)
+    return kwargs
+
   #
   # Formal contract for symbolic operations.
   #
   # NOTE(daiyip): Since methods such as `__getattr__`, `keys` can be overriden
   # by subclasses of `pg.Object`, we introduces a set of methods in signature
   # `sym_<xxx>` as the contract to symbolically operate on a symbolic
   # value, which are less likely to clash with other names. These methods will
```

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/base_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/boilerplate.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/boilerplate.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/boilerplate_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/boilerplate_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/class_wrapper.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/class_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/class_wrapper_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/class_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/compounding.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/compounding.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/compounding_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/compounding_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/contextual.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/contextual.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/contextual_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/contextual_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/dict.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/dict.py`

 * *Files 3% similar despite different names*

```diff
@@ -535,17 +535,22 @@
     # Detach old value from object tree.
     if isinstance(old_value, base.Symbolic):
       old_value.sym_setparent(None)
       old_value.sym_setpath(object_utils.KeyPath())
 
     if (pg_typing.MISSING_VALUE == value and
         (not field or isinstance(field.key, pg_typing.NonConstKey))):
-      assert key in self, (key, self)
-      super().__delitem__(key)
-      new_value = pg_typing.MISSING_VALUE
+      if key in self:
+        # Using pg.MISSING_VALUE for deleting keys.
+        super().__delitem__(key)
+        new_value = pg_typing.MISSING_VALUE
+      else:
+        # This condition could trigger when copying a partial Dict to a Dict
+        # without schema.
+        return None
     else:
       new_value = self._formalized_value(key, field, value)
       super().__setitem__(key, new_value)
 
     # NOTE(daiyip): If current dict is the field dict of a symbolic object,
     # Use parent object as update target.
     target = self
@@ -601,14 +606,32 @@
       if self._as_object_attributes_container and self.sym_parent is not None:
         start = start.sym_parent
       v = self.sym_contextual_getattr(
           key, default=default, getter=v, start=start
       )
     return v
 
+  def _init_kwargs(self) -> typing.Dict[str, Any]:
+    kwargs = super()._init_kwargs()
+    if not self._accessor_writable:
+      kwargs['accessor_writable'] = False
+    if self._onchange_callback is not None:
+      kwargs['onchange_callback'] = self._onchange_callback
+    # NOTE(daiyip): We do not serialize ValueSpec for now as in most use
+    # cases they come from the subclasses of `pg.Object`.
+    return kwargs
+
+  def __getstate__(self) -> Any:
+    """Customizes pickle.dump."""
+    return dict(value=dict(self), kwargs=self._init_kwargs())
+
+  def __setstate__(self, state) -> None:
+    """Customizes pickle.load."""
+    self.__init__(state['value'], **state['kwargs'])
+
   def __getitem__(self, key: str) -> Any:
     """Get item in this Dict."""
     v = self.sym_value(key, default=_RAISE_IF_NOT_FOUND)
     if v is _RAISE_IF_NOT_FOUND:
       raise KeyError(key)
     return v
 
@@ -621,14 +644,26 @@
 
     Raises:
       WritePermissionError: when Dict cannot be modified by accessor or
         is sealed.
       KeyError: Key is not allowed according to the value spec.
       ValueError: Value is not acceptable according to the value spec.
     """
+    # NOTE(daiyip): THIS IS A WORKAROUND FOR WORKING WITH PICKLE.
+    # `pg.Dict` is a subclass of `dict`, therefore, when pickle loads a dict,
+    # it will try to set its items directly by calling `__setitem__` without
+    # calling `pg.Dict.__init__` at the first place. As a result, an error will
+    # raise, which complains about that an attribute set up during `__init__` is
+    # not available. A mitigation to this issue is to detect such calls in
+    # `__setitem__` as the follows, and simply do nothing, which will give a
+    # chance to `pg.Dict.__getstate__` to deal with the restoration logic as
+    # an object (instead of a dict).
+    if not hasattr(self, '_sym_parent'):
+      return
+
     if base.treats_as_sealed(self):
       raise base.WritePermissionError(
           self._error_message('Cannot modify field of a sealed Dict.'))
 
     if not base.writtable_via_accessors(self):
       raise base.WritePermissionError(
           self._error_message(
```

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/dict_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/dict_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for pyglove.Dict."""
 
 import copy
 import inspect
 import io
+import pickle
 import unittest
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
 from pyglove.core.symbolic import contextual
 from pyglove.core.symbolic import flags
@@ -2061,9 +2062,60 @@
             x = 1,
             y = ContextualValue()
           }
         """),
     )
 
 
+def _on_change_callback(updates):
+  del updates
+
+
+class PickleTest(unittest.TestCase):
+
+  def assert_pickle_correctness(self, d: Dict) -> Dict:
+    payload = pickle.dumps(d)
+    d2 = pickle.loads(payload)
+    self.assertEqual(d, d2)
+    self.assertEqual(d.sym_sealed, d2.sym_sealed)
+    self.assertEqual(d.allow_partial, d2.allow_partial)
+    # For now, deserialized `pg.Dict` does not carry value spec, which requires
+    # the user to call `use_spec` on it.
+    self.assertIsNone(d2.value_spec)
+    self.assertEqual(d.accessor_writable, d2.accessor_writable)
+    self.assertIs(d._onchange_callback, d2._onchange_callback)
+    return d2
+
+  def test_basic(self):
+    self.assert_pickle_correctness(Dict(x=1, y=2, z=Dict(p='str')))
+
+  def test_sealed(self):
+    self.assert_pickle_correctness(Dict(x=1).seal())
+
+  def test_partial(self):
+    self.assert_pickle_correctness(
+        Dict.partial(
+            x=1,
+            value_spec=pg_typing.Dict([('x', int)])))
+
+  def test_accessor_writable(self):
+    d = self.assert_pickle_correctness(Dict(x=1).set_accessor_writable(False))
+    with self.assertRaises(base.WritePermissionError):
+      d.y = 1
+
+  def test_with_value_spec(self):
+    self.assert_pickle_correctness(
+        Dict(
+            x=1, y=2, z=Dict(p='str'),
+            value_spec=pg_typing.Dict([
+                ('x', int),
+                ('y', int),
+                ('z', pg_typing.Dict([('p', str)])),
+            ])))
+
+  def test_with_onchange_callback(self):
+    self.assert_pickle_correctness(
+        Dict(x=1, y=2, onchange_callback=_on_change_callback))
+
+
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/diff.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/diff.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/diff_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/diff_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/flags.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/flags.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/flags_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/flags_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/functor.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/functor.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/functor_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/functor_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/list.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -505,14 +505,32 @@
 
     if isinstance(key, slice):
       return [
           _eval(k, v[i]) for i, k in enumerate(range(*self._parse_slice(key)))
       ]
     return _eval(key, v)
 
+  def _init_kwargs(self) -> typing.Dict[str, Any]:
+    kwargs = super()._init_kwargs()
+    if not self._accessor_writable:
+      kwargs['accessor_writable'] = False
+    if self._onchange_callback is not None:
+      kwargs['onchange_callback'] = self._onchange_callback
+    # NOTE(daiyip): We do not serialize ValueSpec for now as in most use
+    # cases they come from the subclasses of `pg.Object`.
+    return kwargs
+
+  def __getstate__(self) -> Any:
+    """Customizes pickle.dump."""
+    return dict(value=list(self), kwargs=self._init_kwargs())
+
+  def __setstate__(self, state) -> None:
+    """Customizes pickle.load."""
+    self.__init__(state['value'], **state['kwargs'])
+
   def __getitem__(self, index) -> Any:
     """Gets the item at a given position."""
     v = self.sym_value(index, _RAISE_IF_NOT_FOUND)
     if v is _RAISE_IF_NOT_FOUND:
       raise IndexError('list index out of range')
     return v
 
@@ -661,14 +679,26 @@
               f'Cannot remove item: min size ({self._value_spec.min_size}) '
               f'is reached.')
         del self[i]
         return
     raise ValueError(f'{value!r} not in list.')
 
   def extend(self, other: Iterable[Any]) -> None:
+    # NOTE(daiyip): THIS IS A WORKAROUND FOR WORKING WITH PICKLE.
+    # `pg.List` is a subclass of `list`, therefore, when pickle loads a list,
+    # it tries to set the list values directly by calling `extend` without
+    # calling `pg.List.__init__` at the first place. As a result, an error will
+    # raise, which complains about that an attribute set up during `__init__` is
+    # not available. A mitigation to this issue is to detect such calls in
+    # `extend`, and simply do nothing as follows, which will give a chance to
+    # `pg.List.__getstate__` to deal with the restoration logic as an object
+    # (instead of a list).
+    if not hasattr(self, '_sym_parent'):
+      return
+
     if base.treats_as_sealed(self):
       raise base.WritePermissionError('Cannot extend a sealed List.')
     other = list(other)
     if self.max_size is not None and len(self) + len(other) > self.max_size:
       raise ValueError(
           f'Cannot extend List: the number of elements '
           f'({len(self) + len(other)}) exceeds max size ({self.max_size}).')
```

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/list_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/list_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for pyglove.List."""
 
 import copy
 import inspect
 import io
+import pickle
 import unittest
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
 from pyglove.core.symbolic import contextual
 from pyglove.core.symbolic import flags
@@ -1781,9 +1782,59 @@
                 ]
               }
             }
           }
         ]"""))
 
 
+def _on_change_callback(updates):
+  del updates
+
+
+class PickleTest(unittest.TestCase):
+
+  def assert_pickle_correctness(self, v: List) -> List:
+    payload = pickle.dumps(v)
+    v2 = pickle.loads(payload)
+    self.assertEqual(v, v2)
+    self.assertEqual(v.sym_sealed, v2.sym_sealed)
+    self.assertEqual(v.sym_partial, v2.sym_partial)
+    # For now, deserialized `pg.List` does not carry value spec, which requires
+    # the user to call `use_spec` on it.
+    self.assertIsNone(v2.value_spec)
+    self.assertEqual(v.accessor_writable, v2.accessor_writable)
+    self.assertEqual(v._onchange_callback, v2._onchange_callback)
+    return v2
+
+  def test_basic(self):
+    self.assert_pickle_correctness(List([0, Dict(x=1)]))
+
+  def test_sealed(self):
+    self.assert_pickle_correctness(List([0]).seal())
+
+  def test_partial(self):
+    self.assert_pickle_correctness(
+        List.partial(
+            value_spec=pg_typing.List(pg_typing.Dict([('x', int)]))))
+
+  def test_accessor_writable(self):
+    v = self.assert_pickle_correctness(List([0]).set_accessor_writable(False))
+    with self.assertRaises(base.WritePermissionError):
+      v[0] = 1
+
+  def test_with_value_spec(self):
+    self.assert_pickle_correctness(
+        List(
+            [Dict(x=1, y=2, z=Dict(p='str'))],
+            value_spec=pg_typing.List(pg_typing.Dict([
+                ('x', int),
+                ('y', int),
+                ('z', pg_typing.Dict([('p', str)])),
+            ]))))
+
+  def test_with_onchange_callback(self):
+    self.assert_pickle_correctness(
+        List([], onchange_callback=_on_change_callback))
+
+
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/object.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -756,14 +756,27 @@
     """Returns True if current object subscribes field updates.
 
     For pg.Object, this return True only when _on_change is overridden
     from subclass.
     """
     return self._on_change.__code__ is not Object._on_change.__code__  # pytype: disable=attribute-error
 
+  def _init_kwargs(self) -> typing.Dict[str, Any]:
+    kwargs = super()._init_kwargs()
+    kwargs.update(self._sym_attributes)
+    return kwargs
+
+  def __getstate__(self) -> Dict[str, Any]:
+    """Customizes pickle.dump."""
+    return dict(kwargs=self._init_kwargs())
+
+  def __setstate__(self, state) -> None:
+    """Customizes pickle.load."""
+    self.__init__(**state['kwargs'])
+
   def __setattr__(self, name: str, value: Any) -> None:
     """Set field value by attribute."""
     # NOTE(daiyip): two types of members are treated as regular members:
     # 1) All private members which prefixed with '_'.
     # 2) Public members that are not declared as symbolic members.
     if (not self.allow_symbolic_attribute
         or not self.__class__.schema.get_field(name)
```

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/object_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/object_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 """Tests for pyglove.Object."""
 
 import copy
 import inspect
 import io
 import os
+import pickle
 import tempfile
 import typing
 import unittest
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
@@ -3126,9 +3127,36 @@
                 )
               }
             )
           ]
         )"""))
 
 
+class Foo(Object):
+  x: typing.List[typing.Dict[str, int]] = [dict(x=1)]
+  y: typing.Dict[str, int]
+  z: bool = True
+
+
+class PickleTest(unittest.TestCase):
+
+  def assert_pickle_correctness(self, v: Object) -> Object:
+    payload = pickle.dumps(v)
+    v2 = pickle.loads(payload)
+    self.assertEqual(v, v2)
+    self.assertEqual(v.sym_sealed, v2.sym_sealed)
+    self.assertEqual(v.sym_partial, v2.sym_partial)
+    self.assertEqual(v.accessor_writable, v2.accessor_writable)
+    return v2
+
+  def test_basic(self):
+    self.assert_pickle_correctness(Foo([dict(x=2)], dict(x=1)))
+
+  def test_sealed(self):
+    self.assert_pickle_correctness(Foo([dict(x=2)], dict(x=1)).seal())
+
+  def test_partial(self):
+    self.assert_pickle_correctness(Foo.partial())
+
+
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/origin.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/origin.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/origin_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/origin_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/pure_symbolic.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/pure_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/schema_utils.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/schema_utils_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/symbolize.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/symbolize.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/symbolic/symbolize_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/symbolic/symbolize_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/tuning/__init__.py` & `pyglove-0.4.1.dev20230726/pyglove/core/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/tuning/backend.py` & `pyglove-0.4.1.dev20230726/pyglove/core/tuning/backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/tuning/backend_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/tuning/backend_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/tuning/early_stopping.py` & `pyglove-0.4.1.dev20230726/pyglove/core/tuning/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/tuning/local_backend.py` & `pyglove-0.4.1.dev20230726/pyglove/core/tuning/local_backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/tuning/protocols.py` & `pyglove-0.4.1.dev20230726/pyglove/core/tuning/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/tuning/protocols_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/tuning/protocols_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/tuning/sample.py` & `pyglove-0.4.1.dev20230726/pyglove/core/tuning/sample.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/tuning/sample_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/tuning/sample_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/__init__.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/annotation_conversion.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/annotation_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/annotation_conversion_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/annotation_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/callable_ext.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/callable_ext.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/callable_ext_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/callable_ext_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/callable_signature.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/callable_signature.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/callable_signature_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/callable_signature_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/class_schema.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/class_schema.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/class_schema_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/class_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/class_schema_utils.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/class_schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/class_schema_utils_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/class_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/custom_typing.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/generic.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/generic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/generic_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/generic_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/key_specs.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/key_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/key_specs_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/key_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/pytype_support.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/pytype_support.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/type_conversion.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/type_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/type_conversion_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/typed_missing.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/typed_missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/typed_missing_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/typed_missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/value_specs.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/value_specs.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Concrete value specifications for field definition."""
+
 import copy
 import functools
 import inspect
 import numbers
 import re
 import sys
 import typing
-
 import __main__
+
 from pyglove.core import object_utils
 from pyglove.core.typing import callable_signature
 from pyglove.core.typing import class_schema
 from pyglove.core.typing import generic
 from pyglove.core.typing import key_specs
 from pyglove.core.typing import type_conversion
 from pyglove.core.typing import typed_missing
@@ -1466,15 +1467,15 @@
 
   def _is_compatible(self, other: 'Object') -> bool:
     """Object specific compatiblity check."""
     # NOTE(daiyip): When either the current spec or the other spec contains
     # unresolved forward declarations, we consider them compatible.
     if not self.type_resolved or not other.type_resolved:
       return True
-    return issubclass(other.cls, self.cls)
+    return generic.is_subclass(other.cls, self.cls)
 
   def _annotate(self) -> typing.Any:
     """Annotate with PyType annotation."""
     if self._forward_ref is not None:
       return self._forward_ref.as_annotation()
     return self._value_type
 
@@ -1876,15 +1877,15 @@
 
   def _is_compatible(self, other: 'Type') -> bool:
     """Type specific compatiblity check."""
     # NOTE(daiyip): When either the current spec or the other spec contains
     # unresolved forward declarations, we consider them compatible.
     if not self.type_resolved or not other.type_resolved:
       return True
-    return issubclass(other.type, self.type)
+    return generic.is_subclass(other.type, self.type)
 
   def _extend(self, base: 'Type') -> None:
     """Type specific extension."""
     if not base.is_compatible(self):
       raise TypeError(f'{self!r} cannot extend {base!r}: incompatible type.')
 
   def _annotate(self) -> typing.Any:
@@ -2098,15 +2099,15 @@
         for vc in v.candidates:
           p = _base_candidate(c, vc)
           if p is not None:
             return p
       else:
         if (c.__class__ is v.__class__
             and (c.__class__ is not Object
-                 or issubclass(c.value_type, v.value_type))):
+                 or generic.is_subclass(c.value_type, v.value_type))):
           return v
       return None
 
     for sc in self.candidates:
       bc = _base_candidate(sc, base)
       if bc is None:
         raise TypeError(
```

### Comparing `pyglove-0.4.1.dev20230725/pyglove/core/typing/value_specs_test.py` & `pyglove-0.4.1.dev20230726/pyglove/core/typing/value_specs_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1738,15 +1738,15 @@
 
     with simulate_forward_declaration(self.A):
       self.assertIs(v.value_type, self.A)
 
     with self.assertRaisesRegex(TypeError, "'A' does not exist in module .*"):
       _ = vs.Object('A').value_type
 
-  def test_geneeric_type(self):
+  def test_generic_type(self):
     class G(typing.Generic[typing.TypeVar('X'), typing.TypeVar('Y')]):
       pass
 
     class G1(G[int, str]):
       pass
 
     o = G1()
@@ -1755,14 +1755,22 @@
     self.assertIs(v.value_type, G[int, str])
     self.assertIs(v.apply(o), o)
 
     self.assertIs(vs.Object(G).apply(o), o)
     with self.assertRaisesRegex(TypeError, 'Expect .* but encountered .*'):
       vs.Object(G[str, int]).apply(o)
 
+    self.assertTrue(
+        vs.Object(G[int, typing.Any]).is_compatible(vs.Object(G[int, str])))
+    self.assertTrue(
+        vs.Object(G[typing.Any, typing.Any]).is_compatible(
+            vs.Object(G[int, str])))
+    self.assertFalse(
+        vs.Object(G[int, str]).is_compatible(vs.Object(G[str, str])))
+
   def test_forward_refs(self):
     self.assertEqual(vs.Object(self.A).forward_refs, set())
     self.assertEqual(vs.Object('Foo').forward_refs, set([forward_ref('Foo')]))
 
   def test_default(self):
     self.assertEqual(vs.Object(self.A).default, typed_missing.MISSING_VALUE)
     a = self.A()
@@ -2480,14 +2488,29 @@
 
     self.assertTrue(
         vs.Type(Exception).noneable().is_compatible(vs.Type(ValueError)))
     self.assertFalse(
         vs.Type(Exception).is_compatible(vs.Type(ValueError).noneable()))
     self.assertFalse(vs.Type(Exception).is_compatible(vs.Type(int)))
 
+    class G(typing.Generic[typing.TypeVar('T1'), typing.TypeVar('T2')]):
+      pass
+
+    class G1(G[int, str]):
+      pass
+
+    self.assertTrue(vs.Type(G[int, str]).is_compatible(vs.Type(G1)))
+    self.assertTrue(
+        vs.Type(G[typing.Any, typing.Any]).is_compatible(vs.Type(G1)))
+    self.assertTrue(
+        vs.Type(G[typing.Any, typing.Any]).is_compatible(
+            vs.Type(G[int, str])))
+    self.assertFalse(vs.Type(G[str, int]).is_compatible(vs.Type(G[int, int])))
+    self.assertFalse(vs.Type(G[str, int]).is_compatible(vs.Type(G1)))
+
   def test_extend(self):
     # Child may make a parent default value not specified.
     self.assertEqual(
         vs.Type(Exception).extend(
             vs.Type(Exception, default=ValueError)).default,
         typed_missing.MISSING_VALUE)
```

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/__init__.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/early_stopping/__init__.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/early_stopping/base.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/early_stopping/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/early_stopping/base_test.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/early_stopping/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/early_stopping/step_wise.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/early_stopping/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/early_stopping/step_wise_test.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/early_stopping/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/__init__.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/base.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/base_test.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/hill_climb.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/hill_climb.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/hill_climb_test.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/hill_climb_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/mutators.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/mutators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/mutators_test.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/mutators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/neat.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/neat.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/neat_test.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/neat_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/nsga2.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/nsga2_test.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/recombinators.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/recombinators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/recombinators_test.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/recombinators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/regularized_evolution.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/regularized_evolution_test.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/regularized_evolution_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/selectors.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/selectors.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/selectors_test.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/selectors_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/where.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/where.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/evolution/where_test.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/evolution/where_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/mutfun/__init__.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/mutfun/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/mutfun/base.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/mutfun/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/mutfun/base_test.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/mutfun/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/mutfun/basic_ops.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/mutfun/basic_ops.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/mutfun/basic_ops_test.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/mutfun/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/scalars/__init__.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/scalars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/scalars/base.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/scalars/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/scalars/base_test.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/scalars/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/scalars/maths.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/scalars/maths.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/scalars/maths_test.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/scalars/maths_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/scalars/randoms.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/scalars/randoms.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/scalars/randoms_test.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/scalars/randoms_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/scalars/step_wise.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/scalars/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove/ext/scalars/step_wise_test.py` & `pyglove-0.4.1.dev20230726/pyglove/ext/scalars/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/pyglove.egg-info/PKG-INFO` & `pyglove-0.4.1.dev20230726/pyglove.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.4.1.dev20230725
+Version: 0.4.1.dev20230726
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.4.1.dev20230725/pyglove.egg-info/SOURCES.txt` & `pyglove-0.4.1.dev20230726/pyglove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyglove-0.4.1.dev20230725/setup.py` & `pyglove-0.4.1.dev20230726/setup.py`

 * *Files identical despite different names*


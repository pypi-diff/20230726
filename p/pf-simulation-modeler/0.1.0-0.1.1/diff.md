# Comparing `tmp/pf-simulation-modeler-0.1.0.tar.gz` & `tmp/pf-simulation-modeler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pf-simulation-modeler-0.1.0.tar", last modified: Wed Jul 26 18:28:12 2023, max compression
+gzip compressed data, was "pf-simulation-modeler-0.1.1.tar", last modified: Wed Jul 26 18:50:55 2023, max compression
```

## Comparing `pf-simulation-modeler-0.1.0.tar` & `pf-simulation-modeler-0.1.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:28:12.836063 pf-simulation-modeler-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      583 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       86 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      762 2023-07-26 18:28:12.836063 pf-simulation-modeler-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:28:12.824063 pf-simulation-modeler-0.1.0/pf_simulation_modeler/
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:28:12.824063 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1223 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:28:12.828063 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/
--rw-r--r--   0 root         (0) root         (0)       64 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2684 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/boundary_conditions.py
--rw-r--r--   0 root         (0) root         (0)     3617 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/cli.py
--rw-r--r--   0 root         (0) root         (0)     4961 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/domain.py
--rw-r--r--   0 root         (0) root         (0)     4500 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)     7554 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:28:12.832063 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/
--rw-r--r--   0 root         (0) root         (0)      559 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/boundary.yaml
--rw-r--r--   0 root         (0) root         (0)      572 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/boundary_ui.xml
--rw-r--r--   0 root         (0) root         (0)      239 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/cycle.yaml
--rw-r--r--   0 root         (0) root         (0)      446 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/cycle_ui.xml
--rw-r--r--   0 root         (0) root         (0)      730 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/domain.yaml
--rw-r--r--   0 root         (0) root         (0)      846 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/domain_ui.xml
--rw-r--r--   0 root         (0) root         (0)      965 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/output_readme.md
--rw-r--r--   0 root         (0) root         (0)     1254 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/soil.yaml
--rw-r--r--   0 root         (0) root         (0)     1651 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/soil_ui.xml
--rw-r--r--   0 root         (0) root         (0)     2245 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/solver.yaml
--rw-r--r--   0 root         (0) root         (0)     1368 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/solver_ui.xml
--rw-r--r--   0 root         (0) root         (0)      334 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/timing.yaml
--rw-r--r--   0 root         (0) root         (0)      860 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/pressure.py
--rw-r--r--   0 root         (0) root         (0)     2726 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/save_project.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:28:12.832063 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/snippets/
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/snippets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4813 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/snippets/boundary_conditions.py
--rw-r--r--   0 root         (0) root         (0)     4357 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/snippets/domain.py
--rw-r--r--   0 root         (0) root         (0)     2211 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/snippets/domain_builder.py
--rw-r--r--   0 root         (0) root         (0)     3437 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/snippets/snippet_manager.py
--rw-r--r--   0 root         (0) root         (0)     4599 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/snippets/solver.py
--rw-r--r--   0 root         (0) root         (0)     2826 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/snippets/subsurface_properties.py
--rw-r--r--   0 root         (0) root         (0)     2880 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/snippets/timing.py
--rw-r--r--   0 root         (0) root         (0)      487 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/solver.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/timing.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/jupyter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:28:12.836063 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)      694 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/boundary_conditions.py
--rw-r--r--   0 root         (0) root         (0)      478 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/code_gen.py
--rw-r--r--   0 root         (0) root         (0)     4597 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/domain.py
--rw-r--r--   0 root         (0) root         (0)      324 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/file_db.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/pressure.py
--rw-r--r--   0 root         (0) root         (0)     7573 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/save_project.py
--rw-r--r--   0 root         (0) root         (0)     1069 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/simulation_type.py
--rw-r--r--   0 root         (0) root         (0)     2185 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/snippet.py
--rw-r--r--   0 root         (0) root         (0)     1344 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/solver.py
--rw-r--r--   0 root         (0) root         (0)      721 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/subsurface_props.py
--rw-r--r--   0 root         (0) root         (0)     1775 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/timing.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:28:12.836063 pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/
--rw-r--r--   0 root         (0) root         (0)      757 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:28:12.836063 pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/serve/
--rw-r--r--   0 root         (0) root         (0)      176 2023-07-26 18:28:07.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/serve/demo.html
--rw-r--r--   0 root         (0) root         (0)    29403 2023-07-26 18:28:08.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/serve/vue-pfsm.common.js
--rw-r--r--   0 root         (0) root         (0)    39644 2023-07-26 18:28:08.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/serve/vue-pfsm.common.js.map
--rw-r--r--   0 root         (0) root         (0)      887 2023-07-26 18:28:08.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/serve/vue-pfsm.css
--rw-r--r--   0 root         (0) root         (0)    29787 2023-07-26 18:28:07.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/serve/vue-pfsm.umd.js
--rw-r--r--   0 root         (0) root         (0)    40181 2023-07-26 18:28:07.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/serve/vue-pfsm.umd.js.map
--rw-r--r--   0 root         (0) root         (0)    13852 2023-07-26 18:28:08.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/serve/vue-pfsm.umd.min.js
--rw-r--r--   0 root         (0) root         (0)    44102 2023-07-26 18:28:08.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/serve/vue-pfsm.umd.min.js.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:28:12.836063 pf-simulation-modeler-0.1.0/pf_simulation_modeler/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler/widgets/pfsm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:28:12.824063 pf-simulation-modeler-0.1.0/pf_simulation_modeler.egg-info/
--rw-r--r--   0 root         (0) root         (0)      762 2023-07-26 18:28:12.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3099 2023-07-26 18:28:12.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 18:28:12.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      190 2023-07-26 18:28:12.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-26 18:28:12.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 18:28:12.000000 pf-simulation-modeler-0.1.0/pf_simulation_modeler.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1181 2023-07-26 18:28:12.836063 pf-simulation-modeler-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 18:27:39.000000 pf-simulation-modeler-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:50:55.112947 pf-simulation-modeler-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)      583 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       86 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2430 2023-07-26 18:50:55.112947 pf-simulation-modeler-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:50:55.092947 pf-simulation-modeler-0.1.1/pf_simulation_modeler/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:50:55.096947 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:50:55.096947 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/boundary_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     3617 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/cli.py
+-rw-r--r--   0 root         (0) root         (0)     4961 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/domain.py
+-rw-r--r--   0 root         (0) root         (0)     4500 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)     7554 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:50:55.100947 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/
+-rw-r--r--   0 root         (0) root         (0)      559 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/boundary.yaml
+-rw-r--r--   0 root         (0) root         (0)      572 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/boundary_ui.xml
+-rw-r--r--   0 root         (0) root         (0)      239 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/cycle.yaml
+-rw-r--r--   0 root         (0) root         (0)      446 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/cycle_ui.xml
+-rw-r--r--   0 root         (0) root         (0)      730 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/domain.yaml
+-rw-r--r--   0 root         (0) root         (0)      846 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/domain_ui.xml
+-rw-r--r--   0 root         (0) root         (0)      965 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/output_readme.md
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/soil.yaml
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/soil_ui.xml
+-rw-r--r--   0 root         (0) root         (0)     2245 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/solver.yaml
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/solver_ui.xml
+-rw-r--r--   0 root         (0) root         (0)      334 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/timing.yaml
+-rw-r--r--   0 root         (0) root         (0)      860 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/pressure.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/save_project.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:50:55.104947 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/snippets/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/snippets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4813 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/snippets/boundary_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     4357 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/snippets/domain.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/snippets/domain_builder.py
+-rw-r--r--   0 root         (0) root         (0)     3437 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/snippets/snippet_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4599 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/snippets/solver.py
+-rw-r--r--   0 root         (0) root         (0)     2826 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/snippets/subsurface_properties.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/snippets/timing.py
+-rw-r--r--   0 root         (0) root         (0)      487 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/solver.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/timing.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/jupyter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:50:55.108947 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      694 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/boundary_conditions.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/code_gen.py
+-rw-r--r--   0 root         (0) root         (0)     4597 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/domain.py
+-rw-r--r--   0 root         (0) root         (0)      324 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/file_db.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/pressure.py
+-rw-r--r--   0 root         (0) root         (0)     7573 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/save_project.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/simulation_type.py
+-rw-r--r--   0 root         (0) root         (0)     2185 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/snippet.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/solver.py
+-rw-r--r--   0 root         (0) root         (0)      721 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/subsurface_props.py
+-rw-r--r--   0 root         (0) root         (0)     1775 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/timing.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:50:55.108947 pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/
+-rw-r--r--   0 root         (0) root         (0)      757 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:50:55.108947 pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/serve/
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-26 18:50:50.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/serve/demo.html
+-rw-r--r--   0 root         (0) root         (0)    29403 2023-07-26 18:50:50.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/serve/vue-pfsm.common.js
+-rw-r--r--   0 root         (0) root         (0)    39644 2023-07-26 18:50:50.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/serve/vue-pfsm.common.js.map
+-rw-r--r--   0 root         (0) root         (0)      887 2023-07-26 18:50:50.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/serve/vue-pfsm.css
+-rw-r--r--   0 root         (0) root         (0)    29787 2023-07-26 18:50:50.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/serve/vue-pfsm.umd.js
+-rw-r--r--   0 root         (0) root         (0)    40181 2023-07-26 18:50:50.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/serve/vue-pfsm.umd.js.map
+-rw-r--r--   0 root         (0) root         (0)    13852 2023-07-26 18:50:50.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/serve/vue-pfsm.umd.min.js
+-rw-r--r--   0 root         (0) root         (0)    44102 2023-07-26 18:50:50.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/serve/vue-pfsm.umd.min.js.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:50:55.112947 pf-simulation-modeler-0.1.1/pf_simulation_modeler/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler/widgets/pfsm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:50:55.096947 pf-simulation-modeler-0.1.1/pf_simulation_modeler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2430 2023-07-26 18:50:55.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3099 2023-07-26 18:50:55.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 18:50:55.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      190 2023-07-26 18:50:55.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-26 18:50:55.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 18:50:55.000000 pf-simulation-modeler-0.1.1/pf_simulation_modeler.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1183 2023-07-26 18:50:55.112947 pf-simulation-modeler-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 18:50:04.000000 pf-simulation-modeler-0.1.1/setup.py
```

### Comparing `pf-simulation-modeler-0.1.0/LICENSE` & `pf-simulation-modeler-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/README.md` & `pf-simulation-modeler-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/__main__.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/__main__.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/boundary_conditions.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/cli.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/cli.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/domain.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/domain.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/engine.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/engine.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/files.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/files.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/boundary.yaml` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/boundary.yaml`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/boundary_ui.xml` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/boundary_ui.xml`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/domain.yaml` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/domain.yaml`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/domain_ui.xml` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/domain_ui.xml`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/output_readme.md` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/output_readme.md`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/soil.yaml` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/soil.yaml`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/soil_ui.xml` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/soil_ui.xml`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/solver.yaml` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/solver.yaml`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/model/solver_ui.xml` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/model/solver_ui.xml`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/pressure.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/pressure.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/save_project.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/save_project.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/snippets/boundary_conditions.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/snippets/boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/snippets/domain.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/snippets/domain.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/snippets/domain_builder.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/snippets/domain_builder.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/snippets/snippet_manager.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/snippets/snippet_manager.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/snippets/solver.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/snippets/solver.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/snippets/subsurface_properties.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/snippets/subsurface_properties.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/snippets/timing.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/snippets/timing.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/engine/timing.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/engine/timing.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/jupyter.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/boundary_conditions.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/domain.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/domain.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/pressure.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/pressure.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/save_project.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/save_project.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/simulation_type.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/simulation_type.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/snippet.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/snippet.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/solver.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/solver.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/subsurface_props.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/subsurface_props.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/timing.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/timing.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/app/ui/ui.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/app/ui/ui.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/__init__.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/__init__.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/serve/vue-pfsm.common.js` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/serve/vue-pfsm.common.js`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/serve/vue-pfsm.common.js.map` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/serve/vue-pfsm.common.js.map`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/serve/vue-pfsm.css` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/serve/vue-pfsm.css`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/serve/vue-pfsm.umd.js` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/serve/vue-pfsm.umd.js`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/serve/vue-pfsm.umd.js.map` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/serve/vue-pfsm.umd.js.map`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/serve/vue-pfsm.umd.min.js` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/serve/vue-pfsm.umd.min.js`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/module/serve/vue-pfsm.umd.min.js.map` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/module/serve/vue-pfsm.umd.min.js.map`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler/widgets/pfsm.py` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler/widgets/pfsm.py`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/pf_simulation_modeler.egg-info/SOURCES.txt` & `pf-simulation-modeler-0.1.1/pf_simulation_modeler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pf-simulation-modeler-0.1.0/setup.cfg` & `pf-simulation-modeler-0.1.1/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = pf-simulation-modeler
-version = 0.1.0
+version = 0.1.1
 description = Parflow Simulation modeler
-long_description = file: README.rst
-long_description_content_type = text/x-rst
+long_description = file: README.md
+long_description_content_type = text/markdown
 author = Kitware Inc.
 license = Apache Software License
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
 	License :: OSI Approved :: Apache Software License
 	Natural Language :: English
```


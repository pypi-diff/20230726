# Comparing `tmp/PDKMaster-0.9.3.tar.gz` & `tmp/PDKMaster-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PDKMaster-0.9.3.tar", last modified: Sat Jun 24 16:06:49 2023, max compression
+gzip compressed data, was "PDKMaster-0.9.4.tar", last modified: Wed Jul 26 12:05:03 2023, max compression
```

## Comparing `PDKMaster-0.9.3.tar` & `PDKMaster-0.9.4.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.972625 PDKMaster-0.9.3/
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.940625 PDKMaster-0.9.3/.ci/
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1069 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/.ci/check-dco.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      155 2022-01-13 16:15:17.000000 PDKMaster-0.9.3/.gitignore
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2183 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/.gitlab-ci.yml
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6586 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/Contributing.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      566 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/LICENSE.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.940625 PDKMaster-0.9.3/LICENSES/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2021-02-28 15:28:15.000000 PDKMaster-0.9.3/LICENSES/agpl-3.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    11358 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/LICENSES/apache-2.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2021-02-28 15:28:15.000000 PDKMaster-0.9.3/LICENSES/cern_ohl_s_v2.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2021-02-28 15:28:15.000000 PDKMaster-0.9.3/LICENSES/gpl-2.0.txt
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.940625 PDKMaster-0.9.3/PDKMaster.egg-info/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9707 2023-06-24 16:06:49.000000 PDKMaster-0.9.3/PDKMaster.egg-info/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3966 2023-06-24 16:06:49.000000 PDKMaster-0.9.3/PDKMaster.egg-info/SOURCES.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-06-24 16:06:49.000000 PDKMaster-0.9.3/PDKMaster.egg-info/dependency_links.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2023-06-24 16:06:49.000000 PDKMaster-0.9.3/PDKMaster.egg-info/requires.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       15 2023-06-24 16:06:49.000000 PDKMaster-0.9.3/PDKMaster.egg-info/top_level.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9707 2023-06-24 16:06:49.972625 PDKMaster-0.9.3/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9239 2023-06-24 15:43:31.000000 PDKMaster-0.9.3/README.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.940625 PDKMaster-0.9.3/ReleaseNotes/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      442 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/ReleaseNotes/v0.1.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1234 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/ReleaseNotes/v0.2.0.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1471 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/ReleaseNotes/v0.3.0.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2547 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/ReleaseNotes/v0.9.0.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.944625 PDKMaster-0.9.3/assura_yaml/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2020-03-11 19:28:52.000000 PDKMaster-0.9.3/assura_yaml/.keepme
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      595 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/checkskill.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       14 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/ci-requirements.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2022-06-14 17:01:59.000000 PDKMaster-0.9.3/dev-requirements.txt
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.944625 PDKMaster-0.9.3/display_yaml/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2020-03-11 19:28:52.000000 PDKMaster-0.9.3/display_yaml/.keepme
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.932624 PDKMaster-0.9.3/docs/
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.944625 PDKMaster-0.9.3/docs/src/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6063 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/docs/src/conf.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      456 2021-07-22 09:01:44.000000 PDKMaster-0.9.3/docs/src/index.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      141 2021-07-22 09:01:44.000000 PDKMaster-0.9.3/docs/src/pdkmaster._util.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      560 2021-07-22 09:01:44.000000 PDKMaster-0.9.3/docs/src/pdkmaster.design.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      443 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/docs/src/pdkmaster.dispatch.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      312 2022-01-13 16:15:17.000000 PDKMaster-0.9.3/docs/src/pdkmaster.io.coriolis.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      462 2022-02-15 17:28:27.000000 PDKMaster-0.9.3/docs/src/pdkmaster.io.klayout.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      934 2021-07-22 09:01:44.000000 PDKMaster-0.9.3/docs/src/pdkmaster.io.parsing.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      318 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/docs/src/pdkmaster.io.pdkmaster.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      262 2022-01-13 16:15:17.000000 PDKMaster-0.9.3/docs/src/pdkmaster.io.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      449 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/docs/src/pdkmaster.io.spice.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      290 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/docs/src/pdkmaster.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1556 2022-01-13 16:15:17.000000 PDKMaster-0.9.3/docs/src/pdkmaster.technology.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3746 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/dodo.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     4469 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/extract_rules.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    26261 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/files.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.948624 PDKMaster-0.9.3/pdkmaster/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      709 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18133 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/_util.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.948624 PDKMaster-0.9.3/pdkmaster/design/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      237 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/design/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6045 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/design/cell.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10199 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/design/circuit.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     8637 2023-04-25 12:12:06.000000 PDKMaster-0.9.3/pdkmaster/design/factory.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.948624 PDKMaster-0.9.3/pdkmaster/design/layout/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      664 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/design/layout/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    28610 2023-06-02 15:47:08.000000 PDKMaster-0.9.3/pdkmaster/design/layout/_circuitlayouter.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    48524 2023-05-26 16:05:30.000000 PDKMaster-0.9.3/pdkmaster/design/layout/_primitivelayouter.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3335 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/design/layout/factory_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    22622 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/design/layout/layout_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2887 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/design/library.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2600 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/design/routinggauge.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.952625 PDKMaster-0.9.3/pdkmaster/dispatch/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1375 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/dispatch/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1378 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/dispatch/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1956 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/dispatch/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7326 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/dispatch/primitive.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2803 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/dispatch/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3801 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/dispatch/shape.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.952625 PDKMaster-0.9.3/pdkmaster/io/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.952625 PDKMaster-0.9.3/pdkmaster/io/coriolis/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/coriolis/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    58622 2023-05-30 07:56:45.000000 PDKMaster-0.9.3/pdkmaster/io/coriolis/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.952625 PDKMaster-0.9.3/pdkmaster/io/klayout/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      142 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/klayout/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37892 2023-05-26 16:05:30.000000 PDKMaster-0.9.3/pdkmaster/io/klayout/export.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    23519 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/klayout/merge_.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.952625 PDKMaster-0.9.3/pdkmaster/io/lefdef/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      261 2023-05-30 07:56:45.000000 PDKMaster-0.9.3/pdkmaster/io/lefdef/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9950 2023-05-30 07:56:45.000000 PDKMaster-0.9.3/pdkmaster/io/lefdef/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.952625 PDKMaster-0.9.3/pdkmaster/io/notebook/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      121 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/notebook/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1253 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/notebook/plotter.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.956625 PDKMaster-0.9.3/pdkmaster/io/parsing/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      214 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/parsing/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18847 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/parsing/assura.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      422 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/parsing/display.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      822 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/parsing/layermap.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17548 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/parsing/skill_grammar.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24374 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/parsing/tf.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.956625 PDKMaster-0.9.3/pdkmaster/io/pdkmaster/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/pdkmaster/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18079 2023-05-26 16:05:30.000000 PDKMaster-0.9.3/pdkmaster/io/pdkmaster/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.956625 PDKMaster-0.9.3/pdkmaster/io/spice/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      165 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/spice/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    15809 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/spice/pyspice.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     5904 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/spice/spice_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      181 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/io/spice/typing.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.960625 PDKMaster-0.9.3/pdkmaster/technology/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      276 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4032 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    77846 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/geometry.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17939 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      627 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/net.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.960625 PDKMaster-0.9.3/pdkmaster/technology/primitive/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      466 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/primitive/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9661 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/primitive/_core.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1519 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/primitive/_derived.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1176 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/primitive/_param.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24763 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/primitive/conductors.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    44372 2023-05-30 07:56:57.000000 PDKMaster-0.9.3/pdkmaster/technology/primitive/devices.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4914 2023-05-30 07:56:57.000000 PDKMaster-0.9.3/pdkmaster/technology/primitive/layers.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6752 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/primitive/rules.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9109 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/property_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2138 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    20002 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/technology_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2059 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/pdkmaster/technology/wafer_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3224 2023-05-30 07:56:45.000000 PDKMaster-0.9.3/pdkmaster/typing.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-06-24 16:06:49.972625 PDKMaster-0.9.3/setup.cfg
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1410 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/setup.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      863 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/skill.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1278 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/skill2yaml.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.960625 PDKMaster-0.9.3/test/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.964625 PDKMaster-0.9.3/test/unit/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7946 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/_util.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.964625 PDKMaster-0.9.3/test/unit/design/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/design/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3025 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/design/cell.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2470 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/design/circuit.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3664 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/design/factory.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37534 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/design/layout.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4584 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/design/library.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.964625 PDKMaster-0.9.3/test/unit/dispatch/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/dispatch/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1343 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/dispatch/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1397 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/dispatch/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1688 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/dispatch/primitive.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1531 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/dispatch/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3403 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/dispatch/shape.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13091 2023-05-30 07:56:45.000000 PDKMaster-0.9.3/test/unit/dummy.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.964625 PDKMaster-0.9.3/test/unit/io/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/io/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.968625 PDKMaster-0.9.3/test/unit/io/klayout/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/io/klayout/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13480 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/io/klayout/export.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    20839 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/io/klayout/merge.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.968625 PDKMaster-0.9.3/test/unit/io/lefdef/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-05-30 07:56:45.000000 PDKMaster-0.9.3/test/unit/io/lefdef/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1573 2023-05-30 07:56:45.000000 PDKMaster-0.9.3/test/unit/io/lefdef/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.968625 PDKMaster-0.9.3/test/unit/io/pdkmaster/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/io/pdkmaster/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1862 2023-05-26 16:05:30.000000 PDKMaster-0.9.3/test/unit/io/pdkmaster/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.968625 PDKMaster-0.9.3/test/unit/io/spice/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/io/spice/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7947 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/io/spice/pyspice.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1317 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/io/spice/spice_.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.972625 PDKMaster-0.9.3/test/unit/technology/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/technology/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1313 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/technology/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    56025 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/technology/geometry.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6112 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/technology/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    53443 2023-05-26 16:05:30.000000 PDKMaster-0.9.3/test/unit/technology/primitive.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2775 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/technology/property.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2072 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/technology/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    12778 2023-05-26 16:05:30.000000 PDKMaster-0.9.3/test/unit/technology/technology.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1052 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/technology/wafer.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1278 2023-04-07 09:59:24.000000 PDKMaster-0.9.3/test/unit/typing.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      673 2020-03-11 19:28:52.000000 PDKMaster-0.9.3/test.tf
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 16:06:49.972625 PDKMaster-0.9.3/tf_yaml/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2020-03-11 19:28:52.000000 PDKMaster-0.9.3/tf_yaml/.keepme
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.104557 PDKMaster-0.9.4/
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.072557 PDKMaster-0.9.4/.ci/
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1069 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/.ci/check-dco.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      155 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/.gitignore
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2183 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/.gitlab-ci.yml
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6586 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/Contributing.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      566 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/LICENSE.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.072557 PDKMaster-0.9.4/LICENSES/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/LICENSES/agpl-3.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    11358 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/LICENSES/apache-2.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/LICENSES/cern_ohl_s_v2.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/LICENSES/gpl-2.0.txt
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.076557 PDKMaster-0.9.4/PDKMaster.egg-info/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9871 2023-07-26 12:05:02.000000 PDKMaster-0.9.4/PDKMaster.egg-info/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3966 2023-07-26 12:05:03.000000 PDKMaster-0.9.4/PDKMaster.egg-info/SOURCES.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-07-26 12:05:02.000000 PDKMaster-0.9.4/PDKMaster.egg-info/dependency_links.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2023-07-26 12:05:02.000000 PDKMaster-0.9.4/PDKMaster.egg-info/requires.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       15 2023-07-26 12:05:02.000000 PDKMaster-0.9.4/PDKMaster.egg-info/top_level.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9871 2023-07-26 12:05:03.104557 PDKMaster-0.9.4/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9403 2023-07-26 12:03:03.000000 PDKMaster-0.9.4/README.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.076557 PDKMaster-0.9.4/ReleaseNotes/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      442 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/ReleaseNotes/v0.1.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1234 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/ReleaseNotes/v0.2.0.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1471 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/ReleaseNotes/v0.3.0.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2547 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/ReleaseNotes/v0.9.0.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.076557 PDKMaster-0.9.4/assura_yaml/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/assura_yaml/.keepme
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      595 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/checkskill.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       14 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/ci-requirements.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/dev-requirements.txt
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.076557 PDKMaster-0.9.4/display_yaml/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/display_yaml/.keepme
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.064557 PDKMaster-0.9.4/docs/
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.080557 PDKMaster-0.9.4/docs/src/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6063 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/conf.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      456 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/index.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      141 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster._util.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      560 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.design.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      443 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.dispatch.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      312 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.io.coriolis.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      462 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.io.klayout.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      934 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.io.parsing.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      318 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.io.pdkmaster.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      262 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.io.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      449 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.io.spice.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      290 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1556 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.technology.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3746 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/dodo.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     4469 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/extract_rules.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    26261 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/files.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.080557 PDKMaster-0.9.4/pdkmaster/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      709 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18133 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/_util.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.080557 PDKMaster-0.9.4/pdkmaster/design/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      237 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6045 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/cell.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10199 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/circuit.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     8637 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/factory.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.084557 PDKMaster-0.9.4/pdkmaster/design/layout/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      664 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/layout/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    28707 2023-07-26 08:56:45.000000 PDKMaster-0.9.4/pdkmaster/design/layout/_circuitlayouter.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    48052 2023-07-26 08:56:45.000000 PDKMaster-0.9.4/pdkmaster/design/layout/_primitivelayouter.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3335 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/layout/factory_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    22622 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/layout/layout_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2887 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/library.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2600 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/routinggauge.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.084557 PDKMaster-0.9.4/pdkmaster/dispatch/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1375 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/dispatch/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1378 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/dispatch/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1956 2023-07-24 14:24:09.000000 PDKMaster-0.9.4/pdkmaster/dispatch/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     8101 2023-07-26 08:56:38.000000 PDKMaster-0.9.4/pdkmaster/dispatch/primitive.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2803 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/dispatch/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3801 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/dispatch/shape.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.084557 PDKMaster-0.9.4/pdkmaster/io/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.084557 PDKMaster-0.9.4/pdkmaster/io/coriolis/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/coriolis/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    58632 2023-07-26 08:24:56.000000 PDKMaster-0.9.4/pdkmaster/io/coriolis/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.084557 PDKMaster-0.9.4/pdkmaster/io/klayout/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      142 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/klayout/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37919 2023-07-26 08:57:55.000000 PDKMaster-0.9.4/pdkmaster/io/klayout/export.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    23519 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/klayout/merge_.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.084557 PDKMaster-0.9.4/pdkmaster/io/lefdef/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      261 2023-07-25 08:57:03.000000 PDKMaster-0.9.4/pdkmaster/io/lefdef/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9948 2023-07-26 08:24:48.000000 PDKMaster-0.9.4/pdkmaster/io/lefdef/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.088557 PDKMaster-0.9.4/pdkmaster/io/notebook/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      121 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/notebook/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1253 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/notebook/plotter.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.088557 PDKMaster-0.9.4/pdkmaster/io/parsing/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      214 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/parsing/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18847 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/parsing/assura.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      422 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/parsing/display.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      822 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/parsing/layermap.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17548 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/parsing/skill_grammar.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24374 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/parsing/tf.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.088557 PDKMaster-0.9.4/pdkmaster/io/pdkmaster/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/pdkmaster/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18067 2023-07-26 08:56:38.000000 PDKMaster-0.9.4/pdkmaster/io/pdkmaster/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.088557 PDKMaster-0.9.4/pdkmaster/io/spice/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      165 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/spice/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    15809 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/spice/pyspice.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     5904 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/spice/spice_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      181 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/spice/typing.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.092557 PDKMaster-0.9.4/pdkmaster/technology/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      276 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4032 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    77846 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/geometry.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18203 2023-07-26 09:02:44.000000 PDKMaster-0.9.4/pdkmaster/technology/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      627 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/net.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.092557 PDKMaster-0.9.4/pdkmaster/technology/primitive/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      466 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/primitive/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10122 2023-07-26 08:56:45.000000 PDKMaster-0.9.4/pdkmaster/technology/primitive/_core.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2421 2023-07-26 08:56:45.000000 PDKMaster-0.9.4/pdkmaster/technology/primitive/_derived.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1176 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/primitive/_param.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24164 2023-07-26 08:57:55.000000 PDKMaster-0.9.4/pdkmaster/technology/primitive/conductors.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    44879 2023-07-26 12:04:52.000000 PDKMaster-0.9.4/pdkmaster/technology/primitive/devices.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4914 2023-07-26 12:04:52.000000 PDKMaster-0.9.4/pdkmaster/technology/primitive/layers.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6752 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/primitive/rules.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9109 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/property_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2138 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    25167 2023-07-26 12:04:52.000000 PDKMaster-0.9.4/pdkmaster/technology/technology_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2246 2023-07-26 12:04:52.000000 PDKMaster-0.9.4/pdkmaster/technology/wafer_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3344 2023-07-26 08:24:56.000000 PDKMaster-0.9.4/pdkmaster/typing.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-07-26 12:05:03.104557 PDKMaster-0.9.4/setup.cfg
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1410 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/setup.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      863 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/skill.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1278 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/skill2yaml.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.096557 PDKMaster-0.9.4/test/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.096557 PDKMaster-0.9.4/test/unit/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7946 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/_util.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.096557 PDKMaster-0.9.4/test/unit/design/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/design/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3025 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/design/cell.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2470 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/design/circuit.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3664 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/design/factory.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37661 2023-07-26 08:56:45.000000 PDKMaster-0.9.4/test/unit/design/layout.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4584 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/design/library.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.100557 PDKMaster-0.9.4/test/unit/dispatch/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/dispatch/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1343 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/dispatch/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1397 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/dispatch/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1752 2023-07-26 08:56:38.000000 PDKMaster-0.9.4/test/unit/dispatch/primitive.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1531 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/dispatch/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3403 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/dispatch/shape.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13201 2023-07-26 08:56:45.000000 PDKMaster-0.9.4/test/unit/dummy.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.100557 PDKMaster-0.9.4/test/unit/io/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.100557 PDKMaster-0.9.4/test/unit/io/klayout/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/klayout/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13480 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/klayout/export.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    20839 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/klayout/merge.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.100557 PDKMaster-0.9.4/test/unit/io/lefdef/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-25 08:57:03.000000 PDKMaster-0.9.4/test/unit/io/lefdef/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1573 2023-07-25 08:57:03.000000 PDKMaster-0.9.4/test/unit/io/lefdef/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.100557 PDKMaster-0.9.4/test/unit/io/pdkmaster/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/pdkmaster/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1862 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/pdkmaster/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.100557 PDKMaster-0.9.4/test/unit/io/spice/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/spice/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7947 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/spice/pyspice.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1317 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/spice/spice_.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.104557 PDKMaster-0.9.4/test/unit/technology/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/technology/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1313 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/technology/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    56025 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/technology/geometry.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6370 2023-07-26 09:02:44.000000 PDKMaster-0.9.4/test/unit/technology/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    53365 2023-07-26 09:02:44.000000 PDKMaster-0.9.4/test/unit/technology/primitive.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2775 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/technology/property.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2072 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/technology/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17585 2023-07-26 12:04:52.000000 PDKMaster-0.9.4/test/unit/technology/technology.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1052 2023-07-26 12:04:52.000000 PDKMaster-0.9.4/test/unit/technology/wafer.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1438 2023-07-26 09:02:44.000000 PDKMaster-0.9.4/test/unit/typing.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      673 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test.tf
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.104557 PDKMaster-0.9.4/tf_yaml/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/tf_yaml/.keepme
```

### Comparing `PDKMaster-0.9.3/.ci/check-dco.py` & `PDKMaster-0.9.4/.ci/check-dco.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/.gitlab-ci.yml` & `PDKMaster-0.9.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/Contributing.md` & `PDKMaster-0.9.4/Contributing.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/LICENSE.md` & `PDKMaster-0.9.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/LICENSES/agpl-3.0.txt` & `PDKMaster-0.9.4/LICENSES/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/LICENSES/apache-2.0.txt` & `PDKMaster-0.9.4/LICENSES/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/LICENSES/cern_ohl_s_v2.txt` & `PDKMaster-0.9.4/LICENSES/cern_ohl_s_v2.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/LICENSES/gpl-2.0.txt` & `PDKMaster-0.9.4/LICENSES/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/PDKMaster.egg-info/PKG-INFO` & `PDKMaster-0.9.4/PDKMaster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDKMaster
-Version: 0.9.3
+Version: 0.9.4
 Summary: ASIC PDK Manager and Design Framework
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: AGPL-3.0-or-later OR GPL-2.0-or-later OR CERN-OHL-S-2.0+ OR Apache-2.0
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/PDKMaster
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/PDKMaster/issues
 Requires-Python: >=3.6
@@ -14,14 +14,18 @@
 # Description
 
 PDK Master is a tool to manage [PDK](https://en.wikipedia.org/wiki/Process_design_kit)s for ASIC design and a framework for designing circuits and layouts in those technologies.
 It is a Python framework under heavy development and with an unstable API.
 
 # Release history
 
+* v0.9.4:
+  * Support for WaferWire without an implant for diode, MOSFET etc.
+  * Roadworks on layer manipulation
+  * API improvements, unification and deprecation
 * v0.9.3:
   * First LEF/DEF support: support exporting tech.lef file
   * Bug fixing
 * v0.9.2: support new namespace in coriolis export
 * v0.9.1: fix coriolis export, primitive type values are not python types.
 * v0.9.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md)
 * v0.3.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.3.0/ReleaseNotes/v0.3.0.md)
```

### Comparing `PDKMaster-0.9.3/PDKMaster.egg-info/SOURCES.txt` & `PDKMaster-0.9.4/PDKMaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/PKG-INFO` & `PDKMaster-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDKMaster
-Version: 0.9.3
+Version: 0.9.4
 Summary: ASIC PDK Manager and Design Framework
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: AGPL-3.0-or-later OR GPL-2.0-or-later OR CERN-OHL-S-2.0+ OR Apache-2.0
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/PDKMaster
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/PDKMaster/issues
 Requires-Python: >=3.6
@@ -14,14 +14,18 @@
 # Description
 
 PDK Master is a tool to manage [PDK](https://en.wikipedia.org/wiki/Process_design_kit)s for ASIC design and a framework for designing circuits and layouts in those technologies.
 It is a Python framework under heavy development and with an unstable API.
 
 # Release history
 
+* v0.9.4:
+  * Support for WaferWire without an implant for diode, MOSFET etc.
+  * Roadworks on layer manipulation
+  * API improvements, unification and deprecation
 * v0.9.3:
   * First LEF/DEF support: support exporting tech.lef file
   * Bug fixing
 * v0.9.2: support new namespace in coriolis export
 * v0.9.1: fix coriolis export, primitive type values are not python types.
 * v0.9.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md)
 * v0.3.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.3.0/ReleaseNotes/v0.3.0.md)
```

### Comparing `PDKMaster-0.9.3/README.md` & `PDKMaster-0.9.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Description
 
 PDK Master is a tool to manage [PDK](https://en.wikipedia.org/wiki/Process_design_kit)s for ASIC design and a framework for designing circuits and layouts in those technologies.
 It is a Python framework under heavy development and with an unstable API.
 
 # Release history
 
+* v0.9.4:
+  * Support for WaferWire without an implant for diode, MOSFET etc.
+  * Roadworks on layer manipulation
+  * API improvements, unification and deprecation
 * v0.9.3:
   * First LEF/DEF support: support exporting tech.lef file
   * Bug fixing
 * v0.9.2: support new namespace in coriolis export
 * v0.9.1: fix coriolis export, primitive type values are not python types.
 * v0.9.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md)
 * v0.3.0: [release notes](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.3.0/ReleaseNotes/v0.3.0.md)
```

### Comparing `PDKMaster-0.9.3/ReleaseNotes/v0.2.0.md` & `PDKMaster-0.9.4/ReleaseNotes/v0.2.0.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/ReleaseNotes/v0.3.0.md` & `PDKMaster-0.9.4/ReleaseNotes/v0.3.0.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/ReleaseNotes/v0.9.0.md` & `PDKMaster-0.9.4/ReleaseNotes/v0.9.0.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/checkskill.py` & `PDKMaster-0.9.4/checkskill.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/docs/src/conf.py` & `PDKMaster-0.9.4/docs/src/conf.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/docs/src/pdkmaster.design.rst` & `PDKMaster-0.9.4/docs/src/pdkmaster.design.rst`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/docs/src/pdkmaster.io.parsing.rst` & `PDKMaster-0.9.4/docs/src/pdkmaster.io.parsing.rst`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/docs/src/pdkmaster.technology.rst` & `PDKMaster-0.9.4/docs/src/pdkmaster.technology.rst`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/dodo.py` & `PDKMaster-0.9.4/dodo.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/extract_rules.py` & `PDKMaster-0.9.4/extract_rules.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/files.py` & `PDKMaster-0.9.4/files.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/__init__.py` & `PDKMaster-0.9.4/pdkmaster/__init__.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/_util.py` & `PDKMaster-0.9.4/pdkmaster/_util.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/design/cell.py` & `PDKMaster-0.9.4/pdkmaster/design/cell.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/design/circuit.py` & `PDKMaster-0.9.4/pdkmaster/design/circuit.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/design/factory.py` & `PDKMaster-0.9.4/pdkmaster/design/factory.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/design/layout/__init__.py` & `PDKMaster-0.9.4/pdkmaster/design/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/design/layout/_circuitlayouter.py` & `PDKMaster-0.9.4/pdkmaster/design/layout/_circuitlayouter.py`

 * *Files 0% similar despite different names*

```diff
@@ -685,15 +685,18 @@
             shape = _geo.Rect.from_rect(rect=shape, right=bottom_right)
             draw = True
         if bottom_top is not None:
             shape = _geo.Rect.from_rect(rect=shape, top=bottom_top)
             draw = True
         if draw:
             kwargs = {}
-            if "bottom_implant" in via_params:
+            if (
+                ("bottom_implant" in via_params)
+                and (via_params["bottom_implant"] is not None)
+            ):
                 kwargs["implant"] = via_params["bottom_implant"]
             if "bottom_implant_enclosure" in via_params:
                 kwargs["implant_enclosure"] = via_params["bottom_implant_enclosure"]
             if "bottom_well" in via_params:
                 kwargs["well"] = via_params["bottom_well"]
                 kwargs["well_net"] = via_params["well_net"]
             l = self.add_wire(wire=bottom, net=net, shape=shape, **kwargs)
```

### Comparing `PDKMaster-0.9.3/pdkmaster/design/layout/_primitivelayouter.py` & `PDKMaster-0.9.4/pdkmaster/design/layout/_primitivelayouter.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,31 +272,23 @@
         super_params.update(marker_params)
 
         return super_params
 
     def WaferWire(self, prim: _prm.WaferWire, **params) -> Dict[str, Any]:
         layparams = []
         ww_params = {}
-        if len(prim.implant) > 1:
-            layparams.extend((
-                _PrimitiveLayoutParam(
-                    primitive=prim, name="implant", choices=prim.implant,
-                ),
-                _EnclosureLayoutParam(
-                    primitive=prim, name="implant_enclosure", allow_none=True,
-                ),
-            ))
-        else:
-            ww_params["implant"] = prim.implant[0]
-            layparams.append(
-                _EnclosureLayoutParam(
-                    primitive=prim, name="implant_enclosure",
-                    default=prim.min_implant_enclosure[0],
-                ),
-            )
+        layparams.extend((
+            _PrimitiveLayoutParam(
+                primitive=prim, name="implant", choices=prim.implant,
+                allow_none=True,
+            ),
+            _EnclosureLayoutParam(
+                primitive=prim, name="implant_enclosure", allow_none=True,
+            ),
+        ))
         if (len(prim.well) > 1) or prim.allow_in_substrate:
             layparams.extend((
                 _PrimitiveLayoutParam(
                     primitive=prim, name="well", allow_none=prim.allow_in_substrate,
                     choices=prim.well
                 ),
                 _EnclosureLayoutParam(
@@ -309,15 +301,15 @@
                 _EnclosureLayoutParam(
                     primitive=prim, name="well_enclosure", default=prim.min_well_enclosure[0],
                 ),
             )
         layparams.append(_NetLayoutParam(
             primitive=prim, name="well_net", allow_none=prim.allow_in_substrate,
         ))
-        if prim.oxide is not None:
+        if prim.oxide:
             layparams.extend((
                 _PrimitiveLayoutParam(
                     primitive=prim, name="oxide", choices=prim.oxide, allow_none=True,
                 ),
                 _EnclosureLayoutParam(
                     primitive=prim, name="oxide_enclosure", allow_none=True,
                 ),
@@ -332,16 +324,14 @@
 
         if (ww_params["well"] is not None) and (ww_params["well_net"] is None):
             raise ValueError("well_net needs to be provided if well is specified")
 
         if ("oxide" in ww_params):
             oxide = ww_params["oxide"]
             if oxide is not None:
-                assert prim.oxide is not None
-                assert prim.min_oxide_enclosure is not None
                 oxide_enclosure = ww_params["oxide_enclosure"]
                 if oxide_enclosure is None:
                     idx = prim.oxide.index(oxide)
                     ww_params["oxide_enclosure"] = prim.min_oxide_enclosure[idx]
 
         super_params = super().WaferWire(prim, **params)
         super_params.update(ww_params)
@@ -392,19 +382,21 @@
                 _NetLayoutParam(primitive=prim, name="well_net", allow_none=True),
                 _EnclosureLayoutParam(
                     primitive=prim, name="bottom_well_enclosure", allow_none=True,
                 ),
             ))
 
         choices = sum(
-            (cast(Tuple[_prm.Insulator, ...], cast(_prm.WaferWire, wire).oxide)
-            for wire in filter(
-                lambda w: isinstance(w, _prm.WaferWire) and (w.oxide is not None),
-                prim.bottom,
-            )),
+            (
+                cast(_prm.WaferWire, wire).oxide
+                for wire in filter(
+                    lambda w: isinstance(w, _prm.WaferWire),
+                    prim.bottom,
+                )
+            ),
             tuple(),
         )
         if choices:
             layparams.extend((
                 _PrimitiveLayoutParam(
                     primitive=prim, name="bottom_oxide", allow_none=True, choices=choices,
                 ),
@@ -434,22 +426,23 @@
         bottom_impl = get_via_param("bottom_implant")
         bottom_impl_enc = get_via_param("bottom_implant_enclosure")
         bottom_well = get_via_param("bottom_well")
         well_net = get_via_param("well_net")
         bottom_well_enc = get_via_param("bottom_well_enclosure")
         if isinstance(bottom, _prm.WaferWire):
             if bottom_impl is None:
-                raise TypeError(
-                    "bottom_implant parameter not provided for "
-                    f"bottom '{bottom.name}' of via '{prim.name}'"
-                )
-
-            if bottom_impl_enc is None:
-                idx = bottom.implant.index(bottom_impl)
-                via_params["bottom_implant_enclosure"] = bottom.min_implant_enclosure[idx]
+                if bottom_impl_enc is not None:
+                    raise TypeError(
+                        "bottom_implant_enclosure provided for bottom "
+                        f"'{bottom.name}' of via {prim.name} without a bottom_implant"
+                    )
+            else:
+                if bottom_impl_enc is None:
+                    idx = bottom.implant.index(bottom_impl)
+                    via_params["bottom_implant_enclosure"] = bottom.min_implant_enclosure[idx]
 
             if bottom_well is not None:
                 if bottom_well not in bottom.well:
                     raise ValueError(
                         f"bottom_well '{bottom_well.name}' not a valid well for "
                         f"bottom wire '{bottom.name}'"
                     )
@@ -505,41 +498,41 @@
 
         super_params = super().MIMCapacitor(prim, **params)
         super_params.update(mim_params)
 
         return super_params
 
     def MOSFET(self, prim: _prm.MOSFET, **params) -> Dict[str, Any]:
+        impl_act_enc = None
         for impl in prim.implant:
             try:
                 idx = prim.gate.active.implant.index(impl)
             except: # pragma: no cover
                 continue
             else:
                 impl_act_enc = prim.gate.active.min_implant_enclosure[idx]
                 break
-        else: # pragma: no cover
-            raise AssertionError("Internal error: no default active implant enclosure")
 
         layparams = [
-            _EnclosureLayoutParam(
-                primitive=prim, name="activeimplant_enclosure",
-                default=impl_act_enc,
-            ),
             _LayoutParam(
                 primitive=prim, name="sd_width", default=prim.computed.min_sd_width),
             _LayoutParam(
                 primitive=prim, name="polyactive_extension",
                 default=prim.computed.min_polyactive_extension,
             ),
             _EnclosuresLayoutParam(
                 primitive=prim, name="gateimplant_enclosures", n=len(prim.implant),
                 default=prim.min_gateimplant_enclosure,
             ),
         ]
+        if impl_act_enc is not None:
+            layparams.append(_EnclosureLayoutParam(
+                primitive=prim, name="activeimplant_enclosure",
+                default=impl_act_enc,
+            ))
         spc = prim.computed.min_gate_space
         if spc is not None:
             layparams.append(
                 _LayoutParam(primitive=prim, name="gate_space", default=spc)
             )
 
         if prim.computed.contact is not None:
@@ -634,27 +627,28 @@
 
     def WaferWire(self, prim: _prm.WaferWire, **waferwire_params) -> LayoutT:
         width = waferwire_params["width"]
         height = waferwire_params["height"]
 
         implant = waferwire_params.pop("implant")
         implant_enclosure = waferwire_params.pop("implant_enclosure")
-        assert implant_enclosure is not None
+        assert (implant is None) or (implant_enclosure is not None)
 
         well = waferwire_params.pop("well", None)
         well_enclosure = waferwire_params.pop("well_enclosure", None)
 
         oxide = waferwire_params.pop("oxide", None)
         oxide_enclosure = waferwire_params.pop("oxide_enclosure", None)
 
         layout = self._WidthSpaceConductor(prim, **waferwire_params)
-        layout.add_shape(layer=implant, net=None, shape=_rect(
-            -0.5*width, -0.5*height, 0.5*width, 0.5*height,
-            enclosure=implant_enclosure,
-        ))
+        if (implant is not None):
+            layout.add_shape(layer=implant, net=None, shape=_rect(
+                -0.5*width, -0.5*height, 0.5*width, 0.5*height,
+                enclosure=implant_enclosure,
+            ))
         if well is not None:
             well_net = waferwire_params["well_net"]
             assert well_net is not None, "Internal error"
             layout.add_shape(layer=well, net=well_net, shape=_rect(
                 -0.5*width, -0.5*height, 0.5*width, 0.5*height,
                 enclosure=well_enclosure,
             ))
@@ -833,18 +827,15 @@
                 ))
         try:
             oxide = via_params["bottom_oxide"]
         except KeyError:
             oxide = None
         else:
             if oxide is not None:
-                assert (
-                    isinstance(bottom, _prm.WaferWire) and (bottom.oxide is not None)
-                    and (bottom.min_oxide_enclosure is not None)
-                )
+                assert isinstance(bottom, _prm.WaferWire)
                 enc = cast(_prp.Enclosure, via_params["bottom_oxide_enclosure"])
                 if enc is None:
                     idx = bottom.oxide.index(oxide)
                     enc = bottom.min_oxide_enclosure[idx]
                 assert (enc is not None), "Unknown enclosure"
                 layout.add_shape(layer=oxide, net=None, shape=_geo.Rect.from_rect(
                     rect=bottom_rect, bias=enc,
@@ -1137,15 +1128,14 @@
             layout += self(ind, width=(act_width + 2*enc), height=(act_height + 2*enc))
 
         return layout
 
     def MOSFET(self, prim: _prm.MOSFET, **mos_params) -> LayoutT:
         l = mos_params["l"]
         w = mos_params["w"]
-        impl_enc = mos_params["activeimplant_enclosure"]
         gate_encs = mos_params["gateimplant_enclosures"]
         sdw = mos_params["sd_width"]
 
         try:
             portnets = cast(Mapping[str, _net.NetT], mos_params["portnets"])
         except KeyError:
             portnets = prim.ports
@@ -1181,20 +1171,22 @@
                 ),
             )
         )
         layout.add_shape(layer=active, net=portnets["sourcedrain1"], shape=mps.parts[0])
         layout.add_shape(layer=active, net=portnets["bulk"], shape=mps.parts[1])
         layout.add_shape(layer=active, net=portnets["sourcedrain2"], shape=mps.parts[2])
 
-        for impl in prim.implant:
-            if impl in active.implant:
-                layout.add_shape(layer=impl, net=None, shape=_rect(
-                    active_left, active_bottom, active_right, active_top,
-                    enclosure=impl_enc
-                ))
+        if len(prim.implant) > 0:
+            impl_enc = mos_params["activeimplant_enclosure"]
+            for impl in prim.implant:
+                if impl in active.implant:
+                    layout.add_shape(layer=impl, net=None, shape=_rect(
+                        active_left, active_bottom, active_right, active_top,
+                        enclosure=impl_enc
+                    ))
 
         poly = prim.gate.poly
         ext = prim.computed.min_polyactive_extension
         poly_left = gate_left
         poly_bottom = gate_bottom - ext
         poly_right = gate_right
         poly_top = gate_top + ext
@@ -1206,15 +1198,14 @@
             enc = active.min_well_enclosure[active.well.index(prim.well)]
             layout.add_shape(layer=prim.well, net=portnets["bulk"], shape=_rect(
                 active_left, active_bottom, active_right, active_top, enclosure=enc,
             ))
 
         oxide = prim.gate.oxide
         if oxide is not None:
-            assert (active.oxide is not None) and (active.min_oxide_enclosure is not None)
             enc = getattr(
                 prim.gate, "min_gateoxide_enclosure", _prp.Enclosure(self.tech.grid),
             )
             layout.add_shape(layer=oxide, net=None, shape=_rect(
                 gate_left, gate_bottom, gate_right, gate_top, enclosure=enc,
             ))
             idx = active.oxide.index(oxide)
```

### Comparing `PDKMaster-0.9.3/pdkmaster/design/layout/factory_.py` & `PDKMaster-0.9.4/pdkmaster/design/layout/factory_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/design/layout/layout_.py` & `PDKMaster-0.9.4/pdkmaster/design/layout/layout_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/design/library.py` & `PDKMaster-0.9.4/pdkmaster/design/library.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/design/routinggauge.py` & `PDKMaster-0.9.4/pdkmaster/design/routinggauge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/dispatch/__init__.py` & `PDKMaster-0.9.4/pdkmaster/dispatch/__init__.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/dispatch/edge.py` & `PDKMaster-0.9.4/pdkmaster/dispatch/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/dispatch/mask.py` & `PDKMaster-0.9.4/pdkmaster/dispatch/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/dispatch/primitive.py` & `PDKMaster-0.9.4/pdkmaster/dispatch/primitive.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,18 +56,36 @@
         prim: _prm.WidthSpaceDesignMaskPrimitiveT, *args, **kwargs,
     ):
         # _DesignMaskPrimitive is handled by _WidthSpacePrimitive() if needed.
         return self._WidthSpacePrimitive(prim, *args, **kwargs)
 
     ### primitive._derived
 
-    def _DerivedPrimitive(self, prim: _prm.DerivedPrimitiveT, *args, **kwargs):
+    def _DerivedPrimitive(self, prim: _prm._derived._DerivedPrimitive, *args, **kwargs):
+        """
+        API Notes:
+            * No backwards compatiblity is provided for overloading this function
+              in user land code. _DerivedPrimitive is considered for internal use only.
+        """
         return self._MaskPrimitive(prim, *args, **kwargs)
 
-    def _Intersect(self, prim: _prm.IntersectT, *args, **kwargs):
+    def _Intersect(self, prim: _prm._derived._Intersect, *args, **kwargs):
+        """
+        API Notes:
+            * No backwards compatiblity is provided for overloading this function
+              in user land code. _Intersect is considered for internal use only.
+        """
+        return self._DerivedPrimitive(prim, *args, **kwargs)
+
+    def _Outside(self, prim: _prm._derived._Outside, * args, **kwargs):
+        """
+        API Notes:
+            * No backwards compatiblity is provided for overloading this function
+              in user land code. _Outside is considered for internal use only.
+        """
         return self._DerivedPrimitive(prim, *args, **kwargs)
 
     ### primitive.layers
 
     def Base(self, prim: _prm.Base, *args, **kwargs):
         return self._MaskPrimitive(prim, *args, **kwargs)
```

### Comparing `PDKMaster-0.9.3/pdkmaster/dispatch/rule.py` & `PDKMaster-0.9.4/pdkmaster/dispatch/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/dispatch/shape.py` & `PDKMaster-0.9.4/pdkmaster/dispatch/shape.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/io/coriolis/export.py` & `PDKMaster-0.9.4/pdkmaster/io/coriolis/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,15 +490,15 @@
 
     def __call__(self, lib: _lbry.Library, *, routinggauge: Optional[_rg.RoutingGauge]):
         def otherdir(dir_):
             return "vertical" if dir_ == "horizontal" else "horizontal"
 
         if isinstance(lib, _lbry.RoutingGaugeLibrary):
             assert routinggauge is None
-            routinggauge = lib.routinggauge[0]
+            routinggauge = next(iter(lib._routinggauge))
 
         if routinggauge is not None:
             bottom_idx = self.metals.index(routinggauge.bottom)
             bottom_dir = routinggauge.bottom_direction
             self.metalsdir = tuple(
                 None if i < (bottom_idx - 1)
                 else bottom_dir if ((i - bottom_idx)%2) == 0
```

### Comparing `PDKMaster-0.9.3/pdkmaster/io/klayout/export.py` & `PDKMaster-0.9.4/pdkmaster/io/klayout/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
 
     is_n = diode.implant.type_ == _prm.nImpl
 
     s_diode = _mask_conv(diode.mask)
     s_conn = _mask_conv(diode.wire.conn_mask)
     s_well = _mask_conv(
         diode.well.mask if diode.well is not None
-        else tech.substrate
+        else tech.substrate_prim.mask
     )
 
     if is_n:
         s_p = s_well
         s_n = s_diode
         s_conn_port = "tC"
     else:
@@ -348,18 +348,18 @@
     return s
 
 
 def _str_lvsmosfet(tech: _tch.Technology, mosfet: _prm.MOSFET, spice_params: SpicePrimParamsT):
     s = f"# {mosfet.name}\n"
 
     s_sd = _mask_conv(mosfet.gate.active.conn_mask)
-    s_gate = _mask_conv(mosfet.gate_mask)
+    s_gate = _mask_conv(mosfet.gate4mosfet.mask)
     s_bulk = _mask_conv(
         mosfet.well.mask if mosfet.well is not None
-        else tech.substrate
+        else tech.substrate_prim.mask
     )
     s_poly = _mask_conv(mosfet.gate.poly.conn_mask)
 
     s += dedent(f"""
         extract_devices(mos4("{spice_params['model']}"), {{
             "SD" => {s_sd}, "G" => {s_gate}, "tG" => {s_poly}, "W" => {s_bulk},
         }})
```

### Comparing `PDKMaster-0.9.3/pdkmaster/io/klayout/merge_.py` & `PDKMaster-0.9.4/pdkmaster/io/klayout/merge_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/io/lefdef/export.py` & `PDKMaster-0.9.4/pdkmaster/io/lefdef/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,27 +155,27 @@
             END UNITS
             MANUFACTURINGGRID {self.tech.grid:.5f} ;
         """)
 
         if self.use_nwell:
             nwell_name = "nwell"
             for well in self.tech.primitives.__iter_type__(prm.Well):
-                if well.type_ == prm.nImplT:
+                if well.type_ == prm.nImpl:
                     nwell_name = well.name
                     break
             tlef_string += dedent(f"""
                 LAYER {nwell_name}
                     TYPE MASTERSLICE ;
                     PROPERTY LEF58_TYPE "TYPE NWELL ;" ;
                 END {nwell_name}
             """)
         if self.use_pwell:
             pwell_name = "pwell"
             for well in self.tech.primitives.__iter_type__(prm.Well):
-                if well.type_ == prm.pImplT:
+                if well.type_ == prm.pImpl:
                     pwell_name = well.name
                     break
             tlef_string += dedent(f"""
                 LAYER {pwell_name}
                     TYPE MASTERSLICE ;
                     PROPERTY LEF58_TYPE "TYPE PWELL ;" ;
                 END {pwell_name}
```

### Comparing `PDKMaster-0.9.3/pdkmaster/io/notebook/plotter.py` & `PDKMaster-0.9.4/pdkmaster/io/notebook/plotter.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/io/parsing/assura.py` & `PDKMaster-0.9.4/pdkmaster/io/parsing/assura.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/io/parsing/layermap.py` & `PDKMaster-0.9.4/pdkmaster/io/parsing/layermap.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/io/parsing/skill_grammar.py` & `PDKMaster-0.9.4/pdkmaster/io/parsing/skill_grammar.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/io/parsing/tf.py` & `PDKMaster-0.9.4/pdkmaster/io/parsing/tf.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/io/pdkmaster/export.py` & `PDKMaster-0.9.4/pdkmaster/io/pdkmaster/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         s += "min_well_enclosure="+_str_enclosures(prim.min_well_enclosure)+",\n"
         if prim.min_substrate_enclosure is not None:
             s += (
                 "min_substrate_enclosure="
                 f"{_str_enclosure(prim.min_substrate_enclosure)},\n"
             )
         s += f"allow_well_crossing={prim.allow_well_crossing},\n"
-        if prim.oxide is not None:
+        if prim.oxide:
             assert prim.min_oxide_enclosure is not None
             s += (
                 f"oxide={_str_primtuple(prim.oxide)},\n"
                 f"min_oxide_enclosure={_str_enclosures(prim.min_oxide_enclosure)},\n"
             )
         s += self._params_widthspacedesignmask(prim)
         return s
```

### Comparing `PDKMaster-0.9.3/pdkmaster/io/spice/pyspice.py` & `PDKMaster-0.9.4/pdkmaster/io/spice/pyspice.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/io/spice/spice_.py` & `PDKMaster-0.9.4/pdkmaster/io/spice/spice_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/technology/edge.py` & `PDKMaster-0.9.4/pdkmaster/technology/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/technology/geometry.py` & `PDKMaster-0.9.4/pdkmaster/technology/geometry.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/technology/mask.py` & `PDKMaster-0.9.4/pdkmaster/technology/mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,19 +172,26 @@
         The condition may only use properties from the same mask on which one
         calls the `parts_with` method.
 
         Example: `small = mask.parts_with(mask.width <= 1.0)`
         """
         return _PartsWith(mask=self, condition=condition)
 
-    def remove(self, what: "MaskT") -> "MaskT":
+    def remove(self, what: MultiT["MaskT"], *args: "MaskT") -> "MaskT":
         """Returns a derived `MaskT` representing the parts of the shapes on
         the `MaskT` that don't overlap with shapes of the other `MaskT` object.
         """
-        return _MaskRemove(from_=self, what=what)
+        what = (*cast_MultiT(what), *args)
+        if len(what) == 0:
+            raise ValueError("No mask given")
+        elif len(what) == 1:
+            mask = what[0]
+        else:
+            mask = Join(what)
+        return _MaskRemove(from_=self, what=mask)
 
     def alias(self, name: str) -> "RuleMaskT":
         """Returns a derived `MaskT` given an alias for another `MaskT` object.
         The return object is also a `_Rule` object in order for scripts that
         are generated from rules can define a variable representing the
         `MaskT` that has been aliased. Typically the variable name will be
         the alias name and further on in generated rules then this variable
@@ -308,16 +315,16 @@
         return super().__hash__()
 
 
 class Join(_Mask):
     """A derived `_Mask` object that represenet the shapes resulting of joining
     all the shapes of the provided masks.
     """
-    def __init__(self, masks: MultiT[MaskT]):
-        self.masks = masks = cast_MultiT(masks)
+    def __init__(self, masks: MultiT[MaskT], *args: MaskT):
+        self.masks = masks = (*cast_MultiT(masks), *args)
 
         super().__init__(name="join({})".format(",".join(mask.name for mask in masks)))
 
         self._hash: Optional[int] = None
 
     @property
     def designmasks(self) -> Iterable[DesignMask]:
```

### Comparing `PDKMaster-0.9.3/pdkmaster/technology/net.py` & `PDKMaster-0.9.4/pdkmaster/technology/net.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/technology/primitive/_core.py` & `PDKMaster-0.9.4/pdkmaster/technology/primitive/_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,14 +111,23 @@
 
         if gen_mask and isinstance(self.mask, _rle.RuleT):
             yield cast(_rle.RuleT, self.mask)
 
     @property
     def designmasks(self):
         return self.mask.designmasks
+
+    def remove(self, what: MultiT["MaskPrimitiveT"], *args: "MaskPrimitiveT") -> "MaskPrimitiveT":
+        """Return a MaskPrimitive based on the MaskPrimitive but with
+        the overlapping parts with another MaskPrimitive removed.
+        """
+        return _drv._Outside(prim=self, where=(*cast_MultiT(what), *args))
+
+    def alias(self, alias: str) -> "MaskPrimitiveT":
+        return _drv._Alias(prim=self, alias=alias)
 MaskPrimitiveT = _MaskPrimitive
 
 
 class Primitives(_util.ExtendedListStrMapping[_Primitive]):
     """A collection of `_Primitive` objects"""
     def __iadd__(self, x: MultiT[_Primitive]) -> "Primitives":
         from ._derived import _DerivedPrimitive
@@ -284,7 +293,10 @@
 class UnconnectedPrimitiveError(Exception):
     """Exception used by `Technology` when checking the primitives list
     of a technology"""
     def __init__(self, *, primitive: _Primitive):
         super().__init__(
             f"primitive '{primitive.name}' is not connected"
         )
+
+
+from . import _derived as _drv
```

### Comparing `PDKMaster-0.9.3/pdkmaster/technology/primitive/_param.py` & `PDKMaster-0.9.4/pdkmaster/technology/primitive/_param.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/technology/primitive/conductors.py` & `PDKMaster-0.9.4/pdkmaster/technology/primitive/conductors.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     MultiT, cast_MultiT, cast_MultiT_n,
     OptMultiT, cast_OptMultiT_n,
 )
 from .. import (
     property_ as _prp, rule as _rle, mask as _msk, edge as _edg, technology_ as _tch,
 )
 
-from . import MaskPrimitiveT, IntersectT
+from . import MaskPrimitiveT
 from ._core import (
-    _Primitive, _PrimitiveNet, _DesignMaskPrimitive, _WidthSpacePrimitive,
+    _Primitive, _PrimitiveNet, _DesignMaskPrimitive, _WidthSpaceDesignMaskPrimitive,
     UnconnectedPrimitiveError,
 )
 from ._derived import _Intersect
 from .layers import Marker, Insulator, Implant
 
 
 __all__ = [
@@ -99,15 +99,15 @@
             self.conn_mask = self.mask.remove(remmask).alias(self.mask.name + "__conn")
             yield self.conn_mask
         else:
             self.conn_mask = self.mask
 ConductorT = _Conductor
 
 
-class _WidthSpaceConductor(_Conductor, _WidthSpacePrimitive):
+class _WidthSpaceConductor(_Conductor, _WidthSpaceDesignMaskPrimitive):
     """_WidthSpacePrimitive that is also a _Conductor"""
     pass
 WidthSpaceConductorT = _WidthSpaceConductor
 
 
 class Well(_WidthSpaceConductor, Implant):
     """Well is an Implant layer that has deeper implant so it forms a
@@ -229,15 +229,15 @@
         allow_in_substrate: bool,
         well: MultiT[Well],
         min_well_enclosure: MultiT[_prp.Enclosure],
         min_well_enclosure_same_type: OptMultiT[Optional[_prp.Enclosure]]=None,
         min_substrate_enclosure: Optional[_prp.Enclosure]=None,
         min_substrate_enclosure_same_type: Optional[_prp.Enclosure]=None,
         allow_well_crossing: bool,
-        oxide: OptMultiT[Insulator]=None,
+        oxide: MultiT[Insulator]=(),
         min_oxide_enclosure: MultiT[Optional[_prp.Enclosure]]=None,
         **super_args
     ):
         self.allow_in_substrate = allow_in_substrate
 
         self.implant = implant = cast_MultiT(implant)
         for impl in implant:
@@ -262,17 +262,14 @@
                 raise ValueError(
                     f"implant_abut member '{impl.name}' not in implant list"
                 )
         self.implant_abut = implant_abut
         self.allow_contactless_implant = allow_contactless_implant
 
         self.well = well = cast_MultiT(well)
-        for w in well:
-            if not any(impl.type_ == w.type_ for impl in implant):
-                raise UnconnectedPrimitiveError(primitive=well[0])
         self.min_well_enclosure = min_well_enclosure = cast_MultiT_n(
             min_well_enclosure, n=len(well),
         )
         self.min_well_enclosure_same_type = cast_OptMultiT_n(
             min_well_enclosure_same_type, n=len(well),
         )
         if allow_in_substrate:
@@ -297,39 +294,40 @@
                 "min_substrate_enclosure has to be 'None' if allow_in_substrate "
                 "is 'False'"
             )
         self.allow_well_crossing = allow_well_crossing
         self.min_substrate_enclosure = min_substrate_enclosure
         self.min_substrate_enclosure_same_type = min_substrate_enclosure_same_type
 
-        if oxide is not None:
-            oxide = cast_MultiT(oxide)
-            min_oxide_enclosure = cast_MultiT_n(min_oxide_enclosure, n=len(oxide))
-        elif min_oxide_enclosure is not None:
-            raise ValueError("min_oxide_enclosure provided with no oxide given")
+        oxide = cast_MultiT(oxide)
+        if (len(oxide) == 0) and (min_oxide_enclosure is None):
+            min_oxide_enclosure = ()
+        min_oxide_enclosure = cast_MultiT_n(min_oxide_enclosure, n=len(oxide))
         self.oxide = oxide
         self.min_oxide_enclosure = min_oxide_enclosure
 
         super().__init__(**super_args)
 
     def _generate_rules(self, *,
         tech: _tch.Technology,
     ) -> Iterable[_rle.RuleT]:
         yield from super()._generate_rules(tech=tech)
 
+        substrate_mask = tech.substrate_prim.mask
+
         for i, impl in enumerate(self.implant):
             sd_mask_impl = _msk.Intersect((self.conn_mask, impl.mask)).alias(
                 f"{self.conn_mask.name}:{impl.name}",
             )
             yield from (sd_mask_impl, _msk.Connect(self.conn_mask, sd_mask_impl))
             if (
                 self.allow_in_substrate
                 and (impl.type_.value == tech.base.type_.value)
             ):
-                yield _msk.Connect(sd_mask_impl, tech.substrate)
+                yield _msk.Connect(sd_mask_impl, substrate_mask)
             if impl not in self.implant_abut:
                 yield _edg.MaskEdge(impl.mask).interact_with(self.mask).length == 0
             enc = self.min_implant_enclosure[i]
             yield self.mask.enclosed_by(impl.mask) >= enc
             for w in self.well:
                 if impl.type_ == w.type_:
                     yield _msk.Connect(sd_mask_impl, w.mask)
@@ -372,81 +370,75 @@
                         )
                     ):
                         yield ww.mask.enclosed_by(w.mask) >= enc2
 
         if self.min_substrate_enclosure is not None:
             if self.min_substrate_enclosure_same_type is None:
                 yield (
-                    self.mask.enclosed_by(tech.substrate)
+                    self.mask.enclosed_by(substrate_mask)
                     >= self.min_substrate_enclosure
                 )
             else:
                 for ww in (
                     cast("_WaferWireIntersect", self.in_(impl)) for impl in filter(
                     # other type
                     lambda impl2: tech.base.type_.value != impl2.type_.value,
                     self.implant,
                 )):
                     yield (
-                        ww.mask.enclosed_by(tech.substrate)
+                        ww.mask.enclosed_by(substrate_mask)
                         >= self.min_substrate_enclosure
                     )
                 for ww in (
                     cast("_WaferWireIntersect", self.in_(impl)) for impl in filter(
                     # same type
                     lambda impl2: tech.base.type_.value == impl2.type_.value,
                     self.implant,
                 )):
                     yield (
-                        ww.mask.enclosed_by(tech.substrate)
+                        ww.mask.enclosed_by(substrate_mask)
                         >= self.min_substrate_enclosure_same_type
                     )
 
-        if self.oxide is not None:
-            assert self.min_oxide_enclosure is not None
-            for i, ox in enumerate(self.oxide):
-                enc = self.min_oxide_enclosure[i]
-                if enc is not None:
-                    yield self.mask.enclosed_by(ox.mask) >= enc
+        for i, ox in enumerate(self.oxide):
+            enc = self.min_oxide_enclosure[i]
+            if enc is not None:
+                yield self.mask.enclosed_by(ox.mask) >= enc
 
         if not self.allow_well_crossing:
             mask_edge = _edg.MaskEdge(self.mask)
             yield from (
                 mask_edge.interact_with(_edg.MaskEdge(w.mask)).length == 0
                 for w in self.well
             )
 
-    def in_(self, prim: MultiT[MaskPrimitiveT]) -> IntersectT:
+    def in_(self, prim: MultiT[MaskPrimitiveT]) -> MaskPrimitiveT:
         return _WaferWireIntersect(waferwire=self, prim=prim)
 
 
 class _WaferWireIntersect(_Intersect):
     """Intersect of WaferWire with one or more of it's implants, wells and
     oxides"""
     def __init__(self, *,
         waferwire: WaferWire, prim: MultiT[MaskPrimitiveT],
     ):
         ww_prims: Set[MaskPrimitiveT] = set(waferwire.implant)
-        if waferwire.well is not None:
-            ww_prims.update(waferwire.well)
-        if waferwire.oxide is not None:
-            ww_prims.update(waferwire.oxide)
+        ww_prims.update(waferwire.well)
+        ww_prims.update(waferwire.oxide)
         prim = cast_MultiT(prim)
         for p in prim:
             if p not in ww_prims:
                 raise ValueError(
                     f"prim '{p.name}' not an implant, well or oxide layer for"
                     f" WaferWire '{waferwire.name}'"
                 )
         self.waferwire = waferwire
         self.prim = prim
 
         super().__init__(prims=(waferwire, *prim))
-# No WaferWireIntersectT is defined as _WaferWireIntersect is only there for type
-# checking and user land only needs IntersectT
 
 
 class GateWire(_WidthSpaceConductor):
     """GateWire is a _WidthSpaceConductor that can act as the
     gate of a MOSFET.
 
     No extra arguments next to the `_WidthSpacePrimitive` and `_DesignMaskPrimitive`
@@ -549,15 +541,15 @@
 
     @property
     def designmasks(self):
         yield from super().designmasks
         for conn in self.bottom + self.top:
             yield from conn.designmasks
 
-    def in_(self, prim: MultiT[MaskPrimitiveT]) -> IntersectT:
+    def in_(self, prim: MultiT[MaskPrimitiveT]) -> MaskPrimitiveT:
         return _ViaIntersect(via=self, prim=prim)
 
 
 class _ViaIntersect(_Intersect):
     """Intersect of WaferWire with one or more of it's implants, wells and
     oxides"""
     def __init__(self, *,
@@ -572,16 +564,14 @@
                 raise ValueError(
                     f"prim '{p.name}' not a bottom or top layer for Via '{via.name}'"
                 )
         self.via = via
         self.prin = prim
 
         super().__init__(prims=(via, *prim))
-# No ViaIntersectT is defined as _ViaIntersect is only there for type
-# checking and user land only needs IntersectT
 
 
 class PadOpening(_WidthSpaceConductor):
     """PadOpening is a layer representing an opening in the top layer in the
     processing of a semiconductor wafer.
 
     Typical application is for wirebonding, bumping for flip-chip or an RDL
```

### Comparing `PDKMaster-0.9.3/pdkmaster/technology/primitive/devices.py` & `PDKMaster-0.9.4/pdkmaster/technology/primitive/devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 
 from .. import (
     property_ as _prp, rule as _rle, geometry as _geo,
     mask as _msk, edge as _edg, wafer_ as _wfr, technology_ as _tch,
 )
 
 from ._core import (
-    _Primitive, _PrimitiveNet, _MaskPrimitive, _WidthSpacePrimitive,
+    _Primitive, _PrimitiveNet, _MaskPrimitive, MaskPrimitiveT,
+    _WidthSpacePrimitive,
 )
 from ._param import _PrimParam
-from ._derived import _Intersect
+from ._derived import _Intersect, _Alias
 from .layers import Marker, ExtraProcess, Insulator, Implant, adjImpl
 from .conductors import Well,  WaferWire, GateWire, MetalWire, MIMTop, Via
 
 
 __all__ = [
     "DevicePrimitiveT", "DeviceParamT", "DeviceParamsT",
     "ResistorWireT", "ResistorIndicatorT", "Resistor",
@@ -566,15 +567,15 @@
         min_contactgate_space: Optional[float]=None,
     ):
         self.active = active
         self.poly = poly
 
         prims = (poly, active)
         if oxide is not None:
-            if (active.oxide is None) or (oxide not in active.oxide):
+            if oxide not in active.oxide:
                 raise ValueError(
                     f"oxide '{oxide.name}' is not valid for active '{active.name}'"
                 )
             prims += (oxide,)
         elif min_gateoxide_enclosure is not None:
             raise TypeError("min_gateoxide_enclosure provided without an oxide")
         self.oxide = oxide
@@ -676,15 +677,15 @@
                 extra_masks += tuple(inside.mask for inside in cast(Any, gate).inside)
         masks = (active_mask, poly_mask)
         if self.oxide is not None:
             masks += (self.oxide.mask,)
         if self.inside is not None:
             masks += tuple(inside.mask for inside in self.inside)
         if extra_masks:
-            masks += (_wfr.outside(extra_masks),)
+            masks += (_wfr.wafer.remove(extra_masks),)
         # Keep the alias but change the mask of the alias
         cast(_msk._MaskAlias, self.mask).mask = _msk.Intersect(masks)
         mask = self.mask
 
         mask_used = False
         rules: List[_rle.RuleT] = []
         if self.min_l is not None:
@@ -730,14 +731,18 @@
     MOS stands for metal-oxide-semiconductor; see
     https://en.wikipedia.org/wiki/MOSFET for explanation of a MOSFET device.
 
     Arguments:
         name: name for the gate.
         gate: the `MOSFETGate` object for this device
         implant: implant layers for this device
+            If no n or p type implant is given for the MOSFET the type of the
+            is considered the opposite of the well/substrate the device is in.
+            It is not allowed to have mosfets with and without n/p type implants
+            in the same well or in the substrate.
         well: optional well in which this MOSFET needs to be located.
             If gate.active can't be put in substrate well has to be
             specified. If specified the well has to be valid for
             gate.active and the implant type has to be opposite to the
             implant types.
         min_l: optional minimum l specification for the MOSFET device
             If not specified the min_l of the gate will be used, which
@@ -849,18 +854,14 @@
             if impl.type_ != adjImpl:
                 if type_ is None:
                     type_ = impl.type_
                 elif type_ != impl.type_:
                     raise ValueError(
                         "both n and p type implants for same MOSFET are not allowed"
                     )
-        if type_ is None:
-            raise ValueError(
-                "at least one n or p type implant has to be specified"
-            )
         wrong = tuple(filter(
             lambda impl: impl not in gate.active.implant,
             implant
         ))
         if wrong:
             names = tuple(impl.name for impl in wrong)
             raise ValueError(
@@ -942,81 +943,92 @@
 
         self.params += (
             _DeviceParam(primitive=self, name="l", default=self.computed.min_l),
             _DeviceParam(primitive=self, name="w", default=self.computed.min_w),
         )
 
     @property
-    def gate_prim(self) -> _Intersect:
+    def has_typeimplant(self) -> bool:
+        return any(impl.type_ != adjImpl for impl in self.implant)
+    @property
+    def gate4mosfet(self) -> MaskPrimitiveT:
         """gate_prim attribute is the primitive representing the gate of the MOSFET
         object. Main reason it exists is to use it in rules; for example a minimum spacing
         to the gate of a transistor.
         """
-        prims: Tuple[_MaskPrimitive, ...] = (self.gate, *self.implant)
-        if self.well is not None:
-            prims += (self.well,)
-
-        return _Intersect(prims=prims)
-
+        if not hasattr(self, "_gate4mosfet"):
+            raise TypeError(
+                "gate4mosfet attribute may not be accessed before the MOSFET is added"
+                " to a technology"
+            )
+        return self._gate4mosfet
+    # Backwards compatibility
+    gate_prim = gate4mosfet
     @property
-    def gate_mask(self):
-        return self._gate_mask
+    def gate_mask(self) -> _msk.MaskT:
+        """
+        API Notes:
+            * Deprecated property; will be removed for V1.0; use gate4mosfet.mask
+        """
+        return self.gate4mosfet.mask
 
     def _generate_rules(self, *,
         tech: _tch.Technology,
     ) -> Iterable[_rle.RuleT]:
         yield from super()._generate_rules(tech=tech)
 
-        markers = (self.well.mask if self.well is not None else tech.substrate,)
-        if self.implant is not None:
-            markers += tuple(impl.mask for impl in self.implant)
-        derivedgate_mask = _msk.Intersect((self.gate.mask, *markers)).alias(
-            f"gate:mosfet:{self.name}",
+        markers = (
+            self.well if self.well is not None else tech.substrate_prim,
+            *self.implant,
+        )
+        derivedgate = cast(
+            _Alias,
+            _Intersect(prims=(self.gate, *markers)).alias(f"gate:mosfet:{self.name}"),
         )
-        self._gate_mask = derivedgate_mask
-        derivedgate_edge = _edg.MaskEdge(derivedgate_mask)
+        self._gate4mosfet = derivedgate
+        derivedgate_edge = _edg.MaskEdge(derivedgate.mask)
         poly_mask = self.gate.poly.mask
         poly_edge = _edg.MaskEdge(poly_mask)
         channel_edge = _edg.Intersect((derivedgate_edge, poly_edge))
         active_mask = self.gate.active.mask
         active_edge = _edg.MaskEdge(active_mask)
         fieldgate_edge = _edg.Intersect((derivedgate_edge, active_edge))
 
-        yield derivedgate_mask
+        yield derivedgate.mask
         if self.min_l is not None:
             yield _edg.Intersect(
                 (derivedgate_edge, active_edge),
             ).length >= self.min_l
         if self.min_w is not None:
             yield _edg.Intersect(
                 (derivedgate_edge, poly_edge),
             ).length >= self.min_w
         if self.min_sd_width is not None:
             yield (
-                active_mask.extend_over(derivedgate_mask) >= self.min_sd_width
+                active_mask.extend_over(derivedgate.mask) >= self.min_sd_width
             )
         if self.min_polyactive_extension is not None:
             yield (
-                poly_mask.extend_over(derivedgate_mask)
+                poly_mask.extend_over(derivedgate.mask)
                 >= self.min_polyactive_extension
             )
         for i in range(len(self.implant)):
             impl_mask = self.implant[i].mask
             enc = self.min_gateimplant_enclosure[i]
             if not enc.is_assymetric:
-                yield derivedgate_mask.enclosed_by(impl_mask) >= enc
+                yield derivedgate.mask.enclosed_by(impl_mask) >= enc
             else:
                 yield channel_edge.enclosed_by(impl_mask) >= enc.spec[0]
                 yield fieldgate_edge.enclosed_by(impl_mask) >= enc.spec[1]
         if self.min_gate_space is not None:
-            yield derivedgate_mask.space >= self.min_gate_space
+            yield derivedgate.mask.space >= self.min_gate_space
         if self.min_contactgate_space is not None:
             assert self.contact is not None
             yield (
-                _msk.Spacing(derivedgate_mask, self.contact.mask)
+                _msk.Spacing(derivedgate.mask, self.contact.mask)
                 >= self.min_contactgate_space
             )
 
     @property
     def designmasks(self):
         yield from super().designmasks
         yield from self.gate.designmasks
```

### Comparing `PDKMaster-0.9.3/pdkmaster/technology/primitive/layers.py` & `PDKMaster-0.9.4/pdkmaster/technology/primitive/layers.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/technology/primitive/rules.py` & `PDKMaster-0.9.4/pdkmaster/technology/primitive/rules.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/technology/property_.py` & `PDKMaster-0.9.4/pdkmaster/technology/property_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/technology/rule.py` & `PDKMaster-0.9.4/pdkmaster/technology/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/pdkmaster/technology/technology_.py` & `PDKMaster-0.9.4/pdkmaster/technology/technology_.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: AGPL-3.0-or-later OR GPL-2.0-or-later OR CERN-OHL-S-2.0+ OR Apache-2.0
 from math import floor, ceil
 import abc
-from typing import Optional, Union, Iterable, cast, overload
+from typing import Dict, Optional, Union, Iterable, cast, overload
 
 from . import (
     property_ as _prp, rule as _rle, mask as _msk, wafer_ as _wfr, geometry as _geo,
     primitive as _prm,
 )
 
 
@@ -39,31 +39,41 @@
         object.
         """
         def __init__(self, tech: "Technology"):
             self.tech = tech
 
         @overload
         def min_space(self,
-            primitive1: "_prm.MaskPrimitiveT", primitive2: None=None,
+            primitive1: "_prm.MaskPrimitiveT", primitive2: None=None, *,
+            max_enclosure: bool=False,
         ) -> float:
             ... # pragma: no cover
         @overload
         def min_space(self,
-            primitive1: "_prm.PrimitiveT", primitive2: "_prm.PrimitiveT",
+            primitive1: "_prm.PrimitiveT", primitive2: "_prm.PrimitiveT", *,
+            max_enclosure: bool=False,
         ) -> float:
             ... # pragma: no cover
         def min_space(self,
-            primitive1: "_prm.PrimitiveT", primitive2: Optional["_prm.PrimitiveT"]=None,
+            primitive1: "_prm.PrimitiveT", primitive2: Optional["_prm.PrimitiveT"]=None, *,
+            max_enclosure: bool=False,
         ) -> float:
             """Compute the minimum space between one or two primitives. It will go
             over all the rules to determine the minimum space for the provided
             primitive.
             This function allows to compute the min_space on primitives that are
             derived from other primitives.
 
+            It is also usable to derive more complex minimum spacing on WaferWire
+            primitives. For exmaple, you can do
+            `tech.computed.min_space(active.in_(nimplant), active.in_(pimplant))`
+            the value is computed so that none of the implants drawn on the first
+            waferwire is not overlapping with the one on the second. The enclosing
+            layer is assumed to be drawn with minimal enclosure.
+
             Arguments:
                 primitive1: the first primitive
                     if primitive2 is not given, the minimum space between shapes
                     on the primitive1 layer is returned.
                 primitive2: the optional second primitive.
                     if specified the minimum space between shape on layer primitive1
                     and shapes on layer primitive2 is returned.
@@ -96,14 +106,90 @@
             if (primitive2 is None) or (primitive1 == primitive2):
                 try:
                     space = cast(_prm.WidthSpacePrimitiveT, primitive1).min_space
                 except AttributeError: # pragma: no cover
                     pass
                 else:
                     spaces.append(space)
+                if isinstance(primitive1, _prm.conductors._WaferWireIntersect):
+                    spaces.append(primitive1.waferwire.min_space)
+
+            if (
+                isinstance(primitive1, _prm.conductors._WaferWireIntersect)
+                and isinstance(primitive2, _prm.WaferWire)
+            ):
+                (primitive1, primitive2) = (primitive2, primitive1)
+
+            def get_enc(*, ww: _prm.WaferWire, prim: _prm.MaskPrimitiveT):
+                enc = None
+                if prim in ww2.implant:
+                    idx = ww2.implant.index(prim)
+                    enc = ww2.min_implant_enclosure[idx]
+                elif prim in ww2.well:
+                    idx = ww2.well.index(prim)
+                    enc = ww2.min_well_enclosure[idx]
+                elif prim in ww2.oxide:
+                    idx = ww2.oxide.index(prim)
+                    enc = ww2.min_oxide_enclosure[idx]
+                else: # pragma: no cover
+                    raise RuntimeError(
+                        "Internal error: unsupported enclosed layer"
+                        f" '{prim.name}' for '{ww2.name}'")
+
+                return (
+                    None if enc is None
+                    else enc.min() if not max_enclosure
+                    else enc.max()
+                )
+
+            if isinstance(primitive1, _prm.WaferWire):
+                if isinstance(primitive2, _prm.conductors._WaferWireIntersect):
+                    ww2 = primitive2.waferwire
+
+                    try:
+                        s = self.min_space(primitive1, ww2)
+                    except: # pragma: no cover
+                        pass
+                    else:
+                        spaces.append(s)
+
+                    if primitive1 == ww2:
+                        for prim in primitive2.prim:
+                            enc = get_enc(ww=ww2, prim=prim)
+                            if enc is not None:
+                                try:
+                                    s = self.min_space(primitive1, prim)
+                                except:
+                                    pass
+                                else:
+                                    spaces.append(enc + s)
+            elif (
+                isinstance(primitive1, _prm.conductors._WaferWireIntersect)
+                and isinstance(primitive2, _prm.conductors._WaferWireIntersect)
+            ):
+                ww1 = primitive1.waferwire
+                ww2 = primitive2.waferwire
+
+                spaces.extend((
+                    self.min_space(ww1, primitive2),
+                    self.min_space(ww2, primitive1),
+                ))
+
+                e1s = []
+                for prim in primitive1.prim:
+                    enc = get_enc(ww=ww1, prim=prim)
+                    if enc is not None:
+                        e1s.append(enc)
+                e2s = []
+                for prim in primitive2.prim:
+                    enc = get_enc(ww=ww2, prim=prim)
+                    if enc is not None:
+                        e2s.append(enc)
+                if (len(e1s) > 0) and (len(e2s) > 0):
+                    spaces.append(max(e1s) + max(e2s))
 
             try:
                 return max(spaces)
             except ValueError:
                 raise AttributeError(
                     f"min_space between {primitive1} and {primitive2} not found",
                 )
@@ -181,21 +267,29 @@
         """
         ... # pragma: no cover
 
     @abc.abstractmethod
     def __init__(self, *, primitives: "_prm.Primitives"):
         self._primitives = primitives
 
-        well_masks = tuple(
-            prim.mask for prim in self._primitives.__iter_type__(_prm.Well)
-        )
-        if not well_masks:
-            self._substrate = _wfr.wafer
+        # primitives needs to contain exectly one Base primitive which
+        # is always called base
+        try:
+            base = primitives.base
+        except:
+            raise ValueError("A technology needs exactly one 'Base` primitive")
+        else:
+            if not isinstance(base, _prm.Base):
+                raise ValueError("A technology needs exactly one 'Base` primitive")
+
+        wells = tuple(self._primitives.__iter_type__(_prm.Well))
+        if not wells:
+            self._substrate_prim = self.base
         else:
-            self._substrate = _wfr.outside(well_masks, alias=f"substrate:{self.name}")
+            self._substrate_prim = self.base.remove(wells).alias(f"substrate:{self.name}")
 
         self._build_interconnect()
         self._build_rules()
 
         primitives._freeze_()
 
         self.computed = self._ComputedSpecs(self)
@@ -287,24 +381,16 @@
                 idx = prims.index(prim)
                 if idx not in neworder:
                     neworder.append(idx)
 
         def get_name(prim):
             return prim.name
 
-        # primitives needs to contain exectly one Base primitive which
-        # is always called base
-        try:
-            base = prims.base
-        except:
-            raise ValueError("A technology needs exactly one 'Base` primitive")
-        else:
-            if not isinstance(base, _prm.Base):
-                raise ValueError("A technology needs exactly one 'Base` primitive")
-        add_prims((base,))
+        # base
+        add_prims((prims.base,))
 
         # set that are build up when going over the primitives
         # bottomwires: primitives that still need to be bottomconnected by a via
         bottomwires = set()
         # implants: used implant not added yet
         implants = set() # Implants to add
         markers = set() # Markers to add
@@ -331,16 +417,15 @@
 
         # Already add implants that are used in the waferwires
         add_prims(sorted(implants, key=get_name))
         implants = set()
 
         # Add the oxides
         for ww in waferwires:
-            if ww.oxide is not None:
-                add_prims(sorted(ww.oxide, key=get_name))
+            add_prims(sorted(ww.oxide, key=get_name))
 
         # process vias
         vias = set(prims.__iter_type__(_prm.Via))
 
         def allwires(wire):
             if isinstance(wire, _prm.Resistor):
                 yield from allwires(wire.wire)
@@ -409,14 +494,30 @@
         polys = {gate.poly for gate in gates}
         for mosfet in mosfets:
             implants.update(mosfet.implant)
             if mosfet.well is not None:
                 implants.add(mosfet.well)
             if mosfet.gate.inside is not None:
                 markers.update(mosfet.gate.inside)
+        # Each well and the substrate may either contain only transistors without
+        # n/p type implants or all with n/p type implants
+        # store first mosfet in a well in wellmosfet, check nect mosfets if they match
+        wellmosfet: Dict[Optional[_prm.Well], _prm.MOSFET] = {}
+        for mos in mosfets:
+            well = mos.well
+            if well not in wellmosfet:
+                wellmosfet[well] = mos
+            else:
+                prevmos = wellmosfet[well]
+                if prevmos.has_typeimplant != mos.has_typeimplant:
+                    name = f"same well '{well.name}'" if well is not None else "substrate"
+                    raise ValueError(
+                        f"MOSFETs '{prevmos.name}' and '{mos.name}' with and without type implant"
+                        f" in {name}"
+                    )
 
         add_prims((
             *sorted(implants, key=get_name),
             *sorted(actives, key=get_name), *sorted(polys, key=get_name),
             *sorted(markers, key=get_name), *sorted(gates, key=get_name),
             *sorted(mosfets, key=get_name),
         ))
@@ -484,38 +585,53 @@
 
         # Generate the rule but don't add them yet.
         for prim in prims:
             prim._derive_rules(self)
 
         # First add substrate alias if needed. This will only be clear
         # after the rules have been generated.
-        sub = self.substrate
-        if isinstance(sub, _msk._MaskAlias):
-            self._rules += sub
-        if sub != _wfr.wafer:
-            self._rules += _msk.Connect(sub, _wfr.wafer)
+        sub_mask = self.substrate_prim.mask
+        if isinstance(sub_mask, _msk._MaskAlias):
+            self._rules += sub_mask
+        if sub_mask != _wfr.wafer:
+            self._rules += _msk.Connect(sub_mask, _wfr.wafer)
 
         # Now we can add the rules
         for prim in prims:
             self._rules += prim.rules
 
         rules._freeze_()
 
     @property
-    def substrate(self) -> _msk.MaskT:
+    def substrate_prim(self) -> "_prm.MaskPrimitiveT":
         """Property representing the substrate of the technology; it's defined as the area
         that is outside any of the wells of the technology.
 
         As this value needs access to the list of wells it's only available afcer the
         technology has been initialized and is not available during run of the `_init()`
         method.
         """
-        if not hasattr(self, "_substrate"):
+        if not hasattr(self, "_substrate_prim"):
             raise AttributeError("substrate may not be accessed during object initialization")
-        return self._substrate
+        return self._substrate_prim
+
+    # Backwards compatibility
+    @property
+    def substrate(self) -> _msk.MaskT:
+        """Property representing the substrate of the technology; it's defined as the area
+        that is outside any of the wells of the technology.
+
+        As this value needs access to the list of wells it's only available afcer the
+        technology has been initialized and is not available during run of the `_init()`
+        method.
+
+        API Notes:
+            * This property is deprecated and will be removedin V1.0; use substrate_prim.mask
+        """
+        return self.substrate_prim.mask
 
     @property
     def rules(self) -> Iterable[_rle.RuleT]:
         """Return all the rules that are derived from the primitives of the technology."""
         return self._rules
 
     @property
```

### Comparing `PDKMaster-0.9.3/pdkmaster/technology/wafer_.py` & `PDKMaster-0.9.4/pdkmaster/technology/wafer_.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # SPDX-License-Identifier: AGPL-3.0-or-later OR GPL-2.0-or-later OR CERN-OHL-S-2.0+ OR Apache-2.0
 from typing import Iterable, Optional
 
 from ..typing import MultiT, cast_MultiT
 from . import property_ as _prp, net as _net, mask as _msk
 
 
-__all__ = ["wafer", "outside", "SubstrateNet"]
+__all__ = [
+    "wafer", "SubstrateNet",
+    # Backwards compatibility
+    "outside",
+]
 
 
 class _Wafer(_msk._Mask):
     """Wafer is a `Mask` that represents a full wafer. Only one object
     is allowed to be created from this class and this is done through
     the wafer variable. This variable is exported from the
     `pdkmaster.technology.wafer_` module and that variable is to be used
@@ -37,17 +41,22 @@
         return self.__class__ is other.__class__
 
     def __hash__(self) -> int:
         return super().__hash__()
 wafer = _Wafer()
 
 
+# Backwards compatibility
 def outside(masks: MultiT[_msk.DesignMask], *, alias: Optional[str]=None) -> _msk.MaskT:
     """Return a mask representing the area on the wafer outside other mask(s).
     Optionally an alias can be given for the generated mask.
+
+    API Notes:
+        * this function is deprecated and will be removed in V1.0.
+          use wafer.remove() instead
     """
     masks = cast_MultiT(masks)
     if len(masks) == 1:
         mask = wafer.remove(masks[0])
     else:
         mask = wafer.remove(_msk.Join(set(masks)))
     if alias is None:
```

### Comparing `PDKMaster-0.9.3/pdkmaster/typing.py` & `PDKMaster-0.9.4/pdkmaster/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
     except TypeError:
         v = (cast(T, vs),)
     else:
         if isinstance(vs, singular_type):
             v = (cast(T, vs),)
         else:
             v = tuple(cast(Iterable[T], vs))
+    if (n == 0) and (len(v) != 0):
+        raise ValueError(f"Value(s) provided for MultiT that has to be zero length")
     if len(v) == 1:
         v *= n
     if len(v) != n:
         raise ValueError(f"Exactly {n} elements need to be provided not {len(v)}")
     return v
 
 def cast_OptMultiT(vs: OptMultiT[T], *, singular_type: Tuple[type, ...]=(str,)) -> Optional[Tuple[T, ...]]:
```

### Comparing `PDKMaster-0.9.3/setup.py` & `PDKMaster-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/skill.py` & `PDKMaster-0.9.4/skill.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/skill2yaml.py` & `PDKMaster-0.9.4/skill2yaml.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/_util.py` & `PDKMaster-0.9.4/test/unit/_util.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/design/cell.py` & `PDKMaster-0.9.4/test/unit/design/cell.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/design/circuit.py` & `PDKMaster-0.9.4/test/unit/design/circuit.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/design/factory.py` & `PDKMaster-0.9.4/test/unit/design/factory.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/design/layout.py` & `PDKMaster-0.9.4/test/unit/design/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,25 +116,21 @@
             well=nwell, min_well_enclosure=_prp.Enclosure(0.1),
             min_well_enclosure_same_type=_prp.Enclosure(0.08),
             allow_well_crossing=False,
             oxide=hvox, min_oxide_enclosure=_prp.Enclosure(0.08),
         )
         params = caster(prim=active2, well_net=net, oxide=hvox)
 
-        self.assertEqual(params["implant"], nplus)
-        self.assertAlmostEqual(params["implant_enclosure"].first, 0.05)
+        self.assertEqual(params["implant"], None)
+        self.assertAlmostEqual(params["implant_enclosure"], None)
         self.assertEqual(params["well"], nwell)
         self.assertAlmostEqual(params["oxide_enclosure"].first, 0.08)
 
         ### Via errors
 
-        # no bottom_implant
-        with self.assertRaises(TypeError):
-            caster(prim=ch, bottom=active)
-
         # wrong bottom_well
         with self.assertRaises(ValueError):
             caster(prim=ch, bottom=active, bottom_implant=nplus, bottom_well=deepwell)
 
         # bottom WaferWire parameters given for GateWire bottom
         with self.assertRaises(TypeError):
             caster(prim=ch, bottom=poly, bottom_implant=nplus)
@@ -672,14 +668,20 @@
                 bottom=prims.metal, bottom_enclosure=enc,
                 bottom_width=mwidth, bottom_height=None,
                 top=prims.metal2, top_enclosure=enc,
                 top_width=mwidth, top_height=None,
             ),
         )
 
+        # Via with bottom_implant_enclosure but without bottom_implant
+        with self.assertRaises(TypeError):
+            layouter(
+                prims.contact, bottom=prims.active, bottom_implant_enclosure=_prp.Enclosure(1.0),
+            )
+
         # Code coverage for bottom_width/bottom_height/top_width/top_width None/float
         # combinations
         layouter(
             prims.via, space=0.35, rows=None, columns=1,
             bottom=prims.metal, bottom_enclosure=enc,
             bottom_width=None, bottom_height=None,
             top=prims.metal2, top_enclosure=enc,
```

### Comparing `PDKMaster-0.9.3/test/unit/design/library.py` & `PDKMaster-0.9.4/test/unit/design/library.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/dispatch/edge.py` & `PDKMaster-0.9.4/test/unit/dispatch/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/dispatch/mask.py` & `PDKMaster-0.9.4/test/unit/dispatch/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/dispatch/primitive.py` & `PDKMaster-0.9.4/test/unit/dispatch/primitive.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 
         pad = _prm.PadOpening(
             name="pad", min_width=20.0, min_space=5.0,
             bottom=dummy_prims.metal, min_bottom_enclosure=_prp.Enclosure(1.0),
         )
         sect1 = dummy_prims.active.in_(dummy_prims.nplus)
         sect2 = dummy_prims.contact.in_(dummy_prims.active)
-        for prim in (*dummy_prims, pad, sect1, sect2):
+        rm1 = dummy_prims.active.remove(dummy_prims.nplus)
+        for prim in (*dummy_prims, pad, sect1, sect2, rm1):
             self.assertIs(disp(prim), type(prim))
 
     def test_hier(self):
         disp = IsWidthSpaceConductor()
 
         self.assertTrue(disp(dummy_prims.nwell))
         self.assertFalse(disp(dummy_prims.nplus))
```

### Comparing `PDKMaster-0.9.3/test/unit/dispatch/rule.py` & `PDKMaster-0.9.4/test/unit/dispatch/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/dispatch/shape.py` & `PDKMaster-0.9.4/test/unit/dispatch/shape.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/dummy.py` & `PDKMaster-0.9.4/test/unit/dummy.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,17 @@
         prims += aux
 
         prims += (
             _prm.Spacing(
                 primitives1=(nplus, pplus), primitives2=mosgate, min_space=0.25,
             ),
             _prm.Spacing(
+                primitives1=active, primitives2=hvox, min_space=0.2,
+            ),
+            _prm.Spacing(
                 primitives1=(nwell, pplus), min_space=2.0,
             ),
             _prm.MinWidth(prim=active.in_(hvox), min_width=0.5),
             _prm.Enclosure(prim=active, by=esd, min_enclosure=_prp.Enclosure(0.1)),
             _prm.NoOverlap(prim1=nplus, prim2=pplus),
         )
```

### Comparing `PDKMaster-0.9.3/test/unit/io/klayout/export.py` & `PDKMaster-0.9.4/test/unit/io/klayout/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/io/klayout/merge.py` & `PDKMaster-0.9.4/test/unit/io/klayout/merge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/io/lefdef/export.py` & `PDKMaster-0.9.4/test/unit/io/lefdef/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/io/pdkmaster/export.py` & `PDKMaster-0.9.4/test/unit/io/pdkmaster/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/io/spice/pyspice.py` & `PDKMaster-0.9.4/test/unit/io/spice/pyspice.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/io/spice/spice_.py` & `PDKMaster-0.9.4/test/unit/io/spice/spice_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/technology/edge.py` & `PDKMaster-0.9.4/test/unit/technology/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/technology/geometry.py` & `PDKMaster-0.9.4/test/unit/technology/geometry.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/technology/mask.py` & `PDKMaster-0.9.4/test/unit/technology/mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,18 @@
             )
 
         mask = _msk.DesignMask(name="mask")
 
         with self.assertRaises(ValueError):
             _msk.Spacing(mask1=mask, mask2=mask)
 
+        # No value given for .remove()
+        with self.assertRaises(ValueError):
+            mask.remove(())
+
     def test_mask(self):
         # We use DesignMask object to also cover code for _Mask and other
         # classes
         mask = _msk.DesignMask(name="MyMask")
         mask2 = _msk.DesignMask(name="MyMask2")
         mask3 = _msk.DesignMask(name="MyMask3")
         
@@ -69,14 +73,18 @@
         with self.assertRaises(TypeError):
             mask.parts_with(cond2)
         self.assertEqual(
             mask.remove(mask2),
             _msk._MaskRemove(from_=mask, what=mask2),
         )
         self.assertEqual(
+            mask.remove(mask2, mask3),
+            _msk._MaskRemove(from_=mask, what=_msk.Join(mask2, mask3))
+        )
+        self.assertEqual(
             alias, _msk._MaskAlias(mask=mask, name="Alias"),
         )
         self.assertEqual(samenet, _msk._SameNet(mask))
 
         self.assertNotEqual(alias, "")
         self.assertNotEqual(samenet, "")
         self.assertNotEqual(mask.extend_over(other=mask2), "")
```

### Comparing `PDKMaster-0.9.3/test/unit/technology/primitive.py` & `PDKMaster-0.9.4/test/unit/technology/primitive.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,41 +31,68 @@
 
 class PrimitiveTest(unittest.TestCase):
     def test_simple(self):
         """Some simple tests not wanting to define own method
         """
         dummy_prims = dummy_tech.primitives
 
+        active = dummy_prims.active
+        nplus = dummy_prims.nplus
+        pplus = dummy_prims.pplus
+        poly = dummy_prims.poly
+
         # _Primitive
         with self.assertRaises(TypeError):
             _prmcore._Primitive(name="error")
         with self.assertRaises(ValueError):
             dummy_prims.metal._derive_rules(tech=dummy_tech)
 
         # _PrimParam
         with self.assertRaises(TypeError):
             _prmparm._PrimParam(
-                primitive=dummy_prims.active, name="error", default=dummy_prims,
+                primitive=active, name="error", default=dummy_prims,
             )
 
         # _DesignMaskPrimitive
         with self.assertRaises(TypeError):
             class MyPrim(_prmcore._DesignMaskPrimitive):
                 def __init__(self, *, name: str, **super_args):
                     super().__init__(name=name, **super_args)
 
                 def _generate_rules(self, *, tech, gen_mask):
                     return super()._generate_rules(tech=tech, gen_mask=gen_mask)
             mask = _msk.DesignMask(name="error")
             MyPrim(name="error", mask=mask)
 
+        # _MaskPrimitive.remove()
+        self.assertEqual(
+            active.remove(poly).mask,
+            active.mask.remove(poly.mask)
+        )
+        self.assertEqual(
+            active.remove((nplus, pplus)).mask,
+            active.mask.remove(_msk.Join((nplus.mask, pplus.mask)))
+        )
+        with self.assertRaises(ValueError):
+            active.remove(())
+
         # _Intersect
+        self.assertEqual(
+            active.in_(nplus).mask,
+            _msk.Intersect((active.mask, nplus.mask)),
+        )
         with self.assertRaises(ValueError):
             # only one prim for _Intersect
-            _prmderv._Intersect(prims=(dummy_prims.active,))
+            _prmderv._Intersect(prims=(active,))
+
+        # _Alias
+        self.assertEqual(
+            active.alias("alias").mask,
+            active.mask.alias("alias"),
+        )
 
     def test_marker(self):
         marker = _prm.Marker(name="TestMarker")
         marker2 = _prm.Marker(name="TestMarker2")
 
         with self.assertRaises(AttributeError):
             # Accessing rules before they are generated.
@@ -230,24 +257,14 @@
         well2 = _prm.Well(
             name="well2", min_width=1.0, min_space=1.0, type_=_prm.nImpl,
         )
 
         with self.assertRaises(TypeError):
             _prm.WaferWire(name="prim1", min_width=1.0, min_space=1.0)
 
-        with self.assertRaises(_prm.UnconnectedPrimitiveError):
-            # Unconnected well
-            _prm.WaferWire(
-                name="prim1", min_width=1.0, min_space=1.0,
-                allow_in_substrate=True,
-                implant=nimpl, min_implant_enclosure=_prp.Enclosure(0.05),
-                implant_abut="all", allow_contactless_implant=False,
-                well=well, min_well_enclosure=_prp.Enclosure(0.1),
-                allow_well_crossing=False,
-            )
         with self.assertRaises(TypeError):
             # well not implant
             _prm.WaferWire(
                 name="prim1", min_width=1.0, min_space=1.0,
                 allow_in_substrate=True,
                 implant=(nimpl, well), min_implant_enclosure=_prp.Enclosure(0.05),
                 implant_abut="all", allow_contactless_implant=False,
@@ -1047,21 +1064,14 @@
             # both n and p type implants
             _prm.MOSFET(
                 name="error", gate=gate1, min_l=1.5, min_w=1.5,
                 implant=(nimpl, pimpl), min_gateimplant_enclosure=_prp.Enclosure(0.2),
                 min_contactgate_space=0.15, well=well,
             )
         with self.assertRaises(ValueError):
-            # only adjust implant
-            _prm.MOSFET(
-                name="error", gate=gate1, min_l=1.5, min_w=1.5,
-                implant=adjust, min_gateimplant_enclosure=_prp.Enclosure(0.2),
-                min_contactgate_space=0.15, well=well,
-            )
-        with self.assertRaises(ValueError):
             # invalid implant for gate.active
             _prm.MOSFET(
                 name="error", gate=gate1, min_l=1.5, min_w=1.5,
                 implant=nimpl2, min_gateimplant_enclosure=_prp.Enclosure(0.2),
                 min_contactgate_space=0.15, well=well,
             )
         with self.assertRaises(ValueError):
@@ -1139,30 +1149,29 @@
             name="prim2", gate=gate2, min_gate_space=1.5,
             implant=nimpl, min_gateimplant_enclosure=_prp.Enclosure(0.2),
             min_sd_width=0.15, min_polyactive_extension=0.2,
             contact=ch, min_contactgate_space=0.1,
         )
         prim3 = _prm.MOSFET(
             name="prim3", gate=gate1, min_l=1.5, min_w=1.5,
-            implant=nimpl, min_gateimplant_enclosure=_prp.Enclosure(0.2),
+            implant=(), min_gateimplant_enclosure=(),
             min_contactgate_space=0.15, well=well,
         )
 
         self.assertEqual(prim1, prim1bis)
         self.assertNotEqual(prim1, prim2)
         self.assertNotEqual(prim1, prim3)
 
-        self.assertEqual(
-            prim1.gate_prim,
-            _prmderv._Intersect(prims=(prim1.gate, *prim1.implant)),
-        )
-        self.assertEqual(
-            prim3.gate_prim,
-            _prmderv._Intersect(prims=(prim3.gate, *prim1.implant, prim3.well)),
-        )
+        self.assertTrue(prim1.has_typeimplant)
+        self.assertTrue(prim2.has_typeimplant)
+        self.assertFalse(prim3.has_typeimplant)
+
+        # Access gate4mosfet before being added to technology
+        with self.assertRaises(TypeError):
+            prim1.gate4mosfet
 
         self.assertAlmostEqual(prim1.computed.min_l, 1.5, places=6)
         self.assertAlmostEqual(prim1.computed.min_sd_width, 0.15, places=6)
         self.assertAlmostEqual(prim1.computed.min_contactgate_space, 0.1, places=6)
         self.assertAlmostEqual(prim3.computed.min_contactgate_space, 0.15, places=6)
         self.assertEqual(prim1.computed.contact, ch)
         self.assertAlmostEqual(prim2.computed.min_l, 1.0, places=6)
```

### Comparing `PDKMaster-0.9.3/test/unit/technology/property.py` & `PDKMaster-0.9.4/test/unit/technology/property.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/technology/rule.py` & `PDKMaster-0.9.4/test/unit/technology/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/technology/technology.py` & `PDKMaster-0.9.4/test/unit/technology/technology.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,26 +35,70 @@
                 def __init__(self):
                     super().__init__(primitives=_prm.Primitives(
                         _prm.Auxiliary(name="base")
                     ))
             ErrorTech()
 
     def test_computed(self):
+        nwell = dummy_prims.nwell
         active = dummy_prims.active
+        nplus = dummy_prims.nplus
+        pplus = dummy_prims.pplus
+        hvox = dummy_prims.hvox
         poly = dummy_prims.poly
         contact = dummy_prims.contact
         metal = dummy_prims.metal
         via = dummy_prims.via
 
         # min_space
+        nenc = active.min_implant_enclosure[active.implant.index(nplus)].min()
+        penc = active.min_implant_enclosure[active.implant.index(pplus)].min()
+        nwenc = active.min_well_enclosure[active.well.index(nwell)].min()
+        hvoxenc = active.min_oxide_enclosure[active.oxide.index(hvox)].min()
+        hvoxspace = dummy_tech.computed.min_space(hvox, active)
+
         self.assertAlmostEqual(
             dummy_tech.computed.min_space(primitive1=active),
             active.min_space,
             places=6,
         )
+        self.assertAlmostEqual(
+            dummy_tech.computed.min_space(primitive1=active.in_(nplus)),
+            active.min_space,
+            places=6,
+        )
+        self.assertAlmostEqual(
+            dummy_tech.computed.min_space(
+                primitive1=active, primitive2=active.in_((pplus, hvox, nwell)),
+            ),
+            hvoxenc + hvoxspace,
+            places=6,
+        )
+        self.assertAlmostEqual(
+            dummy_tech.computed.min_space(
+                primitive1=active.in_(nplus), primitive2=active,
+            ),
+            active.min_space,
+            places=6,
+        )
+        self.assertAlmostEqual(
+            dummy_tech.computed.min_space(
+                primitive1=active.in_(nplus), primitive2=active.in_(pplus),
+            ),
+            nenc + penc,
+            places=6,
+        )
+        self.assertAlmostEqual(
+            dummy_tech.computed.min_space(
+                primitive1=active.in_(nplus),
+                primitive2=active.in_((pplus, nwell, hvox)),
+            ),
+            nenc + max(penc, nwenc, hvoxenc),
+            places=6,
+        )
         with self.assertRaises(AttributeError):
             # No min_space between active and poly
             dummy_tech.computed.min_space(
                 primitive1=active, primitive2=poly
             )
 
         # min_width
@@ -183,14 +227,32 @@
                 )
                 prims += (metal1, pad)
 
                 super().__init__(primitives=prims)
         # Code coverage only
         MyTech()
 
+    def test_substrate(self):
+        self.assertEqual(
+            dummy_tech.substrate_prim,
+            dummy_prims.base.remove(dummy_prims.active.well).alias("substrate:Dummy"),
+        )
+        self.assertEqual(
+            dummy_tech.substrate,
+            dummy_tech.substrate_prim.mask,
+        )
+
+    def test_mosfet(self):
+        nmos = dummy_prims.nmos
+        prim = _prm._derived._Intersect(prims=(nmos.gate, dummy_tech.substrate_prim, *nmos.implant))
+        alias = prim.alias("gate:mosfet:nmos")
+        self.assertEqual(nmos.gate4mosfet._prim, prim)
+        self.assertEqual(nmos.gate4mosfet, alias)
+        self.assertEqual(nmos.gate_mask, nmos.gate4mosfet.mask)
+
     def test_check(self):
         class MyTech(_tch.Technology):
             @property
             def name(self) -> str:
                 return "MyTech"
             @property
             def grid(self) -> float:
@@ -327,14 +389,71 @@
             @property
             def grid(self) -> float:
                 return 5e-3
 
             def __init__(self):
                 prims = _prm.Primitives(_prm.Base(type_=_prm.pBase))
 
+                nimpl = _prm.Implant(
+                    name="nimplant", min_width=1.2, min_space=1.2, type_=_prm.nImpl,
+                )
+                pimpl = _prm.Implant(
+                    name="pimplant", min_width=1.2, min_space=1.2, type_=_prm.pImpl,
+                )
+                nwell = _prm.Well(
+                    name="nwell", min_width=5.0, min_space=3.0, type_=_prm.nImpl,
+                )
+                prims += (nimpl, pimpl, nwell)
+
+                active = _prm.WaferWire(
+                    name="active", min_width=0.8, min_space=0.8,
+                    implant=nimpl, min_implant_enclosure=_prp.Enclosure(0.2),
+                    implant_abut="all", allow_contactless_implant=False,
+                    allow_in_substrate=True,
+                    well=nwell, min_well_enclosure=_prp.Enclosure(0.8),
+                    allow_well_crossing=False,
+                )
+                poly = _prm.GateWire(name="poly", min_width=0.8, min_space=0.8)
+                metal1 = _prm.MetalWire(name="metal1", min_width=1.0, min_space=1.0)
+                contact = _prm.Via(
+                    name="contact", width=0.8, min_space=0.8,
+                    bottom=(active, poly), min_bottom_enclosure=_prp.Enclosure(0.0),
+                    top=metal1, min_top_enclosure=_prp.Enclosure(0.2),
+                )
+                prims += (active, poly, contact, metal1)
+
+                gate = _prm.MOSFETGate(
+                    active=active, poly=poly,
+                    min_sd_width=0.35, min_polyactive_extension=0.35,
+                )
+                nmos_impl = _prm.MOSFET(
+                    name="nmos_impl", gate=gate, implant=nimpl,
+                    min_gateimplant_enclosure=_prp.Enclosure(0.3),
+                )
+                nmos_noimpl = _prm.MOSFET(
+                    name="nmos_noimpl", gate=gate, implant=(),
+                    min_gateimplant_enclosure=(),
+                )
+                prims += (gate, nmos_impl, nmos_noimpl)
+
+                super().__init__(primitives=prims)
+        with self.assertRaises(ValueError):
+            MyTech()
+
+        class MyTech(_tch.Technology):
+            @property
+            def name(self) -> str:
+                return "MyTech"
+            @property
+            def grid(self) -> float:
+                return 5e-3
+
+            def __init__(self):
+                prims = _prm.Primitives(_prm.Base(type_=_prm.pBase))
+
                 metal1 = _prm.MetalWire(name="metal1", min_width=1.0, min_space=1.0)
                 metal2 = _prm.MetalWire(name="metal1", min_width=1.0, min_space=1.0)
                 via = _prm.Via(
                     name="via", width=0.8, min_space=0.8,
                     bottom=metal1, min_bottom_enclosure=_prp.Enclosure(0.2),
                     top=metal2, min_top_enclosure=_prp.Enclosure(0.2),
                 )
@@ -356,19 +475,20 @@
                 super().__init__(primitives=_prm.Primitives((
                     _prm.Base(type_=_prm.pBase),
                     _prm.MIMTop(name="error", min_width=1.0, min_space=1.0),
                 )))
         with self.assertRaises(_prm.UnusedPrimitiveError):
             MyTech()
 
+        # Accessing substrate_prim before primitives were added
         class MyTech(_tch.Technology):
             @property
             def name(self) -> str:
                 return "MyTech"
             @property
             def grid(self) -> float:
                 return 5e-3
 
             def __init__(self):
-                self.substrate
+                self.substrate_prim
         with self.assertRaises(AttributeError):
             MyTech()
```

### Comparing `PDKMaster-0.9.3/test/unit/technology/wafer.py` & `PDKMaster-0.9.4/test/unit/technology/wafer.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.3/test/unit/typing.py` & `PDKMaster-0.9.4/test/unit/typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,9 +21,13 @@
         self.assertEqual(cast_OptMultiT("ab"), ("ab",))
         self.assertEqual(cast_OptMultiT(range(2)), (0, 1))
 
         self.assertIs(cast_OptMultiT_n(None, n=2), None)
         self.assertEqual(cast_OptMultiT_n(2, n=2), (2, 2))
         self.assertEqual(cast_OptMultiT_n("ab", n=3), ("ab", "ab", "ab"))
         self.assertEqual(cast_OptMultiT_n(range(2), n=2), (0, 1))
+        # Value provided for n == 0
+        with self.assertRaises(ValueError):
+            cast_OptMultiT_n(1, n=0)
+        # number of values mismatch with n
         with self.assertRaises(ValueError):
             cast_OptMultiT_n(range(2), n=3)
```

### Comparing `PDKMaster-0.9.3/test.tf` & `PDKMaster-0.9.4/test.tf`

 * *Files identical despite different names*


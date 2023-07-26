# Comparing `tmp/shiny_mdc-1.8.0.tar.gz` & `tmp/shiny_mdc-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiny_mdc-1.8.0.tar", max compression
+gzip compressed data, was "shiny_mdc-1.9.0.tar", max compression
```

## Comparing `shiny_mdc-1.8.0.tar` & `shiny_mdc-1.9.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     8088 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/LICENSE
--rw-r--r--   0        0        0       78 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/README.md
--rw-r--r--   0        0        0     2313 2023-07-23 18:19:49.918340 shiny_mdc-1.8.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/__init__.py
--rw-r--r--   0        0        0     1309 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/_latexmk.py
--rw-r--r--   0        0        0     1867 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/_liquid.py
--rw-r--r--   0        0        0     4920 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/_pandoc.py
--rw-r--r--   0        0        0     5100 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/_templates.py
--rw-r--r--   0        0        0       64 2023-07-23 18:19:49.918340 shiny_mdc-1.8.0/shinymdc/_version.py
--rw-r--r--   0        0        0      410 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/resources/dynamic/addappendices.tex
--rw-r--r--   0        0        0      879 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/resources/dynamic/authsetup.tex
--rw-r--r--   0        0        0      316 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/resources/dynamic/authsetupshort.tex
--rw-r--r--   0        0        0      572 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/resources/dynamic/dblfloatsetup.tex
--rw-r--r--   0        0        0      130 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/resources/dynamic/pdfsetup.tex
--rw-r--r--   0        0        0      491 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/resources/static/bibnonatsetup.tex
--rw-r--r--   0        0        0      345 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/resources/static/bibnosupersetup.tex
--rw-r--r--   0        0        0      721 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/resources/static/bibsupersetup.tex
--rw-r--r--   0        0        0     3266 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/resources/static/floatsetup.tex
--rw-r--r--   0        0        0    19901 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/resources/static/iccv/bibstyle.bst
--rw-r--r--   0        0        0     9433 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/resources/static/iccv/esopic.sty
--rw-r--r--   0        0        0     3869 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/resources/static/iccv/everyshi.sty
--rw-r--r--   0        0        0     8276 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/resources/static/iccv/iccv.sty
--rw-r--r--   0        0        0    26973 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/resources/static/iclr/bibstyle.bst
--rw-r--r--   0        0        0     9153 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/resources/static/iclr/iclr.sty
--rw-r--r--   0        0        0    12284 2023-07-23 18:19:29.762355 shiny_mdc-1.8.0/shinymdc/resources/static/iclr/mathcommands.tex
--rw-r--r--   0        0        0    27146 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/shinymdc/resources/static/icml/bibstyle.bst
--rw-r--r--   0        0        0    27887 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/shinymdc/resources/static/icml/icml.sty
--rw-r--r--   0        0        0      735 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/shinymdc/resources/static/mathsetup.tex
--rw-r--r--   0        0        0     1033 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/shinymdc/resources/static/miscsetup.tex
--rw-r--r--   0        0        0    11306 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/shinymdc/resources/static/neurips/neurips.sty
--rw-r--r--   0        0        0      503 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/shinymdc/resources/static/reqsetup.tex
--rw-r--r--   0        0        0    19840 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/shinymdc/shinymdc.py
--rw-r--r--   0        0        0     1062 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/shinymdc/templates/basic.tex
--rw-r--r--   0        0        0     1354 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/shinymdc/templates/iccv.tex
--rw-r--r--   0        0        0     1475 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/shinymdc/templates/iclr.tex
--rw-r--r--   0        0        0     2222 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/shinymdc/templates/icml.tex
--rw-r--r--   0        0        0      968 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/shinymdc/templates/neurips.tex
--rw-r--r--   0        0        0     3172 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/shinymdc/templates/spacious.tex
--rw-r--r--   0        0        0      464 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/shinymdc/templates/standalone.tex
--rw-r--r--   0        0        0     2678 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/shinymdc/templates/stylish.tex
--rw-r--r--   0        0        0    15953 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/test/figures/anscombe.pdf
--rw-r--r--   0        0        0    40892 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/test/figures/densities.pdf
--rw-r--r--   0        0        0    10736 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/test/figures/diamonds.pdf
--rw-r--r--   0        0        0   197017 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/test/figures/gaussian2d.pdf
--rw-r--r--   0        0        0    28282 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/test/figures/lines.png
--rw-r--r--   0        0        0     2988 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/test/main.md
--rwxr-xr-x   0        0        0      315 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/test/make.sh
--rw-r--r--   0        0        0     1166 2023-07-23 18:19:29.766355 shiny_mdc-1.8.0/test/references.bib
--rw-r--r--   0        0        0   690901 2023-07-23 18:19:29.770355 shiny_mdc-1.8.0/test/samples/basic.pdf
--rw-r--r--   0        0        0   414185 2023-07-23 18:19:29.774355 shiny_mdc-1.8.0/test/samples/iccv.pdf
--rw-r--r--   0        0        0   407653 2023-07-23 18:19:29.774355 shiny_mdc-1.8.0/test/samples/iclr.pdf
--rw-r--r--   0        0        0   446740 2023-07-23 18:19:29.778355 shiny_mdc-1.8.0/test/samples/icml.pdf
--rw-r--r--   0        0        0   451322 2023-07-23 18:19:29.778355 shiny_mdc-1.8.0/test/samples/neurips.pdf
--rw-r--r--   0        0        0   600276 2023-07-23 18:19:29.782355 shiny_mdc-1.8.0/test/samples/spacious.pdf
--rw-r--r--   0        0        0   555527 2023-07-23 18:19:29.782355 shiny_mdc-1.8.0/test/samples/standalone.pdf
--rw-r--r--   0        0        0   425326 2023-07-23 18:19:29.786355 shiny_mdc-1.8.0/test/samples/stylish.pdf
--rw-r--r--   0        0        0     1535 2023-07-23 18:19:29.786355 shiny_mdc-1.8.0/test/sections/appendix1.md
--rw-r--r--   0        0        0     1624 2023-07-23 18:19:29.786355 shiny_mdc-1.8.0/test/sections/appendix2.md
--rw-r--r--   0        0        0        0 2023-07-23 18:19:29.786355 shiny_mdc-1.8.0/test/sections/empty.md
--rw-r--r--   0        0        0     2326 2023-07-23 18:19:29.786355 shiny_mdc-1.8.0/test/sections/main1.md
--rw-r--r--   0        0        0     1351 2023-07-23 18:19:29.786355 shiny_mdc-1.8.0/test/sections/main2.md
--rw-r--r--   0        0        0      992 2023-07-23 18:19:29.786355 shiny_mdc-1.8.0/test/utils/commands.md
--rw-r--r--   0        0        0       41 2023-07-23 18:19:29.786355 shiny_mdc-1.8.0/test/utils/ext.md
--rw-r--r--   0        0        0     1043 1970-01-01 00:00:00.000000 shiny_mdc-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     8474 2023-07-26 03:43:17.607105 shiny_mdc-1.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2023-07-26 03:43:17.607105 shiny_mdc-1.9.0/LICENSE
+-rw-r--r--   0        0        0       78 2023-07-26 03:43:17.607105 shiny_mdc-1.9.0/README.md
+-rw-r--r--   0        0        0     2313 2023-07-26 03:43:35.823432 shiny_mdc-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-07-26 03:43:17.607105 shiny_mdc-1.9.0/shinymdc/__init__.py
+-rw-r--r--   0        0        0     1709 2023-07-26 03:43:17.607105 shiny_mdc-1.9.0/shinymdc/_latexmk.py
+-rw-r--r--   0        0        0     1867 2023-07-26 03:43:17.607105 shiny_mdc-1.9.0/shinymdc/_liquid.py
+-rw-r--r--   0        0        0     4920 2023-07-26 03:43:17.607105 shiny_mdc-1.9.0/shinymdc/_pandoc.py
+-rw-r--r--   0        0        0     5100 2023-07-26 03:43:17.607105 shiny_mdc-1.9.0/shinymdc/_templates.py
+-rw-r--r--   0        0        0       64 2023-07-26 03:43:35.823432 shiny_mdc-1.9.0/shinymdc/_version.py
+-rw-r--r--   0        0        0      410 2023-07-26 03:43:17.607105 shiny_mdc-1.9.0/shinymdc/resources/dynamic/addappendices.tex
+-rw-r--r--   0        0        0      879 2023-07-26 03:43:17.607105 shiny_mdc-1.9.0/shinymdc/resources/dynamic/authsetup.tex
+-rw-r--r--   0        0        0      316 2023-07-26 03:43:17.607105 shiny_mdc-1.9.0/shinymdc/resources/dynamic/authsetupshort.tex
+-rw-r--r--   0        0        0      572 2023-07-26 03:43:17.607105 shiny_mdc-1.9.0/shinymdc/resources/dynamic/dblfloatsetup.tex
+-rw-r--r--   0        0        0      130 2023-07-26 03:43:17.607105 shiny_mdc-1.9.0/shinymdc/resources/dynamic/pdfsetup.tex
+-rw-r--r--   0        0        0      491 2023-07-26 03:43:17.607105 shiny_mdc-1.9.0/shinymdc/resources/static/bibnonatsetup.tex
+-rw-r--r--   0        0        0      345 2023-07-26 03:43:17.607105 shiny_mdc-1.9.0/shinymdc/resources/static/bibnosupersetup.tex
+-rw-r--r--   0        0        0      721 2023-07-26 03:43:17.607105 shiny_mdc-1.9.0/shinymdc/resources/static/bibsupersetup.tex
+-rw-r--r--   0        0        0     3266 2023-07-26 03:43:17.607105 shiny_mdc-1.9.0/shinymdc/resources/static/floatsetup.tex
+-rw-r--r--   0        0        0    19901 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/resources/static/iccv/bibstyle.bst
+-rw-r--r--   0        0        0     9433 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/resources/static/iccv/esopic.sty
+-rw-r--r--   0        0        0     3869 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/resources/static/iccv/everyshi.sty
+-rw-r--r--   0        0        0     8276 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/resources/static/iccv/iccv.sty
+-rw-r--r--   0        0        0    26973 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/resources/static/iclr/bibstyle.bst
+-rw-r--r--   0        0        0     9153 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/resources/static/iclr/iclr.sty
+-rw-r--r--   0        0        0    12284 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/resources/static/iclr/mathcommands.tex
+-rw-r--r--   0        0        0    27146 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/resources/static/icml/bibstyle.bst
+-rw-r--r--   0        0        0    27887 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/resources/static/icml/icml.sty
+-rw-r--r--   0        0        0      735 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/resources/static/mathsetup.tex
+-rw-r--r--   0        0        0     1033 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/resources/static/miscsetup.tex
+-rw-r--r--   0        0        0    11306 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/resources/static/neurips/neurips.sty
+-rw-r--r--   0        0        0      503 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/resources/static/reqsetup.tex
+-rw-r--r--   0        0        0    19996 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/shinymdc.py
+-rw-r--r--   0        0        0     1062 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/templates/basic.tex
+-rw-r--r--   0        0        0     1354 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/templates/iccv.tex
+-rw-r--r--   0        0        0     1475 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/templates/iclr.tex
+-rw-r--r--   0        0        0     2222 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/templates/icml.tex
+-rw-r--r--   0        0        0      968 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/templates/neurips.tex
+-rw-r--r--   0        0        0     3172 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/templates/spacious.tex
+-rw-r--r--   0        0        0      464 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/templates/standalone.tex
+-rw-r--r--   0        0        0     2678 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/shinymdc/templates/stylish.tex
+-rw-r--r--   0        0        0    15953 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/test/figures/anscombe.pdf
+-rw-r--r--   0        0        0    40892 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/test/figures/densities.pdf
+-rw-r--r--   0        0        0    10736 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/test/figures/diamonds.pdf
+-rw-r--r--   0        0        0   197017 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/test/figures/gaussian2d.pdf
+-rw-r--r--   0        0        0    28282 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/test/figures/lines.png
+-rw-r--r--   0        0        0     3051 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/test/main.md
+-rwxr-xr-x   0        0        0      315 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/test/make.sh
+-rw-r--r--   0        0        0     1166 2023-07-26 03:43:17.611105 shiny_mdc-1.9.0/test/references.bib
+-rw-r--r--   0        0        0   690901 2023-07-26 03:43:17.615105 shiny_mdc-1.9.0/test/samples/basic.pdf
+-rw-r--r--   0        0        0   414185 2023-07-26 03:43:17.619105 shiny_mdc-1.9.0/test/samples/iccv.pdf
+-rw-r--r--   0        0        0   407653 2023-07-26 03:43:17.619105 shiny_mdc-1.9.0/test/samples/iclr.pdf
+-rw-r--r--   0        0        0   446740 2023-07-26 03:43:17.619105 shiny_mdc-1.9.0/test/samples/icml.pdf
+-rw-r--r--   0        0        0   451322 2023-07-26 03:43:17.623105 shiny_mdc-1.9.0/test/samples/neurips.pdf
+-rw-r--r--   0        0        0   600276 2023-07-26 03:43:17.627105 shiny_mdc-1.9.0/test/samples/spacious.pdf
+-rw-r--r--   0        0        0   555527 2023-07-26 03:43:17.627105 shiny_mdc-1.9.0/test/samples/standalone.pdf
+-rw-r--r--   0        0        0   425326 2023-07-26 03:43:17.631105 shiny_mdc-1.9.0/test/samples/stylish.pdf
+-rw-r--r--   0        0        0     1535 2023-07-26 03:43:17.631105 shiny_mdc-1.9.0/test/sections/appendix1.md
+-rw-r--r--   0        0        0     1624 2023-07-26 03:43:17.631105 shiny_mdc-1.9.0/test/sections/appendix2.md
+-rw-r--r--   0        0        0        0 2023-07-26 03:43:17.631105 shiny_mdc-1.9.0/test/sections/empty.md
+-rw-r--r--   0        0        0     2326 2023-07-26 03:43:17.631105 shiny_mdc-1.9.0/test/sections/main1.md
+-rw-r--r--   0        0        0     1351 2023-07-26 03:43:17.631105 shiny_mdc-1.9.0/test/sections/main2.md
+-rw-r--r--   0        0        0      992 2023-07-26 03:43:17.631105 shiny_mdc-1.9.0/test/utils/commands.md
+-rw-r--r--   0        0        0       41 2023-07-26 03:43:17.631105 shiny_mdc-1.9.0/test/utils/ext.md
+-rw-r--r--   0        0        0     1043 1970-01-01 00:00:00.000000 shiny_mdc-1.9.0/PKG-INFO
```

### Comparing `shiny_mdc-1.8.0/CHANGELOG.md` & `shiny_mdc-1.9.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+## [1.9.0](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.8.0...v1.9.0) (2023-07-26)
+
+
+### Features
+
+* allow specifying pdf engine ([52d2b46](https://github.com/jayanthkoushik/shiny-mdc/commit/52d2b462628c8e4913f2dbc06ac187a2fad17330))
+* use abbrvnat for stylish template ([79e3789](https://github.com/jayanthkoushik/shiny-mdc/commit/79e37893c8e7cce6c5f47ac47d56013faf346625))
+
 ## [1.8.0](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.7.1...v1.8.0) (2023-07-23)
 
 
 ### Features
 
 * add options for strict and forced modes ([79f96b0](https://github.com/jayanthkoushik/shiny-mdc/commit/79f96b0ddd6d4a90b9ae2737a2b85e18d2ee01f9))
 * add resource to setup pdf metadata ([ad14fbc](https://github.com/jayanthkoushik/shiny-mdc/commit/ad14fbc47d3cd80b40dd7a3e29a8c9ec667a4221))
```

### Comparing `shiny_mdc-1.8.0/LICENSE` & `shiny_mdc-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/pyproject.toml` & `shiny_mdc-1.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shiny-mdc"
-version = "1.8.0"  # managed by `poetry-dynamic-versioning`
+version = "1.9.0"  # managed by `poetry-dynamic-versioning`
 description = "Tool to compile markdown files to tex/pdf using pandoc, latexmk"
 readme = "README.md"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 repository = "https://github.com/jayanthkoushik/shinymdc"
 packages = [
   { include = "shinymdc" }
```

### Comparing `shiny_mdc-1.8.0/shinymdc/_latexmk.py` & `shiny_mdc-1.9.0/shinymdc/_latexmk.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 import subprocess
 import sys
 from pathlib import Path
+from typing import Literal
 
 
 def run_latexmk(
     input_path: Path,
     build_dir: Path,
+    pdf_engine: Literal["pdflatex", "lualatex", "xelatex"],
     clean: bool = False,
     verbose: bool = False,
     force: bool = False,
     strict: bool = False,
 ) -> Path:
     """Compile a LaTeX file using `latexmk`.
 
     Args:
         input_path: Path to input file.
         build_dir: Path to build directory.
+        pdf_engine: PDF engine to use.
         clean: Whether to do a clean build by passing `-gg` to `latexmk`.
         verbose: Whether to enable verbose output.
         force: Whether to pass `-f` to `latexmk`.
         strict: Whether to pass `-Werror` to `latexmk`.
 
     Returns:
         Path to output file.
 
     Raises:
         subprocess.CalledProcessError: If `latexmk` subprocess fails.
     """
-    cmd = ["latexmk", "-pdf", "-interaction=nonstopmode", "-lualatex"]
+    cmd = ["latexmk", "-interaction=nonstopmode"]
+
+    if pdf_engine == "pdflatex":
+        cmd.append("-pdf")
+    elif pdf_engine in ("lualatex", "xelatex"):
+        cmd.append(f"-{pdf_engine}")
+    else:
+        raise ValueError(
+            f"invalid pdf engine (expected 'pdflatex/lualatex/xelatex'): "
+            f"{pdf_engine}"
+        )
 
     if clean:
         cmd.append("-gg")
     if not verbose:
         cmd.append("-silent")
     if force:
         cmd.append("-f")
```

### Comparing `shiny_mdc-1.8.0/shinymdc/_liquid.py` & `shiny_mdc-1.9.0/shinymdc/_liquid.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/_pandoc.py` & `shiny_mdc-1.9.0/shinymdc/_pandoc.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/_templates.py` & `shiny_mdc-1.9.0/shinymdc/_templates.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/resources/dynamic/authsetup.tex` & `shiny_mdc-1.9.0/shinymdc/resources/dynamic/authsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/resources/dynamic/dblfloatsetup.tex` & `shiny_mdc-1.9.0/shinymdc/resources/dynamic/dblfloatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/resources/static/bibsupersetup.tex` & `shiny_mdc-1.9.0/shinymdc/resources/static/bibsupersetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/resources/static/floatsetup.tex` & `shiny_mdc-1.9.0/shinymdc/resources/static/floatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/resources/static/iccv/bibstyle.bst` & `shiny_mdc-1.9.0/shinymdc/resources/static/iccv/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/resources/static/iccv/esopic.sty` & `shiny_mdc-1.9.0/shinymdc/resources/static/iccv/esopic.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/resources/static/iccv/everyshi.sty` & `shiny_mdc-1.9.0/shinymdc/resources/static/iccv/everyshi.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/resources/static/iccv/iccv.sty` & `shiny_mdc-1.9.0/shinymdc/resources/static/iccv/iccv.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/resources/static/iclr/bibstyle.bst` & `shiny_mdc-1.9.0/shinymdc/resources/static/iclr/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/resources/static/iclr/iclr.sty` & `shiny_mdc-1.9.0/shinymdc/resources/static/iclr/iclr.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/resources/static/iclr/mathcommands.tex` & `shiny_mdc-1.9.0/shinymdc/resources/static/iclr/mathcommands.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/resources/static/icml/bibstyle.bst` & `shiny_mdc-1.9.0/shinymdc/resources/static/icml/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/resources/static/icml/icml.sty` & `shiny_mdc-1.9.0/shinymdc/resources/static/icml/icml.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/resources/static/mathsetup.tex` & `shiny_mdc-1.9.0/shinymdc/resources/static/mathsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/resources/static/miscsetup.tex` & `shiny_mdc-1.9.0/shinymdc/resources/static/miscsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/resources/static/neurips/neurips.sty` & `shiny_mdc-1.9.0/shinymdc/resources/static/neurips/neurips.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/shinymdc.py` & `shiny_mdc-1.9.0/shinymdc/shinymdc.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,17 @@
         Annotated[
             Path,
             "output file (will write to standard output if not specified)",
             ["-o", "--output"],
         ]
     ]
 
+    pdf_engine: Annotated[
+        Literal["pdflatex", "lualatex", "xelatex"], "engine for generating pdf",
+    ] = "lualatex"
     template: Annotated[
         Template,
         f"LaTeX template (path to custom template file, or name of a builtin "
         f"template: {'/'.join(BuiltinTemplate.BUILTIN_TEMPLATE_NAMES)})",
         ["-t", "--template"],
     ] = BuiltinTemplate("basic")
 
@@ -475,14 +478,15 @@
         # Compile main tex with latexmk.
         latexmk_build_dir = self.build_dir / "latexmk"
         print(f"+ mkdir -p '{latexmk_build_dir}'", file=sys.stderr)
         latexmk_build_dir.mkdir(exist_ok=True)
         result_path = run_latexmk(
             self.main_tex_path,
             latexmk_build_dir,
+            self.pdf_engine,
             hasattr(self, "clean"),
             hasattr(self, "verbose"),
             hasattr(self, "force"),
             hasattr(self, "strict"),
         )
 
         # Copy result to output file or write it to stdout.
```

### Comparing `shiny_mdc-1.8.0/shinymdc/templates/basic.tex` & `shiny_mdc-1.9.0/shinymdc/templates/basic.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/templates/iccv.tex` & `shiny_mdc-1.9.0/shinymdc/templates/iccv.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/templates/iclr.tex` & `shiny_mdc-1.9.0/shinymdc/templates/iclr.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/templates/icml.tex` & `shiny_mdc-1.9.0/shinymdc/templates/icml.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/templates/neurips.tex` & `shiny_mdc-1.9.0/shinymdc/templates/neurips.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/templates/spacious.tex` & `shiny_mdc-1.9.0/shinymdc/templates/spacious.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/shinymdc/templates/stylish.tex` & `shiny_mdc-1.9.0/shinymdc/templates/stylish.tex`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
 $for(sections)$
 $it$
 $endfor$
 
 $if(bibliography)$
 \footnotesize
-\bibliographystyle{unsrtnat}
+\bibliographystyle{abbrvnat}
 \bibliography{$bibliography$}
 \normalsize
 $endif$
 
 \input{$addappendices$}
 
 \end{document}
```

### Comparing `shiny_mdc-1.8.0/test/figures/anscombe.pdf` & `shiny_mdc-1.9.0/test/figures/anscombe.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/figures/densities.pdf` & `shiny_mdc-1.9.0/test/figures/densities.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/figures/diamonds.pdf` & `shiny_mdc-1.9.0/test/figures/diamonds.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/figures/gaussian2d.pdf` & `shiny_mdc-1.9.0/test/figures/gaussian2d.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/figures/lines.png` & `shiny_mdc-1.9.0/test/figures/lines.png`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/main.md` & `shiny_mdc-1.9.0/test/main.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 ---
 title: "shinymdc-test"
 subtitle: Document to Test 'shinymdc' Features and Templates
 author:
 - name: Author One
   affiliation:
-  - 1
+  - $\bm{\dag}$
   equalcontrib: True
   email: 'author1@institute1.edu'
 - name: Author MiddleName Two
   affiliation:
-  - 1
-  - 2
+  - $\bm{\dag}$
+  - $\bm{\ddag}$
   equalcontrib: True
   email: 'authortwo@institute1.edu'
 - name: Author
   equalcontrib: True
 - name: Author Four
   email: 'author4@author4.com'
 - name: Author Number Five
   email: 'authornumberfive@institutetwo.edu'
   affiliation:
-  - 2
+  - $\bm{\ddag}$
 institute:
-- id: 1
+- id: $\bm{\dag}$
   name: Institute One
-- id: 2
+- id: $\bm{\ddag}$
   name: Institute Two at City, State
 abstract: _Markdown_ **in** **_abstract_**. $x+2$. @sec:ex1. Reference[@texbook].
 bibliography: references.bib
 sections:
 - sections/main1.md
 - sections/main2.md
 - sections/empty.md
```

### Comparing `shiny_mdc-1.8.0/test/references.bib` & `shiny_mdc-1.9.0/test/references.bib`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/samples/basic.pdf` & `shiny_mdc-1.9.0/test/samples/basic.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/samples/iccv.pdf` & `shiny_mdc-1.9.0/test/samples/iccv.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/samples/iclr.pdf` & `shiny_mdc-1.9.0/test/samples/iclr.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/samples/icml.pdf` & `shiny_mdc-1.9.0/test/samples/icml.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/samples/neurips.pdf` & `shiny_mdc-1.9.0/test/samples/neurips.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/samples/spacious.pdf` & `shiny_mdc-1.9.0/test/samples/spacious.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/samples/standalone.pdf` & `shiny_mdc-1.9.0/test/samples/standalone.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/samples/stylish.pdf` & `shiny_mdc-1.9.0/test/samples/stylish.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/sections/appendix1.md` & `shiny_mdc-1.9.0/test/sections/appendix1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/sections/appendix2.md` & `shiny_mdc-1.9.0/test/sections/appendix2.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/sections/main1.md` & `shiny_mdc-1.9.0/test/sections/main1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/sections/main2.md` & `shiny_mdc-1.9.0/test/sections/main2.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/test/utils/commands.md` & `shiny_mdc-1.9.0/test/utils/commands.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.8.0/PKG-INFO` & `shiny_mdc-1.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shiny-mdc
-Version: 1.8.0
+Version: 1.9.0
 Summary: Tool to compile markdown files to tex/pdf using pandoc, latexmk
 Home-page: https://github.com/jayanthkoushik/shinymdc
 License: MIT
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```


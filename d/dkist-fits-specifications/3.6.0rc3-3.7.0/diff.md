# Comparing `tmp/dkist_fits_specifications-3.6.0rc3.tar.gz` & `tmp/dkist_fits_specifications-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_fits_specifications-3.6.0rc3.tar", last modified: Wed Apr 19 19:59:51 2023, max compression
+gzip compressed data, was "dkist_fits_specifications-3.7.0.tar", last modified: Wed Jul 26 20:08:05 2023, max compression
```

## Comparing `dkist_fits_specifications-3.6.0rc3.tar` & `dkist_fits_specifications-3.7.0.tar`

### file list

```diff
@@ -1,99 +1,98 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.722378 dkist_fits_specifications-3.6.0rc3/
--rw-rw-rw-   0 root         (0) root         (0)     3334 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      676 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     4276 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     6509 2023-04-19 19:59:51.722378 dkist_fits_specifications-3.6.0rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6089 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.710378 dkist_fits_specifications-3.6.0rc3/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/changelog/35.spec_change.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.710378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/py.typed
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.714378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/
--rw-rw-rw-   0 root         (0) root         (0)     3584 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.714378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/ao.yml
--rw-rw-rw-   0 root         (0) root         (0)     2951 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/camera.yml
--rw-rw-rw-   0 root         (0) root         (0)      477 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/compression.yml
--rw-rw-rw-   0 root         (0) root         (0)    10244 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/cryonirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     1466 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/dkist-id.yml
--rw-rw-rw-   0 root         (0) root         (0)     4395 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/dlnirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     1709 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/fits.yml
--rw-rw-rw-   0 root         (0) root         (0)     1934 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/pac.yml
--rw-rw-rw-   0 root         (0) root         (0)     2653 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/telescope.yml
--rw-rw-rw-   0 root         (0) root         (0)      930 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/vbi.yml
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/visp.yml
--rw-rw-rw-   0 root         (0) root         (0)     2299 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/vtf.yml
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/wfc.yml
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/ws.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.714378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/
--rw-rw-rw-   0 root         (0) root         (0)    11880 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3117 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/level0.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.718378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/
--rw-rw-rw-   0 root         (0) root         (0)     1811 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/ao.yml
--rw-rw-rw-   0 root         (0) root         (0)     5886 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/camera.yml
--rw-rw-rw-   0 root         (0) root         (0)     6341 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/compression.yml
--rw-rw-rw-   0 root         (0) root         (0)    13479 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/cryonirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     3955 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/datacenter.yml
--rw-rw-rw-   0 root         (0) root         (0)     4144 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/dataset.yml
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/dkist-id.yml
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/dkist-op.yml
--rw-rw-rw-   0 root         (0) root         (0)     8355 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/dlnirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     7276 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/fits.yml
--rw-rw-rw-   0 root         (0) root         (0)     2304 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/pac.yml
--rw-rw-rw-   0 root         (0) root         (0)      778 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/stats.yml
--rw-rw-rw-   0 root         (0) root         (0)     7410 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/telescope.yml
--rw-rw-rw-   0 root         (0) root         (0)     2085 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/vbi.yml
--rw-rw-rw-   0 root         (0) root         (0)     2939 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/visp.yml
--rw-rw-rw-   0 root         (0) root         (0)     3660 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/vtf.yml
--rw-rw-rw-   0 root         (0) root         (0)     1483 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/wfc.yml
--rw-rw-rw-   0 root         (0) root         (0)     1310 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/ws.yml
--rw-rw-rw-   0 root         (0) root         (0)     1001 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/spec214_full_schema.yml
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec_validation_schema.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.718378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1044 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/test_122.py
--rw-rw-rw-   0 root         (0) root         (0)     2687 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/test_214.py
--rw-rw-rw-   0 root         (0) root         (0)     2808 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/test_expansions.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/test_level0_214.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.718378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3374 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/formatter.py
--rw-rw-rw-   0 root         (0) root         (0)     1222 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/frozendict.py
--rw-rw-rw-   0 root         (0) root         (0)     4782 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/spec.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.718378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/sphinx/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/sphinx/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8553 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/sphinx/spec_table.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-04-19 19:59:51.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.714378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6509 2023-04-19 19:59:51.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3370 2023-04-19 19:59:51.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-19 19:59:51.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-19 19:59:51.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-04-19 19:59:51.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-19 19:59:51.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.722378 dkist_fits_specifications-3.6.0rc3/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      872 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3424 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/level_one.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/reference.rst
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/release_history.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.722378 dkist_fits_specifications-3.6.0rc3/docs/specs/
--rw-rw-rw-   0 root         (0) root         (0)     1463 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/specs/spec-122.rst
--rw-rw-rw-   0 root         (0) root         (0)     2668 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/specs/spec-214.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.722378 dkist_fits_specifications-3.6.0rc3/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/licenses/TEMPLATE_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2030 2023-04-19 19:59:51.722378 dkist_fits_specifications-3.6.0rc3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      612 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1327 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)     3334 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      676 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4882 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     6507 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6089 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.541564 dkist_fits_specifications-3.7.0/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.541564 dkist_fits_specifications-3.7.0/dkist_fits_specifications/
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/py.typed
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.541564 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.545564 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/ao.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/camera.yml
+-rw-rw-rw-   0 root         (0) root         (0)      515 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/compression.yml
+-rw-rw-rw-   0 root         (0) root         (0)    10244 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/cryonirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/dkist-id.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4395 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/dlnirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/fits.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/pac.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2653 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/telescope.yml
+-rw-rw-rw-   0 root         (0) root         (0)      930 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/vbi.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/visp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/vtf.yml
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/wfc.yml
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/ws.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.545564 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/
+-rw-rw-rw-   0 root         (0) root         (0)    11880 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3117 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/level0.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.545564 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/ao.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5886 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/camera.yml
+-rw-rw-rw-   0 root         (0) root         (0)     6506 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/compression.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13479 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/cryonirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/datacenter.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4144 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/dataset.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/dkist-id.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/dkist-op.yml
+-rw-rw-rw-   0 root         (0) root         (0)     8355 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/dlnirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     7276 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/fits.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/pac.yml
+-rw-rw-rw-   0 root         (0) root         (0)      778 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/stats.yml
+-rw-rw-rw-   0 root         (0) root         (0)     7410 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/telescope.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2085 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/vbi.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2939 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/visp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3660 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/vtf.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/wfc.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/ws.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/spec214_full_schema.yml
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec_validation_schema.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/test_122.py
+-rw-rw-rw-   0 root         (0) root         (0)     2687 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/test_214.py
+-rw-rw-rw-   0 root         (0) root         (0)     2808 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/test_expansions.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/test_level0_214.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3374 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1222 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/frozendict.py
+-rw-rw-rw-   0 root         (0) root         (0)     4799 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/spec.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/sphinx/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/sphinx/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8553 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/sphinx/spec_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-07-26 20:08:05.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.541564 dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6507 2023-07-26 20:08:05.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2023-07-26 20:08:05.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 20:08:05.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 20:08:05.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-07-26 20:08:05.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-26 20:08:05.000000 dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      872 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3424 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/level_one.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/reference.rst
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/release_history.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/docs/specs/
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/specs/spec-122.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2668 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/docs/specs/spec-214.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-07-26 20:08:05.549564 dkist_fits_specifications-3.7.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      612 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2023-07-26 20:07:47.000000 dkist_fits_specifications-3.7.0/tox.ini
```

### Comparing `dkist_fits_specifications-3.6.0rc3/.gitignore` & `dkist_fits_specifications-3.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/.pre-commit-config.yaml` & `dkist_fits_specifications-3.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/CHANGELOG.rst` & `dkist_fits_specifications-3.7.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+v3.7.0 (2023-07-26)
+===================
+
+Backwards Compatible Changes to the Specification
+-------------------------------------------------
+
+- Adding the FITS standard key `ZBLANK` (`#36 <https://bitbucket.org/dkistdc/dkist-fits-specifications/pull-requests/36>`__)
+
+
+v3.6.0 (2023-04-24)
+===================
+
+Backwards Compatible Changes to the Specification
+-------------------------------------------------
+
+- Add `VBINMOSC` and `VBICMOSC` keys that encode the total number of and current mosaic repeat in VBI data. (`#35 <https://bitbucket.org/dkistdc/dkist-fits-specifications/pull-requests/35>`__)
+
+
 v3.5.0 (2023-04-10)
 ===================
 
 Backwards Compatible Changes to the Specification
 -------------------------------------------------
 
 - Added `NSPECLNS` and `SPECLN<sl>` keys to support inclusion of spectral line information. (`#34 <https://bitbucket.org/dkistdc/dkist-fits-specifications/pull-requests/34>`__)
```

### Comparing `dkist_fits_specifications-3.6.0rc3/PKG-INFO` & `dkist_fits_specifications-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dkist_fits_specifications
-Version: 3.6.0rc3
+Version: 3.7.0
 Summary: Machine readable FITS specifications for DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-fits-specifications/src/main/
 Author: AURA/NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 License-File: licenses/LICENSE.rst
 
 Machine readable FITS specifications for DKIST data.
 ----------------------------------------------------
```

### Comparing `dkist_fits_specifications-3.6.0rc3/README.rst` & `dkist_fits_specifications-3.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/bitbucket-pipelines.yml` & `dkist_fits_specifications-3.7.0/bitbucket-pipelines.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-image: python:3.9
+image: python:3.10
 
 definitions:
   steps:
     - step: &lint
         caches:
           - pip
         name: Lint
@@ -20,15 +20,15 @@
           - git remote set-branches --add origin main
           - git fetch origin main
           - towncrier check --compare-with origin/main
     - step: &test
         name: Test
         script:
           - pip install tox
-          - tox -e py39
+          - tox -e py310
     - step: &docs
         name: Docs
         script:
           - apt-get update
           - apt-get install -y graphviz
           - pip install tox
           - tox -e build_docs
```

### Comparing `dkist_fits_specifications-3.6.0rc3/check_changelog_updated.sh` & `dkist_fits_specifications-3.7.0/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/__init__.py` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/__init__.py` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/ao.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/ao.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/camera.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/camera.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/cryonirsp.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/cryonirsp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/dkist-id.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/dkist-id.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/dlnirsp.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/dlnirsp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/fits.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/fits.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/pac.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/pac.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/telescope.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/telescope.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/vbi.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/vbi.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/visp.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/visp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/vtf.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/vtf.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/wfc.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/wfc.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/ws.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec122/schemas/ws.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/__init__.py` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/level0.py` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/level0.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/ao.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/ao.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/camera.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/camera.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/compression.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/compression.yml`

 * *Files 5% similar despite different names*

```diff
@@ -390,8 +390,18 @@
 00001850: 7261 6374 6572 2073 7472 696e 6720 6769  racter string gi
 00001860: 7669 6e67 2074 6865 206e 616d 6520 6f66  ving the name of
 00001870: 2046 6965 6c64 206e 2e22 0a20 2066 6974   Field n.".  fit
 00001880: 7372 6566 6572 656e 6365 3a20 2237 2e33  sreference: "7.3
 00001890: 3a20 4269 6e61 7279 2054 6162 6c65 2045  : Binary Table E
 000018a0: 7874 656e 7369 6f6e 220a 2020 6578 7061  xtension".  expa
 000018b0: 6e64 3a20 7472 7565 0a20 2074 7970 653a  nd: true.  type:
-000018c0: 2073 7472 0a                              str.
+000018c0: 2073 7472 0a5a 424c 414e 4b3a 0a20 2064   str.ZBLANK:.  d
+000018d0: 6573 6372 6970 7469 6f6e 3a20 2257 6865  escription: "Whe
+000018e0: 6e20 7072 6573 656e 742c 2074 6869 7320  n present, this 
+000018f0: 6865 6164 6572 2073 6861 6c6c 2062 6520  header shall be 
+00001900: 7573 6564 2074 6f20 7374 6f72 6520 7468  used to store th
+00001910: 6520 696e 7465 6765 7220 7661 6c75 6520  e integer value 
+00001920: 7468 6174 2072 6570 7265 7365 6e74 7320  that represents 
+00001930: 756e 6465 6669 6e65 6420 7069 7865 6c73  undefined pixels
+00001940: 2069 6e20 7468 6520 7363 616c 6564 2069   in the scaled i
+00001950: 6e74 6567 6572 2061 7272 6179 220a 2020  nteger array".  
+00001960: 7479 7065 3a20 696e 740a                 type: int.
```

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/cryonirsp.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/cryonirsp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/datacenter.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/datacenter.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/dataset.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/dataset.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/dkist-id.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/dkist-id.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/dkist-op.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/dkist-op.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/dlnirsp.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/dlnirsp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/fits.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/fits.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/pac.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/pac.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/stats.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/stats.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/telescope.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/telescope.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/vbi.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/vbi.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/visp.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/visp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/vtf.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/vtf.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/wfc.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/wfc.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/ws.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/schemas/ws.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/spec214_full_schema.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec214/spec214_full_schema.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec_validation_schema.yml` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/spec_validation_schema.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/test_122.py` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/test_122.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/test_214.py` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/test_214.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/test_expansions.py` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/tests/test_expansions.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/formatter.py` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/frozendict.py` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/frozendict.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/spec.py` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         glob = "*"
 
     files = Path(base_path).glob(f"{glob}.yml")
 
     raw_schemas = {}
     for fname in files:
         schema_name = fname.stem
-        with open(fname) as fobj:
+        with open(fname, encoding="utf8") as fobj:
             raw_schema = tuple(yaml.load_all(fobj, Loader=yaml.SafeLoader))
 
             # Because this function is cached, we want to strongly discourage
             # modification of the return values. We do this by wrapping the
             # expected tree of dicts into frozendict objects which disallow
             # modification
             frozen_header = {}
```

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/sphinx/spec_table.py` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications/utils/sphinx/spec_table.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/PKG-INFO` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dkist-fits-specifications
-Version: 3.6.0rc3
+Version: 3.7.0
 Summary: Machine readable FITS specifications for DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-fits-specifications/src/main/
 Author: AURA/NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 License-File: licenses/LICENSE.rst
 
 Machine readable FITS specifications for DKIST data.
 ----------------------------------------------------
```

### Comparing `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/SOURCES.txt` & `dkist_fits_specifications-3.7.0/dkist_fits_specifications.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 changelog/.gitempty
-changelog/35.spec_change.rst
 dkist_fits_specifications/__init__.py
 dkist_fits_specifications/py.typed
 dkist_fits_specifications/spec_validation_schema.yml
 dkist_fits_specifications/version.py
 dkist_fits_specifications.egg-info/PKG-INFO
 dkist_fits_specifications.egg-info/SOURCES.txt
 dkist_fits_specifications.egg-info/dependency_links.txt
```

### Comparing `dkist_fits_specifications-3.6.0rc3/docs/Makefile` & `dkist_fits_specifications-3.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/docs/conf.py` & `dkist_fits_specifications-3.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/docs/index.rst` & `dkist_fits_specifications-3.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/docs/level_one.rst` & `dkist_fits_specifications-3.7.0/docs/level_one.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/docs/make.bat` & `dkist_fits_specifications-3.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/docs/specs/spec-122.rst` & `dkist_fits_specifications-3.7.0/docs/specs/spec-122.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/docs/specs/spec-214.rst` & `dkist_fits_specifications-3.7.0/docs/specs/spec-214.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/licenses/LICENSE.rst` & `dkist_fits_specifications-3.7.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/licenses/TEMPLATE_LICENSE.rst` & `dkist_fits_specifications-3.7.0/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/pyproject.toml` & `dkist_fits_specifications-3.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/setup.cfg` & `dkist_fits_specifications-3.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 description = Machine readable FITS specifications for DKIST data.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 
 [options]
 zip_safe = False
 packages = find:
-python_requires = >=3.9
+python_requires = >=3.10
 setup_requires = setuptools_scm
 include_package_data = true
 install_requires = 
 	yamale
 	pyyaml
 	astropy
```

### Comparing `dkist_fits_specifications-3.6.0rc3/setup.py` & `dkist_fits_specifications-3.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc3/tox.ini` & `dkist_fits_specifications-3.7.0/tox.ini`

 * *Files identical despite different names*


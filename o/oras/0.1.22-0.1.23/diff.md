# Comparing `tmp/oras-0.1.22.tar.gz` & `tmp/oras-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oras-0.1.22.tar", last modified: Sat Jul 22 14:49:15 2023, max compression
+gzip compressed data, was "oras-0.1.23.tar", last modified: Wed Jul 26 12:07:48 2023, max compression
```

## Comparing `oras-0.1.22.tar` & `oras-0.1.23.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:49:15.163141 oras-0.1.22/
--rw-r--r--   0 runner    (1001) docker     (122)    11343 2023-07-22 14:48:49.000000 oras-0.1.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-22 14:48:49.000000 oras-0.1.22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6440 2023-07-22 14:49:15.163141 oras-0.1.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5596 2023-07-22 14:48:49.000000 oras-0.1.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:49:15.155141 oras-0.1.22/oras/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-22 14:48:49.000000 oras-0.1.22/oras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-07-22 14:48:49.000000 oras-0.1.22/oras/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-07-22 14:48:49.000000 oras-0.1.22/oras/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3812 2023-07-22 14:48:49.000000 oras-0.1.22/oras/container.py
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-22 14:48:49.000000 oras-0.1.22/oras/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-22 14:48:49.000000 oras-0.1.22/oras/defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)     8737 2023-07-22 14:48:49.000000 oras-0.1.22/oras/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:49:15.159141 oras-0.1.22/oras/main/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-22 14:48:49.000000 oras-0.1.22/oras/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-22 14:48:49.000000 oras-0.1.22/oras/main/login.py
--rw-r--r--   0 runner    (1001) docker     (122)     4470 2023-07-22 14:48:49.000000 oras-0.1.22/oras/oci.py
--rw-r--r--   0 runner    (1001) docker     (122)    35967 2023-07-22 14:48:49.000000 oras-0.1.22/oras/provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-07-22 14:48:49.000000 oras-0.1.22/oras/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:49:15.163141 oras-0.1.22/oras/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-22 14:48:49.000000 oras-0.1.22/oras/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-22 14:48:49.000000 oras-0.1.22/oras/tests/annotations.json
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-22 14:48:49.000000 oras-0.1.22/oras/tests/artifact.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      185 2023-07-22 14:48:49.000000 oras-0.1.22/oras/tests/run_registry.sh
--rw-r--r--   0 runner    (1001) docker     (122)     5066 2023-07-22 14:48:49.000000 oras-0.1.22/oras/tests/test_oras.py
--rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-07-22 14:48:49.000000 oras-0.1.22/oras/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-07-22 14:48:49.000000 oras-0.1.22/oras/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:49:15.163141 oras-0.1.22/oras/tests/upload_data/
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-22 14:48:49.000000 oras-0.1.22/oras/tests/upload_data/artifact.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:49:15.163141 oras-0.1.22/oras/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-22 14:48:49.000000 oras-0.1.22/oras/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10818 2023-07-22 14:48:49.000000 oras-0.1.22/oras/utils/fileio.py
--rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-07-22 14:48:49.000000 oras-0.1.22/oras/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (122)      985 2023-07-22 14:48:49.000000 oras-0.1.22/oras/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:49:15.159141 oras-0.1.22/oras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6440 2023-07-22 14:49:14.000000 oras-0.1.22/oras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-22 14:49:15.000000 oras-0.1.22/oras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-22 14:49:14.000000 oras-0.1.22/oras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-22 14:49:10.000000 oras-0.1.22/oras.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-22 14:49:14.000000 oras-0.1.22/oras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-22 14:49:14.000000 oras-0.1.22/oras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-22 14:48:49.000000 oras-0.1.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-07-22 14:49:15.163141 oras-0.1.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3370 2023-07-22 14:48:49.000000 oras-0.1.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 12:07:48.202710 oras-0.1.23/
+-rw-r--r--   0 runner    (1001) docker     (122)    11343 2023-07-26 12:07:13.000000 oras-0.1.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-26 12:07:13.000000 oras-0.1.23/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6778 2023-07-26 12:07:48.202710 oras-0.1.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5934 2023-07-26 12:07:13.000000 oras-0.1.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 12:07:48.198710 oras-0.1.23/oras/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-26 12:07:13.000000 oras-0.1.23/oras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-07-26 12:07:13.000000 oras-0.1.23/oras/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-07-26 12:07:13.000000 oras-0.1.23/oras/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-07-26 12:07:13.000000 oras-0.1.23/oras/container.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-26 12:07:13.000000 oras-0.1.23/oras/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-26 12:07:13.000000 oras-0.1.23/oras/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8737 2023-07-26 12:07:13.000000 oras-0.1.23/oras/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 12:07:48.202710 oras-0.1.23/oras/main/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 12:07:13.000000 oras-0.1.23/oras/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-26 12:07:13.000000 oras-0.1.23/oras/main/login.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4470 2023-07-26 12:07:13.000000 oras-0.1.23/oras/oci.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36601 2023-07-26 12:07:13.000000 oras-0.1.23/oras/provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-07-26 12:07:13.000000 oras-0.1.23/oras/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 12:07:48.202710 oras-0.1.23/oras/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 12:07:13.000000 oras-0.1.23/oras/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-26 12:07:13.000000 oras-0.1.23/oras/tests/annotations.json
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-26 12:07:13.000000 oras-0.1.23/oras/tests/artifact.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      185 2023-07-26 12:07:13.000000 oras-0.1.23/oras/tests/run_registry.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     5066 2023-07-26 12:07:13.000000 oras-0.1.23/oras/tests/test_oras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-07-26 12:07:13.000000 oras-0.1.23/oras/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-07-26 12:07:13.000000 oras-0.1.23/oras/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 12:07:48.202710 oras-0.1.23/oras/tests/upload_data/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-26 12:07:13.000000 oras-0.1.23/oras/tests/upload_data/artifact.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 12:07:48.202710 oras-0.1.23/oras/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-26 12:07:13.000000 oras-0.1.23/oras/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10818 2023-07-26 12:07:13.000000 oras-0.1.23/oras/utils/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-07-26 12:07:13.000000 oras-0.1.23/oras/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      985 2023-07-26 12:07:13.000000 oras-0.1.23/oras/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 12:07:48.198710 oras-0.1.23/oras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6778 2023-07-26 12:07:48.000000 oras-0.1.23/oras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-26 12:07:48.000000 oras-0.1.23/oras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 12:07:48.000000 oras-0.1.23/oras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 12:07:44.000000 oras-0.1.23/oras.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-26 12:07:48.000000 oras-0.1.23/oras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-26 12:07:48.000000 oras-0.1.23/oras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-26 12:07:13.000000 oras-0.1.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-07-26 12:07:48.202710 oras-0.1.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3370 2023-07-26 12:07:13.000000 oras-0.1.23/setup.py
```

### Comparing `oras-0.1.22/LICENSE` & `oras-0.1.23/LICENSE`

 * *Files identical despite different names*

### Comparing `oras-0.1.22/PKG-INFO` & `oras-0.1.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oras
-Version: 0.1.22
+Version: 0.1.23
 Summary: OCI Registry as Storage Python SDK
 Home-page: https://github.com/oras-project/oras-py
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: oci,registry,storage
@@ -22,15 +22,15 @@
 Provides-Extra: tests
 Provides-Extra: docker
 License-File: LICENSE
 
 # ORAS Python
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-12-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-13-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ![ORAS Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/oras.png)
 
 OCI Registry as Storage enables libraries to push OCI Artifacts to [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries. This is a Python SDK for Python developers to empower them to do this in their applications.
 
 See our ⭐️ [Documentation](https://oras-project.github.io/oras-py/) ⭐️ to get started.
@@ -63,14 +63,15 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/shizhMSFT"><img src="https://avatars.githubusercontent.com/u/32161882?v=4?s=100" width="100px;" alt="Shiwei Zhang"/><br /><sub><b>Shiwei Zhang</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=shizhMSFT" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jhlmco"><img src="https://avatars.githubusercontent.com/u/126677738?v=4?s=100" width="100px;" alt="jhlmco"/><br /><sub><b>jhlmco</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=jhlmco" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ananya2003Gupta"><img src="https://avatars.githubusercontent.com/u/90386813?v=4?s=100" width="100px;" alt="Ananya Gupta"/><br /><sub><b>Ananya Gupta</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=Ananya2003Gupta" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sunnycarter"><img src="https://avatars.githubusercontent.com/u/36891339?v=4?s=100" width="100px;" alt="sunnycarter"/><br /><sub><b>sunnycarter</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=sunnycarter" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/mariusbertram"><img src="https://avatars.githubusercontent.com/u/10505884?v=4?s=100" width="100px;" alt="Marius Bertram"/><br /><sub><b>Marius Bertram</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=mariusbertram" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://dev-zero.ch"><img src="https://avatars.githubusercontent.com/u/11307?v=4?s=100" width="100px;" alt="Tiziano Müller"/><br /><sub><b>Tiziano Müller</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=dev-zero" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,35 +1,35 @@
-Metadata-Version: 2.1 Name: oras Version: 0.1.22 Summary: OCI Registry as
+Metadata-Version: 2.1 Name: oras Version: 0.1.23 Summary: OCI Registry as
 Storage Python SDK Home-page: https://github.com/oras-project/oras-py Author:
 Vanessa Sochat Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa
 Sochat License: LICENSE Keywords: oci,registry,storage Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
 Unix Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Description-Content-Type: text/markdown
 Provides-Extra: all Provides-Extra: tests Provides-Extra: docker License-File:
 LICENSE # ORAS Python  [![All Contributors](https://img.shields.io/badge/
-all_contributors-12-orange.svg?style=flat-square)](#contributors-)  ![ORAS
+all_contributors-13-orange.svg?style=flat-square)](#contributors-)  ![ORAS
 Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/
 oras.png) OCI Registry as Storage enables libraries to push OCI Artifacts to
 [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries.
 This is a Python SDK for Python developers to empower them to do this in their
 applications. See our â­ï¸ [Documentation](https://oras-project.github.io/
 oras-py/) â­ï¸ to get started. ## Code of Conduct Please note that this
 project has adopted the [CNCF Code of Conduct](https://github.com/cncf/
 foundation/blob/master/code-of-conduct.md). Please follow it in all your
 interactions with the project members and users. ## ðï¸ Contributors
 ðï¸ We use the [all-contributors](https://github.com/all-contributors/all-
 contributors) tool to generate a contributors graphic below.
-[Vanessasaurus] [Lachlan  [Steve      [Josh     [Bridget   [Matt      [Wolf
- Vanessasaurus  Evenson] Lasker]    Dolitsky]   Kromhout] Warner]  Vollprecht]
-     ð»   Lachlan   Steve   Josh_Dolitsky  Bridget    Matt      Wolf
-                Evenson   Lasker      ð»  Kromhout   Warner  Vollprecht
-                  ð�  ð»               ð»  ð�   ð»
-[Shiwei_Zhang]  [jhlmco] [Ananya  [sunnycarter]  [Marius
- Shiwei_Zhang    jhlmco   Gupta]   sunnycarter  Bertram]
-     ð»     ð� Ananya      ð»   Marius
+[Vanessasaurus] [Lachlan  [Steve      [Josh     [Bridget     [Matt_Warner]     [Wolf
+ Vanessasaurus  Evenson] Lasker]    Dolitsky]   Kromhout]     Matt_Warner   Vollprecht]
+     ð»   Lachlan   Steve   Josh_Dolitsky  Bridget         ð»      Wolf
+                Evenson   Lasker      ð»  Kromhout                    Vollprecht
+                  ð�  ð»               ð»                     ð»
+[Shiwei_Zhang]  [jhlmco] [Ananya  [sunnycarter]  [Marius  [Tiziano_MÃ¼ller]
+ Shiwei_Zhang    jhlmco   Gupta]   sunnycarter  Bertram]   Tiziano_MÃ¼ller
+     ð»     ð� Ananya      ð»   Marius         ð»
                           Gupta                  Bertram
                            ð»               ð»
    ## License This code is licensed under the Apache 2.0 [LICENSE](LICENSE).
```

### Comparing `oras-0.1.22/README.md` & `oras-0.1.23/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ORAS Python
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-12-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-13-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ![ORAS Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/oras.png)
 
 OCI Registry as Storage enables libraries to push OCI Artifacts to [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries. This is a Python SDK for Python developers to empower them to do this in their applications.
 
 See our ⭐️ [Documentation](https://oras-project.github.io/oras-py/) ⭐️ to get started.
@@ -38,14 +38,15 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/shizhMSFT"><img src="https://avatars.githubusercontent.com/u/32161882?v=4?s=100" width="100px;" alt="Shiwei Zhang"/><br /><sub><b>Shiwei Zhang</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=shizhMSFT" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jhlmco"><img src="https://avatars.githubusercontent.com/u/126677738?v=4?s=100" width="100px;" alt="jhlmco"/><br /><sub><b>jhlmco</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=jhlmco" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ananya2003Gupta"><img src="https://avatars.githubusercontent.com/u/90386813?v=4?s=100" width="100px;" alt="Ananya Gupta"/><br /><sub><b>Ananya Gupta</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=Ananya2003Gupta" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sunnycarter"><img src="https://avatars.githubusercontent.com/u/36891339?v=4?s=100" width="100px;" alt="sunnycarter"/><br /><sub><b>sunnycarter</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=sunnycarter" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/mariusbertram"><img src="https://avatars.githubusercontent.com/u/10505884?v=4?s=100" width="100px;" alt="Marius Bertram"/><br /><sub><b>Marius Bertram</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=mariusbertram" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://dev-zero.ch"><img src="https://avatars.githubusercontent.com/u/11307?v=4?s=100" width="100px;" alt="Tiziano Müller"/><br /><sub><b>Tiziano Müller</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=dev-zero" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
 # ORAS Python  [![All Contributors](https://img.shields.io/badge/
-all_contributors-12-orange.svg?style=flat-square)](#contributors-)  ![ORAS
+all_contributors-13-orange.svg?style=flat-square)](#contributors-)  ![ORAS
 Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/
 oras.png) OCI Registry as Storage enables libraries to push OCI Artifacts to
 [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries.
 This is a Python SDK for Python developers to empower them to do this in their
 applications. See our â­ï¸ [Documentation](https://oras-project.github.io/
 oras-py/) â­ï¸ to get started. ## Code of Conduct Please note that this
 project has adopted the [CNCF Code of Conduct](https://github.com/cncf/
 foundation/blob/master/code-of-conduct.md). Please follow it in all your
 interactions with the project members and users. ## ðï¸ Contributors
 ðï¸ We use the [all-contributors](https://github.com/all-contributors/all-
 contributors) tool to generate a contributors graphic below.
-[Vanessasaurus] [Lachlan  [Steve      [Josh     [Bridget   [Matt      [Wolf
- Vanessasaurus  Evenson] Lasker]    Dolitsky]   Kromhout] Warner]  Vollprecht]
-     ð»   Lachlan   Steve   Josh_Dolitsky  Bridget    Matt      Wolf
-                Evenson   Lasker      ð»  Kromhout   Warner  Vollprecht
-                  ð�  ð»               ð»  ð�   ð»
-[Shiwei_Zhang]  [jhlmco] [Ananya  [sunnycarter]  [Marius
- Shiwei_Zhang    jhlmco   Gupta]   sunnycarter  Bertram]
-     ð»     ð� Ananya      ð»   Marius
+[Vanessasaurus] [Lachlan  [Steve      [Josh     [Bridget     [Matt_Warner]     [Wolf
+ Vanessasaurus  Evenson] Lasker]    Dolitsky]   Kromhout]     Matt_Warner   Vollprecht]
+     ð»   Lachlan   Steve   Josh_Dolitsky  Bridget         ð»      Wolf
+                Evenson   Lasker      ð»  Kromhout                    Vollprecht
+                  ð�  ð»               ð»                     ð»
+[Shiwei_Zhang]  [jhlmco] [Ananya  [sunnycarter]  [Marius  [Tiziano_MÃ¼ller]
+ Shiwei_Zhang    jhlmco   Gupta]   sunnycarter  Bertram]   Tiziano_MÃ¼ller
+     ð»     ð� Ananya      ð»   Marius         ð»
                           Gupta                  Bertram
                            ð»               ð»
    ## License This code is licensed under the Apache 2.0 [LICENSE](LICENSE).
```

### Comparing `oras-0.1.22/oras/auth.py` & `oras-0.1.23/oras/auth.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.22/oras/client.py` & `oras-0.1.23/oras/client.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.22/oras/container.py` & `oras-0.1.23/oras/container.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,18 @@
         Get the manifest url for a specific tag, or the one for this container.
 
         The tag provided can also correspond to a digest.
 
         :param tag: an optional tag to provide (if not provided defaults to container)
         :type tag: None or str
         """
-        tag = tag or self.tag
+
+        # an explicitly defined tag has precedence over everything,
+        # but from the already defined ones, prefer the digest for consistency.
+        tag = tag or (self.digest or self.tag)
         return f"{self.registry}/v2/{self.api_prefix}/manifests/{tag}"
 
     def __str__(self) -> str:
         return self.uri
 
     @property
     def uri(self) -> str:
```

### Comparing `oras-0.1.22/oras/decorator.py` & `oras-0.1.23/oras/decorator.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.22/oras/defaults.py` & `oras-0.1.23/oras/defaults.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.22/oras/logger.py` & `oras-0.1.23/oras/logger.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.22/oras/main/login.py` & `oras-0.1.23/oras/main/login.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.22/oras/oci.py` & `oras-0.1.23/oras/oci.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.22/oras/provider.py` & `oras-0.1.23/oras/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 __author__ = "Vanessa Sochat"
 __copyright__ = "Copyright The ORAS Authors."
 __license__ = "Apache-2.0"
 
 import copy
 import os
 import urllib
+from dataclasses import asdict, dataclass
+from http.cookiejar import DefaultCookiePolicy
 from typing import Callable, List, Optional, Tuple, Union
 
 import jsonschema
 import requests
 
 import oras.auth
 import oras.container
@@ -19,14 +21,21 @@
 from oras.logger import logger
 from oras.utils.fileio import PathAndOptionalContent
 
 # container type can be string or container
 container_type = Union[str, oras.container.Container]
 
 
+@dataclass
+class Subject:
+    mediaType: str
+    digest: str
+    size: int
+
+
 class Registry:
     """
     Direct interactions with an OCI registry.
 
     This could also be called a "provider" when we add in the "copy" logic
     and the registry isn't necessarily the "remote" endpoint.
     """
@@ -55,14 +64,19 @@
         self._auths: dict = {}
         self._basic_auth = None
         self._tls_verify = tls_verify
 
         if not tls_verify:
             requests.packages.urllib3.disable_warnings()  # type: ignore
 
+        # Ignore all cookies: some registries try to set one
+        # and take it as a sign they are talking to a browser,
+        # trying to set further CSRF cookies (Harbor is such a case)
+        self.session.cookies.set_policy(DefaultCookiePolicy(allowed_domains=[]))
+
     def logout(self, hostname: str):
         """
         If auths are loaded, remove a hostname.
 
         :param hostname: the registry hostname to remove
         :type hostname: str
         """
@@ -631,14 +645,16 @@
         :type insecure: bool
         :param annotation_file: manifest annotations file
         :type annotation_file: str
         :param manifest_annotations: manifest annotations
         :type manifest_annotations: dict
         :param target: target location to push to
         :type target: str
+        :param subject: optional subject reference
+        :type subject: Subject
         """
         container = self.get_container(kwargs["target"])
         self.load_configs(container, configs=kwargs.get("config_path"))
 
         # Hold state of request for http/https
         validate_path = not kwargs.get("disable_path_validation", False)
 
@@ -708,14 +724,18 @@
         # These over-ride any potentially provided from file
         custom_annots = kwargs.get("manifest_annotations")
         if custom_annots:
             manifest_annots.update(custom_annots)
         if manifest_annots:
             manifest["annotations"] = manifest_annots
 
+        subject = kwargs.get("subject")
+        if subject:
+            manifest["subject"] = asdict(subject)
+
         # Prepare the manifest config (temporary or one provided)
         manifest_config = kwargs.get("manifest_config")
         config_annots = annotset.get_annotations("$config")
         if manifest_config:
             ref, media_type = self._parse_manifest_ref(manifest_config)
             conf, config_file = oras.oci.ManifestConfig(ref, media_type)
         else:
```

### Comparing `oras-0.1.22/oras/schemas.py` & `oras-0.1.23/oras/schemas.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 layer.update(layerProperties)
 
 
 # Manifest
 
 manifestProperties = {
     "schemaVersion": {"type": "number"},
-    "subject": {"type": ["null", "string"]},
+    "subject": {"type": ["null", "object"]},
     "mediaType": {"type": "string"},
     "layers": {"type": "array", "items": layerProperties},
     "config": layerProperties,
     "annotations": {"type": ["object", "null", "array"]},
 }
```

### Comparing `oras-0.1.22/oras/tests/test_oras.py` & `oras-0.1.23/oras/tests/test_oras.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.22/oras/tests/test_provider.py` & `oras-0.1.23/oras/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.22/oras/tests/test_utils.py` & `oras-0.1.23/oras/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.22/oras/utils/fileio.py` & `oras-0.1.23/oras/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.22/oras/utils/request.py` & `oras-0.1.23/oras/utils/request.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.22/oras/version.py` & `oras-0.1.23/oras/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Vanessa Sochat"
 __copyright__ = "Copyright The ORAS Authors."
 __license__ = "Apache-2.0"
 
-__version__ = "0.1.22"
+__version__ = "0.1.23"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "oras"
 PACKAGE_URL = "https://github.com/oras-project/oras-py"
 KEYWORDS = "oci, registry, storage"
 DESCRIPTION = "OCI Registry as Storage Python SDK"
 LICENSE = "LICENSE"
```

### Comparing `oras-0.1.22/oras.egg-info/PKG-INFO` & `oras-0.1.23/oras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oras
-Version: 0.1.22
+Version: 0.1.23
 Summary: OCI Registry as Storage Python SDK
 Home-page: https://github.com/oras-project/oras-py
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: oci,registry,storage
@@ -22,15 +22,15 @@
 Provides-Extra: tests
 Provides-Extra: docker
 License-File: LICENSE
 
 # ORAS Python
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-12-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-13-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ![ORAS Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/oras.png)
 
 OCI Registry as Storage enables libraries to push OCI Artifacts to [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries. This is a Python SDK for Python developers to empower them to do this in their applications.
 
 See our ⭐️ [Documentation](https://oras-project.github.io/oras-py/) ⭐️ to get started.
@@ -63,14 +63,15 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/shizhMSFT"><img src="https://avatars.githubusercontent.com/u/32161882?v=4?s=100" width="100px;" alt="Shiwei Zhang"/><br /><sub><b>Shiwei Zhang</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=shizhMSFT" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jhlmco"><img src="https://avatars.githubusercontent.com/u/126677738?v=4?s=100" width="100px;" alt="jhlmco"/><br /><sub><b>jhlmco</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=jhlmco" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ananya2003Gupta"><img src="https://avatars.githubusercontent.com/u/90386813?v=4?s=100" width="100px;" alt="Ananya Gupta"/><br /><sub><b>Ananya Gupta</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=Ananya2003Gupta" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sunnycarter"><img src="https://avatars.githubusercontent.com/u/36891339?v=4?s=100" width="100px;" alt="sunnycarter"/><br /><sub><b>sunnycarter</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=sunnycarter" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/mariusbertram"><img src="https://avatars.githubusercontent.com/u/10505884?v=4?s=100" width="100px;" alt="Marius Bertram"/><br /><sub><b>Marius Bertram</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=mariusbertram" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://dev-zero.ch"><img src="https://avatars.githubusercontent.com/u/11307?v=4?s=100" width="100px;" alt="Tiziano Müller"/><br /><sub><b>Tiziano Müller</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=dev-zero" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,35 +1,35 @@
-Metadata-Version: 2.1 Name: oras Version: 0.1.22 Summary: OCI Registry as
+Metadata-Version: 2.1 Name: oras Version: 0.1.23 Summary: OCI Registry as
 Storage Python SDK Home-page: https://github.com/oras-project/oras-py Author:
 Vanessa Sochat Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa
 Sochat License: LICENSE Keywords: oci,registry,storage Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
 Unix Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Description-Content-Type: text/markdown
 Provides-Extra: all Provides-Extra: tests Provides-Extra: docker License-File:
 LICENSE # ORAS Python  [![All Contributors](https://img.shields.io/badge/
-all_contributors-12-orange.svg?style=flat-square)](#contributors-)  ![ORAS
+all_contributors-13-orange.svg?style=flat-square)](#contributors-)  ![ORAS
 Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/
 oras.png) OCI Registry as Storage enables libraries to push OCI Artifacts to
 [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries.
 This is a Python SDK for Python developers to empower them to do this in their
 applications. See our â­ï¸ [Documentation](https://oras-project.github.io/
 oras-py/) â­ï¸ to get started. ## Code of Conduct Please note that this
 project has adopted the [CNCF Code of Conduct](https://github.com/cncf/
 foundation/blob/master/code-of-conduct.md). Please follow it in all your
 interactions with the project members and users. ## ðï¸ Contributors
 ðï¸ We use the [all-contributors](https://github.com/all-contributors/all-
 contributors) tool to generate a contributors graphic below.
-[Vanessasaurus] [Lachlan  [Steve      [Josh     [Bridget   [Matt      [Wolf
- Vanessasaurus  Evenson] Lasker]    Dolitsky]   Kromhout] Warner]  Vollprecht]
-     ð»   Lachlan   Steve   Josh_Dolitsky  Bridget    Matt      Wolf
-                Evenson   Lasker      ð»  Kromhout   Warner  Vollprecht
-                  ð�  ð»               ð»  ð�   ð»
-[Shiwei_Zhang]  [jhlmco] [Ananya  [sunnycarter]  [Marius
- Shiwei_Zhang    jhlmco   Gupta]   sunnycarter  Bertram]
-     ð»     ð� Ananya      ð»   Marius
+[Vanessasaurus] [Lachlan  [Steve      [Josh     [Bridget     [Matt_Warner]     [Wolf
+ Vanessasaurus  Evenson] Lasker]    Dolitsky]   Kromhout]     Matt_Warner   Vollprecht]
+     ð»   Lachlan   Steve   Josh_Dolitsky  Bridget         ð»      Wolf
+                Evenson   Lasker      ð»  Kromhout                    Vollprecht
+                  ð�  ð»               ð»                     ð»
+[Shiwei_Zhang]  [jhlmco] [Ananya  [sunnycarter]  [Marius  [Tiziano_MÃ¼ller]
+ Shiwei_Zhang    jhlmco   Gupta]   sunnycarter  Bertram]   Tiziano_MÃ¼ller
+     ð»     ð� Ananya      ð»   Marius         ð»
                           Gupta                  Bertram
                            ð»               ð»
    ## License This code is licensed under the Apache 2.0 [LICENSE](LICENSE).
```

### Comparing `oras-0.1.22/oras.egg-info/SOURCES.txt` & `oras-0.1.23/oras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oras-0.1.22/setup.py` & `oras-0.1.23/setup.py`

 * *Files identical despite different names*


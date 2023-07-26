# Comparing `tmp/jupyterlab_gitlab-3.0.0.tar.gz` & `tmp/jupyterlab_gitlab-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_gitlab-3.0.0.tar", last modified: Mon Aug 23 08:25:43 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterlab_gitlab-3.0.0.tar` & `jupyterlab_gitlab-4.0.0.tar`

### file list

```diff
@@ -1,55 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-23 08:25:43.504258 jupyterlab_gitlab-3.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1517 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      488 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7856 2021-08-23 08:25:43.504258 jupyterlab_gitlab-3.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6897 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      195 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/install.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-23 08:25:43.478256 jupyterlab_gitlab-3.0.0/jupyter-config/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-23 08:25:43.490257 jupyterlab_gitlab-3.0.0/jupyter-config/jupyter_notebook_config.d/
--rw-rw-rw-   0 root         (0) root         (0)       94 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/jupyter-config/jupyter_notebook_config.d/jupyterlab_gitlab.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-23 08:25:43.491257 jupyterlab_gitlab-3.0.0/jupyter-config/jupyter_server_config.d/
--rw-rw-rw-   0 root         (0) root         (0)       92 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/jupyter-config/jupyter_server_config.d/jupyterlab_gitlab.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-23 08:25:43.494257 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      868 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     5842 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/gitlab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-23 08:25:43.497258 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/
--rw-rw-rw-   0 root         (0) root         (0)     3467 2021-08-23 08:25:43.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-23 08:25:43.479256 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/schemas/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-23 08:25:43.498258 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/schemas/jupyterlab-gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      712 2021-08-23 08:25:39.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/schemas/jupyterlab-gitlab/drive.json
--rw-rw-rw-   0 root         (0) root         (0)     3325 2021-08-23 08:25:39.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/schemas/jupyterlab-gitlab/package.json.orig
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-23 08:25:43.500258 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/static/
--rw-r--r--   0 root         (0) root         (0)    12176 2021-08-23 08:25:43.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/static/392.b613df8f5a6e873d0ed2.js
--rw-r--r--   0 root         (0) root         (0)    12564 2021-08-23 08:25:43.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/static/534.2d174fa7be8b96a8c604.js
--rw-r--r--   0 root         (0) root         (0)     1491 2021-08-23 08:25:43.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/static/742.ee2a9c67f39dc93945ac.js
--rw-r--r--   0 root         (0) root         (0)     7716 2021-08-23 08:25:43.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/static/remoteEntry.a23f7c6fbcd0961ed640.js
--rw-r--r--   0 root         (0) root         (0)      160 2021-08-23 08:25:39.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/static/style.js
--rw-r--r--   0 root         (0) root         (0)     3680 2021-08-23 08:25:43.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-23 08:25:43.496258 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7856 2021-08-23 08:25:43.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1352 2021-08-23 08:25:43.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-23 08:25:43.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-23 08:24:22.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       23 2021-08-23 08:25:43.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2021-08-23 08:25:43.000000 jupyterlab_gitlab-3.0.0/jupyterlab_gitlab.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     3325 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/package.json
--rw-rw-rw-   0 root         (0) root         (0)      603 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-23 08:25:43.500258 jupyterlab_gitlab-3.0.0/schema/
--rw-rw-rw-   0 root         (0) root         (0)      712 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/schema/drive.json
--rw-rw-rw-   0 root         (0) root         (0)       73 2021-08-23 08:25:43.505258 jupyterlab_gitlab-3.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3411 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-23 08:25:43.502258 jupyterlab_gitlab-3.0.0/src/
--rw-rw-rw-   0 root         (0) root         (0)     9367 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/src/browser.ts
--rw-rw-rw-   0 root         (0) root         (0)    22339 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/src/contents.ts
--rw-rw-rw-   0 root         (0) root         (0)     5163 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/src/gitlab.ts
--rw-rw-rw-   0 root         (0) root         (0)     4287 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/src/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-23 08:25:43.504258 jupyterlab_gitlab-3.0.0/style/
--rw-rw-rw-   0 root         (0) root         (0)     2239 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/style/base.css
--rw-rw-rw-   0 root         (0) root         (0)     5067 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/style/gitlab-logo-extra-whitespace.svg
--rw-rw-rw-   0 root         (0) root         (0)     2767 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/style/gitlab_stacked_wm_grayscale.svg
--rw-rw-rw-   0 root         (0) root         (0)       25 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/style/index.css
--rw-rw-rw-   0 root         (0) root         (0)       21 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/style/index.js
--rw-rw-rw-   0 root         (0) root         (0)      554 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/tsconfig.json
--rw-rw-rw-   0 root         (0) root         (0)     2969 2021-08-23 08:22:54.000000 jupyterlab_gitlab-3.0.0/tslint.json
--rw-rw-rw-   0 root         (0) root         (0)   267126 2021-08-23 08:25:16.000000 jupyterlab_gitlab-3.0.0/yarn.lock
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/.eslintignore
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/.eslintrc.js
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/.flake8
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/.prettierignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/.prettierrc
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/.yarnrc.yml
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/RELEASE.md
+-rw-r--r--   0        0        0   318271 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/gitception.png
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/install.json
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/tsconfig.json
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/tslint.json
+-rw-r--r--   0        0        0   241463 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/yarn.lock
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/jupyter-config/jupyter_notebook_config.d/jupyterlab_gitlab.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/jupyter-config/jupyter_server_config.d/jupyterlab_gitlab.json
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/jupyter-config/nb-config/jupyterlab_gitlab.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/jupyter-config/server-config/jupyterlab_gitlab.json
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/_version.py
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/gitlab.py
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/labextension/package.json
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/labextension/schemas/jupyterlab-gitlab/drive.json
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/labextension/schemas/jupyterlab-gitlab/package.json.orig
+-rw-r--r--   0        0        0    15221 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/labextension/static/232.2729dbd8de27fb8601e1.js
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/labextension/static/742.ff0c6cd9a5a3198ebae4.js
+-rw-r--r--   0        0        0    13658 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/labextension/static/747.a85ac71c39deaa0e363e.js
+-rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/labextension/static/remoteEntry.b1ef8c77a08638c7aec5.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/labextension/static/style.js
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/schema/drive.json
+-rw-r--r--   0        0        0     9367 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/src/browser.ts
+-rw-r--r--   0        0        0    22782 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/src/contents.ts
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/src/gitlab.ts
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/src/index.ts
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/src/svg.d.ts
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/style/base.css
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/style/gitlab-logo-extra-whitespace.svg
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/style/gitlab_stacked_wm_grayscale.svg
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/style/index.js
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/.gitignore
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/LICENSE
+-rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/README.md
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 jupyterlab_gitlab-4.0.0/PKG-INFO
```

### Comparing `jupyterlab_gitlab-3.0.0/LICENSE` & `jupyterlab_gitlab-4.0.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 BSD 3-Clause License
 
-Copyright (c) 2021, Benjamin Bertrand All rights reserved.
+Copyright (c) 2023, Benjamin Bertrand
+All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
 
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of the copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
 AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
```

### Comparing `jupyterlab_gitlab-3.0.0/PKG-INFO` & `jupyterlab_gitlab-4.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: jupyterlab_gitlab
-Version: 3.0.0
-Summary: JupyterLab viewer for GitLab repositories
-Home-page: https://gitlab.com/beenje/jupyterlab-gitlab
-Author: Benjamin Bertrand
-Author-email: beenje@gmail.com
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3,GitLab
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Jupyter
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # JupyterLab GitLab
 
 A JupyterLab extension for browsing GitLab repositories (in read-only mode).
 
 This extension is based on [jupyterlab-github](https://github.com/jupyterlab/jupyterlab-github).
 All credit to the JupyterLab team, and especially [Ian Rose](https://github.com/ian-r-rose), for the github extension!
 
@@ -66,18 +39,19 @@
 saving files, making commits, forking repositories, etc.
 
 If you want to use git from JupyterLab, you should look at the
 [jupyterlab-git](https://github.com/jupyterlab/jupyterlab-git) extension.
 
 ## Requirements
 
-* JupyterLab >= 3.0
+* JupyterLab >= 4.0
 * JupyterLab 1.x for version 1.x
 * JupyterLab 2.x for version 2.x
 * JupyterLab 3.x for version 3.x
+* JupyterLab 4.x for version 4.x
 * A GitLab account for the server extension
 
 ## Installation
 
 ### Install the server and lab extension
 
 For Jupyterlab >= 3.0, both extensions are installed from the Python package:
@@ -214,9 +188,7 @@
 ```
 
 For JupyterLab < 3, you will also need to run the following command after removing the Python package:
 
 ```bash
 jupyter labextension uninstall jupyterlab-gitlab
 ```
-
-
```

### Comparing `jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/gitlab.py` & `jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/gitlab.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/package.json` & `jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/labextension/package.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9322537112010797%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.2', '@jupyterlab/apputils': '^4.1.2', "*

 * *                   "'@jupyterlab/coreutils': '^6.0.2', '@jupyterlab/docmanager': '^4.0.2', "*

 * *                   "'@jupyterlab/docregistry': '^4.0.2', '@jupyterlab/filebrowser': '^4.0.2', "*

 * *                   "'@jupyterlab/services': '^7.0.2', '@jupyterlab/settingregistry': '^4.0.2', "*

 * *                   "'@jupyterlab/ui-components': '^4.0.2', '@lumino/messaging': '^2.0.0', "*

 * *                   "'@lumino/signaling': […]*

```diff
@@ -3,45 +3,56 @@
         "email": "beenje@gmail.com",
         "name": "Benjamin Bertrand"
     },
     "bugs": {
         "url": "https://gitlab.com/beenje/jupyterlab-gitlab/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
-        "@jupyterlab/apputils": "^3.1.0",
-        "@jupyterlab/coreutils": "^5.1.0",
-        "@jupyterlab/docmanager": "^3.1.0",
-        "@jupyterlab/docregistry": "^3.1.0",
-        "@jupyterlab/filebrowser": "^3.1.0",
-        "@jupyterlab/services": "^6.1.0",
-        "@jupyterlab/settingregistry": "^3.1.0",
-        "@jupyterlab/ui-components": "^3.1.0",
-        "@lumino/messaging": "^1.4.3",
-        "@lumino/signaling": "^1.4.3",
-        "@lumino/widgets": "^1.26.0",
+        "@jupyterlab/application": "^4.0.2",
+        "@jupyterlab/apputils": "^4.1.2",
+        "@jupyterlab/coreutils": "^6.0.2",
+        "@jupyterlab/docmanager": "^4.0.2",
+        "@jupyterlab/docregistry": "^4.0.2",
+        "@jupyterlab/filebrowser": "^4.0.2",
+        "@jupyterlab/services": "^7.0.2",
+        "@jupyterlab/settingregistry": "^4.0.2",
+        "@jupyterlab/ui-components": "^4.0.2",
+        "@lumino/messaging": "^2.0.0",
+        "@lumino/signaling": "^2.0.0",
+        "@lumino/widgets": "^2.0.1",
         "base64-js": "^1.3.0"
     },
     "description": "JupyterLab viewer for GitLab repositories",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.0",
+        "@jupyterlab/builder": "^4.0.0",
         "@types/base64-js": "^1.2.5",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
         "@types/text-encoding": "^0.0.35",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.7.0",
+        "eslint-plugin-prettier": "^4.2.1",
         "husky": "^2.4.1",
         "lint-staged": "^8.2.1",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "typescript": "~4.1.3"
+        "prettier": "^2.8.7",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^14.9.1",
+        "stylelint-config-prettier": "^9.0.4",
+        "stylelint-config-recommended": "^8.0.0",
+        "stylelint-config-standard": "^26.0.0",
+        "stylelint-prettier": "^2.0.0",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.40"
     },
     "directories": {
         "lib": "lib/"
     },
     "files": [
         "lib/*/*d.ts",
         "lib/*/*.js",
@@ -51,15 +62,15 @@
         "style/*.*",
         "style/index.js"
     ],
     "homepage": "https://gitlab.com/beenje/jupyterlab-gitlab",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.a23f7c6fbcd0961ed640.js",
+            "load": "static/remoteEntry.b1ef8c77a08638c7aec5.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab-gitlab"
                 },
@@ -88,31 +99,39 @@
     "main": "lib/index.js",
     "name": "jupyterlab-gitlab",
     "repository": {
         "type": "git",
         "url": "https://gitlab.com/beenje/jupyterlab-gitlab"
     },
     "scripts": {
-        "build": "jlpm run build:lib && jlpm run build:labextension:dev",
+        "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm run clean && jlpm run build:lib && jlpm run build:labextension",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "build:test": "cd test && ./build-tests.sh",
-        "clean": "jlpm run clean:lib",
-        "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
-        "clean:labextension": "rimraf jupyterlab_gitlab/labextension",
+        "clean": "jlpm clean:lib",
+        "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
+        "clean:labextension": "rimraf jupyterlab_gitlab/labextension jupyterlab_gitlab/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "eslint": "eslint . --ext .ts,.tsx --fix",
-        "eslint:check": "eslint . --ext .ts,.tsx",
-        "install:extension": "jlpm run build",
+        "clean:lintcache": "rimraf .eslintcache .stylelintcache",
+        "eslint": "jlpm eslint:check --fix",
+        "eslint:check": "eslint . --cache --ext .ts,.tsx",
+        "install:extension": "jlpm build",
+        "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
+        "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "precommit": "lint-staged",
-        "prettier": "prettier --write '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
+        "prettier": "jlpm prettier:base --write --list-different",
+        "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
+        "prettier:check": "jlpm prettier:base --check",
+        "stylelint": "jlpm stylelint:check --fix",
+        "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "test": "cd test && ./run-tests.sh",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "3.0.0"
+    "version": "4.0.0"
 }
```

### Comparing `jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/schemas/jupyterlab-gitlab/drive.json` & `jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/labextension/schemas/jupyterlab-gitlab/drive.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/static/392.b613df8f5a6e873d0ed2.js` & `jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/labextension/static/232.2729dbd8de27fb8601e1.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,43 +1,45 @@
 "use strict";
 (self.webpackChunkjupyterlab_gitlab = self.webpackChunkjupyterlab_gitlab || []).push([
-    [392], {
-        392: (e, t, s) => {
+    [232], {
+        232: (e, t, s) => {
             s.r(t), s.d(t, {
-                default: () => C
+                default: () => P,
+                gitLabIcon: () => C
             });
-            var r = s(23),
-                i = s(589),
-                n = s(525),
-                o = s(451),
-                a = s(994),
-                l = s(168),
-                c = s(920),
-                h = s(414),
-                d = s(491);
+            var r = s(4),
+                i = s(172),
+                a = s(580),
+                n = s(663),
+                o = s(237),
+                l = s(154),
+                c = s(901),
+                h = s(987),
+                d = s(1),
+                p = s(790);
 
-            function p(e, t) {
-                return d.ServerConnection.makeRequest(e, {}, t).then((e => 200 !== e.status ? e.json().then((t => {
-                    throw new d.ServerConnection.ResponseError(e, t.message)
+            function u(e, t) {
+                return p.ServerConnection.makeRequest(e, {}, t).then((e => 200 !== e.status ? e.json().then((t => {
+                    throw new p.ServerConnection.ResponseError(e, t.message)
                 })) : e.json()))
             }
-            var u = s(959);
-            const m = "https://gitlab.com";
-            class b {
+            var m = s(959);
+            const b = "https://gitlab.com";
+            class _ {
                 constructor(e) {
-                    this._baseUrl = "", this._validUser = !1, this._isDisposed = !1, this._fileChanged = new l.Signal(this), this._serverSettings = d.ServerConnection.makeSettings(), this._fileTypeForPath = t => {
+                    this._baseUrl = "", this._validUser = !1, this._defaultBranch = "", this._isDisposed = !1, this._fileChanged = new c.Signal(this), this._serverSettings = p.ServerConnection.makeSettings(), this._fileTypeForPath = t => {
                         const s = e.getFileTypesForPath(t);
                         return 0 === s.length ? e.getFileType("text") : s[0]
-                    }, this.baseUrl = m, this._useProxy = new Promise((e => {
-                        p(c.URLExt.join(this._serverSettings.baseUrl, "gitlab", g.b64EncodeUrlSafe("/templates/licenses")), this._serverSettings).then((() => {
+                    }, this.baseUrl = b, this._useProxy = new Promise((e => {
+                        u(h.URLExt.join(this._serverSettings.baseUrl, "gitlab", y.b64EncodeUrlSafe("/templates/licenses")), this._serverSettings).then((() => {
                             e(!0)
                         })).catch((() => {
                             console.warn("The JupyterLab GitLab server extension appears to be missing. If you do not install it with application credentials, you are likely to be rate limited by GitLab very quickly"), e(!1)
                         }))
-                    })), this.rateLimitedState = new h.ObservableValue(!1)
+                    })), this.rateLimitedState = new d.ObservableValue(!1)
                 }
                 get name() {
                     return "GitLab"
                 }
                 get validUser() {
                     return this._validUser
                 }
@@ -47,43 +49,49 @@
                 get fileChanged() {
                     return this._fileChanged
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 dispose() {
-                    this.isDisposed || (this._isDisposed = !0, l.Signal.clearData(this))
+                    this.isDisposed || (this._isDisposed = !0, c.Signal.clearData(this))
                 }
                 get baseUrl() {
                     return this._baseUrl
                 }
                 set baseUrl(e) {
                     this._baseUrl = e
                 }
                 get accessToken() {
                     return this._accessToken
                 }
                 set accessToken(e) {
                     this._accessToken = e
                 }
                 get(e, t) {
-                    const s = _(e);
-                    if ("" === s.user) return this._validUser = !1, Promise.resolve(g.dummyDirectory);
+                    const s = g(e);
+                    if ("" === s.user) return this._validUser = !1, Promise.resolve(y.dummyDirectory);
                     if (s.user && !s.repository) return this._listRepos(s.user);
                     let r = "tree";
-                    s.path && (r = !t || "file" !== t.type && "notebook" !== t.type ? c.URLExt.join("tree", "?path=" + encodeURIComponent(s.path)) : c.URLExt.join("files", encodeURIComponent(s.path)) + "?ref=master");
-                    const i = c.URLExt.join("projects", encodeURIComponent(s.user) + "%2F" + encodeURIComponent(s.repository), "repository", r);
-                    return this._apiRequest(i).then((t => (this._validUser = !0, !1 !== this.rateLimitedState.get() && this.rateLimitedState.set(!1), g.gitLabContentsToJupyterContents(e, t, this._fileTypeForPath)))).catch((e => 404 === e.response.status ? (console.warn("GitLab: cannot find group/repo. Perhaps you misspelled something?"), this._validUser = !1, g.dummyDirectory) : 403 === e.response.status && -1 !== e.message.indexOf("rate limit") ? (!0 !== this.rateLimitedState.get() && this.rateLimitedState.set(!0), console.error(e.message), Promise.reject(e)) : (console.error(e.message), Promise.reject(e))))
+                    if (s.path) r = !t || "file" !== t.type && "notebook" !== t.type ? h.URLExt.join("tree", "?path=" + encodeURIComponent(s.path)) : h.URLExt.join("files", encodeURIComponent(s.path)) + "?ref=" + this._defaultBranch;
+                    else {
+                        const e = h.URLExt.join("projects", encodeURIComponent(s.user) + "%2F" + encodeURIComponent(s.repository));
+                        this._apiRequest(e).then((e => {
+                            this._defaultBranch = e.default_branch
+                        }))
+                    }
+                    const i = h.URLExt.join("projects", encodeURIComponent(s.user) + "%2F" + encodeURIComponent(s.repository), "repository", r);
+                    return this._apiRequest(i).then((t => (this._validUser = !0, !1 !== this.rateLimitedState.get() && this.rateLimitedState.set(!1), y.gitLabContentsToJupyterContents(e, t, this._fileTypeForPath)))).catch((e => 404 === e.response.status ? (console.warn("GitLab: cannot find group/repo. Perhaps you misspelled something?"), this._validUser = !1, y.dummyDirectory) : 403 === e.response.status && -1 !== e.message.indexOf("rate limit") ? (!0 !== this.rateLimitedState.get() && this.rateLimitedState.set(!0), console.error(e.message), Promise.reject(e)) : (console.error(e.message), Promise.reject(e))))
                 }
                 getDownloadUrl(e) {
-                    const t = _(e);
+                    const t = g(e);
                     if (!t.user) return Promise.reject("GitLab: no active group");
                     if (!t.path) return Promise.reject("GitLab: No file selected");
-                    const s = c.URLExt.join(this.baseUrl, "api", "v4"),
-                        r = c.URLExt.join(s, "projects", encodeURIComponent(t.user) + "%2F" + encodeURIComponent(t.repository), "repository", "files", encodeURIComponent(t.path), "raw") + "?ref=master";
+                    const s = h.URLExt.join(this.baseUrl, "api", "v4"),
+                        r = h.URLExt.join(s, "projects", encodeURIComponent(t.user) + "%2F" + encodeURIComponent(t.repository), "repository", "files", encodeURIComponent(t.path), "raw") + "?ref=" + this._defaultBranch;
                     return Promise.resolve(r)
                 }
                 newUntitled(e = {}) {
                     return Promise.reject("Repository is read only")
                 }
                 delete(e) {
                     return Promise.reject("Repository is read only")
@@ -106,112 +114,112 @@
                 restoreCheckpoint(e, t) {
                     return Promise.reject("Repository is read only")
                 }
                 deleteCheckpoint(e, t) {
                     return Promise.reject("Read only")
                 }
                 _listRepos(e) {
-                    const t = c.URLExt.encodeParts(c.URLExt.join("groups", e, "projects"));
+                    const t = h.URLExt.encodeParts(h.URLExt.join("groups", e, "projects"));
                     return this._apiRequest(t).catch((t => {
                         if (404 === t.response.status) {
-                            const t = c.URLExt.encodeParts(c.URLExt.join("users", e, "projects"));
+                            const t = h.URLExt.encodeParts(h.URLExt.join("users", e, "projects"));
                             return this._apiRequest(t)
                         }
                         throw t
-                    })).then((e => (this._validUser = !0, !1 !== this.rateLimitedState.get() && this.rateLimitedState.set(!1), g.reposToDirectory(e)))).catch((e => (403 === e.response.status && -1 !== e.message.indexOf("rate limit") ? !0 !== this.rateLimitedState.get() && this.rateLimitedState.set(!0) : (console.error(e.message), console.warn("GitLab: cannot find user. Perhaps you misspelled something?"), this._validUser = !1), g.dummyDirectory)))
+                    })).then((e => (this._validUser = !0, !1 !== this.rateLimitedState.get() && this.rateLimitedState.set(!1), y.reposToDirectory(e)))).catch((e => (403 === e.response.status && -1 !== e.message.indexOf("rate limit") ? !0 !== this.rateLimitedState.get() && this.rateLimitedState.set(!0) : (console.error(e.message), console.warn("GitLab: cannot find user. Perhaps you misspelled something?"), this._validUser = !1), y.dummyDirectory)))
                 }
                 _apiRequest(e) {
                     return this._useProxy.then((t => {
                         const s = e.split("?");
                         let r = s[0];
                         const i = (s[1] || "").split("&"),
-                            n = {};
+                            a = {};
                         for (const e of i)
                             if (e) {
                                 const [t, s] = e.split("=");
-                                n[t] = s
-                            } let o;
-                        return !0 === t ? (o = c.URLExt.join(this._serverSettings.baseUrl, "gitlab"), this.accessToken && (n.private_token = this.accessToken)) : o = c.URLExt.join(this.baseUrl, "api", "v4"), r && (!0 === t && (r = g.b64EncodeUrlSafe(r)), o = c.URLExt.join(o, r)), o += "?" + Object.keys(n).map((e => `${e}=${n[e]}`)).join("&"), !0 === t ? p(o, this._serverSettings) : (a = o, window.fetch(a).then((e => 200 !== e.status ? e.json().then((t => {
-                            throw new d.ServerConnection.ResponseError(e, t.message)
+                                a[t] = s
+                            } let n;
+                        return !0 === t ? (n = h.URLExt.join(this._serverSettings.baseUrl, "gitlab"), this.accessToken && (a.private_token = this.accessToken)) : n = h.URLExt.join(this.baseUrl, "api", "v4"), r && (!0 === t && (r = y.b64EncodeUrlSafe(r)), n = h.URLExt.join(n, r)), n += "?" + Object.keys(a).map((e => `${e}=${a[e]}`)).join("&"), !0 === t ? u(n, this._serverSettings) : (o = n, window.fetch(o).then((e => 200 !== e.status ? e.json().then((t => {
+                            throw new p.ServerConnection.ResponseError(e, t.message)
                         })) : e.json())));
-                        var a
+                        var o
                     }))
                 }
             }
 
-            function _(e) {
+            function g(e) {
                 const t = e.split("/");
                 return {
                     user: t.length > 0 ? t[0] : "",
                     repository: t.length > 1 ? t[1] : "",
-                    path: t.length > 2 ? c.URLExt.join(...t.slice(2)) : ""
+                    path: t.length > 2 ? h.URLExt.join(...t.slice(2)) : ""
                 }
             }
-            var g;
+            var y;
             ! function(e) {
                 function t(e, t) {
                     const s = new Response(t, {
                         status: e,
                         statusText: t
                     });
-                    return new d.ServerConnection.ResponseError(s, t)
+                    return new p.ServerConnection.ResponseError(s, t)
                 }
                 e.dummyDirectory = {
                     type: "directory",
                     path: "",
                     name: "",
                     format: "json",
                     content: [],
                     created: "",
                     writable: !1,
                     last_modified: "",
                     mimetype: ""
-                }, e.gitLabContentsToJupyterContents = function s(r, i, n) {
+                }, e.gitLabContentsToJupyterContents = function s(r, i, a) {
                     if (Array.isArray(i)) return {
-                        name: c.PathExt.basename(r),
+                        name: h.PathExt.basename(r),
                         path: r,
                         format: "json",
                         type: "directory",
                         writable: !1,
                         created: "",
                         last_modified: "",
                         mimetype: "",
-                        content: i.map((e => s(c.PathExt.join(r, e.name), e, n)))
+                        content: i.map((e => s(h.PathExt.join(r, e.name), e, a)))
                     };
                     if ("blob" === i.type || i.hasOwnProperty("file_name")) {
-                        const t = n(r),
+                        const t = a(r),
                             s = i.content;
-                        let o;
+                        let n;
                         switch (t.fileFormat) {
                             case "text":
-                                o = void 0 !== s ? e.b64DecodeUTF8(s) : null;
+                                n = void 0 !== s ? e.b64DecodeUTF8(s) : null;
                                 break;
                             case "base64":
-                                o = void 0 !== s ? s : null;
+                                n = void 0 !== s ? s : null;
                                 break;
                             case "json":
-                                o = void 0 !== s ? JSON.parse(e.b64DecodeUTF8(s)) : null;
+                                n = void 0 !== s ? JSON.parse(e.b64DecodeUTF8(s)) : null;
                                 break;
                             default:
                                 throw new Error(`Unexpected file format: ${t.fileFormat}`)
                         }
                         return {
-                            name: c.PathExt.basename(r),
+                            name: h.PathExt.basename(r),
                             path: r,
                             format: t.fileFormat,
                             type: "file",
                             created: "",
                             writable: !1,
                             last_modified: "",
                             mimetype: t.mimeTypes[0],
-                            content: o
+                            content: n
                         }
                     }
                     if ("tree" === i.type) return {
-                        name: c.PathExt.basename(r),
+                        name: h.PathExt.basename(r),
                         path: r,
                         format: "json",
                         type: "directory",
                         created: "",
                         writable: !1,
                         last_modified: "",
                         mimetype: "",
@@ -239,69 +247,68 @@
                             mimetype: "",
                             content: null
                         })))
                     }
                 }, e.makeError = t;
                 const s = new TextDecoder("utf8");
                 e.b64DecodeUTF8 = function(e) {
-                    const t = u.toByteArray(e.replace(/\n/g, ""));
+                    const t = m.toByteArray(e.replace(/\n/g, ""));
                     return s.decode(t)
                 }, e.b64EncodeUrlSafe = function(e) {
                     return btoa(e).replace(/\+/g, "-").replace(/\//g, "_")
                 }
-            }(g || (g = {}));
-            var y = s(133),
-                w = s(615);
-            class f extends w.Widget {
+            }(y || (y = {}));
+            var f = s(778);
+            class w extends f.Widget {
                 constructor(e, t) {
-                    super(), this._errorPanel = null, this._changeGuard = !1, this.addClass("jp-GitLabBrowser"), this.layout = new w.PanelLayout, this.layout.addWidget(e), this._browser = e, this._drive = t, this.userName = new v, this.userName.node.title = "Click to edit user/group", this._browser.toolbar.addItem("user", this.userName), this.userName.nameChanged.connect(this._onUserChanged, this), this._openGitLabButton = new i.ToolbarButton({
+                    super(), this._errorPanel = null, this._changeGuard = !1, this.addClass("jp-GitLabBrowser"), this.layout = new f.PanelLayout, this.layout.addWidget(e), this._browser = e, this._drive = t, this.userName = new v, this.userName.node.title = "Click to edit user/group", this._browser.toolbar.addItem("user", this.userName), this.userName.nameChanged.connect(this._onUserChanged, this), this._openGitLabButton = new i.ToolbarButton({
                         onClick: () => {
                             let e = this._drive.baseUrl;
                             if (!this._drive.validUser) return void window.open(e);
-                            const t = _(this._browser.model.manager.services.contents.localPath(this._browser.model.path));
-                            e = c.URLExt.join(e, t.user), t.repository && (e = c.URLExt.join(e, t.repository, "tree", "master", t.path)), window.open(e)
+                            const t = g(this._browser.model.manager.services.contents.localPath(this._browser.model.path));
+                            e = h.URLExt.join(e, t.user), t.repository && (e = h.URLExt.join(e, t.repository, "tree", "master", t.path)), window.open(e)
                         },
                         iconClass: "jp-GitLab-icon jp-Icon jp-Icon-16",
                         tooltip: "Open this repository on GitLab"
                     }), this._openGitLabButton.addClass("jp-GitLab-toolbar-item"), this._browser.toolbar.addItem("GitLab", this._openGitLabButton);
                     const s = new i.ToolbarButton({
-                        icon: y.refreshIcon,
+                        icon: a.refreshIcon,
                         onClick: () => {
                             this._browser.model.refresh()
                         },
                         tooltip: "Refresh File List"
                     });
                     s.addClass("jp-GitLab-toolbar-item"), this._browser.toolbar.addItem("gh-refresher", s), this._browser.model.pathChanged.connect(this._onPathChanged, this), this._onPathChanged(), this._drive.rateLimitedState.changed.connect(this._updateErrorPanel, this)
                 }
                 _onUserChanged() {
                     this._changeGuard || (this._changeGuard = !0, this._browser.model.cd(`/${this.userName.name}`).then((() => {
-                        this._changeGuard = !1, this._updateErrorPanel(), document.activeElement === document.body && this._browser.layout.widgets[3].node.focus()
+                        this._changeGuard = !1, this._updateErrorPanel(), document.activeElement === document.body && this._browser.layout.widgets[1].node.focus()
                     })))
                 }
                 _onPathChanged() {
-                    const e = _(this._browser.model.manager.services.contents.localPath(this._browser.model.path));
+                    const e = g(this._browser.model.manager.services.contents.localPath(this._browser.model.path));
                     this._changeGuard || (this._changeGuard = !0, this.userName.name = e.user, this._changeGuard = !1, this._updateErrorPanel())
                 }
                 _updateErrorPanel() {
-                    const e = _(this._browser.model.manager.services.contents.localPath(this._browser.model.path)),
+                    const e = g(this._browser.model.manager.services.contents.localPath(this._browser.model.path)),
                         t = this._drive.rateLimitedState.get(),
                         s = this._drive.validUser;
-                    if (this._errorPanel && (this._browser.layout.widgets[3].node.removeChild(this._errorPanel.node), this._errorPanel.dispose(), this._errorPanel = null), t) this._errorPanel = new L("You have been rate limited by GitLab! You will need to wait about an hour before continuing"), this._browser.layout.widgets[3].node.appendChild(this._errorPanel.node);
+                    if (this._errorPanel && (this._browser.layout.widgets[1].node.removeChild(this._errorPanel.node), this._errorPanel.dispose(), this._errorPanel = null), t) this._errorPanel = new L("You have been rate limited by GitLab! You will need to wait about an hour before continuing"), this._browser.layout.widgets[1].node.appendChild(this._errorPanel.node);
                     else if (s);
                     else {
                         const t = e.user ? `"${e.user}" appears to be an invalid user name!` : "Please enter a GitLab user name";
-                        this._errorPanel = new L(t), this._browser.layout.widgets[3].node.appendChild(this._errorPanel.node)
+                        this._errorPanel = new L(t), this._browser.layout.widgets[1].node.appendChild(this._errorPanel.node)
                     }
                 }
             }
-            class v extends w.Widget {
+            class v extends f.Widget {
                 constructor() {
-                    super(), this._name = "", this._nameChanged = new l.Signal(this), this.addClass("jp-GitLabUserInput");
-                    const e = this.layout = new w.PanelLayout,
-                        t = new w.Widget;
+                    super(), this._name = "", this._nameChanged = new c.Signal(this), this.addClass("jp-GitLabUserInput");
+                    const e = this.layout = new f.PanelLayout,
+                        t = new f.Widget;
                     t.addClass("jp-GitLabUserInput-wrapper"), this._input = document.createElement("input"), this._input.placeholder = "GitLab User or Group", this._input.className = "jp-GitLabUserInput-input", t.node.appendChild(this._input), e.addWidget(t)
                 }
                 get name() {
                     return this._name
                 }
                 set name(e) {
                     if (e === this._name) return;
@@ -313,18 +320,15 @@
                 }
                 get nameChanged() {
                     return this._nameChanged
                 }
                 handleEvent(e) {
                     switch (e.type) {
                         case "keydown":
-                            switch (e.keyCode) {
-                                case 13:
-                                    e.stopPropagation(), e.preventDefault(), this.name = this._input.value, this._input.blur()
-                            }
+                            13 === e.keyCode && (e.stopPropagation(), e.preventDefault(), this.name = this._input.value, this._input.blur());
                             break;
                         case "blur":
                             e.stopPropagation(), e.preventDefault(), this.name = this._input.value;
                             break;
                         case "focus":
                             e.stopPropagation(), e.preventDefault(), this._input.select()
                     }
@@ -332,69 +336,73 @@
                 onAfterAttach(e) {
                     this._input.addEventListener("keydown", this), this._input.addEventListener("blur", this), this._input.addEventListener("focus", this)
                 }
                 onBeforeDetach(e) {
                     this._input.removeEventListener("keydown", this), this._input.removeEventListener("blur", this), this._input.removeEventListener("focus", this)
                 }
             }
-            class L extends w.Widget {
+            class L extends f.Widget {
                 constructor(e) {
                     super(), this.addClass("jp-GitLabErrorPanel");
                     const t = document.createElement("div"),
                         s = document.createElement("div");
                     t.className = "jp-GitLabErrorImage", s.className = "jp-GitLabErrorText", s.textContent = e, this.node.appendChild(t), this.node.appendChild(s)
                 }
             }
             const U = "gitlab-filebrowser",
                 j = "jupyterlab-gitlab:drive",
-                C = {
+                C = new a.LabIcon({
+                    name: `${U}:icon`,
+                    svgstr: '<svg id="Layer_1" data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 622 682"><defs><style>.cls-1{fill:#5c5c5c;}.cls-2{fill:#a1a1a1;}.cls-3{fill:#787878;}</style></defs><title>stacked_wm_grayscale</title><path id="path14" class="cls-1" d="M316.89,497.33h-19l0.06,141.74H375V621.55h-58l-0.06-124.22h0Z"/><path id="path26" class="cls-1" d="M448.32,614.19a32.46,32.46,0,0,1-23.59,10c-14.5,0-20.35-7.14-20.35-16.45,0-14.07,9.74-20.77,30.52-20.77A86.46,86.46,0,0,1,448.32,588v26.19h0Zm-19.7-85.91a63.45,63.45,0,0,0-40.5,14.53l6.73,11.66c7.79-4.54,17.32-9.09,31-9.09,15.58,0,22.51,8,22.51,21.42v6.93a81.48,81.48,0,0,0-13.2-1.08c-33.33,0-50.22,11.69-50.22,36.14,0,21.86,13.42,32.89,33.76,32.89,13.71,0,26.84-6.28,31.38-16.45l3.46,13.85h13.42V566.58c0-22.94-10-38.3-38.31-38.3h0Z"/><path id="path30" class="cls-1" d="M528.4,624.8c-7.14,0-13.42-.87-18.18-3V556.2c6.49-5.41,14.5-9.31,24.68-9.31,18.4,0,25.54,13,25.54,34,0,29.86-11.47,43.93-32,43.93m8-96.52a34.88,34.88,0,0,0-26.19,11.58V521.57l-0.06-24.24H491.54l0.06,138.28c9.31,3.9,22.08,6.06,35.93,6.06,35.5,0,52.6-22.72,52.6-61.89,0-30.95-15.8-51.51-43.73-51.51"/><path id="path34" class="cls-1" d="M109.84,512.7c16.88,0,27.7,5.63,34.85,11.25l8.19-14.18c-11.16-9.78-26.16-15-42.17-15-40.47,0-68.83,24.67-68.83,74.44,0,52.15,30.59,72.5,65.58,72.5a111,111,0,0,0,42.21-8.22l-0.4-55.72V560.2H97.32v17.53h33.12l0.4,42.31c-4.33,2.16-11.9,3.9-22.08,3.9-28.14,0-47-17.7-47-55,0-37.87,19.48-56.26,48.05-56.26"/><path id="path38" class="cls-1" d="M243.79,497.33H225.17l0.06,23.8v82.23c0,22.94,10,38.3,38.31,38.3a64.16,64.16,0,0,0,11.47-1V623.93a57,57,0,0,1-8.66.65c-15.58,0-22.51-8-22.51-21.42v-56.7H275V530.88H243.85l-0.06-33.54h0Z"/><path id="path40" class="cls-1" d="M177.94,639.08h18.61V530.88H177.94v108.2h0Z"/><path id="path42" class="cls-1" d="M177.94,515.94h18.61V497.33H177.94v18.61h0Z"/><path id="path46" class="cls-2" d="M525.05,266.61l-24-74L453.36,46a8.19,8.19,0,0,0-15.58,0L390.12,192.62H231.88L184.22,46a8.19,8.19,0,0,0-15.58,0L121,192.62l-24,74a16.38,16.38,0,0,0,6,18.31L311,436.09,519.1,284.92a16.38,16.38,0,0,0,6-18.31"/><path id="path50" class="cls-1" d="M311,436.09h0l79.12-243.47H231.88L311,436.09h0Z"/><path id="path58" class="cls-3" d="M311,436.09L231.88,192.62H121L311,436.09h0Z"/><path id="path66" class="cls-2" d="M121,192.62h0l-24,74a16.37,16.37,0,0,0,6,18.31L311,436.09,121,192.62h0Z"/><path id="path74" class="cls-1" d="M121,192.62H231.88L184.22,46a8.19,8.19,0,0,0-15.58,0L121,192.62h0Z"/><path id="path78" class="cls-3" d="M311,436.09l79.12-243.47H501L311,436.09h0Z"/><path id="path82" class="cls-2" d="M501,192.62h0l24,74a16.37,16.37,0,0,1-6,18.31L311,436.09,501,192.62h0Z"/><path id="path86" class="cls-1" d="M501,192.62H390.12L437.78,46a8.19,8.19,0,0,1,15.58,0L501,192.62h0Z"/></svg>'
+                }),
+                P = {
                     id: j,
-                    requires: [o.IDocumentManager, a.IFileBrowserFactory, r.ILayoutRestorer, n.ISettingRegistry],
+                    requires: [o.IDocumentManager, l.IFileBrowserFactory, r.ILayoutRestorer, n.ISettingRegistry],
                     activate: function(e, t, s, r, i) {
-                        const n = new b(e.docRegistry);
-                        t.services.contents.addDrive(n);
-                        const o = s.createFileBrowser(U, {
-                                driveName: n.name,
+                        const a = new _(e.docRegistry);
+                        t.services.contents.addDrive(a);
+                        const n = s.createFileBrowser(U, {
+                                driveName: a.name,
                                 refreshInterval: 3e5
                             }),
-                            a = new f(o, n);
-                        a.title.iconClass = "jp-GitLab-icon jp-SideBar-tabIcon", a.title.caption = "Browse GitLab", a.id = "gitlab-file-browser", r.add(a, U), e.shell.add(a, "left", {
+                            o = new w(n, a);
+                        o.title.icon = C, o.title.iconClass = "jp-SideBar-tabIcon", o.title.caption = "Browse GitLab", o.id = "gitlab-file-browser", r.add(o, U), e.shell.add(o, "left", {
                             rank: 102
                         });
                         let l = !1;
                         const c = async e => {
                             const t = e.get("baseUrl").composite,
                                 s = e.get("accessToken").composite;
-                            if (n.baseUrl = t || m, s) {
+                            if (a.baseUrl = t || b, s) {
                                 let t = !0;
-                                l && (t = await P.showWarning()), t ? n.accessToken = s : e.remove("accessToken")
-                            } else n.accessToken = null
+                                l && (t = await R.showWarning()), t ? a.accessToken = s : e.remove("accessToken")
+                            } else a.accessToken = null
                         };
                         Promise.all([i.load(j), e.restored]).then((([e]) => {
                             e.changed.connect(c), c(e), l = !0;
                             const t = e.get("defaultRepo").composite;
-                            t && o.model.restored.then((() => {
-                                o.model.cd(`/${t}`)
+                            t && n.model.restored.then((() => {
+                                n.model.cd(`/${t}`)
                             }))
                         })).catch((e => {
                             console.error(e.message)
                         }))
                     },
                     autoStart: !0
                 };
-            var P;
+            var R;
             ! function(e) {
                 e.showWarning = async function() {
                     return (0, i.showDialog)({
                         title: "Security Alert!",
                         body: "Adding a client side access token can pose a security risk! Please consider using the server extension instead.Do you want to continue?",
                         buttons: [i.Dialog.cancelButton({
                             label: "CANCEL"
                         }), i.Dialog.warnButton({
                             label: "PROCEED"
                         })]
                     }).then((e => !!e.button.accept))
                 }
-            }(P || (P = {}))
+            }(R || (R = {}))
         }
     }
 ]);
```

### Comparing `jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/static/742.ee2a9c67f39dc93945ac.js` & `jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/labextension/static/742.ff0c6cd9a5a3198ebae4.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,41 +1,41 @@
 "use strict";
 (self.webpackChunkjupyterlab_gitlab = self.webpackChunkjupyterlab_gitlab || []).push([
     [742], {
         742: (r, t) => {
             t.byteLength = function(r) {
-                var t = c(r),
+                var t = h(r),
                     e = t[0],
                     n = t[1];
                 return 3 * (e + n) / 4 - n
             }, t.toByteArray = function(r) {
-                var t, e, o = c(r),
-                    h = o[0],
-                    u = o[1],
+                var t, e, o = h(r),
+                    u = o[0],
+                    c = o[1],
                     i = new a(function(r, t, e) {
                         return 3 * (t + e) / 4 - e
-                    }(0, h, u)),
+                    }(0, u, c)),
                     f = 0,
-                    A = u > 0 ? h - 4 : h;
+                    A = c > 0 ? u - 4 : u;
                 for (e = 0; e < A; e += 4) t = n[r.charCodeAt(e)] << 18 | n[r.charCodeAt(e + 1)] << 12 | n[r.charCodeAt(e + 2)] << 6 | n[r.charCodeAt(e + 3)], i[f++] = t >> 16 & 255, i[f++] = t >> 8 & 255, i[f++] = 255 & t;
-                return 2 === u && (t = n[r.charCodeAt(e)] << 2 | n[r.charCodeAt(e + 1)] >> 4, i[f++] = 255 & t), 1 === u && (t = n[r.charCodeAt(e)] << 10 | n[r.charCodeAt(e + 1)] << 4 | n[r.charCodeAt(e + 2)] >> 2, i[f++] = t >> 8 & 255, i[f++] = 255 & t), i
+                return 2 === c && (t = n[r.charCodeAt(e)] << 2 | n[r.charCodeAt(e + 1)] >> 4, i[f++] = 255 & t), 1 === c && (t = n[r.charCodeAt(e)] << 10 | n[r.charCodeAt(e + 1)] << 4 | n[r.charCodeAt(e + 2)] >> 2, i[f++] = t >> 8 & 255, i[f++] = 255 & t), i
             }, t.fromByteArray = function(r) {
-                for (var t, n = r.length, a = n % 3, o = [], h = 16383, u = 0, c = n - a; u < c; u += h) o.push(i(r, u, u + h > c ? c : u + h));
+                for (var t, n = r.length, a = n % 3, o = [], u = 16383, h = 0, i = n - a; h < i; h += u) o.push(c(r, h, h + u > i ? i : h + u));
                 return 1 === a ? (t = r[n - 1], o.push(e[t >> 2] + e[t << 4 & 63] + "==")) : 2 === a && (t = (r[n - 2] << 8) + r[n - 1], o.push(e[t >> 10] + e[t >> 4 & 63] + e[t << 2 & 63] + "=")), o.join("")
             };
-            for (var e = [], n = [], a = "undefined" != typeof Uint8Array ? Uint8Array : Array, o = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/", h = 0, u = o.length; h < u; ++h) e[h] = o[h], n[o.charCodeAt(h)] = h;
+            for (var e = [], n = [], a = "undefined" != typeof Uint8Array ? Uint8Array : Array, o = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/", u = 0; u < 64; ++u) e[u] = o[u], n[o.charCodeAt(u)] = u;
 
-            function c(r) {
+            function h(r) {
                 var t = r.length;
                 if (t % 4 > 0) throw new Error("Invalid string. Length must be a multiple of 4");
                 var e = r.indexOf("=");
                 return -1 === e && (e = t), [e, e === t ? 0 : 4 - e % 4]
             }
 
-            function i(r, t, n) {
-                for (var a, o, h = [], u = t; u < n; u += 3) a = (r[u] << 16 & 16711680) + (r[u + 1] << 8 & 65280) + (255 & r[u + 2]), h.push(e[(o = a) >> 18 & 63] + e[o >> 12 & 63] + e[o >> 6 & 63] + e[63 & o]);
-                return h.join("")
+            function c(r, t, n) {
+                for (var a, o, u = [], h = t; h < n; h += 3) a = (r[h] << 16 & 16711680) + (r[h + 1] << 8 & 65280) + (255 & r[h + 2]), u.push(e[(o = a) >> 18 & 63] + e[o >> 12 & 63] + e[o >> 6 & 63] + e[63 & o]);
+                return u.join("")
             }
             n["-".charCodeAt(0)] = 62, n["_".charCodeAt(0)] = 63
         }
     }
 ]);
```

### Comparing `jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/static/remoteEntry.a23f7c6fbcd0961ed640.js` & `jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/labextension/static/remoteEntry.b1ef8c77a08638c7aec5.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,300 +1,303 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, s, d, f, p, c, h, b, v, g, y, m, j, w, S = {
+    var e, r, t, a, n, o, i, u, l, s, f, d, p, c, h, v, b, g, y, m, j, w, S, E = {
             706: (e, r, t) => {
-                var n = {
-                        "./index": () => t.e(392).then((() => () => t(392))),
-                        "./extension": () => t.e(392).then((() => () => t(392))),
-                        "./style": () => t.e(534).then((() => () => t(534)))
+                var a = {
+                        "./index": () => t.e(232).then((() => () => t(232))),
+                        "./extension": () => t.e(232).then((() => () => t(232))),
+                        "./style": () => t.e(747).then((() => () => t(747)))
                     },
-                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
-                            var n = t.S.default,
-                                a = "default";
+                            var a = "default",
+                                n = t.S[a];
                             if (n && n !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[a] = e, t.I(a, r)
                         }
                     };
                 t.d(r, {
-                    get: () => a,
+                    get: () => n,
                     init: () => o
                 })
             }
         },
-        E = {};
+        k = {};
 
-    function k(e) {
-        var r = E[e];
+    function P(e) {
+        var r = k[e];
         if (void 0 !== r) return r.exports;
-        var t = E[e] = {
+        var t = k[e] = {
             id: e,
             exports: {}
         };
-        return S[e](t, t.exports, k), t.exports
+        return E[e](t, t.exports, P), t.exports
     }
-    k.m = S, k.c = E, k.n = e => {
+    P.m = E, P.c = k, P.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return k.d(r, {
+        return P.d(r, {
             a: r
         }), r
-    }, k.d = (e, r) => {
-        for (var t in r) k.o(r, t) && !k.o(e, t) && Object.defineProperty(e, t, {
+    }, P.d = (e, r) => {
+        for (var t in r) P.o(r, t) && !P.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, k.f = {}, k.e = e => Promise.all(Object.keys(k.f).reduce(((r, t) => (k.f[t](e, r), r)), [])), k.u = e => e + "." + {
-        392: "b613df8f5a6e873d0ed2",
-        534: "2d174fa7be8b96a8c604",
-        742: "ee2a9c67f39dc93945ac"
+    }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
+        232: "2729dbd8de27fb8601e1",
+        742: "ff0c6cd9a5a3198ebae4",
+        747: "a85ac71c39deaa0e363e"
     } [e] + ".js?v=" + {
-        392: "b613df8f5a6e873d0ed2",
-        534: "2d174fa7be8b96a8c604",
-        742: "ee2a9c67f39dc93945ac"
-    } [e], k.g = function() {
+        232: "2729dbd8de27fb8601e1",
+        742: "ff0c6cd9a5a3198ebae4",
+        747: "a85ac71c39deaa0e363e"
+    } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), k.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyterlab-gitlab:", k.l = (t, n, a, o) => {
-        if (e[t]) e[t].push(n);
+    }(), P.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyterlab-gitlab:", P.l = (t, a, n, o) => {
+        if (e[t]) e[t].push(a);
         else {
             var i, u;
-            if (void 0 !== a)
+            if (void 0 !== n)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var d = l[s];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + a) {
-                        i = d;
+                    var f = l[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
+                        i = f;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, k.nc && i.setAttribute("nonce", k.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var f = (r, n) => {
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, P.nc && i.setAttribute("nonce", P.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
+            var d = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(p);
-                    var a = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
+                    var n = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                p = setTimeout(f.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, k.r = e => {
+    }, P.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        k.S = {};
+        P.S = {};
         var e = {},
             r = {};
-        k.I = (t, n) => {
-            n || (n = []);
-            var a = r[t];
-            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
-                if (n.push(a), e[t]) return e[t];
-                k.o(k.S, t) || (k.S[t] = {});
-                var o = k.S[t],
+        P.I = (t, a) => {
+            a || (a = []);
+            var n = r[t];
+            if (n || (n = r[t] = {}), !(a.indexOf(n) >= 0)) {
+                if (a.push(n), e[t]) return e[t];
+                P.o(P.S, t) || (P.S[t] = {});
+                var o = P.S[t],
                     i = "jupyterlab-gitlab",
-                    u = (e, r, t, n) => {
-                        var a = o[e] = o[e] || {},
-                            u = a[r];
-                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (a[r] = {
+                    u = (e, r, t, a) => {
+                        var n = o[e] = o[e] || {},
+                            u = n[r];
+                        (!u || !u.loaded && (!a != !u.eager ? a : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
-                            eager: !!n
+                            eager: !!a
                         })
                     },
                     l = [];
-                switch (t) {
-                    case "default":
-                        u("base64-js", "1.5.1", (() => k.e(742).then((() => () => k(742))))), u("jupyterlab-gitlab", "3.0.0", (() => k.e(392).then((() => () => k(392)))))
-                }
-                return e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("base64-js", "1.5.1", (() => P.e(742).then((() => () => P(742))))), u("jupyterlab-gitlab", "4.0.0", (() => P.e(232).then((() => () => P(232)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        k.g.importScripts && (e = k.g.location + "");
-        var r = k.g.document;
+        P.g.importScripts && (e = P.g.location + "");
+        var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var a = t.length - 1; a > -1 && !e;) e = t[a--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), k.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), P.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
-            n = t[1] ? r(t[1]) : [];
-        return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
-    }, n = (e, r) => {
+            a = t[1] ? r(t[1]) : [];
+        return t[2] && (a.length++, a.push.apply(a, r(t[2]))), t[3] && (a.push([]), a.push.apply(a, r(t[3]))), a
+    }, a = (e, r) => {
         e = t(e), r = t(r);
-        for (var n = 0;;) {
-            if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var a = e[n],
-                o = (typeof a)[0];
-            if (n >= r.length) return "u" == o;
-            var i = r[n],
+        for (var a = 0;;) {
+            if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
+            var n = e[a],
+                o = (typeof n)[0];
+            if (a >= r.length) return "u" == o;
+            var i = r[a],
                 u = (typeof i)[0];
             if (o != u) return "o" == o && "n" == u || "s" == u || "u" == o;
-            if ("o" != o && "u" != o && a != i) return a < i;
-            n++
+            if ("o" != o && "u" != o && n != i) return n < i;
+            a++
         }
-    }, a = e => {
+    }, n = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, u);
             return t
         }
         var i = [];
         for (o = 1; o < e.length; o++) {
             var u = e[o];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : a(u))
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : n(u))
         }
         return l();
 
         function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
-            var n = e[0],
-                a = n < 0;
-            a && (n = -n - 1);
+            var a = e[0],
+                n = a < 0;
+            n && (a = -a - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, d, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > n && !a : "" == f != a);
-                if ("u" == d) {
-                    if (!l || "u" != f) return !1
+                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > a && !n : "" == d != n);
+                if ("u" == f) {
+                    if (!l || "u" != d) return !1
                 } else if (l)
-                    if (f == d)
-                        if (u <= n) {
+                    if (d == f)
+                        if (u <= a) {
                             if (s != e[u]) return !1
                         } else {
-                            if (a ? s > e[u] : s < e[u]) return !1;
+                            if (n ? s > e[u] : s < e[u]) return !1;
                             s != e[u] && (l = !1)
                         }
-                else if ("s" != f && "n" != f) {
-                    if (a || u <= n) return !1;
+                else if ("s" != d && "n" != d) {
+                    if (n || u <= a) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || d < f != a) return !1;
+                    if (u <= a || f < d != n) return !1;
                     l = !1
-                } else "s" != f && "n" != f && (l = !1, u--)
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
-        var t = k.S[e];
-        if (!t || !k.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = P.S[e];
+        if (!t || !P.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
-        return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
+        return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
     }, l = (e, r) => {
         var t = e[r];
-        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, s = (e, r, t) => "Unsatisfied version " + r + " of shared singleton module " + e + " (required " + a(t) + ")", d = (e, r, t, n) => {
-        var a = l(e, t);
-        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(s(t, a, n)), h(e[t][a])
-    }, f = (e, r, t) => {
-        var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, p = (e, r, t, n) => {
+        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
+    }, s = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", f = (e, r, t, a) => {
+        var n = l(e, t);
+        return o(a, n) || c(s(e, t, n, a)), v(e[t][n])
+    }, d = (e, r, t) => {
+        var n = e[r];
+        return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
+    }, p = (e, r, t, a) => {
         var o = e[t];
-        return "No satisfying version (" + a(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
-    }, c = (e, r, t, n) => {
-        "undefined" != typeof console && console.warn && console.warn(p(e, r, t, n))
-    }, h = e => (e.loaded = 1, e.get()), v = (b = e => function(r, t, n, a) {
-        var o = k.I(r);
-        return o && o.then ? o.then(e.bind(e, r, k.S[r], t, n, a)) : e(r, k.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), h(f(r, t, n) || c(r, e, t, n) || u(r, t))))), g = b(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), y = b(((e, r, t, n, a) => {
-        var o = r && k.o(r, t) && f(r, t, n);
-        return o ? h(o) : a()
-    })), m = {}, j = {
-        23: () => g("default", "@jupyterlab/application", [1, 3, 1, 6]),
-        133: () => g("default", "@jupyterlab/ui-components", [1, 3, 1, 6]),
-        168: () => g("default", "@lumino/signaling", [1, 1, 4, 3]),
-        414: () => v("default", "@jupyterlab/observables", [1, 4, 1, 6]),
-        451: () => g("default", "@jupyterlab/docmanager", [1, 3, 1, 6]),
-        491: () => g("default", "@jupyterlab/services", [1, 6, 1, 6]),
-        525: () => g("default", "@jupyterlab/settingregistry", [1, 3, 1, 6]),
-        589: () => g("default", "@jupyterlab/apputils", [1, 3, 1, 6]),
-        615: () => g("default", "@lumino/widgets", [1, 1, 19, 0]),
-        920: () => g("default", "@jupyterlab/coreutils", [1, 5, 1, 6]),
-        959: () => y("default", "base64-js", [1, 1, 3, 0], (() => k.e(742).then((() => () => k(742))))),
-        994: () => g("default", "@jupyterlab/filebrowser", [1, 3, 1, 6])
-    }, w = {
-        392: [23, 133, 168, 414, 451, 491, 525, 589, 615, 920, 959, 994]
-    }, k.f.consumes = (e, r) => {
-        k.o(w, e) && w[e].forEach((e => {
-            if (k.o(m, e)) return r.push(m[e]);
+        return "No satisfying version (" + n(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
+    }, c = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, h = (e, r, t, a) => {
+        c(p(e, r, t, a))
+    }, v = e => (e.loaded = 1, e.get()), g = (b = e => function(r, t, a, n) {
+        var o = P.I(r);
+        return o && o.then ? o.then(e.bind(e, r, P.S[r], t, a, n)) : e(r, P.S[r], t, a, n)
+    })(((e, r, t, a) => (i(e, t), v(d(r, t, a) || h(r, e, t, a) || u(r, t))))), y = b(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), m = b(((e, r, t, a, n) => {
+        var o = r && P.o(r, t) && d(r, t, a);
+        return o ? v(o) : n()
+    })), j = {}, w = {
+        1: () => g("default", "@jupyterlab/observables", [1, 5, 0, 3]),
+        4: () => y("default", "@jupyterlab/application", [1, 4, 0, 3]),
+        154: () => y("default", "@jupyterlab/filebrowser", [1, 4, 0, 3]),
+        172: () => y("default", "@jupyterlab/apputils", [1, 4, 1, 3]),
+        237: () => y("default", "@jupyterlab/docmanager", [1, 4, 0, 3]),
+        580: () => y("default", "@jupyterlab/ui-components", [1, 4, 0, 3]),
+        663: () => y("default", "@jupyterlab/settingregistry", [1, 4, 0, 3]),
+        778: () => y("default", "@lumino/widgets", [1, 2, 0, 1]),
+        790: () => y("default", "@jupyterlab/services", [1, 7, 0, 3]),
+        901: () => y("default", "@lumino/signaling", [1, 2, 0, 0]),
+        959: () => m("default", "base64-js", [1, 1, 3, 0], (() => P.e(742).then((() => () => P(742))))),
+        987: () => y("default", "@jupyterlab/coreutils", [1, 6, 0, 3])
+    }, S = {
+        232: [1, 4, 154, 172, 237, 580, 663, 778, 790, 901, 959, 987]
+    }, P.f.consumes = (e, r) => {
+        P.o(S, e) && S[e].forEach((e => {
+            if (P.o(j, e)) return r.push(j[e]);
             var t = r => {
-                    m[e] = 0, k.m[e] = t => {
-                        delete k.c[e], t.exports = r()
+                    j[e] = 0, P.m[e] = t => {
+                        delete P.c[e], t.exports = r()
                     }
                 },
-                n = r => {
-                    delete m[e], k.m[e] = t => {
-                        throw delete k.c[e], r
+                a = r => {
+                    delete j[e], P.m[e] = t => {
+                        throw delete P.c[e], r
                     }
                 };
             try {
-                var a = j[e]();
-                a.then ? r.push(m[e] = a.then(t).catch(n)) : t(a)
+                var n = w[e]();
+                n.then ? r.push(j[e] = n.then(t).catch(a)) : t(n)
             } catch (e) {
-                n(e)
+                a(e)
             }
         }))
     }, (() => {
+        P.b = document.baseURI || self.location.href;
         var e = {
             836: 0
         };
-        k.f.j = (r, t) => {
-            var n = k.o(e, r) ? e[r] : void 0;
-            if (0 !== n)
-                if (n) t.push(n[2]);
+        P.f.j = (r, t) => {
+            var a = P.o(e, r) ? e[r] : void 0;
+            if (0 !== a)
+                if (a) t.push(a[2]);
                 else {
-                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                    t.push(n[2] = a);
-                    var o = k.p + k.u(r),
+                    var n = new Promise(((t, n) => a = e[r] = [t, n]));
+                    t.push(a[2] = n);
+                    var o = P.p + P.u(r),
                         i = new Error;
-                    k.l(o, (t => {
-                        if (k.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                            var a = t && ("load" === t.type ? "missing" : t.type),
+                    P.l(o, (t => {
+                        if (P.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
+                            var n = t && ("load" === t.type ? "missing" : t.type),
                                 o = t && t.target && t.target.src;
-                            i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
+                            i.message = "Loading chunk " + r + " failed.\n(" + n + ": " + o + ")", i.name = "ChunkLoadError", i.type = n, i.request = o, a[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, a, [o, i, u] = t,
+                var a, n, [o, i, u] = t,
                     l = 0;
-                for (n in i) k.o(i, n) && (k.m[n] = i[n]);
-                for (u && u(k), r && r(t); l < o.length; l++) a = o[l], k.o(e, a) && e[a] && e[a][0](), e[o[l]] = 0
+                if (o.some((r => 0 !== e[r]))) {
+                    for (a in i) P.o(i, a) && (P.m[a] = i[a]);
+                    u && u(P)
+                }
+                for (r && r(t); l < o.length; l++) n = o[l], P.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunkjupyterlab_gitlab = self.webpackChunkjupyterlab_gitlab || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })();
-    var P = k(706);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["jupyterlab-gitlab"] = P
+    })(), P.nc = void 0;
+    var T = P(706);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["jupyterlab-gitlab"] = T
 })();
```

### Comparing `jupyterlab_gitlab-3.0.0/jupyterlab_gitlab/labextension/static/third-party-licenses.json` & `jupyterlab_gitlab-4.0.0/jupyterlab_gitlab/labextension/static/third-party-licenses.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333333%*

 * *Differences: {"'packages'": "{1: {'versionInfo': '6.8.1'}, 2: {'versionInfo': '3.3.3'}}"}*

```diff
@@ -6,17 +6,17 @@
             "name": "base64-js",
             "versionInfo": "1.5.1"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
-            "versionInfo": "5.2.7"
+            "versionInfo": "6.8.1"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
-            "versionInfo": "2.0.0"
+            "versionInfo": "3.3.3"
         }
     ]
 }
```

### Comparing `jupyterlab_gitlab-3.0.0/jupyterlab_gitlab.egg-info/PKG-INFO` & `jupyterlab_gitlab-4.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,60 @@
 Metadata-Version: 2.1
-Name: jupyterlab-gitlab
-Version: 3.0.0
+Name: jupyterlab_gitlab
+Version: 4.0.0
 Summary: JupyterLab viewer for GitLab repositories
-Home-page: https://gitlab.com/beenje/jupyterlab-gitlab
-Author: Benjamin Bertrand
-Author-email: beenje@gmail.com
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3,GitLab
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: Science/Research
+Project-URL: Homepage, https://gitlab.com/beenje/jupyterlab-gitlab
+Project-URL: Bug Tracker, https://gitlab.com/beenje/jupyterlab-gitlab/issues
+Project-URL: Repository, https://gitlab.com/beenje/jupyterlab-gitlab
+Author-email: Benjamin Bertrand <beenje@gmail.com>
+License: BSD 3-Clause License
+        
+        Copyright (c) 2023, Benjamin Bertrand
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+License-File: LICENSE
+Classifier: Framework :: Jupyter
+Classifier: Framework :: Jupyter :: JupyterLab
+Classifier: Framework :: Jupyter :: JupyterLab :: 4
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Jupyter
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Requires-Dist: jupyter-server<3,>=2.0.1
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # JupyterLab GitLab
 
 A JupyterLab extension for browsing GitLab repositories (in read-only mode).
 
 This extension is based on [jupyterlab-github](https://github.com/jupyterlab/jupyterlab-github).
 All credit to the JupyterLab team, and especially [Ian Rose](https://github.com/ian-r-rose), for the github extension!
@@ -66,18 +93,19 @@
 saving files, making commits, forking repositories, etc.
 
 If you want to use git from JupyterLab, you should look at the
 [jupyterlab-git](https://github.com/jupyterlab/jupyterlab-git) extension.
 
 ## Requirements
 
-* JupyterLab >= 3.0
+* JupyterLab >= 4.0
 * JupyterLab 1.x for version 1.x
 * JupyterLab 2.x for version 2.x
 * JupyterLab 3.x for version 3.x
+* JupyterLab 4.x for version 4.x
 * A GitLab account for the server extension
 
 ## Installation
 
 ### Install the server and lab extension
 
 For Jupyterlab >= 3.0, both extensions are installed from the Python package:
@@ -214,9 +242,7 @@
 ```
 
 For JupyterLab < 3, you will also need to run the following command after removing the Python package:
 
 ```bash
 jupyter labextension uninstall jupyterlab-gitlab
 ```
-
-
```

### Comparing `jupyterlab_gitlab-3.0.0/schema/drive.json` & `jupyterlab_gitlab-4.0.0/schema/drive.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_gitlab-3.0.0/src/browser.ts` & `jupyterlab_gitlab-4.0.0/src/browser.ts`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
       this._changeGuard = false;
       this._updateErrorPanel();
       // Once we have the new listing, maybe give the file listing
       // focus. Once the input element is removed, the active element
       // appears to revert to document.body. If the user has subsequently
       // focused another element, don't focus the browser listing.
       if (document.activeElement === document.body) {
-        const listing = (this._browser.layout as PanelLayout).widgets[3];
+        const listing = (this._browser.layout as PanelLayout).widgets[1];
         listing.node.focus();
       }
     });
   }
 
   /**
    * React to the path changing for the browser.
@@ -143,39 +143,39 @@
     );
     const resource = parsePath(localPath);
     const rateLimited = this._drive.rateLimitedState.get();
     const validUser = this._drive.validUser;
 
     // If we currently have an error panel, remove it.
     if (this._errorPanel) {
-      const listing = (this._browser.layout as PanelLayout).widgets[3];
+      const listing = (this._browser.layout as PanelLayout).widgets[1];
       listing.node.removeChild(this._errorPanel.node);
       this._errorPanel.dispose();
       this._errorPanel = null;
     }
 
     // If we are being rate limited, make an error panel.
     if (rateLimited) {
       this._errorPanel = new GitLabErrorPanel(
         'You have been rate limited by GitLab! ' +
           'You will need to wait about an hour before ' +
           'continuing'
       );
-      const listing = (this._browser.layout as PanelLayout).widgets[3];
+      const listing = (this._browser.layout as PanelLayout).widgets[1];
       listing.node.appendChild(this._errorPanel.node);
       return;
     }
 
     // If we have an invalid user, make an error panel.
     if (!validUser) {
       const message = resource.user
         ? `"${resource.user}" appears to be an invalid user name!`
         : 'Please enter a GitLab user name';
       this._errorPanel = new GitLabErrorPanel(message);
-      const listing = (this._browser.layout as PanelLayout).widgets[3];
+      const listing = (this._browser.layout as PanelLayout).widgets[1];
       listing.node.appendChild(this._errorPanel.node);
       return;
     }
   }
 
   private _browser: FileBrowser;
   private _drive: GitLabDrive;
```

### Comparing `jupyterlab_gitlab-3.0.0/src/contents.ts` & `jupyterlab_gitlab-4.0.0/src/contents.ts`

 * *Files 2% similar despite different names*

```diff
@@ -192,27 +192,39 @@
     if (resource.path) {
       if (options && (options.type === 'file' || options.type === 'notebook')) {
         // Get file from repository
         // https://docs.gitlab.com/ee/api/repository_files.html#get-file-from-repository
         // GET /projects/:id/repository/files/:file_path
         // Note that:
         // - we can't use GET /projects/:id/repository/tree?path=file_path (it returns 200 with an empty [])
-        // - ref is required and hard coded to master
+        // - ref is required
         endUrl =
           URLExt.join('files', encodeURIComponent(resource.path)) +
-          '?ref=master';
+          '?ref=' +
+          this._defaultBranch;
       } else {
         // Get a list of repository files and directories in the project
         // https://docs.gitlab.com/ee/api/repositories.html#list-repository-tree
         // GET /projects/:id/repository/tree?path=path
         endUrl = URLExt.join(
           'tree',
           '?path=' + encodeURIComponent(resource.path)
         );
       }
+    } else {
+      // Retrieve and initialize the project default branch
+      const projectApi = URLExt.join(
+        'projects',
+        encodeURIComponent(resource.user) +
+          '%2F' +
+          encodeURIComponent(resource.repository)
+      );
+      this._apiRequest<GitLabRepo>(projectApi).then(contents => {
+        this._defaultBranch = contents.default_branch;
+      });
     }
     // Use namespaced API calls: resource.user + '%2F' + resource.repository
     // See https://docs.gitlab.com/ee/api/README.html#namespaced-path-encoding
     const apiPath = URLExt.join(
       'projects',
       encodeURIComponent(resource.user) +
         '%2F' +
@@ -287,15 +299,17 @@
         encodeURIComponent(resource.user) +
           '%2F' +
           encodeURIComponent(resource.repository),
         'repository',
         'files',
         encodeURIComponent(resource.path),
         'raw'
-      ) + '?ref=master';
+      ) +
+      '?ref=' +
+      this._defaultBranch;
     return Promise.resolve(rawUrl);
   }
 
   /**
    * Create a new untitled file or directory in the specified directory path.
    *
    * @param options: The options used to create the file.
@@ -504,14 +518,15 @@
       }
     });
   }
 
   private _baseUrl = '';
   private _accessToken: string | null | undefined;
   private _validUser = false;
+  private _defaultBranch = '';
   private _serverSettings: ServerConnection.ISettings;
   private _useProxy: Promise<boolean>;
   private _fileTypeForPath: (path: string) => DocumentRegistry.IFileType;
   private _isDisposed = false;
   private _fileChanged = new Signal<this, Contents.IChangedArgs>(this);
 }
```

### Comparing `jupyterlab_gitlab-3.0.0/src/gitlab.ts` & `jupyterlab_gitlab-4.0.0/src/gitlab.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_gitlab-3.0.0/src/index.ts` & `jupyterlab_gitlab-4.0.0/src/index.ts`

 * *Files 7% similar despite different names*

```diff
@@ -5,35 +5,47 @@
   ILayoutRestorer,
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 
 import { Dialog, showDialog } from '@jupyterlab/apputils';
 
+import { LabIcon } from '@jupyterlab/ui-components';
+
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 
 import { IDocumentManager } from '@jupyterlab/docmanager';
 
 import { IFileBrowserFactory } from '@jupyterlab/filebrowser';
 
 import { GitLabDrive, DEFAULT_GITLAB_BASE_URL } from './contents';
 
 import { GitLabFileBrowser } from './browser';
 
+import GitLabSvgStr from '../style/gitlab_stacked_wm_grayscale.svg';
+
 /**
  * GitLab filebrowser plugin state namespace.
  */
 const NAMESPACE = 'gitlab-filebrowser';
 
 /**
  * The ID for the plugin.
  */
 const PLUGIN_ID = 'jupyterlab-gitlab:drive';
 
 /**
+ * GitLab Icon class.
+ */
+export const gitLabIcon = new LabIcon({
+  name: `${NAMESPACE}:icon`,
+  svgstr: GitLabSvgStr
+});
+
+/**
  * The JupyterLab plugin for the GitLab Filebrowser.
  */
 const fileBrowserPlugin: JupyterFrontEndPlugin<void> = {
   id: PLUGIN_ID,
   requires: [
     IDocumentManager,
     IFileBrowserFactory,
@@ -65,15 +77,16 @@
   const browser = factory.createFileBrowser(NAMESPACE, {
     driveName: drive.name,
     refreshInterval: 300000
   });
 
   const gitLabBrowser = new GitLabFileBrowser(browser, drive);
 
-  gitLabBrowser.title.iconClass = 'jp-GitLab-icon jp-SideBar-tabIcon';
+  gitLabBrowser.title.icon = gitLabIcon;
+  gitLabBrowser.title.iconClass = 'jp-SideBar-tabIcon';
   gitLabBrowser.title.caption = 'Browse GitLab';
 
   gitLabBrowser.id = 'gitlab-file-browser';
 
   // Add the file browser widget to the application restorer.
   restorer.add(gitLabBrowser, NAMESPACE);
   app.shell.add(gitLabBrowser, 'left', { rank: 102 });
```

### Comparing `jupyterlab_gitlab-3.0.0/style/base.css` & `jupyterlab_gitlab-4.0.0/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_gitlab-3.0.0/style/gitlab-logo-extra-whitespace.svg` & `jupyterlab_gitlab-4.0.0/style/gitlab-logo-extra-whitespace.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_gitlab-3.0.0/style/gitlab_stacked_wm_grayscale.svg` & `jupyterlab_gitlab-4.0.0/style/gitlab_stacked_wm_grayscale.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_gitlab-3.0.0/tsconfig.json` & `jupyterlab_gitlab-4.0.0/tsconfig.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993421052631579%*

 * *Differences: {"'compilerOptions'": "{'target': 'ES2018'}"}*

```diff
@@ -13,14 +13,14 @@
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
         "strictNullChecks": true,
-        "target": "es2017",
+        "target": "ES2018",
         "types": []
     },
     "include": [
         "src/*"
     ]
 }
```

### Comparing `jupyterlab_gitlab-3.0.0/tslint.json` & `jupyterlab_gitlab-4.0.0/tslint.json`

 * *Files identical despite different names*


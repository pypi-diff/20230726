# Comparing `tmp/airtime-1.0.1.tar.gz` & `tmp/airtime-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtime-1.0.1.tar", last modified: Sun Jul 23 21:24:21 2023, max compression
+gzip compressed data, was "airtime-1.0.2.tar", last modified: Wed Jul 26 15:57:46 2023, max compression
```

## Comparing `airtime-1.0.1.tar` & `airtime-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jana       (501) staff       (20)        0 2023-07-23 21:24:21.478206 airtime-1.0.1/
--rw-r--r--   0 jana       (501) staff       (20)    34523 2023-07-20 16:57:33.000000 airtime-1.0.1/LICENSE
--rw-r--r--   0 jana       (501) staff       (20)     3360 2023-07-23 21:24:21.478098 airtime-1.0.1/PKG-INFO
--rw-r--r--   0 jana       (501) staff       (20)     2572 2023-07-23 21:20:56.000000 airtime-1.0.1/README.md
-drwxr-xr-x   0 jana       (501) staff       (20)        0 2023-07-23 21:24:21.477091 airtime-1.0.1/airtime/
--rw-r--r--   0 jana       (501) staff       (20)      104 2023-07-23 21:18:54.000000 airtime-1.0.1/airtime/__init__.py
--rw-r--r--   0 jana       (501) staff       (20)     3309 2023-07-23 20:05:53.000000 airtime-1.0.1/airtime/teams_analyzer.py
-drwxr-xr-x   0 jana       (501) staff       (20)        0 2023-07-23 21:24:21.477908 airtime-1.0.1/airtime/tests/
--rw-r--r--   0 jana       (501) staff       (20)        0 2023-07-23 21:19:18.000000 airtime-1.0.1/airtime/tests/__init__.py
--rw-r--r--   0 jana       (501) staff       (20)     3449 2023-07-23 20:05:47.000000 airtime-1.0.1/airtime/tests/test_teams_analyzer.py
--rw-r--r--   0 jana       (501) staff       (20)     3327 2023-07-23 20:05:50.000000 airtime-1.0.1/airtime/tests/test_zoom_analyzer.py
--rw-r--r--   0 jana       (501) staff       (20)     3085 2023-07-23 20:05:57.000000 airtime-1.0.1/airtime/zoom_analyzer.py
-drwxr-xr-x   0 jana       (501) staff       (20)        0 2023-07-23 21:24:21.477556 airtime-1.0.1/airtime.egg-info/
--rw-r--r--   0 jana       (501) staff       (20)     3360 2023-07-23 21:24:21.000000 airtime-1.0.1/airtime.egg-info/PKG-INFO
--rw-r--r--   0 jana       (501) staff       (20)      320 2023-07-23 21:24:21.000000 airtime-1.0.1/airtime.egg-info/SOURCES.txt
--rw-r--r--   0 jana       (501) staff       (20)        1 2023-07-23 21:24:21.000000 airtime-1.0.1/airtime.egg-info/dependency_links.txt
--rw-r--r--   0 jana       (501) staff       (20)        8 2023-07-23 21:24:21.000000 airtime-1.0.1/airtime.egg-info/top_level.txt
--rw-r--r--   0 jana       (501) staff       (20)       38 2023-07-23 21:24:21.478259 airtime-1.0.1/setup.cfg
--rw-r--r--   0 jana       (501) staff       (20)     1076 2023-07-23 21:20:37.000000 airtime-1.0.1/setup.py
+drwxr-xr-x   0 jana       (501) staff       (20)        0 2023-07-26 15:57:46.283802 airtime-1.0.2/
+-rw-r--r--   0 jana       (501) staff       (20)    34523 2023-07-20 16:57:33.000000 airtime-1.0.2/LICENSE
+-rw-r--r--   0 jana       (501) staff       (20)     4754 2023-07-26 15:57:46.283683 airtime-1.0.2/PKG-INFO
+-rw-r--r--   0 jana       (501) staff       (20)     3966 2023-07-26 15:54:20.000000 airtime-1.0.2/README.md
+drwxr-xr-x   0 jana       (501) staff       (20)        0 2023-07-26 15:57:46.282348 airtime-1.0.2/airtime/
+-rw-r--r--   0 jana       (501) staff       (20)      104 2023-07-23 21:18:54.000000 airtime-1.0.2/airtime/__init__.py
+-rw-r--r--   0 jana       (501) staff       (20)     3309 2023-07-23 20:05:53.000000 airtime-1.0.2/airtime/teams_analyzer.py
+drwxr-xr-x   0 jana       (501) staff       (20)        0 2023-07-26 15:57:46.283400 airtime-1.0.2/airtime/tests/
+-rw-r--r--   0 jana       (501) staff       (20)        0 2023-07-23 21:19:18.000000 airtime-1.0.2/airtime/tests/__init__.py
+-rw-r--r--   0 jana       (501) staff       (20)     3449 2023-07-23 20:05:47.000000 airtime-1.0.2/airtime/tests/test_teams_analyzer.py
+-rw-r--r--   0 jana       (501) staff       (20)     3327 2023-07-23 20:05:50.000000 airtime-1.0.2/airtime/tests/test_zoom_analyzer.py
+-rw-r--r--   0 jana       (501) staff       (20)     3085 2023-07-23 20:05:57.000000 airtime-1.0.2/airtime/zoom_analyzer.py
+drwxr-xr-x   0 jana       (501) staff       (20)        0 2023-07-26 15:57:46.282931 airtime-1.0.2/airtime.egg-info/
+-rw-r--r--   0 jana       (501) staff       (20)     4754 2023-07-26 15:57:46.000000 airtime-1.0.2/airtime.egg-info/PKG-INFO
+-rw-r--r--   0 jana       (501) staff       (20)      320 2023-07-26 15:57:46.000000 airtime-1.0.2/airtime.egg-info/SOURCES.txt
+-rw-r--r--   0 jana       (501) staff       (20)        1 2023-07-26 15:57:46.000000 airtime-1.0.2/airtime.egg-info/dependency_links.txt
+-rw-r--r--   0 jana       (501) staff       (20)        8 2023-07-26 15:57:46.000000 airtime-1.0.2/airtime.egg-info/top_level.txt
+-rw-r--r--   0 jana       (501) staff       (20)       38 2023-07-26 15:57:46.283848 airtime-1.0.2/setup.cfg
+-rw-r--r--   0 jana       (501) staff       (20)     1076 2023-07-26 15:54:30.000000 airtime-1.0.2/setup.py
```

### Comparing `airtime-1.0.1/LICENSE` & `airtime-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airtime-1.0.1/PKG-INFO` & `airtime-1.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtime
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for analyzing transcripts
 Home-page: https://github.com/jcontd/airtime
 Author: Jana M. Perkins
 Author-email: mailroom@jcontd.com
 License: GNU Affero General Public License v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,25 +16,41 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![License: AGPL-3.0](https://img.shields.io/badge/License-AGPL--3.0-brightgreen.svg)](https://www.gnu.org/licenses/agpl-3.0)
-![Version](https://img.shields.io/badge/version-v1.0.1-blue)
+![Version](https://img.shields.io/badge/version-v1.0.2-blue)
 
 # Airtime
 
-This package contains Python scripts for analyzing meeting transcripts from Zoom and Microsoft Teams meetings. The scripts read the transcript files, calculate spoken word totals for each speaker, and print out the analyzed results.
+This package contains Python scripts for analyzing transcript files from Zoom and Microsoft Teams meetings.
 
-The intended purpose of this package is to allow users to determine what percentage of a given meeting was allocated to which speaker(s), with the goal of fostering better collaborative environments among teams in future meetings.
+These scripts function by reading in a transcript, calculating the spoken word totals for each of its speakers, and displaying the analyzed results. The intended purpose of this package is to allow users to determine what percentage of a given meeting was allocated to which speaker(s).
+
+## Why this matters
+
+Airtime is a project management tool which operates from the assumption that teams and organizations could only stand to benefit from an increase in perspectives from and participation among their members. The first step, of course, remains to create good teams. Once that’s been accomplished, the second step is to then allow all those involved the necessary time and space to make the contributions for which their expertise was initially sought out.
+
+This tool aims to provide those who regularly undertake collaborative work in fields that base their decisions on statistical findings with the necessary data to foster more genuinely collaborative work environments. It’s one thing, in other words, for a team member to convey to their project lead that they often have their contributions minimized in meetings while others monopolize the floor; it’s quite another for them to be able to demonstrate that the data support their experiences and that there’s room to move forward with a data-driven solution.
+
+## Key features
+
+✅ Ease of use: Just 3 lines of code from installation to analysis.
+
+✅ Privacy and security: All analyses run locally on your machine.
+
+✅ Efficient computing: Lightweight algorithms for fast processing times.
+
+*Coming soon: a step-by-step implementation guide for non-developers with no prior Python experience. If you’d like to be notified when this becomes available, please send me an email.*
 
 ## Version
 
-The latest version of this package is v1.0.1.
+The latest version of this package is v1.0.2.
 
 ## Installation and requirements
 
 ```
 pip install airtime
 ```
 
@@ -83,15 +99,15 @@
 SPEAKER TOTALS
 - Holmes: 900 words (90.0% of meeting)
 - Watson: 100 words (10.0% of meeting)
 ```
 
 ## Contributing
 
-Contributions to this package are welcome, and especially in the form of introducing additional transcript formats from other services (e.g., Google Meet). Please open an issue to discuss your idea or submit a Pull Request.
+Contributions to this package are welcome, and especially in the form of introducing additional transcript formats from other services (e.g., Google Meet). Please open an issue to discuss your idea or submit a pull request.
 
 ## License
 
 This package is licensed under the terms of the GNU Affero General Public License (GNU AGPL).
 
 ## Contact information
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `airtime-1.0.1/README.md` & `airtime-1.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,35 @@
 [![License: AGPL-3.0](https://img.shields.io/badge/License-AGPL--3.0-brightgreen.svg)](https://www.gnu.org/licenses/agpl-3.0)
-![Version](https://img.shields.io/badge/version-v1.0.1-blue)
+![Version](https://img.shields.io/badge/version-v1.0.2-blue)
 
 # Airtime
 
-This package contains Python scripts for analyzing meeting transcripts from Zoom and Microsoft Teams meetings. The scripts read the transcript files, calculate spoken word totals for each speaker, and print out the analyzed results.
+This package contains Python scripts for analyzing transcript files from Zoom and Microsoft Teams meetings.
 
-The intended purpose of this package is to allow users to determine what percentage of a given meeting was allocated to which speaker(s), with the goal of fostering better collaborative environments among teams in future meetings.
+These scripts function by reading in a transcript, calculating the spoken word totals for each of its speakers, and displaying the analyzed results. The intended purpose of this package is to allow users to determine what percentage of a given meeting was allocated to which speaker(s).
+
+## Why this matters
+
+Airtime is a project management tool which operates from the assumption that teams and organizations could only stand to benefit from an increase in perspectives from and participation among their members. The first step, of course, remains to create good teams. Once that’s been accomplished, the second step is to then allow all those involved the necessary time and space to make the contributions for which their expertise was initially sought out.
+
+This tool aims to provide those who regularly undertake collaborative work in fields that base their decisions on statistical findings with the necessary data to foster more genuinely collaborative work environments. It’s one thing, in other words, for a team member to convey to their project lead that they often have their contributions minimized in meetings while others monopolize the floor; it’s quite another for them to be able to demonstrate that the data support their experiences and that there’s room to move forward with a data-driven solution.
+
+## Key features
+
+✅ Ease of use: Just 3 lines of code from installation to analysis.
+
+✅ Privacy and security: All analyses run locally on your machine.
+
+✅ Efficient computing: Lightweight algorithms for fast processing times.
+
+*Coming soon: a step-by-step implementation guide for non-developers with no prior Python experience. If you’d like to be notified when this becomes available, please send me an email.*
 
 ## Version
 
-The latest version of this package is v1.0.1.
+The latest version of this package is v1.0.2.
 
 ## Installation and requirements
 
 ```
 pip install airtime
 ```
 
@@ -62,15 +78,15 @@
 SPEAKER TOTALS
 - Holmes: 900 words (90.0% of meeting)
 - Watson: 100 words (10.0% of meeting)
 ```
 
 ## Contributing
 
-Contributions to this package are welcome, and especially in the form of introducing additional transcript formats from other services (e.g., Google Meet). Please open an issue to discuss your idea or submit a Pull Request.
+Contributions to this package are welcome, and especially in the form of introducing additional transcript formats from other services (e.g., Google Meet). Please open an issue to discuss your idea or submit a pull request.
 
 ## License
 
 This package is licensed under the terms of the GNU Affero General Public License (GNU AGPL).
 
 ## Contact information
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `airtime-1.0.1/airtime/teams_analyzer.py` & `airtime-1.0.2/airtime/teams_analyzer.py`

 * *Files identical despite different names*

### Comparing `airtime-1.0.1/airtime/tests/test_teams_analyzer.py` & `airtime-1.0.2/airtime/tests/test_teams_analyzer.py`

 * *Files identical despite different names*

### Comparing `airtime-1.0.1/airtime/tests/test_zoom_analyzer.py` & `airtime-1.0.2/airtime/tests/test_zoom_analyzer.py`

 * *Files identical despite different names*

### Comparing `airtime-1.0.1/airtime/zoom_analyzer.py` & `airtime-1.0.2/airtime/zoom_analyzer.py`

 * *Files identical despite different names*

### Comparing `airtime-1.0.1/airtime.egg-info/PKG-INFO` & `airtime-1.0.2/airtime.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtime
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for analyzing transcripts
 Home-page: https://github.com/jcontd/airtime
 Author: Jana M. Perkins
 Author-email: mailroom@jcontd.com
 License: GNU Affero General Public License v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,25 +16,41 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![License: AGPL-3.0](https://img.shields.io/badge/License-AGPL--3.0-brightgreen.svg)](https://www.gnu.org/licenses/agpl-3.0)
-![Version](https://img.shields.io/badge/version-v1.0.1-blue)
+![Version](https://img.shields.io/badge/version-v1.0.2-blue)
 
 # Airtime
 
-This package contains Python scripts for analyzing meeting transcripts from Zoom and Microsoft Teams meetings. The scripts read the transcript files, calculate spoken word totals for each speaker, and print out the analyzed results.
+This package contains Python scripts for analyzing transcript files from Zoom and Microsoft Teams meetings.
 
-The intended purpose of this package is to allow users to determine what percentage of a given meeting was allocated to which speaker(s), with the goal of fostering better collaborative environments among teams in future meetings.
+These scripts function by reading in a transcript, calculating the spoken word totals for each of its speakers, and displaying the analyzed results. The intended purpose of this package is to allow users to determine what percentage of a given meeting was allocated to which speaker(s).
+
+## Why this matters
+
+Airtime is a project management tool which operates from the assumption that teams and organizations could only stand to benefit from an increase in perspectives from and participation among their members. The first step, of course, remains to create good teams. Once that’s been accomplished, the second step is to then allow all those involved the necessary time and space to make the contributions for which their expertise was initially sought out.
+
+This tool aims to provide those who regularly undertake collaborative work in fields that base their decisions on statistical findings with the necessary data to foster more genuinely collaborative work environments. It’s one thing, in other words, for a team member to convey to their project lead that they often have their contributions minimized in meetings while others monopolize the floor; it’s quite another for them to be able to demonstrate that the data support their experiences and that there’s room to move forward with a data-driven solution.
+
+## Key features
+
+✅ Ease of use: Just 3 lines of code from installation to analysis.
+
+✅ Privacy and security: All analyses run locally on your machine.
+
+✅ Efficient computing: Lightweight algorithms for fast processing times.
+
+*Coming soon: a step-by-step implementation guide for non-developers with no prior Python experience. If you’d like to be notified when this becomes available, please send me an email.*
 
 ## Version
 
-The latest version of this package is v1.0.1.
+The latest version of this package is v1.0.2.
 
 ## Installation and requirements
 
 ```
 pip install airtime
 ```
 
@@ -83,15 +99,15 @@
 SPEAKER TOTALS
 - Holmes: 900 words (90.0% of meeting)
 - Watson: 100 words (10.0% of meeting)
 ```
 
 ## Contributing
 
-Contributions to this package are welcome, and especially in the form of introducing additional transcript formats from other services (e.g., Google Meet). Please open an issue to discuss your idea or submit a Pull Request.
+Contributions to this package are welcome, and especially in the form of introducing additional transcript formats from other services (e.g., Google Meet). Please open an issue to discuss your idea or submit a pull request.
 
 ## License
 
 This package is licensed under the terms of the GNU Affero General Public License (GNU AGPL).
 
 ## Contact information
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `airtime-1.0.1/setup.py` & `airtime-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setup(
     name="airtime",
-    version="1.0.1",
+    version="1.0.2",
     author="Jana M. Perkins",
     author_email="mailroom@jcontd.com",
     description="""A package for analyzing transcripts
     from Zoom and Microsoft Teams meetings""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jcontd/airtime",
```


# Comparing `tmp/UW-RestClients-AdSel-1.9.1.tar.gz` & `tmp/UW-RestClients-AdSel-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UW-RestClients-AdSel-1.9.1.tar", last modified: Fri Jul 21 23:25:07 2023, max compression
+gzip compressed data, was "UW-RestClients-AdSel-1.9.2.tar", last modified: Wed Jul 26 21:30:03 2023, max compression
```

## Comparing `UW-RestClients-AdSel-1.9.1.tar` & `UW-RestClients-AdSel-1.9.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.014321 UW-RestClients-AdSel-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      644 2023-07-21 23:25:07.014321 UW-RestClients-AdSel-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.006321 UW-RestClients-AdSel-1.9.1/UW_RestClients_AdSel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      644 2023-07-21 23:25:06.000000 UW-RestClients-AdSel-1.9.1/UW_RestClients_AdSel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2389 2023-07-21 23:25:06.000000 UW-RestClients-AdSel-1.9.1/UW_RestClients_AdSel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 23:25:06.000000 UW-RestClients-AdSel-1.9.1/UW_RestClients_AdSel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-21 23:25:06.000000 UW-RestClients-AdSel-1.9.1/UW_RestClients_AdSel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-21 23:25:06.000000 UW-RestClients-AdSel-1.9.1/UW_RestClients_AdSel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-21 23:25:07.014321 UW-RestClients-AdSel-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-21 23:25:05.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)    20643 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      332 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/dao.py
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    10671 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.006321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.006321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.006321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.006321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/academicqtr
--rw-r--r--   0 runner    (1001) docker     (122)     1883 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/activities
--rw-r--r--   0 runner    (1001) docker     (122)      503 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/activities?Page=2
--rw-r--r--   0 runner    (1001) docker     (122)      502 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/activities?assignmentType=major
--rw-r--r--   0 runner    (1001) docker     (122)      938 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage
--rw-r--r--   0 runner    (1001) docker     (122)     1772 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage&systemKey=12345
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/
--rw-r--r--   0 runner    (1001) docker     (122)     1234 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20194
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20201/
--rw-r--r--   0 runner    (1001) docker     (122)      368 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20201/0
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/major/
--rw-r--r--   0 runner    (1001) docker     (122)      568 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/major/1
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/major/2
--rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/majors
--rw-r--r--   0 runner    (1001) docker     (122)     2738 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/majorvalues
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.006321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/0/
--rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/0/123
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/0/all
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/
--rw-r--r--   0 runner    (1001) docker     (122)     2073 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/0
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/assignments/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/assignments/cohort/
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/assignments/cohort/bulk
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/assignments/departmentalDecision
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/assignments/major
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/assignments/purpleAndGold
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/cohorts/
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/cohorts/0
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/cohorts/0?Page=2
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/cohorts/1
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.010321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=0
--rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=1
--rw-r--r--   0 runner    (1001) docker     (122)     3477 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/filter
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.006321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.014321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.014321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/0/
--rw-r--r--   0 runner    (1001) docker     (122)      312 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_BIOL_1
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_CHEM_1
--rw-r--r--   0 runner    (1001) docker     (122)      328 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_CSE_1
--rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=1&Limit=100
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=2&Limit=100
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/1?Page=1&Limit=100
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.014321 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/workspaces/
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/workspaces/20194
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 23:25:07.014321 UW-RestClients-AdSel-1.9.1/uw_adsel/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11871 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/tests/test_adsel.py
--rw-r--r--   0 runner    (1001) docker     (122)      119 2023-07-21 23:24:49.000000 UW-RestClients-AdSel-1.9.1/uw_adsel/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.836229 UW-RestClients-AdSel-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-07-26 21:30:03.836229 UW-RestClients-AdSel-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/UW_RestClients_AdSel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-07-26 21:30:03.000000 UW-RestClients-AdSel-1.9.2/UW_RestClients_AdSel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2389 2023-07-26 21:30:03.000000 UW-RestClients-AdSel-1.9.2/UW_RestClients_AdSel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 21:30:03.000000 UW-RestClients-AdSel-1.9.2/UW_RestClients_AdSel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-26 21:30:03.000000 UW-RestClients-AdSel-1.9.2/UW_RestClients_AdSel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-26 21:30:03.000000 UW-RestClients-AdSel-1.9.2/UW_RestClients_AdSel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-26 21:30:03.836229 UW-RestClients-AdSel-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-26 21:30:02.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)    20955 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/dao.py
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10778 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.828229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.828229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.828229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.828229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/academicqtr
+-rw-r--r--   0 runner    (1001) docker     (122)     1883 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/activities
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/activities?Page=2
+-rw-r--r--   0 runner    (1001) docker     (122)      502 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/activities?assignmentType=major
+-rw-r--r--   0 runner    (1001) docker     (122)      938 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage
+-rw-r--r--   0 runner    (1001) docker     (122)     1772 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage&systemKey=12345
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1234 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20194
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20201/
+-rw-r--r--   0 runner    (1001) docker     (122)      368 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20201/0
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/major/
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/major/1
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/major/2
+-rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/majors
+-rw-r--r--   0 runner    (1001) docker     (122)     2738 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/majorvalues
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.828229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/0/123
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/0/all
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/
+-rw-r--r--   0 runner    (1001) docker     (122)     2073 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/0
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/assignments/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/assignments/cohort/
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/assignments/cohort/bulk
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/assignments/departmentalDecision
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/assignments/major
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/assignments/purpleAndGold
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/cohorts/
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/cohorts/0
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/cohorts/0?Page=2
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/cohorts/1
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=0
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=1
+-rw-r--r--   0 runner    (1001) docker     (122)     3477 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/filter
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.828229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/0/
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_BIOL_1
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_CHEM_1
+-rw-r--r--   0 runner    (1001) docker     (122)      328 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/0/0_CSE_1
+-rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=1&Limit=100
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=2&Limit=100
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/1?Page=1&Limit=100
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/workspaces/20194
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 21:30:03.832229 UW-RestClients-AdSel-1.9.2/uw_adsel/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11871 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/tests/test_adsel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-07-26 21:29:53.000000 UW-RestClients-AdSel-1.9.2/uw_adsel/utilities.py
```

### Comparing `UW-RestClients-AdSel-1.9.1/LICENSE` & `UW-RestClients-AdSel-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/PKG-INFO` & `UW-RestClients-AdSel-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UW-RestClients-AdSel
-Version: 1.9.1
+Version: 1.9.2
 Summary: A library for connecting to the AdSel API at the University of Washington
 Home-page: https://github.com/uw-it-aca/uw-restclients-adsel
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `UW-RestClients-AdSel-1.9.1/README.md` & `UW-RestClients-AdSel-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/UW_RestClients_AdSel.egg-info/PKG-INFO` & `UW-RestClients-AdSel-1.9.2/UW_RestClients_AdSel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UW-RestClients-AdSel
-Version: 1.9.1
+Version: 1.9.2
 Summary: A library for connecting to the AdSel API at the University of Washington
 Home-page: https://github.com/uw-it-aca/uw-restclients-adsel
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `UW-RestClients-AdSel-1.9.1/UW_RestClients_AdSel.egg-info/SOURCES.txt` & `UW-RestClients-AdSel-1.9.2/UW_RestClients_AdSel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/setup.py` & `UW-RestClients-AdSel-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/__init__.py` & `UW-RestClients-AdSel-1.9.2/uw_adsel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,14 +425,20 @@
         response = self._get_resource(url)
         return response
 
     def create_workspace(self, workspace):
         url = "{}/admin/workspace".format(self.API)
         return self._post_resource(url, workspace.json_data())
 
+    def duplicate_workspace(self, workspace_id, workspace_name):
+        url = "{}/admin/workspace/duplicate".format(self.API)
+        return self._post_resource(url,
+                                   {"duplicateWorkspaceName": workspace_name,
+                                    "workspaceId": workspace_id})
+
     def get_workspaces_by_qtr(self, qtr):
         url = "{}/workspaces/{}".format(self.API, qtr)
         response = self._get_resource(url)
         workspaces = self._workspaces_from_json(response)
         return workspaces
 
     def _workspaces_from_json(self, response):
```

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/models.py` & `UW-RestClients-AdSel-1.9.2/uw_adsel/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,17 @@
 
 
 class Workspace(models.Model):
     academic_qtr_id = models.IntegerField()
     workspace_id = models.IntegerField()
     workspace_name = models.CharField(max_length=255)
     owner_alias = models.CharField(max_length=255)
+    source_workspace_id = models.IntegerField()
 
     def json_data(self):
         return {
             "academicQtrKeyId": self.academic_qtr_id,
             "workspaceId": self.workspace_id,
             "workspaceName": self.workspace_name,
-            "ownerAlias": self.owner_alias
+            "ownerAlias": self.owner_alias,
+            "sourceWorkspaceId": self.source_workspace_id
         }
```

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/activities` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/activities`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage&systemKey=12345` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/activities?netid=javerage&systemKey=12345`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20194` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/cohorts/20194`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/major/1` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/major/1`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/major/2` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/major/2`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/majors` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/majors`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/admin/majorvalues` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/admin/majorvalues`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/0/123` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/0/123`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/0/all` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/0/all`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/0` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/applications/SystemKeys/0`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/cohorts/0` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/cohorts/0`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/cohorts/0?Page=2` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/cohorts/0?Page=2`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/cohorts/1` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/cohorts/1`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=0` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=0`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=1` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/departmentaldecisions/GetWithCounts?academicQtrKeyId=1`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/filter` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/filter`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=1&Limit=100` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=1&Limit=100`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=2&Limit=100` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/0?Page=2&Limit=100`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/majors/details/1?Page=1&Limit=100` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/majors/details/1?Page=1&Limit=100`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/resources/adsel/file/api/v1/workspaces/20194` & `UW-RestClients-AdSel-1.9.2/uw_adsel/resources/adsel/file/api/v1/workspaces/20194`

 * *Files identical despite different names*

### Comparing `UW-RestClients-AdSel-1.9.1/uw_adsel/tests/test_adsel.py` & `UW-RestClients-AdSel-1.9.2/uw_adsel/tests/test_adsel.py`

 * *Files identical despite different names*


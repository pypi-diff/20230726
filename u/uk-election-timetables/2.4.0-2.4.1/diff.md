# Comparing `tmp/uk-election-timetables-2.4.0.tar.gz` & `tmp/uk-election-timetables-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uk-election-timetables-2.4.0.tar", last modified: Tue Feb 14 15:10:29 2023, max compression
+gzip compressed data, was "uk-election-timetables-2.4.1.tar", last modified: Wed Jul 26 13:19:09 2023, max compression
```

## Comparing `uk-election-timetables-2.4.0.tar` & `uk-election-timetables-2.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 15:10:29.472344 uk-election-timetables-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-02-14 15:10:29.472344 uk-election-timetables-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 15:10:29.472344 uk-election-timetables-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 15:10:29.468344 uk-election-timetables-2.4.0/uk_election_timetables/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/uk_election_timetables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68957 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/uk_election_timetables/bank-holidays.json
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/uk_election_timetables/bank_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/uk_election_timetables/calendars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/uk_election_timetables/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/uk_election_timetables/election.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/uk_election_timetables/election_ids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 15:10:29.472344 uk-election-timetables-2.4.0/uk_election_timetables/elections/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/uk_election_timetables/elections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/uk_election_timetables/elections/greater_london_assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/uk_election_timetables/elections/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/uk_election_timetables/elections/mayor.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/uk_election_timetables/elections/northern_ireland_assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/uk_election_timetables/elections/police_and_crime_commissioner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/uk_election_timetables/elections/scottish_parliament.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/uk_election_timetables/elections/senedd_cymru.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-02-14 15:10:19.000000 uk-election-timetables-2.4.0/uk_election_timetables/elections/uk_parliament.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 15:10:29.468344 uk-election-timetables-2.4.0/uk_election_timetables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-02-14 15:10:29.000000 uk-election-timetables-2.4.0/uk_election_timetables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-02-14 15:10:29.000000 uk-election-timetables-2.4.0/uk_election_timetables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 15:10:29.000000 uk-election-timetables-2.4.0/uk_election_timetables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-14 15:10:29.000000 uk-election-timetables-2.4.0/uk_election_timetables.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:19:09.525026 uk-election-timetables-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-26 13:19:09.525026 uk-election-timetables-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 13:19:09.525026 uk-election-timetables-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:19:09.525026 uk-election-timetables-2.4.1/uk_election_timetables/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/uk_election_timetables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68957 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/uk_election_timetables/bank-holidays.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/uk_election_timetables/bank_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/uk_election_timetables/calendars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/uk_election_timetables/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/uk_election_timetables/election.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/uk_election_timetables/election_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:19:09.525026 uk-election-timetables-2.4.1/uk_election_timetables/elections/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/uk_election_timetables/elections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/uk_election_timetables/elections/greater_london_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/uk_election_timetables/elections/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/uk_election_timetables/elections/mayor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/uk_election_timetables/elections/northern_ireland_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/uk_election_timetables/elections/police_and_crime_commissioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/uk_election_timetables/elections/scottish_parliament.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/uk_election_timetables/elections/senedd_cymru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-26 13:18:58.000000 uk-election-timetables-2.4.1/uk_election_timetables/elections/uk_parliament.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:19:09.525026 uk-election-timetables-2.4.1/uk_election_timetables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-26 13:19:09.000000 uk-election-timetables-2.4.1/uk_election_timetables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-26 13:19:09.000000 uk-election-timetables-2.4.1/uk_election_timetables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:19:09.000000 uk-election-timetables-2.4.1/uk_election_timetables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 13:19:09.000000 uk-election-timetables-2.4.1/uk_election_timetables.egg-info/top_level.txt
```

### Comparing `uk-election-timetables-2.4.0/LICENSE.md` & `uk-election-timetables-2.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uk-election-timetables-2.4.0/PKG-INFO` & `uk-election-timetables-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uk-election-timetables
-Version: 2.4.0
+Version: 2.4.1
 Summary: Derives significant dates for UK elections
 Home-page: https://github.com/DemocracyClub/uk-election-timetables
 Author: Alex Wilson
 Author-email: alex+github@probablyfine.co.uk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
```

### Comparing `uk-election-timetables-2.4.0/README.md` & `uk-election-timetables-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `uk-election-timetables-2.4.0/setup.py` & `uk-election-timetables-2.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `uk-election-timetables-2.4.0/uk_election_timetables/bank-holidays.json` & `uk-election-timetables-2.4.1/uk_election_timetables/bank-holidays.json`

 * *Files identical despite different names*

### Comparing `uk-election-timetables-2.4.0/uk_election_timetables/bank_holidays.py` & `uk-election-timetables-2.4.1/uk_election_timetables/bank_holidays.py`

 * *Files identical despite different names*

### Comparing `uk-election-timetables-2.4.0/uk_election_timetables/calendars.py` & `uk-election-timetables-2.4.1/uk_election_timetables/calendars.py`

 * *Files identical despite different names*

### Comparing `uk-election-timetables-2.4.0/uk_election_timetables/date.py` & `uk-election-timetables-2.4.1/uk_election_timetables/date.py`

 * *Files identical despite different names*

### Comparing `uk-election-timetables-2.4.0/uk_election_timetables/election.py` & `uk-election-timetables-2.4.1/uk_election_timetables/election.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,21 @@
     @property
     def postal_vote_application_deadline(self) -> date:
         """
         Calculates the postal vote application deadline for this Election
 
         This is set out in `The Representation of the People (England and Wales) Regulations 2001 <https://www.legislation.gov.uk/uksi/2001/341/regulation/56/made>`_.
 
+        In Northern Ireland, this is set out in `The Representation of the People (Northern Ireland) Regulations 2008 <https://www.legislation.gov.uk/uksi/2008/1741/regulation/61/made>`
+
         :return: a datetime representing the postal vote application deadline
         """
+        if self.country == Country.NORTHERN_IRELAND:
+            return working_days_before(self.poll_date, 14, self._calendar())
+
         return working_days_before(self.poll_date, 11, self._calendar())
 
     @property
     def vac_application_deadline(self) -> date:
         """
         Calculates the Voter Authority Certificate (VAC) application deadline for this Election
```

### Comparing `uk-election-timetables-2.4.0/uk_election_timetables/election_ids.py` & `uk-election-timetables-2.4.1/uk_election_timetables/election_ids.py`

 * *Files identical despite different names*

### Comparing `uk-election-timetables-2.4.0/uk_election_timetables/elections/__init__.py` & `uk-election-timetables-2.4.1/uk_election_timetables/elections/__init__.py`

 * *Files identical despite different names*

### Comparing `uk-election-timetables-2.4.0/uk_election_timetables/elections/greater_london_assembly.py` & `uk-election-timetables-2.4.1/uk_election_timetables/elections/greater_london_assembly.py`

 * *Files identical despite different names*

### Comparing `uk-election-timetables-2.4.0/uk_election_timetables/elections/local.py` & `uk-election-timetables-2.4.1/uk_election_timetables/elections/local.py`

 * *Files identical despite different names*

### Comparing `uk-election-timetables-2.4.0/uk_election_timetables/elections/mayor.py` & `uk-election-timetables-2.4.1/uk_election_timetables/elections/mayor.py`

 * *Files identical despite different names*

### Comparing `uk-election-timetables-2.4.0/uk_election_timetables/elections/northern_ireland_assembly.py` & `uk-election-timetables-2.4.1/uk_election_timetables/elections/northern_ireland_assembly.py`

 * *Files identical despite different names*

### Comparing `uk-election-timetables-2.4.0/uk_election_timetables/elections/police_and_crime_commissioner.py` & `uk-election-timetables-2.4.1/uk_election_timetables/elections/police_and_crime_commissioner.py`

 * *Files identical despite different names*

### Comparing `uk-election-timetables-2.4.0/uk_election_timetables/elections/scottish_parliament.py` & `uk-election-timetables-2.4.1/uk_election_timetables/elections/scottish_parliament.py`

 * *Files identical despite different names*

### Comparing `uk-election-timetables-2.4.0/uk_election_timetables/elections/senedd_cymru.py` & `uk-election-timetables-2.4.1/uk_election_timetables/elections/senedd_cymru.py`

 * *Files identical despite different names*

### Comparing `uk-election-timetables-2.4.0/uk_election_timetables/elections/uk_parliament.py` & `uk-election-timetables-2.4.1/uk_election_timetables/elections/uk_parliament.py`

 * *Files identical despite different names*

### Comparing `uk-election-timetables-2.4.0/uk_election_timetables.egg-info/PKG-INFO` & `uk-election-timetables-2.4.1/uk_election_timetables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uk-election-timetables
-Version: 2.4.0
+Version: 2.4.1
 Summary: Derives significant dates for UK elections
 Home-page: https://github.com/DemocracyClub/uk-election-timetables
 Author: Alex Wilson
 Author-email: alex+github@probablyfine.co.uk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
```

### Comparing `uk-election-timetables-2.4.0/uk_election_timetables.egg-info/SOURCES.txt` & `uk-election-timetables-2.4.1/uk_election_timetables.egg-info/SOURCES.txt`

 * *Files identical despite different names*


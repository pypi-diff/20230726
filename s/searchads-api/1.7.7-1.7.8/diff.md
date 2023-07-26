# Comparing `tmp/searchads_api-1.7.7.tar.gz` & `tmp/searchads_api-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchads_api-1.7.7.tar", last modified: Wed Mar 29 21:16:19 2023, max compression
+gzip compressed data, was "searchads_api-1.7.8.tar", last modified: Wed Jul 26 08:11:45 2023, max compression
```

## Comparing `searchads_api-1.7.7.tar` & `searchads_api-1.7.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alkattan   (501) staff       (20)        0 2023-03-29 21:16:19.903929 searchads_api-1.7.7/
--rw-r--r--   0 alkattan   (501) staff       (20)     1055 2021-04-15 17:45:24.000000 searchads_api-1.7.7/LICENSE
--rw-r--r--   0 alkattan   (501) staff       (20)     2440 2023-03-29 21:16:19.904183 searchads_api-1.7.7/PKG-INFO
--rw-r--r--   0 alkattan   (501) staff       (20)    14011 2023-03-20 11:06:05.000000 searchads_api-1.7.7/README.md
-drwxr-xr-x   0 alkattan   (501) staff       (20)        0 2023-03-29 21:16:19.890382 searchads_api-1.7.7/searchads_api/
--rw-r--r--   0 alkattan   (501) staff       (20)       30 2022-09-04 20:49:59.000000 searchads_api-1.7.7/searchads_api/__init__.py
--rw-r--r--   0 alkattan   (501) staff       (20)    68689 2023-03-29 21:15:26.000000 searchads_api-1.7.7/searchads_api/api.py
-drwxr-xr-x   0 alkattan   (501) staff       (20)        0 2023-03-29 21:16:19.901737 searchads_api-1.7.7/searchads_api.egg-info/
--rw-r--r--   0 alkattan   (501) staff       (20)     2440 2023-03-29 21:16:19.000000 searchads_api-1.7.7/searchads_api.egg-info/PKG-INFO
--rw-r--r--   0 alkattan   (501) staff       (20)      267 2023-03-29 21:16:19.000000 searchads_api-1.7.7/searchads_api.egg-info/SOURCES.txt
--rw-r--r--   0 alkattan   (501) staff       (20)        1 2023-03-29 21:16:19.000000 searchads_api-1.7.7/searchads_api.egg-info/dependency_links.txt
--rw-r--r--   0 alkattan   (501) staff       (20)       51 2023-03-29 21:16:19.000000 searchads_api-1.7.7/searchads_api.egg-info/requires.txt
--rw-r--r--   0 alkattan   (501) staff       (20)       14 2023-03-29 21:16:19.000000 searchads_api-1.7.7/searchads_api.egg-info/top_level.txt
--rw-r--r--   0 alkattan   (501) staff       (20)       79 2023-03-29 21:16:19.905003 searchads_api-1.7.7/setup.cfg
--rw-r--r--   0 alkattan   (501) staff       (20)     2642 2023-03-29 21:16:09.000000 searchads_api-1.7.7/setup.py
+drwxr-xr-x   0 alkattan   (501) staff       (20)        0 2023-07-26 08:11:45.422456 searchads_api-1.7.8/
+-rw-r--r--   0 alkattan   (501) staff       (20)     1055 2021-04-15 17:45:24.000000 searchads_api-1.7.8/LICENSE
+-rw-r--r--   0 alkattan   (501) staff       (20)     2485 2023-07-26 08:11:45.422761 searchads_api-1.7.8/PKG-INFO
+-rw-r--r--   0 alkattan   (501) staff       (20)    14059 2023-03-30 00:14:00.000000 searchads_api-1.7.8/README.md
+drwxr-xr-x   0 alkattan   (501) staff       (20)        0 2023-07-26 08:11:45.414553 searchads_api-1.7.8/searchads_api/
+-rw-r--r--   0 alkattan   (501) staff       (20)       30 2022-09-04 20:49:59.000000 searchads_api-1.7.8/searchads_api/__init__.py
+-rw-r--r--   0 alkattan   (501) staff       (20)    68689 2023-03-29 21:15:26.000000 searchads_api-1.7.8/searchads_api/api.py
+drwxr-xr-x   0 alkattan   (501) staff       (20)        0 2023-07-26 08:11:45.421596 searchads_api-1.7.8/searchads_api.egg-info/
+-rw-r--r--   0 alkattan   (501) staff       (20)     2485 2023-07-26 08:11:45.000000 searchads_api-1.7.8/searchads_api.egg-info/PKG-INFO
+-rw-r--r--   0 alkattan   (501) staff       (20)      267 2023-07-26 08:11:45.000000 searchads_api-1.7.8/searchads_api.egg-info/SOURCES.txt
+-rw-r--r--   0 alkattan   (501) staff       (20)        1 2023-07-26 08:11:45.000000 searchads_api-1.7.8/searchads_api.egg-info/dependency_links.txt
+-rw-r--r--   0 alkattan   (501) staff       (20)       51 2023-07-26 08:11:45.000000 searchads_api-1.7.8/searchads_api.egg-info/requires.txt
+-rw-r--r--   0 alkattan   (501) staff       (20)       14 2023-07-26 08:11:45.000000 searchads_api-1.7.8/searchads_api.egg-info/top_level.txt
+-rw-r--r--   0 alkattan   (501) staff       (20)       79 2023-07-26 08:11:45.424143 searchads_api-1.7.8/setup.cfg
+-rw-r--r--   0 alkattan   (501) staff       (20)     2687 2023-07-26 08:11:21.000000 searchads_api-1.7.8/setup.py
```

### Comparing `searchads_api-1.7.7/LICENSE` & `searchads_api-1.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `searchads_api-1.7.7/PKG-INFO` & `searchads_api-1.7.8/searchads_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: searchads_api
-Version: 1.7.7
+Name: searchads-api
+Version: 1.7.8
 Summary: Apple Searchads API non-official python library
 Home-page: https://github.com/phiture/searchads_api
 Author: Abdul Majeed Alkattan
 Author-email: alkattan@phiture.com
 Keywords: python,searchads,library
 License-File: LICENSE
 
@@ -13,15 +13,20 @@
 # About Phiture
 
 http://phiture.com is a Berlin-based mobile growth consultancy working with the teams behind leading apps. Using the company’s industry-acclaimed Mobile Growth Stack as a strategic framework, Phiture team offers 4 key services: App Store Optimization, Apple Search Ads, User Retention services and Growth Consulting.
 
 
 # Apple Searchads API Library in Python
 
-In order to facilitate the usage of the Apple Search Ads API Phiture's Engineers have built a library in Python which allows users to manage campaigns, ad groups, keywords and creative sets. This library only requires intermediate Python skills and therefore makes it possible not only for Engineers but also for Data Analysts and Apple Search Ads Consultants to work with it.  While the library is extensive it is not complete and users are encouraged to commit suggestions.
+In order to facilitate the usage of the Apple Search Ads API Phiture's Engineers 
+have built a library in Python which allows users to manage campaigns, ad groups, 
+keywords and creative sets. This library only requires intermediate Python skills 
+and therefore makes it possible not only for Engineers but also for Data Analysts 
+and Apple Search Ads Consultants to work with it.  
+While the library is extensive it is not complete and users are encouraged to commit suggestions.
 
 Read the docs on github.
 
 # Example Usage:
 
 Setup for v4 of the library
 
@@ -57,8 +62,10 @@
 version 1.6.3 includes new bug fixes
 
 version 1.7.1 added impression share reports and new find methods along product pages to match Searchads API version 4.7
 
 version 1.7.6 fixed an issue with token update
 
 version 1.7.7 fixed an issue update_campaign
+
+version 1.7.8 updated the dependencies
```

### Comparing `searchads_api-1.7.7/README.md` & `searchads_api-1.7.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -373,14 +373,15 @@
 - Get a single impression share report using report ID
 
          res = api.get_single_impression_share_report(12345)
 
 
 ## Changelog
 
+* version 1.7.7 fixed an issue update_campaign
 * version 1.7.6 fixed an issue with token update
 * version 1.7.1 added impression share reports and new find methods along product pages to match Searchads API version 4.7
 * version 1.6.3 New bug fixes
 * version 1.6.1 added new product page, reporting, and Ad endpoints. Deprecated creatives endpoints
 * version 1.5.3 fixed token update issue
 * version 1.5.3 deprecated creativesets methods from Apple Search Ads API v4
 * version 1.5.2 fixed a bug in token refresh due to wrong status code
```

### Comparing `searchads_api-1.7.7/searchads_api/api.py` & `searchads_api-1.7.8/searchads_api/api.py`

 * *Files identical despite different names*

### Comparing `searchads_api-1.7.7/searchads_api.egg-info/PKG-INFO` & `searchads_api-1.7.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: searchads-api
-Version: 1.7.7
+Name: searchads_api
+Version: 1.7.8
 Summary: Apple Searchads API non-official python library
 Home-page: https://github.com/phiture/searchads_api
 Author: Abdul Majeed Alkattan
 Author-email: alkattan@phiture.com
 Keywords: python,searchads,library
 License-File: LICENSE
 
@@ -13,15 +13,20 @@
 # About Phiture
 
 http://phiture.com is a Berlin-based mobile growth consultancy working with the teams behind leading apps. Using the company’s industry-acclaimed Mobile Growth Stack as a strategic framework, Phiture team offers 4 key services: App Store Optimization, Apple Search Ads, User Retention services and Growth Consulting.
 
 
 # Apple Searchads API Library in Python
 
-In order to facilitate the usage of the Apple Search Ads API Phiture's Engineers have built a library in Python which allows users to manage campaigns, ad groups, keywords and creative sets. This library only requires intermediate Python skills and therefore makes it possible not only for Engineers but also for Data Analysts and Apple Search Ads Consultants to work with it.  While the library is extensive it is not complete and users are encouraged to commit suggestions.
+In order to facilitate the usage of the Apple Search Ads API Phiture's Engineers 
+have built a library in Python which allows users to manage campaigns, ad groups, 
+keywords and creative sets. This library only requires intermediate Python skills 
+and therefore makes it possible not only for Engineers but also for Data Analysts 
+and Apple Search Ads Consultants to work with it.  
+While the library is extensive it is not complete and users are encouraged to commit suggestions.
 
 Read the docs on github.
 
 # Example Usage:
 
 Setup for v4 of the library
 
@@ -57,8 +62,10 @@
 version 1.6.3 includes new bug fixes
 
 version 1.7.1 added impression share reports and new find methods along product pages to match Searchads API version 4.7
 
 version 1.7.6 fixed an issue with token update
 
 version 1.7.7 fixed an issue update_campaign
+
+version 1.7.8 updated the dependencies
```

### Comparing `searchads_api-1.7.7/setup.py` & `searchads_api-1.7.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name='searchads_api',
     description='Apple Searchads API non-official python library',
-    version='1.7.7',
+    version='1.7.8',
     url='https://github.com/phiture/searchads_api',
     author='Abdul Majeed Alkattan',
     author_email='alkattan@phiture.com',
     packages=["searchads_api"], 
     keywords=['python','searchads','library'],
-    install_requires=['requests>=2.28.1', 'PyJWT==2.6.0', 'cryptography==36.0.2'],
+    install_requires=['requests>=2.31.0', 'PyJWT==2.8.0', 'cryptography==41.0.2'],
     long_description="""
 
 # About Phiture
 
 http://phiture.com is a Berlin-based mobile growth consultancy working with the teams behind leading apps. Using the company’s industry-acclaimed Mobile Growth Stack as a strategic framework, Phiture team offers 4 key services: App Store Optimization, Apple Search Ads, User Retention services and Growth Consulting.
 
 
 # Apple Searchads API Library in Python
 
-In order to facilitate the usage of the Apple Search Ads API Phiture's Engineers have built a library in Python which allows users to manage campaigns, ad groups, keywords and creative sets. This library only requires intermediate Python skills and therefore makes it possible not only for Engineers but also for Data Analysts and Apple Search Ads Consultants to work with it.  While the library is extensive it is not complete and users are encouraged to commit suggestions.
+In order to facilitate the usage of the Apple Search Ads API Phiture's Engineers 
+have built a library in Python which allows users to manage campaigns, ad groups, 
+keywords and creative sets. This library only requires intermediate Python skills 
+and therefore makes it possible not only for Engineers but also for Data Analysts 
+and Apple Search Ads Consultants to work with it.  
+While the library is extensive it is not complete and users are encouraged to commit suggestions.
 
 Read the docs on github.
 
 # Example Usage:
 
 Setup for v4 of the library
 
@@ -60,9 +65,11 @@
 version 1.6.3 includes new bug fixes
 
 version 1.7.1 added impression share reports and new find methods along product pages to match Searchads API version 4.7
 
 version 1.7.6 fixed an issue with token update
 
 version 1.7.7 fixed an issue update_campaign
+
+version 1.7.8 updated the dependencies
     """,
 )
```


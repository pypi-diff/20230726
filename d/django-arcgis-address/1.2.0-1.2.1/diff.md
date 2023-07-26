# Comparing `tmp/django-arcgis-address-1.2.0.tar.gz` & `tmp/django-arcgis-address-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-arcgis-address-1.2.0.tar", last modified: Wed Jul 26 05:47:35 2023, max compression
+gzip compressed data, was "django-arcgis-address-1.2.1.tar", last modified: Wed Jul 26 05:57:54 2023, max compression
```

## Comparing `django-arcgis-address-1.2.0.tar` & `django-arcgis-address-1.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:47:35.206919 django-arcgis-address-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1536 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      440 2023-07-26 05:47:35.206919 django-arcgis-address-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5084 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:47:35.178918 django-arcgis-address-1.2.0/address/
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/compat.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:47:35.206919 django-arcgis-address-1.2.0/address/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     4296 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/migrations/0002_auto_20160213_1726.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/migrations/0003_auto_20200830_1851.py
--rw-rw-rw-   0 root         (0) root         (0)     3952 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/migrations/0004_auto_20210618_2016.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13192 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3392 2023-07-26 05:14:14.000000 django-arcgis-address-1.2.0/address/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2335 2023-07-24 00:06:08.000000 django-arcgis-address-1.2.0/address/widgets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:47:35.206919 django-arcgis-address-1.2.0/django_arcgis_address.egg-info/
--rw-r--r--   0 root         (0) root         (0)      440 2023-07-26 05:47:34.000000 django-arcgis-address-1.2.0/django_arcgis_address.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      606 2023-07-26 05:47:35.000000 django-arcgis-address-1.2.0/django_arcgis_address.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 05:47:34.000000 django-arcgis-address-1.2.0/django_arcgis_address.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-26 05:47:34.000000 django-arcgis-address-1.2.0/django_arcgis_address.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-26 05:47:34.000000 django-arcgis-address-1.2.0/django_arcgis_address.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-26 05:47:35.206919 django-arcgis-address-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      526 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:57:54.653984 django-arcgis-address-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      440 2023-07-26 05:57:54.653984 django-arcgis-address-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5084 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:57:54.649984 django-arcgis-address-1.2.1/address/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.1/address/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.1/address/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.1/address/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.1/address/compat.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.1/address/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:57:54.649984 django-arcgis-address-1.2.1/address/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     4296 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.1/address/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.1/address/migrations/0002_auto_20160213_1726.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.1/address/migrations/0003_auto_20200830_1851.py
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.1/address/migrations/0004_auto_20210618_2016.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.1/address/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13192 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.1/address/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3376 2023-07-26 05:50:45.000000 django-arcgis-address-1.2.1/address/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2335 2023-07-24 00:06:08.000000 django-arcgis-address-1.2.1/address/widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:57:54.653984 django-arcgis-address-1.2.1/django_arcgis_address.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      440 2023-07-26 05:57:54.000000 django-arcgis-address-1.2.1/django_arcgis_address.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      606 2023-07-26 05:57:54.000000 django-arcgis-address-1.2.1/django_arcgis_address.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 05:57:54.000000 django-arcgis-address-1.2.1/django_arcgis_address.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-26 05:57:54.000000 django-arcgis-address-1.2.1/django_arcgis_address.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-26 05:57:54.000000 django-arcgis-address-1.2.1/django_arcgis_address.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-26 05:57:54.653984 django-arcgis-address-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      526 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.1/setup.py
```

### Comparing `django-arcgis-address-1.2.0/LICENSE` & `django-arcgis-address-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-arcgis-address-1.2.0/README.md` & `django-arcgis-address-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django-arcgis-address-1.2.0/address/admin.py` & `django-arcgis-address-1.2.1/address/admin.py`

 * *Files identical despite different names*

### Comparing `django-arcgis-address-1.2.0/address/forms.py` & `django-arcgis-address-1.2.1/address/forms.py`

 * *Files identical despite different names*

### Comparing `django-arcgis-address-1.2.0/address/migrations/0001_initial.py` & `django-arcgis-address-1.2.1/address/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-arcgis-address-1.2.0/address/migrations/0004_auto_20210618_2016.py` & `django-arcgis-address-1.2.1/address/migrations/0004_auto_20210618_2016.py`

 * *Files identical despite different names*

### Comparing `django-arcgis-address-1.2.0/address/models.py` & `django-arcgis-address-1.2.1/address/models.py`

 * *Files identical despite different names*

### Comparing `django-arcgis-address-1.2.0/address/utils.py` & `django-arcgis-address-1.2.1/address/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         return False
     if settings.ARCGIS_ADDRESS_CATEGORIES:
         arcgis_params["category"] = ",".join(settings.ARCGIS_ADDRESS_CATEGORIES)
     return arcgis_params
 
 
 def geocode(raw):
-    arcgis_params = geocode_initialization(list_of_pks_and_raws)
+    arcgis_params = geocode_initialization(raw)
     if not arcgis_params:
         return raw
     arcgis_params["singleLine"] = raw
     keyword = "candidates"
     json_response = get_json_response(keyword, arcgis_params)
     if not json_response:
         return raw
@@ -76,15 +76,15 @@
             list_of_pks_and_raws[pos : pos + BATCH_SIZE]
         )
         if not succesful:
             all_successful = False
             continue
         result = result + temp_result
 
-    return result, all_succesful
+    return result, all_successful
 
 
 # geocode a list of up to BATCH_SIZE
 def geocode_batch(list_of_pks_and_raws):
     arcgis_params = geocode_initialization(list_of_pks_and_raws)
     if not arcgis_params:
         return list_of_pks_and_raws, False
```

### Comparing `django-arcgis-address-1.2.0/address/widgets.py` & `django-arcgis-address-1.2.1/address/widgets.py`

 * *Files identical despite different names*

### Comparing `django-arcgis-address-1.2.0/django_arcgis_address.egg-info/SOURCES.txt` & `django-arcgis-address-1.2.1/django_arcgis_address.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-arcgis-address-1.2.0/setup.py` & `django-arcgis-address-1.2.1/setup.py`

 * *Files identical despite different names*


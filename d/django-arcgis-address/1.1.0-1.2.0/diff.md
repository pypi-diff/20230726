# Comparing `tmp/django-arcgis-address-1.1.0.tar.gz` & `tmp/django-arcgis-address-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-arcgis-address-1.1.0.tar", last modified: Wed Jan  5 11:27:32 2022, max compression
+gzip compressed data, was "django-arcgis-address-1.2.0.tar", last modified: Wed Jul 26 05:47:35 2023, max compression
```

## Comparing `django-arcgis-address-1.1.0.tar` & `django-arcgis-address-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 11:27:32.035264 django-arcgis-address-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-01-05 11:27:01.000000 django-arcgis-address-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-01-05 11:27:32.039264 django-arcgis-address-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5110 2022-01-05 11:27:01.000000 django-arcgis-address-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 11:27:32.035264 django-arcgis-address-1.1.0/address/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-01-05 11:27:01.000000 django-arcgis-address-1.1.0/address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-01-05 11:27:01.000000 django-arcgis-address-1.1.0/address/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-01-05 11:27:01.000000 django-arcgis-address-1.1.0/address/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-01-05 11:27:01.000000 django-arcgis-address-1.1.0/address/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-01-05 11:27:01.000000 django-arcgis-address-1.1.0/address/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 11:27:32.035264 django-arcgis-address-1.1.0/address/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     3311 2022-01-05 11:27:01.000000 django-arcgis-address-1.1.0/address/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-01-05 11:27:01.000000 django-arcgis-address-1.1.0/address/migrations/0002_auto_20160213_1726.py
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-01-05 11:27:01.000000 django-arcgis-address-1.1.0/address/migrations/0003_auto_20200830_1851.py
--rw-r--r--   0 runner    (1001) docker     (121)     3953 2022-01-05 11:27:01.000000 django-arcgis-address-1.1.0/address/migrations/0004_auto_20210618_2016.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-05 11:27:01.000000 django-arcgis-address-1.1.0/address/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13193 2022-01-05 11:27:01.000000 django-arcgis-address-1.1.0/address/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-01-05 11:27:01.000000 django-arcgis-address-1.1.0/address/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2336 2022-01-05 11:27:01.000000 django-arcgis-address-1.1.0/address/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 11:27:32.035264 django-arcgis-address-1.1.0/django_arcgis_address.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-01-05 11:27:31.000000 django-arcgis-address-1.1.0/django_arcgis_address.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-01-05 11:27:31.000000 django-arcgis-address-1.1.0/django_arcgis_address.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-05 11:27:31.000000 django-arcgis-address-1.1.0/django_arcgis_address.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-01-05 11:27:31.000000 django-arcgis-address-1.1.0/django_arcgis_address.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-01-05 11:27:31.000000 django-arcgis-address-1.1.0/django_arcgis_address.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-01-05 11:27:32.039264 django-arcgis-address-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-01-05 11:27:01.000000 django-arcgis-address-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:47:35.206919 django-arcgis-address-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      440 2023-07-26 05:47:35.206919 django-arcgis-address-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5084 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:47:35.178918 django-arcgis-address-1.2.0/address/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/compat.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:47:35.206919 django-arcgis-address-1.2.0/address/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     4296 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/migrations/0002_auto_20160213_1726.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/migrations/0003_auto_20200830_1851.py
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/migrations/0004_auto_20210618_2016.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13192 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/address/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3392 2023-07-26 05:14:14.000000 django-arcgis-address-1.2.0/address/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2335 2023-07-24 00:06:08.000000 django-arcgis-address-1.2.0/address/widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:47:35.206919 django-arcgis-address-1.2.0/django_arcgis_address.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      440 2023-07-26 05:47:34.000000 django-arcgis-address-1.2.0/django_arcgis_address.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      606 2023-07-26 05:47:35.000000 django-arcgis-address-1.2.0/django_arcgis_address.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 05:47:34.000000 django-arcgis-address-1.2.0/django_arcgis_address.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-26 05:47:34.000000 django-arcgis-address-1.2.0/django_arcgis_address.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-26 05:47:34.000000 django-arcgis-address-1.2.0/django_arcgis_address.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-26 05:47:35.206919 django-arcgis-address-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      526 2023-07-14 11:56:27.000000 django-arcgis-address-1.2.0/setup.py
```

### Comparing `django-arcgis-address-1.1.0/LICENSE` & `django-arcgis-address-1.2.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-BSD 2-Clause License
+BSD 3-Clause License
 
-Copyright (c) 2021, Institute of Computer Science, Masaryk University.
-All rights reserved.
+Copyright (c) 2023, Institute of Computer Science, Masaryk University
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
 
 2. Redistributions in binary form must reproduce the above copyright notice,
    this list of conditions and the following disclaimer in the documentation
    and/or other materials provided with the distribution.
 
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
 AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
```

### Comparing `django-arcgis-address-1.1.0/README.md` & `django-arcgis-address-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Django Address 
+# Django Address
 
 **Django models for storing and retrieving postal addresses.**
 
 Based on [django-address](https://github.com/furious-luke/django-address) but uses ESRI ArcGIS instead of Google.
 
 ---
 
 # Overview
+
 Django Address is a set of models and methods for working with postal addresses.
 
 # Requirements
 
-* Python (3.9)
-* Django (3.0) with a theme which includes jQuery (as django.jQuery) and the select2 library
+Django with a theme which includes jQuery (as django.jQuery) and the select2 library
 
 # Installation
 
 ```bash
 pip3 install git+https://github.com/melanger/django-arcgis-address.git
 ```
 
 Then, add `address` to your `INSTALLED_APPS` list in `settings.py`:
 
 ```
 INSTALLED_APPS = [
-    # ... 
+    # ...
     'address',
-    # ... 
+    # ...
 ]
 ```
 
 You can either store your ESRI API key in an environment variable as `ARCGIS_SERVER_API_KEY` and `ARCGIS_CLIENT_API_KEY` or you can
- specify the key in `settings.py`. If you have an environment variable set it will override what you put in settings.py.
- 
+specify the key in `settings.py`. If you have an environment variable set it will override what you put in settings.py.
+
 ```
 ARCGIS_SERVER_API_KEY = '}zIMqHDs"4CJs$l[G.+XHSJ)Wq[?mVgr'
 ARCGIS_CLIENT_API_KEY = '}zIMqHDs"4CJs$l[G.+XHSJ)Wq[?mVgr'
 ```
 
 There is also possibility to customize [ARCGIS category filtering](https://developers.arcgis.com/rest/geocode/api-reference/geocoding-category-filtering.htm) via list variable `ARCGIS_ADDRESS_CATEGORIES`. For example to filter out only adresses, cities and countries, you can set following:
 
@@ -94,20 +94,20 @@
 
 To simplify storage and access of addresses, a subclass of `ForeignKey` named
 `AddressField` has been created. It provides an easy method for setting new
 addresses.
 
 ## ON_DELETE behavior of Address Field
 
-By default, if you delete an Address that is related to another object, 
-Django's [cascade behavior](https://docs.djangoproject.com/en/dev/ref/models/fields/#django.db.models.ForeignKey.on_delete) 
+By default, if you delete an Address that is related to another object,
+Django's [cascade behavior](https://docs.djangoproject.com/en/dev/ref/models/fields/#django.db.models.ForeignKey.on_delete)
 is used. This means the related object will also be deleted. You may also choose
 to set `null=True` when defining an address field to have the address set
 to Null instead of deleting the related object.
- 
+
 ## Creation
 
 It can be created using the same optional arguments as a ForeignKey field.
 For example:
 
 ```python
   from address.models import AddressField
@@ -192,13 +192,14 @@
   address = AddressField()
 ```
 
 The template:
 
 ```html
 <head>
-{{ form.media }} <!-- needed for JS lookup -->
+  {{ form.media }}
+  <!-- needed for JS lookup -->
 </head>
 <body>
   {{ form }}
 </body>
 ```
```

### Comparing `django-arcgis-address-1.1.0/address/admin.py` & `django-arcgis-address-1.2.0/address/admin.py`

 * *Files identical despite different names*

### Comparing `django-arcgis-address-1.1.0/address/forms.py` & `django-arcgis-address-1.2.0/address/forms.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,46 +2,45 @@
 import sys
 
 from django import forms
 
 from .models import Address, to_python
 from .widgets import AddressWidget
 
-if sys.version > '3':
+if sys.version > "3":
     long = int
     basestring = (str, bytes)
     unicode = str
 
 logger = logging.getLogger(__name__)
 
-__all__ = ['AddressWidget', 'AddressField']
+__all__ = ["AddressWidget", "AddressField"]
 
 
 class AddressField(forms.ModelChoiceField):
     widget = AddressWidget
 
     def __init__(self, *args, **kwargs):
-        kwargs['queryset'] = Address.objects.none()
+        kwargs["queryset"] = Address.objects.none()
         super(AddressField, self).__init__(*args, **kwargs)
 
     def to_python(self, value):
-
         # Treat `None`s and empty strings as empty.
-        if value is None or value == '':
+        if value is None or value == "":
             return None
 
         # Check for garbage in the lat/lng components.
-        for field in ['latitude', 'longitude']:
+        for field in ["latitude", "longitude"]:
             if field in value:
                 if value[field]:
                     try:
                         value[field] = float(value[field])
                     except Exception:
                         raise forms.ValidationError(
-                            'Invalid value for %(field)s',
-                            code='invalid',
-                            params={'field': field}
+                            "Invalid value for %(field)s",
+                            code="invalid",
+                            params={"field": field},
                         )
                 else:
                     value[field] = None
 
         return to_python(value)
```

### Comparing `django-arcgis-address-1.1.0/address/migrations/0004_auto_20210618_2016.py` & `django-arcgis-address-1.2.0/address/migrations/0004_auto_20210618_2016.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.0.14 on 2021-06-18 18:16
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("address", "0003_auto_20200830_1851"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="District",
```

### Comparing `django-arcgis-address-1.1.0/address/models.py` & `django-arcgis-address-1.2.0/address/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,14 @@
     elif isinstance(value, basestring):
         obj = Address(raw=value)
         obj.save()
         return obj
 
     # A dictionary of named address components.
     elif isinstance(value, dict):
-
         # Attempt a conversion.
         try:
             return _to_python(value)
         except InconsistentDictError:
             return Address.objects.create(raw=value["raw"])
 
     # Not in any of the formats I recognise.
```

### Comparing `django-arcgis-address-1.1.0/address/widgets.py` & `django-arcgis-address-1.2.0/address/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         classes = attrs.get("class", "")
         classes += (" " if classes else "") + "address"
         attrs["class"] = classes
         kwargs["attrs"] = attrs
         super(AddressWidget, self).__init__(*args, **kwargs)
 
     def render(self, name, value, attrs=None, **kwargs):
-
         # Can accept None, a dictionary of values or an Address object.
         if value in (None, ""):
             ad = {}
         elif isinstance(value, dict):
             ad = value
         elif isinstance(value, (int, long)):
             ad = Address.objects.get(pk=value)
```

### Comparing `django-arcgis-address-1.1.0/django_arcgis_address.egg-info/SOURCES.txt` & `django-arcgis-address-1.2.0/django_arcgis_address.egg-info/SOURCES.txt`

 * *Files identical despite different names*


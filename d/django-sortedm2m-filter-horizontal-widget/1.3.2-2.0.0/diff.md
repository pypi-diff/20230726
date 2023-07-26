# Comparing `tmp/django-sortedm2m-filter-horizontal-widget-1.3.2.tar.gz` & `tmp/django_sortedm2m_filter_horizontal_widget-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-sortedm2m-filter-horizontal-widget-1.3.2.tar", last modified: Mon May  7 09:01:57 2018, max compression
+gzip compressed data, was "django_sortedm2m_filter_horizontal_widget-2.0.0.tar", max compression
```

## Comparing `django-sortedm2m-filter-horizontal-widget-1.3.2.tar` & `django_sortedm2m_filter_horizontal_widget-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,10 @@
-drwxr-xr-x   0 sandervanleeuwen   (502) staff       (20)        0 2018-05-07 09:01:57.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)     4182 2018-05-07 09:01:57.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/PKG-INFO
-drwxr-xr-x   0 sandervanleeuwen   (502) staff       (20)        0 2018-05-07 09:01:57.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/django_sortedm2m_filter_horizontal_widget.egg-info/
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)     4182 2018-05-07 09:01:57.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/django_sortedm2m_filter_horizontal_widget.egg-info/PKG-INFO
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)        1 2017-05-01 15:14:05.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/django_sortedm2m_filter_horizontal_widget.egg-info/not-zip-safe
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)      922 2018-05-07 09:01:57.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/django_sortedm2m_filter_horizontal_widget.egg-info/SOURCES.txt
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)       17 2018-05-07 09:01:57.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/django_sortedm2m_filter_horizontal_widget.egg-info/requires.txt
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)       35 2018-05-07 09:01:57.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/django_sortedm2m_filter_horizontal_widget.egg-info/top_level.txt
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)        1 2018-05-07 09:01:57.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/django_sortedm2m_filter_horizontal_widget.egg-info/dependency_links.txt
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)      161 2017-01-02 14:27:07.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/MANIFEST.in
--rwxr-xr-x   0 sandervanleeuwen   (502) staff       (20)     2831 2017-05-01 15:08:47.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/setup.py
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)       94 2017-01-02 14:27:07.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/AUTHORS.rst
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)       38 2018-05-07 09:01:57.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/setup.cfg
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)     1659 2018-05-07 05:54:24.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/README.rst
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)     1505 2017-01-02 14:27:07.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/LICENSE.txt
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)      766 2018-05-07 09:01:24.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/CHANGES.rst
-drwxr-xr-x   0 sandervanleeuwen   (502) staff       (20)        0 2018-05-07 09:01:57.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/sortedm2m_filter_horizontal_widget/
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)       48 2018-05-07 09:01:24.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/sortedm2m_filter_horizontal_widget/__init__.py
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)     6975 2018-05-07 08:43:41.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/sortedm2m_filter_horizontal_widget/forms.py
-drwxr-xr-x   0 sandervanleeuwen   (502) staff       (20)        0 2018-05-07 09:01:57.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/sortedm2m_filter_horizontal_widget/static/
-drwxr-xr-x   0 sandervanleeuwen   (502) staff       (20)        0 2018-05-07 09:01:57.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)    85925 2017-05-01 14:24:29.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/jquery.min.js
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)     6235 2017-05-01 14:24:29.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/OrderedSelectBox.js
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)     2375 2018-05-07 05:54:24.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/widget.css
--rw-r--r--   0 sandervanleeuwen   (502) staff       (20)    11713 2018-05-07 09:01:24.000000 django-sortedm2m-filter-horizontal-widget-1.3.2/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/OrderedSelectFilter.js
+-rw-r--r--   0        0        0     1505 2023-07-26 07:54:32.253432 django_sortedm2m_filter_horizontal_widget-2.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     1357 2023-07-26 08:52:09.289241 django_sortedm2m_filter_horizontal_widget-2.0.0/README.md
+-rw-r--r--   0        0        0      484 2023-07-26 08:57:57.707299 django_sortedm2m_filter_horizontal_widget-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-07-26 07:54:32.254256 django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/__init__.py
+-rw-r--r--   0        0        0     6980 2023-07-26 08:36:26.261010 django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/forms.py
+-rw-r--r--   0        0        0     6235 2023-07-26 07:54:32.254465 django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/OrderedSelectBox.js
+-rw-r--r--   0        0        0    11713 2023-07-26 07:54:32.254565 django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/OrderedSelectFilter.js
+-rw-r--r--   0        0        0    85925 2023-07-26 07:54:32.254920 django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/jquery.min.js
+-rw-r--r--   0        0        0     2372 2023-07-26 09:02:47.966285 django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/widget.css
+-rw-r--r--   0        0        0     2166 1970-01-01 00:00:00.000000 django_sortedm2m_filter_horizontal_widget-2.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-sortedm2m-filter-horizontal-widget-1.3.2/README.rst` & `django_sortedm2m_filter_horizontal_widget-2.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,50 @@
-=========================================
-django-sortedm2m-filter-horizontal-widget
-=========================================
+# django-sortedm2m-filter-horizontal-widget
 
-``sortedm2m-filter-horizontal-widget`` is an admin widget for Gregor Mülleggers excellent django-sortedm2m_ library.
-
-.. _django-sortedm2m: http://github.com/gregmuellegger/django-sortedm2m
+`sortedm2m-filter-horizontal-widget` is an admin widget for Gregor
+Mülleggers excellent
+[django-sortedm2m](http://github.com/gregmuellegger/django-sortedm2m)
+library.
 
 This allows for a familiar filter horizontal widget.
 
-.. figure:: https://image.ibb.co/fYO8On/Screen_Shot_2018_05_07_at_9_39_30_AM.png
+![](https://image.ibb.co/fYO8On/Screen_Shot_2018_05_07_at_9_39_30_AM.png)
+
+## Installation
+
+`pip install django-sortedm2m-filter-horizontal-widget`
+
+## What version do I need?
 
-Installation
-============
 
-``pip install django-sortedm2m-filter-horizontal-widget``
+| Django  | Install |
+|---------|---------|
+| \< 1.8  | 0.2     |
+| 1.8     | 1.1     |
+| \>= 1.9 | 1.2.1   |
+| \>= 2.0 | 1.3.2   |
+| \>= 3.0 | latest  |
 
-What version do I need?
-=======================
-
-+------------+------------+
-| Django     | Install    |
-+============+============+
-| < 1.8      | 0.2        |
-+------------+------------+
-| 1.8        | 1.1        |
-+------------+------------+
-| >= 1.9     | 1.2.1      |
-+------------+------------+
-| >= 2.0     | latest     |
-+------------+------------+
 
-Usage
-=====
+## Usage
 
-Add ``sortedm2m_filter_horizontal_widget`` to your ``INSTALLED_APPS``. (needed for static files)
+Add `sortedm2m_filter_horizontal_widget` to your `INSTALLED_APPS`
+(needed for static files).
 
-In your ``ModelAdmin`` add the following function to override the default widget. ::
+In your `ModelAdmin` add the following function to override the default
+widget. :
 
     from sortedm2m_filter_horizontal_widget.forms import SortedFilteredSelectMultiple
 
     class MyModelAdmin(admin.ModelAdmin):
         # ...
 
         def formfield_for_manytomany(self, db_field, request=None, **kwargs):
             if db_field.name == 'your_sortedm2m_field_name':
                 kwargs['widget'] = SortedFilteredSelectMultiple()
             return super(MyModelAdmin, self).formfield_for_manytomany(db_field, request, **kwargs)
 
-Todo
-====
+## Todo
 
-* Automatically assign widget if field is specified in ModelAdmin's ``filter_horizontal``.
-* Add tests
+-   Automatically assign widget if field is specified in ModelAdmin\'s
+    `filter_horizontal`.
+-   Add tests
```

### Comparing `django-sortedm2m-filter-horizontal-widget-1.3.2/LICENSE.txt` & `django_sortedm2m_filter_horizontal_widget-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-sortedm2m-filter-horizontal-widget-1.3.2/sortedm2m_filter_horizontal_widget/forms.py` & `django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 import sys
 from itertools import chain
 from django import forms
 from django.conf import settings
 from django.db.models.query import QuerySet
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.utils.html import conditional_escape, escape
 from django.utils.safestring import mark_safe
 
 try:
     from django.forms.utils import flatatt
 except ImportError:
     from django.forms.util import flatatt
 
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
 if sys.version_info[0] < 3:
     iteritems = lambda d: iter(d.iteritems())
     string_types = basestring,
     str_ = unicode
 else:
@@ -49,16 +49,16 @@
     def _has_changed(self, initial, data):
         if initial is None:
             initial = []
         if data is None:
             data = []
         if len(initial) != len(data):
             return True
-        initial_set = [force_text(value) for value in self.prepare_value(initial)]
-        data_set = [force_text(value) for value in data]
+        initial_set = [force_str(value) for value in self.prepare_value(initial)]
+        data_set = [force_str(value) for value in data]
         return data_set != initial_set
 
 
 class SortedFilteredSelectMultiple(forms.SelectMultiple):
     """
     A SortableSelectMultiple with a JavaScript filter interface.
 
@@ -87,15 +87,15 @@
             attrs.update(extra_attrs)
         classes = attrs.setdefault('class', '').split()
         classes.append('sortedm2m')
         if self.is_stacked: classes.append('stacked')
         attrs['class'] = u' '.join(classes)
         return attrs
 
-    def render(self, name, value, attrs=None, choices=()):
+    def render(self, name, value, attrs=None, choices=(), renderer=None):
         if attrs is None: attrs = {}
         if value is None: value = []
         admin_media_prefix = getattr(settings, 'ADMIN_MEDIA_PREFIX', STATIC_URL + 'admin/')
         final_attrs = self.build_attrs(self.attrs, attrs, name=name)
         output = [u'<select multiple="multiple"%s>' % flatatt(final_attrs)]
         options = self.render_options(choices, value)
         if options:
@@ -132,43 +132,43 @@
             });
         })(django.jQuery)
         </script>""" % (admin_media_prefix, admin_media_prefix))
 
         return mark_safe(u'\n'.join(output))
 
     def render_option(self, selected_choices, option_value, option_label):
-        option_value = force_text(option_value)
+        option_value = force_str(option_value)
         selected_html = (option_value in selected_choices) and u' selected="selected"' or ''
         try:
             index = list(selected_choices).index(escape(option_value))
             selected_html = u'%s %s' % (u' data-sort-value="%s"' % index, selected_html)
         except ValueError:
             pass
 
         return u'<option value="%s"%s>%s</option>' % (
             escape(option_value), selected_html,
-            conditional_escape(force_text(option_label)))
+            conditional_escape(force_str(option_label)))
 
     def render_options(self, choices, selected_choices):
         # Normalize to strings.
-        selected_choices = list(force_text(v) for v in selected_choices)
+        selected_choices = list(force_str(v) for v in selected_choices)
         output = []
         for option_value, option_label in chain(self.choices, choices):
             if isinstance(option_label, (list, tuple)):
-                output.append(u'<optgroup label="%s">' % escape(force_text(option_value)))
+                output.append(u'<optgroup label="%s">' % escape(force_str(option_value)))
                 for option in option_label:
                     output.append(self.render_option(selected_choices, *option))
                 output.append(u'</optgroup>')
             else:
                 output.append(self.render_option(selected_choices, option_value, option_label))
         return u'\n'.join(output)
 
     def _has_changed(self, initial, data):
         if initial is None:
             initial = []
         if data is None:
             data = []
         if len(initial) != len(data):
             return True
-        initial_set = [force_text(value) for value in initial]
-        data_set = [force_text(value) for value in data]
+        initial_set = [force_str(value) for value in initial]
+        data_set = [force_str(value) for value in data]
         return data_set != initial_set
```

### Comparing `django-sortedm2m-filter-horizontal-widget-1.3.2/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/jquery.min.js` & `django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-sortedm2m-filter-horizontal-widget-1.3.2/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/OrderedSelectBox.js` & `django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/OrderedSelectBox.js`

 * *Files identical despite different names*

### Comparing `django-sortedm2m-filter-horizontal-widget-1.3.2/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/widget.css` & `django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/widget.css`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 }
 
 .selector ul.selector-chooser {
   float: left;
   width: 22px;
   background-color: #eee;
   border-radius: 10px;
-  margin: 10em 5px 0 5px;
+  margin: 0 5px 0 5px;
   padding: 0;
 }
 
 .selector-chooser li {
   list-style-type: none;
   margin: 0;
   padding: 3px;
```

### Comparing `django-sortedm2m-filter-horizontal-widget-1.3.2/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/OrderedSelectFilter.js` & `django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/OrderedSelectFilter.js`

 * *Files identical despite different names*


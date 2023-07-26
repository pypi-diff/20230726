# Comparing `tmp/django_sortedm2m_filter_horizontal_widget-2.0.0.tar.gz` & `tmp/django_sortedm2m_filter_horizontal_widget-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_sortedm2m_filter_horizontal_widget-2.0.0.tar", max compression
+gzip compressed data, was "django_sortedm2m_filter_horizontal_widget-2.0.1.tar", max compression
```

## Comparing `django_sortedm2m_filter_horizontal_widget-2.0.0.tar` & `django_sortedm2m_filter_horizontal_widget-2.0.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1505 2023-07-26 07:54:32.253432 django_sortedm2m_filter_horizontal_widget-2.0.0/LICENSE.txt
--rw-r--r--   0        0        0     1357 2023-07-26 08:52:09.289241 django_sortedm2m_filter_horizontal_widget-2.0.0/README.md
--rw-r--r--   0        0        0      484 2023-07-26 08:57:57.707299 django_sortedm2m_filter_horizontal_widget-2.0.0/pyproject.toml
--rw-r--r--   0        0        0       48 2023-07-26 07:54:32.254256 django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/__init__.py
--rw-r--r--   0        0        0     6980 2023-07-26 08:36:26.261010 django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/forms.py
--rw-r--r--   0        0        0     6235 2023-07-26 07:54:32.254465 django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/OrderedSelectBox.js
--rw-r--r--   0        0        0    11713 2023-07-26 07:54:32.254565 django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/OrderedSelectFilter.js
--rw-r--r--   0        0        0    85925 2023-07-26 07:54:32.254920 django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/jquery.min.js
--rw-r--r--   0        0        0     2372 2023-07-26 09:02:47.966285 django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/widget.css
--rw-r--r--   0        0        0     2166 1970-01-01 00:00:00.000000 django_sortedm2m_filter_horizontal_widget-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-07-26 07:54:32.253432 django_sortedm2m_filter_horizontal_widget-2.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1357 2023-07-26 09:16:17.814508 django_sortedm2m_filter_horizontal_widget-2.0.1/README.md
+-rw-r--r--   0        0        0      617 2023-07-26 10:25:54.152143 django_sortedm2m_filter_horizontal_widget-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 10:27:00.232842 django_sortedm2m_filter_horizontal_widget-2.0.1/sortedm2m_filter_horizontal_widget/__init__.py
+-rw-r--r--   0        0        0     6731 2023-07-26 10:27:00.230704 django_sortedm2m_filter_horizontal_widget-2.0.1/sortedm2m_filter_horizontal_widget/forms.py
+-rw-r--r--   0        0        0     6235 2023-07-26 07:54:32.254465 django_sortedm2m_filter_horizontal_widget-2.0.1/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/OrderedSelectBox.js
+-rw-r--r--   0        0        0    11713 2023-07-26 07:54:32.254565 django_sortedm2m_filter_horizontal_widget-2.0.1/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/OrderedSelectFilter.js
+-rw-r--r--   0        0        0      473 2023-07-26 09:51:51.926071 django_sortedm2m_filter_horizontal_widget-2.0.1/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/SelectAddButton.js
+-rw-r--r--   0        0        0    85925 2023-07-26 07:54:32.254920 django_sortedm2m_filter_horizontal_widget-2.0.1/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/jquery.min.js
+-rw-r--r--   0        0        0     2260 2023-07-26 09:54:21.723745 django_sortedm2m_filter_horizontal_widget-2.0.1/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/widget.css
+-rw-r--r--   0        0        0     2016 1970-01-01 00:00:00.000000 django_sortedm2m_filter_horizontal_widget-2.0.1/PKG-INFO
```

### Comparing `django_sortedm2m_filter_horizontal_widget-2.0.0/LICENSE.txt` & `django_sortedm2m_filter_horizontal_widget-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_sortedm2m_filter_horizontal_widget-2.0.0/README.md` & `django_sortedm2m_filter_horizontal_widget-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/forms.py` & `django_sortedm2m_filter_horizontal_widget-2.0.1/sortedm2m_filter_horizontal_widget/forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,36 @@
-# -*- coding: utf-8 -*-
-import sys
 from itertools import chain
 from django import forms
 from django.conf import settings
 from django.db.models.query import QuerySet
 from django.utils.encoding import force_str
 from django.utils.html import conditional_escape, escape
 from django.utils.safestring import mark_safe
 
-try:
-    from django.forms.utils import flatatt
-except ImportError:
-    from django.forms.util import flatatt
+from django.forms.utils import flatatt
 
-from django.utils.translation import gettext_lazy as _
-
-
-if sys.version_info[0] < 3:
-    iteritems = lambda d: iter(d.iteritems())
-    string_types = basestring,
-    str_ = unicode
-else:
-    iteritems = lambda d: iter(d.items())
-    string_types = str,
-    str_ = str
-
-
-STATIC_URL = getattr(settings, 'STATIC_URL', settings.MEDIA_URL)
+STATIC_URL = getattr(settings, "STATIC_URL", settings.MEDIA_URL)
 
 
 class SortedMultipleChoiceField(forms.ModelMultipleChoiceField):
     def __init__(self, *args, **kwargs):
-        if not kwargs.get('widget'):
-            kwargs['widget'] = SortedFilteredSelectMultiple(
-                is_stacked=kwargs.get('is_stacked', False)
+        if not kwargs.get("widget"):
+            kwargs["widget"] = SortedFilteredSelectMultiple(
+                is_stacked=kwargs.get("is_stacked", False)
             )
         super(SortedMultipleChoiceField, self).__init__(*args, **kwargs)
 
     def clean(self, value):
         queryset = super(SortedMultipleChoiceField, self).clean(value)
         if value is None or not isinstance(queryset, QuerySet):
             return queryset
-        object_list = dict((
-            (str_(key), value)
-            for key, value in iteritems(queryset.in_bulk(value))))
-        return [object_list[str_(pk)] for pk in value]
+        object_list = dict(
+            ((str(key), value) for key, value in iter(queryset.in_bulk(value).items()))
+        )
+        return [object_list[str(pk)] for pk in value]
 
     def _has_changed(self, initial, data):
         if initial is None:
             initial = []
         if data is None:
             data = []
         if len(initial) != len(data):
@@ -58,61 +40,71 @@
         return data_set != initial_set
 
 
 class SortedFilteredSelectMultiple(forms.SelectMultiple):
     """
     A SortableSelectMultiple with a JavaScript filter interface.
 
-	Requires jQuery to be loaded.
+        Requires jQuery to be loaded.
 
     Note that the resulting JavaScript assumes that the jsi18n
     catalog has been loaded in the page
     """
 
     def __init__(self, is_stacked=False, attrs=None, choices=()):
         self.is_stacked = is_stacked
         super(SortedFilteredSelectMultiple, self).__init__(attrs, choices)
 
     class Media:
         css = {
-            'screen': (STATIC_URL + 'sortedm2m_filter_horizontal_widget/widget.css',)
+            "screen": (STATIC_URL + "sortedm2m_filter_horizontal_widget/widget.css",)
         }
 
-        js = (STATIC_URL + 'sortedm2m_filter_horizontal_widget/OrderedSelectBox.js',
-              STATIC_URL + 'sortedm2m_filter_horizontal_widget/OrderedSelectFilter.js',
-              STATIC_URL + 'sortedm2m_filter_horizontal_widget/jquery.min.js')
+        js = (
+            STATIC_URL + "sortedm2m_filter_horizontal_widget/OrderedSelectBox.js",
+            STATIC_URL + "sortedm2m_filter_horizontal_widget/OrderedSelectFilter.js",
+            STATIC_URL + "sortedm2m_filter_horizontal_widget/jquery.min.js",
+        )
 
     def build_attrs(self, attrs=None, extra_attrs=None, **kwargs):
         attrs = dict(attrs, **kwargs)
         if extra_attrs:
             attrs.update(extra_attrs)
-        classes = attrs.setdefault('class', '').split()
-        classes.append('sortedm2m')
-        if self.is_stacked: classes.append('stacked')
-        attrs['class'] = u' '.join(classes)
+        classes = attrs.setdefault("class", "").split()
+        classes.append("sortedm2m")
+        if self.is_stacked:
+            classes.append("stacked")
+        attrs["class"] = " ".join(classes)
         return attrs
 
     def render(self, name, value, attrs=None, choices=(), renderer=None):
-        if attrs is None: attrs = {}
-        if value is None: value = []
-        admin_media_prefix = getattr(settings, 'ADMIN_MEDIA_PREFIX', STATIC_URL + 'admin/')
+        if attrs is None:
+            attrs = {}
+        if value is None:
+            value = []
+        admin_media_prefix = getattr(
+            settings, "ADMIN_MEDIA_PREFIX", STATIC_URL + "admin/"
+        )
         final_attrs = self.build_attrs(self.attrs, attrs, name=name)
-        output = [u'<select multiple="multiple"%s>' % flatatt(final_attrs)]
+        output = [f'<select multiple="multiple"{flatatt(final_attrs)}>']
         options = self.render_options(choices, value)
         if options:
             output.append(options)
-        if 'verbose_name' in final_attrs.keys():
-            verbose_name = final_attrs['verbose_name']
+        if "verbose_name" in final_attrs.keys():
+            verbose_name = final_attrs["verbose_name"]
         else:
-            verbose_name = name.split('-')[-1]
-        output.append(u'</select>')
-        output.append(u'<script>window.addEventListener("load", function(e) {')
-        output.append(u'OrderedSelectFilter.init("id_%s", "%s", %s, "%s") });</script>\n' % \
-                      (name, verbose_name, int(self.is_stacked), admin_media_prefix))
-        output.append(u"""
+            verbose_name = name.split("-")[-1]
+        output.append("</select>")
+        output.append('<script>window.addEventListener("load", function(e) {')
+        output.append(
+            f"OrderedSelectFilter.init('id_{name}', '{verbose_name}', {int(self.is_stacked)}, '{admin_media_prefix}')"
+        )
+        output.append("});</script>\n")
+        output.append(
+            """
         <script>
         (function($) {
             $(document).ready(function() {
                 var updateOrderedSelectFilter = function() {
                     // If any SelectFilter widgets are a part of the new form,
                     // instantiate a new SelectFilter instance for it.
                     if (typeof OrderedSelectFilter != "undefined"){
@@ -127,44 +119,48 @@
                     }
                 }
                 $(document).on('formset:added', function(row, prefix) {
                     updateOrderedSelectFilter();
                 });
             });
         })(django.jQuery)
-        </script>""" % (admin_media_prefix, admin_media_prefix))
+        </script>"""
+            % (admin_media_prefix, admin_media_prefix)
+        )
 
-        return mark_safe(u'\n'.join(output))
+        return mark_safe("\n".join(output))
 
     def render_option(self, selected_choices, option_value, option_label):
         option_value = force_str(option_value)
-        selected_html = (option_value in selected_choices) and u' selected="selected"' or ''
+        selected_html = (
+            (option_value in selected_choices) and ' selected="selected"' or ""
+        )
         try:
             index = list(selected_choices).index(escape(option_value))
-            selected_html = u'%s %s' % (u' data-sort-value="%s"' % index, selected_html)
+            selected_html = f' data-sort-value="{index}" {selected_html}'
         except ValueError:
             pass
 
-        return u'<option value="%s"%s>%s</option>' % (
-            escape(option_value), selected_html,
-            conditional_escape(force_str(option_label)))
+        return f'<option value="{escape(option_value)}"{selected_html}>{conditional_escape(force_str(option_label))}</option>'
 
     def render_options(self, choices, selected_choices):
         # Normalize to strings.
         selected_choices = list(force_str(v) for v in selected_choices)
         output = []
         for option_value, option_label in chain(self.choices, choices):
             if isinstance(option_label, (list, tuple)):
-                output.append(u'<optgroup label="%s">' % escape(force_str(option_value)))
+                output.append(f'<optgroup label="{escape(force_str(option_value))}">')
                 for option in option_label:
                     output.append(self.render_option(selected_choices, *option))
-                output.append(u'</optgroup>')
+                output.append("</optgroup>")
             else:
-                output.append(self.render_option(selected_choices, option_value, option_label))
-        return u'\n'.join(output)
+                output.append(
+                    self.render_option(selected_choices, option_value, option_label)
+                )
+        return "\n".join(output)
 
     def _has_changed(self, initial, data):
         if initial is None:
             initial = []
         if data is None:
             data = []
         if len(initial) != len(data):
```

### Comparing `django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/OrderedSelectBox.js` & `django_sortedm2m_filter_horizontal_widget-2.0.1/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/OrderedSelectBox.js`

 * *Files identical despite different names*

### Comparing `django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/OrderedSelectFilter.js` & `django_sortedm2m_filter_horizontal_widget-2.0.1/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/OrderedSelectFilter.js`

 * *Files identical despite different names*

### Comparing `django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/jquery.min.js` & `django_sortedm2m_filter_horizontal_widget-2.0.1/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django_sortedm2m_filter_horizontal_widget-2.0.0/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/widget.css` & `django_sortedm2m_filter_horizontal_widget-2.0.1/sortedm2m_filter_horizontal_widget/static/sortedm2m_filter_horizontal_widget/widget.css`

 * *Files 3% similar despite different names*

```diff
@@ -94,20 +94,14 @@
 .selector-up:hover {
   background-position: 0 -15px;
 }
 .selector-down:hover {
   background-position: 0 -47px;
 }
 
-/* Pull add-related button to the left: */
-.related-widget-wrapper-link.add-related {
-  margin-left: -26px;
-}
-
-
 @media (max-width: 1024px) {
   .selector-up {
     background: url(../admin/img/selector-icons.svg) 0 0 no-repeat;
   }
   .selector-down {
     background: url(../admin/img/selector-icons.svg) 0 -41px no-repeat;
   }
```

### Comparing `django_sortedm2m_filter_horizontal_widget-2.0.0/PKG-INFO` & `django_sortedm2m_filter_horizontal_widget-2.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: django-sortedm2m-filter-horizontal-widget
-Version: 2.0.0
+Version: 2.0.1
 Summary: Django admin widget for Gregor Mülleggers django-sortedm2m_ library
 License: BSD
 Author: Sander van Leeuwen
 Author-email: replytosander@gmail.com
-Requires-Python: >=3.5,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django-sortedm2m (>=3.1.1,<4.0.0)
 Description-Content-Type: text/markdown
```


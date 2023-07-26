# Comparing `tmp/wagtail-generic-chooser-0.5.1.tar.gz` & `tmp/wagtail-generic-chooser-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wagtail-generic-chooser-0.5.1.tar", last modified: Tue Jan 24 10:30:13 2023, max compression
+gzip compressed data, was "wagtail-generic-chooser-0.6.tar", last modified: Wed Jul 26 17:25:38 2023, max compression
```

## Comparing `wagtail-generic-chooser-0.5.1.tar` & `wagtail-generic-chooser-0.6.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-24 10:30:13.808594 wagtail-generic-chooser-0.5.1/
--rw-r--r--   0 matthew    (501) staff       (20)     1884 2023-01-24 10:29:20.000000 wagtail-generic-chooser-0.5.1/CHANGELOG.txt
--rw-r--r--   0 matthew    (501) staff       (20)     1508 2019-03-25 18:41:22.000000 wagtail-generic-chooser-0.5.1/LICENSE
--rw-r--r--   0 matthew    (501) staff       (20)      157 2020-10-08 13:55:55.000000 wagtail-generic-chooser-0.5.1/MANIFEST.in
--rw-r--r--   0 matthew    (501) staff       (20)     1203 2023-01-24 10:30:13.808182 wagtail-generic-chooser-0.5.1/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)    15862 2022-11-28 18:27:08.000000 wagtail-generic-chooser-0.5.1/README.md
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-24 10:30:13.796644 wagtail-generic-chooser-0.5.1/generic_chooser/
--rw-r--r--   0 matthew    (501) staff       (20)        0 2019-03-25 19:36:09.000000 wagtail-generic-chooser-0.5.1/generic_chooser/__init__.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-24 10:30:13.791706 wagtail-generic-chooser-0.5.1/generic_chooser/static/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-24 10:30:13.791805 wagtail-generic-chooser-0.5.1/generic_chooser/static/generic_chooser/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-24 10:30:13.800748 wagtail-generic-chooser-0.5.1/generic_chooser/static/generic_chooser/js/
--rw-r--r--   0 matthew    (501) staff       (20)     3391 2023-01-23 13:27:20.000000 wagtail-generic-chooser-0.5.1/generic_chooser/static/generic_chooser/js/chooser-modal.js
--rw-r--r--   0 matthew    (501) staff       (20)      136 2023-01-23 13:27:20.000000 wagtail-generic-chooser-0.5.1/generic_chooser/static/generic_chooser/js/chooser-widget-telepath.js
--rw-r--r--   0 matthew    (501) staff       (20)     4426 2023-01-24 10:26:56.000000 wagtail-generic-chooser-0.5.1/generic_chooser/static/generic_chooser/js/chooser-widget.js
--rw-r--r--   0 matthew    (501) staff       (20)      144 2023-01-23 13:27:20.000000 wagtail-generic-chooser-0.5.1/generic_chooser/static/generic_chooser/js/linked-field-chooser-widget-telepath.js
--rw-r--r--   0 matthew    (501) staff       (20)     2628 2023-01-24 10:26:56.000000 wagtail-generic-chooser-0.5.1/generic_chooser/static/generic_chooser/js/linked-field-chooser-widget.js
--rw-r--r--   0 matthew    (501) staff       (20)    10527 2022-06-10 15:53:55.000000 wagtail-generic-chooser-0.5.1/generic_chooser/static/generic_chooser/js/tabs.js
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-24 10:30:13.792137 wagtail-generic-chooser-0.5.1/generic_chooser/templates/
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-24 10:30:13.804108 wagtail-generic-chooser-0.5.1/generic_chooser/templates/generic_chooser/
--rw-r--r--   0 matthew    (501) staff       (20)      746 2022-06-10 13:14:38.000000 wagtail-generic-chooser-0.5.1/generic_chooser/templates/generic_chooser/_ajax_pagination_nav.html
--rw-r--r--   0 matthew    (501) staff       (20)      981 2019-06-17 11:55:14.000000 wagtail-generic-chooser-0.5.1/generic_chooser/templates/generic_chooser/_create_tab.html
--rw-r--r--   0 matthew    (501) staff       (20)      899 2023-01-23 13:27:20.000000 wagtail-generic-chooser-0.5.1/generic_chooser/templates/generic_chooser/_listing_tab.html
--rw-r--r--   0 matthew    (501) staff       (20)     1029 2023-01-23 13:27:20.000000 wagtail-generic-chooser-0.5.1/generic_chooser/templates/generic_chooser/_results.html
--rw-r--r--   0 matthew    (501) staff       (20)      948 2022-06-10 15:53:55.000000 wagtail-generic-chooser-0.5.1/generic_chooser/templates/generic_chooser/tabbed_modal.html
--rw-r--r--   0 matthew    (501) staff       (20)     1087 2022-11-28 18:27:08.000000 wagtail-generic-chooser-0.5.1/generic_chooser/templates/generic_chooser/tabbed_modal_v3.html
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-24 10:30:13.805529 wagtail-generic-chooser-0.5.1/generic_chooser/templates/generic_chooser/widgets/
--rw-r--r--   0 matthew    (501) staff       (20)     2108 2022-12-05 17:09:46.000000 wagtail-generic-chooser-0.5.1/generic_chooser/templates/generic_chooser/widgets/chooser.html
--rw-r--r--   0 matthew    (501) staff       (20)     2347 2022-12-05 17:09:46.000000 wagtail-generic-chooser-0.5.1/generic_chooser/templates/generic_chooser/widgets/chooser_v4.html
--rw-r--r--   0 matthew    (501) staff       (20)    27254 2023-01-23 13:27:20.000000 wagtail-generic-chooser-0.5.1/generic_chooser/views.py
--rw-r--r--   0 matthew    (501) staff       (20)    11379 2023-01-23 13:27:20.000000 wagtail-generic-chooser-0.5.1/generic_chooser/widgets.py
--rw-r--r--   0 matthew    (501) staff       (20)       38 2023-01-24 10:30:13.808883 wagtail-generic-chooser-0.5.1/setup.cfg
--rw-r--r--   0 matthew    (501) staff       (20)     1432 2023-01-24 10:29:41.000000 wagtail-generic-chooser-0.5.1/setup.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-01-24 10:30:13.807766 wagtail-generic-chooser-0.5.1/wagtail_generic_chooser.egg-info/
--rw-r--r--   0 matthew    (501) staff       (20)     1203 2023-01-24 10:30:13.000000 wagtail-generic-chooser-0.5.1/wagtail_generic_chooser.egg-info/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)     1254 2023-01-24 10:30:13.000000 wagtail-generic-chooser-0.5.1/wagtail_generic_chooser.egg-info/SOURCES.txt
--rw-r--r--   0 matthew    (501) staff       (20)        1 2023-01-24 10:30:13.000000 wagtail-generic-chooser-0.5.1/wagtail_generic_chooser.egg-info/dependency_links.txt
--rw-r--r--   0 matthew    (501) staff       (20)       22 2023-01-24 10:30:13.000000 wagtail-generic-chooser-0.5.1/wagtail_generic_chooser.egg-info/requires.txt
--rw-r--r--   0 matthew    (501) staff       (20)       16 2023-01-24 10:30:13.000000 wagtail-generic-chooser-0.5.1/wagtail_generic_chooser.egg-info/top_level.txt
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-07-26 17:25:38.983164 wagtail-generic-chooser-0.6/
+-rw-r--r--   0 matthew    (501) staff       (20)     2071 2023-07-26 17:19:49.000000 wagtail-generic-chooser-0.6/CHANGELOG.txt
+-rw-r--r--   0 matthew    (501) staff       (20)     1508 2019-03-25 18:41:22.000000 wagtail-generic-chooser-0.6/LICENSE
+-rw-r--r--   0 matthew    (501) staff       (20)      157 2020-10-08 13:55:55.000000 wagtail-generic-chooser-0.6/MANIFEST.in
+-rw-r--r--   0 matthew    (501) staff       (20)     1286 2023-07-26 17:25:38.982741 wagtail-generic-chooser-0.6/PKG-INFO
+-rw-r--r--   0 matthew    (501) staff       (20)    15852 2023-07-26 13:21:15.000000 wagtail-generic-chooser-0.6/README.md
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-07-26 17:25:38.965916 wagtail-generic-chooser-0.6/generic_chooser/
+-rw-r--r--   0 matthew    (501) staff       (20)        0 2019-03-25 19:36:09.000000 wagtail-generic-chooser-0.6/generic_chooser/__init__.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-07-26 17:25:38.959309 wagtail-generic-chooser-0.6/generic_chooser/static/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-07-26 17:25:38.959435 wagtail-generic-chooser-0.6/generic_chooser/static/generic_chooser/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-07-26 17:25:38.972504 wagtail-generic-chooser-0.6/generic_chooser/static/generic_chooser/js/
+-rw-r--r--   0 matthew    (501) staff       (20)     3391 2023-01-23 13:27:20.000000 wagtail-generic-chooser-0.6/generic_chooser/static/generic_chooser/js/chooser-modal.js
+-rw-r--r--   0 matthew    (501) staff       (20)      136 2023-01-23 13:27:20.000000 wagtail-generic-chooser-0.6/generic_chooser/static/generic_chooser/js/chooser-widget-telepath.js
+-rw-r--r--   0 matthew    (501) staff       (20)     4426 2023-01-24 10:26:56.000000 wagtail-generic-chooser-0.6/generic_chooser/static/generic_chooser/js/chooser-widget.js
+-rw-r--r--   0 matthew    (501) staff       (20)      144 2023-01-23 13:27:20.000000 wagtail-generic-chooser-0.6/generic_chooser/static/generic_chooser/js/linked-field-chooser-widget-telepath.js
+-rw-r--r--   0 matthew    (501) staff       (20)     2628 2023-01-24 10:26:56.000000 wagtail-generic-chooser-0.6/generic_chooser/static/generic_chooser/js/linked-field-chooser-widget.js
+-rw-r--r--   0 matthew    (501) staff       (20)    10527 2022-06-10 15:53:55.000000 wagtail-generic-chooser-0.6/generic_chooser/static/generic_chooser/js/tabs.js
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-07-26 17:25:38.959784 wagtail-generic-chooser-0.6/generic_chooser/templates/
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-07-26 17:25:38.978575 wagtail-generic-chooser-0.6/generic_chooser/templates/generic_chooser/
+-rw-r--r--   0 matthew    (501) staff       (20)      746 2022-06-10 13:14:38.000000 wagtail-generic-chooser-0.6/generic_chooser/templates/generic_chooser/_ajax_pagination_nav.html
+-rw-r--r--   0 matthew    (501) staff       (20)     1572 2023-07-26 17:12:43.000000 wagtail-generic-chooser-0.6/generic_chooser/templates/generic_chooser/_create_tab.html
+-rw-r--r--   0 matthew    (501) staff       (20)      899 2023-01-23 13:27:20.000000 wagtail-generic-chooser-0.6/generic_chooser/templates/generic_chooser/_listing_tab.html
+-rw-r--r--   0 matthew    (501) staff       (20)     1029 2023-01-23 13:27:20.000000 wagtail-generic-chooser-0.6/generic_chooser/templates/generic_chooser/_results.html
+-rw-r--r--   0 matthew    (501) staff       (20)      948 2022-06-10 15:53:55.000000 wagtail-generic-chooser-0.6/generic_chooser/templates/generic_chooser/tabbed_modal.html
+-rw-r--r--   0 matthew    (501) staff       (20)     1087 2022-11-28 18:27:08.000000 wagtail-generic-chooser-0.6/generic_chooser/templates/generic_chooser/tabbed_modal_v3.html
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-07-26 17:25:38.979621 wagtail-generic-chooser-0.6/generic_chooser/templates/generic_chooser/widgets/
+-rw-r--r--   0 matthew    (501) staff       (20)     2367 2023-07-26 17:18:23.000000 wagtail-generic-chooser-0.6/generic_chooser/templates/generic_chooser/widgets/chooser.html
+-rw-r--r--   0 matthew    (501) staff       (20)    26983 2023-07-26 17:09:40.000000 wagtail-generic-chooser-0.6/generic_chooser/views.py
+-rw-r--r--   0 matthew    (501) staff       (20)     9429 2023-07-26 17:18:23.000000 wagtail-generic-chooser-0.6/generic_chooser/widgets.py
+-rw-r--r--   0 matthew    (501) staff       (20)       38 2023-07-26 17:25:38.983251 wagtail-generic-chooser-0.6/setup.cfg
+-rw-r--r--   0 matthew    (501) staff       (20)     1544 2023-07-26 17:24:57.000000 wagtail-generic-chooser-0.6/setup.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-07-26 17:25:38.982340 wagtail-generic-chooser-0.6/wagtail_generic_chooser.egg-info/
+-rw-r--r--   0 matthew    (501) staff       (20)     1286 2023-07-26 17:25:38.000000 wagtail-generic-chooser-0.6/wagtail_generic_chooser.egg-info/PKG-INFO
+-rw-r--r--   0 matthew    (501) staff       (20)     1188 2023-07-26 17:25:38.000000 wagtail-generic-chooser-0.6/wagtail_generic_chooser.egg-info/SOURCES.txt
+-rw-r--r--   0 matthew    (501) staff       (20)        1 2023-07-26 17:25:38.000000 wagtail-generic-chooser-0.6/wagtail_generic_chooser.egg-info/dependency_links.txt
+-rw-r--r--   0 matthew    (501) staff       (20)       22 2023-07-26 17:25:38.000000 wagtail-generic-chooser-0.6/wagtail_generic_chooser.egg-info/requires.txt
+-rw-r--r--   0 matthew    (501) staff       (20)       16 2023-07-26 17:25:38.000000 wagtail-generic-chooser-0.6/wagtail_generic_chooser.egg-info/top_level.txt
```

### Comparing `wagtail-generic-chooser-0.5.1/CHANGELOG.txt` & `wagtail-generic-chooser-0.6/CHANGELOG.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+0.6 (2023-07-26)
+----------------
+
+* Wagtail 4.2, 5.0 and 5.1 support (Katherine Domingo, Matt Westcott)
+* Remove conditional code for Wagtail versions prior to 4.1 (Katherine Domingo)
+
+
 0.5.1 (2023-01-24)
 ------------------
 
 * Fix: Ensure `LinkedFieldChooserWidgetFactory.openModal` passes the linked field URL parameters to the modal (Matt Westcott)
 
 
 0.5 (2022-12-05)
```

### Comparing `wagtail-generic-chooser-0.5.1/LICENSE` & `wagtail-generic-chooser-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-generic-chooser-0.5.1/README.md` & `wagtail-generic-chooser-0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 It differs from existing model chooser add-ons ([Naeka/wagtailmodelchooser](https://github.com/Naeka/wagtailmodelchooser/), [neon-jungle/wagtailmodelchooser](https://github.com/neon-jungle/wagtailmodelchooser), [springload/wagtailmodelchoosers](https://github.com/springload/wagtailmodelchoosers)) in that it is designed to be fully configurable through subclassing - in particular, it can be used on data sources other than Django models, such as REST API endpoints.
 
 It is intended that `wagtail-generic-chooser` will be expanded to cover all the functionality of Wagtail's built-in choosers, such as inline object creation forms, and will then be incorporated into Wagtail as the new base implementation of those built-in choosers - this will reduce code duplication and greatly simplify the process of building new admin apps.
 
 ## Requirements
 
-Wagtail 2.4 or higher
+Wagtail 4.1 or higher
 
 ## Installation
 
 Run: `pip install wagtail-generic-chooser`
 
 Then add `generic_chooser` to your project's `INSTALLED_APPS`.
 
@@ -46,15 +46,15 @@
 ```
 
 The viewset can then be registered through Wagtail's `register_admin_viewset` hook:
 
 ```python
 # myapp/wagtail_hooks.py
 
-from wagtail.core import hooks
+from wagtail import hooks
 
 from myapp.views import PersonChooserViewSet
 
 
 @hooks.register('register_admin_viewset')
 def register_person_chooser_viewset():
     return PersonChooserViewSet('person_chooser', url_prefix='person-chooser')
@@ -265,15 +265,15 @@
 
 
 ### StreamField blocks
 
 A chooser widget as defined above can be wrapped in Wagtail's `ChooserBlock` class to be used inside a StreamField. As of Wagtail 2.13, the block definition should be as follows:
 
 ```python
-from wagtail.core.blocks import ChooserBlock
+from wagtail.blocks import ChooserBlock
 
 
 class PersonChooserBlock(ChooserBlock):
     @cached_property
     def target_model(self):
         from .models import Person
         return Person
```

### Comparing `wagtail-generic-chooser-0.5.1/generic_chooser/static/generic_chooser/js/chooser-modal.js` & `wagtail-generic-chooser-0.6/generic_chooser/static/generic_chooser/js/chooser-modal.js`

 * *Files identical despite different names*

### Comparing `wagtail-generic-chooser-0.5.1/generic_chooser/static/generic_chooser/js/chooser-widget.js` & `wagtail-generic-chooser-0.6/generic_chooser/static/generic_chooser/js/chooser-widget.js`

 * *Files identical despite different names*

### Comparing `wagtail-generic-chooser-0.5.1/generic_chooser/static/generic_chooser/js/linked-field-chooser-widget.js` & `wagtail-generic-chooser-0.6/generic_chooser/static/generic_chooser/js/linked-field-chooser-widget.js`

 * *Files identical despite different names*

### Comparing `wagtail-generic-chooser-0.5.1/generic_chooser/static/generic_chooser/js/tabs.js` & `wagtail-generic-chooser-0.6/generic_chooser/static/generic_chooser/js/tabs.js`

 * *Files identical despite different names*

### Comparing `wagtail-generic-chooser-0.5.1/generic_chooser/templates/generic_chooser/_ajax_pagination_nav.html` & `wagtail-generic-chooser-0.6/generic_chooser/templates/generic_chooser/_ajax_pagination_nav.html`

 * *Files identical despite different names*

### Comparing `wagtail-generic-chooser-0.5.1/generic_chooser/templates/generic_chooser/_listing_tab.html` & `wagtail-generic-chooser-0.6/generic_chooser/templates/generic_chooser/_listing_tab.html`

 * *Files identical despite different names*

### Comparing `wagtail-generic-chooser-0.5.1/generic_chooser/templates/generic_chooser/_results.html` & `wagtail-generic-chooser-0.6/generic_chooser/templates/generic_chooser/_results.html`

 * *Files identical despite different names*

### Comparing `wagtail-generic-chooser-0.5.1/generic_chooser/templates/generic_chooser/tabbed_modal.html` & `wagtail-generic-chooser-0.6/generic_chooser/templates/generic_chooser/tabbed_modal.html`

 * *Files identical despite different names*

### Comparing `wagtail-generic-chooser-0.5.1/generic_chooser/templates/generic_chooser/tabbed_modal_v3.html` & `wagtail-generic-chooser-0.6/generic_chooser/templates/generic_chooser/tabbed_modal_v3.html`

 * *Files identical despite different names*

### Comparing `wagtail-generic-chooser-0.5.1/generic_chooser/templates/generic_chooser/widgets/chooser.html` & `wagtail-generic-chooser-0.6/generic_chooser/templates/generic_chooser/widgets/chooser.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,30 @@
+{% load wagtailadmin_tags %}
+
 {% comment %}
     Either the chosen or unchosen div will be shown, depending on the presence
     of the 'blank' class on the container.
 
     Any element with the 'action-choose' class will open the page chooser modal
     when clicked.
 {% endcomment %}
 
 <div id="{{ attrs.id }}-chooser" class="chooser {% block chooser_class %}{{ widget.classname }}{% endblock %} {% if is_empty %}blank{% endif %}" {% if choose_modal_url %}data-choose-modal-url="{{ choose_modal_url }}"{% endif %}>
 
     <div class="chosen">
+        {% block chosen_icon %}
+            <div class="chooser__preview" role="presentation">
+                {% icon name=widget.icon classname="default" %}
+            </div>
+        {% endblock chosen_icon %}
         {% block chosen_state_view %}
-            <span class="title" data-chooser-title>{{ title }}</span>
+            <div class="chooser__title" data-chooser-title>{{ title }}</div>
         {% endblock %}
 
-        <ul class="actions">
+        <ul class="chooser__actions">
             {% if not widget.is_required %}
                 <li><button type="button" class="button action-clear button-small button-secondary">{{ widget.clear_choice_text }}</button></li>
             {% endif %}
             <li><button type="button" class="button action-choose button-small button-secondary">{{ widget.choose_another_text }}</button></li>
             {% if widget.show_edit_link %}
                 <li class="edit-link-wrapper"><a {% if edit_item_url %}href="{{ edit_item_url }}"{% endif %} class="edit-link button button-small button-secondary" target="_blank" rel="noopener noreferrer">{{ widget.link_to_chosen_text }}</a></li>
             {% endif %}
```

#### html2text {}

```diff
@@ -1,13 +1,18 @@
-{% comment %} Either the chosen or unchosen div will be shown, depending on the
-presence of the 'blank' class on the container. Any element with the 'action-
-choose' class will open the page chooser modal when clicked. {% endcomment %}
+{% load wagtailadmin_tags %} {% comment %} Either the chosen or unchosen div
+will be shown, depending on the presence of the 'blank' class on the container.
+Any element with the 'action-choose' class will open the page chooser modal
+when clicked. {% endcomment %}
 % if choose_modal_url %}data-choose-modal-url="{{ choose_modal_url }}"{% endif
 %}>
-{% block chosen_state_view %} {{ title }} {% endblock %}
+{% block chosen_icon %}
+{% icon name=widget.icon classname="default" %}
+{% endblock chosen_icon %} {% block chosen_state_view %}
+{{ title }}
+{% endblock %}
     * {% if not widget.is_required %}
     * {{ widget.clear_choice_text }}
     * {% endif %}
     * {{ widget.choose_another_text }}
     * {% if widget.show_edit_link %}
     * % if edit_item_url %}href="{{ edit_item_url }}"{% endif %} class="edit-
       link button button-small button-secondary" target="_blank" rel="noopener
```

### Comparing `wagtail-generic-chooser-0.5.1/generic_chooser/views.py` & `wagtail-generic-chooser-0.6/generic_chooser/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,25 @@
-import requests
 import urllib
 
+import requests
 from django.contrib.admin.utils import quote, unquote
 from django.core.exceptions import ObjectDoesNotExist, PermissionDenied
 from django.core.paginator import Page, Paginator
 from django.forms import models as model_forms
 from django.http import Http404
 from django.shortcuts import render
 from django.urls import re_path, reverse
 from django.utils.text import camel_case_to_spaces, slugify
 from django.utils.translation import gettext_lazy as _
 from django.views import View
 from django.views.generic.base import ContextMixin
-
-from wagtail import VERSION as WAGTAIL_VERSION
 from wagtail.admin.forms.search import SearchForm
 from wagtail.admin.modal_workflow import render_modal_workflow
 from wagtail.admin.viewsets.base import ViewSet
-
-try:
-    from wagtail.permission_policies import ModelPermissionPolicy
-except ImportError:
-    # Wagtail<3.0
-    from wagtail.core.permission_policies import ModelPermissionPolicy
-
+from wagtail.permission_policies import ModelPermissionPolicy
 from wagtail.search.backends import get_search_backend
 from wagtail.search.index import class_is_indexed
 
 
 class ModalPageFurnitureMixin(ContextMixin):
     """
     Add icon and page title to the template context
@@ -516,18 +508,15 @@
         return result.json()
 
 
 class BaseChooseView(ModalPageFurnitureMixin, ContextMixin, View):
     icon = 'snippet'
     page_title = _("Choose")
 
-    if WAGTAIL_VERSION >= (3, 0):
-        template = 'generic_chooser/tabbed_modal_v3.html'
-    else:
-        template = 'generic_chooser/tabbed_modal.html'
+    template = 'generic_chooser/tabbed_modal_v3.html'
 
     def get_template(self):
         return self.template
 
     def get(self, request):
         # 'results=true' URL param indicates we should only render the results partial
         # rather than serving a full ModalWorkflow response
```

### Comparing `wagtail-generic-chooser-0.5.1/generic_chooser/widgets.py` & `wagtail-generic-chooser-0.6/generic_chooser/widgets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,20 @@
 import json
 
+import requests
 from django.contrib.admin.utils import quote
 from django.core.exceptions import ObjectDoesNotExist
-from django.forms import widgets, Media
+from django.forms import Media, widgets
 from django.template.loader import render_to_string
 from django.urls import reverse
 from django.utils.translation import gettext_lazy as _
-
-import requests
-
-from wagtail import VERSION as WAGTAIL_VERSION
+from wagtail.telepath import register
 from wagtail.utils.widgets import WidgetWithScript
+from wagtail.widget_adapters import WidgetAdapter
 
-try:
-    from wagtail.telepath import register
-except ImportError:
-    try:
-        # Wagtail<3.0
-        from wagtail.core.telepath import register
-    except ImportError:  # do-nothing fallback for Wagtail <2.13
-        def register(adapter, cls):
-            pass
-
-try:
-    from wagtail.widget_adapters import WidgetAdapter
-except ImportError:
-    try:
-        # Wagtail<3.0
-        from wagtail.core.widget_adapters import WidgetAdapter
-    except ImportError:  # do-nothing fallback for Wagtail <2.13
-        class WidgetAdapter:
-            pass
 
 class AdminChooser(WidgetWithScript, widgets.Input):
     input_type = 'hidden'
     choose_one_text = _("Choose an item")
     choose_another_text = _("Choose another item")
     clear_choice_text = _("Clear choice")
     link_to_chosen_text = _("Edit this item")
@@ -60,18 +40,15 @@
     # URL route name for the chooser modal view - should return the URL of the chooser view when
     # reversed with no arguments. If no suitable URL route exists, subclasses can override
     # get_choose_modal_url instead.
     # This will appear as the attribute data-choose-modal-url on the top-level element of the
     # chooser widget.
     choose_modal_url_name = None
 
-    if WAGTAIL_VERSION >= (4, 0):
-        template = "generic_chooser/widgets/chooser_v4.html"
-    else:
-        template = "generic_chooser/widgets/chooser.html"
+    template = "generic_chooser/widgets/chooser.html"
 
     js_constructor_name = "ChooserWidget"
 
     # when looping over form fields, this one should appear in visible_fields, not hidden_fields
     # despite the underlying input being type="hidden"
     is_hidden = False
 
@@ -79,15 +56,15 @@
         return self.model.objects.get(pk=value)
 
     def get_create_item_url(self):
         if self.create_item_url_name is None:
             return None
         else:
             return reverse(self.create_item_url_name)
-    
+
     def get_edit_item_url(self, instance):
         if self.edit_item_url_name is None:
             return None
         else:
             return reverse(self.edit_item_url_name, args=(quote(instance.pk),))
 
     def get_choose_modal_url(self):
@@ -139,20 +116,15 @@
             }
 
     def render_input_html(self, name, value, attrs):
         # render the HTML for just the (hidden) input field
         return super().render_html(name, value, attrs)
 
     def render_html(self, name, value, attrs):
-        if WAGTAIL_VERSION >= (2, 12):
-            # From Wagtail 2.12, get_value_data is called as a preprocessing step in
-            # WidgetWithScript before invoking render_html
-            value_data = value
-        else:
-            value_data = self.get_value_data(value)
+        value_data = value
 
         original_field_html = self.render_input_html(name, value_data['value'], attrs)
 
         return render_to_string(self.template, {
             'widget': self,
             'original_field_html': original_field_html,
             'attrs': attrs,
@@ -190,52 +162,39 @@
         if 'link_to_chosen_text' in kwargs:
             self.link_to_chosen_text = kwargs.pop('link_to_chosen_text')
         if 'show_edit_link' in kwargs:
             self.show_edit_link = kwargs.pop('show_edit_link')
         super().__init__(**kwargs)
 
     class Media:
-        if WAGTAIL_VERSION >= (3, 0):
-            js = [
-                'generic_chooser/js/tabs.js',
-                'generic_chooser/js/chooser-modal.js',
-                'generic_chooser/js/chooser-widget.js',
-            ]
-        else:
-            js = [
-                'generic_chooser/js/chooser-modal.js',
-                'generic_chooser/js/chooser-widget.js',
-            ]
+        js = [
+            'generic_chooser/js/tabs.js',
+            'generic_chooser/js/chooser-modal.js',
+            'generic_chooser/js/chooser-widget.js',
+        ]
 
 
 class AdminChooserAdapter(WidgetAdapter):
     js_constructor = 'wagtail_generic_chooser.widgets.Chooser'
 
     def js_args(self, widget):
         return [
             widget.render_html(
                 "__NAME__", widget.get_value_data(None), attrs={"id": "__ID__"}
             ),
             widget.js_opts(),
         ]
 
     class Media:
-        if WAGTAIL_VERSION >= (3, 0):
-            js = [
-                'generic_chooser/js/tabs.js',
-                'generic_chooser/js/chooser-modal.js',
-                "generic_chooser/js/chooser-widget.js",
-                "generic_chooser/js/chooser-widget-telepath.js",
-            ]
-        else:
-            js = [
-                'generic_chooser/js/chooser-modal.js',
-                "generic_chooser/js/chooser-widget.js",
-                "generic_chooser/js/chooser-widget-telepath.js",
-            ]
+        js = [
+            'generic_chooser/js/tabs.js',
+            'generic_chooser/js/chooser-modal.js',
+            "generic_chooser/js/chooser-widget.js",
+            "generic_chooser/js/chooser-widget-telepath.js",
+        ]
 
 
 register(AdminChooserAdapter(), AdminChooser)
 
 
 class DRFChooser(AdminChooser):
     """A chooser widget associated with a Django REST Framework API endpoint"""
@@ -277,40 +236,27 @@
     def js_opts(self):
         opts = super().js_opts()
         opts.update({'linkedFields': self.linked_fields})
         return opts
 
     @property
     def media(self):
-        if WAGTAIL_VERSION >= (3, 0):
-            return super().media + Media(js=[
-                'generic_chooser/js/tabs.js',
-                'generic_chooser/js/chooser-widget.js',
-                'generic_chooser/js/linked-field-chooser-widget.js',
-            ])
-        else:
-            return super().media + Media(js=[
-                'generic_chooser/js/chooser-widget.js',
-                'generic_chooser/js/linked-field-chooser-widget.js',
-            ])
+        return super().media + Media(js=[
+            'generic_chooser/js/tabs.js',
+            'generic_chooser/js/chooser-widget.js',
+            'generic_chooser/js/linked-field-chooser-widget.js',
+        ])
 
 
 class LinkedFieldChooserAdapter(AdminChooserAdapter):
     js_constructor = 'wagtail_generic_chooser.widgets.LinkedFieldChooser'
 
     class Media:
-        if WAGTAIL_VERSION >= (3, 0):
-            js = [
-                'generic_chooser/js/tabs.js',
-                'generic_chooser/js/chooser-widget.js',
-                "generic_chooser/js/linked-field-chooser-widget.js",
-                "generic_chooser/js/linked-field-chooser-widget-telepath.js",
-            ]
-        else:
-            js = [
-                'generic_chooser/js/chooser-widget.js',
-                "generic_chooser/js/linked-field-chooser-widget.js",
-                "generic_chooser/js/linked-field-chooser-widget-telepath.js",
-            ]
+        js = [
+            'generic_chooser/js/tabs.js',
+            'generic_chooser/js/chooser-widget.js',
+            "generic_chooser/js/linked-field-chooser-widget.js",
+            "generic_chooser/js/linked-field-chooser-widget-telepath.js",
+        ]
 
 
 register(LinkedFieldChooserAdapter(), LinkedFieldMixin)
```

### Comparing `wagtail-generic-chooser-0.5.1/setup.py` & `wagtail-generic-chooser-0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='wagtail-generic-chooser',
-    version='0.5.1',
+    version='0.6',
     description="A toolkit for custom chooser popups in Wagtail",
     author='Matthew Westcott',
     author_email='matthew.westcott@torchbox.com',
     url='https://github.com/wagtail/wagtail-generic-chooser',
     packages=find_packages(exclude=("tests", "tests.*")),
     include_package_data=True,
     install_requires=[
@@ -23,18 +23,21 @@
         'Development Status :: 4 - Beta',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Framework :: Django',
+        'Framework :: Django :: 3',
+        'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Framework :: Wagtail',
-        'Framework :: Wagtail :: 2',
-        'Framework :: Wagtail :: 3',
         'Framework :: Wagtail :: 4',
+        'Framework :: Wagtail :: 5',
     ],
 )
```

### Comparing `wagtail-generic-chooser-0.5.1/wagtail_generic_chooser.egg-info/SOURCES.txt` & `wagtail-generic-chooser-0.6/wagtail_generic_chooser.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -15,13 +15,12 @@
 generic_chooser/templates/generic_chooser/_ajax_pagination_nav.html
 generic_chooser/templates/generic_chooser/_create_tab.html
 generic_chooser/templates/generic_chooser/_listing_tab.html
 generic_chooser/templates/generic_chooser/_results.html
 generic_chooser/templates/generic_chooser/tabbed_modal.html
 generic_chooser/templates/generic_chooser/tabbed_modal_v3.html
 generic_chooser/templates/generic_chooser/widgets/chooser.html
-generic_chooser/templates/generic_chooser/widgets/chooser_v4.html
 wagtail_generic_chooser.egg-info/PKG-INFO
 wagtail_generic_chooser.egg-info/SOURCES.txt
 wagtail_generic_chooser.egg-info/dependency_links.txt
 wagtail_generic_chooser.egg-info/requires.txt
 wagtail_generic_chooser.egg-info/top_level.txt
```


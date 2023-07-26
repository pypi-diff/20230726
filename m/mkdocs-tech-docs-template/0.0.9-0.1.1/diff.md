# Comparing `tmp/mkdocs-tech-docs-template-0.0.9.tar.gz` & `tmp/mkdocs-tech-docs-template-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-tech-docs-template-0.0.9.tar", last modified: Sun Jan 22 11:58:43 2023, max compression
+gzip compressed data, was "mkdocs-tech-docs-template-0.1.1.tar", last modified: Wed Jul 26 13:06:36 2023, max compression
```

## Comparing `mkdocs-tech-docs-template-0.0.9.tar` & `mkdocs-tech-docs-template-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,31 @@
-drwxr-xr-x   0 soumaya.mauthoor   (502) staff       (20)        0 2023-01-22 11:58:43.221674 mkdocs-tech-docs-template-0.0.9/
--rw-r--r--   0 soumaya.mauthoor   (502) staff       (20)     4237 2023-01-22 11:58:43.221740 mkdocs-tech-docs-template-0.0.9/PKG-INFO
-drwxr-xr-x   0 soumaya.mauthoor   (502) staff       (20)        0 2023-01-22 11:58:43.219942 mkdocs-tech-docs-template-0.0.9/docs/
--rw-r--r--   0 soumaya.mauthoor   (502) staff       (20)     3675 2023-01-22 11:54:08.000000 mkdocs-tech-docs-template-0.0.9/docs/README.md
-drwxr-xr-x   0 soumaya.mauthoor   (502) staff       (20)        0 2023-01-22 11:58:43.221163 mkdocs-tech-docs-template-0.0.9/mkdocs_tech_docs_template.egg-info/
--rw-r--r--   0 soumaya.mauthoor   (502) staff       (20)     4237 2023-01-22 11:58:43.000000 mkdocs-tech-docs-template-0.0.9/mkdocs_tech_docs_template.egg-info/PKG-INFO
--rw-r--r--   0 soumaya.mauthoor   (502) staff       (20)      479 2023-01-22 11:58:43.000000 mkdocs-tech-docs-template-0.0.9/mkdocs_tech_docs_template.egg-info/SOURCES.txt
--rw-r--r--   0 soumaya.mauthoor   (502) staff       (20)        1 2023-01-22 11:58:43.000000 mkdocs-tech-docs-template-0.0.9/mkdocs_tech_docs_template.egg-info/dependency_links.txt
--rw-r--r--   0 soumaya.mauthoor   (502) staff       (20)       56 2023-01-22 11:58:43.000000 mkdocs-tech-docs-template-0.0.9/mkdocs_tech_docs_template.egg-info/entry_points.txt
--rw-r--r--   0 soumaya.mauthoor   (502) staff       (20)        1 2023-01-21 13:03:18.000000 mkdocs-tech-docs-template-0.0.9/mkdocs_tech_docs_template.egg-info/not-zip-safe
--rw-r--r--   0 soumaya.mauthoor   (502) staff       (20)       90 2023-01-22 11:58:43.000000 mkdocs-tech-docs-template-0.0.9/mkdocs_tech_docs_template.egg-info/requires.txt
--rw-r--r--   0 soumaya.mauthoor   (502) staff       (20)       19 2023-01-22 11:58:43.000000 mkdocs-tech-docs-template-0.0.9/mkdocs_tech_docs_template.egg-info/top_level.txt
--rw-r--r--   0 soumaya.mauthoor   (502) staff       (20)       81 2023-01-22 11:54:08.000000 mkdocs-tech-docs-template-0.0.9/pyproject.toml
--rw-r--r--   0 soumaya.mauthoor   (502) staff       (20)     1012 2023-01-22 11:58:43.222070 mkdocs-tech-docs-template-0.0.9/setup.cfg
-drwxr-xr-x   0 soumaya.mauthoor   (502) staff       (20)        0 2023-01-22 11:58:43.221570 mkdocs-tech-docs-template-0.0.9/tech_docs_template/
--rw-r--r--   0 soumaya.mauthoor   (502) staff       (20)       22 2023-01-22 11:58:25.000000 mkdocs-tech-docs-template-0.0.9/tech_docs_template/__init__.py
--rw-r--r--   0 soumaya.mauthoor   (502) staff       (20)     1085 2023-01-22 11:54:08.000000 mkdocs-tech-docs-template-0.0.9/tech_docs_template/main.html
--rw-r--r--   0 soumaya.mauthoor   (502) staff       (20)       81 2023-01-22 11:54:08.000000 mkdocs-tech-docs-template-0.0.9/tech_docs_template/mkdocs_theme.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.411674 mkdocs-tech-docs-template-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-26 13:06:36.000000 mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-26 13:06:36.000000 mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:06:36.000000 mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 13:06:36.000000 mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:06:36.000000 mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-26 13:06:36.000000 mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 13:06:36.000000 mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/tech_docs_template/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.411674 mkdocs-tech-docs-template-0.1.1/tech_docs_template/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/tech_docs_template/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/assets/images/govuk-crest-2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/assets/images/ogl.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/tech_docs_template/assets/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/assets/stylesheets/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/tech_docs_template/favicons/
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/favicons/dbt.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/favicons/moj.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/tech_docs_template/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/logos/dbt.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/logos/moj.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/mkdocs_theme.yml
```

### Comparing `mkdocs-tech-docs-template-0.0.9/setup.cfg` & `mkdocs-tech-docs-template-0.1.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -15,29 +15,32 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 zip_safe = False
 install_requires = 
-	mkdocs-material
-	mkdocs-git-revision-date-localized-plugin
+	mkdocs-material >= 9.2
 
 [options.entry_points]
 mkdocs.themes = 
 	tech_docs_template = tech_docs_template
 
 [options.extras_require]
 docs = 
 	markdown-include
 	mkdocs
 
 [options.package_data]
 tech_docs_template = 
 	*.html
 	mkdocs_theme.yml
-	assets/*
+	assets/images/*
+	assets/stylesheets/*
+	favicons/*
+	logos/*
+	partials/*
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mkdocs-tech-docs-template-0.0.9/tech_docs_template/main.html` & `mkdocs-tech-docs-template-0.1.1/tech_docs_template/main.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 {% extends "base.html" %}
 
+{# append our extra stylesheets#}
 {% block styles %}
   {{ super() }}
-  {# append our extra stylesheets to the styles from mkdocs-material #}
   <link rel="stylesheet" href="{{ 'assets/stylesheets/extra.css' | url }}">
 {% endblock %}
 
 {% block footer %}
   <footer class="md-footer">
     <div class="md-footer-meta__inner md-grid">
 
       <div class="md-copyright">
-        <img src="assets/images/ogl.png" >
+
+        {% if config.extra.social %}
+          {% include "partials/social.html" %}
+        {% endif %}
+
+        Made with 
+        <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">
+          Material for MkDocs
+        </a>
+        <br><br>
+        <img src="{{ 'assets/images/ogl.png' |url }}" >
         All content is available under the 
         <a
             href="https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/"
             target="_blank" rel="noopener"
         >
             Open Government Licence v3.0</a>
         , except where otherwise stated
       </div>
 
-      <div>
-        <img class="logo" src="assets/images/govuk-crest-2x.png" width=125px height=102px;>
-        <br>
-        <a class="md-copyright" 
-        href="https://www.nationalarchives.gov.uk/information-management/re-using-public-sector-information/uk-government-licensing-framework/crown-copyright/">© Crown copyright</a>
+      <div class="md-copyright">
+        <a 
+          href="https://www.nationalarchives.gov.uk/information-management/re-using-public-sector-information/uk-government-licensing-framework/crown-copyright/"
+          target="_blank" rel="noopener">
+          <img src="{{ 'assets/images/govuk-crest-2x.png' | url }}" width=125px height=102px;>
+          <br>
+          © Crown copyright
+        </a>
       </div>
 
     </div>
   </footer>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,11 @@
-{% extends "base.html" %} {% block styles %} {{ super() }} {# append our extra
-stylesheets to the styles from mkdocs-material #}
+{% extends "base.html" %} {# append our extra stylesheets#} {% block styles %}
+{{ super() }}
  {% endblock %} {% block footer %}
-[assets/images/ogl.png] All content is available under the Open_Government
-Licence_v3.0 , except where otherwise stated
-[assets/images/govuk-crest-2x.png]
+{% if config.extra.social %} {% include "partials/social.html" %} {% endif %}
+Made with Material_for_MkDocs
+
+[{{ 'assets/images/ogl.png' |url }}] All content is available under the Open
+Government_Licence_v3.0 , except where otherwise stated
+[{{_'assets/images/govuk-crest-2x.png'_|_url_}}]_
 Â©_Crown_copyright
  {% endblock %}
```


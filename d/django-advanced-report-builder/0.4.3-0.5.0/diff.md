# Comparing `tmp/django-advanced-report-builder-0.4.3.tar.gz` & `tmp/django-advanced-report-builder-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-advanced-report-builder-0.4.3.tar", last modified: Tue Jul 25 15:51:07 2023, max compression
+gzip compressed data, was "django-advanced-report-builder-0.5.0.tar", last modified: Wed Jul 26 15:48:58 2023, max compression
```

## Comparing `django-advanced-report-builder-0.4.3.tar` & `django-advanced-report-builder-0.5.0.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.180941 django-advanced-report-builder-0.4.3/
--rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       91 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)      683 2023-07-25 15:51:07.180808 django-advanced-report-builder-0.4.3/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      171 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.149049 django-advanced-report-builder-0.4.3/advanced_report_builder/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     4012 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/admin.py
--rw-r--r--   0 tom        (501) staff       (20)      218 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/apps.py
--rw-r--r--   0 tom        (501) staff       (20)     3394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/columns.py
--rw-r--r--   0 tom        (501) staff       (20)       40 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/customise.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.149579 django-advanced-report-builder-0.4.3/advanced_report_builder/data_merge/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/data_merge/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3830 2023-03-06 12:34:46.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/data_merge/utils.py
--rw-r--r--   0 tom        (501) staff       (20)      951 2023-03-29 16:03:43.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/data_merge/widget.py
--rw-r--r--   0 tom        (501) staff       (20)     5477 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/duplicate.py
--rw-r--r--   0 tom        (501) staff       (20)      192 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/exceptions.py
--rw-r--r--   0 tom        (501) staff       (20)    10853 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/field_types.py
--rw-r--r--   0 tom        (501) staff       (20)    13799 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/filter_query.py
--rw-r--r--   0 tom        (501) staff       (20)      439 2023-06-21 09:07:31.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/generate_series.py
--rw-r--r--   0 tom        (501) staff       (20)     8337 2023-06-21 09:29:22.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/globals.py
--rw-r--r--   0 tom        (501) staff       (20)     1308 2023-04-17 09:39:11.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/includes.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.151685 django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/
--rw-r--r--   0 tom        (501) staff       (20)    14109 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)      591 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0002_auto_20220209_1657.py
--rw-r--r--   0 tom        (501) staff       (20)     1734 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0003_auto_20220215_1219.py
--rw-r--r--   0 tom        (501) staff       (20)      955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0004_customreport.py
--rw-r--r--   0 tom        (501) staff       (20)     3623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0005_auto_20220303_0958.py
--rw-r--r--   0 tom        (501) staff       (20)      914 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0006_auto_20220310_1147.py
--rw-r--r--   0 tom        (501) staff       (20)      607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0007_auto_20220322_1939.py
--rw-r--r--   0 tom        (501) staff       (20)      827 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0008_auto_20220404_1144.py
--rw-r--r--   0 tom        (501) staff       (20)     2485 2023-04-28 15:54:41.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0009_auto_20230428_1554.py
--rw-r--r--   0 tom        (501) staff       (20)      596 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0010_auto_20230428_2033.py
--rw-r--r--   0 tom        (501) staff       (20)      659 2023-06-20 14:49:09.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0011_auto_20230620_1449.py
--rw-r--r--   0 tom        (501) staff       (20)      767 2023-07-18 16:42:15.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0012_auto_20230718_1642.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    19894 2023-07-18 16:42:07.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/models.py
--rw-r--r--   0 tom        (501) staff       (20)      532 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/report_builder.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.142510 django-advanced-report-builder-0.4.3/advanced_report_builder/static/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.143329 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.142594 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/chart-js/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.154057 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/chart-js/js/
--rw-r--r--   0 tom        (501) staff       (20)   334540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js
--rw-r--r--   0 tom        (501) staff       (20)   405847 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js
--rw-r--r--   0 tom        (501) staff       (20)   193925 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js
--rw-r--r--   0 tom        (501) staff       (20)     1430 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js
--rw-r--r--   0 tom        (501) staff       (20)    12893 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.154234 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/
--rw-r--r--   0 tom        (501) staff       (20)    72125 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js
--rw-r--r--   0 tom        (501) staff       (20)     2352 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.142873 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/d3/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.156074 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/d3/js/
--rw-r--r--   0 tom        (501) staff       (20)   575002 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js
--rw-r--r--   0 tom        (501) staff       (20)   275533 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.142769 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/d3-funnel/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.154830 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/
--rw-r--r--   0 tom        (501) staff       (20)   205600 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js
--rw-r--r--   0 tom        (501) staff       (20)    58945 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.142981 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dashboard/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.156724 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dashboard/js/
--rw-r--r--   0 tom        (501) staff       (20)      563 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.143087 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.158078 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/
--rwxr-xr-x   0 tom        (501) staff       (20)      578 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore
--rwxr-xr-x   0 tom        (501) staff       (20)      122 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/.travis.yml
--rwxr-xr-x   0 tom        (501) staff       (20)     1176 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt
--rwxr-xr-x   0 tom        (501) staff       (20)     3291 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.158220 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/bin/
--rwxr-xr-x   0 tom        (501) staff       (20)     1442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer
--rwxr-xr-x   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/bower.json
--rwxr-xr-x   0 tom        (501) staff       (20)     5175 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3374 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1758 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js
--rwxr-xr-x   0 tom        (501) staff       (20)     5190 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/index.js
--rwxr-xr-x   0 tom        (501) staff       (20)      920 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/package.json
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.143265 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/jquery_extendext/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.158504 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/
--rwxr-xr-x   0 tom        (501) staff       (20)     4390 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1324 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.143677 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.159059 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/css/
--rwxr-xr-x   0 tom        (501) staff       (20)     3765 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css
--rwxr-xr-x   0 tom        (501) staff       (20)     3253 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css
--rwxr-xr-x   0 tom        (501) staff       (20)     3756 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css
--rwxr-xr-x   0 tom        (501) staff       (20)     3248 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.163941 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/
--rwxr-xr-x   0 tom        (501) staff       (20)     2962 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3082 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2494 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1431 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2309 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3273 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2672 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2662 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3216 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2917 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2952 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2522 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2299 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1412 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2645 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2787 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2451 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1310 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2627 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2782 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3062 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2503 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.166231 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/js/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.143605 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.166518 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/
--rwxr-xr-x   0 tom        (501) staff       (20)     1212 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js
--rwxr-xr-x   0 tom        (501) staff       (20)   191499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js
--rwxr-xr-x   0 tom        (501) staff       (20)    72607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js
--rwxr-xr-x   0 tom        (501) staff       (20)   201158 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js
--rwxr-xr-x   0 tom        (501) staff       (20)    77072 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.166841 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/scss/
--rwxr-xr-x   0 tom        (501) staff       (20)      442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/scss/dark.scss
--rwxr-xr-x   0 tom        (501) staff       (20)     3887 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.168471 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/
--rwxr-xr-x   0 tom        (501) staff       (20)      266 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-checkbox.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-tooltip-errors.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss
--rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_invert.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      469 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_sortable.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/bt-tooltip-errors.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss
--rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/invert.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      465 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/sortable.scss
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.143926 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.168933 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.169571 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.169735 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/bar/
--rw-r--r--   0 tom        (501) staff       (20)     5295 2023-06-21 09:32:32.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.170193 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/funnel/
--rw-r--r--   0 tom        (501) staff       (20)     1362 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html
--rw-r--r--   0 tom        (501) staff       (20)     1007 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.170383 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/line/
--rw-r--r--   0 tom        (501) staff       (20)     4020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      486 2023-04-26 11:14:19.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/modal.html
--rw-r--r--   0 tom        (501) staff       (20)      270 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/modal_field.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.170566 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/pie/
--rw-r--r--   0 tom        (501) staff       (20)     2084 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      858 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/report.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.170733 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/data_merge/
--rw-r--r--   0 tom        (501) staff       (20)     2975 2023-03-29 15:59:37.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.171818 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/datatables/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.172164 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/datatables/fields/
--rw-r--r--   0 tom        (501) staff       (20)      254 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/datatables/fields/modal.html
--rw-r--r--   0 tom        (501) staff       (20)     3320 2023-04-26 11:10:44.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html
--rw-r--r--   0 tom        (501) staff       (20)      377 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/datatables/modal.html
--rw-r--r--   0 tom        (501) staff       (20)      593 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html
--rw-r--r--   0 tom        (501) staff       (20)      256 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/datatables/query_modal.html
--rw-r--r--   0 tom        (501) staff       (20)     1127 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/datatables/report.html
--rw-r--r--   0 tom        (501) staff       (20)     8458 2023-07-25 15:45:22.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.173261 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/kanban/
--rw-r--r--   0 tom        (501) staff       (20)      499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/kanban/description_modal.html
--rw-r--r--   0 tom        (501) staff       (20)     2038 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      308 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/kanban/modal.html
--rw-r--r--   0 tom        (501) staff       (20)     1961 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/kanban/report.html
--rw-r--r--   0 tom        (501) staff       (20)     3467 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/query_builder.html
--rw-r--r--   0 tom        (501) staff       (20)    11119 2023-07-25 15:45:22.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/select_column.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.173792 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/single_values/
--rw-r--r--   0 tom        (501) staff       (20)     1896 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html
--rw-r--r--   0 tom        (501) staff       (20)     1643 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/single_values/report.html
--rw-r--r--   0 tom        (501) staff       (20)      327 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/toggle.py
--rw-r--r--   0 tom        (501) staff       (20)     4223 2023-06-07 08:15:03.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/urls.py
--rw-r--r--   0 tom        (501) staff       (20)     4446 2023-06-21 08:33:34.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/utils.py
--rw-r--r--   0 tom        (501) staff       (20)    12521 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/variable_date.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.178145 django-advanced-report-builder-0.4.3/advanced_report_builder/views/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    25874 2023-06-21 09:37:24.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/bar_charts.py
--rw-r--r--   0 tom        (501) staff       (20)    18240 2023-04-28 15:13:27.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/charts_base.py
--rw-r--r--   0 tom        (501) staff       (20)     3020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/custom.py
--rw-r--r--   0 tom        (501) staff       (20)     8659 2023-07-25 11:25:17.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/dashboard.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.179205 django-advanced-report-builder-0.4.3/advanced_report_builder/views/datatables/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/datatables/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     6801 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/datatables/datatables.py
--rw-r--r--   0 tom        (501) staff       (20)    25731 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/datatables/modal.py
--rw-r--r--   0 tom        (501) staff       (20)    11394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/datatables/utils.py
--rw-r--r--   0 tom        (501) staff       (20)     8792 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/funnel_charts.py
--rw-r--r--   0 tom        (501) staff       (20)    32161 2023-03-29 16:04:49.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/kanban.py
--rw-r--r--   0 tom        (501) staff       (20)    13046 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/line_charts.py
--rw-r--r--   0 tom        (501) staff       (20)    21031 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/modals_base.py
--rw-r--r--   0 tom        (501) staff       (20)     8753 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/pie_charts.py
--rw-r--r--   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/report.py
--rw-r--r--   0 tom        (501) staff       (20)     8210 2023-04-28 13:58:37.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/report_utils_mixin.py
--rw-r--r--   0 tom        (501) staff       (20)     5048 2023-07-25 11:32:22.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/reports.py
--rw-r--r--   0 tom        (501) staff       (20)    22873 2023-07-18 16:39:40.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/single_values.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.179788 django-advanced-report-builder-0.4.3/advanced_report_builder/views/targets/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/targets/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3021 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/targets/utils.py
--rw-r--r--   0 tom        (501) staff       (20)      786 2023-07-18 16:39:39.000000 django-advanced-report-builder-0.4.3/advanced_report_builder/views/targets/views.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-25 15:51:07.180628 django-advanced-report-builder-0.4.3/django_advanced_report_builder.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)      683 2023-07-25 15:51:07.000000 django-advanced-report-builder-0.4.3/django_advanced_report_builder.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)    11125 2023-07-25 15:51:07.000000 django-advanced-report-builder-0.4.3/django_advanced_report_builder.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-07-25 15:51:07.000000 django-advanced-report-builder-0.4.3/django_advanced_report_builder.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)      149 2023-07-25 15:51:07.000000 django-advanced-report-builder-0.4.3/django_advanced_report_builder.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       24 2023-07-25 15:51:07.000000 django-advanced-report-builder-0.4.3/django_advanced_report_builder.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-07-25 15:51:07.180984 django-advanced-report-builder-0.4.3/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      974 2023-07-25 15:50:41.000000 django-advanced-report-builder-0.4.3/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.584769 django-advanced-report-builder-0.5.0/
+-rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       91 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)      683 2023-07-26 15:48:58.584631 django-advanced-report-builder-0.5.0/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      171 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.552193 django-advanced-report-builder-0.5.0/advanced_report_builder/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     4012 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/admin.py
+-rw-r--r--   0 tom        (501) staff       (20)      218 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/apps.py
+-rw-r--r--   0 tom        (501) staff       (20)     3394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/columns.py
+-rw-r--r--   0 tom        (501) staff       (20)       40 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/customise.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.552728 django-advanced-report-builder-0.5.0/advanced_report_builder/data_merge/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/data_merge/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3948 2023-07-26 15:43:24.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/data_merge/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)      951 2023-03-29 16:03:43.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/data_merge/widget.py
+-rw-r--r--   0 tom        (501) staff       (20)     5477 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/duplicate.py
+-rw-r--r--   0 tom        (501) staff       (20)      192 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/exceptions.py
+-rw-r--r--   0 tom        (501) staff       (20)    10853 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/field_types.py
+-rw-r--r--   0 tom        (501) staff       (20)    14149 2023-07-26 15:43:24.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/filter_query.py
+-rw-r--r--   0 tom        (501) staff       (20)      439 2023-06-21 09:07:31.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/generate_series.py
+-rw-r--r--   0 tom        (501) staff       (20)     8337 2023-06-21 09:29:22.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/globals.py
+-rw-r--r--   0 tom        (501) staff       (20)     1308 2023-04-17 09:39:11.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/includes.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.555504 django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)    14109 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)      591 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0002_auto_20220209_1657.py
+-rw-r--r--   0 tom        (501) staff       (20)     1734 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0003_auto_20220215_1219.py
+-rw-r--r--   0 tom        (501) staff       (20)      955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0004_customreport.py
+-rw-r--r--   0 tom        (501) staff       (20)     3623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0005_auto_20220303_0958.py
+-rw-r--r--   0 tom        (501) staff       (20)      914 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0006_auto_20220310_1147.py
+-rw-r--r--   0 tom        (501) staff       (20)      607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0007_auto_20220322_1939.py
+-rw-r--r--   0 tom        (501) staff       (20)      827 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0008_auto_20220404_1144.py
+-rw-r--r--   0 tom        (501) staff       (20)     2485 2023-04-28 15:54:41.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0009_auto_20230428_1554.py
+-rw-r--r--   0 tom        (501) staff       (20)      596 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0010_auto_20230428_2033.py
+-rw-r--r--   0 tom        (501) staff       (20)      659 2023-06-20 14:49:09.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0011_auto_20230620_1449.py
+-rw-r--r--   0 tom        (501) staff       (20)      767 2023-07-18 16:42:15.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0012_auto_20230718_1642.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    19894 2023-07-18 16:42:07.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/models.py
+-rw-r--r--   0 tom        (501) staff       (20)      532 2023-07-26 15:11:05.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/report_builder.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.543986 django-advanced-report-builder-0.5.0/advanced_report_builder/static/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.544933 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.544081 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/chart-js/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.558440 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/
+-rw-r--r--   0 tom        (501) staff       (20)   334540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js
+-rw-r--r--   0 tom        (501) staff       (20)   405847 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js
+-rw-r--r--   0 tom        (501) staff       (20)   193925 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js
+-rw-r--r--   0 tom        (501) staff       (20)     1430 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js
+-rw-r--r--   0 tom        (501) staff       (20)    12893 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.558605 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/
+-rw-r--r--   0 tom        (501) staff       (20)    72125 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js
+-rw-r--r--   0 tom        (501) staff       (20)     2352 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.544377 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/d3/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.560784 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/d3/js/
+-rw-r--r--   0 tom        (501) staff       (20)   575002 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js
+-rw-r--r--   0 tom        (501) staff       (20)   275533 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.544259 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.559368 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/
+-rw-r--r--   0 tom        (501) staff       (20)   205600 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js
+-rw-r--r--   0 tom        (501) staff       (20)    58945 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.544538 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dashboard/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.561617 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dashboard/js/
+-rw-r--r--   0 tom        (501) staff       (20)      563 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.544659 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.563405 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/
+-rwxr-xr-x   0 tom        (501) staff       (20)      578 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore
+-rwxr-xr-x   0 tom        (501) staff       (20)      122 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/.travis.yml
+-rwxr-xr-x   0 tom        (501) staff       (20)     1176 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt
+-rwxr-xr-x   0 tom        (501) staff       (20)     3291 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.563581 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/bin/
+-rwxr-xr-x   0 tom        (501) staff       (20)     1442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer
+-rwxr-xr-x   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/bower.json
+-rwxr-xr-x   0 tom        (501) staff       (20)     5175 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3374 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1758 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     5190 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/index.js
+-rwxr-xr-x   0 tom        (501) staff       (20)      920 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/package.json
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.544860 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.563911 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/
+-rwxr-xr-x   0 tom        (501) staff       (20)     4390 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1324 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.545448 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.564567 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/
+-rwxr-xr-x   0 tom        (501) staff       (20)     3765 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css
+-rwxr-xr-x   0 tom        (501) staff       (20)     3253 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css
+-rwxr-xr-x   0 tom        (501) staff       (20)     3756 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css
+-rwxr-xr-x   0 tom        (501) staff       (20)     3248 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.569223 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/
+-rwxr-xr-x   0 tom        (501) staff       (20)     2962 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3082 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2494 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1431 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2309 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3273 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2672 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2662 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3216 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2917 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2952 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2522 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2299 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1412 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2645 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2787 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2451 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1310 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2627 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2782 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3062 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2503 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.571266 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.545350 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.571606 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/
+-rwxr-xr-x   0 tom        (501) staff       (20)     1212 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js
+-rwxr-xr-x   0 tom        (501) staff       (20)   191499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js
+-rwxr-xr-x   0 tom        (501) staff       (20)    72607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js
+-rwxr-xr-x   0 tom        (501) staff       (20)   201158 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js
+-rwxr-xr-x   0 tom        (501) staff       (20)    77072 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.571937 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/
+-rwxr-xr-x   0 tom        (501) staff       (20)      442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/dark.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)     3887 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.573706 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/
+-rwxr-xr-x   0 tom        (501) staff       (20)      266 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-checkbox.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-tooltip-errors.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_invert.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      469 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_sortable.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/bt-tooltip-errors.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/invert.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      465 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/sortable.scss
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.545701 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.574318 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.575133 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.575319 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/bar/
+-rw-r--r--   0 tom        (501) staff       (20)     5295 2023-06-21 09:32:32.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.575845 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/
+-rw-r--r--   0 tom        (501) staff       (20)     1362 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)     1007 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.576041 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/line/
+-rw-r--r--   0 tom        (501) staff       (20)     4020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      486 2023-04-26 11:14:19.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)      270 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/modal_field.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.576329 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/pie/
+-rw-r--r--   0 tom        (501) staff       (20)     2084 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      858 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/report.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.576573 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/data_merge/
+-rw-r--r--   0 tom        (501) staff       (20)     2975 2023-03-29 15:59:37.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.577597 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/datatables/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.578037 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/datatables/fields/
+-rw-r--r--   0 tom        (501) staff       (20)      254 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/datatables/fields/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     3320 2023-04-26 11:10:44.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html
+-rw-r--r--   0 tom        (501) staff       (20)      377 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/datatables/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)      593 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html
+-rw-r--r--   0 tom        (501) staff       (20)      256 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/datatables/query_modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     1127 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/datatables/report.html
+-rw-r--r--   0 tom        (501) staff       (20)     8458 2023-07-25 15:45:22.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.579138 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/kanban/
+-rw-r--r--   0 tom        (501) staff       (20)      499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/kanban/description_modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     2038 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      308 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/kanban/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     1961 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/kanban/report.html
+-rw-r--r--   0 tom        (501) staff       (20)     3467 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/query_builder.html
+-rw-r--r--   0 tom        (501) staff       (20)    11119 2023-07-25 15:45:22.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/select_column.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.579755 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/single_values/
+-rw-r--r--   0 tom        (501) staff       (20)     1896 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     1643 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/single_values/report.html
+-rw-r--r--   0 tom        (501) staff       (20)      327 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/toggle.py
+-rw-r--r--   0 tom        (501) staff       (20)     4223 2023-06-07 08:15:03.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/urls.py
+-rw-r--r--   0 tom        (501) staff       (20)     4796 2023-07-26 15:43:24.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)    12521 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/variable_date.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.582592 django-advanced-report-builder-0.5.0/advanced_report_builder/views/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    26004 2023-07-26 15:43:24.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/bar_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)    18552 2023-07-26 15:43:24.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/charts_base.py
+-rw-r--r--   0 tom        (501) staff       (20)     3020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/custom.py
+-rw-r--r--   0 tom        (501) staff       (20)     8659 2023-07-25 11:25:17.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/dashboard.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.583191 django-advanced-report-builder-0.5.0/advanced_report_builder/views/datatables/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/datatables/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     6847 2023-07-26 15:43:24.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/datatables/datatables.py
+-rw-r--r--   0 tom        (501) staff       (20)    25823 2023-07-26 15:43:24.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/datatables/modal.py
+-rw-r--r--   0 tom        (501) staff       (20)    11394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/datatables/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     8875 2023-07-26 15:43:24.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/funnel_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)    32309 2023-07-26 15:43:24.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/kanban.py
+-rw-r--r--   0 tom        (501) staff       (20)    13127 2023-07-26 15:43:24.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/line_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)    21312 2023-07-26 15:45:30.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/modals_base.py
+-rw-r--r--   0 tom        (501) staff       (20)     8834 2023-07-26 15:43:24.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/pie_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/report.py
+-rw-r--r--   0 tom        (501) staff       (20)     8210 2023-04-28 13:58:37.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/report_utils_mixin.py
+-rw-r--r--   0 tom        (501) staff       (20)     5048 2023-07-25 11:32:22.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/reports.py
+-rw-r--r--   0 tom        (501) staff       (20)    22970 2023-07-26 15:43:24.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/single_values.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.583651 django-advanced-report-builder-0.5.0/advanced_report_builder/views/targets/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/targets/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3021 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/targets/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)      786 2023-07-18 16:39:39.000000 django-advanced-report-builder-0.5.0/advanced_report_builder/views/targets/views.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-26 15:48:58.584437 django-advanced-report-builder-0.5.0/django_advanced_report_builder.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)      683 2023-07-26 15:48:58.000000 django-advanced-report-builder-0.5.0/django_advanced_report_builder.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)    11125 2023-07-26 15:48:58.000000 django-advanced-report-builder-0.5.0/django_advanced_report_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-07-26 15:48:58.000000 django-advanced-report-builder-0.5.0/django_advanced_report_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)      149 2023-07-26 15:48:58.000000 django-advanced-report-builder-0.5.0/django_advanced_report_builder.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       24 2023-07-26 15:48:58.000000 django-advanced-report-builder-0.5.0/django_advanced_report_builder.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-07-26 15:48:58.584819 django-advanced-report-builder-0.5.0/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      974 2023-07-26 15:48:08.000000 django-advanced-report-builder-0.5.0/setup.py
```

### Comparing `django-advanced-report-builder-0.4.3/LICENSE` & `django-advanced-report-builder-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/PKG-INFO` & `django-advanced-report-builder-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-report-builder
-Version: 0.4.3
+Version: 0.5.0
 Summary: Django app that allows you to build reports from modals
 Home-page: https://github.com/django-advance-utils/django-advanced-report-builder
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/admin.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/admin.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/columns.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/columns.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/data_merge/utils.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/data_merge/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 
 from django.apps import apps
 
-from advanced_report_builder.utils import get_field_details
+from advanced_report_builder.utils import get_field_details, get_report_builder_class
 
 
 def get_menu_fields(base_model, report_builder_class,
                     menus=None, codes=None, code_prefix='', next_code_prefix='__',
                     previous_base_model=None, table=None):
 
     for report_builder_field in report_builder_class.fields:
@@ -22,15 +22,16 @@
                 codes.add(full_id)
 
     for include_field, include in report_builder_class.includes.items():
         app_label, model, report_builder_fields_str = include['model'].split('.')
 
         new_model = apps.get_model(app_label, model)
         if new_model != previous_base_model:
-            new_report_builder_class = getattr(new_model, report_builder_fields_str, None)
+            new_report_builder_class = get_report_builder_class(model=new_model,
+                                                                class_name=report_builder_fields_str)
             title = new_report_builder_class.title
             if menus is not None:
                 menu = []
             else:
                 menu = None
             get_menu_fields(base_model=new_model,
                             report_builder_class=new_report_builder_class,
```

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/data_merge/widget.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/data_merge/widget.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/duplicate.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/duplicate.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/field_types.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/field_types.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/filter_query.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/filter_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from functools import reduce
 
 from django.apps import apps
 from django.db.models import Q
 from django.shortcuts import get_object_or_404
 
 from advanced_report_builder.models import ReportQuery
+from advanced_report_builder.utils import get_report_builder_class
 from advanced_report_builder.variable_date import VariableDate
 
 
 class FilterQueryMixin:
 
     def __init__(self, *args, **kwargs):
         self.report = None
@@ -251,30 +252,34 @@
             new_field_str = '__'.join(field_parts[1:])
 
             include = report_builder_class.includes.get(include_str)
 
             if include is not None:
                 app_label, model, report_builder_fields_str = include['model'].split('.')
                 new_model = apps.get_model(app_label, model)
-                new_report_builder_fields = getattr(new_model, report_builder_fields_str, None)
+
+                new_report_builder_class = get_report_builder_class(model=new_model,
+                                                                    class_name=report_builder_fields_str)
 
                 if new_model != previous_base_model:
                     result = self._get_report_builder_class(base_model=new_model,
                                                             field_str=new_field_str,
-                                                            report_builder_class=new_report_builder_fields,
+                                                            report_builder_class=new_report_builder_class,
                                                             previous_base_model=base_model)
                     if result:
                         return result
         else:
             include = report_builder_class.includes.get(field_str)
             if include is not None:
                 app_label, model, report_builder_fields_str = include['model'].split('.')
                 new_model = apps.get_model(app_label, model)
-                new_report_builder_fields = getattr(new_model, report_builder_fields_str, None)
-                return new_report_builder_fields
+                new_report_builder_class = get_report_builder_class(model=new_model,
+                                                                    class_name=report_builder_fields_str)
+
+                return new_report_builder_class
         return None
 
     def _get_pivot_details(self, base_model, pivot_str, report_builder_class, previous_base_model=None, include_str=''):
 
         if pivot_str in report_builder_class.pivot_fields:
             pivot_data = report_builder_class.pivot_fields[pivot_str]
             if include_str == '':
@@ -290,20 +295,20 @@
             include_str = pivot_parts[0]
             new_pivot_str = '__'.join(pivot_parts[1:])
 
             include = report_builder_class.includes.get(include_str)
             if include is not None:
                 app_label, model, report_builder_fields_str = include['model'].split('.')
                 new_model = apps.get_model(app_label, model)
-                new_report_builder_fields = getattr(new_model, report_builder_fields_str, None)
-
+                new_report_builder_class = get_report_builder_class(model=new_model,
+                                                                    class_name=report_builder_fields_str)
                 if new_model != previous_base_model:
                     result = self._get_pivot_details(base_model=new_model,
                                                      pivot_str=new_pivot_str,
-                                                     report_builder_class=new_report_builder_fields,
+                                                     report_builder_class=new_report_builder_class,
                                                      previous_base_model=base_model,
                                                      include_str=include_str)
                     if result:
                         return result
         return None
 
     def get_financial_month(self):
```

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/globals.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/globals.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/includes.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/includes.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0001_initial.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0002_auto_20220209_1657.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0002_auto_20220209_1657.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0003_auto_20220215_1219.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0003_auto_20220215_1219.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0004_customreport.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0004_customreport.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0005_auto_20220303_0958.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0005_auto_20220303_0958.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0006_auto_20220310_1147.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0006_auto_20220310_1147.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0007_auto_20220322_1939.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0007_auto_20220322_1939.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0008_auto_20220404_1144.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0008_auto_20220404_1144.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0009_auto_20230428_1554.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0009_auto_20230428_1554.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0010_auto_20230428_2033.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0010_auto_20230428_2033.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0011_auto_20230620_1449.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0011_auto_20230620_1449.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/migrations/0012_auto_20230718_1642.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/migrations/0012_auto_20230718_1642.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/models.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/models.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/report_builder.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/report_builder.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/README.md` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/README.md`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/index.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/index.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/dot/js/package.json` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/dot/js/package.json`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss` & `django-advanced-report-builder-0.5.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/charts/report.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/charts/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/datatables/report.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/datatables/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/kanban/report.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/kanban/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/query_builder.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/query_builder.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/select_column.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/select_column.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/templates/advanced_report_builder/single_values/report.html` & `django-advanced-report-builder-0.5.0/advanced_report_builder/templates/advanced_report_builder/single_values/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/urls.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/urls.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/utils.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -113,7 +113,19 @@
     return _data.replace('-', '@')
 
 
 def decode_attribute(data_attr):
     data_attr = data_attr.replace('@', '-')
     _data = base64.urlsafe_b64decode(data_attr)
     return _data.decode('utf-8', 'ignore')
+
+
+def get_report_builder_class(model, report_type=None, class_name=None):
+    if class_name is None:
+        class_name = report_type.report_builder_class_name
+
+    report_builder_class = getattr(model, class_name, None)
+    if report_builder_class is not None:
+        report_builder_class = report_builder_class()
+    return report_builder_class
+
+
```

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/variable_date.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/variable_date.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/views/bar_charts.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/views/bar_charts.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 from advanced_report_builder.generate_series import GenerateSeries
 from advanced_report_builder.globals import DEFAULT_DATE_FORMAT, \
     DATE_FORMAT_TYPES_DJANGO_FORMAT, NUMBER_FIELDS, ANNOTATION_VALUE_YEAR, ANNOTATION_VALUE_QUARTER, \
     ANNOTATION_VALUE_MONTH, ANNOTATION_VALUE_WEEK, ANNOTATION_VALUE_DAY, ANNOTATION_VALUE_FUNCTIONS, \
     GENERATE_SERIES_INTERVALS
 from advanced_report_builder.models import BarChartReport, ReportType
 from advanced_report_builder.toggle import RBToggle
-from advanced_report_builder.utils import split_attr, encode_attribute, decode_attribute, get_field_details
+from advanced_report_builder.utils import split_attr, encode_attribute, decode_attribute, get_field_details, \
+    get_report_builder_class
 from advanced_report_builder.views.charts_base import ChartBaseView, ChartBaseFieldForm
 from advanced_report_builder.views.datatables.modal import TableFieldModal, TableFieldForm
 from advanced_report_builder.views.datatables.utils import TableUtilsMixin
 from advanced_report_builder.views.modals_base import QueryBuilderModalBaseMixin, QueryBuilderModalBase
 
 
 class BarChartView(ChartBaseView):
@@ -92,16 +93,18 @@
             return super().get_date_field(index=index, fields=fields, base_model=base_model, table=table)
 
         start_field_name = self.chart_report.date_field
         end_field_name = self.chart_report.end_date_field
 
         if start_field_name is None or end_field_name is None:
             return
-        report_builder_class = getattr(base_model,
-                                       self.chart_report.report_type.report_builder_class_name, None)
+
+        report_builder_class = get_report_builder_class(model=base_model,
+                                                        report_type=self.chart_report.report_type)
+
         start_django_field, start_col_type_override, _, _ = get_field_details(base_model=base_model,
                                                                               field=start_field_name,
                                                                               report_builder_class=report_builder_class,
                                                                               table=table)
         if start_col_type_override:
             start_field_name = start_col_type_override.field
 
@@ -298,18 +301,20 @@
         if data_attr.get('has_filter') == '1':
             self.fields['has_filter'].initial = True
             if 'filter' in data_attr:
                 self.fields['filter'].initial = decode_attribute(data_attr['filter'])
 
         self.fields['multiple_columns'] = BooleanField(required=False, widget=RBToggle())
 
-        report_builder_fields = getattr(base_model, report_type.report_builder_class_name, None)
+        report_builder_class = get_report_builder_class(model=base_model,
+                                                        report_type=report_type)
+
         fields = []
         self._get_query_builder_foreign_key_fields(base_model=base_model,
-                                                   report_builder_fields=report_builder_fields,
+                                                   report_builder_class=report_builder_class,
                                                    fields=fields)
 
         self.fields['multiple_column_field'] = ChoiceField(choices=fields, required=False)
 
         if data_attr.get('multiple_columns') == '1':
             self.fields['multiple_columns'].initial = True
             self.fields['multiple_column_field'].initial = data_attr.get('multiple_column_field')
@@ -454,17 +459,16 @@
 
     def setup_table(self):
         bar_chart_report = self.get_bar_chart_report()
         self.chart_report = bar_chart_report
         self.kwargs['enable_links'] = self.slug['enable_links'] == 'True'
         base_model = bar_chart_report.get_base_modal()
         chart_fields = bar_chart_report.fields
-
-        report_builder_class = getattr(base_model,
-                                       bar_chart_report.report_type.report_builder_class_name, None)
+        report_builder_class = get_report_builder_class(model=base_model,
+                                                        report_type=bar_chart_report.report_type)
         table = self.add_table(base_model=base_model)
 
         table_fields = bar_chart_report.breakdown_fields
         fields_used = set()
         self.process_query_results(report_builder_class=report_builder_class,
                                    table=table,
                                    base_model=base_model,
```

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/views/charts_base.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/views/charts_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from django_modals.forms import CrispyForm
 
 from advanced_report_builder.columns import ReportBuilderDateColumn
 from advanced_report_builder.exceptions import ReportError
 from advanced_report_builder.globals import NUMBER_FIELDS, ANNOTATION_VALUE_FUNCTIONS, ANNOTATION_VALUE_YEAR, \
     ANNOTATION_VALUE_QUARTER, ANNOTATION_VALUE_WEEK, ANNOTATION_VALUE_DAY, ANNOTATION_VALUE_MONTH
 from advanced_report_builder.models import ReportType
-from advanced_report_builder.utils import split_slug, get_field_details, split_attr
+from advanced_report_builder.utils import split_slug, get_field_details, split_attr, get_report_builder_class
 from advanced_report_builder.variable_date import VariableDate
 from advanced_report_builder.views.report import ReportBase
 from advanced_report_builder.views.report_utils_mixin import ReportUtilsMixin
 from advanced_report_builder.views.targets.utils import get_target_value
 
 
 class ChartJSTable(DatatableTable):
@@ -127,16 +127,17 @@
         return '%Y-%m-%d'
 
     def get_date_field(self, index, fields, base_model, table):
 
         field_name = self.chart_report.date_field
         if field_name is None:
             return
-        report_builder_class = getattr(base_model,
-                                       self.chart_report.report_type.report_builder_class_name, None)
+        report_builder_class = get_report_builder_class(model=base_model,
+                                                        report_type=self.chart_report.report_type)
+
         django_field, col_type_override, _, _ = get_field_details(base_model=base_model,
                                                                   field=field_name,
                                                                   report_builder_class=report_builder_class,
                                                                   table=table)
 
         if col_type_override:
             field_name = col_type_override.field
@@ -177,16 +178,16 @@
         else:
             table.order_by = ['id']
 
         if not self.chart_report.fields:
             return fields
         chart_fields = self.chart_report.fields
 
-        report_builder_class = getattr(base_model,
-                                       self.chart_report.report_type.report_builder_class_name, None)
+        report_builder_class = get_report_builder_class(model=base_model,
+                                                        report_type=self.chart_report.report_type)
 
         for index, table_field in enumerate(chart_fields, 1):
             field = table_field['field']
 
             django_field, col_type_override, _, _ = get_field_details(base_model=base_model,
                                                                       field=field,
                                                                       report_builder_class=report_builder_class,
@@ -355,29 +356,35 @@
         return self.button('Cancel', commands, css_class, **kwargs)
 
     def get_report_type_details(self):
         data = json.loads(base64.b64decode(self.slug['data']))
 
         report_type = get_object_or_404(ReportType, pk=self.slug['report_type_id'])
         base_model = report_type.content_type.model_class()
-        report_builder_class = getattr(base_model,
-                                       report_type.report_builder_class_name, None)
+
+        report_builder_class = get_report_builder_class(model=base_model,
+                                                        report_type=report_type)
+
         self.django_field, self.col_type_override, _, _ = get_field_details(base_model=base_model,
                                                                             field=data['field'],
                                                                             report_builder_class=report_builder_class)
 
         return report_type, base_model
 
-    def _get_query_builder_foreign_key_fields(self, base_model, report_builder_fields, fields,
+    def _get_query_builder_foreign_key_fields(self, base_model, report_builder_class, fields,
                                               prefix='', title_prefix='', previous_base_model=None):
-        for include_field, include in report_builder_fields.includes.items():
+        for include_field, include in report_builder_class.includes.items():
             app_label, model, report_builder_fields_str = include['model'].split('.')
             new_model = apps.get_model(app_label, model)
             if new_model != previous_base_model:
-                new_report_builder_fields = getattr(new_model, report_builder_fields_str, None)
+                new_report_builder_class = get_report_builder_class(model=new_model,
+                                                                    class_name=report_builder_fields_str)
+                if new_report_builder_class is not None:
+                    new_report_builder_class = new_report_builder_class()
+
                 fields.append((prefix + include_field, title_prefix + include['title']))
                 self._get_query_builder_foreign_key_fields(base_model=new_model,
-                                                           report_builder_fields=new_report_builder_fields,
+                                                           report_builder_class=new_report_builder_class,
                                                            fields=fields,
                                                            prefix=f"{prefix}{include_field}__",
                                                            title_prefix=f"{title_prefix}{include['title']} --> ",
                                                            previous_base_model=base_model)
```

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/views/custom.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/views/custom.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/views/dashboard.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/views/dashboard.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/views/datatables/datatables.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/views/datatables/datatables.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.db import ProgrammingError
 from django_datatables.datatables import DatatableView, DatatableError
 from django_datatables.helpers import row_link
 from django_menus.menu import MenuItem
 
 from advanced_report_builder.columns import ArrowColumn
 from advanced_report_builder.exceptions import ReportError
-from advanced_report_builder.utils import get_field_details, make_slug_str
+from advanced_report_builder.utils import get_field_details, make_slug_str, get_report_builder_class
 from advanced_report_builder.utils import split_slug
 from advanced_report_builder.views.datatables.utils import TableUtilsMixin
 from advanced_report_builder.views.report import ReportBase
 
 
 class TableView(ReportBase, TableUtilsMixin, DatatableView):
     template_name = 'advanced_report_builder/datatables/report.html'
@@ -44,16 +44,16 @@
 
     def setup_table(self, table):
         table.extra_filters = self.extra_filters
         base_model = self.table_report.get_base_modal()
         table_fields = self.table_report.table_fields
         pivot_fields = self.table_report.pivot_fields
         fields_used = set()
-        report_builder_class = getattr(base_model,
-                                       self.table_report.report_type.report_builder_class_name, None)
+        report_builder_class = get_report_builder_class(model=base_model,
+                                                        report_type=self.table_report.report_type)
         self.process_query_results(report_builder_class=report_builder_class,
                                    table=table,
                                    base_model=base_model,
                                    fields_used=fields_used,
                                    table_fields=table_fields,
                                    pivot_fields=pivot_fields)
```

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/views/datatables/modal.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/views/datatables/modal.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 from django_modals.widgets.select2 import Select2Multiple
 from django_modals.widgets.widgets import Toggle
 
 from advanced_report_builder.globals import DATE_FIELDS, NUMBER_FIELDS, ANNOTATION_VALUE_CHOICES, ANNOTATIONS_CHOICES, \
     DATE_FORMAT_TYPES, CURRENCY_COLUMNS, LINK_COLUMNS
 from advanced_report_builder.models import TableReport, ReportQuery, ReportType
 from advanced_report_builder.toggle import RBToggle
-from advanced_report_builder.utils import split_attr, get_field_details, encode_attribute, decode_attribute
+from advanced_report_builder.utils import split_attr, get_field_details, encode_attribute, decode_attribute, \
+    get_report_builder_class
 from advanced_report_builder.views.charts_base import ChartBaseFieldForm
 from advanced_report_builder.views.modals_base import QueryBuilderModalBaseMixin, QueryBuilderModalBase
 
 
 class TableModal(QueryBuilderModalBase):
     template_name = 'advanced_report_builder/datatables/modal.html'
     size = 'xl'
@@ -298,18 +299,19 @@
             if data_attr.get('has_filter') == '1':
                 self.fields['has_filter'].initial = True
                 if 'filter' in data_attr:
                     self.fields['filter'].initial = decode_attribute(data_attr['filter'])
 
             self.fields['multiple_columns'] = BooleanField(required=False, widget=RBToggle())
 
-            report_builder_fields = getattr(base_model, report_type.report_builder_class_name, None)
+            report_builder_class = get_report_builder_class(model=base_model,
+                                                            report_type=report_type)
             fields = []
             self._get_query_builder_foreign_key_fields(base_model=base_model,
-                                                       report_builder_fields=report_builder_fields,
+                                                       report_builder_class=report_builder_class,
                                                        fields=fields)
 
             self.fields['multiple_column_field'] = ChoiceField(choices=fields, required=False)
 
             if data_attr.get('multiple_columns') == '1':
                 self.fields['multiple_columns'].initial = True
                 self.fields['multiple_column_field'].initial = data_attr.get('multiple_column_field')
```

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/views/datatables/utils.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/views/datatables/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/views/funnel_charts.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/views/funnel_charts.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from django_modals.modals import FormModal
 from django_modals.processes import PROCESS_EDIT_DELETE, PERMISSION_OFF
 from django_modals.widgets.colour_picker import ColourPickerWidget
 from django_modals.widgets.select2 import Select2Multiple
 
 from advanced_report_builder.models import FunnelChartReport
 from advanced_report_builder.toggle import RBToggle
-from advanced_report_builder.utils import split_attr, encode_attribute, decode_attribute
+from advanced_report_builder.utils import split_attr, encode_attribute, decode_attribute, get_report_builder_class
 from advanced_report_builder.views.charts_base import ChartBaseView, ChartBaseFieldForm
 from advanced_report_builder.views.modals_base import QueryBuilderModalBaseMixin, QueryBuilderModalBase
 
 
 class FunnelChartView(ChartBaseView):
     use_annotations = False
 
@@ -106,18 +106,20 @@
         if data_attr.get('has_filter') == '1':
             self.fields['has_filter'].initial = True
             if 'filter' in data_attr:
                 self.fields['filter'].initial = decode_attribute(data_attr['filter'])
 
         self.fields['multiple_columns'] = BooleanField(required=False, widget=RBToggle())
 
-        report_builder_fields = getattr(base_model, report_type.report_builder_class_name, None)
+        report_builder_class = get_report_builder_class(model=base_model,
+                                                        report_type=report_type)
+
         fields = []
         self._get_query_builder_foreign_key_fields(base_model=base_model,
-                                                   report_builder_fields=report_builder_fields,
+                                                   report_builder_class=report_builder_class,
                                                    fields=fields)
 
         self.fields['multiple_column_field'] = ChoiceField(choices=fields, required=False)
 
         if data_attr.get('multiple_columns') == '1':
             self.fields['multiple_columns'].initial = True
             self.fields['multiple_column_field'].initial = data_attr.get('multiple_column_field')
```

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/views/kanban.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/views/kanban.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from advanced_report_builder.data_merge.utils import get_menu_fields, get_data_merge_columns
 from advanced_report_builder.data_merge.widget import DataMergeWidget
 from advanced_report_builder.filter_query import FilterQueryMixin
 from advanced_report_builder.globals import DATE_FORMAT_TYPES_DJANGO_FORMAT, DATE_FORMAT_TYPE_DD_MM_YY_SLASH, \
     DATE_FORMAT_TYPE_SHORT_WORDS_MM_YY
 from advanced_report_builder.models import KanbanReport, KanbanReportLane, ReportType, KanbanReportDescription
 from advanced_report_builder.toggle import RBToggle
-from advanced_report_builder.utils import crispy_modal_link_args, get_field_details
+from advanced_report_builder.utils import crispy_modal_link_args, get_field_details, get_report_builder_class
 from advanced_report_builder.variable_date import VariableDate
 from advanced_report_builder.views.charts_base import ChartJSTable
 from advanced_report_builder.views.modals_base import QueryBuilderModalBase
 from advanced_report_builder.views.report import ReportBase
 
 
 class DescriptionColumn(ColumnBase):
@@ -112,15 +112,16 @@
             query = query.filter(table.extra_query_filter)
         return self.view_filter(query, table)
 
     def get_lane(self, base_model, kanban_report_lane, lanes, label=None, extra_query_filter=None, multiple=False):
 
         table = self.chart_js_table(model=base_model)
 
-        report_builder_class = getattr(base_model, kanban_report_lane.report_type.report_builder_class_name, None)
+        report_builder_class = get_report_builder_class(model=base_model,
+                                                        report_type=kanban_report_lane.report_type)
         table_indexes = []
 
         if kanban_report_lane.heading_field is not None:
             table_indexes.append('heading')
             table.add_columns(kanban_report_lane.heading_field)
 
         if kanban_report_lane.background_colour_field is not None:
@@ -218,15 +219,16 @@
         context['title'] = self.get_title()
         kanban_report_lanes = self.chart_report.kanbanreportlane_set.all()
         lanes = []
         headings = []
 
         for kanban_report_lane in kanban_report_lanes:
             base_model = kanban_report_lane.get_base_modal()
-            report_builder_class = getattr(base_model, kanban_report_lane.report_type.report_builder_class_name, None)
+            report_builder_class = get_report_builder_class(model=base_model,
+                                                            report_type=kanban_report_lane.report_type)
             if kanban_report_lane.multiple_type == KanbanReportLane.MULTIPLE_TYPE_NA:
                 self.get_lane(base_model=base_model,
                               kanban_report_lane=kanban_report_lane,
                               lanes=lanes)
                 headings.append({'label': kanban_report_lane.name,
                                  'row_span': 2,
                                  'col_span': 1})
```

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/views/line_charts.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/views/line_charts.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from django_modals.widgets.select2 import Select2Multiple
 
 from advanced_report_builder.exceptions import ReportError
 from advanced_report_builder.globals import ANNOTATION_VALUE_YEAR, \
     ANNOTATION_VALUE_QUARTER, ANNOTATION_VALUE_MONTH, ANNOTATION_VALUE_WEEK, ANNOTATION_VALUE_DAY
 from advanced_report_builder.models import LineChartReport, ReportType
 from advanced_report_builder.toggle import RBToggle
-from advanced_report_builder.utils import split_attr, encode_attribute, decode_attribute
+from advanced_report_builder.utils import split_attr, encode_attribute, decode_attribute, get_report_builder_class
 from advanced_report_builder.views.charts_base import ChartBaseView, ChartJSTable, ChartBaseFieldForm
 from advanced_report_builder.views.modals_base import QueryBuilderModalBaseMixin, QueryBuilderModalBase
 
 
 class LineChartJSTable(ChartJSTable):
     def get_table_array(self, request, results):
         results = super().get_table_array(request, results)
@@ -208,19 +208,19 @@
 
         if data_attr.get('has_filter') == '1':
             self.fields['has_filter'].initial = True
             if 'filter' in data_attr:
                 self.fields['filter'].initial = decode_attribute(data_attr['filter'])
 
         self.fields['multiple_columns'] = BooleanField(required=False, widget=RBToggle())
-
-        report_builder_fields = getattr(base_model, report_type.report_builder_class_name, None)
+        report_builder_class = get_report_builder_class(model=base_model,
+                                                        report_type=report_type)
         fields = []
         self._get_query_builder_foreign_key_fields(base_model=base_model,
-                                                   report_builder_fields=report_builder_fields,
+                                                   report_builder_class=report_builder_class,
                                                    fields=fields)
 
         self.fields['multiple_column_field'] = ChoiceField(choices=fields, required=False)
 
         if data_attr.get('multiple_columns') == '1':
             self.fields['multiple_columns'].initial = True
             self.fields['multiple_column_field'].initial = data_attr.get('multiple_column_field')
```

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/views/modals_base.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/views/modals_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from django_modals.forms import ModelCrispyForm
 from django_modals.modals import ModelFormModal
 from django_modals.widgets.select2 import Select2
 
 from advanced_report_builder.field_types import FieldTypes
 from advanced_report_builder.globals import DATE_FIELDS, NUMBER_FIELDS, LINK_COLUMNS, COLOUR_COLUMNS
 from advanced_report_builder.models import ReportQuery, ReportType
-from advanced_report_builder.utils import get_field_details
+from advanced_report_builder.utils import get_field_details, get_report_builder_class
 
 
 class QueryBuilderModelForm(ModelCrispyForm):
     def submit_button(self, css_class='btn-success modal-submit', button_text='Submit', **kwargs):
         return StrictButton(button_text, onclick=f'save_modal_{ self.form_id }()', css_class=css_class, **kwargs)
 
 
@@ -28,15 +28,16 @@
     @staticmethod
     def get_report_builder_class(report_type_id):
         if not report_type_id:
             return None, None
 
         report_type = get_object_or_404(ReportType, pk=report_type_id)
         base_model = report_type.content_type.model_class()
-        report_builder_class = getattr(base_model, report_type.report_builder_class_name, None)
+        report_builder_class = get_report_builder_class(model=base_model,
+                                                        report_type=report_type)
         return report_builder_class, base_model
 
     def get_query_builder_report_type_field(self, report_type_id):
 
         report_builder_class, base_model = self.get_report_builder_class(report_type_id=report_type_id)
         if report_builder_class is None:
             # noinspection PyUnresolvedReferences
@@ -64,15 +65,16 @@
                                            field=column.column_name,
                                            title=title_prefix + column.title,
                                            column=column,
                                            prefix=prefix)
         for include_field, include in report_builder_class.includes.items():
             app_label, model, report_builder_fields_str = include['model'].split('.')
             new_model = apps.get_model(app_label, model)
-            new_report_builder_fields = getattr(new_model, report_builder_fields_str, None)
+            new_report_builder_class = get_report_builder_class(model=new_model,
+                                                                class_name=report_builder_fields_str)
 
             if new_model != previous_base_model:
                 _foreign_key = getattr(base_model, include_field, None)
 
                 if hasattr(_foreign_key, 'field'):
                     add_null_field = _foreign_key.field.null
                 else:
@@ -85,15 +87,15 @@
                 if isinstance(new_model(), AbstractUser):
                     field_types.get_abstract_user_field(query_builder_filters=query_builder_filters,
                                                         field=prefix + include_field,
                                                         title=title_prefix + include['title'])
 
                 self._get_query_builder_fields(base_model=new_model,
                                                query_builder_filters=query_builder_filters,
-                                               report_builder_class=new_report_builder_fields,
+                                               report_builder_class=new_report_builder_class,
                                                prefix=f"{prefix}{include_field}__",
                                                title_prefix=f"{include['title']} --> ",
                                                previous_base_model=base_model)
 
 
 class QueryBuilderModalBase(QueryBuilderModalBaseMixin, ModelFormModal):
     base_form = QueryBuilderModelForm
@@ -153,18 +155,18 @@
         if colour is None:
             colour = report_builder_class.colour
 
         if tables is not None:
             tables.append({'name': title,
                            'colour': colour})
 
+        report_builder_class_fields = report_builder_class.fields
+
         if extra_fields:
-            report_builder_class_fields = report_builder_class.fields + extra_fields
-        else:
-            report_builder_class_fields = report_builder_class.fields
+            report_builder_class_fields += extra_fields
 
         for report_builder_field in report_builder_class_fields:
 
             if (not isinstance(report_builder_field, str) or
                     report_builder_field not in report_builder_class.exclude_display_fields or
                     (show_order_by_fields and report_builder_field in report_builder_class.order_by_fields)):
                 django_field, col_type_override, columns, _ = get_field_details(
@@ -202,15 +204,16 @@
                                          'colour': colour})
 
         for include_field, include in report_builder_class.includes.items():
             app_label, model, report_builder_fields_str = include['model'].split('.')
 
             new_model = apps.get_model(app_label, model)
             if new_model != previous_base_model:
-                new_report_builder_class = getattr(new_model, report_builder_fields_str, None)
+                new_report_builder_class = get_report_builder_class(model=new_model,
+                                                                    class_name=report_builder_fields_str)
                 self._get_fields(base_model=new_model,
                                  fields=fields,
                                  report_builder_class=new_report_builder_class,
                                  tables=tables,
                                  prefix=f"{prefix}{include_field}__",
                                  title_prefix=f"{title_prefix}{include['title']} -> ",
                                  title=include.get('title'),
@@ -324,45 +327,46 @@
         return JsonResponse({'results': fields})
 
     def setup_field(self, field_type, form, field_name, selected_field_id, report_type):
         _fields = []
         if selected_field_id:
             form.fields[field_name].initial = selected_field_id
             base_model = report_type.content_type.model_class()
-            report_builder_fields = getattr(base_model, report_type.report_builder_class_name, None)
+            report_builder_class = get_report_builder_class(model=base_model,
+                                                            report_type=report_type)
             if field_type == 'date':
                 self._get_date_fields(base_model=base_model,
                                       fields=_fields,
-                                      report_builder_class=report_builder_fields,
+                                      report_builder_class=report_builder_class,
                                       selected_field_id=selected_field_id)
             elif field_type == 'link':
                 self._get_column_link_fields(base_model=base_model,
                                              fields=_fields,
-                                             report_builder_class=report_builder_fields,
+                                             report_builder_class=report_builder_class,
                                              selected_field_id=selected_field_id)
             elif field_type == 'number':
                 self._get_number_fields(base_model=base_model,
                                         fields=_fields,
-                                        report_builder_class=report_builder_fields,
+                                        report_builder_class=report_builder_class,
                                         selected_field_id=selected_field_id)
             elif field_type == 'colour':
                 self._get_colour_fields(base_model=base_model,
                                         fields=_fields,
-                                        report_builder_class=report_builder_fields,
+                                        report_builder_class=report_builder_class,
                                         selected_field_id=selected_field_id)
             elif field_type == 'all':
                 self._get_fields(base_model=base_model,
                                  fields=_fields,
-                                 report_builder_class=report_builder_fields,
+                                 report_builder_class=report_builder_class,
                                  selected_field_id=selected_field_id,
                                  for_select2=True)
             elif field_type == 'order':
                 self._get_fields(base_model=base_model,
                                  fields=_fields,
-                                 report_builder_class=report_builder_fields,
+                                 report_builder_class=report_builder_class,
                                  selected_field_id=selected_field_id,
                                  for_select2=True,
                                  show_order_by_fields=True)
 
         form.fields[field_name].widget = Select2(attrs={'ajax': True})
         form.fields[field_name].widget.select_data = _fields
```

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/views/pie_charts.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/views/pie_charts.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from django_modals.modals import FormModal
 from django_modals.processes import PROCESS_EDIT_DELETE, PERMISSION_OFF
 from django_modals.widgets.colour_picker import ColourPickerWidget
 from django_modals.widgets.select2 import Select2Multiple
 
 from advanced_report_builder.models import PieChartReport
 from advanced_report_builder.toggle import RBToggle
-from advanced_report_builder.utils import split_attr, encode_attribute, decode_attribute
+from advanced_report_builder.utils import split_attr, encode_attribute, decode_attribute, get_report_builder_class
 from advanced_report_builder.views.charts_base import ChartBaseView, ChartBaseFieldForm
 from advanced_report_builder.views.modals_base import QueryBuilderModalBaseMixin, QueryBuilderModalBase
 
 
 class PieChartView(ChartBaseView):
     use_annotations = False
 
@@ -105,19 +105,19 @@
 
         if data_attr.get('has_filter') == '1':
             self.fields['has_filter'].initial = True
             if 'filter' in data_attr:
                 self.fields['filter'].initial = decode_attribute(data_attr['filter'])
 
         self.fields['multiple_columns'] = BooleanField(required=False, widget=RBToggle())
-
-        report_builder_fields = getattr(base_model, report_type.report_builder_class_name, None)
+        report_builder_class = get_report_builder_class(model=base_model,
+                                                        report_type=report_type)
         fields = []
         self._get_query_builder_foreign_key_fields(base_model=base_model,
-                                                   report_builder_fields=report_builder_fields,
+                                                   report_builder_class=report_builder_class,
                                                    fields=fields)
 
         self.fields['multiple_column_field'] = ChoiceField(choices=fields, required=False)
 
         if data_attr.get('multiple_columns') == '1':
             self.fields['multiple_columns'].initial = True
             self.fields['multiple_column_field'].initial = data_attr.get('multiple_column_field')
```

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/views/report_utils_mixin.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/views/report_utils_mixin.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/views/reports.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/views/reports.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/views/single_values.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/views/single_values.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,23 @@
 from django.urls import reverse
 from django_datatables.datatables import DatatableTable
 from django_menus.menu import MenuItem
 from django_modals.fields import FieldEx
 from django_modals.helper import show_modal
 from django_modals.modals import Modal
 from django_modals.processes import PROCESS_EDIT_DELETE, PERMISSION_OFF
-from django_modals.widgets.colour_picker import ColourPickerWidget
 from django_modals.widgets.select2 import Select2Multiple
 from django_modals.widgets.widgets import Toggle
 
 from advanced_report_builder.columns import ReportBuilderNumberColumn
 from advanced_report_builder.exceptions import ReportError
 from advanced_report_builder.globals import NUMBER_FIELDS, ANNOTATION_CHOICE_SUM, \
     ANNOTATION_CHOICE_AVERAGE_SUM_FROM_COUNT
 from advanced_report_builder.models import SingleValueReport, ReportType
-from advanced_report_builder.utils import get_field_details
+from advanced_report_builder.utils import get_field_details, get_report_builder_class
 from advanced_report_builder.variable_date import VariableDate
 from advanced_report_builder.views.charts_base import ChartBaseView
 from advanced_report_builder.views.datatables.modal import TableFieldModal, TableFieldForm
 from advanced_report_builder.views.datatables.utils import TableUtilsMixin
 from advanced_report_builder.views.modals_base import QueryBuilderModalBase
 
 
@@ -38,15 +37,16 @@
         self.report = kwargs.get('report')
         self.chart_report = self.report.singlevaluereport
         return super().dispatch(request, *args, **kwargs)
 
     def _process_aggregations(self, fields, aggregations_type=ANNOTATION_CHOICE_SUM, divider=None):
         field = self.chart_report.field
         base_model = self.chart_report.get_base_modal()
-        report_builder_class = getattr(base_model, self.chart_report.report_type.report_builder_class_name, None)
+        report_builder_class = get_report_builder_class(model=base_model,
+                                                        report_type=self.chart_report.report_type)
 
         django_field, col_type_override, _, _ = get_field_details(base_model=base_model,
                                                                   field=field,
                                                                   report_builder_class=report_builder_class)
 
         if (isinstance(django_field, NUMBER_FIELDS) or
                 col_type_override is not None and col_type_override.annotations):
@@ -136,15 +136,16 @@
 
         return field_name
 
     def _process_percentage(self, fields):
         denominator_field = self.chart_report.field
         numerator_field = self.chart_report.numerator
         base_model = self.chart_report.get_base_modal()
-        report_builder_class = getattr(base_model, self.chart_report.report_type.report_builder_class_name, None)
+        report_builder_class = get_report_builder_class(model=base_model,
+                                                        report_type=self.chart_report.report_type)
 
         deno_django_field, denominator_col_type_override, _, _ = get_field_details(
             base_model=base_model,
             field=denominator_field,
             report_builder_class=report_builder_class)
         if (not isinstance(deno_django_field, NUMBER_FIELDS) and
                 (denominator_col_type_override is not None and not denominator_col_type_override.annotations)):
@@ -426,16 +427,16 @@
         single_value_report = get_object_or_404(SingleValueReport, pk=self.slug['pk'])
         self.kwargs['enable_links'] = self.slug['enable_links'] == 'True'
         self.table_report = single_value_report
         base_model = single_value_report.get_base_modal()
         table = self.add_table(base_model=base_model)
         table.extra_filters = self.extra_filters
         table_fields = single_value_report.breakdown_fields
-        report_builder_class = getattr(base_model,
-                                       self.table_report.report_type.report_builder_class_name, None)
+        report_builder_class = get_report_builder_class(model=base_model,
+                                                        report_type=self.table_report.report_type)
         fields_used = set()
         self.process_query_results(report_builder_class=report_builder_class,
                                    table=table,
                                    base_model=base_model,
                                    fields_used=fields_used,
                                    table_fields=table_fields)
```

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/views/targets/utils.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/views/targets/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/advanced_report_builder/views/targets/views.py` & `django-advanced-report-builder-0.5.0/advanced_report_builder/views/targets/views.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/django_advanced_report_builder.egg-info/PKG-INFO` & `django-advanced-report-builder-0.5.0/django_advanced_report_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-report-builder
-Version: 0.4.3
+Version: 0.5.0
 Summary: Django app that allows you to build reports from modals
 Home-page: https://github.com/django-advance-utils/django-advanced-report-builder
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-advanced-report-builder-0.4.3/django_advanced_report_builder.egg-info/SOURCES.txt` & `django-advanced-report-builder-0.5.0/django_advanced_report_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.3/setup.py` & `django-advanced-report-builder-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-advanced-report-builder",
-    version="0.4.3",
+    version="0.5.0",
     author="Thomas Turner",
     description="Django app that allows you to build reports from modals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/django-advance-utils/django-advanced-report-builder",
     include_package_data=True,
     packages=['advanced_report_builder'],
```


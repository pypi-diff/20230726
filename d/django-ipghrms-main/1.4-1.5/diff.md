# Comparing `tmp/django-ipghrms-main-1.4.tar.gz` & `tmp/django-ipghrms-main-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ipghrms-main-1.4.tar", last modified: Wed Jun 21 01:07:34 2023, max compression
+gzip compressed data, was "django-ipghrms-main-1.5.tar", last modified: Sun Jul 23 09:46:45 2023, max compression
```

## Comparing `django-ipghrms-main-1.4.tar` & `django-ipghrms-main-1.5.tar`

### file list

```diff
@@ -1,623 +1,624 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:34.713454 django-ipghrms-main-1.4/
--rw-rw-rw-   0        0        0     1064 2023-03-27 14:53:43.000000 django-ipghrms-main-1.4/LICENSE
--rw-rw-rw-   0        0        0      143 2023-03-27 14:53:53.000000 django-ipghrms-main-1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      915 2023-06-21 01:07:34.718949 django-ipghrms-main-1.4/PKG-INFO
--rw-rw-rw-   0        0        0      475 2023-03-27 14:27:00.000000 django-ipghrms-main-1.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.512675 django-ipghrms-main-1.4/django_ipghrms_main.egg-info/
--rw-rw-rw-   0        0        0      915 2023-06-21 01:07:22.000000 django-ipghrms-main-1.4/django_ipghrms_main.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    26756 2023-06-21 01:07:22.000000 django-ipghrms-main-1.4/django_ipghrms_main.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 01:07:22.000000 django-ipghrms-main-1.4/django_ipghrms_main.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-21 01:07:22.000000 django-ipghrms-main-1.4/django_ipghrms_main.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.533062 django-ipghrms-main-1.4/main/
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/__init__.py
--rw-rw-rw-   0        0        0       63 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/admin.py
--rw-rw-rw-   0        0        0      140 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/apps.py
--rw-rw-rw-   0        0        0       57 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/models.py
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.438035 django-ipghrms-main-1.4/main/static/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.423505 django-ipghrms-main-1.4/main/static/main/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:28.722475 django-ipghrms-main-1.4/main/static/main/css/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:28.737779 django-ipghrms-main-1.4/main/static/main/css/chart/
--rw-rw-rw-   0        0        0     1194 2023-01-17 10:38:56.000000 django-ipghrms-main-1.4/main/static/main/css/chart/all.css
--rw-rw-rw-   0        0        0      824 2023-01-17 10:39:10.000000 django-ipghrms-main-1.4/main/static/main/css/chart/emp_unit.css
--rw-rw-rw-   0        0        0      224 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/css/custom.css
--rw-rw-rw-   0        0        0     2226 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/css/fontastic.css
--rw-rw-rw-   0        0        0      139 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/css/grasp_mobile_progress_circle-1.0.0.min.css
--rw-rw-rw-   0        0        0      825 2022-12-09 14:49:29.000000 django-ipghrms-main-1.4/main/static/main/css/highchart.css
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:28.748780 django-ipghrms-main-1.4/main/static/main/css/leaflet/
--rw-rw-rw-   0        0        0    14655 2023-06-15 09:00:26.000000 django-ipghrms-main-1.4/main/static/main/css/leaflet/leaflet.css
--rw-rw-rw-   0        0        0     1333 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/css/print.css
--rw-rw-rw-   0        0        0    16263 2023-02-21 01:07:33.000000 django-ipghrms-main-1.4/main/static/main/css/select2.min.css
--rw-rw-rw-   0        0        0    58434 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/css/style.blue.css
--rw-rw-rw-   0        0        0    58424 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/css/style.default.css
--rw-rw-rw-   0        0        0    58424 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/css/style.green.css
--rw-rw-rw-   0        0        0    58434 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/css/style.pink.css
--rw-rw-rw-   0        0        0    58424 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/css/style.red.css
--rw-rw-rw-   0        0        0    58434 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/css/style.sea.css
--rw-rw-rw-   0        0        0    58434 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/css/style.violet.css
--rw-rw-rw-   0        0        0      735 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/css/table_print.css
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:28.772303 django-ipghrms-main-1.4/main/static/main/data/
--rw-rw-rw-   0        0        0     4975 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/data/addresses.json
--rw-rw-rw-   0        0        0     2400 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/data/countries.json
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:28.796340 django-ipghrms-main-1.4/main/static/main/fonts/
--rw-rw-rw-   0        0        0     9304 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/fonts/dashboard.eot
--rw-rw-rw-   0        0        0    20946 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/fonts/dashboard.svg
--rw-rw-rw-   0        0        0     9132 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/fonts/dashboard.ttf
--rw-rw-rw-   0        0        0     6088 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/fonts/dashboard.woff
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:28.822756 django-ipghrms-main-1.4/main/static/main/icons-reference/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:28.852411 django-ipghrms-main-1.4/main/static/main/icons-reference/fonts/
--rw-rw-rw-   0        0        0     9304 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/icons-reference/fonts/dashboard.eot
--rw-rw-rw-   0        0        0    20946 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/icons-reference/fonts/dashboard.svg
--rw-rw-rw-   0        0        0     9132 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/icons-reference/fonts/dashboard.ttf
--rw-rw-rw-   0        0        0     6088 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/icons-reference/fonts/dashboard.woff
--rw-rw-rw-   0        0        0    11561 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/icons-reference/icons-reference.html
--rw-rw-rw-   0        0        0     2211 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/icons-reference/styles.css
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:28.955713 django-ipghrms-main-1.4/main/static/main/images/
--rw-rw-rw-   0        0        0   146968 2022-10-19 17:03:53.000000 django-ipghrms-main-1.4/main/static/main/images/adn.png
--rw-rw-rw-   0        0        0    28017 2023-01-17 06:50:41.000000 django-ipghrms-main-1.4/main/static/main/images/all.png
--rw-rw-rw-   0        0        0   119130 2023-02-24 00:43:52.000000 django-ipghrms-main-1.4/main/static/main/images/banner.jpg
--rw-rw-rw-   0        0        0    10744 2023-01-17 06:48:45.000000 django-ipghrms-main-1.4/main/static/main/images/computer.png
--rw-rw-rw-   0        0        0    20016 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/images/error_404.jpg
--rw-rw-rw-   0        0        0    18422 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/images/error_500.jpg
--rw-rw-rw-   0        0        0    16033 2023-02-21 01:04:40.000000 django-ipghrms-main-1.4/main/static/main/images/favicon.png
--rw-rw-rw-   0        0        0     8968 2023-02-21 01:19:32.000000 django-ipghrms-main-1.4/main/static/main/images/favicon2.png
--rw-rw-rw-   0        0        0    21944 2023-01-17 06:32:36.000000 django-ipghrms-main-1.4/main/static/main/images/female.png
--rw-rw-rw-   0        0        0   401518 2022-11-30 07:27:29.000000 django-ipghrms-main-1.4/main/static/main/images/ipg.png
--rw-rw-rw-   0        0        0    87255 2023-02-08 00:10:54.000000 django-ipghrms-main-1.4/main/static/main/images/man.jpg
--rw-rw-rw-   0        0        0    18513 2023-01-17 06:32:36.000000 django-ipghrms-main-1.4/main/static/main/images/man.png
--rw-rw-rw-   0        0        0    27503 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/images/mop_adn_logo.jpg
--rw-rw-rw-   0        0        0    11406 2023-01-07 13:59:43.000000 django-ipghrms-main-1.4/main/static/main/images/mpm.png
--rw-rw-rw-   0        0        0   158833 2022-10-19 17:03:53.000000 django-ipghrms-main-1.4/main/static/main/images/mpo.png
--rw-rw-rw-   0        0        0    16735 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/images/rdtl.jpg
--rw-rw-rw-   0        0        0    36650 2023-01-17 06:48:47.000000 django-ipghrms-main-1.4/main/static/main/images/science.png
--rw-rw-rw-   0        0        0    81243 2023-02-08 00:10:54.000000 django-ipghrms-main-1.4/main/static/main/images/woman.jpg
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:29.132533 django-ipghrms-main-1.4/main/static/main/js/
--rw-rw-rw-   0        0        0     7671 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/js/charts-custom.js
--rw-rw-rw-   0        0        0     3598 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/js/charts-home.js
--rw-rw-rw-   0        0        0      737 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/js/datatable_custom.js
--rw-rw-rw-   0        0        0    11023 2022-12-07 15:13:35.000000 django-ipghrms-main-1.4/main/static/main/js/fa_kit.js
--rw-rw-rw-   0        0        0     4441 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/js/front.js
--rw-rw-rw-   0        0        0     2161 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/js/grasp_mobile_progress_circle-1.0.0.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:29.627655 django-ipghrms-main-1.4/main/static/main/js/highcharts/
--rw-rw-rw-   0        0        0    49321 2023-01-20 01:59:45.000000 django-ipghrms-main-1.4/main/static/main/js/highcharts/3d.js
--rw-rw-rw-   0        0        0   131239 2022-12-17 09:29:51.000000 django-ipghrms-main-1.4/main/static/main/js/highcharts/accessibility.js
--rw-rw-rw-   0        0        0     5077 2023-01-23 13:22:03.000000 django-ipghrms-main-1.4/main/static/main/js/highcharts/cylinder.js
--rw-rw-rw-   0        0        0    16548 2023-01-20 01:59:10.000000 django-ipghrms-main-1.4/main/static/main/js/highcharts/data.js
--rw-rw-rw-   0        0        0    12790 2022-12-17 09:29:12.000000 django-ipghrms-main-1.4/main/static/main/js/highcharts/export-data.js
--rw-rw-rw-   0        0        0    19874 2022-12-17 09:28:46.000000 django-ipghrms-main-1.4/main/static/main/js/highcharts/exporting.js
--rw-rw-rw-   0        0        0   303580 2022-12-17 09:27:49.000000 django-ipghrms-main-1.4/main/static/main/js/highcharts/highcharts.js
--rw-rw-rw-   0        0        0     8580 2023-01-20 01:57:55.000000 django-ipghrms-main-1.4/main/static/main/js/highcharts/organization.js
--rw-rw-rw-   0        0        0    16383 2023-01-20 01:57:22.000000 django-ipghrms-main-1.4/main/static/main/js/highcharts/sankey.js
--rw-rw-rw-   0        0        0    89475 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/js/jquery.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:29.692670 django-ipghrms-main-1.4/main/static/main/js/leaflet/
--rw-rw-rw-   0        0        0   146720 2023-06-15 09:00:55.000000 django-ipghrms-main-1.4/main/static/main/js/leaflet/leaflet.js
--rw-rw-rw-   0        0        0    73164 2023-02-21 01:09:43.000000 django-ipghrms-main-1.4/main/static/main/js/select2.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:29.902679 django-ipghrms-main-1.4/main/static/main/leaflet/
--rw-rw-rw-   0        0        0       89 2023-02-02 07:31:07.000000 django-ipghrms-main-1.4/main/static/main/leaflet/fullscreen.css
--rw-rw-rw-   0        0        0     3677 2023-02-02 07:30:52.000000 django-ipghrms-main-1.4/main/static/main/leaflet/fullscreen.min.js
--rw-rw-rw-   0        0        0    14270 2023-02-02 07:28:13.000000 django-ipghrms-main-1.4/main/static/main/leaflet/leaflet.css
--rw-rw-rw-   0        0        0   109574 2023-02-02 07:28:42.000000 django-ipghrms-main-1.4/main/static/main/leaflet/leaflet.js
--rw-rw-rw-   0        0        0      884 2023-02-02 07:29:17.000000 django-ipghrms-main-1.4/main/static/main/leaflet/markerCluster.css
--rw-rw-rw-   0        0        0     1022 2023-02-02 07:29:51.000000 django-ipghrms-main-1.4/main/static/main/leaflet/markerClusterDefault.min.css
--rw-rw-rw-   0        0        0    33726 2023-02-02 07:30:30.000000 django-ipghrms-main-1.4/main/static/main/leaflet/markercluster.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.434608 django-ipghrms-main-1.4/main/static/main/vendor/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.423505 django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:29.972383 django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/css/
--rw-rw-rw-   0        0        0    64548 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/css/bootstrap-grid.css
--rw-rw-rw-   0        0        0    48488 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-rw-rw-   0        0        0     4681 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/css/bootstrap-reboot.css
--rw-rw-rw-   0        0        0     3836 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-rw-rw-   0        0        0   188998 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/css/bootstrap.css
--rw-rw-rw-   0        0        0   153188 2023-01-09 14:56:02.000000 django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:30.195573 django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/js/
--rw-rw-rw-   0        0        0   217110 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/js/bootstrap.bundle.js
--rw-rw-rw-   0        0        0    76314 2023-01-09 14:55:59.000000 django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   126044 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/js/bootstrap.js
--rw-rw-rw-   0        0        0    55781 2023-01-09 14:55:57.000000 django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/js/bootstrap.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:30.752544 django-ipghrms-main-1.4/main/static/main/vendor/chart.js/
--rw-rw-rw-   0        0        0   549362 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/chart.js/Chart.bundle.js
--rw-rw-rw-   0        0        0   210419 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/chart.js/Chart.bundle.min.js
--rw-rw-rw-   0        0        0   402502 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/chart.js/Chart.js
--rw-rw-rw-   0        0        0   158741 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/chart.js/Chart.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.423505 django-ipghrms-main-1.4/main/static/main/vendor/datatables/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:30.897220 django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/
--rw-rw-rw-   0        0        0     3499 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/buttons.bootstrap4.min.css
--rw-rw-rw-   0        0        0    10058 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/buttons.dataTables.min.css
--rw-rw-rw-   0        0        0     5222 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/dataTables.bootstrap4.min.css
--rw-rw-rw-   0        0        0     5052 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/dataTables.dateTime.min.css
--rw-rw-rw-   0        0        0      401 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/fixedColumns.dataTables.min.css
--rw-rw-rw-   0        0        0    14202 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/jquery.dataTables.min.css
--rw-rw-rw-   0        0        0     4238 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/responsive.dataTables.min.css
--rw-rw-rw-   0        0        0      578 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/scroller.dataTables.min.css
--rw-rw-rw-   0        0        0     8682 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/searchBuilder.bootstrap4.min.css
--rw-rw-rw-   0        0        0    10102 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/searchBuilder.dataTables.min.css
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:30.917793 django-ipghrms-main-1.4/main/static/main/vendor/datatables/images/
--rw-rw-rw-   0        0        0      160 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/images/sort_asc.png
--rw-rw-rw-   0        0        0      148 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/images/sort_asc_disabled.png
--rw-rw-rw-   0        0        0      201 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/images/sort_both.png
--rw-rw-rw-   0        0        0      158 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/images/sort_desc.png
--rw-rw-rw-   0        0        0      146 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/images/sort_desc_disabled.png
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:31.642928 django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/
--rw-rw-rw-   0        0        0     1043 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/buttons.bootstrap4.min.js
--rw-rw-rw-   0        0        0     2947 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/buttons.colVis.min.js
--rw-rw-rw-   0        0        0    25090 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/buttons.html5.min.js
--rw-rw-rw-   0        0        0     2302 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/buttons.print.min.js
--rw-rw-rw-   0        0        0     3159 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/dataTables.bootstrap4.min.js
--rw-rw-rw-   0        0        0    20467 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/dataTables.buttons.min.js
--rw-rw-rw-   0        0        0    15864 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/dataTables.dateTime.min.js
--rw-rw-rw-   0        0        0    20537 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/dataTables.fixedColumns.min.js
--rw-rw-rw-   0        0        0    16849 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/dataTables.responsive.min.js
--rw-rw-rw-   0        0        0    12871 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/dataTables.scroller.min.js
--rw-rw-rw-   0        0        0    72944 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/dataTables.searchBuilder.min.js
--rw-rw-rw-   0        0        0    84321 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/jquery.dataTables.min.js
--rw-rw-rw-   0        0        0   101939 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/jszip.min.js
--rw-rw-rw-   0        0        0  1093401 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/pdfmake.min.js
--rw-rw-rw-   0        0        0      931 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/searchBuilder.bootstrap4.min.js
--rw-rw-rw-   0        0        0   926228 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/vfs_fonts.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:31.913440 django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/
--rw-rw-rw-   0        0        0      323 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/HELP-US-OUT.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:31.952489 django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/css/
--rw-rw-rw-   0        0        0    37414 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/css/font-awesome.css
--rw-rw-rw-   0        0        0    31000 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/css/font-awesome.min.css
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:32.012586 django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/fonts/
--rw-rw-rw-   0        0        0   134808 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/fonts/FontAwesome.otf
--rw-rw-rw-   0        0        0   165742 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   444379 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.woff2
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:32.294544 django-ipghrms-main-1.4/main/static/main/vendor/jquery/
--rw-rw-rw-   0        0        0     9068 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery/core.js
--rw-rw-rw-   0        0        0   271751 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery/jquery.js
--rw-rw-rw-   0        0        0    86927 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery/jquery.min.js
--rw-rw-rw-   0        0        0   218897 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery/jquery.slim.js
--rw-rw-rw-   0        0        0    69917 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery/jquery.slim.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:32.422663 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/
--rw-rw-rw-   0        0        0    51951 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/additional-methods.js
--rw-rw-rw-   0        0        0    22661 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/additional-methods.min.js
--rw-rw-rw-   0        0        0    50659 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/jquery.validate.js
--rw-rw-rw-   0        0        0    24368 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/jquery.validate.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:33.705121 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/
--rw-rw-rw-   0        0        0     1699 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ar.js
--rw-rw-rw-   0        0        0     1558 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ar.min.js
--rw-rw-rw-   0        0        0     1717 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_az.js
--rw-rw-rw-   0        0        0     1575 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_az.min.js
--rw-rw-rw-   0        0        0     1948 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_bg.js
--rw-rw-rw-   0        0        0     1791 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_bg.min.js
--rw-rw-rw-   0        0        0     2293 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_bn_BD.js
--rw-rw-rw-   0        0        0     2152 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_bn_BD.min.js
--rw-rw-rw-   0        0        0     1546 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ca.js
--rw-rw-rw-   0        0        0     1411 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ca.min.js
--rw-rw-rw-   0        0        0     1515 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_cs.js
--rw-rw-rw-   0        0        0     1360 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_cs.min.js
--rw-rw-rw-   0        0        0     1958 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_da.js
--rw-rw-rw-   0        0        0     1783 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_da.min.js
--rw-rw-rw-   0        0        0     4917 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_de.js
--rw-rw-rw-   0        0        0     4626 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_de.min.js
--rw-rw-rw-   0        0        0     2183 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_el.js
--rw-rw-rw-   0        0        0     2041 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_el.min.js
--rw-rw-rw-   0        0        0     1684 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_es.js
--rw-rw-rw-   0        0        0     1539 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_es.min.js
--rw-rw-rw-   0        0        0     1735 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_es_AR.js
--rw-rw-rw-   0        0        0     1564 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_es_AR.min.js
--rw-rw-rw-   0        0        0     1701 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_es_PE.js
--rw-rw-rw-   0        0        0     1534 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_es_PE.min.js
--rw-rw-rw-   0        0        0     1459 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_et.js
--rw-rw-rw-   0        0        0     1319 2022-10-18 10:39:30.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_et.min.js
--rw-rw-rw-   0        0        0     1517 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_eu.js
--rw-rw-rw-   0        0        0     1374 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_eu.min.js
--rw-rw-rw-   0        0        0     2041 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_fa.js
--rw-rw-rw-   0        0        0     1887 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_fa.min.js
--rw-rw-rw-   0        0        0     1570 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_fi.js
--rw-rw-rw-   0        0        0     1429 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_fi.min.js
--rw-rw-rw-   0        0        0     3506 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_fr.js
--rw-rw-rw-   0        0        0     3274 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_fr.min.js
--rw-rw-rw-   0        0        0     2318 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ge.js
--rw-rw-rw-   0        0        0     2122 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ge.min.js
--rw-rw-rw-   0        0        0     1737 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_gl.js
--rw-rw-rw-   0        0        0     1559 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_gl.min.js
--rw-rw-rw-   0        0        0     1518 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_he.js
--rw-rw-rw-   0        0        0     1380 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_he.min.js
--rw-rw-rw-   0        0        0     1357 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_hr.js
--rw-rw-rw-   0        0        0     1215 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_hr.min.js
--rw-rw-rw-   0        0        0     1405 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_hu.js
--rw-rw-rw-   0        0        0     1267 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_hu.min.js
--rw-rw-rw-   0        0        0     1772 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_hy_AM.js
--rw-rw-rw-   0        0        0     1615 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_hy_AM.min.js
--rw-rw-rw-   0        0        0     1449 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_id.js
--rw-rw-rw-   0        0        0     1312 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_id.min.js
--rw-rw-rw-   0        0        0     1279 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_is.js
--rw-rw-rw-   0        0        0     1146 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_is.min.js
--rw-rw-rw-   0        0        0     1541 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_it.js
--rw-rw-rw-   0        0        0     1393 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_it.min.js
--rw-rw-rw-   0        0        0     1762 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ja.js
--rw-rw-rw-   0        0        0     1619 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ja.min.js
--rw-rw-rw-   0        0        0     2654 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ka.js
--rw-rw-rw-   0        0        0     2504 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ka.min.js
--rw-rw-rw-   0        0        0     2153 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_kk.js
--rw-rw-rw-   0        0        0     2007 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_kk.min.js
--rw-rw-rw-   0        0        0     1453 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ko.js
--rw-rw-rw-   0        0        0     1317 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ko.min.js
--rw-rw-rw-   0        0        0     1559 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_lt.js
--rw-rw-rw-   0        0        0     1413 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_lt.min.js
--rw-rw-rw-   0        0        0     1520 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_lv.js
--rw-rw-rw-   0        0        0     1376 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_lv.min.js
--rw-rw-rw-   0        0        0     1795 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_mk.js
--rw-rw-rw-   0        0        0     1633 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_mk.min.js
--rw-rw-rw-   0        0        0     1461 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_my.js
--rw-rw-rw-   0        0        0     1329 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_my.min.js
--rw-rw-rw-   0        0        0     2032 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_nl.js
--rw-rw-rw-   0        0        0     1813 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_nl.min.js
--rw-rw-rw-   0        0        0     1297 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_no.js
--rw-rw-rw-   0        0        0     1160 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_no.min.js
--rw-rw-rw-   0        0        0     1773 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_pl.js
--rw-rw-rw-   0        0        0     1609 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_pl.min.js
--rw-rw-rw-   0        0        0     5942 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_pt_BR.js
--rw-rw-rw-   0        0        0     5577 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_pt_BR.min.js
--rw-rw-rw-   0        0        0     1885 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_pt_PT.js
--rw-rw-rw-   0        0        0     1710 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_pt_PT.min.js
--rw-rw-rw-   0        0        0     1648 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ro.js
--rw-rw-rw-   0        0        0     1505 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ro.min.js
--rw-rw-rw-   0        0        0     2166 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ru.js
--rw-rw-rw-   0        0        0     2015 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ru.min.js
--rw-rw-rw-   0        0        0     1668 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sd.js
--rw-rw-rw-   0        0        0     1482 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sd.min.js
--rw-rw-rw-   0        0        0     1437 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_si.js
--rw-rw-rw-   0        0        0     1309 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_si.min.js
--rw-rw-rw-   0        0        0     1240 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sk.js
--rw-rw-rw-   0        0        0     1088 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sk.min.js
--rw-rw-rw-   0        0        0     1461 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sl.js
--rw-rw-rw-   0        0        0     1314 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sl.min.js
--rw-rw-rw-   0        0        0     1746 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sr.js
--rw-rw-rw-   0        0        0     1595 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sr.min.js
--rw-rw-rw-   0        0        0     1368 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sr_lat.js
--rw-rw-rw-   0        0        0     1200 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sr_lat.min.js
--rw-rw-rw-   0        0        0     1412 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sv.js
--rw-rw-rw-   0        0        0     1277 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sv.min.js
--rw-rw-rw-   0        0        0     2212 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_th.js
--rw-rw-rw-   0        0        0     2078 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_th.min.js
--rw-rw-rw-   0        0        0     2065 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_tj.js
--rw-rw-rw-   0        0        0     1909 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_tj.min.js
--rw-rw-rw-   0        0        0     1733 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_tr.js
--rw-rw-rw-   0        0        0     1592 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_tr.min.js
--rw-rw-rw-   0        0        0     2121 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_uk.js
--rw-rw-rw-   0        0        0     1962 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_uk.min.js
--rw-rw-rw-   0        0        0     1821 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ur.js
--rw-rw-rw-   0        0        0     1688 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ur.min.js
--rw-rw-rw-   0        0        0     1297 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_vi.js
--rw-rw-rw-   0        0        0     1152 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_vi.min.js
--rw-rw-rw-   0        0        0     1401 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_zh.js
--rw-rw-rw-   0        0        0     1233 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_zh.min.js
--rw-rw-rw-   0        0        0     1311 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_zh_TW.js
--rw-rw-rw-   0        0        0     1125 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_zh_TW.min.js
--rw-rw-rw-   0        0        0      688 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_de.js
--rw-rw-rw-   0        0        0      559 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_de.min.js
--rw-rw-rw-   0        0        0      691 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_es_CL.js
--rw-rw-rw-   0        0        0      559 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_es_CL.min.js
--rw-rw-rw-   0        0        0      667 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_fi.js
--rw-rw-rw-   0        0        0      538 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_fi.min.js
--rw-rw-rw-   0        0        0      688 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_it.js
--rw-rw-rw-   0        0        0      559 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_it.min.js
--rw-rw-rw-   0        0        0      700 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_nl.js
--rw-rw-rw-   0        0        0      571 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_nl.min.js
--rw-rw-rw-   0        0        0      554 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_pt.js
--rw-rw-rw-   0        0        0      461 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_pt.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:33.742284 django-ipghrms-main-1.4/main/static/main/vendor/jquery.cookie/
--rw-rw-rw-   0        0        0     1051 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery.cookie/MIT-LICENSE.txt
--rw-rw-rw-   0        0        0      340 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery.cookie/component.json
--rw-rw-rw-   0        0        0      834 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery.cookie/cookie.jquery.json
--rw-rw-rw-   0        0        0     3121 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/jquery.cookie/jquery.cookie.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:33.852598 django-ipghrms-main-1.4/main/static/main/vendor/malihu-custom-scrollbar-plugin/
--rw-rw-rw-   0        0        0    45479 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/malihu-custom-scrollbar-plugin/jquery.mCustomScrollbar.concat.min.js
--rw-rw-rw-   0        0        0    53583 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/malihu-custom-scrollbar-plugin/jquery.mCustomScrollbar.css
--rw-rw-rw-   0        0        0    92949 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/malihu-custom-scrollbar-plugin/jquery.mCustomScrollbar.js
--rw-rw-rw-   0        0        0     2998 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/malihu-custom-scrollbar-plugin/mCSB_buttons.png
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:33.932706 django-ipghrms-main-1.4/main/static/main/vendor/popper.js/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:34.042546 django-ipghrms-main-1.4/main/static/main/vendor/popper.js/esm/
--rw-rw-rw-   0        0        0    35140 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/popper.js/esm/popper-utils.js
--rw-rw-rw-   0        0        0    10567 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/popper.js/esm/popper-utils.min.js
--rw-rw-rw-   0        0        0    86949 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/popper.js/esm/popper.js
--rw-rw-rw-   0        0        0    20969 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/popper.js/esm/popper.min.js
--rw-rw-rw-   0        0        0    33466 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/popper.js/popper-utils.js
--rw-rw-rw-   0        0        0    10116 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/popper.js/popper-utils.min.js
--rw-rw-rw-   0        0        0    83322 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/popper.js/popper.js
--rw-rw-rw-   0        0        0    19666 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/popper.js/popper.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:34.182404 django-ipghrms-main-1.4/main/static/main/vendor/popper.js/umd/
--rw-rw-rw-   0        0        0    36242 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/popper.js/umd/popper-utils.js
--rw-rw-rw-   0        0        0    10730 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/popper.js/umd/popper-utils.min.js
--rw-rw-rw-   0        0        0    87203 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/popper.js/umd/popper.js
--rw-rw-rw-   0        0        0    21004 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/popper.js/umd/popper.min.js
--rw-rw-rw-   0        0        0     3289 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main/vendor/popper.js/umd/poppper.js.flow
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.372477 django-ipghrms-main-1.4/main/static/main2/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.362490 django-ipghrms-main-1.4/main/static/main2/charts/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.772718 django-ipghrms-main-1.4/main/static/main2/charts/js/
--rw-rw-rw-   0        0        0   238712 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/charts/js/highcharts.js
--rw-rw-rw-   0        0        0   260092 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/charts/js/highmaps.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.955763 django-ipghrms-main-1.4/main/static/main2/charts/js/modules/
--rw-rw-rw-   0        0        0    15071 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/charts/js/modules/data.js
--rw-rw-rw-   0        0        0    10617 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/charts/js/modules/drilldown.js
--rw-rw-rw-   0        0        0    10371 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/charts/js/modules/export-data.js
--rw-rw-rw-   0        0        0    14137 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/charts/js/modules/exporting.js
--rw-rw-rw-   0        0        0    12212 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/charts/js/modules/heatmap.js
--rw-rw-rw-   0        0        0     7853 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/charts/js/modules/series-label.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.992370 django-ipghrms-main-1.4/main/static/main2/css/
--rw-rw-rw-   0        0        0   144877 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/css/bootstrap.min.css
--rw-rw-rw-   0        0        0     1202 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/css/main.css
--rw-rw-rw-   0        0        0     2919 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/css/table-responsive.css
--rw-rw-rw-   0        0        0      564 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/css/table_print.css
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.372477 django-ipghrms-main-1.4/main/static/main2/datatables/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:23.092592 django-ipghrms-main-1.4/main/static/main2/datatables/css/
--rw-rw-rw-   0        0        0     3499 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/css/buttons.bootstrap4.min.css
--rw-rw-rw-   0        0        0    10229 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/css/buttons.dataTables.min.css
--rw-rw-rw-   0        0        0     5222 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/css/dataTables.bootstrap4.min.css
--rw-rw-rw-   0        0        0     5052 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/css/dataTables.dateTime.min.css
--rw-rw-rw-   0        0        0      401 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/css/fixedColumns.dataTables.min.css
--rw-rw-rw-   0        0        0    14202 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/css/jquery.dataTables.min.css
--rw-rw-rw-   0        0        0     4238 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/css/responsive.dataTables.min.css
--rw-rw-rw-   0        0        0      578 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/css/scroller.dataTables.min.css
--rw-rw-rw-   0        0        0     8682 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/css/searchBuilder.bootstrap4.min.css
--rw-rw-rw-   0        0        0    10102 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/css/searchBuilder.dataTables.min.css
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:23.112420 django-ipghrms-main-1.4/main/static/main2/datatables/images/
--rw-rw-rw-   0        0        0      160 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/images/sort_asc.png
--rw-rw-rw-   0        0        0      148 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/images/sort_asc_disabled.png
--rw-rw-rw-   0        0        0      201 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/images/sort_both.png
--rw-rw-rw-   0        0        0      158 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/images/sort_desc.png
--rw-rw-rw-   0        0        0      146 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/images/sort_desc_disabled.png
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:23.983330 django-ipghrms-main-1.4/main/static/main2/datatables/js/
--rw-rw-rw-   0        0        0     1043 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/js/buttons.bootstrap4.min.js
--rw-rw-rw-   0        0        0     2947 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/js/buttons.colVis.min.js
--rw-rw-rw-   0        0        0    25090 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/js/buttons.html5.min.js
--rw-rw-rw-   0        0        0     2514 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/js/buttons.print.min.js
--rw-rw-rw-   0        0        0     3159 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/js/dataTables.bootstrap4.min.js
--rw-rw-rw-   0        0        0    20014 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/js/dataTables.buttons.min.js
--rw-rw-rw-   0        0        0    15864 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/js/dataTables.dateTime.min.js
--rw-rw-rw-   0        0        0    20537 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/js/dataTables.fixedColumns.min.js
--rw-rw-rw-   0        0        0    16849 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/js/dataTables.responsive.min.js
--rw-rw-rw-   0        0        0    12871 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/js/dataTables.scroller.min.js
--rw-rw-rw-   0        0        0    61066 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/js/dataTables.searchBuilder.min.js
--rw-rw-rw-   0        0        0    84321 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/js/jquery.dataTables.min.js
--rw-rw-rw-   0        0        0   101939 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/js/jszip.min.js
--rw-rw-rw-   0        0        0  1093401 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/js/pdfmake.min.js
--rw-rw-rw-   0        0        0      931 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/js/searchBuilder.bootstrap4.min.js
--rw-rw-rw-   0        0        0   926228 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/datatables/js/vfs_fonts.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:24.325237 django-ipghrms-main-1.4/main/static/main2/font-awesome/
--rw-rw-rw-   0        0        0      323 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/font-awesome/HELP-US-OUT.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:24.372298 django-ipghrms-main-1.4/main/static/main2/font-awesome/css/
--rw-rw-rw-   0        0        0    37414 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/font-awesome/css/font-awesome.css
--rw-rw-rw-   0        0        0    31000 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/font-awesome/css/font-awesome.min.css
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:24.475261 django-ipghrms-main-1.4/main/static/main2/font-awesome/fonts/
--rw-rw-rw-   0        0        0   134808 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/font-awesome/fonts/FontAwesome.otf
--rw-rw-rw-   0        0        0   165742 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/font-awesome/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   444379 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/font-awesome/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/font-awesome/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/font-awesome/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/font-awesome/fonts/fontawesome-webfont.woff2
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:24.513323 django-ipghrms-main-1.4/main/static/main2/images/
--rw-rw-rw-   0        0        0    71034 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/images/adn.png
--rw-rw-rw-   0        0        0      686 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/images/details_close.png
--rw-rw-rw-   0        0        0      709 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/images/details_open.png
--rw-rw-rw-   0        0        0    20016 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/images/error_404.jpg
--rw-rw-rw-   0        0        0    18422 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/images/error_500.jpg
--rw-rw-rw-   0        0        0     2393 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/images/favicon.png
--rw-rw-rw-   0        0        0    16735 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/images/rdtl.jpg
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:24.712391 django-ipghrms-main-1.4/main/static/main2/js/
--rw-rw-rw-   0        0        0    48944 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/js/bootstrap.min.js
--rw-rw-rw-   0        0        0    69597 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/js/jquery-3.2.1.slim.min.js
--rw-rw-rw-   0        0        0    89475 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/js/jquery.min.js
--rw-rw-rw-   0        0        0    19188 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/js/popper.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:24.782278 django-ipghrms-main-1.4/main/static/main2/summernote/
--rw-rw-rw-   0        0        0    13198 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/summernote/summernote.css
--rw-rw-rw-   0        0        0   200312 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/summernote/summernote.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:25.028495 django-ipghrms-main-1.4/main/static/main2/tinymce/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.372477 django-ipghrms-main-1.4/main/static/main2/tinymce/icons/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:25.207497 django-ipghrms-main-1.4/main/static/main2/tinymce/icons/default/
--rw-rw-rw-   0        0        0    59776 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/icons/default/icons.min.js
--rw-rw-rw-   0        0        0     6671 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/jquery.tinymce.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:25.272681 django-ipghrms-main-1.4/main/static/main2/tinymce/langs/
--rw-rw-rw-   0        0        0      151 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/langs/README.md
--rw-rw-rw-   0        0        0    26441 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/license.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.407666 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:25.282765 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/advlist/
--rw-rw-rw-   0        0        0     3833 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/advlist/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:25.302399 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/anchor/
--rw-rw-rw-   0        0        0     2784 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/anchor/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:25.332653 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/autolink/
--rw-rw-rw-   0        0        0     2431 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/autolink/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:25.352752 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/autoresize/
--rw-rw-rw-   0        0        0     2206 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/autoresize/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:25.378089 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/autosave/
--rw-rw-rw-   0        0        0     2999 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/autosave/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:25.402495 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/bbcode/
--rw-rw-rw-   0        0        0     3105 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/bbcode/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:25.432482 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/charmap/
--rw-rw-rw-   0        0        0    11992 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/charmap/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:25.462315 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/code/
--rw-rw-rw-   0        0        0     1148 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/code/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:25.512281 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/codesample/
--rw-rw-rw-   0        0        0    44693 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/codesample/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:25.585538 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/colorpicker/
--rw-rw-rw-   0        0        0      515 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/colorpicker/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:25.627357 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/contextmenu/
--rw-rw-rw-   0        0        0      515 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/contextmenu/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:25.652741 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/directionality/
--rw-rw-rw-   0        0        0     4083 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/directionality/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:25.692305 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/emoticons/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:26.672574 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/emoticons/js/
--rw-rw-rw-   0        0        0   485684 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/emoticons/js/emojiimages.js
--rw-rw-rw-   0        0        0   424468 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/emoticons/js/emojiimages.min.js
--rw-rw-rw-   0        0        0   262445 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/emoticons/js/emojis.js
--rw-rw-rw-   0        0        0   201229 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/emoticons/js/emojis.min.js
--rw-rw-rw-   0        0        0     7064 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/emoticons/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:26.752707 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/fullpage/
--rw-rw-rw-   0        0        0     7850 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/fullpage/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:26.782457 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/fullscreen/
--rw-rw-rw-   0        0        0    12736 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/fullscreen/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:26.822420 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/help/
--rw-rw-rw-   0        0        0    13682 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/help/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:26.862759 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/hr/
--rw-rw-rw-   0        0        0      799 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/hr/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:26.897544 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/image/
--rw-rw-rw-   0        0        0    21267 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/image/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:26.938476 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/imagetools/
--rw-rw-rw-   0        0        0    17507 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/imagetools/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:26.970241 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/importcss/
--rw-rw-rw-   0        0        0     4054 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/importcss/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:26.986264 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/insertdatetime/
--rw-rw-rw-   0        0        0     2985 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/insertdatetime/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.012672 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/legacyoutput/
--rw-rw-rw-   0        0        0     3057 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/legacyoutput/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.034185 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/link/
--rw-rw-rw-   0        0        0    16244 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/link/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.072634 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/lists/
--rw-rw-rw-   0        0        0    28664 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/lists/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.114060 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/media/
--rw-rw-rw-   0        0        0    18005 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/media/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.142758 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/nonbreaking/
--rw-rw-rw-   0        0        0     1454 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/nonbreaking/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.162505 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/noneditable/
--rw-rw-rw-   0        0        0     1758 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/noneditable/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.177564 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/pagebreak/
--rw-rw-rw-   0        0        0     1691 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/pagebreak/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.212490 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/paste/
--rw-rw-rw-   0        0        0    22710 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/paste/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.256790 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/preview/
--rw-rw-rw-   0        0        0     2151 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/preview/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.272427 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/print/
--rw-rw-rw-   0        0        0      847 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/print/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.303984 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/quickbars/
--rw-rw-rw-   0        0        0     6404 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/quickbars/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.327167 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/save/
--rw-rw-rw-   0        0        0     1724 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/save/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.357373 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/searchreplace/
--rw-rw-rw-   0        0        0    14953 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/searchreplace/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.383623 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/spellchecker/
--rw-rw-rw-   0        0        0     9881 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/spellchecker/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.415403 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/tabfocus/
--rw-rw-rw-   0        0        0     1878 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/tabfocus/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.482345 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/table/
--rw-rw-rw-   0        0        0   137416 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/table/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.567501 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/template/
--rw-rw-rw-   0        0        0     8291 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/template/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.605903 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/textcolor/
--rw-rw-rw-   0        0        0      511 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/textcolor/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.632345 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/textpattern/
--rw-rw-rw-   0        0        0    18260 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/textpattern/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.662719 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/toc/
--rw-rw-rw-   0        0        0     3366 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/toc/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.686003 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/visualblocks/
--rw-rw-rw-   0        0        0     1443 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/visualblocks/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.702584 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/visualchars/
--rw-rw-rw-   0        0        0     6211 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/visualchars/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.742328 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/wordcount/
--rw-rw-rw-   0        0        0    12267 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/wordcount/plugin.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.412675 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.412675 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/content/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.772576 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/content/dark/
--rw-rw-rw-   0        0        0     1469 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/content/dark/content.min.css
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.792647 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/content/default/
--rw-rw-rw-   0        0        0     1399 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/content/default/content.min.css
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.814487 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/content/document/
--rw-rw-rw-   0        0        0     1498 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/content/document/content.min.css
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.837378 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/content/writer/
--rw-rw-rw-   0        0        0     1420 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/content/writer/content.min.css
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.412675 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:27.971615 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide/
--rw-rw-rw-   0        0        0    21776 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide/content.inline.min.css
--rw-rw-rw-   0        0        0    21835 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide/content.min.css
--rw-rw-rw-   0        0        0      544 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide/content.mobile.min.css
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:28.128953 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide/fonts/
--rw-rw-rw-   0        0        0     4624 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide/fonts/tinymce-mobile.woff
--rw-rw-rw-   0        0        0    61106 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide/skin.min.css
--rw-rw-rw-   0        0        0    21004 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide/skin.mobile.min.css
--rw-rw-rw-   0        0        0      764 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide/skin.shadowdom.min.css
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:28.102736 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide-dark/
--rw-rw-rw-   0        0        0    21776 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide-dark/content.inline.min.css
--rw-rw-rw-   0        0        0    21452 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide-dark/content.min.css
--rw-rw-rw-   0        0        0      544 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide-dark/content.mobile.min.css
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:28.117744 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide-dark/fonts/
--rw-rw-rw-   0        0        0     4624 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide-dark/fonts/tinymce-mobile.woff
--rw-rw-rw-   0        0        0    60990 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide-dark/skin.min.css
--rw-rw-rw-   0        0        0    21004 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide-dark/skin.mobile.min.css
--rw-rw-rw-   0        0        0      764 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide-dark/skin.shadowdom.min.css
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.416199 django-ipghrms-main-1.4/main/static/main2/tinymce/themes/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:28.202418 django-ipghrms-main-1.4/main/static/main2/tinymce/themes/mobile/
--rw-rw-rw-   0        0        0   170929 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/themes/mobile/theme.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:28.432359 django-ipghrms-main-1.4/main/static/main2/tinymce/themes/silver/
--rw-rw-rw-   0        0        0   412281 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/themes/silver/theme.min.js
--rw-rw-rw-   0        0        0   114400 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/tinymce.d.ts
--rw-rw-rw-   0        0        0   399558 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/static/main2/tinymce/tinymce.min.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.440855 django-ipghrms-main-1.4/main/static/notif/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:34.202582 django-ipghrms-main-1.4/main/static/notif/dep/
--rw-rw-rw-   0        0        0      344 2023-01-19 01:05:13.000000 django-ipghrms-main-1.4/main/static/notif/dep/notif0.js
--rw-rw-rw-   0        0        0      206 2023-01-19 01:25:51.000000 django-ipghrms-main-1.4/main/static/notif/dep/notif1.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:34.212393 django-ipghrms-main-1.4/main/static/notif/div/
--rw-rw-rw-   0        0        0      344 2023-01-19 05:03:31.000000 django-ipghrms-main-1.4/main/static/notif/div/notif0.js
--rw-rw-rw-   0        0        0      206 2023-01-19 05:03:41.000000 django-ipghrms-main-1.4/main/static/notif/div/notif1.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:34.252732 django-ipghrms-main-1.4/main/static/notif/hr/
--rw-rw-rw-   0        0        0      341 2023-01-17 02:01:21.000000 django-ipghrms-main-1.4/main/static/notif/hr/notif1.js
--rw-rw-rw-   0        0        0      170 2023-01-17 01:45:23.000000 django-ipghrms-main-1.4/main/static/notif/hr/notif2.js
--rw-rw-rw-   0        0        0      169 2023-01-19 10:18:50.000000 django-ipghrms-main-1.4/main/static/notif/hr/notif3.js
--rw-rw-rw-   0        0        0      170 2023-01-19 10:18:01.000000 django-ipghrms-main-1.4/main/static/notif/hr/notif4.js
--rw-rw-rw-   0        0        0      169 2023-01-19 10:17:55.000000 django-ipghrms-main-1.4/main/static/notif/hr/notif5.js
--rw-rw-rw-   0        0        0      173 2023-01-20 02:17:12.000000 django-ipghrms-main-1.4/main/static/notif/hr/notif6.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:34.262495 django-ipghrms-main-1.4/main/static/notif/pr/
--rw-rw-rw-   0        0        0      341 2023-01-22 06:29:29.000000 django-ipghrms-main-1.4/main/static/notif/pr/notif0.js
--rw-rw-rw-   0        0        0      204 2023-01-22 06:29:41.000000 django-ipghrms-main-1.4/main/static/notif/pr/notif1.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:34.282502 django-ipghrms-main-1.4/main/static/notif/staff/
--rw-rw-rw-   0        0        0      350 2023-01-19 01:54:22.000000 django-ipghrms-main-1.4/main/static/notif/staff/notif0.js
--rw-rw-rw-   0        0        0      210 2023-01-19 01:56:00.000000 django-ipghrms-main-1.4/main/static/notif/staff/notif1.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:34.293778 django-ipghrms-main-1.4/main/static/notif/vice/
--rw-rw-rw-   0        0        0      348 2023-03-11 11:17:11.000000 django-ipghrms-main-1.4/main/static/notif/vice/notif0.js
--rw-rw-rw-   0        0        0      208 2023-01-22 08:15:07.000000 django-ipghrms-main-1.4/main/static/notif/vice/notif1.js
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:22.442546 django-ipghrms-main-1.4/main/templates/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:34.497727 django-ipghrms-main-1.4/main/templates/home/
--rw-rw-rw-   0        0        0      256 2022-01-07 07:43:08.000000 django-ipghrms-main-1.4/main/templates/home/403.html
--rw-rw-rw-   0        0        0      228 2022-01-07 07:43:08.000000 django-ipghrms-main-1.4/main/templates/home/404.html
--rw-rw-rw-   0        0        0      228 2022-01-07 07:43:08.000000 django-ipghrms-main-1.4/main/templates/home/500.html
--rw-rw-rw-   0        0        0     7231 2023-06-11 13:25:21.000000 django-ipghrms-main-1.4/main/templates/home/home.html
--rw-rw-rw-   0        0        0     4100 2023-02-10 01:40:07.000000 django-ipghrms-main-1.4/main/templates/home/home_dep.html
--rw-rw-rw-   0        0        0     4369 2023-02-07 01:20:45.000000 django-ipghrms-main-1.4/main/templates/home/home_staff.html
--rw-rw-rw-   0        0        0     1968 2022-12-12 11:16:25.000000 django-ipghrms-main-1.4/main/templates/home/home_staff_bottom.html
--rw-rw-rw-   0        0        0     7080 2023-02-07 02:05:56.000000 django-ipghrms-main-1.4/main/templates/home/home_staff_left.html
--rw-rw-rw-   0        0        0     2542 2023-02-07 02:09:40.000000 django-ipghrms-main-1.4/main/templates/home/home_staff_right.html
--rw-rw-rw-   0        0        0     4217 2023-02-20 02:03:23.000000 django-ipghrms-main-1.4/main/templates/home/home_unit.html
--rw-rw-rw-   0        0        0     3069 2023-02-06 01:05:14.000000 django-ipghrms-main-1.4/main/templates/home/login.html
--rw-rw-rw-   0        0        0     2442 2023-02-06 01:05:10.000000 django-ipghrms-main-1.4/main/templates/home/logout.html
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:34.602358 django-ipghrms-main-1.4/main/templates/main/
--rw-rw-rw-   0        0        0      264 2023-01-20 01:23:28.000000 django-ipghrms-main-1.4/main/templates/main/footer.html
--rw-rw-rw-   0        0        0     1475 2023-03-07 09:53:43.000000 django-ipghrms-main-1.4/main/templates/main/header.html
--rw-rw-rw-   0        0        0    34995 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/templates/main/index.html
--rw-rw-rw-   0        0        0     5212 2023-03-12 10:10:12.000000 django-ipghrms-main-1.4/main/templates/main/layout.html
--rw-rw-rw-   0        0        0     1912 2023-03-07 10:29:21.000000 django-ipghrms-main-1.4/main/templates/main/sidebar.html
--rw-rw-rw-   0        0        0     1747 2023-02-01 05:04:36.000000 django-ipghrms-main-1.4/main/templates/main/sidebar_admin.html
--rw-rw-rw-   0        0        0     3253 2023-03-13 01:50:28.000000 django-ipghrms-main-1.4/main/templates/main/sidebar_de.html
--rw-rw-rw-   0        0        0     2135 2023-03-13 01:33:59.000000 django-ipghrms-main-1.4/main/templates/main/sidebar_dep.html
--rw-rw-rw-   0        0        0     3295 2023-03-13 01:50:35.000000 django-ipghrms-main-1.4/main/templates/main/sidebar_deputy.html
--rw-rw-rw-   0        0        0     3872 2023-06-21 00:59:28.000000 django-ipghrms-main-1.4/main/templates/main/sidebar_hr.html
--rw-rw-rw-   0        0        0     1879 2022-12-14 13:42:11.000000 django-ipghrms-main-1.4/main/templates/main/sidebar_hr_s.html
--rw-rw-rw-   0        0        0     1530 2023-03-15 01:35:11.000000 django-ipghrms-main-1.4/main/templates/main/sidebar_staff.html
--rw-rw-rw-   0        0        0     2321 2023-03-13 01:02:34.000000 django-ipghrms-main-1.4/main/templates/main/sidebar_unit.html
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:34.662483 django-ipghrms-main-1.4/main/templates/main2/
--rw-rw-rw-   0        0        0     1637 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/templates/main2/admin_navbar.html
--rw-rw-rw-   0        0        0     1825 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/templates/main2/de_navbar.html
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/templates/main2/dep_navbar.html
--rw-rw-rw-   0        0        0     1194 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/templates/main2/deputy_navbar.html
--rw-rw-rw-   0        0        0     1730 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/templates/main2/hr_navbar.html
--rw-rw-rw-   0        0        0     2553 2022-11-30 09:04:05.000000 django-ipghrms-main-1.4/main/templates/main2/layout.html
--rw-rw-rw-   0        0        0     1029 2023-03-07 09:58:09.000000 django-ipghrms-main-1.4/main/templates/main2/navbar.html
--rw-rw-rw-   0        0        0     1425 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/templates/main2/staff_navbar.html
--rw-rw-rw-   0        0        0     1436 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/templates/main2/unit_navbar.html
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:34.702486 django-ipghrms-main-1.4/main/templates/notif_header/
--rw-rw-rw-   0        0        0      990 2023-01-19 01:30:05.000000 django-ipghrms-main-1.4/main/templates/notif_header/dep.html
--rw-rw-rw-   0        0        0      992 2023-01-19 05:20:32.000000 django-ipghrms-main-1.4/main/templates/notif_header/div.html
--rw-rw-rw-   0        0        0     2599 2023-01-20 02:24:18.000000 django-ipghrms-main-1.4/main/templates/notif_header/hr.html
--rw-rw-rw-   0        0        0      989 2023-01-22 06:33:25.000000 django-ipghrms-main-1.4/main/templates/notif_header/pr.html
--rw-rw-rw-   0        0        0      996 2023-01-19 01:59:51.000000 django-ipghrms-main-1.4/main/templates/notif_header/staff.html
--rw-rw-rw-   0        0        0      995 2023-01-22 08:19:14.000000 django-ipghrms-main-1.4/main/templates/notif_header/vice.html
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:34.706284 django-ipghrms-main-1.4/main/templatetags/
-drwxrwxrwx   0        0        0        0 2023-06-21 01:07:34.713454 django-ipghrms-main-1.4/main/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      356 2023-01-17 16:31:24.000000 django-ipghrms-main-1.4/main/templatetags/__pycache__/filter.cpython-310.pyc
--rw-rw-rw-   0        0        0      146 2023-01-17 16:31:13.000000 django-ipghrms-main-1.4/main/templatetags/filter.py
--rw-rw-rw-   0        0        0       60 2022-10-18 10:39:31.000000 django-ipghrms-main-1.4/main/tests.py
--rw-rw-rw-   0        0        0     4178 2023-03-07 09:56:38.000000 django-ipghrms-main-1.4/main/views.py
--rw-rw-rw-   0        0        0      503 2023-06-21 01:07:34.729704 django-ipghrms-main-1.4/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-main-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:45.458398 django-ipghrms-main-1.5/
+-rw-rw-rw-   0        0        0     1064 2023-03-27 14:53:43.000000 django-ipghrms-main-1.5/LICENSE
+-rw-rw-rw-   0        0        0      143 2023-03-27 14:53:53.000000 django-ipghrms-main-1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      915 2023-07-23 09:46:45.458398 django-ipghrms-main-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      475 2023-03-27 14:27:00.000000 django-ipghrms-main-1.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.825874 django-ipghrms-main-1.5/django_ipghrms_main.egg-info/
+-rw-rw-rw-   0        0        0      915 2023-07-23 09:46:32.000000 django-ipghrms-main-1.5/django_ipghrms_main.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    26789 2023-07-23 09:46:32.000000 django-ipghrms-main-1.5/django_ipghrms_main.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-23 09:46:32.000000 django-ipghrms-main-1.5/django_ipghrms_main.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-23 09:46:32.000000 django-ipghrms-main-1.5/django_ipghrms_main.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.856108 django-ipghrms-main-1.5/main/
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/__init__.py
+-rw-rw-rw-   0        0        0       63 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/admin.py
+-rw-rw-rw-   0        0        0      140 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/apps.py
+-rw-rw-rw-   0        0        0       57 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/models.py
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.753538 django-ipghrms-main-1.5/main/static/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.730840 django-ipghrms-main-1.5/main/static/main/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:39.166009 django-ipghrms-main-1.5/main/static/main/css/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:39.183817 django-ipghrms-main-1.5/main/static/main/css/chart/
+-rw-rw-rw-   0        0        0     1194 2023-01-17 10:38:56.000000 django-ipghrms-main-1.5/main/static/main/css/chart/all.css
+-rw-rw-rw-   0        0        0      824 2023-01-17 10:39:10.000000 django-ipghrms-main-1.5/main/static/main/css/chart/emp_unit.css
+-rw-rw-rw-   0        0        0      224 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/css/custom.css
+-rw-rw-rw-   0        0        0     2226 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/css/fontastic.css
+-rw-rw-rw-   0        0        0      139 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/css/grasp_mobile_progress_circle-1.0.0.min.css
+-rw-rw-rw-   0        0        0      825 2022-12-09 14:49:29.000000 django-ipghrms-main-1.5/main/static/main/css/highchart.css
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:39.193745 django-ipghrms-main-1.5/main/static/main/css/leaflet/
+-rw-rw-rw-   0        0        0    14655 2023-06-15 09:00:26.000000 django-ipghrms-main-1.5/main/static/main/css/leaflet/leaflet.css
+-rw-rw-rw-   0        0        0     1333 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/css/print.css
+-rw-rw-rw-   0        0        0    16263 2023-02-21 01:07:33.000000 django-ipghrms-main-1.5/main/static/main/css/select2.min.css
+-rw-rw-rw-   0        0        0    58434 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/css/style.blue.css
+-rw-rw-rw-   0        0        0    58424 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/css/style.default.css
+-rw-rw-rw-   0        0        0    58424 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/css/style.green.css
+-rw-rw-rw-   0        0        0    58434 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/css/style.pink.css
+-rw-rw-rw-   0        0        0    58424 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/css/style.red.css
+-rw-rw-rw-   0        0        0    58434 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/css/style.sea.css
+-rw-rw-rw-   0        0        0    58434 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/css/style.violet.css
+-rw-rw-rw-   0        0        0      735 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/css/table_print.css
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:39.220354 django-ipghrms-main-1.5/main/static/main/data/
+-rw-rw-rw-   0        0        0     4975 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/data/addresses.json
+-rw-rw-rw-   0        0        0     2400 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/data/countries.json
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:39.259776 django-ipghrms-main-1.5/main/static/main/fonts/
+-rw-rw-rw-   0        0        0     9304 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/fonts/dashboard.eot
+-rw-rw-rw-   0        0        0    20946 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/fonts/dashboard.svg
+-rw-rw-rw-   0        0        0     9132 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/fonts/dashboard.ttf
+-rw-rw-rw-   0        0        0     6088 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/fonts/dashboard.woff
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:39.288976 django-ipghrms-main-1.5/main/static/main/icons-reference/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:39.327152 django-ipghrms-main-1.5/main/static/main/icons-reference/fonts/
+-rw-rw-rw-   0        0        0     9304 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/icons-reference/fonts/dashboard.eot
+-rw-rw-rw-   0        0        0    20946 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/icons-reference/fonts/dashboard.svg
+-rw-rw-rw-   0        0        0     9132 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/icons-reference/fonts/dashboard.ttf
+-rw-rw-rw-   0        0        0     6088 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/icons-reference/fonts/dashboard.woff
+-rw-rw-rw-   0        0        0    11561 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/icons-reference/icons-reference.html
+-rw-rw-rw-   0        0        0     2211 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/icons-reference/styles.css
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:39.454959 django-ipghrms-main-1.5/main/static/main/images/
+-rw-rw-rw-   0        0        0   146968 2022-10-19 17:03:53.000000 django-ipghrms-main-1.5/main/static/main/images/adn.png
+-rw-rw-rw-   0        0        0    28017 2023-01-17 06:50:41.000000 django-ipghrms-main-1.5/main/static/main/images/all.png
+-rw-rw-rw-   0        0        0   119130 2023-02-24 00:43:52.000000 django-ipghrms-main-1.5/main/static/main/images/banner.jpg
+-rw-rw-rw-   0        0        0    10744 2023-01-17 06:48:45.000000 django-ipghrms-main-1.5/main/static/main/images/computer.png
+-rw-rw-rw-   0        0        0    20016 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/images/error_404.jpg
+-rw-rw-rw-   0        0        0    18422 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/images/error_500.jpg
+-rw-rw-rw-   0        0        0    16033 2023-02-21 01:04:40.000000 django-ipghrms-main-1.5/main/static/main/images/favicon.png
+-rw-rw-rw-   0        0        0     8968 2023-02-21 01:19:32.000000 django-ipghrms-main-1.5/main/static/main/images/favicon2.png
+-rw-rw-rw-   0        0        0    21944 2023-01-17 06:32:36.000000 django-ipghrms-main-1.5/main/static/main/images/female.png
+-rw-rw-rw-   0        0        0   401518 2022-11-30 07:27:29.000000 django-ipghrms-main-1.5/main/static/main/images/ipg.png
+-rw-rw-rw-   0        0        0    87255 2023-02-08 00:10:54.000000 django-ipghrms-main-1.5/main/static/main/images/man.jpg
+-rw-rw-rw-   0        0        0    18513 2023-01-17 06:32:36.000000 django-ipghrms-main-1.5/main/static/main/images/man.png
+-rw-rw-rw-   0        0        0    27503 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/images/mop_adn_logo.jpg
+-rw-rw-rw-   0        0        0    11406 2023-01-07 13:59:43.000000 django-ipghrms-main-1.5/main/static/main/images/mpm.png
+-rw-rw-rw-   0        0        0   158833 2022-10-19 17:03:53.000000 django-ipghrms-main-1.5/main/static/main/images/mpo.png
+-rw-rw-rw-   0        0        0    16735 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/images/rdtl.jpg
+-rw-rw-rw-   0        0        0    36650 2023-01-17 06:48:47.000000 django-ipghrms-main-1.5/main/static/main/images/science.png
+-rw-rw-rw-   0        0        0    81243 2023-02-08 00:10:54.000000 django-ipghrms-main-1.5/main/static/main/images/woman.jpg
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:39.632604 django-ipghrms-main-1.5/main/static/main/js/
+-rw-rw-rw-   0        0        0     7671 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/js/charts-custom.js
+-rw-rw-rw-   0        0        0     3598 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/js/charts-home.js
+-rw-rw-rw-   0        0        0      737 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/js/datatable_custom.js
+-rw-rw-rw-   0        0        0    11023 2022-12-07 15:13:35.000000 django-ipghrms-main-1.5/main/static/main/js/fa_kit.js
+-rw-rw-rw-   0        0        0     4441 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/js/front.js
+-rw-rw-rw-   0        0        0     2161 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/js/grasp_mobile_progress_circle-1.0.0.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:40.156714 django-ipghrms-main-1.5/main/static/main/js/highcharts/
+-rw-rw-rw-   0        0        0    49321 2023-01-20 01:59:45.000000 django-ipghrms-main-1.5/main/static/main/js/highcharts/3d.js
+-rw-rw-rw-   0        0        0   131239 2022-12-17 09:29:51.000000 django-ipghrms-main-1.5/main/static/main/js/highcharts/accessibility.js
+-rw-rw-rw-   0        0        0     5077 2023-01-23 13:22:03.000000 django-ipghrms-main-1.5/main/static/main/js/highcharts/cylinder.js
+-rw-rw-rw-   0        0        0    16548 2023-01-20 01:59:10.000000 django-ipghrms-main-1.5/main/static/main/js/highcharts/data.js
+-rw-rw-rw-   0        0        0    12790 2022-12-17 09:29:12.000000 django-ipghrms-main-1.5/main/static/main/js/highcharts/export-data.js
+-rw-rw-rw-   0        0        0    19874 2022-12-17 09:28:46.000000 django-ipghrms-main-1.5/main/static/main/js/highcharts/exporting.js
+-rw-rw-rw-   0        0        0   303580 2022-12-17 09:27:49.000000 django-ipghrms-main-1.5/main/static/main/js/highcharts/highcharts.js
+-rw-rw-rw-   0        0        0     8580 2023-01-20 01:57:55.000000 django-ipghrms-main-1.5/main/static/main/js/highcharts/organization.js
+-rw-rw-rw-   0        0        0    16383 2023-01-20 01:57:22.000000 django-ipghrms-main-1.5/main/static/main/js/highcharts/sankey.js
+-rw-rw-rw-   0        0        0    89475 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/js/jquery.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:40.236016 django-ipghrms-main-1.5/main/static/main/js/leaflet/
+-rw-rw-rw-   0        0        0   146720 2023-06-15 09:00:55.000000 django-ipghrms-main-1.5/main/static/main/js/leaflet/leaflet.js
+-rw-rw-rw-   0        0        0    73164 2023-02-21 01:09:43.000000 django-ipghrms-main-1.5/main/static/main/js/select2.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:40.442395 django-ipghrms-main-1.5/main/static/main/leaflet/
+-rw-rw-rw-   0        0        0       89 2023-02-02 07:31:07.000000 django-ipghrms-main-1.5/main/static/main/leaflet/fullscreen.css
+-rw-rw-rw-   0        0        0     3677 2023-02-02 07:30:52.000000 django-ipghrms-main-1.5/main/static/main/leaflet/fullscreen.min.js
+-rw-rw-rw-   0        0        0    14270 2023-02-02 07:28:13.000000 django-ipghrms-main-1.5/main/static/main/leaflet/leaflet.css
+-rw-rw-rw-   0        0        0   109574 2023-02-02 07:28:42.000000 django-ipghrms-main-1.5/main/static/main/leaflet/leaflet.js
+-rw-rw-rw-   0        0        0      884 2023-02-02 07:29:17.000000 django-ipghrms-main-1.5/main/static/main/leaflet/markerCluster.css
+-rw-rw-rw-   0        0        0     1022 2023-02-02 07:29:51.000000 django-ipghrms-main-1.5/main/static/main/leaflet/markerClusterDefault.min.css
+-rw-rw-rw-   0        0        0    33726 2023-02-02 07:30:30.000000 django-ipghrms-main-1.5/main/static/main/leaflet/markercluster.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.752403 django-ipghrms-main-1.5/main/static/main/vendor/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.743851 django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:40.506700 django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/css/
+-rw-rw-rw-   0        0        0    64548 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/css/bootstrap-grid.css
+-rw-rw-rw-   0        0        0    48488 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-rw-rw-   0        0        0     4681 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-rw-rw-   0        0        0     3836 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-rw-rw-   0        0        0   188998 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/css/bootstrap.css
+-rw-rw-rw-   0        0        0   153188 2023-01-09 14:56:02.000000 django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:40.760290 django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/js/
+-rw-rw-rw-   0        0        0   217110 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-rw-rw-   0        0        0    76314 2023-01-09 14:55:59.000000 django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   126044 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/js/bootstrap.js
+-rw-rw-rw-   0        0        0    55781 2023-01-09 14:55:57.000000 django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/js/bootstrap.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:41.320689 django-ipghrms-main-1.5/main/static/main/vendor/chart.js/
+-rw-rw-rw-   0        0        0   549362 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/chart.js/Chart.bundle.js
+-rw-rw-rw-   0        0        0   210419 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/chart.js/Chart.bundle.min.js
+-rw-rw-rw-   0        0        0   402502 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/chart.js/Chart.js
+-rw-rw-rw-   0        0        0   158741 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/chart.js/Chart.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.748106 django-ipghrms-main-1.5/main/static/main/vendor/datatables/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:41.462689 django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/
+-rw-rw-rw-   0        0        0     3499 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/buttons.bootstrap4.min.css
+-rw-rw-rw-   0        0        0    10058 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/buttons.dataTables.min.css
+-rw-rw-rw-   0        0        0     5222 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/dataTables.bootstrap4.min.css
+-rw-rw-rw-   0        0        0     5052 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/dataTables.dateTime.min.css
+-rw-rw-rw-   0        0        0      401 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/fixedColumns.dataTables.min.css
+-rw-rw-rw-   0        0        0    14202 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/jquery.dataTables.min.css
+-rw-rw-rw-   0        0        0     4238 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/responsive.dataTables.min.css
+-rw-rw-rw-   0        0        0      578 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/scroller.dataTables.min.css
+-rw-rw-rw-   0        0        0     8682 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/searchBuilder.bootstrap4.min.css
+-rw-rw-rw-   0        0        0    10102 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/searchBuilder.dataTables.min.css
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:41.486541 django-ipghrms-main-1.5/main/static/main/vendor/datatables/images/
+-rw-rw-rw-   0        0        0      160 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/images/sort_asc.png
+-rw-rw-rw-   0        0        0      148 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/images/sort_asc_disabled.png
+-rw-rw-rw-   0        0        0      201 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/images/sort_both.png
+-rw-rw-rw-   0        0        0      158 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/images/sort_desc.png
+-rw-rw-rw-   0        0        0      146 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/images/sort_desc_disabled.png
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:42.391789 django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/
+-rw-rw-rw-   0        0        0     1043 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/buttons.bootstrap4.min.js
+-rw-rw-rw-   0        0        0     2947 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/buttons.colVis.min.js
+-rw-rw-rw-   0        0        0    25090 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/buttons.html5.min.js
+-rw-rw-rw-   0        0        0     2302 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/buttons.print.min.js
+-rw-rw-rw-   0        0        0     3159 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/dataTables.bootstrap4.min.js
+-rw-rw-rw-   0        0        0    20467 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/dataTables.buttons.min.js
+-rw-rw-rw-   0        0        0    15864 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/dataTables.dateTime.min.js
+-rw-rw-rw-   0        0        0    20537 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/dataTables.fixedColumns.min.js
+-rw-rw-rw-   0        0        0    16849 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/dataTables.responsive.min.js
+-rw-rw-rw-   0        0        0    12871 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/dataTables.scroller.min.js
+-rw-rw-rw-   0        0        0    72944 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/dataTables.searchBuilder.min.js
+-rw-rw-rw-   0        0        0    84321 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/jquery.dataTables.min.js
+-rw-rw-rw-   0        0        0   101939 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/jszip.min.js
+-rw-rw-rw-   0        0        0  1093401 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/pdfmake.min.js
+-rw-rw-rw-   0        0        0      931 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/searchBuilder.bootstrap4.min.js
+-rw-rw-rw-   0        0        0   926228 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/vfs_fonts.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:42.675084 django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/
+-rw-rw-rw-   0        0        0      323 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/HELP-US-OUT.txt
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:42.709227 django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/css/
+-rw-rw-rw-   0        0        0    37414 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/css/font-awesome.css
+-rw-rw-rw-   0        0        0    31000 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/css/font-awesome.min.css
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:42.764814 django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/fonts/
+-rw-rw-rw-   0        0        0   134808 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/fonts/FontAwesome.otf
+-rw-rw-rw-   0        0        0   165742 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   444379 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.woff2
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:43.118234 django-ipghrms-main-1.5/main/static/main/vendor/jquery/
+-rw-rw-rw-   0        0        0     9068 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery/core.js
+-rw-rw-rw-   0        0        0   271751 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery/jquery.js
+-rw-rw-rw-   0        0        0    86927 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery/jquery.min.js
+-rw-rw-rw-   0        0        0   218897 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery/jquery.slim.js
+-rw-rw-rw-   0        0        0    69917 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery/jquery.slim.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:43.310516 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/
+-rw-rw-rw-   0        0        0    51951 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/additional-methods.js
+-rw-rw-rw-   0        0        0    22661 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/additional-methods.min.js
+-rw-rw-rw-   0        0        0    50659 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/jquery.validate.js
+-rw-rw-rw-   0        0        0    24368 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/jquery.validate.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:44.583505 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/
+-rw-rw-rw-   0        0        0     1699 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ar.js
+-rw-rw-rw-   0        0        0     1558 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ar.min.js
+-rw-rw-rw-   0        0        0     1717 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_az.js
+-rw-rw-rw-   0        0        0     1575 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_az.min.js
+-rw-rw-rw-   0        0        0     1948 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_bg.js
+-rw-rw-rw-   0        0        0     1791 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_bg.min.js
+-rw-rw-rw-   0        0        0     2293 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_bn_BD.js
+-rw-rw-rw-   0        0        0     2152 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_bn_BD.min.js
+-rw-rw-rw-   0        0        0     1546 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ca.js
+-rw-rw-rw-   0        0        0     1411 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ca.min.js
+-rw-rw-rw-   0        0        0     1515 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_cs.js
+-rw-rw-rw-   0        0        0     1360 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_cs.min.js
+-rw-rw-rw-   0        0        0     1958 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_da.js
+-rw-rw-rw-   0        0        0     1783 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_da.min.js
+-rw-rw-rw-   0        0        0     4917 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_de.js
+-rw-rw-rw-   0        0        0     4626 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_de.min.js
+-rw-rw-rw-   0        0        0     2183 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_el.js
+-rw-rw-rw-   0        0        0     2041 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_el.min.js
+-rw-rw-rw-   0        0        0     1684 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_es.js
+-rw-rw-rw-   0        0        0     1539 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_es.min.js
+-rw-rw-rw-   0        0        0     1735 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_es_AR.js
+-rw-rw-rw-   0        0        0     1564 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_es_AR.min.js
+-rw-rw-rw-   0        0        0     1701 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_es_PE.js
+-rw-rw-rw-   0        0        0     1534 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_es_PE.min.js
+-rw-rw-rw-   0        0        0     1459 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_et.js
+-rw-rw-rw-   0        0        0     1319 2022-10-18 10:39:30.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_et.min.js
+-rw-rw-rw-   0        0        0     1517 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_eu.js
+-rw-rw-rw-   0        0        0     1374 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_eu.min.js
+-rw-rw-rw-   0        0        0     2041 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_fa.js
+-rw-rw-rw-   0        0        0     1887 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_fa.min.js
+-rw-rw-rw-   0        0        0     1570 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_fi.js
+-rw-rw-rw-   0        0        0     1429 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_fi.min.js
+-rw-rw-rw-   0        0        0     3506 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_fr.js
+-rw-rw-rw-   0        0        0     3274 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_fr.min.js
+-rw-rw-rw-   0        0        0     2318 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ge.js
+-rw-rw-rw-   0        0        0     2122 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ge.min.js
+-rw-rw-rw-   0        0        0     1737 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_gl.js
+-rw-rw-rw-   0        0        0     1559 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_gl.min.js
+-rw-rw-rw-   0        0        0     1518 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_he.js
+-rw-rw-rw-   0        0        0     1380 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_he.min.js
+-rw-rw-rw-   0        0        0     1357 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_hr.js
+-rw-rw-rw-   0        0        0     1215 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_hr.min.js
+-rw-rw-rw-   0        0        0     1405 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_hu.js
+-rw-rw-rw-   0        0        0     1267 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_hu.min.js
+-rw-rw-rw-   0        0        0     1772 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_hy_AM.js
+-rw-rw-rw-   0        0        0     1615 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_hy_AM.min.js
+-rw-rw-rw-   0        0        0     1449 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_id.js
+-rw-rw-rw-   0        0        0     1312 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_id.min.js
+-rw-rw-rw-   0        0        0     1279 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_is.js
+-rw-rw-rw-   0        0        0     1146 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_is.min.js
+-rw-rw-rw-   0        0        0     1541 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_it.js
+-rw-rw-rw-   0        0        0     1393 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_it.min.js
+-rw-rw-rw-   0        0        0     1762 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ja.js
+-rw-rw-rw-   0        0        0     1619 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ja.min.js
+-rw-rw-rw-   0        0        0     2654 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ka.js
+-rw-rw-rw-   0        0        0     2504 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ka.min.js
+-rw-rw-rw-   0        0        0     2153 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_kk.js
+-rw-rw-rw-   0        0        0     2007 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_kk.min.js
+-rw-rw-rw-   0        0        0     1453 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ko.js
+-rw-rw-rw-   0        0        0     1317 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ko.min.js
+-rw-rw-rw-   0        0        0     1559 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_lt.js
+-rw-rw-rw-   0        0        0     1413 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_lt.min.js
+-rw-rw-rw-   0        0        0     1520 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_lv.js
+-rw-rw-rw-   0        0        0     1376 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_lv.min.js
+-rw-rw-rw-   0        0        0     1795 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_mk.js
+-rw-rw-rw-   0        0        0     1633 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_mk.min.js
+-rw-rw-rw-   0        0        0     1461 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_my.js
+-rw-rw-rw-   0        0        0     1329 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_my.min.js
+-rw-rw-rw-   0        0        0     2032 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_nl.js
+-rw-rw-rw-   0        0        0     1813 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_nl.min.js
+-rw-rw-rw-   0        0        0     1297 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_no.js
+-rw-rw-rw-   0        0        0     1160 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_no.min.js
+-rw-rw-rw-   0        0        0     1773 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_pl.js
+-rw-rw-rw-   0        0        0     1609 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_pl.min.js
+-rw-rw-rw-   0        0        0     5942 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_pt_BR.js
+-rw-rw-rw-   0        0        0     5577 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_pt_BR.min.js
+-rw-rw-rw-   0        0        0     1885 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_pt_PT.js
+-rw-rw-rw-   0        0        0     1710 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_pt_PT.min.js
+-rw-rw-rw-   0        0        0     1648 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ro.js
+-rw-rw-rw-   0        0        0     1505 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ro.min.js
+-rw-rw-rw-   0        0        0     2166 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ru.js
+-rw-rw-rw-   0        0        0     2015 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ru.min.js
+-rw-rw-rw-   0        0        0     1668 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sd.js
+-rw-rw-rw-   0        0        0     1482 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sd.min.js
+-rw-rw-rw-   0        0        0     1437 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_si.js
+-rw-rw-rw-   0        0        0     1309 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_si.min.js
+-rw-rw-rw-   0        0        0     1240 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sk.js
+-rw-rw-rw-   0        0        0     1088 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sk.min.js
+-rw-rw-rw-   0        0        0     1461 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sl.js
+-rw-rw-rw-   0        0        0     1314 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sl.min.js
+-rw-rw-rw-   0        0        0     1746 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sr.js
+-rw-rw-rw-   0        0        0     1595 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sr.min.js
+-rw-rw-rw-   0        0        0     1368 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sr_lat.js
+-rw-rw-rw-   0        0        0     1200 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sr_lat.min.js
+-rw-rw-rw-   0        0        0     1412 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sv.js
+-rw-rw-rw-   0        0        0     1277 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sv.min.js
+-rw-rw-rw-   0        0        0     2212 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_th.js
+-rw-rw-rw-   0        0        0     2078 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_th.min.js
+-rw-rw-rw-   0        0        0     2065 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_tj.js
+-rw-rw-rw-   0        0        0     1909 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_tj.min.js
+-rw-rw-rw-   0        0        0     1733 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_tr.js
+-rw-rw-rw-   0        0        0     1592 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_tr.min.js
+-rw-rw-rw-   0        0        0     2121 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_uk.js
+-rw-rw-rw-   0        0        0     1962 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_uk.min.js
+-rw-rw-rw-   0        0        0     1821 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ur.js
+-rw-rw-rw-   0        0        0     1688 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ur.min.js
+-rw-rw-rw-   0        0        0     1297 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_vi.js
+-rw-rw-rw-   0        0        0     1152 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_vi.min.js
+-rw-rw-rw-   0        0        0     1401 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_zh.js
+-rw-rw-rw-   0        0        0     1233 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_zh.min.js
+-rw-rw-rw-   0        0        0     1311 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_zh_TW.js
+-rw-rw-rw-   0        0        0     1125 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_zh_TW.min.js
+-rw-rw-rw-   0        0        0      688 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_de.js
+-rw-rw-rw-   0        0        0      559 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_de.min.js
+-rw-rw-rw-   0        0        0      691 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_es_CL.js
+-rw-rw-rw-   0        0        0      559 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_es_CL.min.js
+-rw-rw-rw-   0        0        0      667 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_fi.js
+-rw-rw-rw-   0        0        0      538 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_fi.min.js
+-rw-rw-rw-   0        0        0      688 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_it.js
+-rw-rw-rw-   0        0        0      559 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_it.min.js
+-rw-rw-rw-   0        0        0      700 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_nl.js
+-rw-rw-rw-   0        0        0      571 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_nl.min.js
+-rw-rw-rw-   0        0        0      554 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_pt.js
+-rw-rw-rw-   0        0        0      461 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_pt.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:44.614676 django-ipghrms-main-1.5/main/static/main/vendor/jquery.cookie/
+-rw-rw-rw-   0        0        0     1051 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery.cookie/MIT-LICENSE.txt
+-rw-rw-rw-   0        0        0      340 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery.cookie/component.json
+-rw-rw-rw-   0        0        0      834 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery.cookie/cookie.jquery.json
+-rw-rw-rw-   0        0        0     3121 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/jquery.cookie/jquery.cookie.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:44.748058 django-ipghrms-main-1.5/main/static/main/vendor/malihu-custom-scrollbar-plugin/
+-rw-rw-rw-   0        0        0    45479 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/malihu-custom-scrollbar-plugin/jquery.mCustomScrollbar.concat.min.js
+-rw-rw-rw-   0        0        0    53583 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/malihu-custom-scrollbar-plugin/jquery.mCustomScrollbar.css
+-rw-rw-rw-   0        0        0    92949 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/malihu-custom-scrollbar-plugin/jquery.mCustomScrollbar.js
+-rw-rw-rw-   0        0        0     2998 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/malihu-custom-scrollbar-plugin/mCSB_buttons.png
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:44.817338 django-ipghrms-main-1.5/main/static/main/vendor/popper.js/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:44.926468 django-ipghrms-main-1.5/main/static/main/vendor/popper.js/esm/
+-rw-rw-rw-   0        0        0    35140 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/popper.js/esm/popper-utils.js
+-rw-rw-rw-   0        0        0    10567 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/popper.js/esm/popper-utils.min.js
+-rw-rw-rw-   0        0        0    86949 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/popper.js/esm/popper.js
+-rw-rw-rw-   0        0        0    20969 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/popper.js/esm/popper.min.js
+-rw-rw-rw-   0        0        0    33466 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/popper.js/popper-utils.js
+-rw-rw-rw-   0        0        0    10116 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/popper.js/popper-utils.min.js
+-rw-rw-rw-   0        0        0    83322 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/popper.js/popper.js
+-rw-rw-rw-   0        0        0    19666 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/popper.js/popper.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:45.075788 django-ipghrms-main-1.5/main/static/main/vendor/popper.js/umd/
+-rw-rw-rw-   0        0        0    36242 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/popper.js/umd/popper-utils.js
+-rw-rw-rw-   0        0        0    10730 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/popper.js/umd/popper-utils.min.js
+-rw-rw-rw-   0        0        0    87203 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/popper.js/umd/popper.js
+-rw-rw-rw-   0        0        0    21004 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/popper.js/umd/popper.min.js
+-rw-rw-rw-   0        0        0     3289 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main/vendor/popper.js/umd/poppper.js.flow
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.709150 django-ipghrms-main-1.5/main/static/main2/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.703926 django-ipghrms-main-1.5/main/static/main2/charts/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:33.092807 django-ipghrms-main-1.5/main/static/main2/charts/js/
+-rw-rw-rw-   0        0        0   238712 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/charts/js/highcharts.js
+-rw-rw-rw-   0        0        0   260092 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/charts/js/highmaps.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:33.278885 django-ipghrms-main-1.5/main/static/main2/charts/js/modules/
+-rw-rw-rw-   0        0        0    15071 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/charts/js/modules/data.js
+-rw-rw-rw-   0        0        0    10617 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/charts/js/modules/drilldown.js
+-rw-rw-rw-   0        0        0    10371 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/charts/js/modules/export-data.js
+-rw-rw-rw-   0        0        0    14137 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/charts/js/modules/exporting.js
+-rw-rw-rw-   0        0        0    12212 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/charts/js/modules/heatmap.js
+-rw-rw-rw-   0        0        0     7853 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/charts/js/modules/series-label.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:33.304631 django-ipghrms-main-1.5/main/static/main2/css/
+-rw-rw-rw-   0        0        0   144877 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0     1202 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/css/main.css
+-rw-rw-rw-   0        0        0     2919 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/css/table-responsive.css
+-rw-rw-rw-   0        0        0      564 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/css/table_print.css
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.706857 django-ipghrms-main-1.5/main/static/main2/datatables/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:33.411658 django-ipghrms-main-1.5/main/static/main2/datatables/css/
+-rw-rw-rw-   0        0        0     3499 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/css/buttons.bootstrap4.min.css
+-rw-rw-rw-   0        0        0    10229 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/css/buttons.dataTables.min.css
+-rw-rw-rw-   0        0        0     5222 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/css/dataTables.bootstrap4.min.css
+-rw-rw-rw-   0        0        0     5052 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/css/dataTables.dateTime.min.css
+-rw-rw-rw-   0        0        0      401 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/css/fixedColumns.dataTables.min.css
+-rw-rw-rw-   0        0        0    14202 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/css/jquery.dataTables.min.css
+-rw-rw-rw-   0        0        0     4238 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/css/responsive.dataTables.min.css
+-rw-rw-rw-   0        0        0      578 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/css/scroller.dataTables.min.css
+-rw-rw-rw-   0        0        0     8682 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/css/searchBuilder.bootstrap4.min.css
+-rw-rw-rw-   0        0        0    10102 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/css/searchBuilder.dataTables.min.css
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:33.427873 django-ipghrms-main-1.5/main/static/main2/datatables/images/
+-rw-rw-rw-   0        0        0      160 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/images/sort_asc.png
+-rw-rw-rw-   0        0        0      148 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/images/sort_asc_disabled.png
+-rw-rw-rw-   0        0        0      201 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/images/sort_both.png
+-rw-rw-rw-   0        0        0      158 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/images/sort_desc.png
+-rw-rw-rw-   0        0        0      146 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/images/sort_desc_disabled.png
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:34.287112 django-ipghrms-main-1.5/main/static/main2/datatables/js/
+-rw-rw-rw-   0        0        0     1043 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/js/buttons.bootstrap4.min.js
+-rw-rw-rw-   0        0        0     2947 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/js/buttons.colVis.min.js
+-rw-rw-rw-   0        0        0    25090 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/js/buttons.html5.min.js
+-rw-rw-rw-   0        0        0     2514 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/js/buttons.print.min.js
+-rw-rw-rw-   0        0        0     3159 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/js/dataTables.bootstrap4.min.js
+-rw-rw-rw-   0        0        0    20014 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/js/dataTables.buttons.min.js
+-rw-rw-rw-   0        0        0    15864 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/js/dataTables.dateTime.min.js
+-rw-rw-rw-   0        0        0    20537 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/js/dataTables.fixedColumns.min.js
+-rw-rw-rw-   0        0        0    16849 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/js/dataTables.responsive.min.js
+-rw-rw-rw-   0        0        0    12871 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/js/dataTables.scroller.min.js
+-rw-rw-rw-   0        0        0    61066 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/js/dataTables.searchBuilder.min.js
+-rw-rw-rw-   0        0        0    84321 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/js/jquery.dataTables.min.js
+-rw-rw-rw-   0        0        0   101939 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/js/jszip.min.js
+-rw-rw-rw-   0        0        0  1093401 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/js/pdfmake.min.js
+-rw-rw-rw-   0        0        0      931 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/js/searchBuilder.bootstrap4.min.js
+-rw-rw-rw-   0        0        0   926228 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/datatables/js/vfs_fonts.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:34.557127 django-ipghrms-main-1.5/main/static/main2/font-awesome/
+-rw-rw-rw-   0        0        0      323 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/font-awesome/HELP-US-OUT.txt
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:34.589092 django-ipghrms-main-1.5/main/static/main2/font-awesome/css/
+-rw-rw-rw-   0        0        0    37414 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/font-awesome/css/font-awesome.css
+-rw-rw-rw-   0        0        0    31000 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/font-awesome/css/font-awesome.min.css
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:34.654623 django-ipghrms-main-1.5/main/static/main2/font-awesome/fonts/
+-rw-rw-rw-   0        0        0   134808 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/font-awesome/fonts/FontAwesome.otf
+-rw-rw-rw-   0        0        0   165742 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/font-awesome/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   444379 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/font-awesome/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/font-awesome/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/font-awesome/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/font-awesome/fonts/fontawesome-webfont.woff2
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:34.684853 django-ipghrms-main-1.5/main/static/main2/images/
+-rw-rw-rw-   0        0        0    71034 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/images/adn.png
+-rw-rw-rw-   0        0        0      686 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/images/details_close.png
+-rw-rw-rw-   0        0        0      709 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/images/details_open.png
+-rw-rw-rw-   0        0        0    20016 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/images/error_404.jpg
+-rw-rw-rw-   0        0        0    18422 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/images/error_500.jpg
+-rw-rw-rw-   0        0        0     2393 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/images/favicon.png
+-rw-rw-rw-   0        0        0    16735 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/images/rdtl.jpg
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:34.865483 django-ipghrms-main-1.5/main/static/main2/js/
+-rw-rw-rw-   0        0        0    48944 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0    69597 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/js/jquery-3.2.1.slim.min.js
+-rw-rw-rw-   0        0        0    89475 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/js/jquery.min.js
+-rw-rw-rw-   0        0        0    19188 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/js/popper.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:34.924741 django-ipghrms-main-1.5/main/static/main2/summernote/
+-rw-rw-rw-   0        0        0    13198 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/summernote/summernote.css
+-rw-rw-rw-   0        0        0   200312 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/summernote/summernote.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:35.143658 django-ipghrms-main-1.5/main/static/main2/tinymce/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.710176 django-ipghrms-main-1.5/main/static/main2/tinymce/icons/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:35.366442 django-ipghrms-main-1.5/main/static/main2/tinymce/icons/default/
+-rw-rw-rw-   0        0        0    59776 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/icons/default/icons.min.js
+-rw-rw-rw-   0        0        0     6671 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/jquery.tinymce.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:35.414136 django-ipghrms-main-1.5/main/static/main2/tinymce/langs/
+-rw-rw-rw-   0        0        0      151 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/langs/README.md
+-rw-rw-rw-   0        0        0    26441 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/license.txt
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.730840 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:35.431855 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/advlist/
+-rw-rw-rw-   0        0        0     3833 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/advlist/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:35.469692 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/anchor/
+-rw-rw-rw-   0        0        0     2784 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/anchor/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:35.492513 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/autolink/
+-rw-rw-rw-   0        0        0     2431 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/autolink/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:35.540466 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/autoresize/
+-rw-rw-rw-   0        0        0     2206 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/autoresize/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:35.571914 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/autosave/
+-rw-rw-rw-   0        0        0     2999 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/autosave/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:35.593338 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/bbcode/
+-rw-rw-rw-   0        0        0     3105 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/bbcode/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:35.622244 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/charmap/
+-rw-rw-rw-   0        0        0    11992 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/charmap/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:35.655419 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/code/
+-rw-rw-rw-   0        0        0     1148 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/code/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:35.699005 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/codesample/
+-rw-rw-rw-   0        0        0    44693 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/codesample/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:35.749283 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/colorpicker/
+-rw-rw-rw-   0        0        0      515 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/colorpicker/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:35.763387 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/contextmenu/
+-rw-rw-rw-   0        0        0      515 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/contextmenu/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:35.796107 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/directionality/
+-rw-rw-rw-   0        0        0     4083 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/directionality/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:35.811214 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/emoticons/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.046332 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/emoticons/js/
+-rw-rw-rw-   0        0        0   485684 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/emoticons/js/emojiimages.js
+-rw-rw-rw-   0        0        0   424468 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/emoticons/js/emojiimages.min.js
+-rw-rw-rw-   0        0        0   262445 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/emoticons/js/emojis.js
+-rw-rw-rw-   0        0        0   201229 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/emoticons/js/emojis.min.js
+-rw-rw-rw-   0        0        0     7064 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/emoticons/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.172768 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/fullpage/
+-rw-rw-rw-   0        0        0     7850 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/fullpage/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.190271 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/fullscreen/
+-rw-rw-rw-   0        0        0    12736 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/fullscreen/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.236382 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/help/
+-rw-rw-rw-   0        0        0    13682 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/help/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.256493 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/hr/
+-rw-rw-rw-   0        0        0      799 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/hr/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.284333 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/image/
+-rw-rw-rw-   0        0        0    21267 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/image/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.347441 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/imagetools/
+-rw-rw-rw-   0        0        0    17507 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/imagetools/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.363270 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/importcss/
+-rw-rw-rw-   0        0        0     4054 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/importcss/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.396368 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/insertdatetime/
+-rw-rw-rw-   0        0        0     2985 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/insertdatetime/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.413655 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/legacyoutput/
+-rw-rw-rw-   0        0        0     3057 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/legacyoutput/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.442955 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/link/
+-rw-rw-rw-   0        0        0    16244 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/link/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.474704 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/lists/
+-rw-rw-rw-   0        0        0    28664 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/lists/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.522699 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/media/
+-rw-rw-rw-   0        0        0    18005 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/media/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.554020 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/nonbreaking/
+-rw-rw-rw-   0        0        0     1454 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/nonbreaking/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.572633 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/noneditable/
+-rw-rw-rw-   0        0        0     1758 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/noneditable/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.586099 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/pagebreak/
+-rw-rw-rw-   0        0        0     1691 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/pagebreak/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.618266 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/paste/
+-rw-rw-rw-   0        0        0    22710 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/paste/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.649865 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/preview/
+-rw-rw-rw-   0        0        0     2151 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/preview/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.666005 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/print/
+-rw-rw-rw-   0        0        0      847 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/print/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.697513 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/quickbars/
+-rw-rw-rw-   0        0        0     6404 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/quickbars/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.718747 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/save/
+-rw-rw-rw-   0        0        0     1724 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/save/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.746243 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/searchreplace/
+-rw-rw-rw-   0        0        0    14953 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/searchreplace/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.792879 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/spellchecker/
+-rw-rw-rw-   0        0        0     9881 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/spellchecker/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.813007 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/tabfocus/
+-rw-rw-rw-   0        0        0     1878 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/tabfocus/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.888745 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/table/
+-rw-rw-rw-   0        0        0   137416 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/table/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.969155 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/template/
+-rw-rw-rw-   0        0        0     8291 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/template/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:37.983944 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/textcolor/
+-rw-rw-rw-   0        0        0      511 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/textcolor/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:38.016395 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/textpattern/
+-rw-rw-rw-   0        0        0    18260 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/textpattern/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:38.036999 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/toc/
+-rw-rw-rw-   0        0        0     3366 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/toc/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:38.062923 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/visualblocks/
+-rw-rw-rw-   0        0        0     1443 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/visualblocks/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:38.095143 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/visualchars/
+-rw-rw-rw-   0        0        0     6211 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/visualchars/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:38.125822 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/wordcount/
+-rw-rw-rw-   0        0        0    12267 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/wordcount/plugin.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.730840 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.730840 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/content/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:38.161852 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/content/dark/
+-rw-rw-rw-   0        0        0     1469 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/content/dark/content.min.css
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:38.189596 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/content/default/
+-rw-rw-rw-   0        0        0     1399 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/content/default/content.min.css
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:38.207623 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/content/document/
+-rw-rw-rw-   0        0        0     1498 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/content/document/content.min.css
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:38.236486 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/content/writer/
+-rw-rw-rw-   0        0        0     1420 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/content/writer/content.min.css
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.730840 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:38.363804 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide/
+-rw-rw-rw-   0        0        0    21776 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide/content.inline.min.css
+-rw-rw-rw-   0        0        0    21835 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide/content.min.css
+-rw-rw-rw-   0        0        0      544 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide/content.mobile.min.css
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:38.512907 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide/fonts/
+-rw-rw-rw-   0        0        0     4624 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide/fonts/tinymce-mobile.woff
+-rw-rw-rw-   0        0        0    61106 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide/skin.min.css
+-rw-rw-rw-   0        0        0    21004 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide/skin.mobile.min.css
+-rw-rw-rw-   0        0        0      764 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide/skin.shadowdom.min.css
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:38.481536 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide-dark/
+-rw-rw-rw-   0        0        0    21776 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide-dark/content.inline.min.css
+-rw-rw-rw-   0        0        0    21452 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide-dark/content.min.css
+-rw-rw-rw-   0        0        0      544 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide-dark/content.mobile.min.css
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:38.502378 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide-dark/fonts/
+-rw-rw-rw-   0        0        0     4624 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide-dark/fonts/tinymce-mobile.woff
+-rw-rw-rw-   0        0        0    60990 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide-dark/skin.min.css
+-rw-rw-rw-   0        0        0    21004 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide-dark/skin.mobile.min.css
+-rw-rw-rw-   0        0        0      764 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide-dark/skin.shadowdom.min.css
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.730840 django-ipghrms-main-1.5/main/static/main2/tinymce/themes/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:38.602025 django-ipghrms-main-1.5/main/static/main2/tinymce/themes/mobile/
+-rw-rw-rw-   0        0        0   170929 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/themes/mobile/theme.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:38.871900 django-ipghrms-main-1.5/main/static/main2/tinymce/themes/silver/
+-rw-rw-rw-   0        0        0   412281 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/themes/silver/theme.min.js
+-rw-rw-rw-   0        0        0   114400 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/tinymce.d.ts
+-rw-rw-rw-   0        0        0   399558 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/static/main2/tinymce/tinymce.min.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.756540 django-ipghrms-main-1.5/main/static/notif/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:45.086515 django-ipghrms-main-1.5/main/static/notif/dep/
+-rw-rw-rw-   0        0        0      344 2023-01-19 01:05:13.000000 django-ipghrms-main-1.5/main/static/notif/dep/notif0.js
+-rw-rw-rw-   0        0        0      206 2023-01-19 01:25:51.000000 django-ipghrms-main-1.5/main/static/notif/dep/notif1.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:45.098674 django-ipghrms-main-1.5/main/static/notif/div/
+-rw-rw-rw-   0        0        0      344 2023-01-19 05:03:31.000000 django-ipghrms-main-1.5/main/static/notif/div/notif0.js
+-rw-rw-rw-   0        0        0      206 2023-01-19 05:03:41.000000 django-ipghrms-main-1.5/main/static/notif/div/notif1.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:45.132410 django-ipghrms-main-1.5/main/static/notif/hr/
+-rw-rw-rw-   0        0        0      341 2023-01-17 02:01:21.000000 django-ipghrms-main-1.5/main/static/notif/hr/notif1.js
+-rw-rw-rw-   0        0        0      170 2023-01-17 01:45:23.000000 django-ipghrms-main-1.5/main/static/notif/hr/notif2.js
+-rw-rw-rw-   0        0        0      169 2023-01-19 10:18:50.000000 django-ipghrms-main-1.5/main/static/notif/hr/notif3.js
+-rw-rw-rw-   0        0        0      170 2023-01-19 10:18:01.000000 django-ipghrms-main-1.5/main/static/notif/hr/notif4.js
+-rw-rw-rw-   0        0        0      169 2023-01-19 10:17:55.000000 django-ipghrms-main-1.5/main/static/notif/hr/notif5.js
+-rw-rw-rw-   0        0        0      173 2023-01-20 02:17:12.000000 django-ipghrms-main-1.5/main/static/notif/hr/notif6.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:45.148302 django-ipghrms-main-1.5/main/static/notif/pr/
+-rw-rw-rw-   0        0        0      341 2023-01-22 06:29:29.000000 django-ipghrms-main-1.5/main/static/notif/pr/notif0.js
+-rw-rw-rw-   0        0        0      204 2023-01-22 06:29:41.000000 django-ipghrms-main-1.5/main/static/notif/pr/notif1.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:45.163947 django-ipghrms-main-1.5/main/static/notif/staff/
+-rw-rw-rw-   0        0        0      350 2023-01-19 01:54:22.000000 django-ipghrms-main-1.5/main/static/notif/staff/notif0.js
+-rw-rw-rw-   0        0        0      210 2023-01-19 01:56:00.000000 django-ipghrms-main-1.5/main/static/notif/staff/notif1.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:45.176044 django-ipghrms-main-1.5/main/static/notif/vice/
+-rw-rw-rw-   0        0        0      348 2023-03-11 11:17:11.000000 django-ipghrms-main-1.5/main/static/notif/vice/notif0.js
+-rw-rw-rw-   0        0        0      208 2023-01-22 08:15:07.000000 django-ipghrms-main-1.5/main/static/notif/vice/notif1.js
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:32.757091 django-ipghrms-main-1.5/main/templates/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:45.291382 django-ipghrms-main-1.5/main/templates/home/
+-rw-rw-rw-   0        0        0      256 2022-01-07 07:43:08.000000 django-ipghrms-main-1.5/main/templates/home/403.html
+-rw-rw-rw-   0        0        0      296 2023-07-23 09:19:53.000000 django-ipghrms-main-1.5/main/templates/home/404.html
+-rw-rw-rw-   0        0        0      266 2023-07-23 09:19:46.000000 django-ipghrms-main-1.5/main/templates/home/500.html
+-rw-rw-rw-   0        0        0     7231 2023-06-11 13:25:21.000000 django-ipghrms-main-1.5/main/templates/home/home.html
+-rw-rw-rw-   0        0        0     4100 2023-02-10 01:40:07.000000 django-ipghrms-main-1.5/main/templates/home/home_dep.html
+-rw-rw-rw-   0        0        0     4369 2023-02-07 01:20:45.000000 django-ipghrms-main-1.5/main/templates/home/home_staff.html
+-rw-rw-rw-   0        0        0     1968 2022-12-12 11:16:25.000000 django-ipghrms-main-1.5/main/templates/home/home_staff_bottom.html
+-rw-rw-rw-   0        0        0     7080 2023-02-07 02:05:56.000000 django-ipghrms-main-1.5/main/templates/home/home_staff_left.html
+-rw-rw-rw-   0        0        0     2542 2023-02-07 02:09:40.000000 django-ipghrms-main-1.5/main/templates/home/home_staff_right.html
+-rw-rw-rw-   0        0        0     4217 2023-02-20 02:03:23.000000 django-ipghrms-main-1.5/main/templates/home/home_unit.html
+-rw-rw-rw-   0        0        0     3069 2023-02-06 01:05:14.000000 django-ipghrms-main-1.5/main/templates/home/login.html
+-rw-rw-rw-   0        0        0     2442 2023-02-06 01:05:10.000000 django-ipghrms-main-1.5/main/templates/home/logout.html
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:45.372388 django-ipghrms-main-1.5/main/templates/main/
+-rw-rw-rw-   0        0        0      264 2023-01-20 01:23:28.000000 django-ipghrms-main-1.5/main/templates/main/footer.html
+-rw-rw-rw-   0        0        0     1475 2023-03-07 09:53:43.000000 django-ipghrms-main-1.5/main/templates/main/header.html
+-rw-rw-rw-   0        0        0    34995 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/templates/main/index.html
+-rw-rw-rw-   0        0        0     5212 2023-03-12 10:10:12.000000 django-ipghrms-main-1.5/main/templates/main/layout.html
+-rw-rw-rw-   0        0        0     1048 2023-07-23 09:13:56.000000 django-ipghrms-main-1.5/main/templates/main/layout2.html
+-rw-rw-rw-   0        0        0     1912 2023-03-07 10:29:21.000000 django-ipghrms-main-1.5/main/templates/main/sidebar.html
+-rw-rw-rw-   0        0        0     1747 2023-02-01 05:04:36.000000 django-ipghrms-main-1.5/main/templates/main/sidebar_admin.html
+-rw-rw-rw-   0        0        0     3253 2023-03-13 01:50:28.000000 django-ipghrms-main-1.5/main/templates/main/sidebar_de.html
+-rw-rw-rw-   0        0        0     2135 2023-03-13 01:33:59.000000 django-ipghrms-main-1.5/main/templates/main/sidebar_dep.html
+-rw-rw-rw-   0        0        0     3295 2023-03-13 01:50:35.000000 django-ipghrms-main-1.5/main/templates/main/sidebar_deputy.html
+-rw-rw-rw-   0        0        0     3872 2023-06-21 00:59:28.000000 django-ipghrms-main-1.5/main/templates/main/sidebar_hr.html
+-rw-rw-rw-   0        0        0     1879 2022-12-14 13:42:11.000000 django-ipghrms-main-1.5/main/templates/main/sidebar_hr_s.html
+-rw-rw-rw-   0        0        0     1530 2023-03-15 01:35:11.000000 django-ipghrms-main-1.5/main/templates/main/sidebar_staff.html
+-rw-rw-rw-   0        0        0     2321 2023-03-13 01:02:34.000000 django-ipghrms-main-1.5/main/templates/main/sidebar_unit.html
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:45.412478 django-ipghrms-main-1.5/main/templates/main2/
+-rw-rw-rw-   0        0        0     1637 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/templates/main2/admin_navbar.html
+-rw-rw-rw-   0        0        0     1825 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/templates/main2/de_navbar.html
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/templates/main2/dep_navbar.html
+-rw-rw-rw-   0        0        0     1194 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/templates/main2/deputy_navbar.html
+-rw-rw-rw-   0        0        0     1730 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/templates/main2/hr_navbar.html
+-rw-rw-rw-   0        0        0     2553 2022-11-30 09:04:05.000000 django-ipghrms-main-1.5/main/templates/main2/layout.html
+-rw-rw-rw-   0        0        0     1029 2023-03-07 09:58:09.000000 django-ipghrms-main-1.5/main/templates/main2/navbar.html
+-rw-rw-rw-   0        0        0     1425 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/templates/main2/staff_navbar.html
+-rw-rw-rw-   0        0        0     1436 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/templates/main2/unit_navbar.html
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:45.444179 django-ipghrms-main-1.5/main/templates/notif_header/
+-rw-rw-rw-   0        0        0      990 2023-01-19 01:30:05.000000 django-ipghrms-main-1.5/main/templates/notif_header/dep.html
+-rw-rw-rw-   0        0        0      992 2023-01-19 05:20:32.000000 django-ipghrms-main-1.5/main/templates/notif_header/div.html
+-rw-rw-rw-   0        0        0     2599 2023-01-20 02:24:18.000000 django-ipghrms-main-1.5/main/templates/notif_header/hr.html
+-rw-rw-rw-   0        0        0      989 2023-01-22 06:33:25.000000 django-ipghrms-main-1.5/main/templates/notif_header/pr.html
+-rw-rw-rw-   0        0        0      996 2023-01-19 01:59:51.000000 django-ipghrms-main-1.5/main/templates/notif_header/staff.html
+-rw-rw-rw-   0        0        0      995 2023-01-22 08:19:14.000000 django-ipghrms-main-1.5/main/templates/notif_header/vice.html
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:45.450683 django-ipghrms-main-1.5/main/templatetags/
+drwxrwxrwx   0        0        0        0 2023-07-23 09:46:45.458398 django-ipghrms-main-1.5/main/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      356 2023-01-17 16:31:24.000000 django-ipghrms-main-1.5/main/templatetags/__pycache__/filter.cpython-310.pyc
+-rw-rw-rw-   0        0        0      146 2023-01-17 16:31:13.000000 django-ipghrms-main-1.5/main/templatetags/filter.py
+-rw-rw-rw-   0        0        0       60 2022-10-18 10:39:31.000000 django-ipghrms-main-1.5/main/tests.py
+-rw-rw-rw-   0        0        0     4434 2023-07-23 09:27:16.000000 django-ipghrms-main-1.5/main/views.py
+-rw-rw-rw-   0        0        0      503 2023-07-23 09:46:45.465556 django-ipghrms-main-1.5/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-main-1.5/setup.py
```

### Comparing `django-ipghrms-main-1.4/LICENSE` & `django-ipghrms-main-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/PKG-INFO` & `django-ipghrms-main-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-main
-Version: 1.4
+Version: 1.5
 Summary: Django IPG HRMS APP MAIN
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
```

### Comparing `django-ipghrms-main-1.4/django_ipghrms_main.egg-info/PKG-INFO` & `django-ipghrms-main-1.5/django_ipghrms_main.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-main
-Version: 1.4
+Version: 1.5
 Summary: Django IPG HRMS APP MAIN
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
```

### Comparing `django-ipghrms-main-1.4/django_ipghrms_main.egg-info/SOURCES.txt` & `django-ipghrms-main-1.5/django_ipghrms_main.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -460,14 +460,15 @@
 main/templates/home/home_unit.html
 main/templates/home/login.html
 main/templates/home/logout.html
 main/templates/main/footer.html
 main/templates/main/header.html
 main/templates/main/index.html
 main/templates/main/layout.html
+main/templates/main/layout2.html
 main/templates/main/sidebar.html
 main/templates/main/sidebar_admin.html
 main/templates/main/sidebar_de.html
 main/templates/main/sidebar_dep.html
 main/templates/main/sidebar_deputy.html
 main/templates/main/sidebar_hr.html
 main/templates/main/sidebar_hr_s.html
```

### Comparing `django-ipghrms-main-1.4/main/static/main/css/chart/all.css` & `django-ipghrms-main-1.5/main/static/main/css/chart/all.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/css/chart/emp_unit.css` & `django-ipghrms-main-1.5/main/static/main/css/chart/emp_unit.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/css/fontastic.css` & `django-ipghrms-main-1.5/main/static/main/css/fontastic.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/css/highchart.css` & `django-ipghrms-main-1.5/main/static/main/css/highchart.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/css/leaflet/leaflet.css` & `django-ipghrms-main-1.5/main/static/main/css/leaflet/leaflet.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/css/print.css` & `django-ipghrms-main-1.5/main/static/main/css/print.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/css/select2.min.css` & `django-ipghrms-main-1.5/main/static/main/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/css/style.blue.css` & `django-ipghrms-main-1.5/main/static/main/css/style.blue.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/css/style.default.css` & `django-ipghrms-main-1.5/main/static/main/css/style.default.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/css/style.green.css` & `django-ipghrms-main-1.5/main/static/main/css/style.green.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/css/style.pink.css` & `django-ipghrms-main-1.5/main/static/main/css/style.pink.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/css/style.red.css` & `django-ipghrms-main-1.5/main/static/main/css/style.red.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/css/style.sea.css` & `django-ipghrms-main-1.5/main/static/main/css/style.sea.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/css/style.violet.css` & `django-ipghrms-main-1.5/main/static/main/css/style.violet.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/css/table_print.css` & `django-ipghrms-main-1.5/main/static/main/css/table_print.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/data/addresses.json` & `django-ipghrms-main-1.5/main/static/main/data/addresses.json`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/data/countries.json` & `django-ipghrms-main-1.5/main/static/main/data/countries.json`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/fonts/dashboard.eot` & `django-ipghrms-main-1.5/main/static/main/fonts/dashboard.eot`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/fonts/dashboard.svg` & `django-ipghrms-main-1.5/main/static/main/fonts/dashboard.svg`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/fonts/dashboard.ttf` & `django-ipghrms-main-1.5/main/static/main/fonts/dashboard.ttf`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/fonts/dashboard.woff` & `django-ipghrms-main-1.5/main/static/main/fonts/dashboard.woff`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/icons-reference/fonts/dashboard.eot` & `django-ipghrms-main-1.5/main/static/main/icons-reference/fonts/dashboard.eot`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/icons-reference/fonts/dashboard.svg` & `django-ipghrms-main-1.5/main/static/main/icons-reference/fonts/dashboard.svg`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/icons-reference/fonts/dashboard.ttf` & `django-ipghrms-main-1.5/main/static/main/icons-reference/fonts/dashboard.ttf`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/icons-reference/fonts/dashboard.woff` & `django-ipghrms-main-1.5/main/static/main/icons-reference/fonts/dashboard.woff`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/icons-reference/icons-reference.html` & `django-ipghrms-main-1.5/main/static/main/icons-reference/icons-reference.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/icons-reference/styles.css` & `django-ipghrms-main-1.5/main/static/main/icons-reference/styles.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/adn.png` & `django-ipghrms-main-1.5/main/static/main/images/adn.png`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/all.png` & `django-ipghrms-main-1.5/main/static/main/images/all.png`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/banner.jpg` & `django-ipghrms-main-1.5/main/static/main/images/banner.jpg`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/computer.png` & `django-ipghrms-main-1.5/main/static/main/images/computer.png`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/error_404.jpg` & `django-ipghrms-main-1.5/main/static/main/images/error_404.jpg`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/error_500.jpg` & `django-ipghrms-main-1.5/main/static/main/images/error_500.jpg`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/favicon.png` & `django-ipghrms-main-1.5/main/static/main/images/favicon.png`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/favicon2.png` & `django-ipghrms-main-1.5/main/static/main/images/favicon2.png`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/female.png` & `django-ipghrms-main-1.5/main/static/main/images/female.png`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/ipg.png` & `django-ipghrms-main-1.5/main/static/main/images/ipg.png`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/man.jpg` & `django-ipghrms-main-1.5/main/static/main/images/man.jpg`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/man.png` & `django-ipghrms-main-1.5/main/static/main/images/man.png`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/mop_adn_logo.jpg` & `django-ipghrms-main-1.5/main/static/main/images/mop_adn_logo.jpg`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/mpm.png` & `django-ipghrms-main-1.5/main/static/main/images/mpm.png`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/mpo.png` & `django-ipghrms-main-1.5/main/static/main/images/mpo.png`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/rdtl.jpg` & `django-ipghrms-main-1.5/main/static/main/images/rdtl.jpg`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/science.png` & `django-ipghrms-main-1.5/main/static/main/images/science.png`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/images/woman.jpg` & `django-ipghrms-main-1.5/main/static/main/images/woman.jpg`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/charts-custom.js` & `django-ipghrms-main-1.5/main/static/main/js/charts-custom.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/charts-home.js` & `django-ipghrms-main-1.5/main/static/main/js/charts-home.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/datatable_custom.js` & `django-ipghrms-main-1.5/main/static/main/js/datatable_custom.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/fa_kit.js` & `django-ipghrms-main-1.5/main/static/main/js/fa_kit.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/front.js` & `django-ipghrms-main-1.5/main/static/main/js/front.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/grasp_mobile_progress_circle-1.0.0.min.js` & `django-ipghrms-main-1.5/main/static/main/js/grasp_mobile_progress_circle-1.0.0.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/highcharts/3d.js` & `django-ipghrms-main-1.5/main/static/main/js/highcharts/3d.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/highcharts/accessibility.js` & `django-ipghrms-main-1.5/main/static/main/js/highcharts/accessibility.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/highcharts/cylinder.js` & `django-ipghrms-main-1.5/main/static/main/js/highcharts/cylinder.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/highcharts/data.js` & `django-ipghrms-main-1.5/main/static/main/js/highcharts/data.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/highcharts/export-data.js` & `django-ipghrms-main-1.5/main/static/main/js/highcharts/export-data.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/highcharts/exporting.js` & `django-ipghrms-main-1.5/main/static/main/js/highcharts/exporting.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/highcharts/highcharts.js` & `django-ipghrms-main-1.5/main/static/main/js/highcharts/highcharts.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/highcharts/organization.js` & `django-ipghrms-main-1.5/main/static/main/js/highcharts/organization.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/highcharts/sankey.js` & `django-ipghrms-main-1.5/main/static/main/js/highcharts/sankey.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/jquery.min.js` & `django-ipghrms-main-1.5/main/static/main/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/leaflet/leaflet.js` & `django-ipghrms-main-1.5/main/static/main/js/leaflet/leaflet.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/js/select2.min.js` & `django-ipghrms-main-1.5/main/static/main/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/leaflet/fullscreen.min.js` & `django-ipghrms-main-1.5/main/static/main/leaflet/fullscreen.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/leaflet/leaflet.css` & `django-ipghrms-main-1.5/main/static/main/leaflet/leaflet.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/leaflet/leaflet.js` & `django-ipghrms-main-1.5/main/static/main/leaflet/leaflet.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/leaflet/markerCluster.css` & `django-ipghrms-main-1.5/main/static/main/leaflet/markerCluster.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/leaflet/markerClusterDefault.min.css` & `django-ipghrms-main-1.5/main/static/main/leaflet/markerClusterDefault.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/leaflet/markercluster.js` & `django-ipghrms-main-1.5/main/static/main/leaflet/markercluster.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/css/bootstrap-grid.css` & `django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/css/bootstrap-grid.min.css` & `django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/css/bootstrap-reboot.css` & `django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/css/bootstrap-reboot.min.css` & `django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/css/bootstrap.css` & `django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/css/bootstrap.min.css` & `django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/js/bootstrap.bundle.js` & `django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/js/bootstrap.bundle.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/js/bootstrap.js` & `django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/bootstrap/js/bootstrap.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/chart.js/Chart.bundle.js` & `django-ipghrms-main-1.5/main/static/main/vendor/chart.js/Chart.bundle.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/chart.js/Chart.bundle.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/chart.js/Chart.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/chart.js/Chart.js` & `django-ipghrms-main-1.5/main/static/main/vendor/chart.js/Chart.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/chart.js/Chart.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/chart.js/Chart.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/buttons.bootstrap4.min.css` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/buttons.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/buttons.dataTables.min.css` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/buttons.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/dataTables.bootstrap4.min.css` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/dataTables.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/dataTables.dateTime.min.css` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/dataTables.dateTime.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/jquery.dataTables.min.css` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/responsive.dataTables.min.css` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/responsive.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/scroller.dataTables.min.css` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/scroller.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/searchBuilder.bootstrap4.min.css` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/searchBuilder.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/css/searchBuilder.dataTables.min.css` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/css/searchBuilder.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/buttons.bootstrap4.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/buttons.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/buttons.colVis.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/buttons.colVis.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/buttons.html5.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/buttons.html5.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/buttons.print.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/buttons.print.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/dataTables.bootstrap4.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/dataTables.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/dataTables.buttons.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/dataTables.buttons.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/dataTables.dateTime.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/dataTables.dateTime.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/dataTables.fixedColumns.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/dataTables.fixedColumns.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/dataTables.responsive.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/dataTables.responsive.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/dataTables.scroller.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/dataTables.scroller.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/dataTables.searchBuilder.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/dataTables.searchBuilder.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/jquery.dataTables.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/jszip.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/jszip.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/pdfmake.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/pdfmake.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/searchBuilder.bootstrap4.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/searchBuilder.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/datatables/js/vfs_fonts.js` & `django-ipghrms-main-1.5/main/static/main/vendor/datatables/js/vfs_fonts.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/css/font-awesome.css` & `django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/css/font-awesome.min.css` & `django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/fonts/FontAwesome.otf` & `django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.eot` & `django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.svg` & `django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.ttf` & `django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.woff` & `django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.woff2` & `django-ipghrms-main-1.5/main/static/main/vendor/font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery/core.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery/core.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery/jquery.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery/jquery.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery/jquery.slim.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery/jquery.slim.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery/jquery.slim.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/additional-methods.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/additional-methods.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/additional-methods.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/additional-methods.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/jquery.validate.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/jquery.validate.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/jquery.validate.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/jquery.validate.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ar.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ar.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ar.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ar.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_az.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_az.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_az.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_az.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_bg.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_bg.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_bg.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_bg.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_bn_BD.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_bn_BD.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_bn_BD.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_bn_BD.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ca.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ca.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ca.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ca.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_cs.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_cs.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_cs.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_cs.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_da.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_da.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_da.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_da.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_de.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_de.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_de.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_de.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_el.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_el.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_el.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_el.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_es.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_es.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_es.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_es.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_es_AR.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_es_AR.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_es_AR.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_es_AR.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_es_PE.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_es_PE.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_es_PE.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_es_PE.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_et.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_et.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_et.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_et.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_eu.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_eu.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_eu.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_eu.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_fa.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_fa.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_fa.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_fa.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_fi.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_fi.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_fi.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_fi.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_fr.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_fr.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_fr.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_fr.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ge.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ge.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ge.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ge.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_gl.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_gl.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_gl.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_gl.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_he.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_he.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_he.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_he.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_hr.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_hr.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_hr.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_hr.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_hu.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_hu.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_hu.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_hu.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_hy_AM.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_hy_AM.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_hy_AM.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_hy_AM.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_id.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_id.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_id.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_id.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_is.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_is.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_is.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_is.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_it.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_it.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_it.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_it.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ja.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ja.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ja.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ja.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ka.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ka.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ka.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ka.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_kk.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_kk.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_kk.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_kk.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ko.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ko.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ko.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ko.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_lt.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_lt.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_lt.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_lt.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_lv.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_lv.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_lv.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_lv.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_mk.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_mk.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_mk.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_mk.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_my.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_my.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_my.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_my.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_nl.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_nl.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_nl.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_nl.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_no.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_no.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_no.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_no.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_pl.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_pl.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_pl.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_pl.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_pt_BR.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_pt_BR.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_pt_BR.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_pt_BR.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_pt_PT.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_pt_PT.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_pt_PT.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_pt_PT.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ro.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ro.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ro.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ro.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ru.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ru.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ru.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ru.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sd.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sd.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sd.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sd.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_si.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_si.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_si.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_si.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sk.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sk.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sk.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sk.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sl.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sl.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sl.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sl.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sr.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sr.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sr.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sr.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sr_lat.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sr_lat.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sr_lat.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sr_lat.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sv.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sv.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_sv.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_sv.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_th.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_th.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_th.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_th.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_tj.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_tj.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_tj.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_tj.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_tr.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_tr.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_tr.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_tr.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_uk.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_uk.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_uk.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_uk.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ur.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ur.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_ur.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_ur.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_vi.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_vi.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_vi.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_vi.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_zh.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_zh.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_zh.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_zh.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_zh_TW.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_zh_TW.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/messages_zh_TW.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/messages_zh_TW.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_de.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_de.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_de.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_de.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_es_CL.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_es_CL.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_es_CL.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_es_CL.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_fi.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_fi.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_fi.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_fi.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_it.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_it.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_it.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_it.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_nl.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_nl.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_nl.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_nl.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery-validation/localization/methods_pt.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery-validation/localization/methods_pt.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery.cookie/MIT-LICENSE.txt` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery.cookie/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery.cookie/cookie.jquery.json` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery.cookie/cookie.jquery.json`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/jquery.cookie/jquery.cookie.js` & `django-ipghrms-main-1.5/main/static/main/vendor/jquery.cookie/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/malihu-custom-scrollbar-plugin/jquery.mCustomScrollbar.concat.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/malihu-custom-scrollbar-plugin/jquery.mCustomScrollbar.concat.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/malihu-custom-scrollbar-plugin/jquery.mCustomScrollbar.css` & `django-ipghrms-main-1.5/main/static/main/vendor/malihu-custom-scrollbar-plugin/jquery.mCustomScrollbar.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/malihu-custom-scrollbar-plugin/jquery.mCustomScrollbar.js` & `django-ipghrms-main-1.5/main/static/main/vendor/malihu-custom-scrollbar-plugin/jquery.mCustomScrollbar.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/malihu-custom-scrollbar-plugin/mCSB_buttons.png` & `django-ipghrms-main-1.5/main/static/main/vendor/malihu-custom-scrollbar-plugin/mCSB_buttons.png`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/popper.js/esm/popper-utils.js` & `django-ipghrms-main-1.5/main/static/main/vendor/popper.js/esm/popper-utils.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/popper.js/esm/popper-utils.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/popper.js/esm/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/popper.js/esm/popper.js` & `django-ipghrms-main-1.5/main/static/main/vendor/popper.js/esm/popper.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/popper.js/esm/popper.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/popper.js/esm/popper.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/popper.js/popper-utils.js` & `django-ipghrms-main-1.5/main/static/main/vendor/popper.js/popper-utils.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/popper.js/popper-utils.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/popper.js/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/popper.js/popper.js` & `django-ipghrms-main-1.5/main/static/main/vendor/popper.js/popper.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/popper.js/popper.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/popper.js/popper.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/popper.js/umd/popper-utils.js` & `django-ipghrms-main-1.5/main/static/main/vendor/popper.js/umd/popper-utils.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/popper.js/umd/popper-utils.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/popper.js/umd/popper-utils.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/popper.js/umd/popper.js` & `django-ipghrms-main-1.5/main/static/main/vendor/popper.js/umd/popper.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/popper.js/umd/popper.min.js` & `django-ipghrms-main-1.5/main/static/main/vendor/popper.js/umd/popper.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main/vendor/popper.js/umd/poppper.js.flow` & `django-ipghrms-main-1.5/main/static/main/vendor/popper.js/umd/poppper.js.flow`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/charts/js/highcharts.js` & `django-ipghrms-main-1.5/main/static/main2/charts/js/highcharts.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/charts/js/highmaps.js` & `django-ipghrms-main-1.5/main/static/main2/charts/js/highmaps.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/charts/js/modules/data.js` & `django-ipghrms-main-1.5/main/static/main2/charts/js/modules/data.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/charts/js/modules/drilldown.js` & `django-ipghrms-main-1.5/main/static/main2/charts/js/modules/drilldown.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/charts/js/modules/export-data.js` & `django-ipghrms-main-1.5/main/static/main2/charts/js/modules/export-data.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/charts/js/modules/exporting.js` & `django-ipghrms-main-1.5/main/static/main2/charts/js/modules/exporting.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/charts/js/modules/heatmap.js` & `django-ipghrms-main-1.5/main/static/main2/charts/js/modules/heatmap.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/charts/js/modules/series-label.js` & `django-ipghrms-main-1.5/main/static/main2/charts/js/modules/series-label.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/css/bootstrap.min.css` & `django-ipghrms-main-1.5/main/static/main2/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/css/main.css` & `django-ipghrms-main-1.5/main/static/main2/css/main.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/css/table-responsive.css` & `django-ipghrms-main-1.5/main/static/main2/css/table-responsive.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/css/table_print.css` & `django-ipghrms-main-1.5/main/static/main2/css/table_print.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/css/buttons.bootstrap4.min.css` & `django-ipghrms-main-1.5/main/static/main2/datatables/css/buttons.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/css/buttons.dataTables.min.css` & `django-ipghrms-main-1.5/main/static/main2/datatables/css/buttons.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/css/dataTables.bootstrap4.min.css` & `django-ipghrms-main-1.5/main/static/main2/datatables/css/dataTables.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/css/dataTables.dateTime.min.css` & `django-ipghrms-main-1.5/main/static/main2/datatables/css/dataTables.dateTime.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/css/jquery.dataTables.min.css` & `django-ipghrms-main-1.5/main/static/main2/datatables/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/css/responsive.dataTables.min.css` & `django-ipghrms-main-1.5/main/static/main2/datatables/css/responsive.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/css/scroller.dataTables.min.css` & `django-ipghrms-main-1.5/main/static/main2/datatables/css/scroller.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/css/searchBuilder.bootstrap4.min.css` & `django-ipghrms-main-1.5/main/static/main2/datatables/css/searchBuilder.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/css/searchBuilder.dataTables.min.css` & `django-ipghrms-main-1.5/main/static/main2/datatables/css/searchBuilder.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/js/buttons.bootstrap4.min.js` & `django-ipghrms-main-1.5/main/static/main2/datatables/js/buttons.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/js/buttons.colVis.min.js` & `django-ipghrms-main-1.5/main/static/main2/datatables/js/buttons.colVis.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/js/buttons.html5.min.js` & `django-ipghrms-main-1.5/main/static/main2/datatables/js/buttons.html5.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/js/buttons.print.min.js` & `django-ipghrms-main-1.5/main/static/main2/datatables/js/buttons.print.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/js/dataTables.bootstrap4.min.js` & `django-ipghrms-main-1.5/main/static/main2/datatables/js/dataTables.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/js/dataTables.buttons.min.js` & `django-ipghrms-main-1.5/main/static/main2/datatables/js/dataTables.buttons.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/js/dataTables.dateTime.min.js` & `django-ipghrms-main-1.5/main/static/main2/datatables/js/dataTables.dateTime.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/js/dataTables.fixedColumns.min.js` & `django-ipghrms-main-1.5/main/static/main2/datatables/js/dataTables.fixedColumns.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/js/dataTables.responsive.min.js` & `django-ipghrms-main-1.5/main/static/main2/datatables/js/dataTables.responsive.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/js/dataTables.scroller.min.js` & `django-ipghrms-main-1.5/main/static/main2/datatables/js/dataTables.scroller.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/js/dataTables.searchBuilder.min.js` & `django-ipghrms-main-1.5/main/static/main2/datatables/js/dataTables.searchBuilder.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/js/jquery.dataTables.min.js` & `django-ipghrms-main-1.5/main/static/main2/datatables/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/js/jszip.min.js` & `django-ipghrms-main-1.5/main/static/main2/datatables/js/jszip.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/js/pdfmake.min.js` & `django-ipghrms-main-1.5/main/static/main2/datatables/js/pdfmake.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/js/searchBuilder.bootstrap4.min.js` & `django-ipghrms-main-1.5/main/static/main2/datatables/js/searchBuilder.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/datatables/js/vfs_fonts.js` & `django-ipghrms-main-1.5/main/static/main2/datatables/js/vfs_fonts.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/font-awesome/css/font-awesome.css` & `django-ipghrms-main-1.5/main/static/main2/font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/font-awesome/css/font-awesome.min.css` & `django-ipghrms-main-1.5/main/static/main2/font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/font-awesome/fonts/FontAwesome.otf` & `django-ipghrms-main-1.5/main/static/main2/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/font-awesome/fonts/fontawesome-webfont.eot` & `django-ipghrms-main-1.5/main/static/main2/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/font-awesome/fonts/fontawesome-webfont.svg` & `django-ipghrms-main-1.5/main/static/main2/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/font-awesome/fonts/fontawesome-webfont.ttf` & `django-ipghrms-main-1.5/main/static/main2/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/font-awesome/fonts/fontawesome-webfont.woff` & `django-ipghrms-main-1.5/main/static/main2/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/font-awesome/fonts/fontawesome-webfont.woff2` & `django-ipghrms-main-1.5/main/static/main2/font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/images/adn.png` & `django-ipghrms-main-1.5/main/static/main2/images/adn.png`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/images/details_close.png` & `django-ipghrms-main-1.5/main/static/main2/images/details_close.png`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/images/details_open.png` & `django-ipghrms-main-1.5/main/static/main2/images/details_open.png`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/images/error_404.jpg` & `django-ipghrms-main-1.5/main/static/main2/images/error_404.jpg`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/images/error_500.jpg` & `django-ipghrms-main-1.5/main/static/main2/images/error_500.jpg`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/images/favicon.png` & `django-ipghrms-main-1.5/main/static/main2/images/favicon.png`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/images/rdtl.jpg` & `django-ipghrms-main-1.5/main/static/main2/images/rdtl.jpg`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/js/bootstrap.min.js` & `django-ipghrms-main-1.5/main/static/main2/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/js/jquery-3.2.1.slim.min.js` & `django-ipghrms-main-1.5/main/static/main2/js/jquery-3.2.1.slim.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/js/jquery.min.js` & `django-ipghrms-main-1.5/main/static/main2/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/js/popper.min.js` & `django-ipghrms-main-1.5/main/static/main2/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/summernote/summernote.css` & `django-ipghrms-main-1.5/main/static/main2/summernote/summernote.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/summernote/summernote.js` & `django-ipghrms-main-1.5/main/static/main2/summernote/summernote.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/icons/default/icons.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/icons/default/icons.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/jquery.tinymce.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/jquery.tinymce.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/license.txt` & `django-ipghrms-main-1.5/main/static/main2/tinymce/license.txt`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/advlist/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/advlist/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/anchor/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/anchor/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/autolink/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/autolink/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/autoresize/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/autoresize/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/autosave/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/autosave/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/bbcode/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/bbcode/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/charmap/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/charmap/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/code/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/code/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/codesample/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/codesample/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/colorpicker/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/colorpicker/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/contextmenu/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/contextmenu/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/directionality/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/directionality/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/emoticons/js/emojiimages.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/emoticons/js/emojiimages.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/emoticons/js/emojiimages.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/emoticons/js/emojiimages.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/emoticons/js/emojis.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/emoticons/js/emojis.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/emoticons/js/emojis.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/emoticons/js/emojis.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/emoticons/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/emoticons/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/fullpage/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/fullpage/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/fullscreen/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/fullscreen/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/help/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/help/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/hr/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/hr/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/image/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/image/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/imagetools/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/imagetools/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/importcss/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/importcss/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/insertdatetime/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/insertdatetime/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/legacyoutput/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/legacyoutput/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/link/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/link/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/lists/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/lists/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/media/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/media/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/nonbreaking/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/nonbreaking/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/noneditable/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/noneditable/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/pagebreak/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/pagebreak/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/paste/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/paste/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/preview/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/preview/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/print/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/print/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/quickbars/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/quickbars/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/save/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/save/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/searchreplace/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/searchreplace/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/spellchecker/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/spellchecker/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/tabfocus/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/tabfocus/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/table/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/table/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/template/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/template/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/textpattern/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/textpattern/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/toc/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/toc/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/visualblocks/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/visualblocks/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/visualchars/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/visualchars/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/plugins/wordcount/plugin.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/plugins/wordcount/plugin.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/content/dark/content.min.css` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/content/dark/content.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/content/default/content.min.css` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/content/default/content.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/content/document/content.min.css` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/content/document/content.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/content/writer/content.min.css` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/content/writer/content.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide/content.inline.min.css` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide/content.inline.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide/content.min.css` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide/content.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide/content.mobile.min.css` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide/content.mobile.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide/fonts/tinymce-mobile.woff` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide/fonts/tinymce-mobile.woff`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide/skin.min.css` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide/skin.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide/skin.mobile.min.css` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide/skin.mobile.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide/skin.shadowdom.min.css` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide/skin.shadowdom.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide-dark/content.inline.min.css` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide-dark/content.inline.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide-dark/content.min.css` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide-dark/content.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide-dark/content.mobile.min.css` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide-dark/content.mobile.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide-dark/fonts/tinymce-mobile.woff` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide-dark/fonts/tinymce-mobile.woff`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide-dark/skin.min.css` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide-dark/skin.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide-dark/skin.mobile.min.css` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide-dark/skin.mobile.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/skins/ui/oxide-dark/skin.shadowdom.min.css` & `django-ipghrms-main-1.5/main/static/main2/tinymce/skins/ui/oxide-dark/skin.shadowdom.min.css`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/themes/mobile/theme.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/themes/mobile/theme.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/themes/silver/theme.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/themes/silver/theme.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/tinymce.d.ts` & `django-ipghrms-main-1.5/main/static/main2/tinymce/tinymce.d.ts`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/static/main2/tinymce/tinymce.min.js` & `django-ipghrms-main-1.5/main/static/main2/tinymce/tinymce.min.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/home/home.html` & `django-ipghrms-main-1.5/main/templates/home/home.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/home/home_dep.html` & `django-ipghrms-main-1.5/main/templates/home/home_dep.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/home/home_staff.html` & `django-ipghrms-main-1.5/main/templates/home/home_staff.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/home/home_staff_bottom.html` & `django-ipghrms-main-1.5/main/templates/home/home_staff_bottom.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/home/home_staff_left.html` & `django-ipghrms-main-1.5/main/templates/home/home_staff_left.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/home/home_staff_right.html` & `django-ipghrms-main-1.5/main/templates/home/home_staff_right.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/home/home_unit.html` & `django-ipghrms-main-1.5/main/templates/home/home_unit.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/home/login.html` & `django-ipghrms-main-1.5/main/templates/home/login.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/home/logout.html` & `django-ipghrms-main-1.5/main/templates/home/logout.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main/header.html` & `django-ipghrms-main-1.5/main/templates/main/header.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main/index.html` & `django-ipghrms-main-1.5/main/templates/main/index.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main/layout.html` & `django-ipghrms-main-1.5/main/templates/main/layout.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main/sidebar.html` & `django-ipghrms-main-1.5/main/templates/main/sidebar.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main/sidebar_admin.html` & `django-ipghrms-main-1.5/main/templates/main/sidebar_admin.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main/sidebar_de.html` & `django-ipghrms-main-1.5/main/templates/main/sidebar_de.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main/sidebar_dep.html` & `django-ipghrms-main-1.5/main/templates/main/sidebar_dep.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main/sidebar_deputy.html` & `django-ipghrms-main-1.5/main/templates/main/sidebar_deputy.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main/sidebar_hr.html` & `django-ipghrms-main-1.5/main/templates/main/sidebar_hr.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main/sidebar_hr_s.html` & `django-ipghrms-main-1.5/main/templates/main/sidebar_hr_s.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main/sidebar_staff.html` & `django-ipghrms-main-1.5/main/templates/main/sidebar_staff.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main/sidebar_unit.html` & `django-ipghrms-main-1.5/main/templates/main/sidebar_unit.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main2/admin_navbar.html` & `django-ipghrms-main-1.5/main/templates/main2/admin_navbar.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main2/de_navbar.html` & `django-ipghrms-main-1.5/main/templates/main2/de_navbar.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main2/deputy_navbar.html` & `django-ipghrms-main-1.5/main/templates/main2/deputy_navbar.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main2/hr_navbar.html` & `django-ipghrms-main-1.5/main/templates/main2/hr_navbar.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main2/layout.html` & `django-ipghrms-main-1.5/main/templates/main2/layout.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main2/navbar.html` & `django-ipghrms-main-1.5/main/templates/main2/navbar.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main2/staff_navbar.html` & `django-ipghrms-main-1.5/main/templates/main2/staff_navbar.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/main2/unit_navbar.html` & `django-ipghrms-main-1.5/main/templates/main2/unit_navbar.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/notif_header/dep.html` & `django-ipghrms-main-1.5/main/templates/notif_header/dep.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/notif_header/div.html` & `django-ipghrms-main-1.5/main/templates/notif_header/div.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/notif_header/hr.html` & `django-ipghrms-main-1.5/main/templates/notif_header/hr.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/notif_header/pr.html` & `django-ipghrms-main-1.5/main/templates/notif_header/pr.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/notif_header/staff.html` & `django-ipghrms-main-1.5/main/templates/notif_header/staff.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/templates/notif_header/vice.html` & `django-ipghrms-main-1.5/main/templates/notif_header/vice.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-main-1.4/main/views.py` & `django-ipghrms-main-1.5/main/views.py`

 * *Files 19% similar despite different names*

```diff
@@ -79,7 +79,16 @@
 			'group': group, 'recplan': recplan, 'painels': painels, 'painel_check': painel_check,
 			'title': 'Painel HRMS', 'legend': 'Painel HRMS'
 		}
 		return render(request, 'home/home_unit.html', context)
 	else: 
 		context = { 'group': group, 'title': 'Painel HRMS', 'legend': 'Painel HRMS', 'painel_check':painel_check }
 		return render(request, 'home/home.html', context)
+	
+def handle_404(request, exception):
+    template_name = "home/404.html"
+    return render(request, template_name, status=404)
+
+def handle_500(request, exception):
+    template_name = "home/500.html"
+    return render(request, template_name, status=404)
+
```


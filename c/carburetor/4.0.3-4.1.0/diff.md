# Comparing `tmp/carburetor-4.0.3.tar.gz` & `tmp/carburetor-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carburetor-4.0.3.tar", last modified: Wed Mar 22 02:27:19 2023, max compression
+gzip compressed data, was "carburetor-4.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `carburetor-4.0.3.tar` & `carburetor-4.1.0.tar`

### file list

```diff
@@ -1,80 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.763463 carburetor-4.0.3/
--rw-rw-rw-   0 root         (0) root         (0)    35079 2023-03-22 02:03:59.000000 carburetor-4.0.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-03-22 02:03:59.000000 carburetor-4.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2018 2023-03-22 02:27:19.763463 carburetor-4.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1315 2023-03-22 02:03:59.000000 carburetor-4.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.759463 carburetor-4.0.3/carburetor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-22 02:27:12.000000 carburetor-4.0.3/carburetor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6779 2023-03-22 02:03:59.000000 carburetor-4.0.3/carburetor/actions.py
--rwxrwxrwx   0 root         (0) root         (0)     1137 2023-03-22 02:03:59.000000 carburetor-4.0.3/carburetor/carburetor.py
--rw-rw-rw-   0 root         (0) root         (0)      972 2023-03-22 02:03:59.000000 carburetor-4.0.3/carburetor/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.759463 carburetor-4.0.3/carburetor/desktop/
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-03-22 02:03:59.000000 carburetor-4.0.3/carburetor/desktop/carburetor.1
--rw-rw-rw-   0 root         (0) root         (0)    14735 2023-03-22 02:03:59.000000 carburetor-4.0.3/carburetor/desktop/carburetor.svg
--rw-rw-rw-   0 root         (0) root         (0)      593 2023-03-22 02:03:59.000000 carburetor-4.0.3/carburetor/desktop/org.tractor.carburetor.desktop
--rw-rw-rw-   0 root         (0) root         (0)     2924 2023-03-22 02:03:59.000000 carburetor-4.0.3/carburetor/desktop/org.tractor.carburetor.metainfo.xml
--rw-rw-rw-   0 root         (0) root         (0)     6963 2023-03-22 02:03:59.000000 carburetor-4.0.3/carburetor/handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.759463 carburetor-4.0.3/carburetor/locales/
--rw-rw-rw-   0 root         (0) root         (0)     5368 2023-03-22 02:03:59.000000 carburetor-4.0.3/carburetor/locales/carburetor.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.755463 carburetor-4.0.3/carburetor/locales/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.759463 carburetor-4.0.3/carburetor/locales/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4377 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/de/LC_MESSAGES/carburetor.mo
--rw-rw-rw-   0 root         (0) root         (0)     8051 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/de/LC_MESSAGES/carburetor.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.755463 carburetor-4.0.3/carburetor/locales/el/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.759463 carburetor-4.0.3/carburetor/locales/el/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     2558 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/el/LC_MESSAGES/carburetor.mo
--rw-rw-rw-   0 root         (0) root         (0)     8786 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/el/LC_MESSAGES/carburetor.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.755463 carburetor-4.0.3/carburetor/locales/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.759463 carburetor-4.0.3/carburetor/locales/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4401 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/es/LC_MESSAGES/carburetor.mo
--rw-rw-rw-   0 root         (0) root         (0)     7997 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/es/LC_MESSAGES/carburetor.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.755463 carburetor-4.0.3/carburetor/locales/fa/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.759463 carburetor-4.0.3/carburetor/locales/fa/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5075 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/fa/LC_MESSAGES/carburetor.mo
--rw-rw-rw-   0 root         (0) root         (0)     8774 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/fa/LC_MESSAGES/carburetor.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.755463 carburetor-4.0.3/carburetor/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.759463 carburetor-4.0.3/carburetor/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4342 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/fr/LC_MESSAGES/carburetor.mo
--rw-rw-rw-   0 root         (0) root         (0)     7895 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/fr/LC_MESSAGES/carburetor.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.755463 carburetor-4.0.3/carburetor/locales/hr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.759463 carburetor-4.0.3/carburetor/locales/hr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4436 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/hr/LC_MESSAGES/carburetor.mo
--rw-rw-rw-   0 root         (0) root         (0)     7792 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/hr/LC_MESSAGES/carburetor.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.755463 carburetor-4.0.3/carburetor/locales/nb_NO/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.759463 carburetor-4.0.3/carburetor/locales/nb_NO/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4074 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/nb_NO/LC_MESSAGES/carburetor.mo
--rw-rw-rw-   0 root         (0) root         (0)     7616 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/nb_NO/LC_MESSAGES/carburetor.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.755463 carburetor-4.0.3/carburetor/locales/pl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.759463 carburetor-4.0.3/carburetor/locales/pl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1190 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/pl/LC_MESSAGES/carburetor.mo
--rw-rw-rw-   0 root         (0) root         (0)     7654 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/pl/LC_MESSAGES/carburetor.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.755463 carburetor-4.0.3/carburetor/locales/pt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.759463 carburetor-4.0.3/carburetor/locales/pt/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4479 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/pt/LC_MESSAGES/carburetor.mo
--rw-rw-rw-   0 root         (0) root         (0)     7965 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/pt/LC_MESSAGES/carburetor.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.755463 carburetor-4.0.3/carburetor/locales/pt_BR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.759463 carburetor-4.0.3/carburetor/locales/pt_BR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3592 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/pt_BR/LC_MESSAGES/carburetor.mo
--rw-rw-rw-   0 root         (0) root         (0)     7960 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/pt_BR/LC_MESSAGES/carburetor.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.755463 carburetor-4.0.3/carburetor/locales/tr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.759463 carburetor-4.0.3/carburetor/locales/tr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4462 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/tr/LC_MESSAGES/carburetor.mo
--rw-rw-rw-   0 root         (0) root         (0)     7984 2023-03-22 02:21:42.000000 carburetor-4.0.3/carburetor/locales/tr/LC_MESSAGES/carburetor.po
--rw-rw-rw-   0 root         (0) root         (0)     3608 2023-03-22 02:03:59.000000 carburetor-4.0.3/carburetor/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.759463 carburetor-4.0.3/carburetor/ui/
--rw-rw-rw-   0 root         (0) root         (0)     1783 2023-03-22 02:03:59.000000 carburetor-4.0.3/carburetor/ui/about.ui
--rw-rw-rw-   0 root         (0) root         (0)      764 2023-03-22 02:03:59.000000 carburetor-4.0.3/carburetor/ui/actionmenu.ui
--rw-rw-rw-   0 root         (0) root         (0)     3973 2023-03-22 02:03:59.000000 carburetor-4.0.3/carburetor/ui/main.ui
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-03-22 02:03:59.000000 carburetor-4.0.3/carburetor/ui/mainmenu.ui
--rw-rw-rw-   0 root         (0) root         (0)    10683 2023-03-22 02:03:59.000000 carburetor-4.0.3/carburetor/ui/preferences.ui
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-03-22 02:03:59.000000 carburetor-4.0.3/carburetor/ui/style.css
--rw-rw-rw-   0 root         (0) root         (0)     1098 2023-03-22 02:03:59.000000 carburetor-4.0.3/carburetor/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 02:27:19.759463 carburetor-4.0.3/carburetor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2018 2023-03-22 02:27:19.000000 carburetor-4.0.3/carburetor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1819 2023-03-22 02:27:19.000000 carburetor-4.0.3/carburetor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 02:27:19.000000 carburetor-4.0.3/carburetor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-03-22 02:27:19.000000 carburetor-4.0.3/carburetor.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-22 02:27:19.000000 carburetor-4.0.3/carburetor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-03-22 02:27:19.000000 carburetor-4.0.3/carburetor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-22 02:27:19.763463 carburetor-4.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1339 2023-03-22 02:03:59.000000 carburetor-4.0.3/setup.py
+-rw-r--r--   0        0        0     1379 2023-07-26 13:02:28.076363 carburetor-4.1.0/.gitignore
+-rw-r--r--   0        0        0     1328 2023-07-26 13:02:28.076363 carburetor-4.1.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2034 2023-07-26 13:02:28.076363 carburetor-4.1.0/CHANGELOG
+-rw-r--r--   0        0        0     1041 2023-07-26 13:02:28.076363 carburetor-4.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    35079 2023-07-26 13:02:28.076363 carburetor-4.1.0/LICENSE
+-rw-r--r--   0        0        0      112 2023-07-26 13:02:28.076363 carburetor-4.1.0/MANIFEST.in
+-rw-r--r--   0        0        0     1060 2023-07-26 13:02:28.076363 carburetor-4.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 13:02:28.108363 carburetor-4.1.0/carburetor/__init__.py
+-rw-r--r--   0        0        0     6779 2023-07-26 13:02:28.076363 carburetor-4.1.0/carburetor/actions.py
+-rwxr-xr-x   0        0        0     1142 2023-07-26 13:02:28.076363 carburetor-4.1.0/carburetor/carburetor.py
+-rw-r--r--   0        0        0      972 2023-07-26 13:02:28.076363 carburetor-4.1.0/carburetor/config.py
+-rw-r--r--   0        0        0      508 2023-07-26 13:02:28.076363 carburetor-4.1.0/carburetor/desktop/carburetor.1
+-rw-r--r--   0        0        0    14735 2023-07-26 13:02:28.076363 carburetor-4.1.0/carburetor/desktop/carburetor.svg
+-rw-r--r--   0        0        0      593 2023-07-26 13:02:28.076363 carburetor-4.1.0/carburetor/desktop/io.frama.tractor.carburetor.desktop
+-rw-r--r--   0        0        0     3435 2023-07-26 13:02:28.076363 carburetor-4.1.0/carburetor/desktop/io.frama.tractor.carburetor.metainfo.xml
+-rw-r--r--   0        0        0     6963 2023-07-26 13:02:28.076363 carburetor-4.1.0/carburetor/handler.py
+-rw-r--r--   0        0        0     5283 2023-07-26 13:02:28.076363 carburetor-4.1.0/carburetor/locales/carburetor.pot
+-rw-r--r--   0        0        0     4459 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/de/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7992 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/de/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     2556 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/el/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     8714 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/el/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     4401 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/es/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7949 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/es/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     5075 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/fa/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     8676 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/fa/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     4372 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/fr/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7836 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/fr/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     4436 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/hr/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7744 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/hr/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     4253 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/nb_NO/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7599 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/nb_NO/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     4395 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/nl/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     6706 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/nl/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     3300 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/pl/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7281 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/pl/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     4479 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/pt/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7917 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/pt/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     3921 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/pt_BR/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7864 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/pt_BR/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     4462 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/tr/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7936 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/locales/tr/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     3608 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/tasks.py
+-rw-r--r--   0        0        0      994 2023-07-26 13:02:28.080363 carburetor-4.1.0/carburetor/ui.py
+-rw-r--r--   0        0        0     1903 2023-07-26 13:02:28.084363 carburetor-4.1.0/carburetor/ui/about.ui
+-rw-r--r--   0        0        0     5162 2023-07-26 13:02:28.084363 carburetor-4.1.0/carburetor/ui/main.ui
+-rw-r--r--   0        0        0    10821 2023-07-26 13:02:28.084363 carburetor-4.1.0/carburetor/ui/preferences.ui
+-rw-r--r--   0        0        0      114 2023-07-26 13:02:28.084363 carburetor-4.1.0/carburetor/ui/style.css
+-rw-r--r--   0        0        0      934 2023-07-26 13:02:28.084363 carburetor-4.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0      354 2023-07-26 13:02:28.084363 carburetor-4.1.0/update_pot
+-rw-r--r--   0        0        0     1794 1970-01-01 00:00:00.000000 carburetor-4.1.0/PKG-INFO
```

### Comparing `carburetor-4.0.3/LICENSE` & `carburetor-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `carburetor-4.0.3/carburetor/actions.py` & `carburetor-4.1.0/carburetor/actions.py`

 * *Files identical despite different names*

### Comparing `carburetor-4.0.3/carburetor/carburetor.py` & `carburetor-4.1.0/carburetor/carburetor.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 class Application(Adw.Application):
     """
     main window of carburetor
     """
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(
-            *args, application_id="org.tractor.carburetor", **kwargs
+            *args, application_id="io.frama.tractor.carburetor", **kwargs
         )
         self.window = None
         self.prefs = None
         self.about = None
 
     def do_startup(self, *args, **kwargs) -> None:
         Adw.Application.do_startup(self)
```

### Comparing `carburetor-4.0.3/carburetor/config.py` & `carburetor-4.1.0/carburetor/config.py`

 * *Files identical despite different names*

### Comparing `carburetor-4.0.3/carburetor/desktop/carburetor.svg` & `carburetor-4.1.0/carburetor/desktop/carburetor.svg`

 * *Files identical despite different names*

### Comparing `carburetor-4.0.3/carburetor/desktop/org.tractor.carburetor.desktop` & `carburetor-4.1.0/carburetor/desktop/io.frama.tractor.carburetor.desktop`

 * *Files identical despite different names*

### Comparing `carburetor-4.0.3/carburetor/desktop/org.tractor.carburetor.metainfo.xml` & `carburetor-4.1.0/carburetor/desktop/io.frama.tractor.carburetor.metainfo.xml`

 * *Files 13% similar despite different names*

#### Comparing `carburetor-4.0.3/carburetor/desktop/org.tractor.carburetor.metainfo.xml` & `carburetor-4.1.0/carburetor/desktop/io.frama.tractor.carburetor.metainfo.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <component type="desktop-application">
-  <id>org.tractor.carburetor</id>
+  <id>io.frama.tractor.carburetor</id>
   <name>Carburetor</name>
   <summary>The Onion Routing app</summary>
   <description>
     <p>A graphical settings app for tractor which is a package uses Python stem library to provide a connection through the onion proxy and sets up proxy in user session, so you don't have to mess up with TOR on your system anymore.</p>
   </description>
   <metadata_license>CC-BY-SA-4.0</metadata_license>
   <project_license>GPL-3.0-or-later</project_license>
@@ -24,47 +24,54 @@
     <internet>always</internet>
   </requires>
   <kudos>
     <kudo>HiDpiIcon</kudo>
     <kudo>ModernToolkit</kudo>
   </kudos>
   <content_rating type="oars-1.1"/>
-  <launchable type="desktop-id">org.tractor.carburetor.desktop</launchable>
+  <launchable type="desktop-id">io.frama.tractor.carburetor.desktop</launchable>
   <provides>
     <binary>carburetor</binary>
   </provides>
   <translation type="gettext">carburetor</translation>
-  <url type="homepage">https://framagit.org/tractor</url>
+  <url type="homepage">https://tractor.frama.io</url>
   <url type="vcs-browser">https://framagit.org/tractor/carburetor</url>
   <url type="bugtracker">https://framagit.org/tractor/carburetor/-/issues</url>
   <url type="contribute">https://framagit.org/tractor/carburetor/-/blob/main/CONTRIBUTING.md</url>
   <url type="translate">https://hosted.weblate.org/engage/carburetor</url>
   <screenshots>
     <screenshot type="default">
       <caption>Main Page of Carburetor in Desktop mode</caption>
       <caption xml:lang="fa">صفحهٔ اصلی کاربراتور در حالت میزکار</caption>
-      <image xml:lang="fa">https://wiki.ubuntu.ir/images/9/91/Carburetor.png</image>
+      <image type="source">https://tractor.frama.io/images/carburetor-main.png</image>
+      <image xml:lang="fa">https://tractor.frama.io/images/carburetor-main-fa.png</image>
+    </screenshot>
+    <screenshot>
+      <caption>Carburetor preferences in dark mode</caption>
+      <caption xml:lang="fa">ترجیحات کاربراتور در حالت تیره</caption>
+      <image type="source">https://tractor.frama.io/images/carburetor-preferences-general.png</image>
+      <image xml:lang="fa">https://tractor.frama.io/images/carburetor-preferences-general-fa.png</image>
     </screenshot>
     <screenshot>
       <caption>Carburetor preferences in Mobile mode</caption>
       <caption xml:lang="fa">ترجیحات کاربراتور در حالت همراه</caption>
-      <image xml:lang="fa">https://wiki.ubuntu.ir/images/c/cd/Carburetor-Settings.png</image>
+      <image type="source" xml:lang="fa">https://wiki.ubuntu.ir/images/c/cd/Carburetor-Settings.png</image>
     </screenshot>
   </screenshots>
   <branding>
     <color type="primary">#7d4698</color>
   </branding>
-  <custom>
-    <value key="Purism::form_factor">workstation</value>
-    <value key="Purism::form_factor">mobile</value>
-  </custom>
   <releases>
     <release version="4.0" date="2022-12-03" urgency="medium">
       <url>https://framagit.org/tractor/carburetor/-/releases/4.0</url>
       <artifacts>
         <artifact type="source">
           <location>https://framagit.org/tractor/carburetor/-/archive/4.0/carburetor-4.0.tar.bz2</location>
         </artifact>
       </artifacts>
     </release>
   </releases>
+  <custom>
+    <value key="Purism::form_factor">workstation</value>
+    <value key="Purism::form_factor">mobile</value>
+  </custom>
 </component>
```

### Comparing `carburetor-4.0.3/carburetor/handler.py` & `carburetor-4.1.0/carburetor/handler.py`

 * *Files identical despite different names*

### Comparing `carburetor-4.0.3/carburetor/locales/carburetor.pot` & `carburetor-4.1.0/carburetor/locales/carburetor.pot`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 04:31+0330\n"
+"POT-Creation-Date: 2023-06-18 01:44+0330\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -53,15 +53,15 @@
 msgid "_Disconnect"
 msgstr ""
 
 #: carburetor/actions.py:233
 msgid "Tractor is running"
 msgstr ""
 
-#: carburetor/config.py:37 carburetor/ui/about.ui:27 carburetor/ui/main.ui:32
+#: carburetor/config.py:37 carburetor/ui/about.ui:23 carburetor/ui/main.ui:33
 msgid "Carburetor"
 msgstr ""
 
 #: carburetor/handler.py:112
 msgid "Austria"
 msgstr ""
 
@@ -149,15 +149,15 @@
 msgid "United States"
 msgstr ""
 
 #: carburetor/handler.py:148
 msgid "Auto (Best)"
 msgstr ""
 
-#: carburetor/handler.py:238 carburetor/ui/preferences.ui:139
+#: carburetor/handler.py:238 carburetor/ui/preferences.ui:140
 msgid "None"
 msgstr ""
 
 #: carburetor/handler.py:239
 msgid "Vanilla"
 msgstr ""
 
@@ -173,130 +173,126 @@
 msgid "Tractor is connected"
 msgstr ""
 
 #: carburetor/tasks.py:140
 msgid "Tractor couldn't connect"
 msgstr ""
 
-#: carburetor/ui/about.ui:21
+#: carburetor/ui/about.ui:24
 msgid "GTK frontend for Tractor"
 msgstr ""
 
-#: carburetor/ui/about.ui:22
+#: carburetor/ui/about.ui:25
 msgid "Copyright © 2019-2023, Tractor Team"
 msgstr ""
 
-#: carburetor/ui/about.ui:30
-msgid "Source Code"
-msgstr ""
-
-#: carburetor/ui/actionmenu.ui:9
-msgid "_New ID"
+#: carburetor/ui/main.ui:32
+msgid "For Tractor"
 msgstr ""
 
-#: carburetor/ui/actionmenu.ui:13
-msgid "_Check connection"
+#: carburetor/ui/main.ui:94
+msgid "Preferences"
 msgstr ""
 
-#: carburetor/ui/actionmenu.ui:17
-msgid "_Toggle proxy on system"
+#: carburetor/ui/main.ui:98
+msgid "About Carburetor"
 msgstr ""
 
-#: carburetor/ui/mainmenu.ui:10
-msgid "Preferences"
+#: carburetor/ui/main.ui:102
+msgid "Quit"
 msgstr ""
 
-#: carburetor/ui/mainmenu.ui:14
-msgid "About Carburetor"
+#: carburetor/ui/main.ui:110
+msgid "_New ID"
 msgstr ""
 
-#: carburetor/ui/mainmenu.ui:18
-msgid "Quit"
+#: carburetor/ui/main.ui:114
+msgid "_Check connection"
 msgstr ""
 
-#: carburetor/ui/main.ui:31
-msgid "For Tractor"
+#: carburetor/ui/main.ui:118
+msgid "_Toggle proxy on system"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:27
+#: carburetor/ui/preferences.ui:28
 msgid "General"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:30
+#: carburetor/ui/preferences.ui:31
 msgid "Exit Node"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:34
+#: carburetor/ui/preferences.ui:35
 msgid "The country you want to connect from"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:35
+#: carburetor/ui/preferences.ui:36
 msgid "Exit Country"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:44
+#: carburetor/ui/preferences.ui:45
 msgid "Accept Connections"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:47
+#: carburetor/ui/preferences.ui:48
 msgid "Allow external devices to use this network"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:63
+#: carburetor/ui/preferences.ui:64
 msgid "Ports"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:66
+#: carburetor/ui/preferences.ui:67
 msgid "Socks Port"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:69
+#: carburetor/ui/preferences.ui:70
 msgid "Local port on which Tractor would be listen"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:83
+#: carburetor/ui/preferences.ui:84
 msgid "DNS Port"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:86
+#: carburetor/ui/preferences.ui:87
 msgid "Local port on which you would have an anonymous name server"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:100
+#: carburetor/ui/preferences.ui:101
 msgid "HTTP Port"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:103
+#: carburetor/ui/preferences.ui:104
 msgid "Local port on which a HTTP tunnel would be listen"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:120 carburetor/ui/preferences.ui:151
+#: carburetor/ui/preferences.ui:121 carburetor/ui/preferences.ui:152
 msgid "Bridges"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:123
+#: carburetor/ui/preferences.ui:124
 msgid "Type"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:127
+#: carburetor/ui/preferences.ui:128
 msgid "Type of bridge"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:134
+#: carburetor/ui/preferences.ui:135
 msgid "Client Transport Plugin"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:172
+#: carburetor/ui/preferences.ui:174
 msgid "_Save"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:173
+#: carburetor/ui/preferences.ui:175
 msgid "Save Bridges as a file in your local configs"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:192
+#: carburetor/ui/preferences.ui:194
 msgid "Please check the syntax of bridges"
 msgstr ""
 
-#: carburetor/ui/preferences.ui:193
+#: carburetor/ui/preferences.ui:195
 msgid "Can not save the bridges"
 msgstr ""
```

### Comparing `carburetor-4.0.3/carburetor/locales/de/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.0/carburetor/locales/de/LC_MESSAGES/carburetor.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: German <https://hosted.weblate.org/projects/carburetor/"
 "translations/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 msgid "About Carburetor"
 msgstr "Über Carburetor"
 
 msgid "Accept Connections"
 msgstr "Verbindungen Akzeptieren"
 
@@ -165,14 +165,17 @@
 
 msgid "Switzerland"
 msgstr "Schweiz"
 
 msgid "The country you want to connect from"
 msgstr "Das Land, aus dem Sie eine Verbindung herstellen möchten"
 
+msgid "Tractor couldn't connect"
+msgstr "Traktor konnte keine Verbindung herstellen"
+
 msgid "Tractor is connected"
 msgstr "Tractor ist verbunden"
 
 msgid "Tractor is not running!"
 msgstr "Tractor ist ausgeschaltet!"
 
 msgid "Tractor is running"
```

### Comparing `carburetor-4.0.3/carburetor/locales/de/LC_MESSAGES/carburetor.po` & `carburetor-4.1.0/carburetor/locales/de/LC_MESSAGES/carburetor.po`

 * *Files 6% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 # Sina Carnelious <sinacarnelious@protonmail.com>, 2021.
 # Sina Aghighi <sinaaghighi@protonmail.com>, 2021.
 # Ettore Atalan <atalanttore@googlemail.com>, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 04:31+0330\n"
-"PO-Revision-Date: 2023-03-22 02:18+0000\n"
+"POT-Creation-Date: 2023-06-18 01:44+0330\n"
+"PO-Revision-Date: 2023-05-17 09:51+0000\n"
 "Last-Translator: Danial Behzadi <dani.behzi@ubuntu.com>\n"
 "Language-Team: German <https://hosted.weblate.org/projects/carburetor/"
 "translations/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 "Generated-By: pygettext.py 1.5\n"
 
 #: carburetor/actions.py:94
 msgid "Disconnecting…"
 msgstr "Verbindung wird getrennt …"
 
 #: carburetor/actions.py:98
@@ -60,15 +60,15 @@
 msgid "_Disconnect"
 msgstr "_Trennen"
 
 #: carburetor/actions.py:233
 msgid "Tractor is running"
 msgstr "Tractor wird ausgeführt"
 
-#: carburetor/config.py:37 carburetor/ui/about.ui:27 carburetor/ui/main.ui:32
+#: carburetor/config.py:37 carburetor/ui/about.ui:23 carburetor/ui/main.ui:33
 msgid "Carburetor"
 msgstr "Carburetor"
 
 #: carburetor/handler.py:112
 msgid "Austria"
 msgstr "Österreich"
 
@@ -156,15 +156,15 @@
 msgid "United States"
 msgstr "Vereinigte Staaten"
 
 #: carburetor/handler.py:148
 msgid "Auto (Best)"
 msgstr "Automatisch (Optimal)"
 
-#: carburetor/handler.py:238 carburetor/ui/preferences.ui:139
+#: carburetor/handler.py:238 carburetor/ui/preferences.ui:140
 msgid "None"
 msgstr "Kein"
 
 #: carburetor/handler.py:239
 msgid "Vanilla"
 msgstr "Vanille"
 
@@ -177,142 +177,140 @@
 msgstr "Übersetzer Anerkennungen"
 
 #: carburetor/tasks.py:138
 msgid "Tractor is connected"
 msgstr "Tractor ist verbunden"
 
 #: carburetor/tasks.py:140
-#, fuzzy
 msgid "Tractor couldn't connect"
 msgstr "Traktor konnte keine Verbindung herstellen"
 
-#: carburetor/ui/about.ui:21
+#: carburetor/ui/about.ui:24
 msgid "GTK frontend for Tractor"
 msgstr "GTK Frontend für Tractor"
 
-#: carburetor/ui/about.ui:22
+#: carburetor/ui/about.ui:25
 msgid "Copyright © 2019-2023, Tractor Team"
 msgstr "Copyright © 2019-2023, Tractor Team"
 
-#: carburetor/ui/about.ui:30
-msgid "Source Code"
-msgstr "Quellcode"
-
-#: carburetor/ui/actionmenu.ui:9
-msgid "_New ID"
-msgstr "_Neue ID"
-
-#: carburetor/ui/actionmenu.ui:13
-msgid "_Check connection"
-msgstr "_Verbindung prüfen"
-
-#: carburetor/ui/actionmenu.ui:17
-msgid "_Toggle proxy on system"
-msgstr "Proxy auf System umschal_ten"
+#: carburetor/ui/main.ui:32
+msgid "For Tractor"
+msgstr "Für Tractor"
 
-#: carburetor/ui/mainmenu.ui:10
+#: carburetor/ui/main.ui:94
 msgid "Preferences"
 msgstr "Einstellungen"
 
-#: carburetor/ui/mainmenu.ui:14
+#: carburetor/ui/main.ui:98
 msgid "About Carburetor"
 msgstr "Über Carburetor"
 
-#: carburetor/ui/mainmenu.ui:18
+#: carburetor/ui/main.ui:102
 msgid "Quit"
 msgstr "Beenden"
 
-#: carburetor/ui/main.ui:31
-msgid "For Tractor"
-msgstr "Für Tractor"
+#: carburetor/ui/main.ui:110
+msgid "_New ID"
+msgstr "_Neue ID"
+
+#: carburetor/ui/main.ui:114
+msgid "_Check connection"
+msgstr "_Verbindung prüfen"
 
-#: carburetor/ui/preferences.ui:27
+#: carburetor/ui/main.ui:118
+msgid "_Toggle proxy on system"
+msgstr "Proxy auf System umschal_ten"
+
+#: carburetor/ui/preferences.ui:28
 msgid "General"
 msgstr "Allgemein"
 
-#: carburetor/ui/preferences.ui:30
+#: carburetor/ui/preferences.ui:31
 msgid "Exit Node"
 msgstr "Exit-Knoten"
 
-#: carburetor/ui/preferences.ui:34
+#: carburetor/ui/preferences.ui:35
 msgid "The country you want to connect from"
 msgstr "Das Land, aus dem Sie eine Verbindung herstellen möchten"
 
-#: carburetor/ui/preferences.ui:35
+#: carburetor/ui/preferences.ui:36
 msgid "Exit Country"
 msgstr "Ausgang Land"
 
-#: carburetor/ui/preferences.ui:44
+#: carburetor/ui/preferences.ui:45
 msgid "Accept Connections"
 msgstr "Verbindungen Akzeptieren"
 
-#: carburetor/ui/preferences.ui:47
+#: carburetor/ui/preferences.ui:48
 msgid "Allow external devices to use this network"
 msgstr "Ermöglichen Sie externen Geräten, dieses Netzwerk zu verwenden"
 
-#: carburetor/ui/preferences.ui:63
+#: carburetor/ui/preferences.ui:64
 msgid "Ports"
 msgstr "Ports"
 
-#: carburetor/ui/preferences.ui:66
+#: carburetor/ui/preferences.ui:67
 msgid "Socks Port"
 msgstr "Socks-Port"
 
-#: carburetor/ui/preferences.ui:69
+#: carburetor/ui/preferences.ui:70
 msgid "Local port on which Tractor would be listen"
 msgstr "Lokaler Port, auf dem Tractor lauschen soll"
 
-#: carburetor/ui/preferences.ui:83
+#: carburetor/ui/preferences.ui:84
 msgid "DNS Port"
 msgstr "DNS-Port"
 
-#: carburetor/ui/preferences.ui:86
+#: carburetor/ui/preferences.ui:87
 msgid "Local port on which you would have an anonymous name server"
 msgstr "Lokaler Port, auf dem der anonyme DNS-Server läuft"
 
-#: carburetor/ui/preferences.ui:100
+#: carburetor/ui/preferences.ui:101
 msgid "HTTP Port"
 msgstr "HTTP-Port"
 
-#: carburetor/ui/preferences.ui:103
+#: carburetor/ui/preferences.ui:104
 msgid "Local port on which a HTTP tunnel would be listen"
 msgstr "Lokaler Port, an dem ein HTTP-Tunnel abgehört werden soll"
 
-#: carburetor/ui/preferences.ui:120 carburetor/ui/preferences.ui:151
+#: carburetor/ui/preferences.ui:121 carburetor/ui/preferences.ui:152
 msgid "Bridges"
 msgstr "Brücken"
 
-#: carburetor/ui/preferences.ui:123
+#: carburetor/ui/preferences.ui:124
 msgid "Type"
 msgstr "Typ"
 
-#: carburetor/ui/preferences.ui:127
+#: carburetor/ui/preferences.ui:128
 msgid "Type of bridge"
 msgstr "Art der Brücke"
 
-#: carburetor/ui/preferences.ui:134
+#: carburetor/ui/preferences.ui:135
 msgid "Client Transport Plugin"
 msgstr "Klient Transport Plugin"
 
-#: carburetor/ui/preferences.ui:172
+#: carburetor/ui/preferences.ui:174
 msgid "_Save"
 msgstr "_Speichern"
 
-#: carburetor/ui/preferences.ui:173
+#: carburetor/ui/preferences.ui:175
 msgid "Save Bridges as a file in your local configs"
 msgstr "Speichern Sie Bridges als Datei in Ihren lokalen Konfigurationen"
 
-#: carburetor/ui/preferences.ui:192
+#: carburetor/ui/preferences.ui:194
 msgid "Please check the syntax of bridges"
 msgstr "Bitte Syntax der Bridges prüfen"
 
-#: carburetor/ui/preferences.ui:193
+#: carburetor/ui/preferences.ui:195
 msgid "Can not save the bridges"
 msgstr "Die Bridges konnten nicht gespeichert werden"
 
+#~ msgid "Source Code"
+#~ msgstr "Quellcode"
+
 #~ msgid "_Cancel"
 #~ msgstr "_Abbrechen"
 
 #~ msgid "Use obfs4proxy"
 #~ msgstr "Benutzen obfs4proxy"
 
 #~ msgid "Please specify the plugin executable file"
```

### Comparing `carburetor-4.0.3/carburetor/locales/el/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.0/carburetor/locales/el/LC_MESSAGES/carburetor.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Greek <https://hosted.weblate.org/projects/carburetor/"
 "translations/el/>\n"
 "Language: el\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 msgid "Accept Connections"
 msgstr "Αποδοχή σύνδεσης"
 
 msgid "Allow external devices to use this network"
 msgstr ""
 "Πότε επιτρέπεται ή όχι σε εξωτερικές συσκευές να χρησιμοποιούν αυτό το δίκτυο"
```

### Comparing `carburetor-4.0.3/carburetor/locales/el/LC_MESSAGES/carburetor.po` & `carburetor-4.1.0/carburetor/locales/el/LC_MESSAGES/carburetor.po`

 * *Files 10% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 # Copyright (C) YEAR ORGANIZATION
 # george k <norhorn@gmail.com>, 2020.
 # Danial Behzadi <dani.behzi@ubuntu.com>, 2020, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 04:31+0330\n"
-"PO-Revision-Date: 2023-03-22 02:19+0000\n"
-"Last-Translator: Danial Behzadi <dani.behzi@ubuntu.com>\n"
+"POT-Creation-Date: 2023-06-18 01:44+0330\n"
+"PO-Revision-Date: 2023-04-23 10:46+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Greek <https://hosted.weblate.org/projects/carburetor/"
 "translations/el/>\n"
 "Language: el\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 "Generated-By: pygettext.py 1.5\n"
 
 #: carburetor/actions.py:94
 #, fuzzy
 msgid "Disconnecting…"
 msgstr "Αποσύνδεση…"
 
 #: carburetor/actions.py:98
 #, fuzzy
 msgid "Connecting…"
-msgstr "Γίνεται σύνδεση…"
+msgstr "Σύνδεση…"
 
 #: carburetor/actions.py:110
 msgid "You have a new identity!"
 msgstr "Έχετε νέα ταυτότητα!"
 
 #: carburetor/actions.py:112
 #, fuzzy
@@ -52,27 +52,27 @@
 #, fuzzy
 msgid "Tractor is stopped"
 msgstr "Το τρακτέρ έχει σταματήσει"
 
 #: carburetor/actions.py:220
 #, fuzzy
 msgid "Running"
-msgstr "Τρέξιμο"
+msgstr "Τρέχων"
 
 #: carburetor/actions.py:223
 #, fuzzy
 msgid "_Disconnect"
 msgstr "Α_ποσύνδεση"
 
 #: carburetor/actions.py:233
 #, fuzzy
 msgid "Tractor is running"
 msgstr "Το τρακτέρ τρέχει"
 
-#: carburetor/config.py:37 carburetor/ui/about.ui:27 carburetor/ui/main.ui:32
+#: carburetor/config.py:37 carburetor/ui/about.ui:23 carburetor/ui/main.ui:33
 msgid "Carburetor"
 msgstr "Carburetor"
 
 #: carburetor/handler.py:112
 msgid "Austria"
 msgstr "Αυστρία"
 
@@ -160,15 +160,15 @@
 msgid "United States"
 msgstr "Ηνωμένες Πολιτείες"
 
 #: carburetor/handler.py:148
 msgid "Auto (Best)"
 msgstr "Αυτόματο (καλύτερο)"
 
-#: carburetor/handler.py:238 carburetor/ui/preferences.ui:139
+#: carburetor/handler.py:238 carburetor/ui/preferences.ui:140
 #, fuzzy
 msgid "None"
 msgstr "Κανένα"
 
 #: carburetor/handler.py:239
 #, fuzzy
 msgid "Vanilla"
@@ -190,161 +190,160 @@
 msgstr "Το τρακτέρ είναι συνδεδεμένο"
 
 #: carburetor/tasks.py:140
 #, fuzzy
 msgid "Tractor couldn't connect"
 msgstr "Το τρακτέρ δεν μπορούσε να συνδεθεί"
 
-#: carburetor/ui/about.ui:21
+#: carburetor/ui/about.ui:24
 #, fuzzy
 msgid "GTK frontend for Tractor"
 msgstr "GTK frontend για τρακτέρ"
 
-#: carburetor/ui/about.ui:22
+#: carburetor/ui/about.ui:25
 msgid "Copyright © 2019-2023, Tractor Team"
 msgstr "Πνευματικά δικαιώματα © 2019-2023, Tractor Team"
 
-#: carburetor/ui/about.ui:30
+#: carburetor/ui/main.ui:32
 #, fuzzy
-msgid "Source Code"
-msgstr "Πηγαίος κώδικας"
-
-#: carburetor/ui/actionmenu.ui:9
-msgid "_New ID"
-msgstr "_Νέο ID"
-
-#: carburetor/ui/actionmenu.ui:13
-#, fuzzy
-msgid "_Check connection"
-msgstr "_Έλεγχος σύνδεσης"
-
-#: carburetor/ui/actionmenu.ui:17
-#, fuzzy
-msgid "_Toggle proxy on system"
-msgstr "_Εναλλαγή διακομιστή μεσολάβησης στο σύστημα"
+msgid "For Tractor"
+msgstr "Για τρακτέρ"
 
-#: carburetor/ui/mainmenu.ui:10
+#: carburetor/ui/main.ui:94
 #, fuzzy
 msgid "Preferences"
 msgstr "Προτιμήσεις"
 
-#: carburetor/ui/mainmenu.ui:14
+#: carburetor/ui/main.ui:98
 #, fuzzy
 msgid "About Carburetor"
 msgstr "Σχετικά με το καρμπυρατέρ"
 
-#: carburetor/ui/mainmenu.ui:18
+#: carburetor/ui/main.ui:102
 #, fuzzy
 msgid "Quit"
 msgstr "Έξοδος"
 
-#: carburetor/ui/main.ui:31
+#: carburetor/ui/main.ui:110
+msgid "_New ID"
+msgstr "_Νέο ID"
+
+#: carburetor/ui/main.ui:114
 #, fuzzy
-msgid "For Tractor"
-msgstr "Για τρακτέρ"
+msgid "_Check connection"
+msgstr "_Έλεγχος σύνδεσης"
+
+#: carburetor/ui/main.ui:118
+#, fuzzy
+msgid "_Toggle proxy on system"
+msgstr "_Εναλλαγή διακομιστή μεσολάβησης στο σύστημα"
 
-#: carburetor/ui/preferences.ui:27
+#: carburetor/ui/preferences.ui:28
 #, fuzzy
 msgid "General"
 msgstr "Γενικά"
 
-#: carburetor/ui/preferences.ui:30
+#: carburetor/ui/preferences.ui:31
 msgid "Exit Node"
 msgstr "Κόμβος εξόδου"
 
-#: carburetor/ui/preferences.ui:34
+#: carburetor/ui/preferences.ui:35
 msgid "The country you want to connect from"
 msgstr "Η χώρα από την οποία θέλετε να συνδεθείτε"
 
-#: carburetor/ui/preferences.ui:35
+#: carburetor/ui/preferences.ui:36
 #, fuzzy
 msgid "Exit Country"
 msgstr "Έξοδος από τη χώρα"
 
-#: carburetor/ui/preferences.ui:44
+#: carburetor/ui/preferences.ui:45
 msgid "Accept Connections"
 msgstr "Αποδοχή σύνδεσης"
 
-#: carburetor/ui/preferences.ui:47
+#: carburetor/ui/preferences.ui:48
 msgid "Allow external devices to use this network"
 msgstr ""
 "Πότε επιτρέπεται ή όχι σε εξωτερικές συσκευές να χρησιμοποιούν αυτό το δίκτυο"
 
-#: carburetor/ui/preferences.ui:63
+#: carburetor/ui/preferences.ui:64
 #, fuzzy
 msgid "Ports"
 msgstr "Θύρες"
 
-#: carburetor/ui/preferences.ui:66
+#: carburetor/ui/preferences.ui:67
 msgid "Socks Port"
 msgstr "θύρα Socks"
 
-#: carburetor/ui/preferences.ui:69
+#: carburetor/ui/preferences.ui:70
 #, fuzzy
 msgid "Local port on which Tractor would be listen"
 msgstr "Τοπικό λιμάνι στο οποίο θα ακούτε το Tractor"
 
-#: carburetor/ui/preferences.ui:83
+#: carburetor/ui/preferences.ui:84
 msgid "DNS Port"
 msgstr "θύρα DNS"
 
-#: carburetor/ui/preferences.ui:86
+#: carburetor/ui/preferences.ui:87
 #, fuzzy
 msgid "Local port on which you would have an anonymous name server"
 msgstr "Τοπική θύρα στην οποία θα έχετε έναν ανώνυμο διακομιστή ονομάτων"
 
-#: carburetor/ui/preferences.ui:100
+#: carburetor/ui/preferences.ui:101
 msgid "HTTP Port"
 msgstr "θύρα HTTP"
 
-#: carburetor/ui/preferences.ui:103
+#: carburetor/ui/preferences.ui:104
 #, fuzzy
 msgid "Local port on which a HTTP tunnel would be listen"
 msgstr "Τοπική θύρα στην οποία θα ακούγεται ένα τούνελ HTTP"
 
-#: carburetor/ui/preferences.ui:120 carburetor/ui/preferences.ui:151
+#: carburetor/ui/preferences.ui:121 carburetor/ui/preferences.ui:152
 #, fuzzy
 msgid "Bridges"
 msgstr "Γέφυρες"
 
-#: carburetor/ui/preferences.ui:123
+#: carburetor/ui/preferences.ui:124
 #, fuzzy
 msgid "Type"
 msgstr "Τύπος"
 
-#: carburetor/ui/preferences.ui:127
+#: carburetor/ui/preferences.ui:128
 #, fuzzy
 msgid "Type of bridge"
 msgstr "Τύπος γέφυρας"
 
-#: carburetor/ui/preferences.ui:134
+#: carburetor/ui/preferences.ui:135
 #, fuzzy
 msgid "Client Transport Plugin"
-msgstr "Προσθήκη μεταφοράς πελάτη"
+msgstr "Προσθήκη μεταφοράς πελατών"
 
-#: carburetor/ui/preferences.ui:172
+#: carburetor/ui/preferences.ui:174
 msgid "_Save"
 msgstr "_Αποθήκευση"
 
-#: carburetor/ui/preferences.ui:173
+#: carburetor/ui/preferences.ui:175
 #, fuzzy
 msgid "Save Bridges as a file in your local configs"
 msgstr "Αποθηκεύστε τα Bridges ως αρχείο στις τοπικές ρυθμίσεις παραμέτρων σας"
 
-#: carburetor/ui/preferences.ui:192
+#: carburetor/ui/preferences.ui:194
 #, fuzzy
 msgid "Please check the syntax of bridges"
 msgstr "Ελέγξτε τη σύνταξη των γεφυρών"
 
-#: carburetor/ui/preferences.ui:193
+#: carburetor/ui/preferences.ui:195
 #, fuzzy
 msgid "Can not save the bridges"
 msgstr "Δεν μπορώ να σώσω τις γέφυρες"
 
 #, fuzzy
+#~ msgid "Source Code"
+#~ msgstr "Πηγαίος κώδικας"
+
+#, fuzzy
 #~ msgid "_Cancel"
 #~ msgstr "Γαλλία"
 
 #, fuzzy
 #~ msgid "Use obfs4proxy"
 #~ msgstr "Αφαίρεση διακομιστή μεσολάβησης"
```

### Comparing `carburetor-4.0.3/carburetor/locales/es/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.0/carburetor/locales/es/LC_MESSAGES/carburetor.mo`

 * *Files identical despite different names*

### Comparing `carburetor-4.0.3/carburetor/locales/es/LC_MESSAGES/carburetor.po` & `carburetor-4.1.0/carburetor/locales/es/LC_MESSAGES/carburetor.po`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Jose David M <jquintana202020@gmail.com>, 2021.
 # badlop <badlop@process-one.net>, 2021.
 # gallegonovato <fran-carro@hotmail.es>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 04:31+0330\n"
+"POT-Creation-Date: 2023-06-18 01:44+0330\n"
 "PO-Revision-Date: 2023-03-22 02:19+0000\n"
 "Last-Translator: Danial Behzadi <dani.behzi@ubuntu.com>\n"
 "Language-Team: Spanish <https://hosted.weblate.org/projects/carburetor/"
 "translations/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -59,15 +59,15 @@
 msgid "_Disconnect"
 msgstr "_Desconectar"
 
 #: carburetor/actions.py:233
 msgid "Tractor is running"
 msgstr "Tractor está ejecutándose"
 
-#: carburetor/config.py:37 carburetor/ui/about.ui:27 carburetor/ui/main.ui:32
+#: carburetor/config.py:37 carburetor/ui/about.ui:23 carburetor/ui/main.ui:33
 msgid "Carburetor"
 msgstr "Carburetor"
 
 #: carburetor/handler.py:112
 msgid "Austria"
 msgstr "Austria"
 
@@ -155,15 +155,15 @@
 msgid "United States"
 msgstr "Estados Unidos"
 
 #: carburetor/handler.py:148
 msgid "Auto (Best)"
 msgstr "Automático (el mejor)"
 
-#: carburetor/handler.py:238 carburetor/ui/preferences.ui:139
+#: carburetor/handler.py:238 carburetor/ui/preferences.ui:140
 msgid "None"
 msgstr "Ninguno"
 
 #: carburetor/handler.py:239
 msgid "Vanilla"
 msgstr "Vanilla Tor"
 
@@ -179,139 +179,138 @@
 msgid "Tractor is connected"
 msgstr "Tractor está conectado"
 
 #: carburetor/tasks.py:140
 msgid "Tractor couldn't connect"
 msgstr "Tractor no pudo conectarse"
 
-#: carburetor/ui/about.ui:21
+#: carburetor/ui/about.ui:24
 msgid "GTK frontend for Tractor"
 msgstr "Interfaz GTK de Tractor"
 
-#: carburetor/ui/about.ui:22
+#: carburetor/ui/about.ui:25
 msgid "Copyright © 2019-2023, Tractor Team"
 msgstr "Copyright © 2019-2023, Tractor Team"
 
-#: carburetor/ui/about.ui:30
-msgid "Source Code"
-msgstr "Código Fuente"
-
-#: carburetor/ui/actionmenu.ui:9
-msgid "_New ID"
-msgstr "_Identidad nueva"
-
-#: carburetor/ui/actionmenu.ui:13
-msgid "_Check connection"
-msgstr "Verificar conexión"
-
-#: carburetor/ui/actionmenu.ui:17
-msgid "_Toggle proxy on system"
-msgstr "_Alternar el proxy en el sistema"
+#: carburetor/ui/main.ui:32
+msgid "For Tractor"
+msgstr "Para Tractor"
 
-#: carburetor/ui/mainmenu.ui:10
+#: carburetor/ui/main.ui:94
 msgid "Preferences"
 msgstr "Preferencias"
 
-#: carburetor/ui/mainmenu.ui:14
+#: carburetor/ui/main.ui:98
 msgid "About Carburetor"
 msgstr "Acerca de Carburetor"
 
-#: carburetor/ui/mainmenu.ui:18
+#: carburetor/ui/main.ui:102
 msgid "Quit"
 msgstr "Salir"
 
-#: carburetor/ui/main.ui:31
-msgid "For Tractor"
-msgstr "Para Tractor"
+#: carburetor/ui/main.ui:110
+msgid "_New ID"
+msgstr "_Identidad nueva"
+
+#: carburetor/ui/main.ui:114
+msgid "_Check connection"
+msgstr "Verificar conexión"
 
-#: carburetor/ui/preferences.ui:27
+#: carburetor/ui/main.ui:118
+msgid "_Toggle proxy on system"
+msgstr "_Alternar el proxy en el sistema"
+
+#: carburetor/ui/preferences.ui:28
 msgid "General"
 msgstr "General"
 
-#: carburetor/ui/preferences.ui:30
+#: carburetor/ui/preferences.ui:31
 msgid "Exit Node"
 msgstr "Nodo de salida"
 
-#: carburetor/ui/preferences.ui:34
+#: carburetor/ui/preferences.ui:35
 msgid "The country you want to connect from"
 msgstr "El país desde el cual quiere conectarse"
 
-#: carburetor/ui/preferences.ui:35
+#: carburetor/ui/preferences.ui:36
 msgid "Exit Country"
 msgstr "Salir País"
 
-#: carburetor/ui/preferences.ui:44
+#: carburetor/ui/preferences.ui:45
 msgid "Accept Connections"
 msgstr "Aceptar conexión"
 
-#: carburetor/ui/preferences.ui:47
+#: carburetor/ui/preferences.ui:48
 msgid "Allow external devices to use this network"
 msgstr ""
 "Indica si debe permitirse a los dispositivos externos el uso de esta red"
 
-#: carburetor/ui/preferences.ui:63
+#: carburetor/ui/preferences.ui:64
 msgid "Ports"
 msgstr "Puertos"
 
-#: carburetor/ui/preferences.ui:66
+#: carburetor/ui/preferences.ui:67
 msgid "Socks Port"
 msgstr "Puerto de SOCKS"
 
-#: carburetor/ui/preferences.ui:69
+#: carburetor/ui/preferences.ui:70
 msgid "Local port on which Tractor would be listen"
 msgstr "Puerto local en el que Tractor estaría escuchando"
 
-#: carburetor/ui/preferences.ui:83
+#: carburetor/ui/preferences.ui:84
 msgid "DNS Port"
 msgstr "Puerto de DNS"
 
-#: carburetor/ui/preferences.ui:86
+#: carburetor/ui/preferences.ui:87
 msgid "Local port on which you would have an anonymous name server"
 msgstr "Puerto local en el cual tendrías un servidor de nombre anónimo"
 
-#: carburetor/ui/preferences.ui:100
+#: carburetor/ui/preferences.ui:101
 msgid "HTTP Port"
 msgstr "Puerto de HTTP"
 
-#: carburetor/ui/preferences.ui:103
+#: carburetor/ui/preferences.ui:104
 msgid "Local port on which a HTTP tunnel would be listen"
 msgstr "El puerto local en el que se escucharía un túnel HTTP"
 
-#: carburetor/ui/preferences.ui:120 carburetor/ui/preferences.ui:151
+#: carburetor/ui/preferences.ui:121 carburetor/ui/preferences.ui:152
 msgid "Bridges"
 msgstr "Puentes"
 
-#: carburetor/ui/preferences.ui:123
+#: carburetor/ui/preferences.ui:124
 msgid "Type"
 msgstr "Tipo"
 
-#: carburetor/ui/preferences.ui:127
+#: carburetor/ui/preferences.ui:128
 msgid "Type of bridge"
 msgstr "Tipo de puente"
 
-#: carburetor/ui/preferences.ui:134
+#: carburetor/ui/preferences.ui:135
 msgid "Client Transport Plugin"
 msgstr "Plugin de transporte Cliente"
 
-#: carburetor/ui/preferences.ui:172
+#: carburetor/ui/preferences.ui:174
 msgid "_Save"
 msgstr "_Guardar"
 
-#: carburetor/ui/preferences.ui:173
+#: carburetor/ui/preferences.ui:175
 msgid "Save Bridges as a file in your local configs"
 msgstr "Guarde Bridges como un archivo en sus configuraciones locales"
 
-#: carburetor/ui/preferences.ui:192
+#: carburetor/ui/preferences.ui:194
 msgid "Please check the syntax of bridges"
 msgstr "Compruebe la sintaxis de los puentes"
 
-#: carburetor/ui/preferences.ui:193
+#: carburetor/ui/preferences.ui:195
 msgid "Can not save the bridges"
 msgstr "No se pueden guardar los puentes"
 
+#~ msgid "Source Code"
+#~ msgstr "Código Fuente"
+
 #~ msgid "_Cancel"
 #~ msgstr "_Cancelar"
 
 #~ msgid "Use obfs4proxy"
 #~ msgstr "Usar obfs4proxy"
 
 #~ msgid "Please specify the plugin executable file"
```

### Comparing `carburetor-4.0.3/carburetor/locales/fa/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.0/carburetor/locales/fa/LC_MESSAGES/carburetor.mo`

 * *Files identical despite different names*

### Comparing `carburetor-4.0.3/carburetor/locales/fa/LC_MESSAGES/carburetor.po` & `carburetor-4.1.0/carburetor/locales/fa/LC_MESSAGES/carburetor.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Carburetor Translation Project
 # Copyright (C) 2018 Tractor Team
 # Danial Behzadi <dani.behzi@ubuntu.com>, 2018, 2019, 2020, 2021, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Carburetor\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 04:31+0330\n"
+"POT-Creation-Date: 2023-06-18 01:44+0330\n"
 "PO-Revision-Date: 2023-03-22 02:19+0000\n"
 "Last-Translator: Danial Behzadi <dani.behzi@ubuntu.com>\n"
 "Language-Team: Persian <https://hosted.weblate.org/projects/carburetor/"
 "translations/fa/>\n"
 "Language: fa\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -55,16 +55,15 @@
 msgid "_Disconnect"
 msgstr "_قطع شدن"
 
 #: carburetor/actions.py:233
 msgid "Tractor is running"
 msgstr "تراکتور در حال اجراست"
 
-#: carburetor/config.py:37 carburetor/ui/about.ui:27 carburetor/ui/main.ui:32
-#: carburetor/config.py:36
+#: carburetor/config.py:37 carburetor/ui/about.ui:23 carburetor/ui/main.ui:33
 msgid "Carburetor"
 msgstr "کاربراتور"
 
 #: carburetor/handler.py:112
 msgid "Austria"
 msgstr "اتریش"
 
@@ -152,15 +151,15 @@
 msgid "United States"
 msgstr "آمریکا"
 
 #: carburetor/handler.py:148
 msgid "Auto (Best)"
 msgstr "خودکار (بهترین)"
 
-#: carburetor/handler.py:238 carburetor/ui/preferences.ui:139
+#: carburetor/handler.py:238 carburetor/ui/preferences.ui:140
 msgid "None"
 msgstr "هیچ‌کدام"
 
 #: carburetor/handler.py:239
 msgid "Vanilla"
 msgstr "وانیلی"
 
@@ -176,141 +175,139 @@
 msgid "Tractor is connected"
 msgstr "تراکتور وصل است"
 
 #: carburetor/tasks.py:140
 msgid "Tractor couldn't connect"
 msgstr "تراکتور نتوانست وصل شود"
 
-#: carburetor/ui/about.ui:21
+#: carburetor/ui/about.ui:24
 msgid "GTK frontend for Tractor"
 msgstr "پیشانهٔ GTK برای تراکتور"
 
-#: carburetor/ui/about.ui:22
+#: carburetor/ui/about.ui:25
 msgid "Copyright © 2019-2023, Tractor Team"
 msgstr "حق رونوشت © ۱۳۹۸-۱۴۰۲، تیم تراکتور"
 
-#: carburetor/ui/about.ui:30
-msgid "Source Code"
-msgstr "کد مبدأ"
-
-#: carburetor/ui/actionmenu.ui:9
-msgid "_New ID"
-msgstr "_هویت جدید"
-
-#: carburetor/ui/actionmenu.ui:13
-msgid "_Check connection"
-msgstr "_بررسی اتّصال"
-
-#: carburetor/ui/actionmenu.ui:17
-msgid "_Toggle proxy on system"
-msgstr "_تغییر وضعیت پیشکار روی سامانه"
+#: carburetor/ui/main.ui:32
+msgid "For Tractor"
+msgstr "برای تراکتور"
 
-#: carburetor/ui/mainmenu.ui:10
+#: carburetor/ui/main.ui:94
 msgid "Preferences"
 msgstr "ترجیحات"
 
-#: carburetor/ui/mainmenu.ui:14
+#: carburetor/ui/main.ui:98
 msgid "About Carburetor"
 msgstr "دربارهٔ کاربراتور"
 
-#: carburetor/ui/mainmenu.ui:18
+#: carburetor/ui/main.ui:102
 msgid "Quit"
 msgstr "خروج"
 
-#: carburetor/ui/main.ui:31
-msgid "For Tractor"
-msgstr "برای تراکتور"
+#: carburetor/ui/main.ui:110
+msgid "_New ID"
+msgstr "_هویت جدید"
+
+#: carburetor/ui/main.ui:114
+msgid "_Check connection"
+msgstr "_بررسی اتّصال"
+
+#: carburetor/ui/main.ui:118
+msgid "_Toggle proxy on system"
+msgstr "_تغییر وضعیت پیشکار روی سامانه"
 
-#: carburetor/ui/preferences.ui:27
+#: carburetor/ui/preferences.ui:28
 msgid "General"
 msgstr "عمومی"
 
-#: carburetor/ui/preferences.ui:30
+#: carburetor/ui/preferences.ui:31
 msgid "Exit Node"
 msgstr "گره خروجی"
 
-#: carburetor/ui/preferences.ui:34
+#: carburetor/ui/preferences.ui:35
 msgid "The country you want to connect from"
 msgstr "کشوری که می‌خواهید از آن وصل شوید"
 
-#: carburetor/ui/preferences.ui:35
+#: carburetor/ui/preferences.ui:36
 msgid "Exit Country"
 msgstr "کشور خروجی"
 
-#: carburetor/ui/preferences.ui:44
+#: carburetor/ui/preferences.ui:45
 msgid "Accept Connections"
 msgstr "پذیرش اتّصال‌ها"
 
-#: carburetor/ui/preferences.ui:47
+#: carburetor/ui/preferences.ui:48
 msgid "Allow external devices to use this network"
 msgstr "اجازه به افزاره‌های خارجی برای استفاده از این شبکه"
 
-#: carburetor/ui/preferences.ui:63
+#: carburetor/ui/preferences.ui:64
 msgid "Ports"
 msgstr "درگاه‌ها"
 
-#: carburetor/ui/preferences.ui:66
+#: carburetor/ui/preferences.ui:67
 msgid "Socks Port"
 msgstr "درگاه ساکس"
 
-#: carburetor/ui/preferences.ui:69
+#: carburetor/ui/preferences.ui:70
 msgid "Local port on which Tractor would be listen"
 msgstr "درگاه محلّی برای شنود تراکتور"
 
-#: carburetor/ui/preferences.ui:83
+#: carburetor/ui/preferences.ui:84
 msgid "DNS Port"
 msgstr "درگاه ساناد"
 
-#: carburetor/ui/preferences.ui:86
+#: carburetor/ui/preferences.ui:87
 msgid "Local port on which you would have an anonymous name server"
 msgstr "درگاه محلّی برای ساناد ناشناس"
 
-#: carburetor/ui/preferences.ui:100
+#: carburetor/ui/preferences.ui:101
 msgid "HTTP Port"
 msgstr "درگاه HTTP"
 
-#: carburetor/ui/preferences.ui:103
+#: carburetor/ui/preferences.ui:104
 msgid "Local port on which a HTTP tunnel would be listen"
 msgstr "درگاه محلّی برای شنود یک تونل HTTP"
 
-#: carburetor/ui/preferences.ui:120 carburetor/ui/preferences.ui:151
+#: carburetor/ui/preferences.ui:121 carburetor/ui/preferences.ui:152
 msgid "Bridges"
 msgstr "پل‌ها"
 
-#: carburetor/ui/preferences.ui:123
+#: carburetor/ui/preferences.ui:124
 msgid "Type"
 msgstr "گونه"
 
-#: carburetor/ui/preferences.ui:127
+#: carburetor/ui/preferences.ui:128
 msgid "Type of bridge"
 msgstr "گونهٔ پل"
 
-#: carburetor/ui/preferences.ui:134
+#: carburetor/ui/preferences.ui:135
 msgid "Client Transport Plugin"
 msgstr "افزایهٔ جابه‌جایی کارخواه"
 
-#: carburetor/ui/preferences.ui:172
+#: carburetor/ui/preferences.ui:174
 msgid "_Save"
 msgstr "_ذخیره"
 
-#: carburetor/ui/preferences.ui:173
+#: carburetor/ui/preferences.ui:175
 msgid "Save Bridges as a file in your local configs"
 msgstr "ذخیرهٔ پل‌ها به شکل یک پرونده در پیکربندی‌های شخصیتان"
 
-#: carburetor/ui/preferences.ui:192
+#: carburetor/ui/preferences.ui:194
 msgid "Please check the syntax of bridges"
 msgstr "لطفاً ترکیب پل‌ها را بررسی کنید"
 
-#: carburetor/ui/preferences.ui:193
+#: carburetor/ui/preferences.ui:195
 msgid "Can not save the bridges"
 msgstr "نمی‌توان پل‌ها را ذخیره کرد"
 
-#: carburetor/ui/about.ui:22
-msgid "Copyright © 2019-2022, Tractor Team"
-msgstr "حق رونوشت © ۱۳۹۸-۱۴۰۲، تیم تراکتور"
+#~ msgid "Source Code"
+#~ msgstr "کد مبدأ"
+
+#~ msgid "Copyright © 2019-2022, Tractor Team"
+#~ msgstr "حق رونوشت © ۱۳۹۸-۱۴۰۲، تیم تراکتور"
 
 #~ msgid "none"
 #~ msgstr "هیچ‌کدام"
 
 #~ msgid "vanilla"
 #~ msgstr "وانیلی"
```

### Comparing `carburetor-4.0.3/carburetor/locales/fr/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.0/carburetor/locales/fr/LC_MESSAGES/carburetor.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: French <https://hosted.weblate.org/projects/carburetor/"
 "translations/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 msgid "About Carburetor"
 msgstr "À propos de Carburetor"
 
 msgid "Accept Connections"
 msgstr "Accepter des connexions"
 
@@ -195,14 +195,17 @@
 
 msgid "United Kingdom"
 msgstr "Royaume-Uni"
 
 msgid "United States"
 msgstr "États-Unis"
 
+msgid "Vanilla"
+msgstr "Vanille"
+
 msgid "You have a new identity!"
 msgstr "Vous avez une nouvelle identité !"
 
 msgid "_Check connection"
 msgstr "_Vérifier la connexion"
 
 msgid "_Connect"
```

### Comparing `carburetor-4.0.3/carburetor/locales/fr/LC_MESSAGES/carburetor.po` & `carburetor-4.1.0/carburetor/locales/fr/LC_MESSAGES/carburetor.po`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 # J. Lavoie <j.lavoie@net-c.ca>, 2020, 2021.
 # rene-coty <irenee.thirion@e.email>, 2023.
 # "J. Lavoie" <j.lavoie@net-c.ca>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 04:31+0330\n"
-"PO-Revision-Date: 2023-03-22 02:20+0000\n"
+"POT-Creation-Date: 2023-06-18 01:44+0330\n"
+"PO-Revision-Date: 2023-04-23 12:06+0000\n"
 "Last-Translator: Danial Behzadi <dani.behzi@ubuntu.com>\n"
 "Language-Team: French <https://hosted.weblate.org/projects/carburetor/"
 "translations/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 "Generated-By: pygettext.py 1.5\n"
 
 #: carburetor/actions.py:94
 msgid "Disconnecting…"
 msgstr "Déconnexion…"
 
 #: carburetor/actions.py:98
@@ -58,15 +58,15 @@
 msgid "_Disconnect"
 msgstr "_Déconnecter"
 
 #: carburetor/actions.py:233
 msgid "Tractor is running"
 msgstr "Tractor est en marche"
 
-#: carburetor/config.py:37 carburetor/ui/about.ui:27 carburetor/ui/main.ui:32
+#: carburetor/config.py:37 carburetor/ui/about.ui:23 carburetor/ui/main.ui:33
 msgid "Carburetor"
 msgstr "Carburetor"
 
 #: carburetor/handler.py:112
 msgid "Austria"
 msgstr "Autriche"
 
@@ -154,20 +154,19 @@
 msgid "United States"
 msgstr "États-Unis"
 
 #: carburetor/handler.py:148
 msgid "Auto (Best)"
 msgstr "Auto (recommandé)"
 
-#: carburetor/handler.py:238 carburetor/ui/preferences.ui:139
+#: carburetor/handler.py:238 carburetor/ui/preferences.ui:140
 msgid "None"
 msgstr "Aucun"
 
 #: carburetor/handler.py:239
-#, fuzzy
 msgid "Vanilla"
 msgstr "Vanille"
 
 #: carburetor/handler.py:240
 msgid "Obfuscated"
 msgstr "Obfusqué"
 
@@ -179,138 +178,137 @@
 msgid "Tractor is connected"
 msgstr "Tractor est connecté"
 
 #: carburetor/tasks.py:140
 msgid "Tractor couldn't connect"
 msgstr "Tractor n’a pas pu se connecter"
 
-#: carburetor/ui/about.ui:21
+#: carburetor/ui/about.ui:24
 msgid "GTK frontend for Tractor"
 msgstr "Interface GTK pour Tractor"
 
-#: carburetor/ui/about.ui:22
+#: carburetor/ui/about.ui:25
 msgid "Copyright © 2019-2023, Tractor Team"
 msgstr "Copyright © 2019-2023, Équipe Tractor"
 
-#: carburetor/ui/about.ui:30
-msgid "Source Code"
-msgstr "Code source"
-
-#: carburetor/ui/actionmenu.ui:9
-msgid "_New ID"
-msgstr "_Nouvel ID"
-
-#: carburetor/ui/actionmenu.ui:13
-msgid "_Check connection"
-msgstr "_Vérifier la connexion"
-
-#: carburetor/ui/actionmenu.ui:17
-msgid "_Toggle proxy on system"
-msgstr "_Basculer le proxy sur le système"
+#: carburetor/ui/main.ui:32
+msgid "For Tractor"
+msgstr "Pour Tractor"
 
-#: carburetor/ui/mainmenu.ui:10
+#: carburetor/ui/main.ui:94
 msgid "Preferences"
 msgstr "Préférences"
 
-#: carburetor/ui/mainmenu.ui:14
+#: carburetor/ui/main.ui:98
 msgid "About Carburetor"
 msgstr "À propos de Carburetor"
 
-#: carburetor/ui/mainmenu.ui:18
+#: carburetor/ui/main.ui:102
 msgid "Quit"
 msgstr "Quitter"
 
-#: carburetor/ui/main.ui:31
-msgid "For Tractor"
-msgstr "Pour Tractor"
+#: carburetor/ui/main.ui:110
+msgid "_New ID"
+msgstr "_Nouvel ID"
+
+#: carburetor/ui/main.ui:114
+msgid "_Check connection"
+msgstr "_Vérifier la connexion"
 
-#: carburetor/ui/preferences.ui:27
+#: carburetor/ui/main.ui:118
+msgid "_Toggle proxy on system"
+msgstr "_Basculer le proxy sur le système"
+
+#: carburetor/ui/preferences.ui:28
 msgid "General"
 msgstr "Général"
 
-#: carburetor/ui/preferences.ui:30
+#: carburetor/ui/preferences.ui:31
 msgid "Exit Node"
 msgstr "Nœud de sortie"
 
-#: carburetor/ui/preferences.ui:34
+#: carburetor/ui/preferences.ui:35
 msgid "The country you want to connect from"
 msgstr "Le pays depuis lequel vous voulez être connecté·e"
 
-#: carburetor/ui/preferences.ui:35
+#: carburetor/ui/preferences.ui:36
 msgid "Exit Country"
 msgstr "Pays de sortie"
 
-#: carburetor/ui/preferences.ui:44
+#: carburetor/ui/preferences.ui:45
 msgid "Accept Connections"
 msgstr "Accepter des connexions"
 
-#: carburetor/ui/preferences.ui:47
+#: carburetor/ui/preferences.ui:48
 msgid "Allow external devices to use this network"
 msgstr "Autoriser ou non les appareils extérieurs à utiliser ce réseau"
 
-#: carburetor/ui/preferences.ui:63
+#: carburetor/ui/preferences.ui:64
 msgid "Ports"
 msgstr "Ports"
 
-#: carburetor/ui/preferences.ui:66
+#: carburetor/ui/preferences.ui:67
 msgid "Socks Port"
 msgstr "Port SOCKS"
 
-#: carburetor/ui/preferences.ui:69
+#: carburetor/ui/preferences.ui:70
 msgid "Local port on which Tractor would be listen"
 msgstr "Port local via lequel Tractor serait écouté"
 
-#: carburetor/ui/preferences.ui:83
+#: carburetor/ui/preferences.ui:84
 msgid "DNS Port"
 msgstr "Port DNS"
 
-#: carburetor/ui/preferences.ui:86
+#: carburetor/ui/preferences.ui:87
 msgid "Local port on which you would have an anonymous name server"
 msgstr "Port local pour un serveur DNS anonyme que vous pourriez avoir"
 
-#: carburetor/ui/preferences.ui:100
+#: carburetor/ui/preferences.ui:101
 msgid "HTTP Port"
 msgstr "Port HTTP"
 
-#: carburetor/ui/preferences.ui:103
+#: carburetor/ui/preferences.ui:104
 msgid "Local port on which a HTTP tunnel would be listen"
 msgstr "Port local via lequel Tractor serait écouté"
 
-#: carburetor/ui/preferences.ui:120 carburetor/ui/preferences.ui:151
+#: carburetor/ui/preferences.ui:121 carburetor/ui/preferences.ui:152
 msgid "Bridges"
 msgstr "Ponts"
 
-#: carburetor/ui/preferences.ui:123
+#: carburetor/ui/preferences.ui:124
 msgid "Type"
 msgstr "Type"
 
-#: carburetor/ui/preferences.ui:127
+#: carburetor/ui/preferences.ui:128
 msgid "Type of bridge"
 msgstr "Type de pont"
 
-#: carburetor/ui/preferences.ui:134
+#: carburetor/ui/preferences.ui:135
 msgid "Client Transport Plugin"
 msgstr "Extension de transport des clients"
 
-#: carburetor/ui/preferences.ui:172
+#: carburetor/ui/preferences.ui:174
 msgid "_Save"
 msgstr "_Enregistrer"
 
-#: carburetor/ui/preferences.ui:173
+#: carburetor/ui/preferences.ui:175
 msgid "Save Bridges as a file in your local configs"
 msgstr "Enregistrer les ponts dans un fichier de votre configuration locale"
 
-#: carburetor/ui/preferences.ui:192
+#: carburetor/ui/preferences.ui:194
 msgid "Please check the syntax of bridges"
 msgstr "Veuillez vérifier leur syntaxe"
 
-#: carburetor/ui/preferences.ui:193
+#: carburetor/ui/preferences.ui:195
 msgid "Can not save the bridges"
 msgstr "Impossible d'enregistrer les ponts"
 
+#~ msgid "Source Code"
+#~ msgstr "Code source"
+
 #~ msgid "_Cancel"
 #~ msgstr "_Annuler"
 
 #~ msgid "Use obfs4proxy"
 #~ msgstr "Utiliser obfs4proxy"
 
 #~ msgid "Please specify the plugin executable file"
```

### Comparing `carburetor-4.0.3/carburetor/locales/hr/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.0/carburetor/locales/hr/LC_MESSAGES/carburetor.mo`

 * *Files identical despite different names*

### Comparing `carburetor-4.0.3/carburetor/locales/hr/LC_MESSAGES/carburetor.po` & `carburetor-4.1.0/carburetor/locales/hr/LC_MESSAGES/carburetor.po`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Milo Ivir <mail@milotype.de>, 2020, 2021, 2022.
 # Danial Behzadi <dani.behzi@ubuntu.com>, 2020, 2021, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 04:31+0330\n"
+"POT-Creation-Date: 2023-06-18 01:44+0330\n"
 "PO-Revision-Date: 2023-03-22 02:20+0000\n"
 "Last-Translator: Danial Behzadi <dani.behzi@ubuntu.com>\n"
 "Language-Team: Croatian <https://hosted.weblate.org/projects/carburetor/"
 "translations/hr/>\n"
 "Language: hr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
+"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 "X-Generator: Weblate 4.16.2-dev\n"
 
 #: carburetor/actions.py:94
 msgid "Disconnecting…"
 msgstr "Odspajanje …"
 
 #: carburetor/actions.py:98
@@ -56,15 +56,15 @@
 msgid "_Disconnect"
 msgstr "_Odspojeno"
 
 #: carburetor/actions.py:233
 msgid "Tractor is running"
 msgstr "Tractor je pokrenut"
 
-#: carburetor/config.py:37 carburetor/ui/about.ui:27 carburetor/ui/main.ui:32
+#: carburetor/config.py:37 carburetor/ui/about.ui:23 carburetor/ui/main.ui:33
 msgid "Carburetor"
 msgstr "Carburetor"
 
 #: carburetor/handler.py:112
 msgid "Austria"
 msgstr "Austrija"
 
@@ -152,15 +152,15 @@
 msgid "United States"
 msgstr "Sjedinjene Države"
 
 #: carburetor/handler.py:148
 msgid "Auto (Best)"
 msgstr "Automatski (najbolje)"
 
-#: carburetor/handler.py:238 carburetor/ui/preferences.ui:139
+#: carburetor/handler.py:238 carburetor/ui/preferences.ui:140
 msgid "None"
 msgstr "Ništa"
 
 #: carburetor/handler.py:239
 msgid "Vanilla"
 msgstr "Vanilla"
 
@@ -176,138 +176,137 @@
 msgid "Tractor is connected"
 msgstr "Tractor je povezan"
 
 #: carburetor/tasks.py:140
 msgid "Tractor couldn't connect"
 msgstr "Tractor se nije uspio povezati"
 
-#: carburetor/ui/about.ui:21
+#: carburetor/ui/about.ui:24
 msgid "GTK frontend for Tractor"
 msgstr "GTK sučelje za Tractor"
 
-#: carburetor/ui/about.ui:22
+#: carburetor/ui/about.ui:25
 msgid "Copyright © 2019-2023, Tractor Team"
 msgstr "Autorska prava © 2019. – 2023., Tractor tim"
 
-#: carburetor/ui/about.ui:30
-msgid "Source Code"
-msgstr "Izvorni kod"
-
-#: carburetor/ui/actionmenu.ui:9
-msgid "_New ID"
-msgstr "_Novi ID"
-
-#: carburetor/ui/actionmenu.ui:13
-msgid "_Check connection"
-msgstr "_Provjeri vezu"
-
-#: carburetor/ui/actionmenu.ui:17
-msgid "_Toggle proxy on system"
-msgstr "_Uklj./Isklj. proxy na sustavu"
+#: carburetor/ui/main.ui:32
+msgid "For Tractor"
+msgstr "Za Tractor"
 
-#: carburetor/ui/mainmenu.ui:10
+#: carburetor/ui/main.ui:94
 msgid "Preferences"
 msgstr "Postavke"
 
-#: carburetor/ui/mainmenu.ui:14
+#: carburetor/ui/main.ui:98
 msgid "About Carburetor"
 msgstr "Carburetor podaci"
 
-#: carburetor/ui/mainmenu.ui:18
+#: carburetor/ui/main.ui:102
 msgid "Quit"
 msgstr "Zatvori program"
 
-#: carburetor/ui/main.ui:31
-msgid "For Tractor"
-msgstr "Za Tractor"
+#: carburetor/ui/main.ui:110
+msgid "_New ID"
+msgstr "_Novi ID"
+
+#: carburetor/ui/main.ui:114
+msgid "_Check connection"
+msgstr "_Provjeri vezu"
 
-#: carburetor/ui/preferences.ui:27
+#: carburetor/ui/main.ui:118
+msgid "_Toggle proxy on system"
+msgstr "_Uklj./Isklj. proxy na sustavu"
+
+#: carburetor/ui/preferences.ui:28
 msgid "General"
 msgstr "Opće"
 
-#: carburetor/ui/preferences.ui:30
+#: carburetor/ui/preferences.ui:31
 msgid "Exit Node"
 msgstr "Čvor izlaza"
 
-#: carburetor/ui/preferences.ui:34
+#: carburetor/ui/preferences.ui:35
 msgid "The country you want to connect from"
 msgstr "Zemlja iz koje se želiš povezati"
 
-#: carburetor/ui/preferences.ui:35
+#: carburetor/ui/preferences.ui:36
 msgid "Exit Country"
 msgstr "Zemlja izlaza"
 
-#: carburetor/ui/preferences.ui:44
+#: carburetor/ui/preferences.ui:45
 msgid "Accept Connections"
 msgstr "Prihvati veze"
 
-#: carburetor/ui/preferences.ui:47
+#: carburetor/ui/preferences.ui:48
 msgid "Allow external devices to use this network"
 msgstr "Dopusti vanjskim uređajima koristiti ovu mrežu"
 
-#: carburetor/ui/preferences.ui:63
+#: carburetor/ui/preferences.ui:64
 msgid "Ports"
 msgstr "Priključci"
 
-#: carburetor/ui/preferences.ui:66
+#: carburetor/ui/preferences.ui:67
 msgid "Socks Port"
 msgstr "Priključak za Socks"
 
-#: carburetor/ui/preferences.ui:69
+#: carburetor/ui/preferences.ui:70
 msgid "Local port on which Tractor would be listen"
 msgstr "Lokalni priključak na kojem se Tractor prisluškuje"
 
-#: carburetor/ui/preferences.ui:83
+#: carburetor/ui/preferences.ui:84
 msgid "DNS Port"
 msgstr "Priključak za DNS"
 
-#: carburetor/ui/preferences.ui:86
+#: carburetor/ui/preferences.ui:87
 msgid "Local port on which you would have an anonymous name server"
 msgstr "Lokalni priključak na kojem se može nalaziti anonimni poslužitelj"
 
-#: carburetor/ui/preferences.ui:100
+#: carburetor/ui/preferences.ui:101
 msgid "HTTP Port"
 msgstr "Priključak za HTTP"
 
-#: carburetor/ui/preferences.ui:103
+#: carburetor/ui/preferences.ui:104
 msgid "Local port on which a HTTP tunnel would be listen"
 msgstr "Lokalni priključak na kojem se HTTP tunel prisluškuje"
 
-#: carburetor/ui/preferences.ui:120 carburetor/ui/preferences.ui:151
+#: carburetor/ui/preferences.ui:121 carburetor/ui/preferences.ui:152
 msgid "Bridges"
 msgstr "Mostovi"
 
-#: carburetor/ui/preferences.ui:123
+#: carburetor/ui/preferences.ui:124
 msgid "Type"
 msgstr "Vrsta"
 
-#: carburetor/ui/preferences.ui:127
+#: carburetor/ui/preferences.ui:128
 msgid "Type of bridge"
 msgstr "Vrsta mosta"
 
-#: carburetor/ui/preferences.ui:134
+#: carburetor/ui/preferences.ui:135
 msgid "Client Transport Plugin"
 msgstr "Dodatak klijentskog transporta"
 
-#: carburetor/ui/preferences.ui:172
+#: carburetor/ui/preferences.ui:174
 msgid "_Save"
 msgstr "_Spremi"
 
-#: carburetor/ui/preferences.ui:173
+#: carburetor/ui/preferences.ui:175
 msgid "Save Bridges as a file in your local configs"
 msgstr "Spremi mostove kao datoteku u lokalnim konfiguracijama"
 
-#: carburetor/ui/preferences.ui:192
+#: carburetor/ui/preferences.ui:194
 msgid "Please check the syntax of bridges"
 msgstr "Provjeri sintaksu mostova"
 
-#: carburetor/ui/preferences.ui:193
+#: carburetor/ui/preferences.ui:195
 msgid "Can not save the bridges"
 msgstr "Nije moguće spremiti mostove"
 
+#~ msgid "Source Code"
+#~ msgstr "Izvorni kod"
+
 #~ msgid "_Cancel"
 #~ msgstr "_Odustani"
 
 #~ msgid "Use obfs4proxy"
 #~ msgstr "Koristi obfs4proxy"
 
 #~ msgid "Please specify the plugin executable file"
```

### Comparing `carburetor-4.0.3/carburetor/locales/nb_NO/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.0/carburetor/locales/nb_NO/LC_MESSAGES/carburetor.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/"
 "carburetor/translations/nb_NO/>\n"
 "Language: nb_NO\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"X-Generator: Weblate 4.18.1\n"
 
 msgid "About Carburetor"
 msgstr "Om Carburetor"
 
 msgid "Accept Connections"
 msgstr "Godta tilkobling"
 
@@ -168,17 +168,23 @@
 
 msgid "The country you want to connect from"
 msgstr "Landet du ønsker å koble til fra"
 
 msgid "Tractor couldn't connect"
 msgstr "Tractor kunne ikke koble til"
 
+msgid "Tractor is connected"
+msgstr "Traktoren er tilkoblet"
+
 msgid "Tractor is not running!"
 msgstr "Tractor kjører ikke!"
 
+msgid "Tractor is running"
+msgstr "Tractor kjører"
+
 msgid "Tractor is stopped"
 msgstr "Tractor er stoppet"
 
 msgid "Type"
 msgstr "Type"
 
 msgid "Type of bridge"
@@ -210,9 +216,12 @@
 
 msgid "_New ID"
 msgstr "_Ny ID"
 
 msgid "_Save"
 msgstr "_Lagre"
 
+msgid "_Toggle proxy on system"
+msgstr "_Slå mellomtjener på systemet"
+
 msgid "translator-credits"
 msgstr "Allan Nordhøy, <epost@anotheragency.no>"
```

### Comparing `carburetor-4.0.3/carburetor/locales/nb_NO/LC_MESSAGES/carburetor.po` & `carburetor-4.1.0/carburetor/locales/nb_NO/LC_MESSAGES/carburetor.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Carburetor Translation Project
 # Copyright (C) 2018 Tractor Team
 # Danial Behzadi <dani.behzi@ubuntu.com>, 2018, 2020, 2021, 2022, 2023.
 # Allan Nordhøy <epost@anotheragency.no>, 2021, 2023.
+# Petter Reinholdtsen <pere-weblate@hungry.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 04:31+0330\n"
-"PO-Revision-Date: 2023-03-22 02:21+0000\n"
-"Last-Translator: Danial Behzadi <dani.behzi@ubuntu.com>\n"
+"POT-Creation-Date: 2023-06-18 01:44+0330\n"
+"PO-Revision-Date: 2023-06-29 07:49+0000\n"
+"Last-Translator: Petter Reinholdtsen <pere-weblate@hungry.com>\n"
 "Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/"
 "carburetor/translations/nb_NO/>\n"
 "Language: nb_NO\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"X-Generator: Weblate 4.18.1\n"
 "Generated-By: pygettext.py 1.5\n"
 
 #: carburetor/actions.py:94
 msgid "Disconnecting…"
 msgstr "Kobler fra …"
 
 #: carburetor/actions.py:98
@@ -52,19 +53,18 @@
 msgstr "Kjører"
 
 #: carburetor/actions.py:223
 msgid "_Disconnect"
 msgstr "_Koble fra"
 
 #: carburetor/actions.py:233
-#, fuzzy
 msgid "Tractor is running"
 msgstr "Tractor kjører"
 
-#: carburetor/config.py:37 carburetor/ui/about.ui:27 carburetor/ui/main.ui:32
+#: carburetor/config.py:37 carburetor/ui/about.ui:23 carburetor/ui/main.ui:33
 msgid "Carburetor"
 msgstr "Carburetor"
 
 #: carburetor/handler.py:112
 msgid "Austria"
 msgstr "Østerrike"
 
@@ -152,15 +152,15 @@
 msgid "United States"
 msgstr "Amerikas forente stater"
 
 #: carburetor/handler.py:148
 msgid "Auto (Best)"
 msgstr "Auto (best)"
 
-#: carburetor/handler.py:238 carburetor/ui/preferences.ui:139
+#: carburetor/handler.py:238 carburetor/ui/preferences.ui:140
 msgid "None"
 msgstr "Ingen"
 
 #: carburetor/handler.py:239
 msgid "Vanilla"
 msgstr "Uten endringer"
 
@@ -169,147 +169,144 @@
 msgstr "Tilslørt"
 
 #: carburetor/handler.py:309
 msgid "translator-credits"
 msgstr "Allan Nordhøy, <epost@anotheragency.no>"
 
 #: carburetor/tasks.py:138
-#, fuzzy
 msgid "Tractor is connected"
 msgstr "Traktoren er tilkoblet"
 
 #: carburetor/tasks.py:140
 msgid "Tractor couldn't connect"
 msgstr "Tractor kunne ikke koble til"
 
-#: carburetor/ui/about.ui:21
+#: carburetor/ui/about.ui:24
 msgid "GTK frontend for Tractor"
 msgstr "GTK-skjermflate for Tractor"
 
-#: carburetor/ui/about.ui:22
+#: carburetor/ui/about.ui:25
 msgid "Copyright © 2019-2023, Tractor Team"
 msgstr "Opphavsrett © 2019–2023, Tractor-laget"
 
-#: carburetor/ui/about.ui:30
-msgid "Source Code"
-msgstr "Kildekode"
-
-#: carburetor/ui/actionmenu.ui:9
-msgid "_New ID"
-msgstr "_Ny ID"
-
-#: carburetor/ui/actionmenu.ui:13
-msgid "_Check connection"
-msgstr "_Sjekk tilkobling"
-
-#: carburetor/ui/actionmenu.ui:17
-#, fuzzy
-msgid "_Toggle proxy on system"
-msgstr "_Slå mellom proxy på systemet"
+#: carburetor/ui/main.ui:32
+msgid "For Tractor"
+msgstr "For Tractor"
 
-#: carburetor/ui/mainmenu.ui:10
+#: carburetor/ui/main.ui:94
 msgid "Preferences"
 msgstr "Innstillinger"
 
-#: carburetor/ui/mainmenu.ui:14
+#: carburetor/ui/main.ui:98
 msgid "About Carburetor"
 msgstr "Om Carburetor"
 
-#: carburetor/ui/mainmenu.ui:18
+#: carburetor/ui/main.ui:102
 msgid "Quit"
 msgstr "Avslutt"
 
-#: carburetor/ui/main.ui:31
-msgid "For Tractor"
-msgstr "For Tractor"
+#: carburetor/ui/main.ui:110
+msgid "_New ID"
+msgstr "_Ny ID"
+
+#: carburetor/ui/main.ui:114
+msgid "_Check connection"
+msgstr "_Sjekk tilkobling"
 
-#: carburetor/ui/preferences.ui:27
+#: carburetor/ui/main.ui:118
+msgid "_Toggle proxy on system"
+msgstr "_Slå mellomtjener på systemet"
+
+#: carburetor/ui/preferences.ui:28
 msgid "General"
 msgstr "Generelt"
 
-#: carburetor/ui/preferences.ui:30
+#: carburetor/ui/preferences.ui:31
 msgid "Exit Node"
 msgstr "Utgangsnode"
 
-#: carburetor/ui/preferences.ui:34
+#: carburetor/ui/preferences.ui:35
 msgid "The country you want to connect from"
 msgstr "Landet du ønsker å koble til fra"
 
-#: carburetor/ui/preferences.ui:35
+#: carburetor/ui/preferences.ui:36
 msgid "Exit Country"
 msgstr "Avslutt land"
 
-#: carburetor/ui/preferences.ui:44
+#: carburetor/ui/preferences.ui:45
 msgid "Accept Connections"
 msgstr "Godta tilkobling"
 
-#: carburetor/ui/preferences.ui:47
+#: carburetor/ui/preferences.ui:48
 msgid "Allow external devices to use this network"
 msgstr "Hvorvidt eksterne enheter skal tillates å bruke dette nettverket"
 
-#: carburetor/ui/preferences.ui:63
+#: carburetor/ui/preferences.ui:64
 msgid "Ports"
 msgstr "Porter"
 
-#: carburetor/ui/preferences.ui:66
+#: carburetor/ui/preferences.ui:67
 msgid "Socks Port"
 msgstr "SOCKS-port"
 
-#: carburetor/ui/preferences.ui:69
+#: carburetor/ui/preferences.ui:70
 msgid "Local port on which Tractor would be listen"
 msgstr "Lokal port Tractor skal lytte til"
 
-#: carburetor/ui/preferences.ui:83
+#: carburetor/ui/preferences.ui:84
 msgid "DNS Port"
 msgstr "DNS-port"
 
-#: carburetor/ui/preferences.ui:86
+#: carburetor/ui/preferences.ui:87
 msgid "Local port on which you would have an anonymous name server"
 msgstr "Lokal port du har en anonym navnetjener på"
 
-#: carburetor/ui/preferences.ui:100
+#: carburetor/ui/preferences.ui:101
 msgid "HTTP Port"
 msgstr "HTTP-port"
 
-#: carburetor/ui/preferences.ui:103
+#: carburetor/ui/preferences.ui:104
 msgid "Local port on which a HTTP tunnel would be listen"
 msgstr "Lokal port Tractor skal lytte til"
 
-#: carburetor/ui/preferences.ui:120 carburetor/ui/preferences.ui:151
+#: carburetor/ui/preferences.ui:121 carburetor/ui/preferences.ui:152
 msgid "Bridges"
 msgstr "Broer"
 
-#: carburetor/ui/preferences.ui:123
+#: carburetor/ui/preferences.ui:124
 msgid "Type"
 msgstr "Type"
 
-#: carburetor/ui/preferences.ui:127
+#: carburetor/ui/preferences.ui:128
 msgid "Type of bridge"
 msgstr "Brotype"
 
-#: carburetor/ui/preferences.ui:134
+#: carburetor/ui/preferences.ui:135
 msgid "Client Transport Plugin"
 msgstr "Klienttransport-programtillegg"
 
-#: carburetor/ui/preferences.ui:172
+#: carburetor/ui/preferences.ui:174
 msgid "_Save"
 msgstr "_Lagre"
 
-#: carburetor/ui/preferences.ui:173
+#: carburetor/ui/preferences.ui:175
 msgid "Save Bridges as a file in your local configs"
 msgstr "Lagre broer i en fil i ditt lokaloppsett"
 
-#: carburetor/ui/preferences.ui:192
+#: carburetor/ui/preferences.ui:194
 msgid "Please check the syntax of bridges"
 msgstr "Sjekk syntaksen for broene"
 
-#: carburetor/ui/preferences.ui:193
+#: carburetor/ui/preferences.ui:195
 msgid "Can not save the bridges"
 msgstr "Kan ikke lagre broene"
 
+#~ msgid "Source Code"
+#~ msgstr "Kildekode"
+
 #~ msgid "_Cancel"
 #~ msgstr "_Avbryt"
 
 #~ msgid "Use obfs4proxy"
 #~ msgstr "Bruk obfs4proxy"
 
 #~ msgid "Please specify the plugin executable file"
```

### Comparing `carburetor-4.0.3/carburetor/locales/pl/LC_MESSAGES/carburetor.po` & `carburetor-4.1.0/carburetor/locales/pt_BR/LC_MESSAGES/carburetor.po`

 * *Files 22% similar despite different names*

```diff
@@ -1,380 +1,355 @@
 # SOME DESCRIPTIVE TITLE.
-# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
-# This file is distributed under the same license as the PACKAGE package.
-# Michal Biesiada <blade-14@o2.pl>, 2020.
-# Danial Behzadi <dani.behzi@ubuntu.com>, 2020, 2023.
+# Copyright (C) YEAR ORGANIZATION
+# lucas estevão dos santos <lucas.estevao@hotmail.com.br>, 2020.
+# Samuel Carvalho de Araújo <samuelnegro12345@gmail.com>, 2020.
+# joaooliva <joaooliva@protonmail.com>, 2020, 2021.
+# Danial Behzadi <dani.behzi@ubuntu.com>, 2020, 2022, 2023.
+# Thiago Carmona Monteiro <Guarakami1807@protonmail.ch>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 04:31+0330\n"
-"PO-Revision-Date: 2023-03-22 02:21+0000\n"
+"POT-Creation-Date: 2023-06-18 01:44+0330\n"
+"PO-Revision-Date: 2023-05-18 10:50+0000\n"
 "Last-Translator: Danial Behzadi <dani.behzi@ubuntu.com>\n"
-"Language-Team: Polish <https://hosted.weblate.org/projects/carburetor/"
-"translations/pl/>\n"
-"Language: pl\n"
+"Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/"
+"carburetor/translations/pt_BR/>\n"
+"Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
-"|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"X-Generator: Weblate 4.18-dev\n"
+"Generated-By: pygettext.py 1.5\n"
 
 #: carburetor/actions.py:94
-#, fuzzy
 msgid "Disconnecting…"
-msgstr "Rozłączanie…"
+msgstr "Desconectando…"
 
 #: carburetor/actions.py:98
-#, fuzzy
 msgid "Connecting…"
-msgstr "Łączenie…"
+msgstr "Conectando…"
 
 #: carburetor/actions.py:110
-#, fuzzy
 msgid "You have a new identity!"
-msgstr "Masz nową tożsamość!"
+msgstr "Tem uma nova identidade!"
 
 #: carburetor/actions.py:112
-#, fuzzy
 msgid "Tractor is not running!"
-msgstr "Traktor nie jedzie!"
+msgstr "Tractor não está funcionando!"
 
 #: carburetor/actions.py:196
-#, fuzzy
 msgid "Stopped"
-msgstr "Zatrzymane"
+msgstr "Parou"
 
 #: carburetor/actions.py:199
-#, fuzzy
 msgid "_Connect"
-msgstr "P_ołącz"
+msgstr "_Conecta"
 
 #: carburetor/actions.py:211
-#, fuzzy
 msgid "Tractor is stopped"
-msgstr "Ciągnik jest zatrzymany"
+msgstr "Tractor está parado"
 
 #: carburetor/actions.py:220
-#, fuzzy
 msgid "Running"
-msgstr "Działające"
+msgstr "Rodando"
 
 #: carburetor/actions.py:223
-#, fuzzy
 msgid "_Disconnect"
-msgstr "_Zerwij połączenie"
+msgstr "_Desconecta"
 
 #: carburetor/actions.py:233
-#, fuzzy
 msgid "Tractor is running"
-msgstr "Traktor pracuje"
+msgstr "Tractor está sendo executado"
 
-#: carburetor/config.py:37 carburetor/ui/about.ui:27 carburetor/ui/main.ui:32
+#: carburetor/config.py:37 carburetor/ui/about.ui:23 carburetor/ui/main.ui:33
 msgid "Carburetor"
 msgstr "Carburetor"
 
 #: carburetor/handler.py:112
 msgid "Austria"
-msgstr "Austria"
+msgstr "Áustria"
 
 #: carburetor/handler.py:113
 msgid "Bulgaria"
-msgstr "Bułgaria"
+msgstr "Bulgária"
 
 #: carburetor/handler.py:114
 msgid "Canada"
-msgstr "Kanada"
+msgstr "Canadá"
 
 #: carburetor/handler.py:115
-#, fuzzy
 msgid "Switzerland"
-msgstr "Szwajcaria"
+msgstr "Suíça"
 
 #: carburetor/handler.py:116
 msgid "Czech"
-msgstr "Czechy"
+msgstr "República Checa"
 
 #: carburetor/handler.py:117
 msgid "Germany"
-msgstr "Niemcy"
+msgstr "Alemanha"
 
 #: carburetor/handler.py:118
-#, fuzzy
 msgid "Spain"
-msgstr "Hiszpania"
+msgstr "Espanha"
 
 #: carburetor/handler.py:119
 msgid "Finland"
-msgstr "Finlandia"
+msgstr "Finlândia"
 
 #: carburetor/handler.py:120
 msgid "France"
-msgstr "Francja"
+msgstr "França"
 
 #: carburetor/handler.py:121
 msgid "Ireland"
-msgstr "Irlandia"
+msgstr "Irlanda"
 
 #: carburetor/handler.py:122
 msgid "Moldova"
-msgstr "Mołdawia"
+msgstr "Moldávia"
 
 #: carburetor/handler.py:123
 msgid "Netherlands"
-msgstr "Holandia"
+msgstr "Países Baixos"
 
 #: carburetor/handler.py:124
 msgid "Norway"
-msgstr "Norwegia"
+msgstr "Noruega"
 
 #: carburetor/handler.py:125
 msgid "Poland"
-msgstr "Polska"
+msgstr "Polônia"
 
 #: carburetor/handler.py:126
 msgid "Romania"
-msgstr "Rumunia"
+msgstr "Romênia"
 
 #: carburetor/handler.py:127
-#, fuzzy
 msgid "Seychelles"
-msgstr "Seszele"
+msgstr "Seicheles"
 
 #: carburetor/handler.py:128
-#, fuzzy
 msgid "Sweden"
-msgstr "Szwecja"
+msgstr "Suécia"
 
 #: carburetor/handler.py:129
-#, fuzzy
 msgid "Singapore"
-msgstr "Singapur"
+msgstr "Singapura"
 
 #: carburetor/handler.py:130
 msgid "Russia"
-msgstr "Rosja"
+msgstr "Rússia"
 
 #: carburetor/handler.py:131
-#, fuzzy
 msgid "Ukraine"
-msgstr "Ukraina"
+msgstr "Ucrânia"
 
 #: carburetor/handler.py:132
-#, fuzzy
 msgid "United Kingdom"
-msgstr "Wielka Brytania"
+msgstr "Reino Unido"
 
 #: carburetor/handler.py:133
-#, fuzzy
 msgid "United States"
-msgstr "Stany Zjednoczone"
+msgstr "Estados Unidos da América"
 
 #: carburetor/handler.py:148
-#, fuzzy
 msgid "Auto (Best)"
-msgstr "Automatyczny (najlepszy)"
+msgstr "Automático (Melhor)"
 
-#: carburetor/handler.py:238 carburetor/ui/preferences.ui:139
-#, fuzzy
+#: carburetor/handler.py:238 carburetor/ui/preferences.ui:140
 msgid "None"
-msgstr "Brak"
+msgstr "Nenhum"
 
 #: carburetor/handler.py:239
-#, fuzzy
 msgid "Vanilla"
-msgstr "Wanilia"
+msgstr "Baunilha"
 
 #: carburetor/handler.py:240
-#, fuzzy
 msgid "Obfuscated"
-msgstr "Zaciemniony"
+msgstr "ofuscado"
 
 #: carburetor/handler.py:309
-#, fuzzy
 msgid "translator-credits"
-msgstr ""
-"Radek Raczkowski, Adam Hulewicz, Radosław Korotkiewicz, David Troianovskyi"
+msgstr "Créditos da tradução"
 
 #: carburetor/tasks.py:138
-#, fuzzy
 msgid "Tractor is connected"
-msgstr "Ciągnik jest podłączony"
+msgstr "Tractor está conectado"
 
 #: carburetor/tasks.py:140
-#, fuzzy
 msgid "Tractor couldn't connect"
-msgstr "Ciągnik nie mógł się połączyć"
+msgstr "Tractor não conseguiu conectar"
 
-#: carburetor/ui/about.ui:21
-#, fuzzy
+#: carburetor/ui/about.ui:24
 msgid "GTK frontend for Tractor"
-msgstr "Interfejs GTK dla ciągnika"
+msgstr "Interface GTK para Tractor"
 
-#: carburetor/ui/about.ui:22
+#: carburetor/ui/about.ui:25
 msgid "Copyright © 2019-2023, Tractor Team"
-msgstr "Copyright © 2019-2023, Zespół Traktorów"
+msgstr "Copyright © 2019-2023, Tractor Team"
 
-#: carburetor/ui/about.ui:30
+#: carburetor/ui/main.ui:32
 #, fuzzy
-msgid "Source Code"
-msgstr "Kod źródłowy"
-
-#: carburetor/ui/actionmenu.ui:9
-#, fuzzy
-msgid "_New ID"
-msgstr "_Nowy identyfikator"
-
-#: carburetor/ui/actionmenu.ui:13
-#, fuzzy
-msgid "_Check connection"
-msgstr "_Sprawdź połączenie"
-
-#: carburetor/ui/actionmenu.ui:17
-#, fuzzy
-msgid "_Toggle proxy on system"
-msgstr "_Przełącz proxy w systemie"
+msgid "For Tractor"
+msgstr "para trator"
 
-#: carburetor/ui/mainmenu.ui:10
-#, fuzzy
+#: carburetor/ui/main.ui:94
 msgid "Preferences"
-msgstr "Ustawienia"
+msgstr "Preferências"
 
-#: carburetor/ui/mainmenu.ui:14
+#: carburetor/ui/main.ui:98
 #, fuzzy
 msgid "About Carburetor"
-msgstr "O gaźniku"
+msgstr "Sobre Carburador"
 
-#: carburetor/ui/mainmenu.ui:18
-#, fuzzy
+#: carburetor/ui/main.ui:102
 msgid "Quit"
-msgstr "Zakończ"
+msgstr "Sair"
 
-#: carburetor/ui/main.ui:31
-#, fuzzy
-msgid "For Tractor"
-msgstr "Dla ciągnika"
+#: carburetor/ui/main.ui:110
+msgid "_New ID"
+msgstr "_Nova identidade (ID)"
+
+#: carburetor/ui/main.ui:114
+msgid "_Check connection"
+msgstr "_Verifique a conexão"
 
-#: carburetor/ui/preferences.ui:27
+#: carburetor/ui/main.ui:118
 #, fuzzy
+msgid "_Toggle proxy on system"
+msgstr "_Alternar proxy no sistema"
+
+#: carburetor/ui/preferences.ui:28
 msgid "General"
-msgstr "Ogólny"
+msgstr "Geral"
 
-#: carburetor/ui/preferences.ui:30
-#, fuzzy
+#: carburetor/ui/preferences.ui:31
 msgid "Exit Node"
-msgstr "Węzły wyjściowe"
+msgstr "Nodo de saída"
 
-#: carburetor/ui/preferences.ui:34
-#, fuzzy
+#: carburetor/ui/preferences.ui:35
 msgid "The country you want to connect from"
-msgstr "Kraj, z którego chcesz się połączyć"
+msgstr "O país do qual quer se conectar"
 
-#: carburetor/ui/preferences.ui:35
+#: carburetor/ui/preferences.ui:36
 #, fuzzy
 msgid "Exit Country"
-msgstr "Wyjdź z kraju"
+msgstr "país de saída"
 
-#: carburetor/ui/preferences.ui:44
-#, fuzzy
+#: carburetor/ui/preferences.ui:45
 msgid "Accept Connections"
-msgstr "Zaakceptuj połączenia"
+msgstr "Aceitar conexão"
 
-#: carburetor/ui/preferences.ui:47
-#, fuzzy
+#: carburetor/ui/preferences.ui:48
 msgid "Allow external devices to use this network"
-msgstr "Zezwól urządzeniom zewnętrznym na korzystanie z tej sieci"
+msgstr "Permitir ou não que dispositivos externos usem esta rede"
 
-#: carburetor/ui/preferences.ui:63
-#, fuzzy
+#: carburetor/ui/preferences.ui:64
 msgid "Ports"
-msgstr "Porty"
+msgstr "Portas"
 
-#: carburetor/ui/preferences.ui:66
-#, fuzzy
+#: carburetor/ui/preferences.ui:67
 msgid "Socks Port"
-msgstr "Port skarpet"
+msgstr "Porta do Socket"
 
-#: carburetor/ui/preferences.ui:69
-#, fuzzy
+#: carburetor/ui/preferences.ui:70
 msgid "Local port on which Tractor would be listen"
-msgstr "Lokalny port, na którym Traktor będzie nasłuchiwał"
+msgstr "Porta local na qual o Tractor estaria escutando"
 
-#: carburetor/ui/preferences.ui:83
-#, fuzzy
+#: carburetor/ui/preferences.ui:84
 msgid "DNS Port"
-msgstr "Port DNS"
+msgstr "Porta de DNS"
 
-#: carburetor/ui/preferences.ui:86
-#, fuzzy
+#: carburetor/ui/preferences.ui:87
 msgid "Local port on which you would have an anonymous name server"
-msgstr "Port lokalny, na którym miałbyś anonimowy serwer nazw"
+msgstr "Porta local na qual você teria um servidor de nomes anônimo"
 
-#: carburetor/ui/preferences.ui:100
-#, fuzzy
+#: carburetor/ui/preferences.ui:101
 msgid "HTTP Port"
-msgstr "Port HTTP"
+msgstr "Porta de HTTP"
 
-#: carburetor/ui/preferences.ui:103
-#, fuzzy
+#: carburetor/ui/preferences.ui:104
 msgid "Local port on which a HTTP tunnel would be listen"
-msgstr "Port lokalny, na którym nasłuchiwałby tunel HTTP"
+msgstr "Porta local na qual um túnel HTTP seria escutado"
 
-#: carburetor/ui/preferences.ui:120 carburetor/ui/preferences.ui:151
-#, fuzzy
+#: carburetor/ui/preferences.ui:121 carburetor/ui/preferences.ui:152
 msgid "Bridges"
-msgstr "Mostki"
+msgstr "Pontes"
 
-#: carburetor/ui/preferences.ui:123
+#: carburetor/ui/preferences.ui:124
 #, fuzzy
 msgid "Type"
-msgstr "Rodzaj"
+msgstr "Tipo"
 
-#: carburetor/ui/preferences.ui:127
+#: carburetor/ui/preferences.ui:128
 #, fuzzy
 msgid "Type of bridge"
-msgstr "Rodzaj mostu"
+msgstr "Tipo de ponte"
 
-#: carburetor/ui/preferences.ui:134
+#: carburetor/ui/preferences.ui:135
 #, fuzzy
 msgid "Client Transport Plugin"
-msgstr "Wtyczka transportu klienta"
+msgstr "Plug-in de transporte do cliente"
 
-#: carburetor/ui/preferences.ui:172
-#, fuzzy
+#: carburetor/ui/preferences.ui:174
 msgid "_Save"
-msgstr "_Zapisz"
+msgstr "_Salvar"
 
-#: carburetor/ui/preferences.ui:173
+#: carburetor/ui/preferences.ui:175
 #, fuzzy
 msgid "Save Bridges as a file in your local configs"
-msgstr "Zapisz Bridges jako plik w swoich lokalnych konfiguracjach"
+msgstr "Salve Bridges como um arquivo em suas configurações locais"
 
-#: carburetor/ui/preferences.ui:192
-#, fuzzy
+#: carburetor/ui/preferences.ui:194
 msgid "Please check the syntax of bridges"
-msgstr "Sprawdź składnię mostów"
+msgstr "Por favor, verifique a sintaxe das pontes"
 
-#: carburetor/ui/preferences.ui:193
-#, fuzzy
+#: carburetor/ui/preferences.ui:195
 msgid "Can not save the bridges"
-msgstr "Nie można uratować mostów"
+msgstr "Não é possível salvar as pontes"
+
+#~ msgid "Source Code"
+#~ msgstr "Código-fonte"
 
 #, fuzzy
 #~ msgid "_Cancel"
-#~ msgstr "Francja"
+#~ msgstr "França"
+
+#, fuzzy
+#~ msgid "Use obfs4proxy"
+#~ msgstr "Proxy não configurado"
 
 #~ msgid "Start"
-#~ msgstr "Start"
+#~ msgstr "Iniciar"
 
 #~ msgid "Stop"
-#~ msgstr "Stop"
+#~ msgstr "Parar"
 
 #~ msgid "stopping…"
-#~ msgstr "zatrzymywanie…"
+#~ msgstr "parando…"
 
 #~ msgid "starting…"
-#~ msgstr "rozpoczynanie…"
+#~ msgstr "iniciando…"
+
+#~ msgid "Unset Proxy"
+#~ msgstr "Proxy não configurado"
 
 #~ msgid "Set Proxy"
-#~ msgstr "Ustaw Proxy"
+#~ msgstr "Configurar proxy"
+
+#~ msgid "<b>Use bridges</b>"
+#~ msgstr "<b>Usar pontes</b>"
+
+#~ msgid "<small>Bridges help you to bypass tor sensorship</small>"
+#~ msgstr "<small>As pontes te ajudam a contornar a censura do Tor</small>"
+
+#~ msgid "Bridges:"
+#~ msgstr "Pontes:"
+
+#~ msgid "<b>obfs4proxy executable</b>"
+#~ msgstr "<b>obfs4proxy executável</b>"
+
+#~ msgid "<small>You should specify where is obfs4proxy file</small>"
+#~ msgstr "<small>Deve especificar onde está o arquivo obfs4proxy</small>"
```

### Comparing `carburetor-4.0.3/carburetor/locales/pt/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.0/carburetor/locales/pt/LC_MESSAGES/carburetor.mo`

 * *Files identical despite different names*

### Comparing `carburetor-4.0.3/carburetor/locales/pt/LC_MESSAGES/carburetor.po` & `carburetor-4.1.0/carburetor/locales/pt/LC_MESSAGES/carburetor.po`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Danial Behzadi <dani.behzi@ubuntu.com>, 2020, 2021, 2022, 2023.
 # Sérgio Morais <lalocas@protonmail.com>, 2021.
 # SC <lalocas@protonmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 04:31+0330\n"
+"POT-Creation-Date: 2023-06-18 01:44+0330\n"
 "PO-Revision-Date: 2023-03-22 02:21+0000\n"
 "Last-Translator: Danial Behzadi <dani.behzi@ubuntu.com>\n"
 "Language-Team: Portuguese <https://hosted.weblate.org/projects/carburetor/"
 "translations/pt/>\n"
 "Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -58,15 +58,15 @@
 msgid "_Disconnect"
 msgstr "_Desconectar"
 
 #: carburetor/actions.py:233
 msgid "Tractor is running"
 msgstr "Tractor está em execução"
 
-#: carburetor/config.py:37 carburetor/ui/about.ui:27 carburetor/ui/main.ui:32
+#: carburetor/config.py:37 carburetor/ui/about.ui:23 carburetor/ui/main.ui:33
 msgid "Carburetor"
 msgstr "Carburetor"
 
 #: carburetor/handler.py:112
 msgid "Austria"
 msgstr "Áustria"
 
@@ -154,15 +154,15 @@
 msgid "United States"
 msgstr "Estados Unidos da América"
 
 #: carburetor/handler.py:148
 msgid "Auto (Best)"
 msgstr "Automático (melhor)"
 
-#: carburetor/handler.py:238 carburetor/ui/preferences.ui:139
+#: carburetor/handler.py:238 carburetor/ui/preferences.ui:140
 msgid "None"
 msgstr "Nenhum"
 
 #: carburetor/handler.py:239
 msgid "Vanilla"
 msgstr "Vanilla"
 
@@ -181,138 +181,137 @@
 msgid "Tractor is connected"
 msgstr "Tractor está conectado"
 
 #: carburetor/tasks.py:140
 msgid "Tractor couldn't connect"
 msgstr "O Tractor não conseguiu conectar-se"
 
-#: carburetor/ui/about.ui:21
+#: carburetor/ui/about.ui:24
 msgid "GTK frontend for Tractor"
 msgstr "GTK frontend para o Tractor"
 
-#: carburetor/ui/about.ui:22
+#: carburetor/ui/about.ui:25
 msgid "Copyright © 2019-2023, Tractor Team"
 msgstr "Direitos de autor © 2019-2023, Equipa do Tractor"
 
-#: carburetor/ui/about.ui:30
-msgid "Source Code"
-msgstr "Código-fonte"
-
-#: carburetor/ui/actionmenu.ui:9
-msgid "_New ID"
-msgstr "_Nova identidade (ID)"
-
-#: carburetor/ui/actionmenu.ui:13
-msgid "_Check connection"
-msgstr "_Verifique a conexão"
-
-#: carburetor/ui/actionmenu.ui:17
-msgid "_Toggle proxy on system"
-msgstr "_Alternar o proxy no sistema"
+#: carburetor/ui/main.ui:32
+msgid "For Tractor"
+msgstr "Para o Tractor"
 
-#: carburetor/ui/mainmenu.ui:10
+#: carburetor/ui/main.ui:94
 msgid "Preferences"
 msgstr "Preferências"
 
-#: carburetor/ui/mainmenu.ui:14
+#: carburetor/ui/main.ui:98
 msgid "About Carburetor"
 msgstr "Sobre o Carburetor"
 
-#: carburetor/ui/mainmenu.ui:18
+#: carburetor/ui/main.ui:102
 msgid "Quit"
 msgstr "Sair"
 
-#: carburetor/ui/main.ui:31
-msgid "For Tractor"
-msgstr "Para o Tractor"
+#: carburetor/ui/main.ui:110
+msgid "_New ID"
+msgstr "_Nova identidade (ID)"
+
+#: carburetor/ui/main.ui:114
+msgid "_Check connection"
+msgstr "_Verifique a conexão"
 
-#: carburetor/ui/preferences.ui:27
+#: carburetor/ui/main.ui:118
+msgid "_Toggle proxy on system"
+msgstr "_Alternar o proxy no sistema"
+
+#: carburetor/ui/preferences.ui:28
 msgid "General"
 msgstr "Geral"
 
-#: carburetor/ui/preferences.ui:30
+#: carburetor/ui/preferences.ui:31
 msgid "Exit Node"
 msgstr "Nó de saída"
 
-#: carburetor/ui/preferences.ui:34
+#: carburetor/ui/preferences.ui:35
 msgid "The country you want to connect from"
 msgstr "O país de onde quer ligar"
 
-#: carburetor/ui/preferences.ui:35
+#: carburetor/ui/preferences.ui:36
 msgid "Exit Country"
 msgstr "País da saída"
 
-#: carburetor/ui/preferences.ui:44
+#: carburetor/ui/preferences.ui:45
 msgid "Accept Connections"
 msgstr "Aceitar conexão"
 
-#: carburetor/ui/preferences.ui:47
+#: carburetor/ui/preferences.ui:48
 msgid "Allow external devices to use this network"
 msgstr "Permitir ou não que os aparelhos externos usem esta rede"
 
-#: carburetor/ui/preferences.ui:63
+#: carburetor/ui/preferences.ui:64
 msgid "Ports"
 msgstr "Portas"
 
-#: carburetor/ui/preferences.ui:66
+#: carburetor/ui/preferences.ui:67
 msgid "Socks Port"
 msgstr "Porta socks"
 
-#: carburetor/ui/preferences.ui:69
+#: carburetor/ui/preferences.ui:70
 msgid "Local port on which Tractor would be listen"
 msgstr "Porta local na qual o Tractor estará à escuta"
 
-#: carburetor/ui/preferences.ui:83
+#: carburetor/ui/preferences.ui:84
 msgid "DNS Port"
 msgstr "Porta de DNS"
 
-#: carburetor/ui/preferences.ui:86
+#: carburetor/ui/preferences.ui:87
 msgid "Local port on which you would have an anonymous name server"
 msgstr "Porta local do servidor de nome anónimo DNS"
 
-#: carburetor/ui/preferences.ui:100
+#: carburetor/ui/preferences.ui:101
 msgid "HTTP Port"
 msgstr "Porta de HTTP"
 
-#: carburetor/ui/preferences.ui:103
+#: carburetor/ui/preferences.ui:104
 msgid "Local port on which a HTTP tunnel would be listen"
 msgstr "Porta local a qual o túnel HTTP estará à escuta"
 
-#: carburetor/ui/preferences.ui:120 carburetor/ui/preferences.ui:151
+#: carburetor/ui/preferences.ui:121 carburetor/ui/preferences.ui:152
 msgid "Bridges"
 msgstr "Pontes"
 
-#: carburetor/ui/preferences.ui:123
+#: carburetor/ui/preferences.ui:124
 msgid "Type"
 msgstr "Tipo"
 
-#: carburetor/ui/preferences.ui:127
+#: carburetor/ui/preferences.ui:128
 msgid "Type of bridge"
 msgstr "Tipo de ponte"
 
-#: carburetor/ui/preferences.ui:134
+#: carburetor/ui/preferences.ui:135
 msgid "Client Transport Plugin"
 msgstr "Plugin de cliente Transport"
 
-#: carburetor/ui/preferences.ui:172
+#: carburetor/ui/preferences.ui:174
 msgid "_Save"
 msgstr "_Guardar"
 
-#: carburetor/ui/preferences.ui:173
+#: carburetor/ui/preferences.ui:175
 msgid "Save Bridges as a file in your local configs"
 msgstr "Guardar pontes como um ficheiro nas suas configurações locais"
 
-#: carburetor/ui/preferences.ui:192
+#: carburetor/ui/preferences.ui:194
 msgid "Please check the syntax of bridges"
 msgstr "Por favor, verifique a sintaxe das pontes"
 
-#: carburetor/ui/preferences.ui:193
+#: carburetor/ui/preferences.ui:195
 msgid "Can not save the bridges"
 msgstr "Não é possível guardar as pontes"
 
+#~ msgid "Source Code"
+#~ msgstr "Código-fonte"
+
 #~ msgid "_Cancel"
 #~ msgstr "_Cancelar"
 
 #~ msgid "Use obfs4proxy"
 #~ msgstr "Usar obfs4proxy"
 
 #~ msgid "Please specify the plugin executable file"
```

### Comparing `carburetor-4.0.3/carburetor/locales/pt_BR/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.0/carburetor/locales/pt_BR/LC_MESSAGES/carburetor.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/"
 "carburetor/translations/pt_BR/>\n"
 "Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 msgid "Accept Connections"
 msgstr "Aceitar conexão"
 
 msgid "Allow external devices to use this network"
 msgstr "Permitir ou não que dispositivos externos usem esta rede"
 
@@ -60,14 +60,17 @@
 
 msgid "Finland"
 msgstr "Finlândia"
 
 msgid "France"
 msgstr "França"
 
+msgid "GTK frontend for Tractor"
+msgstr "Interface GTK para Tractor"
+
 msgid "General"
 msgstr "Geral"
 
 msgid "Germany"
 msgstr "Alemanha"
 
 msgid "HTTP Port"
@@ -147,14 +150,20 @@
 
 msgid "Switzerland"
 msgstr "Suíça"
 
 msgid "The country you want to connect from"
 msgstr "O país do qual quer se conectar"
 
+msgid "Tractor couldn't connect"
+msgstr "Tractor não conseguiu conectar"
+
+msgid "Tractor is connected"
+msgstr "Tractor está conectado"
+
 msgid "Tractor is not running!"
 msgstr "Tractor não está funcionando!"
 
 msgid "Tractor is running"
 msgstr "Tractor está sendo executado"
 
 msgid "Tractor is stopped"
@@ -165,17 +174,23 @@
 
 msgid "United Kingdom"
 msgstr "Reino Unido"
 
 msgid "United States"
 msgstr "Estados Unidos da América"
 
+msgid "Vanilla"
+msgstr "Baunilha"
+
 msgid "You have a new identity!"
 msgstr "Tem uma nova identidade!"
 
+msgid "_Check connection"
+msgstr "_Verifique a conexão"
+
 msgid "_Connect"
 msgstr "_Conecta"
 
 msgid "_Disconnect"
 msgstr "_Desconecta"
 
 msgid "_New ID"
```

### Comparing `carburetor-4.0.3/carburetor/locales/pt_BR/LC_MESSAGES/carburetor.po` & `carburetor-4.1.0/carburetor/locales/pl/LC_MESSAGES/carburetor.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,361 +1,340 @@
 # SOME DESCRIPTIVE TITLE.
-# Copyright (C) YEAR ORGANIZATION
-# lucas estevão dos santos <lucas.estevao@hotmail.com.br>, 2020.
-# Samuel Carvalho de Araújo <samuelnegro12345@gmail.com>, 2020.
-# joaooliva <joaooliva@protonmail.com>, 2020, 2021.
-# Danial Behzadi <dani.behzi@ubuntu.com>, 2020, 2022, 2023.
-# Thiago Carmona Monteiro <Guarakami1807@protonmail.ch>, 2022.
+# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
+# This file is distributed under the same license as the PACKAGE package.
+# Michal Biesiada <blade-14@o2.pl>, 2020.
+# Danial Behzadi <dani.behzi@ubuntu.com>, 2020, 2023.
+# gnu-ewm <gnu.ewm@protonmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 04:31+0330\n"
-"PO-Revision-Date: 2023-03-22 02:21+0000\n"
-"Last-Translator: Danial Behzadi <dani.behzi@ubuntu.com>\n"
-"Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/"
-"carburetor/translations/pt_BR/>\n"
-"Language: pt_BR\n"
+"POT-Creation-Date: 2023-06-18 01:44+0330\n"
+"PO-Revision-Date: 2023-04-23 10:46+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Polish <https://hosted.weblate.org/projects/carburetor/"
+"translations/pl/>\n"
+"Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
-"Generated-By: pygettext.py 1.5\n"
+"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: carburetor/actions.py:94
 msgid "Disconnecting…"
-msgstr "Desconectando…"
+msgstr "Rozłączanie…"
 
 #: carburetor/actions.py:98
 msgid "Connecting…"
-msgstr "Conectando…"
+msgstr "Łączenie…"
 
 #: carburetor/actions.py:110
 msgid "You have a new identity!"
-msgstr "Tem uma nova identidade!"
+msgstr "Masz nową tożsamość!"
 
 #: carburetor/actions.py:112
+#, fuzzy
 msgid "Tractor is not running!"
-msgstr "Tractor não está funcionando!"
+msgstr "Traktor nie jedzie!"
 
 #: carburetor/actions.py:196
 msgid "Stopped"
-msgstr "Parou"
+msgstr "Zatrzymane"
 
 #: carburetor/actions.py:199
 msgid "_Connect"
-msgstr "_Conecta"
+msgstr "Połą_cz"
 
 #: carburetor/actions.py:211
+#, fuzzy
 msgid "Tractor is stopped"
-msgstr "Tractor está parado"
+msgstr "Ciągnik jest zatrzymany"
 
 #: carburetor/actions.py:220
 msgid "Running"
-msgstr "Rodando"
+msgstr "Działające"
 
 #: carburetor/actions.py:223
 msgid "_Disconnect"
-msgstr "_Desconecta"
+msgstr "_Zerwij połączenie"
 
 #: carburetor/actions.py:233
+#, fuzzy
 msgid "Tractor is running"
-msgstr "Tractor está sendo executado"
+msgstr "Traktor pracuje"
 
-#: carburetor/config.py:37 carburetor/ui/about.ui:27 carburetor/ui/main.ui:32
+#: carburetor/config.py:37 carburetor/ui/about.ui:23 carburetor/ui/main.ui:33
 msgid "Carburetor"
 msgstr "Carburetor"
 
 #: carburetor/handler.py:112
 msgid "Austria"
-msgstr "Áustria"
+msgstr "Austria"
 
 #: carburetor/handler.py:113
 msgid "Bulgaria"
-msgstr "Bulgária"
+msgstr "Bułgaria"
 
 #: carburetor/handler.py:114
 msgid "Canada"
-msgstr "Canadá"
+msgstr "Kanada"
 
 #: carburetor/handler.py:115
 msgid "Switzerland"
-msgstr "Suíça"
+msgstr "Szwajcaria"
 
 #: carburetor/handler.py:116
 msgid "Czech"
-msgstr "República Checa"
+msgstr "Czechy"
 
 #: carburetor/handler.py:117
 msgid "Germany"
-msgstr "Alemanha"
+msgstr "Niemcy"
 
 #: carburetor/handler.py:118
 msgid "Spain"
-msgstr "Espanha"
+msgstr "Hiszpania"
 
 #: carburetor/handler.py:119
 msgid "Finland"
-msgstr "Finlândia"
+msgstr "Finlandia"
 
 #: carburetor/handler.py:120
 msgid "France"
-msgstr "França"
+msgstr "Francja"
 
 #: carburetor/handler.py:121
 msgid "Ireland"
-msgstr "Irlanda"
+msgstr "Irlandia"
 
 #: carburetor/handler.py:122
 msgid "Moldova"
-msgstr "Moldávia"
+msgstr "Mołdawia"
 
 #: carburetor/handler.py:123
 msgid "Netherlands"
-msgstr "Países Baixos"
+msgstr "Holandia"
 
 #: carburetor/handler.py:124
 msgid "Norway"
-msgstr "Noruega"
+msgstr "Norwegia"
 
 #: carburetor/handler.py:125
 msgid "Poland"
-msgstr "Polônia"
+msgstr "Polska"
 
 #: carburetor/handler.py:126
 msgid "Romania"
-msgstr "Romênia"
+msgstr "Rumunia"
 
 #: carburetor/handler.py:127
 msgid "Seychelles"
-msgstr "Seicheles"
+msgstr "Seszele"
 
 #: carburetor/handler.py:128
 msgid "Sweden"
-msgstr "Suécia"
+msgstr "Szwecja"
 
 #: carburetor/handler.py:129
 msgid "Singapore"
-msgstr "Singapura"
+msgstr "Singapur"
 
 #: carburetor/handler.py:130
 msgid "Russia"
-msgstr "Rússia"
+msgstr "Rosja"
 
 #: carburetor/handler.py:131
 msgid "Ukraine"
-msgstr "Ucrânia"
+msgstr "Ukraina"
 
 #: carburetor/handler.py:132
 msgid "United Kingdom"
-msgstr "Reino Unido"
+msgstr "Wielka Brytania"
 
 #: carburetor/handler.py:133
 msgid "United States"
-msgstr "Estados Unidos da América"
+msgstr "Stany Zjednoczone"
 
 #: carburetor/handler.py:148
 msgid "Auto (Best)"
-msgstr "Automático (Melhor)"
+msgstr "Automatycznie (najlepiej)"
 
-#: carburetor/handler.py:238 carburetor/ui/preferences.ui:139
+#: carburetor/handler.py:238 carburetor/ui/preferences.ui:140
 msgid "None"
-msgstr "Nenhum"
+msgstr "Brak"
 
 #: carburetor/handler.py:239
-#, fuzzy
 msgid "Vanilla"
-msgstr "Baunilha"
+msgstr "Wanilia"
 
 #: carburetor/handler.py:240
 msgid "Obfuscated"
-msgstr "ofuscado"
+msgstr "Zaciemnione"
 
 #: carburetor/handler.py:309
 msgid "translator-credits"
-msgstr "Créditos da tradução"
+msgstr ""
+"Radek Raczkowski, Adam Hulewicz, Radosław Korotkiewicz, David Troianovskyi"
 
 #: carburetor/tasks.py:138
 #, fuzzy
 msgid "Tractor is connected"
-msgstr "O trator está conectado"
+msgstr "Ciągnik jest podłączony"
 
 #: carburetor/tasks.py:140
 #, fuzzy
 msgid "Tractor couldn't connect"
-msgstr "O trator não conseguiu conectar"
+msgstr "Ciągnik nie mógł się połączyć"
 
-#: carburetor/ui/about.ui:21
+#: carburetor/ui/about.ui:24
 #, fuzzy
 msgid "GTK frontend for Tractor"
-msgstr "Interface GTK para trator"
+msgstr "Interfejs GTK dla ciągnika"
 
-#: carburetor/ui/about.ui:22
+#: carburetor/ui/about.ui:25
 msgid "Copyright © 2019-2023, Tractor Team"
-msgstr "Copyright © 2019-2023, Tractor Team"
-
-#: carburetor/ui/about.ui:30
-msgid "Source Code"
-msgstr "Código-fonte"
-
-#: carburetor/ui/actionmenu.ui:9
-msgid "_New ID"
-msgstr "_Nova identidade (ID)"
-
-#: carburetor/ui/actionmenu.ui:13
-#, fuzzy
-msgid "_Check connection"
-msgstr "_Verifique a conexão"
+msgstr "Copyright © 2019-2023, Zespół Traktorów"
 
-#: carburetor/ui/actionmenu.ui:17
+#: carburetor/ui/main.ui:32
 #, fuzzy
-msgid "_Toggle proxy on system"
-msgstr "_Alternar proxy no sistema"
+msgid "For Tractor"
+msgstr "Dla ciągnika"
 
-#: carburetor/ui/mainmenu.ui:10
+#: carburetor/ui/main.ui:94
 msgid "Preferences"
-msgstr "Preferências"
+msgstr "Preferencje"
 
-#: carburetor/ui/mainmenu.ui:14
+#: carburetor/ui/main.ui:98
 #, fuzzy
 msgid "About Carburetor"
-msgstr "Sobre Carburador"
+msgstr "O gaźniku"
 
-#: carburetor/ui/mainmenu.ui:18
+#: carburetor/ui/main.ui:102
 msgid "Quit"
-msgstr "Sair"
+msgstr "Zakończ"
 
-#: carburetor/ui/main.ui:31
-#, fuzzy
-msgid "For Tractor"
-msgstr "para trator"
+#: carburetor/ui/main.ui:110
+msgid "_New ID"
+msgstr "_Nowy identyfikator"
+
+#: carburetor/ui/main.ui:114
+msgid "_Check connection"
+msgstr "_Sprawdź połączenie"
+
+#: carburetor/ui/main.ui:118
+msgid "_Toggle proxy on system"
+msgstr "_Przełącz proxy w systemie"
 
-#: carburetor/ui/preferences.ui:27
+#: carburetor/ui/preferences.ui:28
 msgid "General"
-msgstr "Geral"
+msgstr "Ogólne"
 
-#: carburetor/ui/preferences.ui:30
+#: carburetor/ui/preferences.ui:31
 msgid "Exit Node"
-msgstr "Nodo de saída"
+msgstr "Węzły wyjściowe"
 
-#: carburetor/ui/preferences.ui:34
+#: carburetor/ui/preferences.ui:35
 msgid "The country you want to connect from"
-msgstr "O país do qual quer se conectar"
+msgstr "Kraj, z którego chcesz się połączyć"
 
-#: carburetor/ui/preferences.ui:35
+#: carburetor/ui/preferences.ui:36
 #, fuzzy
 msgid "Exit Country"
-msgstr "país de saída"
+msgstr "Wyjdź z kraju"
 
-#: carburetor/ui/preferences.ui:44
+#: carburetor/ui/preferences.ui:45
 msgid "Accept Connections"
-msgstr "Aceitar conexão"
+msgstr "Zaakceptuj połączenia"
 
-#: carburetor/ui/preferences.ui:47
+#: carburetor/ui/preferences.ui:48
 msgid "Allow external devices to use this network"
-msgstr "Permitir ou não que dispositivos externos usem esta rede"
+msgstr "Zezwól urządzeniom zewnętrznym na korzystanie z tej sieci"
 
-#: carburetor/ui/preferences.ui:63
+#: carburetor/ui/preferences.ui:64
 msgid "Ports"
-msgstr "Portas"
+msgstr "Porty"
 
-#: carburetor/ui/preferences.ui:66
+#: carburetor/ui/preferences.ui:67
+#, fuzzy
 msgid "Socks Port"
-msgstr "Porta do Socket"
+msgstr "Port skarpet"
 
-#: carburetor/ui/preferences.ui:69
+#: carburetor/ui/preferences.ui:70
+#, fuzzy
 msgid "Local port on which Tractor would be listen"
-msgstr "Porta local na qual o Tractor estaria escutando"
+msgstr "Port lokalny, na którym Tractor będzie nasłuchiwał"
 
-#: carburetor/ui/preferences.ui:83
+#: carburetor/ui/preferences.ui:84
 msgid "DNS Port"
-msgstr "Porta de DNS"
+msgstr "Port DNS"
 
-#: carburetor/ui/preferences.ui:86
+#: carburetor/ui/preferences.ui:87
+#, fuzzy
 msgid "Local port on which you would have an anonymous name server"
-msgstr "Porta local na qual você teria um servidor de nomes anônimo"
+msgstr "Port lokalny, na którym miałbyś anonimowy serwer nazw"
 
-#: carburetor/ui/preferences.ui:100
+#: carburetor/ui/preferences.ui:101
 msgid "HTTP Port"
-msgstr "Porta de HTTP"
+msgstr "Port HTTP"
 
-#: carburetor/ui/preferences.ui:103
+#: carburetor/ui/preferences.ui:104
+#, fuzzy
 msgid "Local port on which a HTTP tunnel would be listen"
-msgstr "Porta local na qual um túnel HTTP seria escutado"
+msgstr "Port lokalny, na którym nasłuchiwałby tunel HTTP"
 
-#: carburetor/ui/preferences.ui:120 carburetor/ui/preferences.ui:151
+#: carburetor/ui/preferences.ui:121 carburetor/ui/preferences.ui:152
 msgid "Bridges"
-msgstr "Pontes"
+msgstr "Mostki"
 
-#: carburetor/ui/preferences.ui:123
-#, fuzzy
+#: carburetor/ui/preferences.ui:124
 msgid "Type"
-msgstr "Tipo"
+msgstr "Rodzaj"
 
-#: carburetor/ui/preferences.ui:127
-#, fuzzy
+#: carburetor/ui/preferences.ui:128
 msgid "Type of bridge"
-msgstr "Tipo de ponte"
+msgstr "Rodzaj mostu"
 
-#: carburetor/ui/preferences.ui:134
-#, fuzzy
+#: carburetor/ui/preferences.ui:135
 msgid "Client Transport Plugin"
-msgstr "Plug-in de transporte do cliente"
+msgstr "Wtyczka transportu klienta"
 
-#: carburetor/ui/preferences.ui:172
+#: carburetor/ui/preferences.ui:174
 msgid "_Save"
-msgstr "_Salvar"
+msgstr "_Zapisz"
 
-#: carburetor/ui/preferences.ui:173
+#: carburetor/ui/preferences.ui:175
 #, fuzzy
 msgid "Save Bridges as a file in your local configs"
-msgstr "Salve Bridges como um arquivo em suas configurações locais"
+msgstr "Zapisz Bridges jako plik w swoich lokalnych konfiguracjach"
 
-#: carburetor/ui/preferences.ui:192
+#: carburetor/ui/preferences.ui:194
 msgid "Please check the syntax of bridges"
-msgstr "Por favor, verifique a sintaxe das pontes"
+msgstr "Sprawdź składnię mostów"
 
-#: carburetor/ui/preferences.ui:193
+#: carburetor/ui/preferences.ui:195
+#, fuzzy
 msgid "Can not save the bridges"
-msgstr "Não é possível salvar as pontes"
+msgstr "Nie można uratować mostów"
 
-#, fuzzy
-#~ msgid "_Cancel"
-#~ msgstr "França"
+#~ msgid "Source Code"
+#~ msgstr "Kod źródłowy"
 
 #, fuzzy
-#~ msgid "Use obfs4proxy"
-#~ msgstr "Proxy não configurado"
+#~ msgid "_Cancel"
+#~ msgstr "Francja"
 
 #~ msgid "Start"
-#~ msgstr "Iniciar"
+#~ msgstr "Start"
 
 #~ msgid "Stop"
-#~ msgstr "Parar"
+#~ msgstr "Stop"
 
 #~ msgid "stopping…"
-#~ msgstr "parando…"
+#~ msgstr "zatrzymywanie…"
 
 #~ msgid "starting…"
-#~ msgstr "iniciando…"
-
-#~ msgid "Unset Proxy"
-#~ msgstr "Proxy não configurado"
+#~ msgstr "rozpoczynanie…"
 
 #~ msgid "Set Proxy"
-#~ msgstr "Configurar proxy"
-
-#~ msgid "<b>Use bridges</b>"
-#~ msgstr "<b>Usar pontes</b>"
-
-#~ msgid "<small>Bridges help you to bypass tor sensorship</small>"
-#~ msgstr "<small>As pontes te ajudam a contornar a censura do Tor</small>"
-
-#~ msgid "Bridges:"
-#~ msgstr "Pontes:"
-
-#~ msgid "<b>obfs4proxy executable</b>"
-#~ msgstr "<b>obfs4proxy executável</b>"
-
-#~ msgid "<small>You should specify where is obfs4proxy file</small>"
-#~ msgstr "<small>Deve especificar onde está o arquivo obfs4proxy</small>"
+#~ msgstr "Ustaw Proxy"
```

### Comparing `carburetor-4.0.3/carburetor/locales/tr/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.0/carburetor/locales/tr/LC_MESSAGES/carburetor.mo`

 * *Files identical despite different names*

### Comparing `carburetor-4.0.3/carburetor/locales/tr/LC_MESSAGES/carburetor.po` & `carburetor-4.1.0/carburetor/locales/tr/LC_MESSAGES/carburetor.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Oğuz Ersen <oguzersen@protonmail.com>, 2020, 2021.
 # Danial Behzadi <dani.behzi@ubuntu.com>, 2020, 2021, 2023.
 # Oğuz Ersen <oguz@ersen.moe>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-22 04:31+0330\n"
+"POT-Creation-Date: 2023-06-18 01:44+0330\n"
 "PO-Revision-Date: 2023-03-22 02:21+0000\n"
 "Last-Translator: Danial Behzadi <dani.behzi@ubuntu.com>\n"
 "Language-Team: Turkish <https://hosted.weblate.org/projects/carburetor/"
 "translations/tr/>\n"
 "Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -56,15 +56,15 @@
 msgid "_Disconnect"
 msgstr "Bağlantıyı _kes"
 
 #: carburetor/actions.py:233
 msgid "Tractor is running"
 msgstr "Tractor çalışıyor"
 
-#: carburetor/config.py:37 carburetor/ui/about.ui:27 carburetor/ui/main.ui:32
+#: carburetor/config.py:37 carburetor/ui/about.ui:23 carburetor/ui/main.ui:33
 msgid "Carburetor"
 msgstr "Carburetor"
 
 #: carburetor/handler.py:112
 msgid "Austria"
 msgstr "Avusturya"
 
@@ -152,15 +152,15 @@
 msgid "United States"
 msgstr "Amerika Birleşik Devletleri"
 
 #: carburetor/handler.py:148
 msgid "Auto (Best)"
 msgstr "Otomatik (En iyisi)"
 
-#: carburetor/handler.py:238 carburetor/ui/preferences.ui:139
+#: carburetor/handler.py:238 carburetor/ui/preferences.ui:140
 msgid "None"
 msgstr "Yok"
 
 #: carburetor/handler.py:239
 msgid "Vanilla"
 msgstr "Sade"
 
@@ -176,138 +176,137 @@
 msgid "Tractor is connected"
 msgstr "Tractor bağlandı"
 
 #: carburetor/tasks.py:140
 msgid "Tractor couldn't connect"
 msgstr "Tractor bağlanamadı"
 
-#: carburetor/ui/about.ui:21
+#: carburetor/ui/about.ui:24
 msgid "GTK frontend for Tractor"
 msgstr "Tractor için GTK önyüzü"
 
-#: carburetor/ui/about.ui:22
+#: carburetor/ui/about.ui:25
 msgid "Copyright © 2019-2023, Tractor Team"
 msgstr "Telif Hakkı © 2019-2023, Tractor Ekibi"
 
-#: carburetor/ui/about.ui:30
-msgid "Source Code"
-msgstr "Kaynak Kodları"
-
-#: carburetor/ui/actionmenu.ui:9
-msgid "_New ID"
-msgstr "_Yeni kimlik"
-
-#: carburetor/ui/actionmenu.ui:13
-msgid "_Check connection"
-msgstr "Bağlantıyı _denetle"
-
-#: carburetor/ui/actionmenu.ui:17
-msgid "_Toggle proxy on system"
-msgstr "Sistemde vekil sunucu _aç/kapat"
+#: carburetor/ui/main.ui:32
+msgid "For Tractor"
+msgstr "Tractor için"
 
-#: carburetor/ui/mainmenu.ui:10
+#: carburetor/ui/main.ui:94
 msgid "Preferences"
 msgstr "Tercihler"
 
-#: carburetor/ui/mainmenu.ui:14
+#: carburetor/ui/main.ui:98
 msgid "About Carburetor"
 msgstr "Carburetor Hakkında"
 
-#: carburetor/ui/mainmenu.ui:18
+#: carburetor/ui/main.ui:102
 msgid "Quit"
 msgstr "Çıkış"
 
-#: carburetor/ui/main.ui:31
-msgid "For Tractor"
-msgstr "Tractor için"
+#: carburetor/ui/main.ui:110
+msgid "_New ID"
+msgstr "_Yeni kimlik"
+
+#: carburetor/ui/main.ui:114
+msgid "_Check connection"
+msgstr "Bağlantıyı _denetle"
 
-#: carburetor/ui/preferences.ui:27
+#: carburetor/ui/main.ui:118
+msgid "_Toggle proxy on system"
+msgstr "Sistemde vekil sunucu _aç/kapat"
+
+#: carburetor/ui/preferences.ui:28
 msgid "General"
 msgstr "Genel"
 
-#: carburetor/ui/preferences.ui:30
+#: carburetor/ui/preferences.ui:31
 msgid "Exit Node"
 msgstr "Çıkış Düğümü"
 
-#: carburetor/ui/preferences.ui:34
+#: carburetor/ui/preferences.ui:35
 msgid "The country you want to connect from"
 msgstr "Üzerinden bağlanmak istediğiniz ülke"
 
-#: carburetor/ui/preferences.ui:35
+#: carburetor/ui/preferences.ui:36
 msgid "Exit Country"
 msgstr "Çıkış Ülkesi"
 
-#: carburetor/ui/preferences.ui:44
+#: carburetor/ui/preferences.ui:45
 msgid "Accept Connections"
 msgstr "Bağlantıları Kabul Et"
 
-#: carburetor/ui/preferences.ui:47
+#: carburetor/ui/preferences.ui:48
 msgid "Allow external devices to use this network"
 msgstr "Harici aygıtların bu ağı kullanmasına izin ver"
 
-#: carburetor/ui/preferences.ui:63
+#: carburetor/ui/preferences.ui:64
 msgid "Ports"
 msgstr "Bağlantı Noktaları"
 
-#: carburetor/ui/preferences.ui:66
+#: carburetor/ui/preferences.ui:67
 msgid "Socks Port"
 msgstr "Socks Bağlantı Noktası"
 
-#: carburetor/ui/preferences.ui:69
+#: carburetor/ui/preferences.ui:70
 msgid "Local port on which Tractor would be listen"
 msgstr "Tractor'un dinleyeceği yerel bağlantı noktası"
 
-#: carburetor/ui/preferences.ui:83
+#: carburetor/ui/preferences.ui:84
 msgid "DNS Port"
 msgstr "DNS Bağlantı Noktası"
 
-#: carburetor/ui/preferences.ui:86
+#: carburetor/ui/preferences.ui:87
 msgid "Local port on which you would have an anonymous name server"
 msgstr "Anonim bir ad sunucunuzun olacağı yerel bağlantı noktası"
 
-#: carburetor/ui/preferences.ui:100
+#: carburetor/ui/preferences.ui:101
 msgid "HTTP Port"
 msgstr "HTTP Bağlantı Noktası"
 
-#: carburetor/ui/preferences.ui:103
+#: carburetor/ui/preferences.ui:104
 msgid "Local port on which a HTTP tunnel would be listen"
 msgstr "HTTP tünelinin dinleyeceği yerel bağlantı noktası"
 
-#: carburetor/ui/preferences.ui:120 carburetor/ui/preferences.ui:151
+#: carburetor/ui/preferences.ui:121 carburetor/ui/preferences.ui:152
 msgid "Bridges"
 msgstr "Köprüler"
 
-#: carburetor/ui/preferences.ui:123
+#: carburetor/ui/preferences.ui:124
 msgid "Type"
 msgstr "Tür"
 
-#: carburetor/ui/preferences.ui:127
+#: carburetor/ui/preferences.ui:128
 msgid "Type of bridge"
 msgstr "Köprü türü"
 
-#: carburetor/ui/preferences.ui:134
+#: carburetor/ui/preferences.ui:135
 msgid "Client Transport Plugin"
 msgstr "İstemci Taşıma Eklentisi"
 
-#: carburetor/ui/preferences.ui:172
+#: carburetor/ui/preferences.ui:174
 msgid "_Save"
 msgstr "_Kaydet"
 
-#: carburetor/ui/preferences.ui:173
+#: carburetor/ui/preferences.ui:175
 msgid "Save Bridges as a file in your local configs"
 msgstr "Köprüleri yerel bir yapılandırma dosyası olarak kaydet"
 
-#: carburetor/ui/preferences.ui:192
+#: carburetor/ui/preferences.ui:194
 msgid "Please check the syntax of bridges"
 msgstr "Lütfen köprülerin söz dizimini gözden geçirin"
 
-#: carburetor/ui/preferences.ui:193
+#: carburetor/ui/preferences.ui:195
 msgid "Can not save the bridges"
 msgstr "Köprüler kaydedilemiyor"
 
+#~ msgid "Source Code"
+#~ msgstr "Kaynak Kodları"
+
 #~ msgid "none"
 #~ msgstr "yok"
 
 #~ msgid "_Cancel"
 #~ msgstr "_İptal"
 
 #~ msgid "Use obfs4proxy"
```

### Comparing `carburetor-4.0.3/carburetor/tasks.py` & `carburetor-4.1.0/carburetor/tasks.py`

 * *Files identical despite different names*

### Comparing `carburetor-4.0.3/carburetor/ui/about.ui` & `carburetor-4.1.0/carburetor/ui/about.ui`

 * *Files 10% similar despite different names*

#### Comparing `carburetor-4.0.3/carburetor/ui/about.ui` & `carburetor-4.1.0/carburetor/ui/about.ui`

```diff
@@ -1,33 +1,35 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- Created with Cambalache 0.10.3 -->
+<!-- Created with Cambalache 0.12.0 -->
+<!-- Danial Behzadi <dani.behzi@ubuntu.com>, 2023-->
 <interface>
+  <!-- interface-name about.ui -->
   <!-- interface-description This file is part of Carburetor. -->
   <!-- interface-copyright Carburetor is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 Carburetor is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with Carburetor.  If not, see <http://www.gnu.org/licenses/>. -->
   <!-- interface-authors Danial Behzadi <dani.behzi@ubuntu.com> -->
-  <requires lib="gtk" version="4.6"/>
-  <object class="GtkAboutDialog" id="AboutDialog">
-    <property name="authors">Danial Behzadi &lt;dani.behzi@ubuntu.com&gt;</property>
+  <requires lib="libadwaita" version="1.3"/>
+  <object class="AdwAboutWindow" id="AboutDialog">
+    <property name="application-icon">carburetor</property>
+    <property name="application-name" translatable="yes">Carburetor</property>
     <property name="comments" translatable="yes">GTK frontend for Tractor</property>
     <property name="copyright" translatable="yes">Copyright © 2019-2023, Tractor Team</property>
+    <property name="developers">Danial Behzadi &lt;dani.behzi@ubuntu.com&gt;</property>
     <property name="hide-on-close">True</property>
+    <property name="issue-url">https://framagit.org/tractor/carburetor/issues/new</property>
     <property name="license-type">gpl-3-0</property>
-    <property name="logo-icon-name">Carburetor</property>
     <property name="modal">True</property>
-    <property name="program-name" translatable="yes">Carburetor</property>
-    <property name="version">4.0.3</property>
+    <property name="version">4.1.0</property>
     <property name="website">https://framagit.org/tractor/carburetor</property>
-    <property name="website-label" translatable="yes">Source Code</property>
     <signal name="realize" handler="on_about_realize"/>
   </object>
 </interface>
```

### Comparing `carburetor-4.0.3/carburetor/ui/main.ui` & `carburetor-4.1.0/carburetor/ui/main.ui`

 * *Files 22% similar despite different names*

#### Comparing `carburetor-4.0.3/carburetor/ui/main.ui` & `carburetor-4.1.0/carburetor/ui/main.ui`

```diff
@@ -1,9 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- Created with Cambalache 0.10.3 -->
+<!-- Created with Cambalache 0.12.0 -->
+<!-- Danial Behzadi <dani.behzi@ubuntu.com>, 2022-2023-->
 <interface>
   <!-- interface-name caburetor.ui -->
   <!-- interface-description This file is part of Carburetor. -->
   <!-- interface-copyright Carburetor is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -49,18 +50,18 @@
             </child>
           </object>
         </child>
         <child>
           <object class="GtkOverlay" id="ProgressOverlay">
             <child type="overlay">
               <object class="GtkProgressBar" id="ProgressBar">
+                <property name="valign">start</property>
                 <style>
                   <class name="osd"/>
                 </style>
-                <property name="valign">start</property>
               </object>
             </child>
             <child>
               <object class="AdwToastOverlay" id="ToastOverlay">
                 <child>
                   <object class="AdwStatusPage" id="MainPage">
                     <property name="hexpand">True</property>
@@ -82,8 +83,41 @@
               </object>
             </child>
           </object>
         </child>
       </object>
     </child>
   </object>
+  <!-- Custom fragments -->
+  <menu id="AppMenu">
+    <section>
+      <item>
+        <attribute name="label" translatable="yes">Preferences</attribute>
+        <attribute name="action">app.preferences</attribute>
+      </item>
+      <item>
+        <attribute name="label" translatable="yes">About Carburetor</attribute>
+        <attribute name="action">app.about</attribute>
+      </item>
+      <item>
+        <attribute name="label" translatable="yes">Quit</attribute>
+        <attribute name="action">app.quit</attribute>
+      </item>
+    </section>
+  </menu>
+  <menu id="ActionMenu">
+    <section>
+      <item>
+        <attribute name="label" translatable="yes">_New ID</attribute>
+        <attribute name="action">app.new_id</attribute>
+      </item>
+      <item>
+        <attribute name="label" translatable="yes">_Check connection</attribute>
+        <attribute name="action">app.check_connection</attribute>
+      </item>
+      <item>
+        <attribute name="label" translatable="yes">_Toggle proxy on system</attribute>
+        <attribute name="action">app.toggle_proxy</attribute>
+      </item>
+    </section>
+  </menu>
 </interface>
```

### Comparing `carburetor-4.0.3/carburetor/ui/preferences.ui` & `carburetor-4.1.0/carburetor/ui/preferences.ui`

 * *Files 1% similar despite different names*

#### Comparing `carburetor-4.0.3/carburetor/ui/preferences.ui` & `carburetor-4.1.0/carburetor/ui/preferences.ui`

```diff
@@ -1,9 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- Created with Cambalache 0.10.3 -->
+<!-- Created with Cambalache 0.12.0 -->
+<!-- Danial Behzadi <dani.behzi@ubuntu.com>, 2022-2023-->
 <interface>
   <!-- interface-name preferences.ui -->
   <!-- interface-description This file is part of Carburetor. -->
   <!-- interface-copyright Carburetor is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -157,14 +158,15 @@
                     <property name="orientation">vertical</property>
                     <child>
                       <object class="GtkScrolledWindow">
                         <property name="vexpand">True</property>
                         <child>
                           <object class="GtkTextView" id="BridgesTextView">
                             <property name="accepts-tab">False</property>
+                            <property name="css-classes">bridgeslist</property>
                             <property name="input-hints">no-emoji | no-spellcheck</property>
                             <signal name="realize" handler="on_bridgetextview_realize"/>
                           </object>
                         </child>
                       </object>
                     </child>
                     <child>
```

### Comparing `carburetor-4.0.3/carburetor/ui.py` & `carburetor-4.1.0/carburetor/ui.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 
 def initialize_builder() -> None:
     """
     connect builder to files and handlers
     """
     builder.add_from_file(ui_dir + "/about.ui")
     builder.add_from_file(ui_dir + "/preferences.ui")
-    builder.add_from_file(ui_dir + "/actionmenu.ui")
-    builder.add_from_file(ui_dir + "/mainmenu.ui")
     builder.add_from_file(ui_dir + "/main.ui")
 
 
 def get(obj: str):
     """
     get object from ui
     """
```


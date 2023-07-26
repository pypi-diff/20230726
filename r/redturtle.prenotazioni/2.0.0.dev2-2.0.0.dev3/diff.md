# Comparing `tmp/redturtle.prenotazioni-2.0.0.dev2.tar.gz` & `tmp/redturtle.prenotazioni-2.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redturtle.prenotazioni-2.0.0.dev2.tar", last modified: Fri Jun 30 10:39:22 2023, max compression
+gzip compressed data, was "redturtle.prenotazioni-2.0.0.dev3.tar", last modified: Thu Jul 20 07:22:36 2023, max compression
```

## Comparing `redturtle.prenotazioni-2.0.0.dev2.tar` & `redturtle.prenotazioni-2.0.0.dev3.tar`

### file list

```diff
@@ -1,284 +1,284 @@
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.425210 redturtle.prenotazioni-2.0.0.dev2/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      748 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/APP_IO.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6889 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/CHANGES.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       79 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/CONTRIBUTORS.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      586 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/DEVELOP.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/LICENSE.GPL
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/LICENSE.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      110 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/MANIFEST.in
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    24498 2023-06-30 10:39:22.425210 redturtle.prenotazioni-2.0.0.dev2/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    16268 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/README.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      164 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/TODO.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      105 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/constraints-5.2.x.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       27 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/constraints.txt
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.401210 redturtle.prenotazioni-2.0.0.dev2/docs/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7921 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/docs/conf.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       89 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/docs/index.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      476 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/requirements-6.0.x.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       48 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/requirements.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      344 2023-06-30 10:39:22.425210 redturtle.prenotazioni-2.0.0.dev2/setup.cfg
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3282 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/setup.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.397210 redturtle.prenotazioni-2.0.0.dev2/src/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.401210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.405210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2297 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.405210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/actions/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/actions/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      226 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/actions/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3325 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/actions/mail.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.405210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5157 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/booker.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4924 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4440 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/conflict.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3979 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/ical.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/prenotazione_menu.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8479 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/slot.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6903 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/stringinterp.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1816 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/base.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7260 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      541 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/custom_radio_input.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4782 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/delete_reservation.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      674 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/folderfactories.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      155 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/interfaces.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/overrides/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/overrides/.gitkeep
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3168 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazione.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    14679 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazione_add.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6919 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazione_move.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2038 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazione_print.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    30638 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1736 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    11366 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazioni_search.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/.gitkeep
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      364 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/calendar-add.png
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      503 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/calendar-icon.png
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      266 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/cross-icon.png
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9794 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1600 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      922 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/times-solid.png
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.397210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.397210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2108 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2377 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map
--rw-rw-r--   0 mauro     (1000) mauro     (1000)   342590 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      148 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js.map
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4616 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4486 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1059 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2718 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.less
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1555 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      103 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.less
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1507 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      961 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1261 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/index.js
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.409210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/utils/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      941 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      298 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/utils/widgetContext.js
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.413210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/stats/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/stats/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      614 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/stats/booking_stats.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3862 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/stats/booking_stats.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      575 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/stats/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.413210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2809 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1860 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5466 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2300 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       42 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/nofollow.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8165 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    10429 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    15258 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2266 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5916 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4895 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1892 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/week.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      333 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/week_table_overrides_widget_input.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9540 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/vacations.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1524 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/viewlets.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    10867 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/week.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1193 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/widget.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6310 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/z3c_custom_widget.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      383 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/config.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2327 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.413210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1785 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/pause.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7355 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/prenotazione.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      367 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/prenotazioni_day.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    17762 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/prenotazioni_folder.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      371 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/prenotazioni_week.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      371 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/prenotazioni_year.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8119 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/validators.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.413210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/contentrules/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/contentrules/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2080 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/contentrules/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      214 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/contentrules/handlers.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6160 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.413210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1567 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1860 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/events_logger.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      835 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/prenotazione.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1189 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/prenotazioni_folder.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.413210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/indexers/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/indexers/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      211 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/indexers/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      832 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/indexers/searchable_text.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1191 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/indexes.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      519 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/interfaces.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.397210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/en/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    35726 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.397210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/it/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    45854 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      830 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/manual.pot
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    35854 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1618 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/update.py
--rwxrwxr-x   0 mauro     (1000) mauro     (1000)      503 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/update.sh
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/monkeypatcher/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/monkeypatcher/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      499 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/monkeypatcher/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1282 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/permissions.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      478 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/prenotazione_event.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.397210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2345 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/actions.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      192 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/browserlayer.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      166 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/catalog.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6288 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/contentrules.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      325 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/metadata.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/registry/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5093 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/registry/caching.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1980 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/registry/resources.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      914 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/registry/settings.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1645 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/rolemap.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3551 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3811 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3094 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3795 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3796 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      564 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.397210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7373 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7623 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      540 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/to_1402/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1381 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/to_1500/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      196 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/to_1500/types.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/uninstall/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      132 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/uninstall/browserlayer.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/uninstall/registry/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      412 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/uninstall/registry/resources.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      123 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/uninstall/registry/settings.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      199 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/adapters/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/adapters/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      309 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/adapters/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3380 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      559 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      162 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.417210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4469 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/add.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1015 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1152 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/delete.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1166 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.421210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking_schema/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking_schema/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      409 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking_schema/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4198 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.421210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/bookings/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/bookings/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      279 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1926 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/bookings/search.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      308 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.421210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/month_slots/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/month_slots/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      395 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/month_slots/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2209 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/month_slots/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.421210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/week_slots/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/week_slots/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      392 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/week_slots/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2998 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/week_slots/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.421210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6955 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/app_io.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.421210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5302 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/README.md
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      246 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8614 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/api.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1034 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/cli.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    16384 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/io.db
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       45 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/io_tools.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1945 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/monkey.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2825 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/rdbms.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    27521 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/spec.yaml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      961 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/storage.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1062 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/setuphandlers.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3271 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/testing.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.421210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6283 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_booking_info.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8479 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_booking_schema.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8293 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_delete_booking.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9673 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_delete_booking_api.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    10405 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_month_slots.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5762 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_prenotazione.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5913 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8811 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9432 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_send_ical.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3536 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_setup.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    12116 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_week_table_overrides.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6301 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/upgrades.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2798 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/upgrades.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.421210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/utilities/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/utilities/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/utilities/dateutils.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1119 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/utilities/urls.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.425210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/viewlets/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/viewlets/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      472 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/viewlets/app_io.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      593 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/viewlets/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.425210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/viewlets/templates/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      957 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/viewlets/templates/app_io.pt
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.425210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1096 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      607 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/gates.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1010 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      598 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/review_states.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1696 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/tipologies.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1054 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2549 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/voc_months.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1367 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-30 10:39:22.401210 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    24498 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    12266 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/SOURCES.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/dependency_links.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      179 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/entry_points.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/namespace_packages.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/not-zip-safe
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      399 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/requires.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-06-30 10:39:22.000000 redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/top_level.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.826599 redturtle.prenotazioni-2.0.0.dev3/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      748 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/APP_IO.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7013 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/CHANGES.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       79 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/CONTRIBUTORS.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      586 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/DEVELOP.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/LICENSE.GPL
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/LICENSE.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      110 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/MANIFEST.in
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    24622 2023-07-20 07:22:36.826599 redturtle.prenotazioni-2.0.0.dev3/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    16268 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/README.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      164 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/TODO.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      105 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/constraints-5.2.x.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       27 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/constraints.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.802598 redturtle.prenotazioni-2.0.0.dev3/docs/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7921 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/docs/conf.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       89 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/docs/index.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      476 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/requirements-6.0.x.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       48 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/requirements.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      344 2023-07-20 07:22:36.826599 redturtle.prenotazioni-2.0.0.dev3/setup.cfg
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3282 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/setup.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.798598 redturtle.prenotazioni-2.0.0.dev3/src/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.806598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.806598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2297 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.806598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/actions/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/actions/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      226 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/actions/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3325 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/actions/mail.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.806598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/adapters/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/adapters/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5157 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/adapters/booker.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4924 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/adapters/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4440 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/adapters/conflict.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3979 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/adapters/ical.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/adapters/prenotazione_menu.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8479 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/adapters/slot.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6903 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/adapters/stringinterp.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.810598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1816 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/base.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7260 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      541 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/custom_radio_input.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4782 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/delete_reservation.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      674 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/folderfactories.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      155 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/interfaces.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.810598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/overrides/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/overrides/.gitkeep
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3168 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    14679 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/prenotazione_add.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6919 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/prenotazione_move.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2038 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/prenotazione_print.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    30643 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1736 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    11366 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/prenotazioni_search.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.810598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/.gitkeep
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      364 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/calendar-add.png
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      503 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/calendar-icon.png
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      266 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/cross-icon.png
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9794 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1600 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      922 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/times-solid.png
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.798598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.798598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/dist/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.810598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/dist/prod/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2108 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2377 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)   342590 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      148 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js.map
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.810598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.810598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4616 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.810598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4486 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1059 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.814598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/fields/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2718 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.less
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1555 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      103 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.less
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1507 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      961 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1261 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/index.js
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.814598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/utils/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      941 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      298 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/utils/widgetContext.js
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.814598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/stats/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/stats/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      614 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/stats/booking_stats.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3862 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/stats/booking_stats.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      575 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/stats/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.814598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2809 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1860 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5466 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2300 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       42 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/nofollow.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8165 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/prenotazione.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    10429 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    15258 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2266 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5916 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4895 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1892 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/week.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      333 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/week_table_overrides_widget_input.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9540 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/vacations.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1524 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/viewlets.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    10867 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/week.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1193 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/widget.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6310 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/z3c_custom_widget.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      383 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/config.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2327 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.814598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/content/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/content/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1785 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/content/pause.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7483 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/content/prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      367 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/content/prenotazioni_day.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    17970 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/content/prenotazioni_folder.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      371 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/content/prenotazioni_week.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      371 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/content/prenotazioni_year.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8119 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/content/validators.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.814598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/contentrules/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/contentrules/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2080 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/contentrules/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      214 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/contentrules/handlers.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6160 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.814598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/events/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/events/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1567 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/events/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1860 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/events/events_logger.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      835 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/events/prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1189 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/events/prenotazioni_folder.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.818598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/indexers/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/indexers/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      211 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/indexers/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      832 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/indexers/searchable_text.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1191 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/indexes.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      519 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/interfaces.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.818598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/locales/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.798598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/locales/en/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.818598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    35726 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.798598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/locales/it/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.818598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    45845 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      830 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/locales/manual.pot
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    35854 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1618 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/locales/update.py
+-rwxrwxr-x   0 mauro     (1000) mauro     (1000)      503 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/locales/update.sh
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.818598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/monkeypatcher/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/monkeypatcher/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      499 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/monkeypatcher/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1282 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/permissions.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      478 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/prenotazione_event.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.802598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.818598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2345 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/actions.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      192 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/browserlayer.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      166 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/catalog.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6288 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/contentrules.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      325 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/metadata.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.818598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/registry/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5093 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/registry/caching.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1980 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/registry/resources.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      914 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/registry/settings.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1645 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/rolemap.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.818598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/types/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3551 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3811 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3094 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3795 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3796 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      564 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/types.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.798598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/workflows/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.818598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7373 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.818598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7623 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      540 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/workflows.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.818598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/to_1402/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1381 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.818598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/to_1500/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      196 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/to_1500/types.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.818598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/uninstall/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      132 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/uninstall/browserlayer.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.818598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/uninstall/registry/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      412 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/uninstall/registry/resources.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      123 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/uninstall/registry/settings.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.818598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      199 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.818598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/serializers/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/serializers/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.822598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/serializers/adapters/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/serializers/adapters/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      309 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/serializers/adapters/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3506 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      558 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      162 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/serializers/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.822598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.822598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/booking/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/booking/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4469 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/booking/add.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1015 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1152 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/booking/delete.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1166 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/booking/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.822598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/booking_schema/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/booking_schema/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      409 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/booking_schema/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4198 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.822598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/bookings/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/bookings/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      506 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2212 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/bookings/search.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      308 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.822598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/month_slots/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/month_slots/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      395 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/month_slots/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2209 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/month_slots/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.822598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/week_slots/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/week_slots/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      392 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/week_slots/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2998 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/week_slots/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.822598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6955 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/app_io.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.822598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5302 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/README.md
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      246 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8614 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/api.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1034 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/cli.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    16384 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/io.db
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       45 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/io_tools.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1945 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/monkey.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2825 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/rdbms.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    27521 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/spec.yaml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      961 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/storage.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1062 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/setuphandlers.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3271 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/testing.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.826599 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6283 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_booking_info.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8479 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_booking_schema.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8293 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_delete_booking.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9673 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_delete_booking_api.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    10405 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_month_slots.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5762 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5913 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8473 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9432 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_send_ical.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3536 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_setup.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    12116 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_week_table_overrides.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6301 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/upgrades.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2798 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/upgrades.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.826599 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/utilities/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/utilities/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/utilities/dateutils.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1119 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/utilities/urls.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.826599 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/viewlets/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/viewlets/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      472 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/viewlets/app_io.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      593 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/viewlets/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.826599 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/viewlets/templates/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      957 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/viewlets/templates/app_io.pt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.826599 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1096 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      607 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/gates.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1010 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      598 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/review_states.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1696 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/tipologies.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1054 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2549 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/voc_months.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1367 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-20 07:22:36.806598 redturtle.prenotazioni-2.0.0.dev3/src/redturtle.prenotazioni.egg-info/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    24622 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle.prenotazioni.egg-info/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    12266 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle.prenotazioni.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle.prenotazioni.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      179 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle.prenotazioni.egg-info/entry_points.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle.prenotazioni.egg-info/namespace_packages.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle.prenotazioni.egg-info/not-zip-safe
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      399 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle.prenotazioni.egg-info/requires.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-07-20 07:22:36.000000 redturtle.prenotazioni-2.0.0.dev3/src/redturtle.prenotazioni.egg-info/top_level.txt
```

### Comparing `redturtle.prenotazioni-2.0.0.dev2/APP_IO.txt` & `redturtle.prenotazioni-2.0.0.dev3/APP_IO.txt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/CHANGES.rst` & `redturtle.prenotazioni-2.0.0.dev3/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Changelog
 =========
 
 
+2.0.0.dev3 (2023-07-20)
+-----------------------
+
+- Change "day" type in week_table (TODO: need an upgrade step?)
+  [mauro]
+
 2.0.0.dev2 (2023-06-30)
 -----------------------
 
 - reorganize backend form
   [mamico]
 
 - booking_type filter in @months-slots
```

### Comparing `redturtle.prenotazioni-2.0.0.dev2/DEVELOP.rst` & `redturtle.prenotazioni-2.0.0.dev3/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/LICENSE.GPL` & `redturtle.prenotazioni-2.0.0.dev3/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/LICENSE.rst` & `redturtle.prenotazioni-2.0.0.dev3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/PKG-INFO` & `redturtle.prenotazioni-2.0.0.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.prenotazioni
-Version: 2.0.0.dev2
+Version: 2.0.0.dev3
 Summary: An add-on for Plone
 Home-page: https://github.com/redturtle/redturtle.prenotazioni
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/redturtle.prenotazioni
 Project-URL: Source, https://github.com/redturtle/redturtle.prenotazioni
@@ -633,14 +633,20 @@
 - Daniele Andreotti, daniele.andreotti@redturtle.it
 
 
 Changelog
 =========
 
 
+2.0.0.dev3 (2023-07-20)
+-----------------------
+
+- Change "day" type in week_table (TODO: need an upgrade step?)
+  [mauro]
+
 2.0.0.dev2 (2023-06-30)
 -----------------------
 
 - reorganize backend form
   [mamico]
 
 - booking_type filter in @months-slots
```

### Comparing `redturtle.prenotazioni-2.0.0.dev2/README.rst` & `redturtle.prenotazioni-2.0.0.dev3/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/docs/conf.py` & `redturtle.prenotazioni-2.0.0.dev3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/setup.py` & `redturtle.prenotazioni-2.0.0.dev3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="redturtle.prenotazioni",
-    version="2.0.0.dev2",
+    version="2.0.0.dev3",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/__init__.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/actions/mail.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/actions/mail.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/booker.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/adapters/booker.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/adapters/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/conflict.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/adapters/conflict.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/ical.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/adapters/ical.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/slot.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/adapters/slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/adapters/stringinterp.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/adapters/stringinterp.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/base.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/base.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/custom_radio_input.pt` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/custom_radio_input.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/delete_reservation.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/delete_reservation.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/folderfactories.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/folderfactories.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazione_add.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/prenotazione_add.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazione_move.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/prenotazione_move.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazione_print.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/prenotazione_print.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -609,15 +609,15 @@
     def get_pauses_in_day_folder(self, booking_date):
         """
         This method takes all pauses from the week table and convert it on slot
         :param booking_date: a date as a datetime or a string
         """
         weekday = booking_date.weekday()
         pause_table = self.context.pause_table or []
-        today_pauses = [row for row in pause_table if row["day"] == weekday]
+        today_pauses = [row for row in pause_table if row["day"] == str(weekday)]
         pauses = []
         if today_pauses:
             for pause in today_pauses:
                 pause = Pause(
                     pause["pause_start"][:2] + ":" + pause["pause_start"][2:],
                     pause["pause_end"][:2] + ":" + pause["pause_end"][2:],
                     "",
```

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/prenotazioni_search.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/prenotazioni_search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/times-solid.png` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/times-solid.png`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/index.js` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/stats/booking_stats.pt` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/stats/booking_stats.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/stats/booking_stats.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/stats/booking_stats.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/stats/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/stats/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione.pt` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/prenotazione.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/templates/week.pt` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/templates/week.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/vacations.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/vacations.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/viewlets.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/week.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/week.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/widget.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/widget.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/browser/z3c_custom_widget.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/browser/z3c_custom_widget.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/pause.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/content/pause.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/content/prenotazione.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,16 @@
     reg_tool = api.portal.get_tool(name="portal_registration")
     if value and reg_tool.isValidEmail(value):
         return True
     else:
         raise InvalidEmailAddress
 
 
+# TODO: validare considerando anche TINIT-XXX...
+# (vedi https://it.wikipedia.org/wiki/Codice_fiscale#Codice_fiscale_ordinario)
 def check_valid_fiscalcode(value):
     # fiscal code development
     if value == "AAAAAA00A00A000A":
         return True
     if not value:
         return True
     value = value.upper()
```

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/prenotazioni_folder.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/content/prenotazioni_folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,17 +60,22 @@
             )
         data.append(row_data)
     return data
 
 
 class IWeekTableRow(model.Schema):
     day = schema.TextLine(
-        title=_("day_label", default="Day of week"), required=True, default=""
+        title=_("day_label", default="Day of week"),
+        required=True,
+        default="",
     )
-    form.mode(day="display")
+    # TODO: sarebbe bello, ma datagrid non funziona:
+    # su plone si rompe, su volto non considera il mode=display
+    # ancora peggio readonly=true sul field
+    # form.mode(day="display")
     morning_start = schema.Choice(
         title=_("morning_start_label", default="Start time in the morning"),
         vocabulary="redturtle.prenotazioni.VocOreInizio",
         required=False,
     )
     morning_end = schema.Choice(
         title=_("morning_end_label", default="End time in the morning"),
@@ -94,21 +99,21 @@
 class IPauseTableRow(model.Schema):
     day = schema.Choice(
         title=_("day_label", default="Day of week"),
         required=True,
         vocabulary=SimpleVocabulary(
             [
                 SimpleTerm(value=None, token=None, title=_("Select a day")),
-                SimpleTerm(value=0, token=0, title=_("Monday")),
-                SimpleTerm(value=1, token=1, title=_("Tuesday")),
-                SimpleTerm(value=2, token=2, title=_("Wednesday")),
-                SimpleTerm(value=3, token=3, title=_("Thursday")),
-                SimpleTerm(value=4, token=4, title=_("Friday")),
-                SimpleTerm(value=5, token=5, title=_("Saturday")),
-                SimpleTerm(value=6, token=6, title=_("Sunday")),
+                SimpleTerm(value="0", token="0", title=_("Monday")),
+                SimpleTerm(value="1", token="1", title=_("Tuesday")),
+                SimpleTerm(value="2", token="2", title=_("Wednesday")),
+                SimpleTerm(value="3", token="3", title=_("Thursday")),
+                SimpleTerm(value="4", token="4", title=_("Friday")),
+                SimpleTerm(value="5", token="5", title=_("Saturday")),
+                SimpleTerm(value="6", token="6", title=_("Sunday")),
             ]
         ),
     )
     pause_start = schema.Choice(
         title=_("pause_start_label", default="Pause start"),
         vocabulary="redturtle.prenotazioni.VocOreInizio",
         required=False,
```

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/content/validators.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/content/validators.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/contentrules/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/contentrules/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/events_logger.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/events/events_logger.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/events/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/events/prenotazioni_folder.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/events/prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/indexers/searchable_text.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/indexers/searchable_text.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/indexes.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/indexes.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/interfaces.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/interfaces.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:398
 msgid "Insert here the contact phone"
 msgstr "Inserire il numero di telefono per contattare l'ufficio"
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:295
 msgid "Insert pause table schema."
-msgstr "Inserisci le pause giornaliere. Esistono tre tipi di vincolo: una data di termine pausa deve essere maggiore maggiore della data di inizio pausa; le pause nello stesso giorno non possono sovrapporsi; le pause devono essere comprese fra l'inizio e la fine dell'orario di lavoro."
+msgstr "Inserisci le pause giornaliere. Esistono tre tipi di vincolo: una data di termine pausa deve essere maggiore della data di inizio pausa; le pause nello stesso giorno non possono sovrapporsi; le pause devono essere comprese fra l'inizio e la fine dell'orario di lavoro."
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:224
 msgid "Insert week table schema."
 msgstr "Compila la tabella degli orari della settimana."
 
 #: redturtle/prenotazioni/configure.zcml:31
 msgid "Installs the redturtle.prenotazioni add-on."
```

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/manual.pot` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/locales/update.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/locales/update.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/permissions.zcml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/permissions.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/actions.xml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/contentrules.xml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/contentrules.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/registry/caching.xml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/registry/resources.xml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/registry/resources.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/registry/settings.xml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/registry/settings.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/rolemap.xml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/types.xml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/default/workflows.xml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,29 +13,33 @@
 
 
 @implementer(ISerializeToJson)
 @adapter(IPrenotazione, IRequest)
 class PrenotazioneSerializer:
     def __init__(self, prenotazione, request):
         self.prenotazione = prenotazione
-        self.reqeuest = request
+        self.request = request
 
     def __call__(self, *args, **kwargs):
         booking_folder = self.prenotazione.getPrenotazioniFolder()
         useful_docs = getattr(booking_folder, "cosa_serve", "")
+        if self.prenotazione.fiscalcode:
+            fiscalcode = self.prenotazione.fiscalcode.upper()
+        else:
+            fiscalcode = None
         return {
             "UID": self.prenotazione.UID(),
             "@type": self.prenotazione.portal_type,
             "title": self.prenotazione.title,
             "description": self.prenotazione.description,
             "gate": self.prenotazione.gate,
             "id": self.prenotazione.id,
             "phone": self.prenotazione.phone,
             "email": self.prenotazione.email,
-            "fiscalcode": self.prenotazione.fiscalcode,
+            "fiscalcode": fiscalcode,
             "company": self.prenotazione.company,
             "staff_notes": self.prenotazione.staff_notes,
             "booking_date": datetimelike_to_iso(self.prenotazione.booking_date),
             "booking_expiration_date": datetimelike_to_iso(
                 self.prenotazione.booking_expiration_date
             ),
             "booking_type": self.prenotazione.booking_type,
@@ -45,15 +49,15 @@
 
 
 @implementer(ISerializeToPrenotazioneSearchableItem)
 @adapter(IPrenotazione, IRequest)
 class PrenotazioneSearchableItemSerializer:
     def __init__(self, prenotazione, request):
         self.prenotazione = prenotazione
-        self.reqeuest = request
+        self.request = request
 
     def __call__(self, *args, **kwargs):
         wf_tool = api.portal.get_tool("portal_workflow")
         status = wf_tool.getStatusOf("prenotazioni_workflow", self.prenotazione)
 
         return {
             "booking_id": self.prenotazione.UID(),
@@ -64,15 +68,15 @@
                 self.prenotazione.booking_expiration_date
             ),
             "booking_type": self.prenotazione.booking_type,
             # "booking_room": None,
             "booking_gate": self.prenotazione.gate,
             "booking_status": status["review_state"],
             "booking_status_label": translate(
-                status["review_state"], context=self.reqeuest
+                status["review_state"], context=self.request
             ),
             "booking_status_date": datetimelike_to_iso(status["time"]),
             "booking_status_notes": status["comments"],
             "email": self.prenotazione.email,
             "fiscalcode": self.prenotazione.fiscalcode,
             "phone": self.prenotazione.phone,
             "staff_notes": self.prenotazione.staff_notes,
```

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 
 
 @implementer(ISerializeToJson)
 @adapter(ISlot, IRequest)
 class SlotSerializer:
     def __init__(self, context, request):
         self.context = context
-        self.reqeuest = request
+        self.request = request
 
     def __call__(self, *args, **kwargs):
         return {"start": self.context.start(), "stop": self.context.stop()}
```

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/add.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/booking/add.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/delete.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/booking/delete.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking/get.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/booking/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/bookings/search.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/bookings/search.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,42 +16,48 @@
     """
 
     def publishTraverse(self, request, userid):
         if not request.get("userid", None):
             request.set("userid", userid)
         return self
 
-    def reply(self):
-        start_date = self.request.get("from", None)
-        end_date = self.request.get("to", None)
-
+    def query(self):
+        query = {
+            "portal_type": "Prenotazione",
+        }
         if api.user.is_anonymous():
             raise Unauthorized("You must be logged in to perform this action")
         elif api.user.has_permission("redturtle.prenotazioni: search prenotazioni"):
             userid = self.request.get("userid", None)
         else:
             userid = api.user.get_current().getUserId()
-
-        response = {"id": self.context.absolute_url() + "/@bookings"}
-        query = {
-            "portal_type": "Prenotazione",
-        }
-
+        if userid:
+            query["fiscalcode"] = userid.upper()
+        start_date = self.request.get("from", None)
+        end_date = self.request.get("to", None)
         if start_date or end_date:
             query["Date"] = {
                 "query": [DateTime(i) for i in [start_date, end_date] if i],
                 "range": f"{start_date and 'min' or ''}{start_date and end_date and ':' or ''}{end_date and 'max' or ''}",  # noqa: E501
             }
+        return query
 
-        if userid:
-            query["fiscalcode"] = userid
-
+    def reply(self):
+        response = {"id": self.context.absolute_url() + "/@bookings"}
+        query = self.query()
         response["items"] = [
             getMultiAdapter(
                 (i.getObject(), self.request),
                 ISerializeToPrenotazioneSearchableItem,
             )()
             for i in api.portal.get_tool("portal_catalog")(**query)
         ]
         response["items_total"] = len(response["items"])
 
         return response
+
+
+class BookingsSearchFolder(BookingsSearch):
+    def query(self):
+        query = super(BookingsSearchFolder, self).query()
+        query["path"] = "/".join(self.context.getPhysicalPath())
+        return query
```

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/month_slots/get.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/month_slots/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/restapi/services/week_slots/get.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/restapi/services/week_slots/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/app_io.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/app_io.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/README.md` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/README.md`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/api.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/cli.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/cli.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/io.db` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/io.db`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/monkey.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/monkey.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/rdbms.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/rdbms.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/spec.yaml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/spec.yaml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/scripts/io_tools/storage.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/scripts/io_tools/storage.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/setuphandlers.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/testing.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/testing.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_booking_info.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_booking_info.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_booking_schema.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_booking_schema.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_delete_booking.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_delete_booking.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_delete_booking_api.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_delete_booking_api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_month_slots.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_month_slots.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_send_ical.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,43 @@
-# -*- coding: utf-8 -*-
-from datetime import date
+# -*- coding: UTF-8 -*-
+from collective.contentrules.mailfromfield.actions.mail import MailFromFieldAction
+from datetime import date, datetime
 from datetime import timedelta
-from dateutil import parser
 from plone import api
 from plone.app.testing import setRoles
-from plone.app.testing import SITE_OWNER_NAME
-from plone.app.testing import SITE_OWNER_PASSWORD
 from plone.app.testing import TEST_USER_ID
-from plone.app.testing import TEST_USER_PASSWORD
-from plone.restapi.testing import RelativeSession
-from redturtle.prenotazioni.testing import (
-    REDTURTLE_PRENOTAZIONI_API_FUNCTIONAL_TESTING,
-)
+from plone.contentrules.rule.interfaces import IExecutable
+from Products.CMFCore.WorkflowCore import ActionSucceededEvent
+from redturtle.prenotazioni.adapters.booker import IBooker
+from redturtle.prenotazioni.prenotazione_event import MovedPrenotazione
+from redturtle.prenotazioni.testing import REDTURTLE_PRENOTAZIONI_FUNCTIONAL_TESTING
+from zope.component import getMultiAdapter
+from zope.interface import implementer
+from zope.interface.interfaces import IObjectEvent
 
-import transaction
+import base64
+import email
 import unittest
 
 
-class TestPrenotazioniSearch(unittest.TestCase):
-    """Test the restapi search endpoint (<portal_url>/@bookings)"""
+@implementer(IObjectEvent)
+class DummyEvent(object):
+    def __init__(self, object):
+        self.object = object
 
-    layer = REDTURTLE_PRENOTAZIONI_API_FUNCTIONAL_TESTING
+
+class TestSendIcal(unittest.TestCase):
+    layer = REDTURTLE_PRENOTAZIONI_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
-        self.portal_url = self.portal.absolute_url()
-        self.testing_fiscal_code = "TESTINGFISCALCODE"
-        self.testing_booking_date = parser.parse("2023-04-28 16:00:00")
-        self.booking_expiration_date = parser.parse("2023-04-28 16:00:00") + timedelta(
-            days=100
-        )
-
+        self.mailhost = self.portal.MailHost
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
 
-        self.api_session = RelativeSession(self.portal_url)
-        self.api_session.headers.update({"Accept": "application/json"})
-        self.api_session.auth = (SITE_OWNER_NAME, SITE_OWNER_PASSWORD)
-
         self.folder_prenotazioni = api.content.create(
             container=self.portal,
             type="PrenotazioniFolder",
             title="Prenota foo",
             description="",
             daData=date.today(),
             week_table=[
@@ -50,183 +46,242 @@
                     "morning_start": "0700",
                     "morning_end": "1000",
                     "afternoon_start": None,
                     "afternoon_end": None,
                 },
                 {
                     "day": "Martedì",
-                    "morning_start": None,
-                    "morning_end": None,
+                    "morning_start": "0700",
+                    "morning_end": "1000",
                     "afternoon_start": None,
                     "afternoon_end": None,
                 },
                 {
                     "day": "Mercoledì",
-                    "morning_start": None,
-                    "morning_end": None,
+                    "morning_start": "0700",
+                    "morning_end": "1000",
                     "afternoon_start": None,
                     "afternoon_end": None,
                 },
                 {
                     "day": "Giovedì",
-                    "morning_start": None,
-                    "morning_end": None,
+                    "morning_start": "0700",
+                    "morning_end": "1000",
                     "afternoon_start": None,
                     "afternoon_end": None,
                 },
                 {
                     "day": "Venerdì",
-                    "morning_start": None,
-                    "morning_end": None,
+                    "morning_start": "0700",
+                    "morning_end": "1000",
                     "afternoon_start": None,
                     "afternoon_end": None,
                 },
                 {
                     "day": "Sabato",
-                    "morning_start": None,
-                    "morning_end": None,
+                    "morning_start": "0700",
+                    "morning_end": "1000",
                     "afternoon_start": None,
                     "afternoon_end": None,
                 },
                 {
                     "day": "Domenica",
-                    "morning_start": None,
-                    "morning_end": None,
+                    "morning_start": "0700",
+                    "morning_end": "1000",
                     "afternoon_start": None,
                     "afternoon_end": None,
                 },
             ],
             booking_types=[
                 {"name": "Type A", "duration": "30"},
             ],
             gates=["Gate A"],
         )
+        self.today = datetime.now().replace(hour=8)
+        self.tomorrow = self.today + timedelta(1)
 
-        year = api.content.create(
-            container=self.folder_prenotazioni,
-            type="PrenotazioniYear",
-            title="Year",
-        )
-        week = api.content.create(container=year, type="PrenotazioniWeek", title="Week")
-        self.day_folder = api.content.create(
-            container=week, type="PrenotazioniDay", title="Day"
-        )
-        self.day_folder1 = api.content.create(
-            container=week, type="PrenotazioniDay", title="Day"
-        )
-        self.day_folder2 = api.content.create(
-            container=week, type="PrenotazioniDay", title="Day"
-        )
-
-        self.prenotazione_fscode = api.content.create(
-            container=self.day_folder,
-            type="Prenotazione",
-            title="Prenotazione",
-            booking_date=self.testing_booking_date - timedelta(days=2),
-            booking_expiration_date=self.booking_expiration_date,
-            fiscalcode=self.testing_fiscal_code,
-        )
-        self.prenotazione_no_fscode = api.content.create(
-            container=self.day_folder,
-            type="Prenotazione",
-            booking_date=self.testing_booking_date - timedelta(days=2),
-            booking_expiration_date=self.booking_expiration_date,
-            title="Prenotazione",
-        )
-        self.prenotazione_datetime = api.content.create(
-            container=self.day_folder,
-            type="Prenotazione",
-            title="Prenotazione",
-            booking_date=self.testing_booking_date,
-            booking_expiration_date=self.booking_expiration_date,
-            fiscalcode=self.testing_fiscal_code,
-        )
-        self.prenotazione_datetime_plus2 = api.content.create(
-            container=self.day_folder1,
-            type="Prenotazione",
-            title="Prenotazione",
-            booking_date=self.testing_booking_date + timedelta(days=2),
-            booking_expiration_date=self.booking_expiration_date,
-            fiscalcode=self.testing_fiscal_code,
-        )
-        self.prenotazione_datetime_plus4 = api.content.create(
-            container=self.day_folder2,
-            type="Prenotazione",
-            title="Prenotazione",
-            booking_date=self.testing_booking_date + timedelta(days=4),
-            booking_expiration_date=self.booking_expiration_date,
-            fiscalcode=self.testing_fiscal_code,
-        )
-        transaction.commit()
-
-    def tearDown(self):
-        self.api_session.close()
-
-    def test_view_permission(self):
-        self.assertEqual(
-            self.api_session.get(f"{self.portal.absolute_url()}/@bookings").status_code,
-            200,
-        )
-
-        setRoles(self.portal, TEST_USER_ID, [])
-
-        self.api_session.auth = (TEST_USER_ID, TEST_USER_PASSWORD)
-
-        self.assertEqual(
-            self.api_session.get(f"{self.portal.absolute_url()}/@bookings").status_code,
-            401,
-        )
-
-    def test_search_by_fiscalcode(self):
-        result_uids = [
-            i["booking_id"]
-            for i in self.api_session.get(
-                f"{self.portal.absolute_url()}/@bookings/{self.testing_fiscal_code}"  # noqa: E501
-            ).json()["items"]
-        ]
-
-        self.assertIn(self.prenotazione_fscode.UID(), result_uids)
-        self.assertNotIn(self.prenotazione_no_fscode.UID(), result_uids)
-
-    def test_search_by_fiscalcode_traverse(self):
-        res = self.api_session.get(
-            f"{self.portal.absolute_url()}/@bookings/{self.testing_fiscal_code}"
-        )
-        self.assertEqual(res.status_code, 200)
-        ids = [i["booking_id"] for i in res.json()["items"]]
-        self.assertIn(self.prenotazione_fscode.UID(), ids)
-        self.assertNotIn(self.prenotazione_no_fscode.UID(), ids)
-
-    def test_search_by_date(self):
-        # test by start date
-        res = self.api_session.get(
-            f"{self.portal.absolute_url()}/@bookings?from={str(self.testing_booking_date + timedelta(days=1))}&fiscalcode={self.testing_fiscal_code}"
-        )
-
-        self.assertEqual(res.status_code, 200)
-
-        ids = [i["booking_id"] for i in res.json()["items"]]
-        self.assertNotIn(self.prenotazione_datetime.UID(), ids)
-        self.assertIn(self.prenotazione_datetime_plus2.UID(), ids)
-
-        # test by end date
-        result_uids = [
-            i["booking_id"]
-            for i in self.api_session.get(
-                f"{self.portal.absolute_url()}/@bookings?to={str(self.testing_booking_date + timedelta(days=3))}&fiscalcode={self.testing_fiscal_code}"
-            ).json()["items"]
-        ]
-
-        self.assertIn(self.prenotazione_datetime_plus2.UID(), result_uids)
-        self.assertNotIn(self.prenotazione_datetime_plus4.UID(), result_uids)
-
-        # test btw strart and end date
-        result_uids = [
-            i["booking_id"]
-            for i in self.api_session.get(
-                f"{self.portal.absolute_url()}/@bookings?from={str(self.testing_booking_date + timedelta(days=1))}&to={str(self.testing_booking_date + timedelta(days=3))}&fiscalcode={self.testing_fiscal_code}"
-            ).json()["items"]
-        ]
-
-        self.assertIn(self.prenotazione_datetime_plus2.UID(), result_uids)
-        self.assertNotIn(self.prenotazione_datetime_plus4.UID(), result_uids)
-        self.assertNotIn(self.prenotazione_datetime.UID(), result_uids)
+    def create_booking(self):
+        booker = IBooker(self.folder_prenotazioni)
+        return booker.create(
+            {
+                "booking_date": self.tomorrow,  # tomorrow
+                "booking_type": "Type A",
+                "title": "foo",
+                "email": "jdoe@redturtle.it",
+            }
+        )
+
+    def test_ical_sent_on_confirm(self):
+        booking = self.create_booking()
+        e = MailFromFieldAction()
+        e.source = "foo@bar.be"
+        e.fieldName = "email"
+        e.target = "target"
+        e.message = "Test mail"
+        e.subject = "Subject"
+        ex = getMultiAdapter(
+            (
+                self.portal,
+                e,
+                ActionSucceededEvent(
+                    object=booking,
+                    workflow=None,
+                    action="confirm",
+                    result="",
+                ),
+            ),
+            IExecutable,
+        )
+        ex()
+        mailSent = self.mailhost.messages[0]
+        message = email.message_from_bytes(mailSent)
+
+        self.assertTrue(len(message.get_payload()), 2)
+
+        attachment = message.get_payload()[1]
+        data = base64.b64decode(attachment.get_payload()).decode("utf-8")
+
+        self.assertTrue(message.is_multipart())
+        self.assertEqual(attachment.get_filename(), "foo.ics")
+        self.assertIn("SUMMARY:Booking for Prenota foo", data)
+        if api.env.plone_version() < "6":
+            self.assertIn(
+                "DTSTART;VALUE=DATE-TIME:{}".format(
+                    booking.booking_date.strftime("%Y%m%dT%H%M%S")
+                ),
+                data,
+            )
+            self.assertIn(
+                "DTEND;VALUE=DATE-TIME:{}".format(
+                    booking.booking_expiration_date.strftime("%Y%m%dT%H%M%S")
+                ),
+                data,
+            )
+        else:
+            self.assertIn(
+                "DTSTART:{}".format(booking.booking_date.strftime("%Y%m%dT%H%M%S")),
+                data,
+            )
+            self.assertIn(
+                "DTEND:{}".format(
+                    booking.booking_expiration_date.strftime("%Y%m%dT%H%M%S")
+                ),
+                data,
+            )
+        self.assertIn("UID:{}".format(booking.UID()), data)
+
+    def test_ical_not_sent_on_refuse(self):
+        booking = self.create_booking()
+        e = MailFromFieldAction()
+        e.source = "foo@bar.be"
+        e.fieldName = "email"
+        e.target = "target"
+        e.message = "Test mail"
+        e.subject = "Subject"
+        ex = getMultiAdapter(
+            (
+                self.portal,
+                e,
+                ActionSucceededEvent(
+                    object=booking,
+                    workflow=None,
+                    action="refuse",
+                    result="",
+                ),
+            ),
+            IExecutable,
+        )
+        ex()
+        mailSent = self.mailhost.messages[0]
+        message = email.message_from_bytes(mailSent)
+
+        self.assertFalse(message.is_multipart())
+        self.assertEqual(message.get_payload(), "Test mail\n")
+
+    def test_ical_not_sent_on_submit(self):
+        booking = self.create_booking()
+        e = MailFromFieldAction()
+        e.source = "foo@bar.be"
+        e.fieldName = "email"
+        e.target = "target"
+        e.message = "Test mail"
+        e.subject = "Subject"
+        ex = getMultiAdapter(
+            (
+                self.portal,
+                e,
+                ActionSucceededEvent(
+                    object=booking,
+                    workflow=None,
+                    action="submit",
+                    result="",
+                ),
+            ),
+            IExecutable,
+        )
+        ex()
+        mailSent = self.mailhost.messages[0]
+        message = email.message_from_bytes(mailSent)
+
+        self.assertFalse(message.is_multipart())
+        self.assertEqual(message.get_payload(), "Test mail\n")
+
+    def test_ical_sent_on_move(self):
+        booking = self.create_booking()
+
+        # move date one day after
+        booking.booking_date = booking.booking_date + timedelta(1)
+        booking.booking_expiration_date = booking.booking_expiration_date + timedelta(1)
+
+        e = MailFromFieldAction()
+        e.source = "foo@bar.be"
+        e.fieldName = "email"
+        e.target = "target"
+        e.message = "Test mail"
+        e.subject = "Subject"
+        ex = getMultiAdapter(
+            (
+                self.portal,
+                e,
+                MovedPrenotazione(
+                    obj=booking,
+                ),
+            ),
+            IExecutable,
+        )
+        ex()
+        mailSent = self.mailhost.messages[0]
+        message = email.message_from_bytes(mailSent)
+
+        self.assertTrue(len(message.get_payload()), 2)
+
+        attachment = message.get_payload()[1]
+        data = base64.b64decode(attachment.get_payload()).decode("utf-8")
+
+        self.assertTrue(message.is_multipart())
+        self.assertEqual(attachment.get_filename(), "foo.ics")
+        self.assertIn("SUMMARY:Booking for Prenota foo", data)
+        if api.env.plone_version() < "6":
+            self.assertIn(
+                "DTSTART;VALUE=DATE-TIME:{}".format(
+                    booking.booking_date.strftime("%Y%m%dT%H%M%S")
+                ),
+                data,
+            )
+            self.assertIn(
+                "DTEND;VALUE=DATE-TIME:{}".format(
+                    booking.booking_expiration_date.strftime("%Y%m%dT%H%M%S")
+                ),
+                data,
+            )
+        else:
+            self.assertIn(
+                "DTSTART:{}".format(booking.booking_date.strftime("%Y%m%dT%H%M%S")),
+                data,
+            )
+            self.assertIn(
+                "DTEND:{}".format(
+                    booking.booking_expiration_date.strftime("%Y%m%dT%H%M%S")
+                ),
+                data,
+            )
+        self.assertIn("UID:{}".format(booking.UID()), data)
```

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_setup.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/tests/test_week_table_overrides.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/tests/test_week_table_overrides.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/upgrades.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/upgrades.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/upgrades.zcml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/utilities/dateutils.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/utilities/dateutils.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/utilities/urls.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/utilities/urls.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/viewlets/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/viewlets/templates/app_io.pt` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/viewlets/templates/app_io.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/gates.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/gates.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/review_states.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/review_states.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/tipologies.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/tipologies.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/voc_months.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/voc_months.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/PKG-INFO` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle.prenotazioni.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.prenotazioni
-Version: 2.0.0.dev2
+Version: 2.0.0.dev3
 Summary: An add-on for Plone
 Home-page: https://github.com/redturtle/redturtle.prenotazioni
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/redturtle.prenotazioni
 Project-URL: Source, https://github.com/redturtle/redturtle.prenotazioni
@@ -633,14 +633,20 @@
 - Daniele Andreotti, daniele.andreotti@redturtle.it
 
 
 Changelog
 =========
 
 
+2.0.0.dev3 (2023-07-20)
+-----------------------
+
+- Change "day" type in week_table (TODO: need an upgrade step?)
+  [mauro]
+
 2.0.0.dev2 (2023-06-30)
 -----------------------
 
 - reorganize backend form
   [mamico]
 
 - booking_type filter in @months-slots
```

### Comparing `redturtle.prenotazioni-2.0.0.dev2/src/redturtle.prenotazioni.egg-info/SOURCES.txt` & `redturtle.prenotazioni-2.0.0.dev3/src/redturtle.prenotazioni.egg-info/SOURCES.txt`

 * *Files identical despite different names*


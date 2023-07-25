# Comparing `tmp/NEMO-4.6.0.tar.gz` & `tmp/NEMO-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NEMO-4.6.0.tar", last modified: Tue Jul 18 17:03:24 2023, max compression
+gzip compressed data, was "NEMO-4.6.1.tar", last modified: Tue Jul 25 22:28:31 2023, max compression
```

## Comparing `NEMO-4.6.0.tar` & `NEMO-4.6.1.tar`

### file list

```diff
@@ -1,512 +1,513 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.973250 NEMO-4.6.0/
--rw-rw-rw-   0 root         (0) root         (0)     1865 2023-07-18 17:03:12.000000 NEMO-4.6.0/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-18 17:03:12.000000 NEMO-4.6.0/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.906249 NEMO-4.6.0/NEMO/
--rw-rw-rw-   0 root         (0) root         (0)     1254 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4594 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/actions.py
--rw-rw-rw-   0 root         (0) root         (0)    49666 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.907250 NEMO-4.6.0/NEMO/apps/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.908249 NEMO-4.6.0/NEMO/apps/area_access/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.893249 NEMO-4.6.0/NEMO/apps/area_access/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.908249 NEMO-4.6.0/NEMO/apps/area_access/static/area_access/
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/static/area_access/area_access.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.894249 NEMO-4.6.0/NEMO/apps/area_access/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.910250 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/
--rw-rw-rw-   0 root         (0) root         (0)     1727 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/already_logged_in.html
--rw-rw-rw-   0 root         (0) root         (0)      349 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/badge_not_found.html
--rw-rw-rw-   0 root         (0) root         (0)     9006 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/base.html
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/choose_project.html
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/door_is_open.html
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/farewell_screen.html
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/inactive.html
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/login_success.html
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/logout_success.html
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/logout_warning.html
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/no_active_projects.html
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/not_logged_in.html
--rw-rw-rw-   0 root         (0) root         (0)      210 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/physical_access_denied.html
--rw-rw-rw-   0 root         (0) root         (0)      566 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/resource_unavailable.html
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/welcome_screen.html
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    12663 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/area_access/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.912249 NEMO-4.6.0/NEMO/apps/contracts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4147 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      212 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/customization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.912249 NEMO-4.6.0/NEMO/apps/contracts/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.912249 NEMO-4.6.0/NEMO/apps/contracts/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/management/commands/send_email_contract_reminders.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.912249 NEMO-4.6.0/NEMO/apps/contracts/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     5839 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5550 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.894249 NEMO-4.6.0/NEMO/apps/contracts/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.913250 NEMO-4.6.0/NEMO/apps/contracts/templates/contracts/
--rw-rw-rw-   0 root         (0) root         (0)     4319 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/templates/contracts/contractors.html
--rw-rw-rw-   0 root         (0) root         (0)     4204 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/templates/contracts/contracts_and_procurements.html
--rw-rw-rw-   0 root         (0) root         (0)     3726 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/templates/contracts/procurements.html
--rw-rw-rw-   0 root         (0) root         (0)     5069 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/templates/contracts/service_contracts.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.913250 NEMO-4.6.0/NEMO/apps/contracts/templates/customizations/
--rw-rw-rw-   0 root         (0) root         (0)     2580 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/templates/customizations/customizations_contracts.html
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.914250 NEMO-4.6.0/NEMO/apps/contracts/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10827 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/contracts/views/contracts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.914250 NEMO-4.6.0/NEMO/apps/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.895249 NEMO-4.6.0/NEMO/apps/kiosk/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.915249 NEMO-4.6.0/NEMO/apps/kiosk/static/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/static/kiosk/kiosk.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.895249 NEMO-4.6.0/NEMO/apps/kiosk/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.916250 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/acknowledgement.html
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/category_choices.html
--rw-rw-rw-   0 root         (0) root         (0)     2044 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/choices.html
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/error.html
--rw-rw-rw-   0 root         (0) root         (0)     2923 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)    12592 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/kiosk.html
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/success.html
--rw-rw-rw-   0 root         (0) root         (0)    17312 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/tool_information.html
--rw-rw-rw-   0 root         (0) root         (0)     1108 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html
--rw-rw-rw-   0 root         (0) root         (0)     4472 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    13386 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/kiosk/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.917250 NEMO-4.6.0/NEMO/apps/sensors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7128 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/customizations.py
--rw-rw-rw-   0 root         (0) root         (0)     5237 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/evaluators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.917250 NEMO-4.6.0/NEMO/apps/sensors/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.918250 NEMO-4.6.0/NEMO/apps/sensors/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/management/commands/manage_sensor_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.918250 NEMO-4.6.0/NEMO/apps/sensors/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     7794 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13007 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/models.py
--rw-rw-rw-   0 root         (0) root         (0)     4906 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/sensors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.895249 NEMO-4.6.0/NEMO/apps/sensors/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.920250 NEMO-4.6.0/NEMO/apps/sensors/static/sensors/
--rw-rw-rw-   0 root         (0) root         (0)   408236 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/static/sensors/chart.js
--rw-rw-rw-   0 root         (0) root         (0)   195090 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/static/sensors/chart.min.js
--rw-rw-rw-   0 root         (0) root         (0)     1376 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js
--rw-rw-rw-   0 root         (0) root         (0)     7659 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/static/sensors/daterangepicker.css
--rw-rw-rw-   0 root         (0) root         (0)    66305 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/static/sensors/daterangepicker.js
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/static/sensors/sensors.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.896249 NEMO-4.6.0/NEMO/apps/sensors/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.920250 NEMO-4.6.0/NEMO/apps/sensors/templates/customizations/
--rw-rw-rw-   0 root         (0) root         (0)     4718 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/templates/customizations/customizations_sensors.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.920250 NEMO-4.6.0/NEMO/apps/sensors/templates/sensors/
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/templates/sensors/sensor_alerts.html
--rw-rw-rw-   0 root         (0) root         (0)    15165 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/templates/sensors/sensor_data.html
--rw-rw-rw-   0 root         (0) root         (0)     3879 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/templates/sensors/sensors.html
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     5650 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/apps/sensors/views.py
--rw-rw-rw-   0 root         (0) root         (0)     3966 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/context_processors.py
--rw-rw-rw-   0 root         (0) root         (0)     5776 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3833 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    14224 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/forms.py
--rw-rw-rw-   0 root         (0) root         (0)    17784 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/interlocks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.920250 NEMO-4.6.0/NEMO/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.922250 NEMO-4.6.0/NEMO/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/cancel_unused_reservations.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/create_closure_alerts.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/manage_recurring_charges.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/manage_tool_qualifications.py
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/send_email_out_of_time_reservation_notification.py
--rw-rw-rw-   0 root         (0) root         (0)      415 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/send_email_reservation_ending_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/send_email_reservation_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/send_email_usage_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      456 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/send_email_user_access_expiration_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/management/commands/send_email_weekend_access_notification.py
--rw-rw-rw-   0 root         (0) root         (0)     5578 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.927250 NEMO-4.6.0/NEMO/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    50307 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0001_version_1_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)    32962 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0002_version_1_0_0_squashed.py
--rw-rw-rw-   0 root         (0) root         (0)     7988 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0012_version_2_0_0_squashed.py
--rw-rw-rw-   0 root         (0) root         (0)     9904 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0020_version_3_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1712 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0021_version_3_1_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0022_version_3_3_0.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0023_badgereader.py
--rw-rw-rw-   0 root         (0) root         (0)      705 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0024_contactinformation_user.py
--rw-rw-rw-   0 root         (0) root         (0)     2674 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0025_version_3_6_0.py
--rw-rw-rw-   0 root         (0) root         (0)     5405 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0026_version_3_7_0.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0027_version_3_8_0.py
--rw-rw-rw-   0 root         (0) root         (0)     2231 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0028_version_3_9_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0030_version_3_9_2.py
--rw-rw-rw-   0 root         (0) root         (0)     2785 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0031_version_3_10_0.py
--rw-rw-rw-   0 root         (0) root         (0)     3166 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0032_version_3_11_0.py
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0033_version_3_12_0.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0034_version_3_13_0.py
--rw-rw-rw-   0 root         (0) root         (0)     6747 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0035_version_3_14_0.py
--rw-rw-rw-   0 root         (0) root         (0)     7792 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0036_version_3_15_0.py
--rw-rw-rw-   0 root         (0) root         (0)     3717 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0037_version_3_16_0.py
--rw-rw-rw-   0 root         (0) root         (0)      935 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0038_version_4_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)     3601 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0039_version_4_1_0.py
--rw-rw-rw-   0 root         (0) root         (0)     2444 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0040_version_4_2_0.py
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0041_version_4_2_1.py
--rw-rw-rw-   0 root         (0) root         (0)    16447 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0042_version_4_3_0.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0043_version_4_3_2.py
--rw-rw-rw-   0 root         (0) root         (0)     5416 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0044_version_4_4_0.py
--rw-rw-rw-   0 root         (0) root         (0)    13447 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0045_version_4_5_0.py
--rw-rw-rw-   0 root         (0) root         (0)     2037 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0045_version_4_5_5.py
--rw-rw-rw-   0 root         (0) root         (0)     2997 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/0046_version_4_6_0.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2299 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/migrations_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     7993 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/model_tree.py
--rw-rw-rw-   0 root         (0) root         (0)   148191 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1429 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)    49662 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/policy.py
--rw-rw-rw-   0 root         (0) root         (0)     9943 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/provisioning.py
--rw-rw-rw-   0 root         (0) root         (0)     5646 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/rates.py
--rw-rw-rw-   0 root         (0) root         (0)     1037 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/rest_filter_backend.py
--rw-rw-rw-   0 root         (0) root         (0)    11173 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.931250 NEMO-4.6.0/NEMO/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.931250 NEMO-4.6.0/NEMO/static/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.931250 NEMO-4.6.0/NEMO/static/admin/physical_access_level/
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/admin/physical_access_level/access_level.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.932250 NEMO-4.6.0/NEMO/static/admin/questions_preview/
--rw-rw-rw-   0 root         (0) root         (0)     4122 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/admin/questions_preview/questions_preview.css
--rw-rw-rw-   0 root         (0) root         (0)     1372 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/admin/questions_preview/questions_preview.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.932250 NEMO-4.6.0/NEMO/static/admin/reservation_questions/
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/admin/reservation_questions/reservation_questions.js
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/admin/time_options_override.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.932250 NEMO-4.6.0/NEMO/static/admin/tool/
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/admin/tool/tool.js
--rw-rw-rw-   0 root         (0) root         (0)     1515 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/badge_reader.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.897249 NEMO-4.6.0/NEMO/static/bootstrap/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.934250 NEMO-4.6.0/NEMO/static/bootstrap/css/
--rw-rw-rw-   0 root         (0) root         (0)    22608 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap-theme.css
--rw-rw-rw-   0 root         (0) root         (0)    43339 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap-theme.css.map
--rw-rw-rw-   0 root         (0) root         (0)    19963 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap-theme.min.css
--rw-rw-rw-   0 root         (0) root         (0)   141622 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap.css
--rw-rw-rw-   0 root         (0) root         (0)   380986 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap.css.map
--rw-rw-rw-   0 root         (0) root         (0)   117305 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.935250 NEMO-4.6.0/NEMO/static/bootstrap/fonts/
--rw-rw-rw-   0 root         (0) root         (0)    20127 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0 root         (0) root         (0)   108738 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0 root         (0) root         (0)    45404 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)    23424 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0 root         (0) root         (0)    18028 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.935250 NEMO-4.6.0/NEMO/static/bootstrap/js/
--rw-rw-rw-   0 root         (0) root         (0)    67546 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/js/bootstrap.js
--rw-rw-rw-   0 root         (0) root         (0)    35951 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.935250 NEMO-4.6.0/NEMO/static/datetimepicker/
--rw-rw-rw-   0 root         (0) root         (0)     9020 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/datetimepicker/bootstrap-datetimepicker.css
--rw-rw-rw-   0 root         (0) root         (0)   105978 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/datetimepicker/bootstrap-datetimepicker.js
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.937250 NEMO-4.6.0/NEMO/static/fullcalendar/
--rw-rw-rw-   0 root         (0) root         (0)    28531 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/fullcalendar/fullcalendar.css
--rw-rw-rw-   0 root         (0) root         (0)   357749 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/fullcalendar/fullcalendar.js
--rw-rw-rw-   0 root         (0) root         (0)    13687 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/fullcalendar/fullcalendar.min.css
--rw-rw-rw-   0 root         (0) root         (0)   168700 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/fullcalendar/fullcalendar.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.937250 NEMO-4.6.0/NEMO/static/icons/
--rw-rw-rw-   0 root         (0) root         (0)    24065 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/icons/agreement.png
--rw-rw-rw-   0 root         (0) root         (0)    16685 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/icons/caution.png
--rw-rw-rw-   0 root         (0) root         (0)     4664 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/icons/preferences.png
--rw-rw-rw-   0 root         (0) root         (0)   247387 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/jquery.js
--rw-rw-rw-   0 root         (0) root         (0)    84320 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/jquery.min.js
--rw-rw-rw-   0 root         (0) root         (0)  1183392 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/jumbotron_watermark.bmp
--rw-rw-rw-   0 root         (0) root         (0)     1017 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/mobile.js
--rw-rw-rw-   0 root         (0) root         (0)   174603 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/moment.js
--rw-rw-rw-   0 root         (0) root         (0)    58102 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/moment.min.js
--rw-rw-rw-   0 root         (0) root         (0)    86041 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/moment.min.js.map
--rw-rw-rw-   0 root         (0) root         (0)    17874 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/nemo.css
--rw-rw-rw-   0 root         (0) root         (0)    21828 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/nemo.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.938250 NEMO-4.6.0/NEMO/static/numpad/
--rw-rw-rw-   0 root         (0) root         (0)    12285 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/numpad/custom_numpad.jquery.js
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/numpad/numpad.jquery.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.939250 NEMO-4.6.0/NEMO/static/pickadate/
--rw-rw-rw-   0 root         (0) root         (0)     3795 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/pickadate/default.css
--rw-rw-rw-   0 root         (0) root         (0)     6040 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/pickadate/default.date.css
--rw-rw-rw-   0 root         (0) root         (0)     2785 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/pickadate/default.time.css
--rw-rw-rw-   0 root         (0) root         (0)    48215 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/pickadate/picker.date.js
--rw-rw-rw-   0 root         (0) root         (0)    36941 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/pickadate/picker.js
--rw-rw-rw-   0 root         (0) root         (0)    31899 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/pickadate/picker.time.js
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/robots.txt
--rw-rw-rw-   0 root         (0) root         (0)    48446 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/typeahead.jquery.js
--rw-rw-rw-   0 root         (0) root         (0)    20748 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/typeahead.jquery.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.939250 NEMO-4.6.0/NEMO/static/virtualkeyboard/
--rw-rw-rw-   0 root         (0) root         (0)   113008 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/virtualkeyboard/jquery.keyboard.js
--rw-rw-rw-   0 root         (0) root         (0)    47325 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/virtualkeyboard/jquery.keyboard.min.js
--rw-rw-rw-   0 root         (0) root         (0)     7848 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/virtualkeyboard/keyboard-basic.css
--rw-rw-rw-   0 root         (0) root         (0)     5889 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/static/virtualkeyboard/keyboard-basic.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.942250 NEMO-4.6.0/NEMO/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.942250 NEMO-4.6.0/NEMO/templates/abuse/
--rw-rw-rw-   0 root         (0) root         (0)     4059 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/abuse/abuse.html
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/abuse/user_drill_down.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.943250 NEMO-4.6.0/NEMO/templates/accounts_and_projects/
--rw-rw-rw-   0 root         (0) root         (0)     7665 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/accounts_and_projects/account_and_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     6409 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/accounts_and_projects/accounts_and_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     2843 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/accounts_and_projects/create_account.html
--rw-rw-rw-   0 root         (0) root         (0)     6693 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/accounts_and_projects/create_project.html
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/accounts_and_projects/documents_for_project.html
--rw-rw-rw-   0 root         (0) root         (0)     3544 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/accounts_and_projects/projects.html
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/accounts_and_projects/users_for_project.html
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/acknowledgement.html
--rw-rw-rw-   0 root         (0) root         (0)     4694 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/alerts.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.944250 NEMO-4.6.0/NEMO/templates/area_access/
--rw-rw-rw-   0 root         (0) root         (0)     2951 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/area_access/area_access.html
--rw-rw-rw-   0 root         (0) root         (0)     1748 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/area_access/calendar_self_login.html
--rw-rw-rw-   0 root         (0) root         (0)     1111 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/area_access/change_project.html
--rw-rw-rw-   0 root         (0) root         (0)     1141 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/area_access/login_areas.html
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/area_access/new_area_access_record.html
--rw-rw-rw-   0 root         (0) root         (0)     1938 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/area_access/new_area_access_record_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1454 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/area_access/self_login.html
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/authorization_failed.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.945250 NEMO-4.6.0/NEMO/templates/base/
--rw-rw-rw-   0 root         (0) root         (0)      308 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/base/footer.html
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/base/impersonate_header.html
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/base/navbar.html
--rw-rw-rw-   0 root         (0) root         (0)     8117 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/base/navbar_base.html
--rw-rw-rw-   0 root         (0) root         (0)      308 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/base/popup.html
--rw-rw-rw-   0 root         (0) root         (0)     6174 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.947250 NEMO-4.6.0/NEMO/templates/calendar/
--rw-rw-rw-   0 root         (0) root         (0)    24673 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/calendar.html
--rw-rw-rw-   0 root         (0) root         (0)     1442 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/configuration.html
--rw-rw-rw-   0 root         (0) root         (0)     2834 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/configuration_helper.html
--rw-rw-rw-   0 root         (0) root         (0)     1315 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/policy_dialog.html
--rw-rw-rw-   0 root         (0) root         (0)     1361 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/project_choice.html
--rw-rw-rw-   0 root         (0) root         (0)     1512 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/proxy_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     1862 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/reservation_event_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     1680 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/reservation_questions.html
--rw-rw-rw-   0 root         (0) root         (0)     1285 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/reservation_warning.html
--rw-rw-rw-   0 root         (0) root         (0)     4410 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/scheduled_outage_information.html
--rw-rw-rw-   0 root         (0) root         (0)     2011 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/specific_user_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     2543 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/calendar/usage_event_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     6530 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/configuration_agenda.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.948250 NEMO-4.6.0/NEMO/templates/consumables/
--rw-rw-rw-   0 root         (0) root         (0)     8224 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/consumables/consumables.html
--rw-rw-rw-   0 root         (0) root         (0)     1538 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/consumables/consumables_order.html
--rw-rw-rw-   0 root         (0) root         (0)    11695 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/consumables/recurring_charge.html
--rw-rw-rw-   0 root         (0) root         (0)     5473 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/consumables/recurring_charges.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.948250 NEMO-4.6.0/NEMO/templates/contact/
--rw-rw-rw-   0 root         (0) root         (0)      692 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/contact/contact_staff.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.950250 NEMO-4.6.0/NEMO/templates/customizations/
--rw-rw-rw-   0 root         (0) root         (0)     1848 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations.html
--rw-rw-rw-   0 root         (0) root         (0)     4324 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_application.html
--rw-rw-rw-   0 root         (0) root         (0)     7799 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_calendar.html
--rw-rw-rw-   0 root         (0) root         (0)     7634 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     4202 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_emails.html
--rw-rw-rw-   0 root         (0) root         (0)     2545 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_interlock.html
--rw-rw-rw-   0 root         (0) root         (0)     5553 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_projects_and_accounts.html
--rw-rw-rw-   0 root         (0) root         (0)     2224 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_rates.html
--rw-rw-rw-   0 root         (0) root         (0)     3519 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_recurring_charges.html
--rw-rw-rw-   0 root         (0) root         (0)     2183 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_remote_work.html
--rw-rw-rw-   0 root         (0) root         (0)    16717 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     3678 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_safety.html
--rw-rw-rw-   0 root         (0) root         (0)    27806 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_templates.html
--rw-rw-rw-   0 root         (0) root         (0)     9253 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_tool.html
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_upload.html
--rw-rw-rw-   0 root         (0) root         (0)     5214 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/customizations/customizations_user.html
--rw-rw-rw-   0 root         (0) root         (0)      502 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/display_success_and_redirect.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.951250 NEMO-4.6.0/NEMO/templates/email/
--rw-rw-rw-   0 root         (0) root         (0)     7825 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/email/compose_email.html
--rw-rw-rw-   0 root         (0) root         (0)     3153 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/email/email_broadcast.html
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/email/email_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.951250 NEMO-4.6.0/NEMO/templates/event_details/
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/event_details/area_access_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1376 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/event_details/outage_details.html
--rw-rw-rw-   0 root         (0) root         (0)    12242 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/event_details/reservation_details.html
--rw-rw-rw-   0 root         (0) root         (0)      589 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/event_details/usage_details.html
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/facility_rules.html
--rw-rw-rw-   0 root         (0) root         (0)     1247 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/feedback.html
--rw-rw-rw-   0 root         (0) root         (0)      937 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/history.html
--rw-rw-rw-   0 root         (0) root         (0)     1260 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/impersonate.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.952250 NEMO-4.6.0/NEMO/templates/jumbotron/
--rw-rw-rw-   0 root         (0) root         (0)     2059 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/jumbotron/jumbotron.html
--rw-rw-rw-   0 root         (0) root         (0)     3635 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/jumbotron/jumbotron_content.html
--rw-rw-rw-   0 root         (0) root         (0)     8670 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/landing.html
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/login.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.952250 NEMO-4.6.0/NEMO/templates/maintenance/
--rw-rw-rw-   0 root         (0) root         (0)     1558 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/maintenance/closed_task_details.html
--rw-rw-rw-   0 root         (0) root         (0)     5566 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/maintenance/maintenance.html
--rw-rw-rw-   0 root         (0) root         (0)     7450 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/maintenance/pending_task_details.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.953250 NEMO-4.6.0/NEMO/templates/mobile/
--rw-rw-rw-   0 root         (0) root         (0)      762 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/cancellation_result.html
--rw-rw-rw-   0 root         (0) root         (0)     1916 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/choose_item.html
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/error.html
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/individual_outage.html
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/individual_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     5899 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/new_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/no_active_projects.html
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/reservation_success.html
--rw-rw-rw-   0 root         (0) root         (0)     1442 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/mobile/view_calendar.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.954250 NEMO-4.6.0/NEMO/templates/news/
--rw-rw-rw-   0 root         (0) root         (0)      981 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/news/archived_news.html
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/news/new_news_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/news/news_update_form.html
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/news/recent_news.html
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/no_project.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.954250 NEMO-4.6.0/NEMO/templates/occupancy/
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/occupancy/occupancy.html
--rw-rw-rw-   0 root         (0) root         (0)     1841 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/occupancy/occupancy_content.html
--rw-rw-rw-   0 root         (0) root         (0)     1147 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/occupancy/occupancy_count.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.955250 NEMO-4.6.0/NEMO/templates/pagination/
--rw-rw-rw-   0 root         (0) root         (0)      865 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/pagination/pagination_base.html
--rw-rw-rw-   0 root         (0) root         (0)      521 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/pagination/pagination_column.html
--rw-rw-rw-   0 root         (0) root         (0)      673 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/pagination/pagination_pages.html
--rw-rw-rw-   0 root         (0) root         (0)      642 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/pagination/pagination_selector.html
--rw-rw-rw-   0 root         (0) root         (0)     2841 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/qualifications.html
--rw-rw-rw-   0 root         (0) root         (0)     5462 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/refresh_sidebar_icons.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.955250 NEMO-4.6.0/NEMO/templates/remote_work/
--rw-rw-rw-   0 root         (0) root         (0)    10616 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/remote_work/remote_work.html
--rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/remote_work/remote_work_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.955250 NEMO-4.6.0/NEMO/templates/requests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.956250 NEMO-4.6.0/NEMO/templates/requests/access_requests/
--rw-rw-rw-   0 root         (0) root         (0)     7754 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/access_requests/access_request.html
--rw-rw-rw-   0 root         (0) root         (0)     3450 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/access_requests/access_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     3480 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/access_requests/access_requests_table.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.956250 NEMO-4.6.0/NEMO/templates/requests/adjustment_requests/
--rw-rw-rw-   0 root         (0) root         (0)     8607 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/adjustment_requests/adjustment_request.html
--rw-rw-rw-   0 root         (0) root         (0)     3733 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/adjustment_requests/adjustment_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     7257 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.957250 NEMO-4.6.0/NEMO/templates/requests/buddy_requests/
--rw-rw-rw-   0 root         (0) root         (0)     3910 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/buddy_requests/buddy_request.html
--rw-rw-rw-   0 root         (0) root         (0)     5602 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/buddy_requests/buddy_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     4246 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/requests/user_requests.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.957250 NEMO-4.6.0/NEMO/templates/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2950 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/resources/modify_resource.html
--rw-rw-rw-   0 root         (0) root         (0)     3846 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/resources/resource_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/resources/resources.html
--rw-rw-rw-   0 root         (0) root         (0)     3898 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/resources/scheduled_outage.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.957250 NEMO-4.6.0/NEMO/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/rest_framework/api.html
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/rest_framework/custom_error.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.959250 NEMO-4.6.0/NEMO/templates/safety/
--rw-rw-rw-   0 root         (0) root         (0)     3112 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/safety/safety.html
--rw-rw-rw-   0 root         (0) root         (0)     1733 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/safety/safety_base.html
--rw-rw-rw-   0 root         (0) root         (0)     7807 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/safety/safety_data_sheets.html
--rw-rw-rw-   0 root         (0) root         (0)     1976 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/safety/safety_issues.html
--rw-rw-rw-   0 root         (0) root         (0)     1723 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/safety/safety_issues_create.html
--rw-rw-rw-   0 root         (0) root         (0)     1722 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/safety/safety_issues_resolved.html
--rw-rw-rw-   0 root         (0) root         (0)     1762 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/safety/safety_issues_update.html
--rw-rw-rw-   0 root         (0) root         (0)     1877 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/safety/safety_items.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.959250 NEMO-4.6.0/NEMO/templates/snippets/
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/snippets/button.html
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/snippets/contact_person.html
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/snippets/document_list.html
--rw-rw-rw-   0 root         (0) root         (0)     1128 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/snippets/embedded_document.html
--rw-rw-rw-   0 root         (0) root         (0)     1673 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/snippets/tool_info.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.960250 NEMO-4.6.0/NEMO/templates/staff_charges/
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/staff_charges/change_status.html
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/staff_charges/choose_project.html
--rw-rw-rw-   0 root         (0) root         (0)      498 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/staff_charges/end_area_charge.html
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/staff_charges/new_staff_charge.html
--rw-rw-rw-   0 root         (0) root         (0)     1014 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/staff_charges/reminder.html
--rw-rw-rw-   0 root         (0) root         (0)     1854 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/staff_charges/staff_charges_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.961250 NEMO-4.6.0/NEMO/templates/status_dashboard/
--rw-rw-rw-   0 root         (0) root         (0)     1554 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/status_dashboard/occupancy.html
--rw-rw-rw-   0 root         (0) root         (0)     9771 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/status_dashboard/staff.html
--rw-rw-rw-   0 root         (0) root         (0)     7709 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/status_dashboard/staff_absence.html
--rw-rw-rw-   0 root         (0) root         (0)     6650 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/status_dashboard/status_dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/status_dashboard/tools.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.961250 NEMO-4.6.0/NEMO/templates/tasks/
--rw-rw-rw-   0 root         (0) root         (0)     2542 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tasks/resolve.html
--rw-rw-rw-   0 root         (0) root         (0)     5037 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tasks/update.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.962250 NEMO-4.6.0/NEMO/templates/tool_control/
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tool_control/get_projects.html
--rw-rw-rw-   0 root         (0) root         (0)      737 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tool_control/interlock_error.html
--rw-rw-rw-   0 root         (0) root         (0)     3502 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tool_control/past_tasks_and_comments.html
--rw-rw-rw-   0 root         (0) root         (0)     2466 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tool_control/qualified_users.html
--rw-rw-rw-   0 root         (0) root         (0)    15303 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tool_control/tool_control.html
--rw-rw-rw-   0 root         (0) root         (0)    37737 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tool_control/tool_status.html
--rw-rw-rw-   0 root         (0) root         (0)     6142 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tool_control/usage_data.html
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/tool_control/use_tool_for_other.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.963250 NEMO-4.6.0/NEMO/templates/training/
--rw-rw-rw-   0 root         (0) root         (0)      512 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/training/get_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     4971 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/training/training.html
--rw-rw-rw-   0 root         (0) root         (0)     1962 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/training/training_entry.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.963250 NEMO-4.6.0/NEMO/templates/usage/
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/usage/adjustment_request_button.html
--rw-rw-rw-   0 root         (0) root         (0)     3573 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/usage/billing.html
--rw-rw-rw-   0 root         (0) root         (0)     9218 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/usage/usage.html
--rw-rw-rw-   0 root         (0) root         (0)     7812 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/usage/usage_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.964250 NEMO-4.6.0/NEMO/templates/users/
--rw-rw-rw-   0 root         (0) root         (0)    20776 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/users/create_or_modify_user.html
--rw-rw-rw-   0 root         (0) root         (0)    18558 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/users/preferences.html
--rw-rw-rw-   0 root         (0) root         (0)     3758 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/users/safe_deactivation.html
--rw-rw-rw-   0 root         (0) root         (0)     4181 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templates/users/users.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.964250 NEMO-4.6.0/NEMO/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8447 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/templatetags/custom_tags_and_filters.py
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    26303 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    24642 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.972250 NEMO-4.6.0/NEMO/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4308 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/abuse.py
--rw-rw-rw-   0 root         (0) root         (0)    14733 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/access_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     8275 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/accounts_and_projects.py
--rw-rw-rw-   0 root         (0) root         (0)    18760 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/adjustment_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     1812 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/alerts.py
--rw-rw-rw-   0 root         (0) root         (0)    14004 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/api.py
--rw-rw-rw-   0 root         (0) root         (0)    12252 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/api_billing.py
--rw-rw-rw-   0 root         (0) root         (0)     2415 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/api_file_import.py
--rw-rw-rw-   0 root         (0) root         (0)    19042 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/area_access.py
--rw-rw-rw-   0 root         (0) root         (0)    12070 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     6625 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/buddy_requests.py
--rw-rw-rw-   0 root         (0) root         (0)    71717 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/calendar.py
--rw-rw-rw-   0 root         (0) root         (0)     2334 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/charge_validation.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/configuration_agenda.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    10947 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/consumables.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/contact_staff.py
--rw-rw-rw-   0 root         (0) root         (0)    18708 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/customization.py
--rw-rw-rw-   0 root         (0) root         (0)     3442 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/documents.py
--rw-rw-rw-   0 root         (0) root         (0)    10015 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/email.py
--rw-rw-rw-   0 root         (0) root         (0)     1973 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/event_details.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/feedback.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/get_projects.py
--rw-rw-rw-   0 root         (0) root         (0)     4168 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/history.py
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/jumbotron.py
--rw-rw-rw-   0 root         (0) root         (0)     3293 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/landing.py
--rw-rw-rw-   0 root         (0) root         (0)     2718 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/maintenance.py
--rw-rw-rw-   0 root         (0) root         (0)     8072 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/mobile.py
--rw-rw-rw-   0 root         (0) root         (0)     3356 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/news.py
--rw-rw-rw-   0 root         (0) root         (0)     5459 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/notifications.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     4822 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/qualifications.py
--rw-rw-rw-   0 root         (0) root         (0)     9506 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/remote_work.py
--rw-rw-rw-   0 root         (0) root         (0)     3700 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     8877 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/safety.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/sidebar.py
--rw-rw-rw-   0 root         (0) root         (0)    20146 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/status_dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)    13615 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)    23995 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/tool_control.py
--rw-rw-rw-   0 root         (0) root         (0)     6043 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/training.py
--rw-rw-rw-   0 root         (0) root         (0)     1909 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/tutorials.py
--rw-rw-rw-   0 root         (0) root         (0)    18360 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1049 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/user_requests.py
--rw-rw-rw-   0 root         (0) root         (0)    20715 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/views/users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.972250 NEMO-4.6.0/NEMO/widgets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2968 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/widgets/configuration_editor.py
--rw-rw-rw-   0 root         (0) root         (0)    26383 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/widgets/dynamic_form.py
--rw-rw-rw-   0 root         (0) root         (0)     8029 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/widgets/item_tree.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-18 17:03:12.000000 NEMO-4.6.0/NEMO/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.907250 NEMO-4.6.0/NEMO.egg-info/
--rw-r--r--   0 root         (0) root         (0)      904 2023-07-18 17:03:24.000000 NEMO-4.6.0/NEMO.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17375 2023-07-18 17:03:24.000000 NEMO-4.6.0/NEMO.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 17:03:24.000000 NEMO-4.6.0/NEMO.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-18 17:03:24.000000 NEMO-4.6.0/NEMO.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      264 2023-07-18 17:03:24.000000 NEMO-4.6.0/NEMO.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-18 17:03:24.000000 NEMO-4.6.0/NEMO.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      904 2023-07-18 17:03:24.973250 NEMO-4.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4066 2023-07-18 17:03:12.000000 NEMO-4.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:03:24.973250 NEMO-4.6.0/resources/
--rw-rw-rw-   0 root         (0) root         (0)    17135 2023-07-18 17:03:12.000000 NEMO-4.6.0/resources/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     3981 2023-07-18 17:03:12.000000 NEMO-4.6.0/resources/splash_pad_settings.py
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-18 17:03:24.974250 NEMO-4.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-18 17:03:12.000000 NEMO-4.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.189839 NEMO-4.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1865 2023-07-18 17:03:12.000000 NEMO-4.6.1/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-18 17:03:12.000000 NEMO-4.6.1/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.123838 NEMO-4.6.1/NEMO/
+-rw-rw-rw-   0 root         (0) root         (0)     1254 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4594 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)    49666 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.124838 NEMO-4.6.1/NEMO/apps/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/apps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.125838 NEMO-4.6.1/NEMO/apps/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/apps/area_access/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.108838 NEMO-4.6.1/NEMO/apps/area_access/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.125838 NEMO-4.6.1/NEMO/apps/area_access/static/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/static/area_access/area_access.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.108838 NEMO-4.6.1/NEMO/apps/area_access/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.127838 NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/already_logged_in.html
+-rw-rw-rw-   0 root         (0) root         (0)      349 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/badge_not_found.html
+-rw-rw-rw-   0 root         (0) root         (0)     9006 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/choose_project.html
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/door_is_open.html
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/farewell_screen.html
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/inactive.html
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/login_success.html
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/logout_success.html
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/logout_warning.html
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/no_active_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/not_logged_in.html
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/physical_access_denied.html
+-rw-rw-rw-   0 root         (0) root         (0)      566 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/resource_unavailable.html
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/welcome_screen.html
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    12663 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/area_access/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.128838 NEMO-4.6.1/NEMO/apps/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/apps/contracts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4147 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/contracts/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/contracts/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/contracts/customization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.128838 NEMO-4.6.1/NEMO/apps/contracts/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/apps/contracts/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.129838 NEMO-4.6.1/NEMO/apps/contracts/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/apps/contracts/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/contracts/management/commands/send_email_contract_reminders.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.129838 NEMO-4.6.1/NEMO/apps/contracts/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     5839 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/contracts/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/apps/contracts/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5550 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/contracts/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.108838 NEMO-4.6.1/NEMO/apps/contracts/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.130838 NEMO-4.6.1/NEMO/apps/contracts/templates/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)     4319 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/contracts/templates/contracts/contractors.html
+-rw-rw-rw-   0 root         (0) root         (0)     4204 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/contracts/templates/contracts/contracts_and_procurements.html
+-rw-rw-rw-   0 root         (0) root         (0)     3726 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/contracts/templates/contracts/procurements.html
+-rw-rw-rw-   0 root         (0) root         (0)     5069 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/contracts/templates/contracts/service_contracts.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.130838 NEMO-4.6.1/NEMO/apps/contracts/templates/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)     2580 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/contracts/templates/customizations/customizations_contracts.html
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/contracts/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.130838 NEMO-4.6.1/NEMO/apps/contracts/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/apps/contracts/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10827 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/contracts/views/contracts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.131838 NEMO-4.6.1/NEMO/apps/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/apps/kiosk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.109838 NEMO-4.6.1/NEMO/apps/kiosk/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.131838 NEMO-4.6.1/NEMO/apps/kiosk/static/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/kiosk/static/kiosk/kiosk.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.109838 NEMO-4.6.1/NEMO/apps/kiosk/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.132838 NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/acknowledgement.html
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/category_choices.html
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/choices.html
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/error.html
+-rw-rw-rw-   0 root         (0) root         (0)     2923 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)    12592 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/kiosk.html
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/success.html
+-rw-rw-rw-   0 root         (0) root         (0)    17312 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/tool_information.html
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html
+-rw-rw-rw-   0 root         (0) root         (0)     4472 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/kiosk/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    13386 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/kiosk/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.134838 NEMO-4.6.1/NEMO/apps/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/apps/sensors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7128 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/customizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/evaluators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.134838 NEMO-4.6.1/NEMO/apps/sensors/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/apps/sensors/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.134838 NEMO-4.6.1/NEMO/apps/sensors/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/apps/sensors/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/management/commands/manage_sensor_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.134838 NEMO-4.6.1/NEMO/apps/sensors/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     7794 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/apps/sensors/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13007 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4906 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/sensors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.110838 NEMO-4.6.1/NEMO/apps/sensors/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.137838 NEMO-4.6.1/NEMO/apps/sensors/static/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)   408236 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/static/sensors/chart.js
+-rw-rw-rw-   0 root         (0) root         (0)   195090 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/static/sensors/chart.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     1376 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js
+-rw-rw-rw-   0 root         (0) root         (0)     7659 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/static/sensors/daterangepicker.css
+-rw-rw-rw-   0 root         (0) root         (0)    66305 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/static/sensors/daterangepicker.js
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/static/sensors/sensors.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.110838 NEMO-4.6.1/NEMO/apps/sensors/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.137838 NEMO-4.6.1/NEMO/apps/sensors/templates/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)     4718 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/templates/customizations/customizations_sensors.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.137838 NEMO-4.6.1/NEMO/apps/sensors/templates/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/templates/sensors/sensor_alerts.html
+-rw-rw-rw-   0 root         (0) root         (0)    15165 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/templates/sensors/sensor_data.html
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/templates/sensors/sensors.html
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     5650 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/apps/sensors/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     3966 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/context_processors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5776 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3833 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    14224 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)    17784 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/interlocks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.138838 NEMO-4.6.1/NEMO/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.139838 NEMO-4.6.1/NEMO/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/management/commands/cancel_unused_reservations.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/management/commands/create_closure_alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/management/commands/manage_recurring_charges.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/management/commands/manage_tool_qualifications.py
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/management/commands/send_email_out_of_time_reservation_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)      415 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/management/commands/send_email_reservation_ending_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/management/commands/send_email_reservation_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/management/commands/send_email_usage_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      456 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/management/commands/send_email_user_access_expiration_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/management/commands/send_email_weekend_access_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     5578 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.144838 NEMO-4.6.1/NEMO/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    50307 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0001_version_1_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)    32962 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0002_version_1_0_0_squashed.py
+-rw-rw-rw-   0 root         (0) root         (0)     7988 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0012_version_2_0_0_squashed.py
+-rw-rw-rw-   0 root         (0) root         (0)     9904 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0020_version_3_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1712 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0021_version_3_1_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0022_version_3_3_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0023_badgereader.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0024_contactinformation_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     2674 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0025_version_3_6_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     5405 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0026_version_3_7_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0027_version_3_8_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     2231 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0028_version_3_9_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0030_version_3_9_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0031_version_3_10_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0032_version_3_11_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0033_version_3_12_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0034_version_3_13_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     6747 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0035_version_3_14_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     7792 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0036_version_3_15_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3717 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0037_version_3_16_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      935 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0038_version_4_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3601 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0039_version_4_1_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     2444 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0040_version_4_2_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0041_version_4_2_1.py
+-rw-rw-rw-   0 root         (0) root         (0)    16447 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0042_version_4_3_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0043_version_4_3_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5416 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0044_version_4_4_0.py
+-rw-rw-rw-   0 root         (0) root         (0)    13447 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0045_version_4_5_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     2037 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0045_version_4_5_5.py
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations/0046_version_4_6_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/migrations/0047_version_4_6_1.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/migrations_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     7993 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/model_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)   148192 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1429 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)    49662 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     9943 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/provisioning.py
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/rates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1037 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/rest_filter_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)    11173 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.148838 NEMO-4.6.1/NEMO/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.149838 NEMO-4.6.1/NEMO/static/admin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.149838 NEMO-4.6.1/NEMO/static/admin/physical_access_level/
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/admin/physical_access_level/access_level.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.149838 NEMO-4.6.1/NEMO/static/admin/questions_preview/
+-rw-rw-rw-   0 root         (0) root         (0)     4122 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/admin/questions_preview/questions_preview.css
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/admin/questions_preview/questions_preview.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.149838 NEMO-4.6.1/NEMO/static/admin/reservation_questions/
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/admin/reservation_questions/reservation_questions.js
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/admin/time_options_override.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.149838 NEMO-4.6.1/NEMO/static/admin/tool/
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/admin/tool/tool.js
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/badge_reader.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.112838 NEMO-4.6.1/NEMO/static/bootstrap/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.151838 NEMO-4.6.1/NEMO/static/bootstrap/css/
+-rw-rw-rw-   0 root         (0) root         (0)    22608 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/bootstrap/css/bootstrap-theme.css
+-rw-rw-rw-   0 root         (0) root         (0)    43339 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/bootstrap/css/bootstrap-theme.css.map
+-rw-rw-rw-   0 root         (0) root         (0)    19963 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/bootstrap/css/bootstrap-theme.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   141622 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/bootstrap/css/bootstrap.css
+-rw-rw-rw-   0 root         (0) root         (0)   380986 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/bootstrap/css/bootstrap.css.map
+-rw-rw-rw-   0 root         (0) root         (0)   117305 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.152839 NEMO-4.6.1/NEMO/static/bootstrap/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    20127 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0 root         (0) root         (0)   108738 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0 root         (0) root         (0)    45404 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    23424 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0 root         (0) root         (0)    18028 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.153838 NEMO-4.6.1/NEMO/static/bootstrap/js/
+-rw-rw-rw-   0 root         (0) root         (0)    67546 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/bootstrap/js/bootstrap.js
+-rw-rw-rw-   0 root         (0) root         (0)    35951 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.153838 NEMO-4.6.1/NEMO/static/datetimepicker/
+-rw-rw-rw-   0 root         (0) root         (0)     9020 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/datetimepicker/bootstrap-datetimepicker.css
+-rw-rw-rw-   0 root         (0) root         (0)   105978 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/datetimepicker/bootstrap-datetimepicker.js
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.154838 NEMO-4.6.1/NEMO/static/fullcalendar/
+-rw-rw-rw-   0 root         (0) root         (0)    28531 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/fullcalendar/fullcalendar.css
+-rw-rw-rw-   0 root         (0) root         (0)   357749 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/fullcalendar/fullcalendar.js
+-rw-rw-rw-   0 root         (0) root         (0)    13687 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/fullcalendar/fullcalendar.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   168700 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/fullcalendar/fullcalendar.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.155839 NEMO-4.6.1/NEMO/static/icons/
+-rw-rw-rw-   0 root         (0) root         (0)    24065 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/icons/agreement.png
+-rw-rw-rw-   0 root         (0) root         (0)    16685 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/icons/caution.png
+-rw-rw-rw-   0 root         (0) root         (0)     4664 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/icons/preferences.png
+-rw-rw-rw-   0 root         (0) root         (0)   247387 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)    84320 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/jquery.min.js
+-rw-rw-rw-   0 root         (0) root         (0)  1183392 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/jumbotron_watermark.bmp
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/mobile.js
+-rw-rw-rw-   0 root         (0) root         (0)   174603 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/moment.js
+-rw-rw-rw-   0 root         (0) root         (0)    58102 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/moment.min.js
+-rw-rw-rw-   0 root         (0) root         (0)    86041 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/moment.min.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    18140 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/static/nemo.css
+-rw-rw-rw-   0 root         (0) root         (0)    21828 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/nemo.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.155839 NEMO-4.6.1/NEMO/static/numpad/
+-rw-rw-rw-   0 root         (0) root         (0)    12285 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/numpad/custom_numpad.jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/numpad/numpad.jquery.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.156839 NEMO-4.6.1/NEMO/static/pickadate/
+-rw-rw-rw-   0 root         (0) root         (0)     3795 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/pickadate/default.css
+-rw-rw-rw-   0 root         (0) root         (0)     6040 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/pickadate/default.date.css
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/pickadate/default.time.css
+-rw-rw-rw-   0 root         (0) root         (0)    48215 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/pickadate/picker.date.js
+-rw-rw-rw-   0 root         (0) root         (0)    36941 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/pickadate/picker.js
+-rw-rw-rw-   0 root         (0) root         (0)    31899 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/pickadate/picker.time.js
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/robots.txt
+-rw-rw-rw-   0 root         (0) root         (0)    48446 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/typeahead.jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)    20748 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/typeahead.jquery.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.157838 NEMO-4.6.1/NEMO/static/virtualkeyboard/
+-rw-rw-rw-   0 root         (0) root         (0)   113008 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/virtualkeyboard/jquery.keyboard.js
+-rw-rw-rw-   0 root         (0) root         (0)    47325 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/virtualkeyboard/jquery.keyboard.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     7848 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/virtualkeyboard/keyboard-basic.css
+-rw-rw-rw-   0 root         (0) root         (0)     5889 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/static/virtualkeyboard/keyboard-basic.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.159839 NEMO-4.6.1/NEMO/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.159839 NEMO-4.6.1/NEMO/templates/abuse/
+-rw-rw-rw-   0 root         (0) root         (0)     4059 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/abuse/abuse.html
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/abuse/user_drill_down.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.160838 NEMO-4.6.1/NEMO/templates/accounts_and_projects/
+-rw-rw-rw-   0 root         (0) root         (0)     7665 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/accounts_and_projects/account_and_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     6409 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/accounts_and_projects/accounts_and_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     2843 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/accounts_and_projects/create_account.html
+-rw-rw-rw-   0 root         (0) root         (0)     6693 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/accounts_and_projects/create_project.html
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/accounts_and_projects/documents_for_project.html
+-rw-rw-rw-   0 root         (0) root         (0)     3544 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/accounts_and_projects/projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/accounts_and_projects/users_for_project.html
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/acknowledgement.html
+-rw-rw-rw-   0 root         (0) root         (0)     4694 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/alerts.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.161839 NEMO-4.6.1/NEMO/templates/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/area_access/area_access.html
+-rw-rw-rw-   0 root         (0) root         (0)     1748 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/area_access/calendar_self_login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1111 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/area_access/change_project.html
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/area_access/login_areas.html
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/area_access/new_area_access_record.html
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/area_access/new_area_access_record_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/area_access/self_login.html
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/authorization_failed.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.162839 NEMO-4.6.1/NEMO/templates/base/
+-rw-rw-rw-   0 root         (0) root         (0)      308 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/base/footer.html
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/base/impersonate_header.html
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/base/navbar.html
+-rw-rw-rw-   0 root         (0) root         (0)     8117 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/base/navbar_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      308 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/base/popup.html
+-rw-rw-rw-   0 root         (0) root         (0)     6174 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.164839 NEMO-4.6.1/NEMO/templates/calendar/
+-rw-rw-rw-   0 root         (0) root         (0)    24673 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/calendar/calendar.html
+-rw-rw-rw-   0 root         (0) root         (0)     1442 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/calendar/configuration.html
+-rw-rw-rw-   0 root         (0) root         (0)     2834 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/calendar/configuration_helper.html
+-rw-rw-rw-   0 root         (0) root         (0)     1315 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/calendar/policy_dialog.html
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/calendar/project_choice.html
+-rw-rw-rw-   0 root         (0) root         (0)     1512 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/calendar/proxy_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     1862 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/calendar/reservation_event_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     1680 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/calendar/reservation_questions.html
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/calendar/reservation_warning.html
+-rw-rw-rw-   0 root         (0) root         (0)     4410 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/calendar/scheduled_outage_information.html
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/calendar/specific_user_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     2543 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/calendar/usage_event_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     6530 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/configuration_agenda.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.165839 NEMO-4.6.1/NEMO/templates/consumables/
+-rw-rw-rw-   0 root         (0) root         (0)     8224 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/consumables/consumables.html
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/consumables/consumables_order.html
+-rw-rw-rw-   0 root         (0) root         (0)    11695 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/consumables/recurring_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)     5473 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/consumables/recurring_charges.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.165839 NEMO-4.6.1/NEMO/templates/contact/
+-rw-rw-rw-   0 root         (0) root         (0)      692 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/contact/contact_staff.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.167839 NEMO-4.6.1/NEMO/templates/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/customizations/customizations.html
+-rw-rw-rw-   0 root         (0) root         (0)     4882 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/templates/customizations/customizations_application.html
+-rw-rw-rw-   0 root         (0) root         (0)     7799 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/customizations/customizations_calendar.html
+-rw-rw-rw-   0 root         (0) root         (0)     7634 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/customizations/customizations_dashboard.html
+-rw-rw-rw-   0 root         (0) root         (0)     4202 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/customizations/customizations_emails.html
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/customizations/customizations_interlock.html
+-rw-rw-rw-   0 root         (0) root         (0)     5553 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/customizations/customizations_projects_and_accounts.html
+-rw-rw-rw-   0 root         (0) root         (0)     2224 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/customizations/customizations_rates.html
+-rw-rw-rw-   0 root         (0) root         (0)     3519 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/customizations/customizations_recurring_charges.html
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/customizations/customizations_remote_work.html
+-rw-rw-rw-   0 root         (0) root         (0)    16717 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/customizations/customizations_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     3678 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/customizations/customizations_safety.html
+-rw-rw-rw-   0 root         (0) root         (0)    27806 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/customizations/customizations_templates.html
+-rw-rw-rw-   0 root         (0) root         (0)     9253 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/customizations/customizations_tool.html
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/customizations/customizations_upload.html
+-rw-rw-rw-   0 root         (0) root         (0)     5214 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/customizations/customizations_user.html
+-rw-rw-rw-   0 root         (0) root         (0)      502 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/display_success_and_redirect.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.168839 NEMO-4.6.1/NEMO/templates/email/
+-rw-rw-rw-   0 root         (0) root         (0)     7825 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/email/compose_email.html
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/email/email_broadcast.html
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/email/email_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.168839 NEMO-4.6.1/NEMO/templates/event_details/
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/event_details/area_access_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1376 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/event_details/outage_details.html
+-rw-rw-rw-   0 root         (0) root         (0)    12242 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/event_details/reservation_details.html
+-rw-rw-rw-   0 root         (0) root         (0)      589 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/event_details/usage_details.html
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/facility_rules.html
+-rw-rw-rw-   0 root         (0) root         (0)     1247 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/feedback.html
+-rw-rw-rw-   0 root         (0) root         (0)      937 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/history.html
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/impersonate.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.169839 NEMO-4.6.1/NEMO/templates/jumbotron/
+-rw-rw-rw-   0 root         (0) root         (0)     2059 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/jumbotron/jumbotron.html
+-rw-rw-rw-   0 root         (0) root         (0)     3635 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/jumbotron/jumbotron_content.html
+-rw-rw-rw-   0 root         (0) root         (0)     8670 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/landing.html
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/login.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.169839 NEMO-4.6.1/NEMO/templates/maintenance/
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/maintenance/closed_task_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     5566 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/maintenance/maintenance.html
+-rw-rw-rw-   0 root         (0) root         (0)     7450 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/maintenance/pending_task_details.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.170839 NEMO-4.6.1/NEMO/templates/mobile/
+-rw-rw-rw-   0 root         (0) root         (0)      762 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/mobile/cancellation_result.html
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/mobile/choose_item.html
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/mobile/error.html
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/mobile/individual_outage.html
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/mobile/individual_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     5899 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/mobile/new_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/mobile/no_active_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/mobile/reservation_success.html
+-rw-rw-rw-   0 root         (0) root         (0)     1442 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/mobile/view_calendar.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.171839 NEMO-4.6.1/NEMO/templates/news/
+-rw-rw-rw-   0 root         (0) root         (0)      981 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/news/archived_news.html
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/news/new_news_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/news/news_update_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/news/recent_news.html
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/no_project.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.171839 NEMO-4.6.1/NEMO/templates/occupancy/
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/occupancy/occupancy.html
+-rw-rw-rw-   0 root         (0) root         (0)     1841 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/occupancy/occupancy_content.html
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/occupancy/occupancy_count.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.172839 NEMO-4.6.1/NEMO/templates/pagination/
+-rw-rw-rw-   0 root         (0) root         (0)      865 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/pagination/pagination_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      521 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/pagination/pagination_column.html
+-rw-rw-rw-   0 root         (0) root         (0)      673 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/pagination/pagination_pages.html
+-rw-rw-rw-   0 root         (0) root         (0)      642 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/pagination/pagination_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/qualifications.html
+-rw-rw-rw-   0 root         (0) root         (0)     5462 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/refresh_sidebar_icons.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.172839 NEMO-4.6.1/NEMO/templates/remote_work/
+-rw-rw-rw-   0 root         (0) root         (0)    10616 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/remote_work/remote_work.html
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/remote_work/remote_work_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.172839 NEMO-4.6.1/NEMO/templates/requests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.173839 NEMO-4.6.1/NEMO/templates/requests/access_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     7754 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/requests/access_requests/access_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     3450 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/requests/access_requests/access_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     3480 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/requests/access_requests/access_requests_table.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.173839 NEMO-4.6.1/NEMO/templates/requests/adjustment_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     8607 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/requests/adjustment_requests/adjustment_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     3733 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/requests/adjustment_requests/adjustment_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     7257 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.173839 NEMO-4.6.1/NEMO/templates/requests/buddy_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     3910 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/requests/buddy_requests/buddy_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     5602 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/requests/buddy_requests/buddy_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     4246 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/requests/user_requests.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.174839 NEMO-4.6.1/NEMO/templates/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2950 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/resources/modify_resource.html
+-rw-rw-rw-   0 root         (0) root         (0)     3846 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/resources/resource_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/resources/resources.html
+-rw-rw-rw-   0 root         (0) root         (0)     3898 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/resources/scheduled_outage.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.174839 NEMO-4.6.1/NEMO/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/rest_framework/api.html
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/rest_framework/custom_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.176839 NEMO-4.6.1/NEMO/templates/safety/
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/safety/safety.html
+-rw-rw-rw-   0 root         (0) root         (0)     1733 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/safety/safety_base.html
+-rw-rw-rw-   0 root         (0) root         (0)     7807 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/safety/safety_data_sheets.html
+-rw-rw-rw-   0 root         (0) root         (0)     1976 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/safety/safety_issues.html
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/safety/safety_issues_create.html
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/safety/safety_issues_resolved.html
+-rw-rw-rw-   0 root         (0) root         (0)     1762 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/safety/safety_issues_update.html
+-rw-rw-rw-   0 root         (0) root         (0)     1877 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/safety/safety_items.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.176839 NEMO-4.6.1/NEMO/templates/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/snippets/button.html
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/snippets/contact_person.html
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/snippets/document_list.html
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/snippets/embedded_document.html
+-rw-rw-rw-   0 root         (0) root         (0)     1673 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/snippets/tool_info.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.177839 NEMO-4.6.1/NEMO/templates/staff_charges/
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/staff_charges/change_status.html
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/staff_charges/choose_project.html
+-rw-rw-rw-   0 root         (0) root         (0)      498 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/staff_charges/end_area_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/staff_charges/new_staff_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/staff_charges/reminder.html
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/staff_charges/staff_charges_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.178839 NEMO-4.6.1/NEMO/templates/status_dashboard/
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/status_dashboard/occupancy.html
+-rw-rw-rw-   0 root         (0) root         (0)     9772 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/templates/status_dashboard/staff.html
+-rw-rw-rw-   0 root         (0) root         (0)     7709 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/status_dashboard/staff_absence.html
+-rw-rw-rw-   0 root         (0) root         (0)     6650 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/status_dashboard/status_dashboard.html
+-rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/status_dashboard/tools.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.178839 NEMO-4.6.1/NEMO/templates/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/tasks/resolve.html
+-rw-rw-rw-   0 root         (0) root         (0)     5037 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/tasks/update.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.179839 NEMO-4.6.1/NEMO/templates/tool_control/
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/tool_control/get_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      737 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/tool_control/interlock_error.html
+-rw-rw-rw-   0 root         (0) root         (0)     3502 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/tool_control/past_tasks_and_comments.html
+-rw-rw-rw-   0 root         (0) root         (0)     2466 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/tool_control/qualified_users.html
+-rw-rw-rw-   0 root         (0) root         (0)    15303 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/tool_control/tool_control.html
+-rw-rw-rw-   0 root         (0) root         (0)    37737 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/tool_control/tool_status.html
+-rw-rw-rw-   0 root         (0) root         (0)     6142 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/tool_control/usage_data.html
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/tool_control/use_tool_for_other.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.180839 NEMO-4.6.1/NEMO/templates/training/
+-rw-rw-rw-   0 root         (0) root         (0)      512 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/training/get_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     4971 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/training/training.html
+-rw-rw-rw-   0 root         (0) root         (0)     1962 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/training/training_entry.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.180839 NEMO-4.6.1/NEMO/templates/usage/
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/usage/adjustment_request_button.html
+-rw-rw-rw-   0 root         (0) root         (0)     3573 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/usage/billing.html
+-rw-rw-rw-   0 root         (0) root         (0)     9218 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/usage/usage.html
+-rw-rw-rw-   0 root         (0) root         (0)     7812 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/usage/usage_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.181839 NEMO-4.6.1/NEMO/templates/users/
+-rw-rw-rw-   0 root         (0) root         (0)    20776 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/users/create_or_modify_user.html
+-rw-rw-rw-   0 root         (0) root         (0)    18558 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/users/preferences.html
+-rw-rw-rw-   0 root         (0) root         (0)     3758 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/users/safe_deactivation.html
+-rw-rw-rw-   0 root         (0) root         (0)     4181 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templates/users/users.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.181839 NEMO-4.6.1/NEMO/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8447 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/templatetags/custom_tags_and_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    26303 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    24695 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.188839 NEMO-4.6.1/NEMO/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4308 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/abuse.py
+-rw-rw-rw-   0 root         (0) root         (0)    14733 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/access_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     8275 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/accounts_and_projects.py
+-rw-rw-rw-   0 root         (0) root         (0)    19286 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/views/adjustment_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     1812 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)    14004 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    12252 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/api_billing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2415 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/api_file_import.py
+-rw-rw-rw-   0 root         (0) root         (0)    19042 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/area_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    12070 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     6625 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/buddy_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    71831 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/views/calendar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2334 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/charge_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/configuration_agenda.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    10947 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/consumables.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/contact_staff.py
+-rw-rw-rw-   0 root         (0) root         (0)    18748 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/views/customization.py
+-rw-rw-rw-   0 root         (0) root         (0)     3442 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/documents.py
+-rw-rw-rw-   0 root         (0) root         (0)    10015 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/event_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/feedback.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/get_projects.py
+-rw-rw-rw-   0 root         (0) root         (0)     4168 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/history.py
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/jumbotron.py
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/landing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/maintenance.py
+-rw-rw-rw-   0 root         (0) root         (0)     8072 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/mobile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3356 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/news.py
+-rw-rw-rw-   0 root         (0) root         (0)     5095 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/views/notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     4822 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/qualifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     9506 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/remote_work.py
+-rw-rw-rw-   0 root         (0) root         (0)     3700 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     8877 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/safety.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/sidebar.py
+-rw-rw-rw-   0 root         (0) root         (0)    20146 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/status_dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)    13615 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)    23995 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/tool_control.py
+-rw-rw-rw-   0 root         (0) root         (0)     6043 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/training.py
+-rw-rw-rw-   0 root         (0) root         (0)     1909 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/tutorials.py
+-rw-rw-rw-   0 root         (0) root         (0)    18360 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/user_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    20715 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/views/users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.189839 NEMO-4.6.1/NEMO/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 22:28:19.000000 NEMO-4.6.1/NEMO/widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2968 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/widgets/configuration_editor.py
+-rw-rw-rw-   0 root         (0) root         (0)    26383 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/widgets/dynamic_form.py
+-rw-rw-rw-   0 root         (0) root         (0)     8029 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/widgets/item_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-18 17:03:12.000000 NEMO-4.6.1/NEMO/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.124838 NEMO-4.6.1/NEMO.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      904 2023-07-25 22:28:31.000000 NEMO-4.6.1/NEMO.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17413 2023-07-25 22:28:31.000000 NEMO-4.6.1/NEMO.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 22:28:31.000000 NEMO-4.6.1/NEMO.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-25 22:28:31.000000 NEMO-4.6.1/NEMO.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      264 2023-07-25 22:28:31.000000 NEMO-4.6.1/NEMO.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-25 22:28:31.000000 NEMO-4.6.1/NEMO.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      904 2023-07-25 22:28:31.190839 NEMO-4.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4066 2023-07-18 17:03:12.000000 NEMO-4.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 22:28:31.189839 NEMO-4.6.1/resources/
+-rw-rw-rw-   0 root         (0) root         (0)    17163 2023-07-25 22:28:19.000000 NEMO-4.6.1/resources/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     3981 2023-07-18 17:03:12.000000 NEMO-4.6.1/resources/splash_pad_settings.py
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-25 22:28:31.190839 NEMO-4.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-25 22:28:19.000000 NEMO-4.6.1/setup.py
```

### Comparing `NEMO-4.6.0/LICENSE.md` & `NEMO-4.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/__init__.py` & `NEMO-4.6.1/NEMO/__init__.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/actions.py` & `NEMO-4.6.1/NEMO/actions.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/admin.py` & `NEMO-4.6.1/NEMO/admin.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/already_logged_in.html` & `NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/already_logged_in.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/base.html` & `NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/choose_project.html` & `NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/choose_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/logout_warning.html` & `NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/logout_warning.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/area_access/templates/area_access/resource_unavailable.html` & `NEMO-4.6.1/NEMO/apps/area_access/templates/area_access/resource_unavailable.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/area_access/urls.py` & `NEMO-4.6.1/NEMO/apps/area_access/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/area_access/views.py` & `NEMO-4.6.1/NEMO/apps/area_access/views.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/contracts/admin.py` & `NEMO-4.6.1/NEMO/apps/contracts/admin.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/contracts/migrations/0001_initial.py` & `NEMO-4.6.1/NEMO/apps/contracts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/contracts/models.py` & `NEMO-4.6.1/NEMO/apps/contracts/models.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/contracts/templates/contracts/contractors.html` & `NEMO-4.6.1/NEMO/apps/contracts/templates/contracts/contractors.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/contracts/templates/contracts/contracts_and_procurements.html` & `NEMO-4.6.1/NEMO/apps/contracts/templates/contracts/contracts_and_procurements.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/contracts/templates/contracts/procurements.html` & `NEMO-4.6.1/NEMO/apps/contracts/templates/contracts/procurements.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/contracts/templates/contracts/service_contracts.html` & `NEMO-4.6.1/NEMO/apps/contracts/templates/contracts/service_contracts.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/contracts/templates/customizations/customizations_contracts.html` & `NEMO-4.6.1/NEMO/apps/contracts/templates/customizations/customizations_contracts.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/contracts/urls.py` & `NEMO-4.6.1/NEMO/apps/contracts/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/contracts/views/contracts.py` & `NEMO-4.6.1/NEMO/apps/contracts/views/contracts.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/category_choices.html` & `NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/category_choices.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/choices.html` & `NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/choices.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/error.html` & `NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/error.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html` & `NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/kiosk.html` & `NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/kiosk.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/success.html` & `NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/success.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/tool_information.html` & `NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/tool_information.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html` & `NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html` & `NEMO-4.6.1/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/kiosk/urls.py` & `NEMO-4.6.1/NEMO/apps/kiosk/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/kiosk/views.py` & `NEMO-4.6.1/NEMO/apps/kiosk/views.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/sensors/admin.py` & `NEMO-4.6.1/NEMO/apps/sensors/admin.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/sensors/customizations.py` & `NEMO-4.6.1/NEMO/apps/sensors/customizations.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/sensors/evaluators.py` & `NEMO-4.6.1/NEMO/apps/sensors/evaluators.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/sensors/migrations/0001_initial.py` & `NEMO-4.6.1/NEMO/apps/sensors/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/sensors/models.py` & `NEMO-4.6.1/NEMO/apps/sensors/models.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/sensors/sensors.py` & `NEMO-4.6.1/NEMO/apps/sensors/sensors.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/sensors/static/sensors/chart.js` & `NEMO-4.6.1/NEMO/apps/sensors/static/sensors/chart.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/sensors/static/sensors/chart.min.js` & `NEMO-4.6.1/NEMO/apps/sensors/static/sensors/chart.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js` & `NEMO-4.6.1/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/sensors/static/sensors/daterangepicker.css` & `NEMO-4.6.1/NEMO/apps/sensors/static/sensors/daterangepicker.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/sensors/static/sensors/daterangepicker.js` & `NEMO-4.6.1/NEMO/apps/sensors/static/sensors/daterangepicker.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/sensors/static/sensors/sensors.css` & `NEMO-4.6.1/NEMO/apps/sensors/static/sensors/sensors.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/sensors/templates/customizations/customizations_sensors.html` & `NEMO-4.6.1/NEMO/apps/sensors/templates/customizations/customizations_sensors.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/sensors/templates/sensors/sensor_data.html` & `NEMO-4.6.1/NEMO/apps/sensors/templates/sensors/sensor_data.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/sensors/templates/sensors/sensors.html` & `NEMO-4.6.1/NEMO/apps/sensors/templates/sensors/sensors.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/sensors/urls.py` & `NEMO-4.6.1/NEMO/apps/sensors/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/apps/sensors/views.py` & `NEMO-4.6.1/NEMO/apps/sensors/views.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/context_processors.py` & `NEMO-4.6.1/NEMO/context_processors.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/decorators.py` & `NEMO-4.6.1/NEMO/decorators.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/exceptions.py` & `NEMO-4.6.1/NEMO/exceptions.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/fields.py` & `NEMO-4.6.1/NEMO/fields.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/forms.py` & `NEMO-4.6.1/NEMO/forms.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/interlocks.py` & `NEMO-4.6.1/NEMO/interlocks.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/management/commands/send_email_usage_reminders.py` & `NEMO-4.6.1/NEMO/management/commands/send_email_usage_reminders.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/middleware.py` & `NEMO-4.6.1/NEMO/middleware.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0001_version_1_0_0.py` & `NEMO-4.6.1/NEMO/migrations/0001_version_1_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0002_version_1_0_0_squashed.py` & `NEMO-4.6.1/NEMO/migrations/0002_version_1_0_0_squashed.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0012_version_2_0_0_squashed.py` & `NEMO-4.6.1/NEMO/migrations/0012_version_2_0_0_squashed.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0020_version_3_0_0.py` & `NEMO-4.6.1/NEMO/migrations/0020_version_3_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0021_version_3_1_0.py` & `NEMO-4.6.1/NEMO/migrations/0021_version_3_1_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0022_version_3_3_0.py` & `NEMO-4.6.1/NEMO/migrations/0022_version_3_3_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0023_badgereader.py` & `NEMO-4.6.1/NEMO/migrations/0023_badgereader.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0024_contactinformation_user.py` & `NEMO-4.6.1/NEMO/migrations/0024_contactinformation_user.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0025_version_3_6_0.py` & `NEMO-4.6.1/NEMO/migrations/0025_version_3_6_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0026_version_3_7_0.py` & `NEMO-4.6.1/NEMO/migrations/0026_version_3_7_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0028_version_3_9_0.py` & `NEMO-4.6.1/NEMO/migrations/0028_version_3_9_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0030_version_3_9_2.py` & `NEMO-4.6.1/NEMO/migrations/0030_version_3_9_2.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0031_version_3_10_0.py` & `NEMO-4.6.1/NEMO/migrations/0031_version_3_10_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0032_version_3_11_0.py` & `NEMO-4.6.1/NEMO/migrations/0032_version_3_11_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0035_version_3_14_0.py` & `NEMO-4.6.1/NEMO/migrations/0035_version_3_14_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0036_version_3_15_0.py` & `NEMO-4.6.1/NEMO/migrations/0036_version_3_15_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0037_version_3_16_0.py` & `NEMO-4.6.1/NEMO/migrations/0037_version_3_16_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0038_version_4_0_0.py` & `NEMO-4.6.1/NEMO/migrations/0038_version_4_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0039_version_4_1_0.py` & `NEMO-4.6.1/NEMO/migrations/0039_version_4_1_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0040_version_4_2_0.py` & `NEMO-4.6.1/NEMO/migrations/0040_version_4_2_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0042_version_4_3_0.py` & `NEMO-4.6.1/NEMO/migrations/0042_version_4_3_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0043_version_4_3_2.py` & `NEMO-4.6.1/NEMO/migrations/0043_version_4_3_2.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0044_version_4_4_0.py` & `NEMO-4.6.1/NEMO/migrations/0044_version_4_4_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0045_version_4_5_0.py` & `NEMO-4.6.1/NEMO/migrations/0045_version_4_5_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0045_version_4_5_5.py` & `NEMO-4.6.1/NEMO/migrations/0045_version_4_5_5.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations/0046_version_4_6_0.py` & `NEMO-4.6.1/NEMO/migrations/0046_version_4_6_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/migrations_utils.py` & `NEMO-4.6.1/NEMO/migrations_utils.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/mixins.py` & `NEMO-4.6.1/NEMO/mixins.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/model_tree.py` & `NEMO-4.6.1/NEMO/model_tree.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/models.py` & `NEMO-4.6.1/NEMO/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2563,15 +2563,15 @@
 		ordering = ['display_order']
 
 	def __str__(self):
 		return str(self.name)
 
 
 class Customization(BaseModel):
-	name = models.CharField(primary_key=True, max_length=50)
+	name = models.CharField(primary_key=True, max_length=100)
 	value = models.TextField()
 
 	class Meta:
 		ordering = ["name"]
 
 	def __str__(self):
 		return str(self.name)
```

### Comparing `NEMO-4.6.0/NEMO/parsers.py` & `NEMO-4.6.1/NEMO/parsers.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/permissions.py` & `NEMO-4.6.1/NEMO/permissions.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/policy.py` & `NEMO-4.6.1/NEMO/policy.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/provisioning.py` & `NEMO-4.6.1/NEMO/provisioning.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/rates.py` & `NEMO-4.6.1/NEMO/rates.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/rest_filter_backend.py` & `NEMO-4.6.1/NEMO/rest_filter_backend.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/serializers.py` & `NEMO-4.6.1/NEMO/serializers.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/admin/physical_access_level/access_level.js` & `NEMO-4.6.1/NEMO/static/admin/physical_access_level/access_level.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/admin/questions_preview/questions_preview.css` & `NEMO-4.6.1/NEMO/static/admin/questions_preview/questions_preview.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/admin/questions_preview/questions_preview.js` & `NEMO-4.6.1/NEMO/static/admin/questions_preview/questions_preview.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/admin/time_options_override.js` & `NEMO-4.6.1/NEMO/static/admin/time_options_override.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/admin/tool/tool.js` & `NEMO-4.6.1/NEMO/static/admin/tool/tool.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/badge_reader.js` & `NEMO-4.6.1/NEMO/static/badge_reader.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap-theme.css` & `NEMO-4.6.1/NEMO/static/bootstrap/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap-theme.css.map` & `NEMO-4.6.1/NEMO/static/bootstrap/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap-theme.min.css` & `NEMO-4.6.1/NEMO/static/bootstrap/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap.css` & `NEMO-4.6.1/NEMO/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap.css.map` & `NEMO-4.6.1/NEMO/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/bootstrap/css/bootstrap.min.css` & `NEMO-4.6.1/NEMO/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot` & `NEMO-4.6.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg` & `NEMO-4.6.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `NEMO-4.6.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff` & `NEMO-4.6.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `NEMO-4.6.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/bootstrap/js/bootstrap.js` & `NEMO-4.6.1/NEMO/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/bootstrap/js/bootstrap.min.js` & `NEMO-4.6.1/NEMO/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/datetimepicker/bootstrap-datetimepicker.css` & `NEMO-4.6.1/NEMO/static/datetimepicker/bootstrap-datetimepicker.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/datetimepicker/bootstrap-datetimepicker.js` & `NEMO-4.6.1/NEMO/static/datetimepicker/bootstrap-datetimepicker.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/favicon.ico` & `NEMO-4.6.1/NEMO/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/fullcalendar/fullcalendar.css` & `NEMO-4.6.1/NEMO/static/fullcalendar/fullcalendar.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/fullcalendar/fullcalendar.js` & `NEMO-4.6.1/NEMO/static/fullcalendar/fullcalendar.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/fullcalendar/fullcalendar.min.css` & `NEMO-4.6.1/NEMO/static/fullcalendar/fullcalendar.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/fullcalendar/fullcalendar.min.js` & `NEMO-4.6.1/NEMO/static/fullcalendar/fullcalendar.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/icons/agreement.png` & `NEMO-4.6.1/NEMO/static/icons/agreement.png`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/icons/caution.png` & `NEMO-4.6.1/NEMO/static/icons/caution.png`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/icons/preferences.png` & `NEMO-4.6.1/NEMO/static/icons/preferences.png`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/jquery.js` & `NEMO-4.6.1/NEMO/static/jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/jquery.min.js` & `NEMO-4.6.1/NEMO/static/jquery.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/jumbotron_watermark.bmp` & `NEMO-4.6.1/NEMO/static/jumbotron_watermark.bmp`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/mobile.js` & `NEMO-4.6.1/NEMO/static/mobile.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/moment.js` & `NEMO-4.6.1/NEMO/static/moment.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/moment.min.js` & `NEMO-4.6.1/NEMO/static/moment.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/moment.min.js.map` & `NEMO-4.6.1/NEMO/static/moment.min.js.map`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/nemo.css` & `NEMO-4.6.1/NEMO/static/nemo.css`

 * *Files 2% similar despite different names*

```diff
@@ -237,14 +237,24 @@
 
 table > tbody > tr.no-border > td, table > tbody > tr.no-border > th,
 table > thead > tr.no-border > td, table > thead > tr.no-border > th
 {
 	border: none;
 }
 
+.table-borderless > tbody > tr > td,
+.table-borderless > tbody > tr > th,
+.table-borderless > tfoot > tr > td,
+.table-borderless > tfoot > tr > th,
+.table-borderless > thead > tr > td,
+.table-borderless > thead > tr > th
+{
+    border: none;
+}
+
 .table .thead-light th, .table.thead-light th
 {
     color: #495057;
     background-color: #e9ecef;
     border-color: #dee2e6;
 }
 
@@ -1087,14 +1097,15 @@
 }
 
 .usage-charge-adjustment-button
 {
 	position: absolute;
 	top: 15px;
 	right: 15px;
+	white-space: nowrap;
 }
 
 /* Table default color enforcing (useful when using sticky columns) */
 .table > thead > tr > td.default,
 .table > tbody > tr > td.default,
 .table > tfoot > tr > td.default,
 .table > thead > tr > th.default,
```

### Comparing `NEMO-4.6.0/NEMO/static/nemo.js` & `NEMO-4.6.1/NEMO/static/nemo.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/numpad/custom_numpad.jquery.js` & `NEMO-4.6.1/NEMO/static/numpad/custom_numpad.jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/pickadate/default.css` & `NEMO-4.6.1/NEMO/static/pickadate/default.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/pickadate/default.date.css` & `NEMO-4.6.1/NEMO/static/pickadate/default.date.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/pickadate/default.time.css` & `NEMO-4.6.1/NEMO/static/pickadate/default.time.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/pickadate/picker.date.js` & `NEMO-4.6.1/NEMO/static/pickadate/picker.date.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/pickadate/picker.js` & `NEMO-4.6.1/NEMO/static/pickadate/picker.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/pickadate/picker.time.js` & `NEMO-4.6.1/NEMO/static/pickadate/picker.time.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/typeahead.jquery.js` & `NEMO-4.6.1/NEMO/static/typeahead.jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/typeahead.jquery.min.js` & `NEMO-4.6.1/NEMO/static/typeahead.jquery.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/virtualkeyboard/jquery.keyboard.js` & `NEMO-4.6.1/NEMO/static/virtualkeyboard/jquery.keyboard.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/virtualkeyboard/jquery.keyboard.min.js` & `NEMO-4.6.1/NEMO/static/virtualkeyboard/jquery.keyboard.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/virtualkeyboard/keyboard-basic.css` & `NEMO-4.6.1/NEMO/static/virtualkeyboard/keyboard-basic.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/static/virtualkeyboard/keyboard-basic.min.css` & `NEMO-4.6.1/NEMO/static/virtualkeyboard/keyboard-basic.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/abuse/abuse.html` & `NEMO-4.6.1/NEMO/templates/abuse/abuse.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/abuse/user_drill_down.html` & `NEMO-4.6.1/NEMO/templates/abuse/user_drill_down.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/accounts_and_projects/account_and_projects.html` & `NEMO-4.6.1/NEMO/templates/accounts_and_projects/account_and_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/accounts_and_projects/accounts_and_projects.html` & `NEMO-4.6.1/NEMO/templates/accounts_and_projects/accounts_and_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/accounts_and_projects/create_account.html` & `NEMO-4.6.1/NEMO/templates/accounts_and_projects/create_account.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/accounts_and_projects/create_project.html` & `NEMO-4.6.1/NEMO/templates/accounts_and_projects/create_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/accounts_and_projects/documents_for_project.html` & `NEMO-4.6.1/NEMO/templates/accounts_and_projects/documents_for_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/accounts_and_projects/projects.html` & `NEMO-4.6.1/NEMO/templates/accounts_and_projects/projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/accounts_and_projects/users_for_project.html` & `NEMO-4.6.1/NEMO/templates/accounts_and_projects/users_for_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/alerts.html` & `NEMO-4.6.1/NEMO/templates/alerts.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/area_access/area_access.html` & `NEMO-4.6.1/NEMO/templates/area_access/area_access.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/area_access/calendar_self_login.html` & `NEMO-4.6.1/NEMO/templates/area_access/calendar_self_login.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/area_access/change_project.html` & `NEMO-4.6.1/NEMO/templates/area_access/change_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/area_access/login_areas.html` & `NEMO-4.6.1/NEMO/templates/area_access/login_areas.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/area_access/new_area_access_record.html` & `NEMO-4.6.1/NEMO/templates/area_access/new_area_access_record.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/area_access/new_area_access_record_details.html` & `NEMO-4.6.1/NEMO/templates/area_access/new_area_access_record_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/area_access/self_login.html` & `NEMO-4.6.1/NEMO/templates/area_access/self_login.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/authorization_failed.html` & `NEMO-4.6.1/NEMO/templates/authorization_failed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/base/navbar_base.html` & `NEMO-4.6.1/NEMO/templates/base/navbar_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/base.html` & `NEMO-4.6.1/NEMO/templates/base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/calendar/calendar.html` & `NEMO-4.6.1/NEMO/templates/calendar/calendar.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/calendar/configuration.html` & `NEMO-4.6.1/NEMO/templates/calendar/configuration.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/calendar/configuration_helper.html` & `NEMO-4.6.1/NEMO/templates/calendar/configuration_helper.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/calendar/policy_dialog.html` & `NEMO-4.6.1/NEMO/templates/calendar/policy_dialog.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/calendar/project_choice.html` & `NEMO-4.6.1/NEMO/templates/calendar/project_choice.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/calendar/proxy_reservation.html` & `NEMO-4.6.1/NEMO/templates/calendar/proxy_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/calendar/reservation_event_feed.html` & `NEMO-4.6.1/NEMO/templates/calendar/reservation_event_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/calendar/reservation_questions.html` & `NEMO-4.6.1/NEMO/templates/calendar/reservation_questions.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/calendar/reservation_warning.html` & `NEMO-4.6.1/NEMO/templates/calendar/reservation_warning.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/calendar/scheduled_outage_information.html` & `NEMO-4.6.1/NEMO/templates/calendar/scheduled_outage_information.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/calendar/specific_user_feed.html` & `NEMO-4.6.1/NEMO/templates/calendar/specific_user_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/calendar/usage_event_feed.html` & `NEMO-4.6.1/NEMO/templates/calendar/usage_event_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/configuration_agenda.html` & `NEMO-4.6.1/NEMO/templates/configuration_agenda.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/consumables/consumables.html` & `NEMO-4.6.1/NEMO/templates/consumables/consumables.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/consumables/consumables_order.html` & `NEMO-4.6.1/NEMO/templates/consumables/consumables_order.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/consumables/recurring_charge.html` & `NEMO-4.6.1/NEMO/templates/consumables/recurring_charge.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/consumables/recurring_charges.html` & `NEMO-4.6.1/NEMO/templates/consumables/recurring_charges.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/contact/contact_staff.html` & `NEMO-4.6.1/NEMO/templates/contact/contact_staff.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/customizations/customizations.html` & `NEMO-4.6.1/NEMO/templates/customizations/customizations.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/customizations/customizations_application.html` & `NEMO-4.6.1/NEMO/templates/customizations/customizations_application.html`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,23 @@
                     <label><input type="checkbox" name="self_log_out" {% if self_log_out %}checked{% endif %} value="enabled">Allow users to log themselves out of access controlled areas from the landing page</label><br/>
                     <label><input type="checkbox" name="calendar_login_logout" {% if calendar_login_logout %}checked{% endif %} value="enabled">Show access controlled area login/logout button on calendar view (requires login and/or logout feature enabled above)</label>
                     {% if "NEMO.apps.area_access"|app_installed %}<label><input type="checkbox" name="area_logout_already_logged_in" {% if area_logout_already_logged_in %}checked{% endif %} value="enabled">Automatically log users out when they try to log in to an area they are already logged in (single entrance/exit tablet mode)</label>{% endif %}
                 </div>
             </div>
         </div>
         <div class="form-group">
+            <label class="control-label col-md-3">Area usage reminder</label>
+            <div class="col-md-9">
+                <div class="checkbox">
+                    <input type="hidden" name="area_in_usage_reminders" value="off"/>
+                    <label><input type="checkbox" name="area_in_usage_reminders" {% if area_in_usage_reminders != "off" %}checked{% endif %} value="">In usage reminder emails, show areas users are currently logged in</label><br/>
+                </div>
+            </div>
+        </div>
+        <div class="form-group">
             <label class="control-label col-md-3">Consumables</label>
             <div class="col-md-9">
                 <div class="checkbox">
                     <label><input type="checkbox" name="consumable_user_self_checkout" {% if consumable_user_self_checkout %}checked{% endif %} value="enabled">Allow users to self-checkout consumables</label>
                 </div>
             </div>
             <div class="col-md-offset-3 col-md-9 help-block light-grey">
```

#### html2text {}

```diff
@@ -14,14 +14,18 @@
 themselves out of access controlled areas from the landing page
 % if calendar_login_logout %}checked{% endif %} value="enabled">Show access
 controlled area login/logout button on calendar view (requires login and/or
 logout feature enabled above) {% if "NEMO.apps.area_access"|app_installed %}
 % if area_logout_already_logged_in %}checked{% endif %}
 value="enabled">Automatically log users out when they try to log in to an area
 they are already logged in (single entrance/exit tablet mode){% endif %}
+Area usage reminder
+
+% if area_in_usage_reminders != "off" %}checked{% endif %} value="">In usage
+reminder emails, show areas users are currently logged in
 Consumables
 % if consumable_user_self_checkout %}checked{% endif %} value="enabled">Allow
 users to self-checkout consumables
 If enabled, you need to add a {% if "django.contrib.admin"|app_installed
 %}landing_page_choice{% else %}landing page option{% endif %} with url /
 consumables/ so users can have a way to get to the page.
 {% if "NEMO.apps.area_access"|app_installed or "NEMO.apps.kiosk"|app_installed
```

### Comparing `NEMO-4.6.0/NEMO/templates/customizations/customizations_calendar.html` & `NEMO-4.6.1/NEMO/templates/customizations/customizations_calendar.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/customizations/customizations_dashboard.html` & `NEMO-4.6.1/NEMO/templates/customizations/customizations_dashboard.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/customizations/customizations_emails.html` & `NEMO-4.6.1/NEMO/templates/customizations/customizations_emails.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/customizations/customizations_interlock.html` & `NEMO-4.6.1/NEMO/templates/customizations/customizations_interlock.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/customizations/customizations_projects_and_accounts.html` & `NEMO-4.6.1/NEMO/templates/customizations/customizations_projects_and_accounts.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/customizations/customizations_rates.html` & `NEMO-4.6.1/NEMO/templates/customizations/customizations_rates.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/customizations/customizations_recurring_charges.html` & `NEMO-4.6.1/NEMO/templates/customizations/customizations_recurring_charges.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/customizations/customizations_remote_work.html` & `NEMO-4.6.1/NEMO/templates/customizations/customizations_remote_work.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/customizations/customizations_requests.html` & `NEMO-4.6.1/NEMO/templates/customizations/customizations_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/customizations/customizations_safety.html` & `NEMO-4.6.1/NEMO/templates/customizations/customizations_safety.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/customizations/customizations_templates.html` & `NEMO-4.6.1/NEMO/templates/customizations/customizations_templates.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/customizations/customizations_tool.html` & `NEMO-4.6.1/NEMO/templates/customizations/customizations_tool.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/customizations/customizations_upload.html` & `NEMO-4.6.1/NEMO/templates/customizations/customizations_upload.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/customizations/customizations_user.html` & `NEMO-4.6.1/NEMO/templates/customizations/customizations_user.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/email/compose_email.html` & `NEMO-4.6.1/NEMO/templates/email/compose_email.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/email/email_broadcast.html` & `NEMO-4.6.1/NEMO/templates/email/email_broadcast.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/email/email_form.html` & `NEMO-4.6.1/NEMO/templates/email/email_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/event_details/area_access_details.html` & `NEMO-4.6.1/NEMO/templates/event_details/area_access_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/event_details/outage_details.html` & `NEMO-4.6.1/NEMO/templates/event_details/outage_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/event_details/reservation_details.html` & `NEMO-4.6.1/NEMO/templates/event_details/reservation_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/event_details/usage_details.html` & `NEMO-4.6.1/NEMO/templates/event_details/usage_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/feedback.html` & `NEMO-4.6.1/NEMO/templates/feedback.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/history.html` & `NEMO-4.6.1/NEMO/templates/history.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/impersonate.html` & `NEMO-4.6.1/NEMO/templates/impersonate.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/jumbotron/jumbotron.html` & `NEMO-4.6.1/NEMO/templates/jumbotron/jumbotron.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/jumbotron/jumbotron_content.html` & `NEMO-4.6.1/NEMO/templates/jumbotron/jumbotron_content.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/landing.html` & `NEMO-4.6.1/NEMO/templates/landing.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/login.html` & `NEMO-4.6.1/NEMO/templates/login.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/maintenance/closed_task_details.html` & `NEMO-4.6.1/NEMO/templates/maintenance/closed_task_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/maintenance/maintenance.html` & `NEMO-4.6.1/NEMO/templates/maintenance/maintenance.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/maintenance/pending_task_details.html` & `NEMO-4.6.1/NEMO/templates/maintenance/pending_task_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/mobile/cancellation_result.html` & `NEMO-4.6.1/NEMO/templates/mobile/cancellation_result.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/mobile/choose_item.html` & `NEMO-4.6.1/NEMO/templates/mobile/choose_item.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/mobile/individual_outage.html` & `NEMO-4.6.1/NEMO/templates/mobile/individual_outage.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/mobile/individual_reservation.html` & `NEMO-4.6.1/NEMO/templates/mobile/individual_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/mobile/new_reservation.html` & `NEMO-4.6.1/NEMO/templates/mobile/new_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/mobile/reservation_success.html` & `NEMO-4.6.1/NEMO/templates/mobile/reservation_success.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/mobile/view_calendar.html` & `NEMO-4.6.1/NEMO/templates/mobile/view_calendar.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/news/archived_news.html` & `NEMO-4.6.1/NEMO/templates/news/archived_news.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/news/new_news_form.html` & `NEMO-4.6.1/NEMO/templates/news/new_news_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/news/news_update_form.html` & `NEMO-4.6.1/NEMO/templates/news/news_update_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/news/recent_news.html` & `NEMO-4.6.1/NEMO/templates/news/recent_news.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/occupancy/occupancy_content.html` & `NEMO-4.6.1/NEMO/templates/occupancy/occupancy_content.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/occupancy/occupancy_count.html` & `NEMO-4.6.1/NEMO/templates/occupancy/occupancy_count.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/pagination/pagination_base.html` & `NEMO-4.6.1/NEMO/templates/pagination/pagination_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/pagination/pagination_column.html` & `NEMO-4.6.1/NEMO/templates/pagination/pagination_column.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/pagination/pagination_pages.html` & `NEMO-4.6.1/NEMO/templates/pagination/pagination_pages.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/pagination/pagination_selector.html` & `NEMO-4.6.1/NEMO/templates/pagination/pagination_selector.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/qualifications.html` & `NEMO-4.6.1/NEMO/templates/qualifications.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/refresh_sidebar_icons.html` & `NEMO-4.6.1/NEMO/templates/refresh_sidebar_icons.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/remote_work/remote_work.html` & `NEMO-4.6.1/NEMO/templates/remote_work/remote_work.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/remote_work/remote_work_base.html` & `NEMO-4.6.1/NEMO/templates/remote_work/remote_work_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/requests/access_requests/access_request.html` & `NEMO-4.6.1/NEMO/templates/requests/access_requests/access_request.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/requests/access_requests/access_requests.html` & `NEMO-4.6.1/NEMO/templates/requests/access_requests/access_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/requests/access_requests/access_requests_table.html` & `NEMO-4.6.1/NEMO/templates/requests/access_requests/access_requests_table.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/requests/adjustment_requests/adjustment_request.html` & `NEMO-4.6.1/NEMO/templates/requests/adjustment_requests/adjustment_request.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/requests/adjustment_requests/adjustment_requests.html` & `NEMO-4.6.1/NEMO/templates/requests/adjustment_requests/adjustment_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html` & `NEMO-4.6.1/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/requests/buddy_requests/buddy_request.html` & `NEMO-4.6.1/NEMO/templates/requests/buddy_requests/buddy_request.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/requests/buddy_requests/buddy_requests.html` & `NEMO-4.6.1/NEMO/templates/requests/buddy_requests/buddy_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/requests/user_requests.html` & `NEMO-4.6.1/NEMO/templates/requests/user_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/resources/modify_resource.html` & `NEMO-4.6.1/NEMO/templates/resources/modify_resource.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/resources/resource_details.html` & `NEMO-4.6.1/NEMO/templates/resources/resource_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/resources/resources.html` & `NEMO-4.6.1/NEMO/templates/resources/resources.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/resources/scheduled_outage.html` & `NEMO-4.6.1/NEMO/templates/resources/scheduled_outage.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/rest_framework/api.html` & `NEMO-4.6.1/NEMO/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/safety/safety.html` & `NEMO-4.6.1/NEMO/templates/safety/safety.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/safety/safety_base.html` & `NEMO-4.6.1/NEMO/templates/safety/safety_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/safety/safety_data_sheets.html` & `NEMO-4.6.1/NEMO/templates/safety/safety_data_sheets.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/safety/safety_issues.html` & `NEMO-4.6.1/NEMO/templates/safety/safety_issues.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/safety/safety_issues_create.html` & `NEMO-4.6.1/NEMO/templates/safety/safety_issues_create.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/safety/safety_issues_resolved.html` & `NEMO-4.6.1/NEMO/templates/safety/safety_issues_resolved.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/safety/safety_issues_update.html` & `NEMO-4.6.1/NEMO/templates/safety/safety_issues_update.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/safety/safety_items.html` & `NEMO-4.6.1/NEMO/templates/safety/safety_items.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/snippets/button.html` & `NEMO-4.6.1/NEMO/templates/snippets/button.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/snippets/contact_person.html` & `NEMO-4.6.1/NEMO/templates/snippets/contact_person.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/snippets/document_list.html` & `NEMO-4.6.1/NEMO/templates/snippets/document_list.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/snippets/embedded_document.html` & `NEMO-4.6.1/NEMO/templates/snippets/embedded_document.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/snippets/tool_info.html` & `NEMO-4.6.1/NEMO/templates/snippets/tool_info.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/staff_charges/change_status.html` & `NEMO-4.6.1/NEMO/templates/staff_charges/change_status.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/staff_charges/choose_project.html` & `NEMO-4.6.1/NEMO/templates/staff_charges/choose_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/staff_charges/new_staff_charge.html` & `NEMO-4.6.1/NEMO/templates/staff_charges/new_staff_charge.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/staff_charges/reminder.html` & `NEMO-4.6.1/NEMO/templates/staff_charges/reminder.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/staff_charges/staff_charges_base.html` & `NEMO-4.6.1/NEMO/templates/staff_charges/staff_charges_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/status_dashboard/occupancy.html` & `NEMO-4.6.1/NEMO/templates/status_dashboard/occupancy.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/status_dashboard/staff.html` & `NEMO-4.6.1/NEMO/templates/status_dashboard/staff.html`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 <div id="contact-info-tooltip-container" class="info-tooltip-container" style="overflow-x: auto; margin-top: 25px; margin-bottom: 20px; border: 1px solid #ddd;">
     <table class="table table-responsive table-hover-first" style="margin: 0;border-collapse: collapse">
         <thead>
             <tr class="no-border">
                 <th class="sticky" style="background-color: white; {% if days_length == 1 %}width:33%{% endif %}" aria-label="Blank corner cell"></th>
                 {% if prev %}
                     <th class="button-column-minimum" style="vertical-align: middle;" aria-label="Previous page cell">
-                        <a style="cursor: pointer" onclick="refresh_staff_status_dashboard('timestamp={{ page_timestamp }}&view=week');" aria-label="Previous page button">
+                        <a style="cursor: pointer" onclick="refresh_staff_status_dashboard('timestamp={{ prev }}&view={{ page_view }}');" aria-label="Previous page button">
                             <i class="glyphicon glyphicon-chevron-left chevron" style="padding: 0"></i>
                         </a>
                     </th>
                 {% endif %}
                 {% for day in days %}
                     {% now 'Y-m-d' as today %}
                     <th class="text-center {% if day|date:'Y-m-d' == today %}alert-info{% endif %}">
```

### Comparing `NEMO-4.6.0/NEMO/templates/status_dashboard/staff_absence.html` & `NEMO-4.6.1/NEMO/templates/status_dashboard/staff_absence.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/status_dashboard/status_dashboard.html` & `NEMO-4.6.1/NEMO/templates/status_dashboard/status_dashboard.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/status_dashboard/tools.html` & `NEMO-4.6.1/NEMO/templates/status_dashboard/tools.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/tasks/resolve.html` & `NEMO-4.6.1/NEMO/templates/tasks/resolve.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/tasks/update.html` & `NEMO-4.6.1/NEMO/templates/tasks/update.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/tool_control/get_projects.html` & `NEMO-4.6.1/NEMO/templates/tool_control/get_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/tool_control/interlock_error.html` & `NEMO-4.6.1/NEMO/templates/tool_control/interlock_error.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/tool_control/past_tasks_and_comments.html` & `NEMO-4.6.1/NEMO/templates/tool_control/past_tasks_and_comments.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/tool_control/qualified_users.html` & `NEMO-4.6.1/NEMO/templates/tool_control/qualified_users.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/tool_control/tool_control.html` & `NEMO-4.6.1/NEMO/templates/tool_control/tool_control.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/tool_control/tool_status.html` & `NEMO-4.6.1/NEMO/templates/tool_control/tool_status.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/tool_control/usage_data.html` & `NEMO-4.6.1/NEMO/templates/tool_control/usage_data.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/training/get_projects.html` & `NEMO-4.6.1/NEMO/templates/training/get_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/training/training.html` & `NEMO-4.6.1/NEMO/templates/training/training.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/training/training_entry.html` & `NEMO-4.6.1/NEMO/templates/training/training_entry.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/usage/adjustment_request_button.html` & `NEMO-4.6.1/NEMO/templates/usage/adjustment_request_button.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/usage/billing.html` & `NEMO-4.6.1/NEMO/templates/usage/billing.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/usage/usage.html` & `NEMO-4.6.1/NEMO/templates/usage/usage.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/usage/usage_base.html` & `NEMO-4.6.1/NEMO/templates/usage/usage_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/users/create_or_modify_user.html` & `NEMO-4.6.1/NEMO/templates/users/create_or_modify_user.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/users/preferences.html` & `NEMO-4.6.1/NEMO/templates/users/preferences.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/users/safe_deactivation.html` & `NEMO-4.6.1/NEMO/templates/users/safe_deactivation.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templates/users/users.html` & `NEMO-4.6.1/NEMO/templates/users/users.html`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/templatetags/custom_tags_and_filters.py` & `NEMO-4.6.1/NEMO/templatetags/custom_tags_and_filters.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/urls.py` & `NEMO-4.6.1/NEMO/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/utilities.py` & `NEMO-4.6.1/NEMO/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,29 +518,29 @@
 	return f"chemical_documents/{chemical_name}/{filename}"
 
 
 def document_filename_upload(instance, filename):
 	return instance.get_filename_upload(filename)
 
 
-def resize_image(image: InMemoryUploadedFile, max: int, quality=85) -> InMemoryUploadedFile:
+def resize_image(image: InMemoryUploadedFile, max_size: int, quality=85) -> InMemoryUploadedFile:
 	"""Returns a resized image based on the given maximum size"""
 	with Image.open(image) as img:
 		width, height = img.size
 		# no need to resize if width or height is already less than the max
-		if width <= max or height <= max:
+		if width <= max_size or height <= max_size:
 			return image
 		if width > height:
-			width_ratio = max / float(width)
+			width_ratio = max_size / float(width)
 			new_height = int((float(height) * float(width_ratio)))
-			img = img.resize((max, new_height), Image.ANTIALIAS)
+			img = img.resize((max_size, new_height), Image.Resampling.LANCZOS)
 		else:
-			height_ratio = max / float(height)
+			height_ratio = max_size / float(height)
 			new_width = int((float(width) * float(height_ratio)))
-			img = img.resize((new_width, max), Image.ANTIALIAS)
+			img = img.resize((new_width, max_size), Image.Resampling.LANCZOS)
 		with BytesIO() as buffer:
 			img.save(fp=buffer, format="PNG", quality=quality)
 			resized_image = ContentFile(buffer.getvalue())
 	file_name_without_ext = os.path.splitext(image.name)[0]
 	return InMemoryUploadedFile(
 		resized_image, "ImageField", "%s.png" % file_name_without_ext, "image/png", resized_image.tell(), None
 	)
```

### Comparing `NEMO-4.6.0/NEMO/views/abuse.py` & `NEMO-4.6.1/NEMO/views/abuse.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/access_requests.py` & `NEMO-4.6.1/NEMO/views/access_requests.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/accounts_and_projects.py` & `NEMO-4.6.1/NEMO/views/accounts_and_projects.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/adjustment_requests.py` & `NEMO-4.6.1/NEMO/views/adjustment_requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from datetime import timedelta
-from typing import List
+from typing import List, Set
 
 from django.contrib.auth.decorators import login_required
 from django.contrib.contenttypes.models import ContentType
-from django.db.models import Q
+from django.db.models import Q, QuerySet
 from django.http import HttpResponse, HttpResponseBadRequest
 from django.shortcuts import get_object_or_404, redirect, render
 from django.template.defaultfilters import linebreaksbr
 from django.urls import reverse
 from django.utils import timezone
-from django.views.decorators.http import require_GET, require_POST, require_http_methods
+from django.views.decorators.http import require_GET, require_http_methods, require_POST
 
 from NEMO.decorators import accounting_or_user_office_or_manager_required
 from NEMO.forms import AdjustmentRequestForm
 from NEMO.mixins import BillableItemMixin
 from NEMO.models import (
     AdjustmentRequest,
     AreaAccessRecord,
@@ -23,27 +23,23 @@
     Reservation,
     StaffCharge,
     UsageEvent,
     User,
 )
 from NEMO.utilities import (
     BasicDisplayTable,
-    EmailCategory,
     bootstrap_primary_color,
+    EmailCategory,
     export_format_datetime,
     get_full_url,
     quiet_int,
     render_email_template,
     send_mail,
 )
-from NEMO.views.customization import (
-    EmailsCustomization,
-    UserRequestsCustomization,
-    get_media_file_contents,
-)
+from NEMO.views.customization import (EmailsCustomization, get_media_file_contents, UserRequestsCustomization)
 from NEMO.views.notifications import (
     create_adjustment_request_notification,
     create_request_message_notification,
     delete_notification,
     get_notifications,
 )
 
@@ -146,22 +142,35 @@
                         adjustment_request.status = RequestStatus.APPROVED
                     else:
                         adjustment_request.status = RequestStatus.DENIED
                     adjustment_request.reviewer = user
 
             form.instance.last_updated_by = user
             new_adjustment_request = form.save()
-            create_adjustment_request_notification(new_adjustment_request)
+
+            # Create the list of facility managers to notify. If the adjustment request has a tool and no one added that
+            # tool to their adjustment request list, send to everyone (otherwise nobody would see it)
+            managers_to_notify: Set[User] = set()
+            tool = getattr(adjustment_request.item, "tool", None) if adjustment_request.item else None
+            reviewers: QuerySet = User.objects.filter(is_active=True, is_facility_manager=True)
+            if tool:
+                reviewers_filter = reviewers.filter(Q(preferences__tool_adjustment_notifications__isnull=True) | Q(preferences__tool_adjustment_notifications__in=[tool]))
+                if reviewers_filter.exists():
+                    # Only limit managers if at least one person will receive the notification.
+                    reviewers = reviewers_filter
+            managers_to_notify.update(list(reviewers))
+
+            create_adjustment_request_notification(new_adjustment_request, managers_to_notify)
             if edit:
                 # remove notification for current user and other facility managers
                 delete_notification(Notification.Types.ADJUSTMENT_REQUEST, adjustment_request.id, [user])
                 if user.is_facility_manager:
                     managers = User.objects.filter(is_active=True, is_facility_manager=True)
                     delete_notification(Notification.Types.ADJUSTMENT_REQUEST, adjustment_request.id, managers)
-            send_request_received_email(request, new_adjustment_request, edit)
+            send_request_received_email(request, new_adjustment_request, edit, managers_to_notify)
             return redirect("user_requests", "adjustment")
         else:
             item_type = form.cleaned_data.get("item_type")
             item_id = form.cleaned_data.get("item_id")
             if item_type and item_id:
                 dictionary["change_times_allowed"] = can_change_times(item_type.get_object_for_this_type(pk=item_id))
             dictionary["form"] = form
@@ -215,24 +224,19 @@
 
     adjustment_request.deleted = True
     adjustment_request.save(update_fields=["deleted"])
     delete_notification(Notification.Types.ADJUSTMENT_REQUEST, adjustment_request.id)
     return redirect("user_requests", "adjustment")
 
 
-def send_request_received_email(request, adjustment_request: AdjustmentRequest, edit):
+def send_request_received_email(request, adjustment_request: AdjustmentRequest, edit, facility_managers: Set[User]):
     user_office_email = EmailsCustomization.get("user_office_email_address")
     adjustment_request_notification_email = get_media_file_contents("adjustment_request_notification_email.html")
     if user_office_email and adjustment_request_notification_email:
         # cc facility managers
-        tool = getattr(adjustment_request.item, "tool", None) if adjustment_request.item else None
-        facility_managers_qs = User.objects.filter(is_active=True, is_facility_manager=True)
-        if tool:
-            facility_managers_qs = facility_managers_qs.filter(Q(preferences__tool_adjustment_notifications__isnull=True)|Q(preferences__tool_adjustment_notifications__in=[tool]))
-        facility_managers: List[User] = list(facility_managers_qs)
         manager_emails = [
             email
             for user in facility_managers
             for email in user.get_emails(user.get_preferences().email_send_adjustment_request_updates)
         ]
         status = (
             "approved"
```

### Comparing `NEMO-4.6.0/NEMO/views/alerts.py` & `NEMO-4.6.1/NEMO/views/alerts.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/api.py` & `NEMO-4.6.1/NEMO/views/api.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/api_billing.py` & `NEMO-4.6.1/NEMO/views/api_billing.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/api_file_import.py` & `NEMO-4.6.1/NEMO/views/api_file_import.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/area_access.py` & `NEMO-4.6.1/NEMO/views/area_access.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/authentication.py` & `NEMO-4.6.1/NEMO/views/authentication.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/buddy_requests.py` & `NEMO-4.6.1/NEMO/views/buddy_requests.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/calendar.py` & `NEMO-4.6.1/NEMO/views/calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 	ReservationItemType,
 	ReservationQuestions,
 	ScheduledOutage,
 	ScheduledOutageCategory,
 	StaffCharge,
 	Tool,
 	UsageEvent,
-	User, UserPreferences,
+	User,
+	UserPreferences,
 )
 from NEMO.policy import policy_class as policy
 from NEMO.utilities import (
 	EmailCategory,
 	RecurrenceFrequency,
 	as_timezone,
 	beginning_of_the_day,
@@ -887,15 +888,17 @@
 	projects_to_exclude = request.GET.getlist("projects_to_exclude[]")
 	return send_email_usage_reminders(projects_to_exclude, request)
 
 
 def send_email_usage_reminders(projects_to_exclude=None, request=None):
 	if projects_to_exclude is None:
 		projects_to_exclude = []
-	busy_users = AreaAccessRecord.objects.filter(end=None, staff_charge=None).exclude(project__id__in=projects_to_exclude)
+	busy_users = AreaAccessRecord.objects.none()
+	if ApplicationCustomization.get_bool("area_in_usage_reminders"):
+		busy_users = AreaAccessRecord.objects.filter(end=None, staff_charge=None).exclude(project__id__in=projects_to_exclude)
 	busy_tools = UsageEvent.objects.filter(end=None).exclude(project__id__in=projects_to_exclude)
 
 	# Make lists of all the things a user is logged in to.
 	# We don't want to send 3 separate emails if a user is logged into three things.
 	# Just send one email for all the things!
 	aggregate = {}
 	for access_record in busy_users:
```

### Comparing `NEMO-4.6.0/NEMO/views/charge_validation.py` & `NEMO-4.6.1/NEMO/views/charge_validation.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/configuration_agenda.py` & `NEMO-4.6.1/NEMO/views/configuration_agenda.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/consumables.py` & `NEMO-4.6.1/NEMO/views/consumables.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/customization.py` & `NEMO-4.6.1/NEMO/views/customization.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,15 @@
 		"site_title": "NEMO",
 		"self_log_in": "",
 		"self_log_out": "",
 		"calendar_login_logout": "",
 		"area_logout_already_logged_in": "",
 		"default_badge_reader_id": "",
 		"consumable_user_self_checkout": "",
+		"area_in_usage_reminders": "enabled",
 	}
 
 	def context(self) -> Dict:
 		context_dict = super().context()
 		context_dict["badge_readers"] = BadgeReader.objects.all()
 		return context_dict
```

### Comparing `NEMO-4.6.0/NEMO/views/documents.py` & `NEMO-4.6.1/NEMO/views/documents.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/email.py` & `NEMO-4.6.1/NEMO/views/email.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/event_details.py` & `NEMO-4.6.1/NEMO/views/event_details.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/feedback.py` & `NEMO-4.6.1/NEMO/views/feedback.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/get_projects.py` & `NEMO-4.6.1/NEMO/views/get_projects.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/history.py` & `NEMO-4.6.1/NEMO/views/history.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/jumbotron.py` & `NEMO-4.6.1/NEMO/views/jumbotron.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/landing.py` & `NEMO-4.6.1/NEMO/views/landing.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/maintenance.py` & `NEMO-4.6.1/NEMO/views/maintenance.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/mobile.py` & `NEMO-4.6.1/NEMO/views/mobile.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/news.py` & `NEMO-4.6.1/NEMO/views/news.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/notifications.py` & `NEMO-4.6.1/NEMO/views/notifications.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from datetime import datetime, timedelta
 from typing import List, Set
 
 from django.contrib.contenttypes.models import ContentType
-from django.db.models import Q
 from django.utils import timezone
 
 from NEMO.models import (
 	AdjustmentRequest,
 	BuddyRequest,
 	Notification,
 	RequestMessage,
@@ -114,21 +113,16 @@
 			notification_type=Notification.Types.TEMPORARY_ACCESS_REQUEST,
 			content_type=ContentType.objects.get_for_model(access_request),
 			object_id=access_request.id,
 			defaults={"expiration": expiration},
 		)
 
 
-def create_adjustment_request_notification(adjustment_request: AdjustmentRequest):
-	users_to_notify = {adjustment_request.creator}
-	tool = getattr(adjustment_request.item, "tool", None) if adjustment_request.item else None
-	reviewers = User.objects.filter(is_active=True, is_facility_manager=True)
-	if tool:
-		reviewers = reviewers.filter(Q(preferences__tool_adjustment_notifications__isnull=True) | Q(preferences__tool_adjustment_notifications__in=[tool]))
-	users_to_notify.update(reviewers)
+def create_adjustment_request_notification(adjustment_request: AdjustmentRequest, users_to_notify: Set[User]):
+	users_to_notify.add(adjustment_request.creator)
 	expiration = timezone.now() + timedelta(days=30)  # 30 days for adjustment requests to expire
 	for user in users_to_notify:
 		# Only update users other than the one who last updated it
 		if not adjustment_request.last_updated_by or adjustment_request.last_updated_by != user:
 			Notification.objects.get_or_create(
 				user=user,
 				notification_type=Notification.Types.ADJUSTMENT_REQUEST,
```

### Comparing `NEMO-4.6.0/NEMO/views/pagination.py` & `NEMO-4.6.1/NEMO/views/pagination.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/qualifications.py` & `NEMO-4.6.1/NEMO/views/qualifications.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/remote_work.py` & `NEMO-4.6.1/NEMO/views/remote_work.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/resources.py` & `NEMO-4.6.1/NEMO/views/resources.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/safety.py` & `NEMO-4.6.1/NEMO/views/safety.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/sidebar.py` & `NEMO-4.6.1/NEMO/views/sidebar.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/status_dashboard.py` & `NEMO-4.6.1/NEMO/views/status_dashboard.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/tasks.py` & `NEMO-4.6.1/NEMO/views/tasks.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/tool_control.py` & `NEMO-4.6.1/NEMO/views/tool_control.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/training.py` & `NEMO-4.6.1/NEMO/views/training.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/tutorials.py` & `NEMO-4.6.1/NEMO/views/tutorials.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/usage.py` & `NEMO-4.6.1/NEMO/views/usage.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/user_requests.py` & `NEMO-4.6.1/NEMO/views/user_requests.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/views/users.py` & `NEMO-4.6.1/NEMO/views/users.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/widgets/configuration_editor.py` & `NEMO-4.6.1/NEMO/widgets/configuration_editor.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/widgets/dynamic_form.py` & `NEMO-4.6.1/NEMO/widgets/dynamic_form.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO/widgets/item_tree.py` & `NEMO-4.6.1/NEMO/widgets/item_tree.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/NEMO.egg-info/PKG-INFO` & `NEMO-4.6.1/NEMO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NEMO
-Version: 4.6.0
+Version: 4.6.1
 Summary: NEMO is a laboratory logistics web application. Use it to schedule reservations, control tool access, track maintenance issues, and more.
 Home-page: https://github.com/usnistgov/NEMO
 Author: Center for Nanoscale Science and Technology
 Author-email: CNSTapplications@nist.gov
 License: Public domain
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `NEMO-4.6.0/NEMO.egg-info/SOURCES.txt` & `NEMO-4.6.1/NEMO.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -147,14 +147,15 @@
 NEMO/migrations/0041_version_4_2_1.py
 NEMO/migrations/0042_version_4_3_0.py
 NEMO/migrations/0043_version_4_3_2.py
 NEMO/migrations/0044_version_4_4_0.py
 NEMO/migrations/0045_version_4_5_0.py
 NEMO/migrations/0045_version_4_5_5.py
 NEMO/migrations/0046_version_4_6_0.py
+NEMO/migrations/0047_version_4_6_1.py
 NEMO/migrations/__init__.py
 NEMO/static/badge_reader.js
 NEMO/static/favicon.ico
 NEMO/static/jquery.js
 NEMO/static/jquery.min.js
 NEMO/static/jumbotron_watermark.bmp
 NEMO/static/mobile.js
```

### Comparing `NEMO-4.6.0/PKG-INFO` & `NEMO-4.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NEMO
-Version: 4.6.0
+Version: 4.6.1
 Summary: NEMO is a laboratory logistics web application. Use it to schedule reservations, control tool access, track maintenance issues, and more.
 Home-page: https://github.com/usnistgov/NEMO
 Author: Center for Nanoscale Science and Technology
 Author-email: CNSTapplications@nist.gov
 License: Public domain
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `NEMO-4.6.0/README.md` & `NEMO-4.6.1/README.md`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/resources/settings.py` & `NEMO-4.6.1/resources/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,32 +300,32 @@
 # AUTHENTICATION_BACKENDS = ["NEMO.views.authentication.RemoteUserAuthenticationBackend"]
 
 # Username regex validation. For example limit usernames to only alphanumerics and underscore
 # USERNAME_REGEX = "^[A-Za-z0-9_]+$"
 
 # Specify your list of LDAP authentication servers only if you choose to use LDAP authentication
 # Below is an example with a free ldap testing server. Usernames and passwords available at https://www.forumsys.com/tutorials/integration-how-to/ldap/online-ldap-test-server/
-LDAP_SERVERS = [
-    {
-        "url": "ldap.forumsys.com",
-        "port": 389,
-        "use_ssl": False,
-        "bind_as_authentication": False,
-        "base_dn": "dc=example,dc=com",
-    }
-]
+# LDAP_SERVERS = [
+#     {
+#         "url": "ldap.forumsys.com",
+#         "port": 389,
+#         "use_ssl": False,
+#         "bind_as_authentication": False,
+#         "base_dn": "dc=example,dc=com",
+#     }
+# ]
 
 # NEMO can integrate with a custom Identity Service to manage user accounts on
 # related computer systems, which streamlines user onboarding and offboarding.
 # You would need to build this service yourself.
-IDENTITY_SERVICE = {
-    "available": False,
-    "url": "myidentityservice.com",
-    "domains": [],
-}
+# IDENTITY_SERVICE = {
+#     "available": False,
+#     "url": "myidentityservice.com",
+#     "domains": [],
+# }
 
 # Audit log. Update this list based on your audit needs. See supported fields at https://django-auditlog.readthedocs.io/en/latest/usage.html#settings
 AUDITLOG_INCLUDE_TRACKING_MODELS = (
     # Track changes to user access expiration, roles and managed projects
     {
         "model": "NEMO.User",
         "include_fields": ["access_expiration", "is_staff", "is_service_personnel", "is_technician", "is_facility_manager", "is_superuser"],
```

### Comparing `NEMO-4.6.0/resources/splash_pad_settings.py` & `NEMO-4.6.1/resources/splash_pad_settings.py`

 * *Files identical despite different names*

### Comparing `NEMO-4.6.0/setup.py` & `NEMO-4.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 setup(
 	name='NEMO',
-	version='4.6.0',
+	version='4.6.1',
 	python_requires='>=3.8, <4',
 	packages=find_namespace_packages(exclude=['NEMO.tests', 'NEMO.tests.*']),
 	include_package_data=True,
 	url='https://github.com/usnistgov/NEMO',
 	license='Public domain',
 	author='Center for Nanoscale Science and Technology',
 	author_email='CNSTapplications@nist.gov',
```


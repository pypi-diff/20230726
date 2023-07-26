# Comparing `tmp/liquidctl-1.9.0.tar.gz` & `tmp/liquidctl-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liquidctl-1.9.0.tar", last modified: Tue Apr  5 06:15:36 2022, max compression
+gzip compressed data, was "liquidctl-1.9.1.tar", last modified: Wed Apr  6 01:48:42 2022, max compression
```

## Comparing `liquidctl-1.9.0.tar` & `liquidctl-1.9.1.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.524751 liquidctl-1.9.0/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       85 2022-03-12 06:43:09.000000 liquidctl-1.9.0/.gitignore
--rw-r--r--   0 jonas     (1000) jonas     (1000)    30181 2022-04-05 05:50:29.000000 liquidctl-1.9.0/CHANGELOG.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3357 2022-01-23 16:42:00.000000 liquidctl-1.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1877 2021-06-17 19:45:37.000000 liquidctl-1.9.0/CONTRIBUTING.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2095 2022-03-23 10:55:17.000000 liquidctl-1.9.0/FUNDING.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)    35149 2018-08-26 10:31:19.000000 liquidctl-1.9.0/LICENSE.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)       28 2022-03-03 13:43:31.000000 liquidctl-1.9.0/MANIFEST.in
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3005 2022-04-05 06:15:36.524751 liquidctl-1.9.0/PKG-INFO
--rw-r--r--   0 jonas     (1000) jonas     (1000)    33918 2022-04-05 05:50:29.000000 liquidctl-1.9.0/README.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)      818 2022-03-03 13:43:31.000000 liquidctl-1.9.0/SECURITY.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)      301 2022-02-16 13:17:57.000000 liquidctl-1.9.0/conftest.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.518085 liquidctl-1.9.0/docs/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2253 2022-03-03 13:43:31.000000 liquidctl-1.9.0/docs/README.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4035 2022-03-03 13:43:31.000000 liquidctl-1.9.0/docs/asetek-690lc-guide.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2384 2022-01-06 05:18:20.000000 liquidctl-1.9.0/docs/asetek-pro-guide.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2478 2022-03-03 13:43:31.000000 liquidctl-1.9.0/docs/corsair-commander-core-guide.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6990 2022-03-03 13:43:31.000000 liquidctl-1.9.0/docs/corsair-commander-guide.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4664 2022-03-03 13:43:31.000000 liquidctl-1.9.0/docs/corsair-hxi-rmi-psu-guide.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4290 2022-01-06 05:18:35.000000 liquidctl-1.9.0/docs/corsair-platinum-pro-xt-guide.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4854 2021-07-04 04:50:04.000000 liquidctl-1.9.0/docs/ddr4-guide.md
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.518085 liquidctl-1.9.0/docs/developer/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5665 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/capturing-usb-traffic.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6884 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/creating-vm-for-capture.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3367 2022-03-03 13:43:31.000000 liquidctl-1.9.0/docs/developer/hwmon.md
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.521418 liquidctl-1.9.0/docs/developer/images/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1370 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/images/create_vm.png
--rw-r--r--   0 jonas     (1000) jonas     (1000)    42464 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/images/create_vm_1.png
--rw-r--r--   0 jonas     (1000) jonas     (1000)    91208 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/images/create_vm_10.png
--rw-r--r--   0 jonas     (1000) jonas     (1000)    17994 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/images/create_vm_2.png
--rw-r--r--   0 jonas     (1000) jonas     (1000)    37688 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/images/create_vm_3.png
--rw-r--r--   0 jonas     (1000) jonas     (1000)    40306 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/images/create_vm_4.png
--rw-r--r--   0 jonas     (1000) jonas     (1000)    32348 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/images/create_vm_5.png
--rw-r--r--   0 jonas     (1000) jonas     (1000)    36519 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/images/create_vm_6.png
--rw-r--r--   0 jonas     (1000) jonas     (1000)    45373 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/images/create_vm_7.png
--rw-r--r--   0 jonas     (1000) jonas     (1000)   102648 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/images/create_vm_8.png
--rw-r--r--   0 jonas     (1000) jonas     (1000)    90381 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/images/create_vm_9.png
--rw-r--r--   0 jonas     (1000) jonas     (1000)   377287 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/images/icue.png
--rw-r--r--   0 jonas     (1000) jonas     (1000)   154210 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/images/vendor_product_id.png
--rw-r--r--   0 jonas     (1000) jonas     (1000)    83927 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/images/wireshark_1.png
--rw-r--r--   0 jonas     (1000) jonas     (1000)    83644 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/images/wireshark_2.png
--rw-r--r--   0 jonas     (1000) jonas     (1000)   284166 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/images/wireshark_3.png
--rw-r--r--   0 jonas     (1000) jonas     (1000)   132844 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/images/wireshark_4.png
--rw-r--r--   0 jonas     (1000) jonas     (1000)     9121 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/porting-drivers-from-opencorsairlink.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4339 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/process.md
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.521418 liquidctl-1.9.0/docs/developer/protocol/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6122 2022-01-21 15:06:29.000000 liquidctl-1.9.0/docs/developer/protocol/commander_core.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5062 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/protocol/lighting_node_rgb.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3523 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/protocol/vengeance_rgb.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2363 2022-04-05 06:15:00.000000 liquidctl-1.9.0/docs/developer/release-checklist.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7228 2022-02-23 08:49:07.000000 liquidctl-1.9.0/docs/developer/style-guide.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12258 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/developer/techniques-for-analyzing-usb-protocols.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4399 2022-03-03 13:43:31.000000 liquidctl-1.9.0/docs/gigabyte-rgb-fusion2-guide.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7322 2022-03-03 13:43:31.000000 liquidctl-1.9.0/docs/kraken-x2-m2-guide.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8069 2022-03-03 13:43:31.000000 liquidctl-1.9.0/docs/kraken-x3-z3-guide.md
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.521418 liquidctl-1.9.0/docs/linux/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3106 2021-06-17 19:45:37.000000 liquidctl-1.9.0/docs/linux/making-systemd-units-wait-for-devices.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8649 2022-03-03 13:43:31.000000 liquidctl-1.9.0/docs/nvidia-guide.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1683 2021-07-04 04:50:32.000000 liquidctl-1.9.0/docs/nzxt-e-series-psu-guide.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6751 2022-03-03 13:43:31.000000 liquidctl-1.9.0/docs/nzxt-hue2-guide.md
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6074 2022-03-03 13:43:31.000000 liquidctl-1.9.0/docs/nzxt-smart-device-v1-guide.md
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.521418 liquidctl-1.9.0/docs/windows/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3469 2022-03-03 13:43:31.000000 liquidctl-1.9.0/docs/windows/running-your-first-command-line-program.md
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.521418 liquidctl-1.9.0/extra/
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.521418 liquidctl-1.9.0/extra/completions/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8138 2022-03-03 13:43:31.000000 liquidctl-1.9.0/extra/completions/liquidctl.bash
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.521418 liquidctl-1.9.0/extra/contrib/
--rwxr-xr-x   0 jonas     (1000) jonas     (1000)     2743 2022-03-03 13:43:31.000000 liquidctl-1.9.0/extra/contrib/fusion_rgb_cycle.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.521418 liquidctl-1.9.0/extra/contrib/liquidctlfan/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3854 2021-06-17 19:45:37.000000 liquidctl-1.9.0/extra/contrib/liquidctlfan/README.md
--rwxr-xr-x   0 jonas     (1000) jonas     (1000)     8431 2021-06-17 19:45:37.000000 liquidctl-1.9.0/extra/contrib/liquidctlfan/liquidctlfan
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.521418 liquidctl-1.9.0/extra/contrib/liquidctlfan/systemd/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      364 2021-06-17 19:45:37.000000 liquidctl-1.9.0/extra/contrib/liquidctlfan/systemd/liquidctlfan.service
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.521418 liquidctl-1.9.0/extra/dist/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1660 2022-03-12 06:42:39.000000 liquidctl-1.9.0/extra/dist/pypi-readme.md
--rwxr-xr-x   0 jonas     (1000) jonas     (1000)     3636 2022-04-05 05:47:47.000000 liquidctl-1.9.0/extra/krakenduty-poc
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.521418 liquidctl-1.9.0/extra/linux/
--rw-r--r--   0 jonas     (1000) jonas     (1000)    20881 2022-04-05 05:28:11.000000 liquidctl-1.9.0/extra/linux/71-liquidctl.rules
--rwxr-xr-x   0 jonas     (1000) jonas     (1000)     5171 2022-04-04 02:58:32.000000 liquidctl-1.9.0/extra/linux/generate-uaccess-udev-rules.py
--rwxr-xr-x   0 jonas     (1000) jonas     (1000)     3132 2022-02-04 23:26:15.000000 liquidctl-1.9.0/extra/liquiddump
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.521418 liquidctl-1.9.0/extra/old-tests/
--rwxr-xr-x   0 jonas     (1000) jonas     (1000)     1836 2021-06-17 19:45:37.000000 liquidctl-1.9.0/extra/old-tests/asetek_legacy
--rwxr-xr-x   0 jonas     (1000) jonas     (1000)     1830 2021-06-17 19:45:37.000000 liquidctl-1.9.0/extra/old-tests/asetek_modern
--rwxr-xr-x   0 jonas     (1000) jonas     (1000)      556 2021-06-17 19:45:37.000000 liquidctl-1.9.0/extra/old-tests/asetek_modern_rainbow
--rwxr-xr-x   0 jonas     (1000) jonas     (1000)     3173 2021-06-17 19:45:37.000000 liquidctl-1.9.0/extra/old-tests/kraken_two
--rwxr-xr-x   0 jonas     (1000) jonas     (1000)     4957 2022-02-04 23:26:15.000000 liquidctl-1.9.0/extra/prometheus-liquidctl-exporter
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.521418 liquidctl-1.9.0/extra/windows/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4807 2022-02-04 23:26:15.000000 liquidctl-1.9.0/extra/windows/LQiNFO.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    29956 2021-06-17 19:45:37.000000 liquidctl-1.9.0/extra/windows/liquidctl_logo_v1_circle_256.ico
--rw-r--r--   0 jonas     (1000) jonas     (1000)    13508 2022-01-21 15:06:29.000000 liquidctl-1.9.0/extra/windows/redist-notices.txt
--rwxr-xr-x   0 jonas     (1000) jonas     (1000)    10051 2022-02-04 23:26:15.000000 liquidctl-1.9.0/extra/yoda
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.521418 liquidctl-1.9.0/liquidctl/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      152 2022-03-03 13:43:31.000000 liquidctl-1.9.0/liquidctl/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      119 2022-03-03 13:43:31.000000 liquidctl-1.9.0/liquidctl/__main__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      142 2022-04-05 06:15:35.000000 liquidctl-1.9.0/liquidctl/_version.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    18587 2022-03-05 05:42:41.000000 liquidctl-1.9.0/liquidctl/cli.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.524751 liquidctl-1.9.0/liquidctl/driver/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2638 2022-02-04 23:26:15.000000 liquidctl-1.9.0/liquidctl/driver/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    18955 2022-03-05 08:03:51.000000 liquidctl-1.9.0/liquidctl/driver/asetek.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8430 2022-03-04 12:58:11.000000 liquidctl-1.9.0/liquidctl/driver/asetek_pro.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5051 2022-03-03 13:43:31.000000 liquidctl-1.9.0/liquidctl/driver/base.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8140 2022-02-04 23:26:15.000000 liquidctl-1.9.0/liquidctl/driver/commander_core.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    21651 2022-03-03 13:43:31.000000 liquidctl-1.9.0/liquidctl/driver/commander_pro.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12248 2022-03-03 13:43:31.000000 liquidctl-1.9.0/liquidctl/driver/corsair_hid_psu.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12856 2022-03-05 05:53:51.000000 liquidctl-1.9.0/liquidctl/driver/ddr4.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1644 2022-03-03 13:43:31.000000 liquidctl-1.9.0/liquidctl/driver/hwmon.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    17121 2022-03-12 20:31:09.000000 liquidctl-1.9.0/liquidctl/driver/hydro_platinum.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12537 2022-04-05 05:50:29.000000 liquidctl-1.9.0/liquidctl/driver/kraken2.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    18269 2022-03-03 13:43:31.000000 liquidctl-1.9.0/liquidctl/driver/kraken3.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    21851 2022-03-05 05:53:51.000000 liquidctl-1.9.0/liquidctl/driver/nvidia.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5193 2022-02-04 23:26:15.000000 liquidctl-1.9.0/liquidctl/driver/nzxt_epsu.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10259 2022-02-04 23:26:15.000000 liquidctl-1.9.0/liquidctl/driver/rgb_fusion2.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    27308 2022-03-05 08:03:54.000000 liquidctl-1.9.0/liquidctl/driver/smart_device.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12267 2022-03-05 06:33:20.000000 liquidctl-1.9.0/liquidctl/driver/smbus.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    21611 2022-03-08 08:15:52.000000 liquidctl-1.9.0/liquidctl/driver/usb.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      378 2022-02-18 04:38:26.000000 liquidctl-1.9.0/liquidctl/error.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7171 2022-02-04 08:10:54.000000 liquidctl-1.9.0/liquidctl/keyval.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5989 2022-02-27 09:34:34.000000 liquidctl-1.9.0/liquidctl/pmbus.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12479 2022-02-04 08:10:54.000000 liquidctl-1.9.0/liquidctl/util.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1574 2022-03-17 14:48:53.000000 liquidctl-1.9.0/liquidctl/version.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    16073 2022-04-05 05:50:29.000000 liquidctl-1.9.0/liquidctl.8
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.521418 liquidctl-1.9.0/liquidctl.egg-info/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3005 2022-04-05 06:15:36.000000 liquidctl-1.9.0/liquidctl.egg-info/PKG-INFO
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4109 2022-04-05 06:15:36.000000 liquidctl-1.9.0/liquidctl.egg-info/SOURCES.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2022-04-05 06:15:36.000000 liquidctl-1.9.0/liquidctl.egg-info/dependency_links.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)       49 2022-04-05 06:15:36.000000 liquidctl-1.9.0/liquidctl.egg-info/entry_points.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)      134 2022-04-05 06:15:36.000000 liquidctl-1.9.0/liquidctl.egg-info/requires.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)       10 2022-04-05 06:15:36.000000 liquidctl-1.9.0/liquidctl.egg-info/top_level.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2683 2022-03-17 14:48:53.000000 liquidctl-1.9.0/pyproject.toml
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1561 2022-04-05 06:15:36.524751 liquidctl-1.9.0/setup.cfg
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-05 06:15:36.524751 liquidctl-1.9.0/tests/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8304 2022-03-03 13:43:31.000000 liquidctl-1.9.0/tests/_testutils.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2659 2022-02-04 08:10:54.000000 liquidctl-1.9.0/tests/test_api.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5761 2022-02-04 08:10:54.000000 liquidctl-1.9.0/tests/test_asetek.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3531 2022-03-04 12:55:23.000000 liquidctl-1.9.0/tests/test_asetek_pro.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      718 2022-02-23 08:49:07.000000 liquidctl-1.9.0/tests/test_backward_compatibility_10.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1610 2022-03-03 13:43:31.000000 liquidctl-1.9.0/tests/test_backward_compatibility_11.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      181 2021-12-10 23:17:20.000000 liquidctl-1.9.0/tests/test_backward_compatibility_12.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      845 2021-12-10 23:17:20.000000 liquidctl-1.9.0/tests/test_backward_compatibility_13.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5080 2022-02-04 08:10:54.000000 liquidctl-1.9.0/tests/test_backward_compatibility_14.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1830 2022-02-04 08:10:54.000000 liquidctl-1.9.0/tests/test_backward_compatibility_15.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      352 2022-03-04 12:58:00.000000 liquidctl-1.9.0/tests/test_backward_compatibility_18.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2329 2022-02-04 08:10:54.000000 liquidctl-1.9.0/tests/test_cli.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10784 2022-03-03 13:43:31.000000 liquidctl-1.9.0/tests/test_commander_core.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    43880 2022-03-03 13:43:31.000000 liquidctl-1.9.0/tests/test_commander_pro.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6596 2022-03-03 13:43:31.000000 liquidctl-1.9.0/tests/test_corsair_hid_psu.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12771 2022-02-04 08:10:54.000000 liquidctl-1.9.0/tests/test_ddr4.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4481 2022-02-04 08:10:54.000000 liquidctl-1.9.0/tests/test_hidapi_device.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      950 2022-03-03 13:43:31.000000 liquidctl-1.9.0/tests/test_hwmon.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    14254 2022-02-04 08:10:54.000000 liquidctl-1.9.0/tests/test_hydro_platinum.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7804 2022-02-23 08:49:07.000000 liquidctl-1.9.0/tests/test_keyval.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5411 2022-04-05 05:53:18.000000 liquidctl-1.9.0/tests/test_kraken2.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5165 2022-03-03 13:43:31.000000 liquidctl-1.9.0/tests/test_kraken3.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    14889 2022-03-03 13:43:31.000000 liquidctl-1.9.0/tests/test_nvidia.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1097 2022-02-04 08:10:54.000000 liquidctl-1.9.0/tests/test_nzxt_epsu.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8045 2022-02-04 08:10:54.000000 liquidctl-1.9.0/tests/test_rgb_fusion2.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4651 2022-03-03 13:43:31.000000 liquidctl-1.9.0/tests/test_smart_device.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4627 2022-03-03 13:43:31.000000 liquidctl-1.9.0/tests/test_smart_device2.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4401 2022-02-04 08:10:54.000000 liquidctl-1.9.0/tests/test_smbus.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1429 2022-02-04 08:10:54.000000 liquidctl-1.9.0/tests/test_usb.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      215 2022-03-03 13:43:31.000000 liquidctl-1.9.0/tox.ini
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.135363 liquidctl-1.9.1/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       85 2022-03-12 06:43:09.000000 liquidctl-1.9.1/.gitignore
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    30862 2022-04-06 01:47:31.000000 liquidctl-1.9.1/CHANGELOG.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3357 2022-01-23 16:42:00.000000 liquidctl-1.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1877 2021-06-17 19:45:37.000000 liquidctl-1.9.1/CONTRIBUTING.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2095 2022-03-23 10:55:17.000000 liquidctl-1.9.1/FUNDING.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    35149 2018-08-26 10:31:19.000000 liquidctl-1.9.1/LICENSE.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       28 2022-03-03 13:43:31.000000 liquidctl-1.9.1/MANIFEST.in
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3005 2022-04-06 01:48:42.135363 liquidctl-1.9.1/PKG-INFO
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    33918 2022-04-06 01:39:08.000000 liquidctl-1.9.1/README.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      818 2022-03-03 13:43:31.000000 liquidctl-1.9.1/SECURITY.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      301 2022-02-16 13:17:57.000000 liquidctl-1.9.1/conftest.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.125363 liquidctl-1.9.1/docs/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2253 2022-03-03 13:43:31.000000 liquidctl-1.9.1/docs/README.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4035 2022-03-03 13:43:31.000000 liquidctl-1.9.1/docs/asetek-690lc-guide.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2384 2022-01-06 05:18:20.000000 liquidctl-1.9.1/docs/asetek-pro-guide.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2478 2022-03-03 13:43:31.000000 liquidctl-1.9.1/docs/corsair-commander-core-guide.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6990 2022-03-03 13:43:31.000000 liquidctl-1.9.1/docs/corsair-commander-guide.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4664 2022-03-03 13:43:31.000000 liquidctl-1.9.1/docs/corsair-hxi-rmi-psu-guide.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4290 2022-01-06 05:18:35.000000 liquidctl-1.9.1/docs/corsair-platinum-pro-xt-guide.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4854 2021-07-04 04:50:04.000000 liquidctl-1.9.1/docs/ddr4-guide.md
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.125363 liquidctl-1.9.1/docs/developer/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5665 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/capturing-usb-traffic.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6884 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/creating-vm-for-capture.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3367 2022-03-03 13:43:31.000000 liquidctl-1.9.1/docs/developer/hwmon.md
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.128697 liquidctl-1.9.1/docs/developer/images/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1370 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/images/create_vm.png
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    42464 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/images/create_vm_1.png
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    91208 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/images/create_vm_10.png
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    17994 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/images/create_vm_2.png
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    37688 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/images/create_vm_3.png
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    40306 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/images/create_vm_4.png
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    32348 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/images/create_vm_5.png
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    36519 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/images/create_vm_6.png
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    45373 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/images/create_vm_7.png
+-rw-r--r--   0 jonas     (1000) jonas     (1000)   102648 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/images/create_vm_8.png
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    90381 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/images/create_vm_9.png
+-rw-r--r--   0 jonas     (1000) jonas     (1000)   377287 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/images/icue.png
+-rw-r--r--   0 jonas     (1000) jonas     (1000)   154210 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/images/vendor_product_id.png
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    83927 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/images/wireshark_1.png
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    83644 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/images/wireshark_2.png
+-rw-r--r--   0 jonas     (1000) jonas     (1000)   284166 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/images/wireshark_3.png
+-rw-r--r--   0 jonas     (1000) jonas     (1000)   132844 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/images/wireshark_4.png
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     9121 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/porting-drivers-from-opencorsairlink.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4339 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/process.md
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.128697 liquidctl-1.9.1/docs/developer/protocol/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6122 2022-01-21 15:06:29.000000 liquidctl-1.9.1/docs/developer/protocol/commander_core.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5062 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/protocol/lighting_node_rgb.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3523 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/protocol/vengeance_rgb.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2567 2022-04-05 06:20:45.000000 liquidctl-1.9.1/docs/developer/release-checklist.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7228 2022-02-23 08:49:07.000000 liquidctl-1.9.1/docs/developer/style-guide.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12258 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/developer/techniques-for-analyzing-usb-protocols.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4399 2022-03-03 13:43:31.000000 liquidctl-1.9.1/docs/gigabyte-rgb-fusion2-guide.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7322 2022-03-03 13:43:31.000000 liquidctl-1.9.1/docs/kraken-x2-m2-guide.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8069 2022-03-03 13:43:31.000000 liquidctl-1.9.1/docs/kraken-x3-z3-guide.md
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.128697 liquidctl-1.9.1/docs/linux/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3106 2021-06-17 19:45:37.000000 liquidctl-1.9.1/docs/linux/making-systemd-units-wait-for-devices.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8649 2022-03-03 13:43:31.000000 liquidctl-1.9.1/docs/nvidia-guide.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1683 2021-07-04 04:50:32.000000 liquidctl-1.9.1/docs/nzxt-e-series-psu-guide.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6751 2022-03-03 13:43:31.000000 liquidctl-1.9.1/docs/nzxt-hue2-guide.md
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6074 2022-03-03 13:43:31.000000 liquidctl-1.9.1/docs/nzxt-smart-device-v1-guide.md
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.128697 liquidctl-1.9.1/docs/windows/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3469 2022-03-03 13:43:31.000000 liquidctl-1.9.1/docs/windows/running-your-first-command-line-program.md
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.128697 liquidctl-1.9.1/extra/
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.128697 liquidctl-1.9.1/extra/completions/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8138 2022-03-03 13:43:31.000000 liquidctl-1.9.1/extra/completions/liquidctl.bash
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.128697 liquidctl-1.9.1/extra/contrib/
+-rwxr-xr-x   0 jonas     (1000) jonas     (1000)     2743 2022-03-03 13:43:31.000000 liquidctl-1.9.1/extra/contrib/fusion_rgb_cycle.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.128697 liquidctl-1.9.1/extra/contrib/liquidctlfan/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3854 2021-06-17 19:45:37.000000 liquidctl-1.9.1/extra/contrib/liquidctlfan/README.md
+-rwxr-xr-x   0 jonas     (1000) jonas     (1000)     8431 2021-06-17 19:45:37.000000 liquidctl-1.9.1/extra/contrib/liquidctlfan/liquidctlfan
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.128697 liquidctl-1.9.1/extra/contrib/liquidctlfan/systemd/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      364 2021-06-17 19:45:37.000000 liquidctl-1.9.1/extra/contrib/liquidctlfan/systemd/liquidctlfan.service
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.128697 liquidctl-1.9.1/extra/dist/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1660 2022-03-12 06:42:39.000000 liquidctl-1.9.1/extra/dist/pypi-readme.md
+-rwxr-xr-x   0 jonas     (1000) jonas     (1000)     3636 2022-04-05 05:47:47.000000 liquidctl-1.9.1/extra/krakenduty-poc
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.128697 liquidctl-1.9.1/extra/linux/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    20881 2022-04-05 05:28:11.000000 liquidctl-1.9.1/extra/linux/71-liquidctl.rules
+-rwxr-xr-x   0 jonas     (1000) jonas     (1000)     5171 2022-04-04 02:58:32.000000 liquidctl-1.9.1/extra/linux/generate-uaccess-udev-rules.py
+-rwxr-xr-x   0 jonas     (1000) jonas     (1000)     3132 2022-02-04 23:26:15.000000 liquidctl-1.9.1/extra/liquiddump
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.128697 liquidctl-1.9.1/extra/old-tests/
+-rwxr-xr-x   0 jonas     (1000) jonas     (1000)     1836 2021-06-17 19:45:37.000000 liquidctl-1.9.1/extra/old-tests/asetek_legacy
+-rwxr-xr-x   0 jonas     (1000) jonas     (1000)     1830 2021-06-17 19:45:37.000000 liquidctl-1.9.1/extra/old-tests/asetek_modern
+-rwxr-xr-x   0 jonas     (1000) jonas     (1000)      556 2021-06-17 19:45:37.000000 liquidctl-1.9.1/extra/old-tests/asetek_modern_rainbow
+-rwxr-xr-x   0 jonas     (1000) jonas     (1000)     3173 2021-06-17 19:45:37.000000 liquidctl-1.9.1/extra/old-tests/kraken_two
+-rwxr-xr-x   0 jonas     (1000) jonas     (1000)     4957 2022-02-04 23:26:15.000000 liquidctl-1.9.1/extra/prometheus-liquidctl-exporter
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.128697 liquidctl-1.9.1/extra/windows/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4807 2022-02-04 23:26:15.000000 liquidctl-1.9.1/extra/windows/LQiNFO.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    29956 2021-06-17 19:45:37.000000 liquidctl-1.9.1/extra/windows/liquidctl_logo_v1_circle_256.ico
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    13508 2022-01-21 15:06:29.000000 liquidctl-1.9.1/extra/windows/redist-notices.txt
+-rwxr-xr-x   0 jonas     (1000) jonas     (1000)    10051 2022-02-04 23:26:15.000000 liquidctl-1.9.1/extra/yoda
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.128697 liquidctl-1.9.1/liquidctl/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      152 2022-03-03 13:43:31.000000 liquidctl-1.9.1/liquidctl/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      119 2022-03-03 13:43:31.000000 liquidctl-1.9.1/liquidctl/__main__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      142 2022-04-06 01:48:41.000000 liquidctl-1.9.1/liquidctl/_version.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    18587 2022-03-05 05:42:41.000000 liquidctl-1.9.1/liquidctl/cli.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.132030 liquidctl-1.9.1/liquidctl/driver/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2638 2022-02-04 23:26:15.000000 liquidctl-1.9.1/liquidctl/driver/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    18955 2022-03-05 08:03:51.000000 liquidctl-1.9.1/liquidctl/driver/asetek.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8430 2022-03-04 12:58:11.000000 liquidctl-1.9.1/liquidctl/driver/asetek_pro.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5051 2022-03-03 13:43:31.000000 liquidctl-1.9.1/liquidctl/driver/base.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8140 2022-02-04 23:26:15.000000 liquidctl-1.9.1/liquidctl/driver/commander_core.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    21651 2022-03-03 13:43:31.000000 liquidctl-1.9.1/liquidctl/driver/commander_pro.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12248 2022-03-03 13:43:31.000000 liquidctl-1.9.1/liquidctl/driver/corsair_hid_psu.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12856 2022-03-05 05:53:51.000000 liquidctl-1.9.1/liquidctl/driver/ddr4.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1644 2022-03-03 13:43:31.000000 liquidctl-1.9.1/liquidctl/driver/hwmon.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    17121 2022-03-12 20:31:09.000000 liquidctl-1.9.1/liquidctl/driver/hydro_platinum.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12537 2022-04-05 05:50:29.000000 liquidctl-1.9.1/liquidctl/driver/kraken2.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    18251 2022-04-05 19:46:47.000000 liquidctl-1.9.1/liquidctl/driver/kraken3.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    21851 2022-03-05 05:53:51.000000 liquidctl-1.9.1/liquidctl/driver/nvidia.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5193 2022-02-04 23:26:15.000000 liquidctl-1.9.1/liquidctl/driver/nzxt_epsu.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10259 2022-02-04 23:26:15.000000 liquidctl-1.9.1/liquidctl/driver/rgb_fusion2.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    27302 2022-04-05 19:46:47.000000 liquidctl-1.9.1/liquidctl/driver/smart_device.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12267 2022-03-05 06:33:20.000000 liquidctl-1.9.1/liquidctl/driver/smbus.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    21611 2022-03-08 08:15:52.000000 liquidctl-1.9.1/liquidctl/driver/usb.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      378 2022-02-18 04:38:26.000000 liquidctl-1.9.1/liquidctl/error.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7171 2022-02-04 08:10:54.000000 liquidctl-1.9.1/liquidctl/keyval.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5989 2022-02-27 09:34:34.000000 liquidctl-1.9.1/liquidctl/pmbus.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12479 2022-02-04 08:10:54.000000 liquidctl-1.9.1/liquidctl/util.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1574 2022-03-17 14:48:53.000000 liquidctl-1.9.1/liquidctl/version.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    16073 2022-04-05 05:50:29.000000 liquidctl-1.9.1/liquidctl.8
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.132030 liquidctl-1.9.1/liquidctl.egg-info/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3005 2022-04-06 01:48:41.000000 liquidctl-1.9.1/liquidctl.egg-info/PKG-INFO
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4109 2022-04-06 01:48:42.000000 liquidctl-1.9.1/liquidctl.egg-info/SOURCES.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2022-04-06 01:48:41.000000 liquidctl-1.9.1/liquidctl.egg-info/dependency_links.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       49 2022-04-06 01:48:41.000000 liquidctl-1.9.1/liquidctl.egg-info/entry_points.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      134 2022-04-06 01:48:42.000000 liquidctl-1.9.1/liquidctl.egg-info/requires.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       10 2022-04-06 01:48:42.000000 liquidctl-1.9.1/liquidctl.egg-info/top_level.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2683 2022-03-17 14:48:53.000000 liquidctl-1.9.1/pyproject.toml
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1561 2022-04-06 01:48:42.135363 liquidctl-1.9.1/setup.cfg
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2022-04-06 01:48:42.135363 liquidctl-1.9.1/tests/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8304 2022-03-03 13:43:31.000000 liquidctl-1.9.1/tests/_testutils.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2659 2022-02-04 08:10:54.000000 liquidctl-1.9.1/tests/test_api.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5761 2022-02-04 08:10:54.000000 liquidctl-1.9.1/tests/test_asetek.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3531 2022-03-04 12:55:23.000000 liquidctl-1.9.1/tests/test_asetek_pro.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      718 2022-02-23 08:49:07.000000 liquidctl-1.9.1/tests/test_backward_compatibility_10.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1610 2022-03-03 13:43:31.000000 liquidctl-1.9.1/tests/test_backward_compatibility_11.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      181 2021-12-10 23:17:20.000000 liquidctl-1.9.1/tests/test_backward_compatibility_12.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      845 2021-12-10 23:17:20.000000 liquidctl-1.9.1/tests/test_backward_compatibility_13.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5080 2022-02-04 08:10:54.000000 liquidctl-1.9.1/tests/test_backward_compatibility_14.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1830 2022-02-04 08:10:54.000000 liquidctl-1.9.1/tests/test_backward_compatibility_15.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      352 2022-03-04 12:58:00.000000 liquidctl-1.9.1/tests/test_backward_compatibility_18.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2329 2022-02-04 08:10:54.000000 liquidctl-1.9.1/tests/test_cli.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10784 2022-03-03 13:43:31.000000 liquidctl-1.9.1/tests/test_commander_core.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    43880 2022-03-03 13:43:31.000000 liquidctl-1.9.1/tests/test_commander_pro.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6596 2022-03-03 13:43:31.000000 liquidctl-1.9.1/tests/test_corsair_hid_psu.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12771 2022-02-04 08:10:54.000000 liquidctl-1.9.1/tests/test_ddr4.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4481 2022-02-04 08:10:54.000000 liquidctl-1.9.1/tests/test_hidapi_device.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      950 2022-03-03 13:43:31.000000 liquidctl-1.9.1/tests/test_hwmon.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    14254 2022-02-04 08:10:54.000000 liquidctl-1.9.1/tests/test_hydro_platinum.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7804 2022-02-23 08:49:07.000000 liquidctl-1.9.1/tests/test_keyval.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5411 2022-04-05 05:53:18.000000 liquidctl-1.9.1/tests/test_kraken2.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5159 2022-04-05 19:47:02.000000 liquidctl-1.9.1/tests/test_kraken3.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    14889 2022-03-03 13:43:31.000000 liquidctl-1.9.1/tests/test_nvidia.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1097 2022-02-04 08:10:54.000000 liquidctl-1.9.1/tests/test_nzxt_epsu.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8045 2022-02-04 08:10:54.000000 liquidctl-1.9.1/tests/test_rgb_fusion2.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4651 2022-03-03 13:43:31.000000 liquidctl-1.9.1/tests/test_smart_device.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4609 2022-04-05 19:47:02.000000 liquidctl-1.9.1/tests/test_smart_device2.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4401 2022-02-04 08:10:54.000000 liquidctl-1.9.1/tests/test_smbus.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1429 2022-02-04 08:10:54.000000 liquidctl-1.9.1/tests/test_usb.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      215 2022-03-03 13:43:31.000000 liquidctl-1.9.1/tox.ini
```

### Comparing `liquidctl-1.9.0/CHANGELOG.md` & `liquidctl-1.9.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,28 @@
 # Changelog
 
+## [1.9.1] – 2022-04-05
+
+### Changes since 1.9.0
+
+Fixed:
+- Remove excess `_input` suffix when reading `pwmN` attributes from hwmon
+  (#445, PR #446)
+
+### Notes for downstream packagers
+
+Starting with 1.9.0, liquidctl now uses a PEP 517 build.  See the notes for the
+1.9.0 release for more information.
+
+### Know issues
+
+- Corsair Hydro Platinum and Pro XT coolers lock up if simultaneously accessed
+  from more than one program and driver instance (#274)
+
+
 ## [1.9.0] – 2022-04-05
 
 ### Changes since 1.8.1
 
 Added:
 - Add support for persisting settings on modern Asetek 690LC coolers (#355)
 - Add support for setting fixed fan/pump speeds on the Corsair Commander Core
@@ -105,14 +124,21 @@
 [setuptools_scm]: https://github.com/pypa/setuptools_scm
 
 ### Know issues
 
 - Corsair Hydro Platinum and Pro XT coolers lock up if simultaneously accessed
   from more than one program and driver instance (#274)
 
+### Checksums
+
+```
+9e1ae595be2c3ea5899e12741c11307da27e86bc88f7f93c5ae40bb2aa03dc70  dist/liquidctl-1.9.0.tar.gz
+3820c29c0fc86bd6bd601d55a593f1cd476cd563875b45488bef26fc272abf6d  dist/liquidctl-1.9.0-py3-none-any.whl
+```
+
 
 ## [1.8.1] – 2022-01-21
 
 ### Changes since 1.8.0
 
 Fixed:
 - Strip non-determinism from sdist/egg SOURCES.txt metadata
```

### Comparing `liquidctl-1.9.0/CODE_OF_CONDUCT.md` & `liquidctl-1.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/CONTRIBUTING.md` & `liquidctl-1.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/FUNDING.md` & `liquidctl-1.9.1/FUNDING.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/LICENSE.txt` & `liquidctl-1.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/PKG-INFO` & `liquidctl-1.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liquidctl
-Version: 1.9.0
+Version: 1.9.1
 Summary: Cross-platform tool and drivers for liquid coolers and other devices
 Home-page: https://github.com/liquidctl/liquidctl
 Author: Jonas Malaco
 Author-email: jonas@protocubo.io
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/liquidctl/liquidctl/blob/main/README.md
 Project-URL: Changelog, https://github.com/liquidctl/liquidctl/blob/main/CHANGELOG.md
```

### Comparing `liquidctl-1.9.0/README.md` & `liquidctl-1.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -324,16 +324,16 @@
 This will also install the necessary Python libraries.
 
 
 ```bash
 # the latest stable version
 python -m pip install liquidctl
 
-# a specific version (e.g. 1.9.0)
-python -m pip install liquidctl==1.9.0
+# a specific version (e.g. 1.9.1)
+python -m pip install liquidctl==1.9.1
 ```
 
 If [git] is installed, pip can also install the latest snapshot of the official
 liquidctl source code repository on GitHub.
 
 ```bash
 # the latest snapshot of the official source code repository (requires git)
```

### Comparing `liquidctl-1.9.0/SECURITY.md` & `liquidctl-1.9.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/README.md` & `liquidctl-1.9.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/asetek-690lc-guide.md` & `liquidctl-1.9.1/docs/asetek-690lc-guide.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/asetek-pro-guide.md` & `liquidctl-1.9.1/docs/asetek-pro-guide.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/corsair-commander-core-guide.md` & `liquidctl-1.9.1/docs/corsair-commander-core-guide.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/corsair-commander-guide.md` & `liquidctl-1.9.1/docs/corsair-commander-guide.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/corsair-hxi-rmi-psu-guide.md` & `liquidctl-1.9.1/docs/corsair-hxi-rmi-psu-guide.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/corsair-platinum-pro-xt-guide.md` & `liquidctl-1.9.1/docs/corsair-platinum-pro-xt-guide.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/ddr4-guide.md` & `liquidctl-1.9.1/docs/ddr4-guide.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/capturing-usb-traffic.md` & `liquidctl-1.9.1/docs/developer/capturing-usb-traffic.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/creating-vm-for-capture.md` & `liquidctl-1.9.1/docs/developer/creating-vm-for-capture.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/hwmon.md` & `liquidctl-1.9.1/docs/developer/hwmon.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/images/create_vm.png` & `liquidctl-1.9.1/docs/developer/images/create_vm.png`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/images/create_vm_1.png` & `liquidctl-1.9.1/docs/developer/images/create_vm_1.png`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/images/create_vm_10.png` & `liquidctl-1.9.1/docs/developer/images/create_vm_10.png`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/images/create_vm_2.png` & `liquidctl-1.9.1/docs/developer/images/create_vm_2.png`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/images/create_vm_3.png` & `liquidctl-1.9.1/docs/developer/images/create_vm_3.png`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/images/create_vm_4.png` & `liquidctl-1.9.1/docs/developer/images/create_vm_4.png`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/images/create_vm_5.png` & `liquidctl-1.9.1/docs/developer/images/create_vm_5.png`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/images/create_vm_6.png` & `liquidctl-1.9.1/docs/developer/images/create_vm_6.png`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/images/create_vm_7.png` & `liquidctl-1.9.1/docs/developer/images/create_vm_7.png`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/images/create_vm_8.png` & `liquidctl-1.9.1/docs/developer/images/create_vm_8.png`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/images/create_vm_9.png` & `liquidctl-1.9.1/docs/developer/images/create_vm_9.png`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/images/icue.png` & `liquidctl-1.9.1/docs/developer/images/icue.png`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/images/vendor_product_id.png` & `liquidctl-1.9.1/docs/developer/images/vendor_product_id.png`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/images/wireshark_1.png` & `liquidctl-1.9.1/docs/developer/images/wireshark_1.png`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/images/wireshark_2.png` & `liquidctl-1.9.1/docs/developer/images/wireshark_2.png`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/images/wireshark_3.png` & `liquidctl-1.9.1/docs/developer/images/wireshark_3.png`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/images/wireshark_4.png` & `liquidctl-1.9.1/docs/developer/images/wireshark_4.png`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/porting-drivers-from-opencorsairlink.md` & `liquidctl-1.9.1/docs/developer/porting-drivers-from-opencorsairlink.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/process.md` & `liquidctl-1.9.1/docs/developer/process.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/protocol/commander_core.md` & `liquidctl-1.9.1/docs/developer/protocol/commander_core.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/protocol/lighting_node_rgb.md` & `liquidctl-1.9.1/docs/developer/protocol/lighting_node_rgb.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/protocol/vengeance_rgb.md` & `liquidctl-1.9.1/docs/developer/protocol/vengeance_rgb.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/release-checklist.md` & `liquidctl-1.9.1/docs/developer/release-checklist.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,68 @@
 # Release checklist
 
 ## Prepare system
 
- - [ ] Ensure publishing dependencies are installed:
-       `pacman -S twine`
+ - [ ] Ensure publishing dependencies are installed: twine
+ - [ ] Export helper enviroment variable: `export VERSION=<version>`
 
 ## Prepare repository
 
- - [ ] Update liquidctl/version.py
  - [ ] Update last update date in the man page
- - [ ] Make sure the CHANGELOG is up to date
+ - [ ] Update the CHANGELOG
  - [ ] Remove "N/New driver, ..." notes from the table of supported devices (and merge lines if appropriate)
+ - [ ] Update version in pip install liquidctl==version examples
  - [ ] Regenerate the udev rules:
        `(cd extra/linux && python generate-uaccess-udev-rules.py > 71-liquidctl.rules)`
  - [ ] Commit:
        `git commit -m "release: prepare for v$VERSION"`
 
-## Test
+## Test locally
 
  - [ ] Run unit and doc tests:
        `python -m pytest`
 
 Then install locally and:
 
  - [ ] Run my personal setup scripts:
        `liquidcfg && liquiddyncfg`
  - [ ] Test yoda:
        `extra/yoda --match kraken control pump with '(20,50),(50,100)' on coretemp.package_id_0 and fan with '(20,25),(34,100)' on _internal.liquid --verbose`
  - [ ] Test krakenduty:
        `extra/krakenduty-poc train && extra/krakenduty-poc status`
  - [ ] Test liquiddump:
        `extra/liquiddump | jq -c .`
- - [ ] Test krakenx (git):
-       `colctl --mode fading --color_count 2 --color0 192,32,64 --color1 246,11,21 --fan_speed "(30, 100), (40, 100)" --pump_speed "(30, 100), (40, 100)"`
 
-## Source distribution
+## Test in CI
+
+ - [ ] Push HEAD:
+       `git push origin HEAD`
+ - [ ] Check all CI statuses (pytest, flake8 linting, and `list --verbose`)
+
+## Build source distribution and wheel
 
- - [ ] Build the source distribution and wheel:
-       `python -m build`
- - [ ] Check that all necessary files are in the `dist/liquidctl-$VERSION.tar.gz` sdist
- - [ ] Check the `dist/liquidctl-$VERSION.whl` wheel
  - [ ] Tag HEAD with changelog and PGP signature:
        `git tag -as "v$VERSION"`
- - [ ] Push HEAD and vVERSION tag:
-       `git push origin HEAD "v$VERSION"`
- - [ ] Check all CI statuses (pytest, flake8 linting, and `list --verbose`)
- - [ ] Sign the source distribution:
+ - [ ] Build the source distribution and wheel (stash any changes to this file beforehand):
+       `python -m build`
+ - [ ] Check that all necessary files are in the `dist/liquidctl-$VERSION.tar.gz` sdist
+ - [ ] Check the contents of the `dist/liquidctl-$VERSION.whl` wheel
+ - [ ] Sign both sdist and wheel:
        `gpg --detach-sign -a "dist/liquidctl-$VERSION.tar.gz"`
+       `gpg --detach-sign -a "dist/liquidctl-$VERSION-py3-none-any.whl"`
 
 ## Release
 
- - [ ] Upload:
-       `twine upload dist/liquidctl-$VERSION.tar.gz{,.asc}`
- - [ ] Upgrade the vVERSION tag on GitHub to a release (with sdist and corresponding GPG signatures)
- - [ ] Update the HEAD changelog with the release file SHA256 sums:
-       `sha256sum dist/liquidctl-$VERSION.tar.gz | tee "dist/liquidctl-$VERSION.sha256sums"`
+ - [ ] Push vVERSION tag:
+       `git push origin "v$VERSION"`
+ - [ ] Upload sdist and wheel to PyPI:
+       `twine upload dist/liquidctl-$VERSION{.tar.gz,-py3-none-any.whl}{,.asc}`
+ - [ ] Generate SHA256 checksums for the release files:
+       `sha256sum dist/liquidctl-$VERSION{.tar.gz,-py3-none-any.whl} | tee "dist/liquidctl-$VERSION.sha256sums"`
+ - [ ] Upgrade the vVERSION tag on GitHub to a release (with sdist, wheel, and corresponding GPG signatures)
+ - [ ] Update the HEAD changelog with the SHA256 checksums
 
 ## Post release
 
  - [ ] Merge the release branch into the main branch (if appropriate)
  - [ ] Update the HEAD release-checklist with this checklist
  - [ ] Update ArchLinux `liquidctl-git`
```

### Comparing `liquidctl-1.9.0/docs/developer/style-guide.md` & `liquidctl-1.9.1/docs/developer/style-guide.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/developer/techniques-for-analyzing-usb-protocols.md` & `liquidctl-1.9.1/docs/developer/techniques-for-analyzing-usb-protocols.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/gigabyte-rgb-fusion2-guide.md` & `liquidctl-1.9.1/docs/gigabyte-rgb-fusion2-guide.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/kraken-x2-m2-guide.md` & `liquidctl-1.9.1/docs/kraken-x2-m2-guide.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/kraken-x3-z3-guide.md` & `liquidctl-1.9.1/docs/kraken-x3-z3-guide.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/linux/making-systemd-units-wait-for-devices.md` & `liquidctl-1.9.1/docs/linux/making-systemd-units-wait-for-devices.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/nvidia-guide.md` & `liquidctl-1.9.1/docs/nvidia-guide.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/nzxt-e-series-psu-guide.md` & `liquidctl-1.9.1/docs/nzxt-e-series-psu-guide.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/nzxt-hue2-guide.md` & `liquidctl-1.9.1/docs/nzxt-hue2-guide.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/nzxt-smart-device-v1-guide.md` & `liquidctl-1.9.1/docs/nzxt-smart-device-v1-guide.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/docs/windows/running-your-first-command-line-program.md` & `liquidctl-1.9.1/docs/windows/running-your-first-command-line-program.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/completions/liquidctl.bash` & `liquidctl-1.9.1/extra/completions/liquidctl.bash`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/contrib/fusion_rgb_cycle.py` & `liquidctl-1.9.1/extra/contrib/fusion_rgb_cycle.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/contrib/liquidctlfan/README.md` & `liquidctl-1.9.1/extra/contrib/liquidctlfan/README.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/contrib/liquidctlfan/liquidctlfan` & `liquidctl-1.9.1/extra/contrib/liquidctlfan/liquidctlfan`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/dist/pypi-readme.md` & `liquidctl-1.9.1/extra/dist/pypi-readme.md`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/krakenduty-poc` & `liquidctl-1.9.1/extra/krakenduty-poc`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/linux/71-liquidctl.rules` & `liquidctl-1.9.1/extra/linux/71-liquidctl.rules`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/linux/generate-uaccess-udev-rules.py` & `liquidctl-1.9.1/extra/linux/generate-uaccess-udev-rules.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/liquiddump` & `liquidctl-1.9.1/extra/liquiddump`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/old-tests/asetek_legacy` & `liquidctl-1.9.1/extra/old-tests/asetek_legacy`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/old-tests/asetek_modern` & `liquidctl-1.9.1/extra/old-tests/asetek_modern`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/old-tests/asetek_modern_rainbow` & `liquidctl-1.9.1/extra/old-tests/asetek_modern_rainbow`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/old-tests/kraken_two` & `liquidctl-1.9.1/extra/old-tests/kraken_two`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/prometheus-liquidctl-exporter` & `liquidctl-1.9.1/extra/prometheus-liquidctl-exporter`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/windows/LQiNFO.py` & `liquidctl-1.9.1/extra/windows/LQiNFO.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/windows/liquidctl_logo_v1_circle_256.ico` & `liquidctl-1.9.1/extra/windows/liquidctl_logo_v1_circle_256.ico`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/windows/redist-notices.txt` & `liquidctl-1.9.1/extra/windows/redist-notices.txt`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/extra/yoda` & `liquidctl-1.9.1/extra/yoda`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/cli.py` & `liquidctl-1.9.1/liquidctl/cli.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/driver/__init__.py` & `liquidctl-1.9.1/liquidctl/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/driver/asetek.py` & `liquidctl-1.9.1/liquidctl/driver/asetek.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/driver/asetek_pro.py` & `liquidctl-1.9.1/liquidctl/driver/asetek_pro.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/driver/base.py` & `liquidctl-1.9.1/liquidctl/driver/base.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/driver/commander_core.py` & `liquidctl-1.9.1/liquidctl/driver/commander_core.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/driver/commander_pro.py` & `liquidctl-1.9.1/liquidctl/driver/commander_pro.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/driver/corsair_hid_psu.py` & `liquidctl-1.9.1/liquidctl/driver/corsair_hid_psu.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/driver/ddr4.py` & `liquidctl-1.9.1/liquidctl/driver/ddr4.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/driver/hwmon.py` & `liquidctl-1.9.1/liquidctl/driver/hwmon.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/driver/hydro_platinum.py` & `liquidctl-1.9.1/liquidctl/driver/hydro_platinum.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/driver/kraken2.py` & `liquidctl-1.9.1/liquidctl/driver/kraken2.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/driver/kraken3.py` & `liquidctl-1.9.1/liquidctl/driver/kraken3.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,28 +241,28 @@
             (_STATUS_PUMP_DUTY, msg[19], '%'),
         ]
 
     def _get_status_from_hwmon(self):
         return [
             (_STATUS_TEMPERATURE, self._hwmon.get_int('temp1_input') * 1e-3, '°C'),
             (_STATUS_PUMP_SPEED, self._hwmon.get_int('fan1_input'), 'rpm'),
-            (_STATUS_PUMP_DUTY, self._hwmon.get_int('pwm1_input') * 100. / 255, '%'),
+            (_STATUS_PUMP_DUTY, self._hwmon.get_int('pwm1') * 100. / 255, '%'),
         ]
 
     def get_status(self, direct_access=False, **kwargs):
         """Get a status report.
 
         Returns a list of `(property, value, unit)` tuples.
         """
 
-        # no driver currently supports pwm1_input, so silently fallback to
+        # no driver currently supports pwm1, so silently fallback to
         # direct mode if it isn't available; for the same reason, also don't
         # yet issue a warning when directly accessing the device
 
-        if self._hwmon and not direct_access and self._hwmon.has_attribute('pwm1_input'):
+        if self._hwmon and not direct_access and self._hwmon.has_attribute('pwm1'):
             _LOGGER.info('bound to %s kernel driver, reading status from hwmon', self._hwmon.module)
             return self._get_status_from_hwmon()
 
         if self._hwmon:
             level = logging.WARNING if direct_access else logging.INFO
             _LOGGER.log(level, 'directly reading the status despite %s kernel driver',
                         self._hwmon.module)
```

### Comparing `liquidctl-1.9.0/liquidctl/driver/nvidia.py` & `liquidctl-1.9.1/liquidctl/driver/nvidia.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/driver/nzxt_epsu.py` & `liquidctl-1.9.1/liquidctl/driver/nzxt_epsu.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/driver/rgb_fusion2.py` & `liquidctl-1.9.1/liquidctl/driver/rgb_fusion2.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/driver/smart_device.py` & `liquidctl-1.9.1/liquidctl/driver/smart_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,15 +545,15 @@
 
     def _get_status_from_hwmon(self):
         ret = []
         modes = ['DC', 'PWM']
 
         for n in range(1, len(self._speed_channels) + 1):
             ret.append((f'Fan {n} speed', self._hwmon.get_int(f'fan{n}_input'), 'rpm')),
-            ret.append((f'Fan {n} duty', self._hwmon.get_int(f'pwm{n}_input') * 100. / 255, '%')),
+            ret.append((f'Fan {n} duty', self._hwmon.get_int(f'pwm{n}') * 100. / 255, '%')),
             ret.append((f'Fan {n} control mode', modes[self._hwmon.get_int(f'pwm{n}_mode')], '')),
 
         # noise level is not available through hwmon, but also not very accurate or useful
 
         return sorted(ret)
 
     def get_status(self, direct_access=False, **kwargs):
```

### Comparing `liquidctl-1.9.0/liquidctl/driver/smbus.py` & `liquidctl-1.9.1/liquidctl/driver/smbus.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/driver/usb.py` & `liquidctl-1.9.1/liquidctl/driver/usb.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/keyval.py` & `liquidctl-1.9.1/liquidctl/keyval.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/pmbus.py` & `liquidctl-1.9.1/liquidctl/pmbus.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/util.py` & `liquidctl-1.9.1/liquidctl/util.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl/version.py` & `liquidctl-1.9.1/liquidctl/version.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl.8` & `liquidctl-1.9.1/liquidctl.8`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/liquidctl.egg-info/PKG-INFO` & `liquidctl-1.9.1/liquidctl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liquidctl
-Version: 1.9.0
+Version: 1.9.1
 Summary: Cross-platform tool and drivers for liquid coolers and other devices
 Home-page: https://github.com/liquidctl/liquidctl
 Author: Jonas Malaco
 Author-email: jonas@protocubo.io
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/liquidctl/liquidctl/blob/main/README.md
 Project-URL: Changelog, https://github.com/liquidctl/liquidctl/blob/main/CHANGELOG.md
```

### Comparing `liquidctl-1.9.0/liquidctl.egg-info/SOURCES.txt` & `liquidctl-1.9.1/liquidctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/pyproject.toml` & `liquidctl-1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/setup.cfg` & `liquidctl-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/_testutils.py` & `liquidctl-1.9.1/tests/_testutils.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_api.py` & `liquidctl-1.9.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_asetek.py` & `liquidctl-1.9.1/tests/test_asetek.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_asetek_pro.py` & `liquidctl-1.9.1/tests/test_asetek_pro.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_backward_compatibility_10.py` & `liquidctl-1.9.1/tests/test_backward_compatibility_10.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_backward_compatibility_11.py` & `liquidctl-1.9.1/tests/test_backward_compatibility_11.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_backward_compatibility_13.py` & `liquidctl-1.9.1/tests/test_backward_compatibility_13.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_backward_compatibility_14.py` & `liquidctl-1.9.1/tests/test_backward_compatibility_14.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_backward_compatibility_15.py` & `liquidctl-1.9.1/tests/test_backward_compatibility_15.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_cli.py` & `liquidctl-1.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_commander_core.py` & `liquidctl-1.9.1/tests/test_commander_core.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_commander_pro.py` & `liquidctl-1.9.1/tests/test_commander_pro.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_corsair_hid_psu.py` & `liquidctl-1.9.1/tests/test_corsair_hid_psu.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_ddr4.py` & `liquidctl-1.9.1/tests/test_ddr4.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_hidapi_device.py` & `liquidctl-1.9.1/tests/test_hidapi_device.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_hwmon.py` & `liquidctl-1.9.1/tests/test_hwmon.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_hydro_platinum.py` & `liquidctl-1.9.1/tests/test_hydro_platinum.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_keyval.py` & `liquidctl-1.9.1/tests/test_keyval.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_kraken2.py` & `liquidctl-1.9.1/tests/test_kraken2.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_kraken3.py` & `liquidctl-1.9.1/tests/test_kraken3.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     assert pump_duty == ("Pump duty", 53, "%")
 
 
 def test_krakenx3_reads_status_from_hwmon(mock_krakenx3, tmp_path):
     mock_krakenx3._hwmon = HwmonDevice("mock_module", tmp_path)
     (tmp_path / "temp1_input").write_text("33100\n")
     (tmp_path / "fan1_input").write_text("1704\n")
-    (tmp_path / "pwm1_input").write_text("135\n")
+    (tmp_path / "pwm1").write_text("135\n")
 
     temperature, pump_speed, pump_duty = mock_krakenx3.get_status()
 
     assert temperature == ("Liquid temperature", 33.1, "°C")
     assert pump_speed == ("Pump speed", 1704, "rpm")
     assert pump_duty == ("Pump duty", pytest.approx(53, rel=1.0 / 255), "%")
```

### Comparing `liquidctl-1.9.0/tests/test_nvidia.py` & `liquidctl-1.9.1/tests/test_nvidia.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_nzxt_epsu.py` & `liquidctl-1.9.1/tests/test_nzxt_epsu.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_rgb_fusion2.py` & `liquidctl-1.9.1/tests/test_rgb_fusion2.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_smart_device.py` & `liquidctl-1.9.1/tests/test_smart_device.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_smart_device2.py` & `liquidctl-1.9.1/tests/test_smart_device2.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,17 @@
     mock_smart2._hwmon = HwmonDevice("mock_module", tmp_path)
     (tmp_path / "pwm1_enable").write_text("1\n")
     (tmp_path / "pwm2_enable").write_text("0\n")
     (tmp_path / "pwm3_enable").write_text("0\n")
     (tmp_path / "pwm1_mode").write_text("1\n")
     (tmp_path / "pwm2_mode").write_text("0\n")
     (tmp_path / "pwm3_mode").write_text("0\n")
-    (tmp_path / "pwm1_input").write_text("127\n")
-    (tmp_path / "pwm2_input").write_text("102\n")
-    (tmp_path / "pwm3_input").write_text("102\n")
+    (tmp_path / "pwm1").write_text("127\n")
+    (tmp_path / "pwm2").write_text("102\n")
+    (tmp_path / "pwm3").write_text("102\n")
     (tmp_path / "fan1_input").write_text("1020\n")
     (tmp_path / "fan2_input").write_text("0\n")
     (tmp_path / "fan3_input").write_text("0\n")
 
     expected = [
         ("Fan 1 speed", 1020, "rpm"),
         ("Fan 1 duty", pytest.approx(50, rel=1.0 / 255), "%"),
```

### Comparing `liquidctl-1.9.0/tests/test_smbus.py` & `liquidctl-1.9.1/tests/test_smbus.py`

 * *Files identical despite different names*

### Comparing `liquidctl-1.9.0/tests/test_usb.py` & `liquidctl-1.9.1/tests/test_usb.py`

 * *Files identical despite different names*


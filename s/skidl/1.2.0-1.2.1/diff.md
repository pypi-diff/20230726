# Comparing `tmp/skidl-1.2.0.tar.gz` & `tmp/skidl-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skidl-1.2.0.tar", last modified: Sat Jul 15 17:02:09 2023, max compression
+gzip compressed data, was "skidl-1.2.1.tar", last modified: Wed Jul 26 17:14:02 2023, max compression
```

## Comparing `skidl-1.2.0.tar` & `skidl-1.2.1.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-15 17:02:09.741043 skidl-1.2.0/
--rwxrwxrwx   0 devb      (1000) devb      (1000)      292 2020-10-21 16:56:05.000000 skidl-1.2.0/.editorconfig
-drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-15 17:02:09.705043 skidl-1.2.0/.github/
-drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-15 17:02:09.709043 skidl-1.2.0/.github/ISSUE_TEMPLATE/
--rwxrwxrwx   0 devb      (1000) devb      (1000)      673 2020-10-21 16:56:05.000000 skidl-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rwxrwxrwx   0 devb      (1000) devb      (1000)      633 2020-10-21 16:56:05.000000 skidl-1.2.0/.github/ISSUE_TEMPLATE/skidl-feature-request.md
--rw-rw-r--   0 devb      (1000) devb      (1000)      682 2023-07-14 21:45:39.000000 skidl-1.2.0/.gitignore
--rwxrwxrwx   0 devb      (1000) devb      (1000)        0 2020-10-21 16:56:05.000000 skidl-1.2.0/.nojekyll
--rw-rw-r--   0 devb      (1000) devb      (1000)      915 2023-07-14 21:45:39.000000 skidl-1.2.0/.travis.yml
-drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-15 17:02:09.709043 skidl-1.2.0/.vscode/
--rw-rw-r--   0 devb      (1000) devb      (1000)      267 2023-07-14 21:45:39.000000 skidl-1.2.0/.vscode/settings.json
--rw-rw-r--   0 devb      (1000) devb      (1000)      251 2021-11-10 21:29:45.000000 skidl-1.2.0/AUTHORS.rst
--rw-rw-r--   0 devb      (1000) devb      (1000)     2592 2021-11-10 21:29:45.000000 skidl-1.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 devb      (1000) devb      (1000)    13644 2023-07-15 14:46:00.000000 skidl-1.2.0/HISTORY.rst
--rw-rw-r--   0 devb      (1000) devb      (1000)     1089 2021-11-10 21:29:45.000000 skidl-1.2.0/LICENSE
--rw-rw-r--   0 devb      (1000) devb      (1000)      345 2023-07-14 21:45:39.000000 skidl-1.2.0/MANIFEST.in
--rw-rw-r--   0 devb      (1000) devb      (1000)     1579 2023-07-14 21:45:39.000000 skidl-1.2.0/Makefile
--rw-rw-r--   0 devb      (1000) devb      (1000)    21664 2023-07-15 17:02:09.741043 skidl-1.2.0/PKG-INFO
--rw-rw-r--   0 devb      (1000) devb      (1000)     6936 2023-07-14 21:45:39.000000 skidl-1.2.0/README.rst
-drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-15 17:02:09.709043 skidl-1.2.0/icons/
--rwxrwxrwx   0 devb      (1000) devb      (1000)       81 2020-10-21 16:56:06.000000 skidl-1.2.0/icons/make_ico.cmd
--rwxrwxrwx   0 devb      (1000) devb      (1000)   308213 2020-10-21 16:56:06.000000 skidl-1.2.0/icons/part_fp_search_icon.ico
--rwxrwxrwx   0 devb      (1000) devb      (1000)    74186 2020-10-21 16:56:06.000000 skidl-1.2.0/icons/part_fp_search_icon.png
--rwxrwxrwx   0 devb      (1000) devb      (1000)    13553 2020-10-21 16:56:06.000000 skidl-1.2.0/icons/part_fp_search_icon_master.svg
--rwxrwxrwx   0 devb      (1000) devb      (1000)      496 2020-10-21 16:56:06.000000 skidl-1.2.0/pyproject.toml
--rwxrwxrwx   0 devb      (1000) devb      (1000)       49 2021-04-30 20:57:13.000000 skidl-1.2.0/requirements.txt
--rwxrwxrwx   0 devb      (1000) devb      (1000)       61 2023-07-15 17:02:09.741043 skidl-1.2.0/setup.cfg
--rw-rw-r--   0 devb      (1000) devb      (1000)     2566 2023-07-14 21:45:39.000000 skidl-1.2.0/setup.py
-drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-15 17:02:09.705043 skidl-1.2.0/src/
-drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-15 17:02:09.713043 skidl-1.2.0/src/skidl/
--rw-rw-r--   0 devb      (1000) devb      (1000)     2076 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/__init__.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     1508 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/alias.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    15319 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/bus.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    41722 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/circuit.py
--rw-rw-r--   0 devb      (1000) devb      (1000)      493 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/common.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     3803 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/config.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     3699 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/erc.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     2362 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/group.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     7844 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/interface.py
-drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-15 17:02:09.737043 skidl-1.2.0/src/skidl/libs/
--rw-rw-r--   0 devb      (1000) devb      (1000)    42158 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/74xgxx_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)   153929 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/74xx_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    12446 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/Altera_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    11293 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/ESD_Protection_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     2679 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/LEM_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     6015 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/Lattice_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     8538 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/NXP_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    16377 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/Oscillators_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    20048 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/Power_Management_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     1075 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/RFSolutions_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     2114 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/Worldsemi_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     6135 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/Xicor_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     5393 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/Zilog_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)        0 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/__init__.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     9841 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/ac-dc_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)   138224 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/actel_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)   102591 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/adc-dac_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     4473 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/allegro_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    14637 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/analog_devices_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     7065 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/analog_switches_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)   677194 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/atmel_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    23570 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/audio_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    20429 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/battery_management_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     6841 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/bbd_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     2251 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/bosch_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    35355 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/brooktre_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    41704 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/cmos4000_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     6105 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/cmos_ieee_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)   311091 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/conn_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     1281 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/contrib_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)      627 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/convert_libs.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    22211 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/cypress_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    81018 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/dc-dc_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)   142960 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/device_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    28336 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/digital-audio_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    13182 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/diode_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    17169 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/display_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    21867 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/dsp_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    12420 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/elec-unifil_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    39708 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/ftdi_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    10067 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/gennum_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     2525 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/graphic_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     8132 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/hc11_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    50059 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/intel_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    76127 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/interface_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     7290 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/intersil_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     8735 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/ir_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     1843 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/leds_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    72984 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/linear_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)      437 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/logo_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    14100 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/maxim_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     1364 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/mechanical_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)   121674 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/memory_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    35245 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/microchip_dspic33dsc_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     6252 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/microchip_pic10mcu_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    23730 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/microchip_pic12mcu_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    57867 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/microchip_pic16mcu_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)   109898 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/microchip_pic18mcu_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     4054 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/microchip_pic24mcu_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    12658 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/microchip_pic32mcu_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    32523 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/microchip_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    15659 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/microcontrollers_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    10208 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/modules_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    23324 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/motor_drivers_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)   265746 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/motorola_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     6316 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/motors_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)   334414 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/msp430_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     2414 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/nordicsemi_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)   122160 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/nxp_armmcu_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     2938 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/onsemi_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    63636 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/opto_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    17036 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/philips_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     8114 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/power_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    32202 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/powerint_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)      923 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/pspice_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    65867 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/pyspice_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    24735 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/references_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    76322 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/regul_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     9914 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/relays_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    39046 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/rfcom_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    46371 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/sensors_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     8888 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/silabs_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     2245 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/siliconi_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     1207 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/skidl_lib_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)  4119071 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/stm32_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     8126 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/stm8_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     8411 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/supertex_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    25693 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/switches_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    73772 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/texas_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    11592 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/transf_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    86534 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/transistors_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     2064 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/triac_thyristor_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    10423 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/ttl_ieee_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     8564 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/valves_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    13398 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/video_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     5080 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/wiznet_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)   183562 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/xilinx_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)      738 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/libs/zetex_sklib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     7696 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/logger.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    30989 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/net.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     1158 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/netclass.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     5952 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/netlist_to_skidl.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     5851 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/netpinlist.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     4130 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/network.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     1481 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/note.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     4324 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/package.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    48222 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/part.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    15171 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/part_query.py
--rw-rw-r--   0 devb      (1000) devb      (1000)       81 2023-07-15 17:02:08.000000 skidl-1.2.0/src/skidl/pckg_info.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    27457 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/pin.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     3317 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/protonet.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     1884 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/pyspice.py
-drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-15 17:02:09.737043 skidl-1.2.0/src/skidl/schematics/
--rw-rw-r--   0 devb      (1000) devb      (1000)        0 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/schematics/__init__.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    11343 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/schematics/debug_draw.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    25063 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/schematics/gen_schematic.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    13930 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/schematics/geometry.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    62364 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/schematics/place.py
--rw-rw-r--   0 devb      (1000) devb      (1000)   140696 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/schematics/route.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     8350 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/schlib.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     4068 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/scriptinfo.py
-drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-15 17:02:09.737043 skidl-1.2.0/src/skidl/scripts/
--rw-rw-r--   0 devb      (1000) devb      (1000)     3704 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/scripts/netlist_to_skidl_main.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     4473 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/skidl.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     5194 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/skidlbaseobj.py
-drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-15 17:02:09.737043 skidl-1.2.0/src/skidl/tools/
--rw-rw-r--   0 devb      (1000) devb      (1000)     1939 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/tools/__init__.py
-drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-15 17:02:09.741043 skidl-1.2.0/src/skidl/tools/kicad/
--rw-rw-r--   0 devb      (1000) devb      (1000)      409 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/tools/kicad/__init__.py
--rw-rw-r--   0 devb      (1000) devb      (1000)      319 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/tools/kicad/constants.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    17469 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/tools/kicad/eeschema_v5.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    10842 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/tools/kicad/kicad.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    53541 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/tools/kicad/v5.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    11075 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/tools/kicad/v6.py
-drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-15 17:02:09.741043 skidl-1.2.0/src/skidl/tools/skidl/
--rw-rw-r--   0 devb      (1000) devb      (1000)      164 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/tools/skidl/__init__.py
--rw-rw-r--   0 devb      (1000) devb      (1000)     2428 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/tools/skidl/skidl.py
-drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-15 17:02:09.741043 skidl-1.2.0/src/skidl/tools/spice/
--rw-rw-r--   0 devb      (1000) devb      (1000)      408 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/tools/spice/__init__.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    22685 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/tools/spice/spice.py
--rw-rw-r--   0 devb      (1000) devb      (1000)    29874 2023-07-14 21:45:39.000000 skidl-1.2.0/src/skidl/utilities.py
-drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-15 17:02:09.713043 skidl-1.2.0/src/skidl.egg-info/
--rw-rw-r--   0 devb      (1000) devb      (1000)    21664 2023-07-15 17:02:08.000000 skidl-1.2.0/src/skidl.egg-info/PKG-INFO
--rw-rw-r--   0 devb      (1000) devb      (1000)     5052 2023-07-15 17:02:09.000000 skidl-1.2.0/src/skidl.egg-info/SOURCES.txt
--rw-rw-r--   0 devb      (1000) devb      (1000)        1 2023-07-15 17:02:08.000000 skidl-1.2.0/src/skidl.egg-info/dependency_links.txt
--rw-rw-r--   0 devb      (1000) devb      (1000)       78 2023-07-15 17:02:08.000000 skidl-1.2.0/src/skidl.egg-info/entry_points.txt
--rw-rw-r--   0 devb      (1000) devb      (1000)        1 2023-01-10 18:59:49.000000 skidl-1.2.0/src/skidl.egg-info/not-zip-safe
--rw-rw-r--   0 devb      (1000) devb      (1000)      119 2023-07-15 17:02:08.000000 skidl-1.2.0/src/skidl.egg-info/requires.txt
--rw-rw-r--   0 devb      (1000) devb      (1000)        6 2023-07-15 17:02:08.000000 skidl-1.2.0/src/skidl.egg-info/top_level.txt
--rw-rw-r--   0 devb      (1000) devb      (1000)     3929 2023-07-14 21:45:39.000000 skidl-1.2.0/tox.ini
+drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-26 17:14:02.417424 skidl-1.2.1/
+-rwxrwxrwx   0 devb      (1000) devb      (1000)      292 2020-10-21 16:56:05.000000 skidl-1.2.1/.editorconfig
+drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-26 17:14:02.377424 skidl-1.2.1/.github/
+drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-26 17:14:02.381424 skidl-1.2.1/.github/ISSUE_TEMPLATE/
+-rwxrwxrwx   0 devb      (1000) devb      (1000)      673 2020-10-21 16:56:05.000000 skidl-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rwxrwxrwx   0 devb      (1000) devb      (1000)      633 2020-10-21 16:56:05.000000 skidl-1.2.1/.github/ISSUE_TEMPLATE/skidl-feature-request.md
+-rw-rw-r--   0 devb      (1000) devb      (1000)      682 2023-07-23 20:23:31.000000 skidl-1.2.1/.gitignore
+-rwxrwxrwx   0 devb      (1000) devb      (1000)        0 2020-10-21 16:56:05.000000 skidl-1.2.1/.nojekyll
+-rw-rw-r--   0 devb      (1000) devb      (1000)      915 2023-07-23 20:19:46.000000 skidl-1.2.1/.travis.yml
+drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-26 17:14:02.381424 skidl-1.2.1/.vscode/
+-rw-rw-r--   0 devb      (1000) devb      (1000)      267 2023-07-23 20:23:31.000000 skidl-1.2.1/.vscode/settings.json
+-rw-rw-r--   0 devb      (1000) devb      (1000)      251 2021-11-10 21:29:45.000000 skidl-1.2.1/AUTHORS.rst
+-rw-rw-r--   0 devb      (1000) devb      (1000)     2592 2021-11-10 21:29:45.000000 skidl-1.2.1/CONTRIBUTING.rst
+-rw-rw-r--   0 devb      (1000) devb      (1000)    13770 2023-07-26 17:05:16.000000 skidl-1.2.1/HISTORY.rst
+-rw-rw-r--   0 devb      (1000) devb      (1000)     1089 2021-11-10 21:29:45.000000 skidl-1.2.1/LICENSE
+-rw-rw-r--   0 devb      (1000) devb      (1000)      345 2023-07-23 20:19:46.000000 skidl-1.2.1/MANIFEST.in
+-rw-rw-r--   0 devb      (1000) devb      (1000)     1579 2023-07-23 20:19:46.000000 skidl-1.2.1/Makefile
+-rw-rw-r--   0 devb      (1000) devb      (1000)    21790 2023-07-26 17:14:02.417424 skidl-1.2.1/PKG-INFO
+-rw-rw-r--   0 devb      (1000) devb      (1000)     6936 2023-07-23 20:23:31.000000 skidl-1.2.1/README.rst
+drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-26 17:14:02.385424 skidl-1.2.1/icons/
+-rwxrwxrwx   0 devb      (1000) devb      (1000)       81 2020-10-21 16:56:06.000000 skidl-1.2.1/icons/make_ico.cmd
+-rwxrwxrwx   0 devb      (1000) devb      (1000)   308213 2020-10-21 16:56:06.000000 skidl-1.2.1/icons/part_fp_search_icon.ico
+-rwxrwxrwx   0 devb      (1000) devb      (1000)    74186 2020-10-21 16:56:06.000000 skidl-1.2.1/icons/part_fp_search_icon.png
+-rwxrwxrwx   0 devb      (1000) devb      (1000)    13553 2020-10-21 16:56:06.000000 skidl-1.2.1/icons/part_fp_search_icon_master.svg
+-rwxrwxrwx   0 devb      (1000) devb      (1000)      496 2020-10-21 16:56:06.000000 skidl-1.2.1/pyproject.toml
+-rwxrwxrwx   0 devb      (1000) devb      (1000)       49 2021-04-30 20:57:13.000000 skidl-1.2.1/requirements.txt
+-rwxrwxrwx   0 devb      (1000) devb      (1000)       61 2023-07-26 17:14:02.417424 skidl-1.2.1/setup.cfg
+-rw-rw-r--   0 devb      (1000) devb      (1000)     2566 2023-07-26 17:05:55.000000 skidl-1.2.1/setup.py
+drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-26 17:14:02.377424 skidl-1.2.1/src/
+drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-26 17:14:02.389424 skidl-1.2.1/src/skidl/
+-rw-rw-r--   0 devb      (1000) devb      (1000)     1997 2023-07-26 17:02:32.000000 skidl-1.2.1/src/skidl/__init__.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     1508 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/alias.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    15319 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/bus.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    42282 2023-07-26 17:02:32.000000 skidl-1.2.1/src/skidl/circuit.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)      493 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/common.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     4892 2023-07-26 17:02:32.000000 skidl-1.2.1/src/skidl/config_.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     3699 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/erc.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     2362 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/group.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     7844 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/interface.py
+drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-26 17:14:02.413424 skidl-1.2.1/src/skidl/libs/
+-rw-rw-r--   0 devb      (1000) devb      (1000)    42158 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/74xgxx_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)   153929 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/74xx_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    12446 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/Altera_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    11293 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/ESD_Protection_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     2679 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/LEM_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     6015 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/Lattice_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     8538 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/NXP_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    16377 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/Oscillators_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    20048 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/Power_Management_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     1075 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/RFSolutions_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     2114 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/Worldsemi_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     6135 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/Xicor_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     5393 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/Zilog_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)        0 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/__init__.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     9841 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/ac-dc_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)   138224 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/actel_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)   102591 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/adc-dac_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     4473 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/allegro_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    14637 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/analog_devices_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     7065 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/analog_switches_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)   677194 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/atmel_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    23570 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/audio_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    20429 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/battery_management_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     6841 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/bbd_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     2251 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/bosch_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    35355 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/brooktre_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    41704 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/cmos4000_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     6105 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/cmos_ieee_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)   311091 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/conn_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     1281 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/contrib_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)      627 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/libs/convert_libs.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    22211 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/cypress_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    81018 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/dc-dc_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)   142960 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/device_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    28336 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/digital-audio_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    13182 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/diode_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    17169 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/display_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    21867 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/dsp_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    12420 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/elec-unifil_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    39708 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/ftdi_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    10067 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/gennum_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     2525 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/graphic_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     8132 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/hc11_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    50059 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/intel_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    76127 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/interface_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     7290 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/intersil_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     8735 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/ir_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     1843 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/leds_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    72984 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/linear_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)      437 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/logo_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    14100 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/maxim_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     1364 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/mechanical_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)   121674 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/memory_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    35245 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/microchip_dspic33dsc_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     6252 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/microchip_pic10mcu_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    23730 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/microchip_pic12mcu_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    57867 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/microchip_pic16mcu_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)   109898 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/microchip_pic18mcu_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     4054 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/microchip_pic24mcu_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    12658 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/microchip_pic32mcu_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    32523 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/microchip_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    15659 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/microcontrollers_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    10208 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/modules_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    23324 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/motor_drivers_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)   265746 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/motorola_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     6316 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/motors_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)   334414 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/msp430_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     2414 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/nordicsemi_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)   122160 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/nxp_armmcu_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     2938 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/onsemi_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    63636 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/opto_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    17036 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/philips_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     8114 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/power_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    32202 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/powerint_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)      923 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/pspice_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    65867 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/libs/pyspice_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    24735 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/references_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    76322 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/regul_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     9914 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/relays_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    39046 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/rfcom_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    46371 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/sensors_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     8888 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/silabs_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     2245 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/siliconi_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     1207 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/skidl_lib_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)  4119071 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/stm32_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     8126 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/stm8_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     8411 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/supertex_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    25693 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/switches_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    73772 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/texas_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    11592 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/transf_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    86534 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/transistors_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     2064 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/triac_thyristor_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    10423 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/ttl_ieee_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     8564 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/valves_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    13398 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/video_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     5080 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/wiznet_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)   183562 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/xilinx_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)      738 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/libs/zetex_sklib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     7738 2023-07-26 17:02:32.000000 skidl-1.2.1/src/skidl/logger.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    30882 2023-07-26 17:02:32.000000 skidl-1.2.1/src/skidl/net.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     1158 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/netclass.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     5952 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/netlist_to_skidl.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     5851 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/netpinlist.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     4130 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/network.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     1481 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/note.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     4324 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/package.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    48157 2023-07-26 17:02:32.000000 skidl-1.2.1/src/skidl/part.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    15076 2023-07-26 17:02:32.000000 skidl-1.2.1/src/skidl/part_query.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)       81 2023-07-26 17:14:01.000000 skidl-1.2.1/src/skidl/pckg_info.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    27457 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/pin.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     3317 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/protonet.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     1884 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/pyspice.py
+drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-26 17:14:02.413424 skidl-1.2.1/src/skidl/schematics/
+-rw-rw-r--   0 devb      (1000) devb      (1000)        0 2023-07-23 20:23:31.000000 skidl-1.2.1/src/skidl/schematics/__init__.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    11343 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/schematics/debug_draw.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    25063 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/schematics/gen_schematic.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    13930 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/schematics/geometry.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    62357 2023-07-26 17:02:32.000000 skidl-1.2.1/src/skidl/schematics/place.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)   140689 2023-07-26 17:02:32.000000 skidl-1.2.1/src/skidl/schematics/route.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     8911 2023-07-26 17:02:32.000000 skidl-1.2.1/src/skidl/schlib.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     4068 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/scriptinfo.py
+drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-26 17:14:02.413424 skidl-1.2.1/src/skidl/scripts/
+-rw-rw-r--   0 devb      (1000) devb      (1000)     3704 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/scripts/netlist_to_skidl_main.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     2591 2023-07-26 17:02:32.000000 skidl-1.2.1/src/skidl/skidl.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     5194 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/skidlbaseobj.py
+drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-26 17:14:02.413424 skidl-1.2.1/src/skidl/tools/
+-rw-rw-r--   0 devb      (1000) devb      (1000)     1939 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/tools/__init__.py
+drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-26 17:14:02.417424 skidl-1.2.1/src/skidl/tools/kicad/
+-rw-rw-r--   0 devb      (1000) devb      (1000)      409 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/tools/kicad/__init__.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)      319 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/tools/kicad/constants.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    17469 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/tools/kicad/eeschema_v5.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    10842 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/tools/kicad/kicad.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    53541 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/tools/kicad/v5.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    11075 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/tools/kicad/v6.py
+drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-26 17:14:02.417424 skidl-1.2.1/src/skidl/tools/skidl/
+-rw-rw-r--   0 devb      (1000) devb      (1000)      164 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/tools/skidl/__init__.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)     2428 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/tools/skidl/skidl.py
+drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-26 17:14:02.417424 skidl-1.2.1/src/skidl/tools/spice/
+-rw-rw-r--   0 devb      (1000) devb      (1000)      408 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/tools/spice/__init__.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    22685 2023-07-26 14:57:44.000000 skidl-1.2.1/src/skidl/tools/spice/spice.py
+-rw-rw-r--   0 devb      (1000) devb      (1000)    30645 2023-07-26 17:02:32.000000 skidl-1.2.1/src/skidl/utilities.py
+drwxrwxr-x   0 devb      (1000) devb      (1000)        0 2023-07-26 17:14:02.389424 skidl-1.2.1/src/skidl.egg-info/
+-rw-rw-r--   0 devb      (1000) devb      (1000)    21790 2023-07-26 17:14:01.000000 skidl-1.2.1/src/skidl.egg-info/PKG-INFO
+-rw-rw-r--   0 devb      (1000) devb      (1000)     5053 2023-07-26 17:14:02.000000 skidl-1.2.1/src/skidl.egg-info/SOURCES.txt
+-rw-rw-r--   0 devb      (1000) devb      (1000)        1 2023-07-26 17:14:01.000000 skidl-1.2.1/src/skidl.egg-info/dependency_links.txt
+-rw-rw-r--   0 devb      (1000) devb      (1000)       78 2023-07-26 17:14:01.000000 skidl-1.2.1/src/skidl.egg-info/entry_points.txt
+-rw-rw-r--   0 devb      (1000) devb      (1000)        1 2023-07-16 08:39:20.000000 skidl-1.2.1/src/skidl.egg-info/not-zip-safe
+-rw-rw-r--   0 devb      (1000) devb      (1000)      119 2023-07-26 17:14:01.000000 skidl-1.2.1/src/skidl.egg-info/requires.txt
+-rw-rw-r--   0 devb      (1000) devb      (1000)        6 2023-07-26 17:14:01.000000 skidl-1.2.1/src/skidl.egg-info/top_level.txt
+-rw-rw-r--   0 devb      (1000) devb      (1000)     4346 2023-07-26 17:02:32.000000 skidl-1.2.1/tox.ini
```

### Comparing `skidl-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `skidl-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/.github/ISSUE_TEMPLATE/skidl-feature-request.md` & `skidl-1.2.1/.github/ISSUE_TEMPLATE/skidl-feature-request.md`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/.gitignore` & `skidl-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/.travis.yml` & `skidl-1.2.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/CONTRIBUTING.rst` & `skidl-1.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/HISTORY.rst` & `skidl-1.2.1/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. :changelog:
 
 History
 -------
 
+
+1.2.1 (2023-07-26)
+______________________
+- `is_url` function fixed to solve problems with `search` and loading libraries.
+
+
 1.2.0 (2023-07-14)
 ______________________
 
 - Added ability to generate an editable schematic from a Circuit object. (Currently only works for KiCad V5.)
 - Added Group object for creating hierarchy without using function calls.
 - `generate_pcb` now takes an optional list of footprint library directories.
 - If not explicitly declared, `Part` objects will load the default footprint from their symbol definition.
```

### Comparing `skidl-1.2.0/LICENSE` & `skidl-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/Makefile` & `skidl-1.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/PKG-INFO` & `skidl-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skidl
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python package for textually describing electronic circuit schematics.
 Home-page: https://github.com/devbisme/skidl
 Author: Dave Vandenbout
 Author-email: devb@xess.com
 License: MIT
 Project-URL: Documentation, https://devbisme.github.io/skidl
 Project-URL: Source, https://github.com/devbisme/skidl
@@ -207,14 +207,20 @@
     )
 
 
 
 History
 -------
 
+
+1.2.1 (2023-07-26)
+______________________
+- `is_url` function fixed to solve problems with `search` and loading libraries.
+
+
 1.2.0 (2023-07-14)
 ______________________
 
 - Added ability to generate an editable schematic from a Circuit object. (Currently only works for KiCad V5.)
 - Added Group object for creating hierarchy without using function calls.
 - `generate_pcb` now takes an optional list of footprint library directories.
 - If not explicitly declared, `Part` objects will load the default footprint from their symbol definition.
```

### Comparing `skidl-1.2.0/README.rst` & `skidl-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/icons/part_fp_search_icon.ico` & `skidl-1.2.1/icons/part_fp_search_icon.ico`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/icons/part_fp_search_icon.png` & `skidl-1.2.1/icons/part_fp_search_icon.png`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/icons/part_fp_search_icon_master.svg` & `skidl-1.2.1/icons/part_fp_search_icon_master.svg`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/setup.py` & `skidl-1.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import sys
 
 import setuptools
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 __author__ = "Dave Vandenbout"
 __email__ = "devb@xess.com"
 
 if "sdist" in sys.argv[1:]:
     with open("src/skidl/pckg_info.py", "w") as f:
         for name in ["__version__", "__author__", "__email__"]:
             f.write('{} = "{}"\n'.format(name, locals()[name]))
```

### Comparing `skidl-1.2.0/src/skidl/__init__.py` & `skidl-1.2.1/src/skidl/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,35 +45,31 @@
     search_parts,
     search_parts_iter,
     show,
     show_footprint,
     show_part,
 )
 from .pin import Pin
-from .schlib import SchLib
+from .schlib import SchLib, load_backup_lib
 from .skidl import (
     ERC,
     POWER,
     backup_parts,
+    config,
     empty_footprint_handler,
     erc_assert,
     footprint_search_paths,
     generate_graph,
     generate_netlist,
     generate_pcb,
     generate_schematic,
     generate_svg,
     generate_xml,
-    get_backup_lib,
-    get_default_tool,
-    get_query_backup_lib,
     lib_search_paths,
-    load_backup_lib,
     no_files,
     reset,
-    set_backup_lib,
     set_default_tool,
-    set_query_backup_lib,
 )
 from .tools import KICAD, SKIDL, SPICE, node
+from .utilities import Rgx
 
 standard_library.install_aliases()
```

### Comparing `skidl-1.2.0/src/skidl/alias.py` & `skidl-1.2.1/src/skidl/alias.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/bus.py` & `skidl-1.2.1/src/skidl/bus.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/circuit.py` & `skidl-1.2.1/src/skidl/circuit.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import graphviz
 from future import standard_library
 
 from .bus import Bus
 from .common import builtins
 from .erc import dflt_circuit_erc
 from .group import Group
-from .logger import active_logger, erc_logger
+from .logger import active_logger, erc_logger, stop_log_file_output
 from .net import NCNet, Net
 from .part import Part, PartUnit
 from .pckg_info import __version__
 from .pin import Pin
 from .schlib import SchLib
 from .scriptinfo import get_script_name, get_skidl_trace
 from .skidlbaseobj import SkidlBaseObject
@@ -81,27 +81,33 @@
         # Set passed-in attributes for the circuit.
         for k, v in list(kwargs.items()):
             setattr(self, k, v)
 
     def reset(self, init=False):
         """Clear any circuitry and cached part libraries and start over."""
 
+        try:
+            from . import skidl
+            config = skidl.config
+        except ImportError:
+            # For Python 2. Always gotta be different...
+            from .skidl import config
+
         # Clear circuitry.
         self.mini_reset(init)
 
         # Also clear any cached libraries.
         SchLib.reset()
-        global backup_lib
-        backup_lib = None
+        
+        # Clear out any old backup lib so the new one will get reloaded when it's needed.
+        config.backup_lib = None
 
     def mini_reset(self, init=False):
         """Clear any circuitry but don't erase any loaded part libraries."""
 
-        # Group.reset()
-
         self.group_name_cntr = Counter()
 
         self.name = ""
         self.parts = []
         self.nets = []
         self.netclasses = {}
         self.buses = []
@@ -564,30 +570,30 @@
 
         self._preprocess()
 
         # Extract arguments:
         #     Get EDA tool the netlist will be generated for.
         #     Get file the netlist will be stored in (if any).
         #     Get flag controlling the generation of a backup library.
-        tool = kwargs.pop("tool", skidl.get_default_tool())
+        tool = kwargs.pop("tool", skidl.config.tool)
         file_ = kwargs.pop("file_", None)
         do_backup = kwargs.pop("do_backup", True)
 
         netlist = tool_modules[tool].gen_netlist(self, **kwargs)
 
         active_logger.report_summary("generating netlist")
 
         if not self.no_files:
             with opened(file_ or (get_script_name() + ".net"), "w") as f:
                 f.write(str(netlist))
 
         if do_backup:
             self.backup_parts()  # Create a new backup lib for the circuit parts.
-            global backup_lib  # Clear out any old backup lib so the new one
-            backup_lib = None  #   will get reloaded when it's needed.
+            # Clear out any old backup lib so the new one will get reloaded when it's needed.
+            skidl.config.backup_lib = None
 
         return netlist
 
     def generate_pcb(self, **kwargs):
         """
         Create a PCB file from the circuit.
 
@@ -611,24 +617,24 @@
         self._preprocess()
 
         # Extract arguments:
         #     Get EDA tool the netlist will be generated for.
         #     Get file the netlist will be stored in (if any).
         #     Get flag controlling the generation of a backup library.
         #     Get list of footprint libraries.
-        tool = kwargs.pop("tool", skidl.get_default_tool())
+        tool = kwargs.pop("tool", skidl.config.tool)
         file_ = kwargs.pop("file_", None)
         do_backup = kwargs.pop("do_backup", True)
         fp_libs = kwargs.pop("fp_libs", None)
 
         if not self.no_files:
             if do_backup:
                 self.backup_parts()  # Create a new backup lib for the circuit parts.
-                global backup_lib  # Clear out any old backup lib so the new one
-                backup_lib = None  #   will get reloaded when it's needed.
+                # Clear out any old backup lib so the new one will get reloaded when it's needed.
+                skidl.config.backup_lib = None
             tool_modules[tool].gen_pcb(self, file_, fp_libs=fp_libs)
 
         active_logger.report_summary("creating PCB")
 
     def generate_xml(self, file_=None, tool=None):
         """
         Return netlist as an XML string and also write it to a file/stream.
@@ -647,15 +653,15 @@
 
         # Reset the counters to clear any warnings/errors from previous run.
         active_logger.error.reset()
         active_logger.warning.reset()
 
         self._preprocess()
 
-        tool = tool or skidl.get_default_tool()
+        tool = tool or skidl.config.tool
         netlist = tool_modules[tool].gen_xml(self)
 
         if not self.no_files:
             with opened(file_ or (get_script_name() + ".xml"), "w") as f:
                 f.write(netlist)
 
         active_logger.report_summary("generating XML")
@@ -1024,15 +1030,15 @@
         if kwargs.get("empty_footprint_handler]"):
             skidl.empty_footprint_handler = kwargs["empty_footprint_handler"]
         else:
             skidl.empty_footprint_handler = _empty_footprint_handler
 
         self._preprocess()
 
-        tool = kwargs.pop("tool", skidl.get_default_tool())
+        tool = kwargs.pop("tool", skidl.config.tool)
 
         try:
             tool_modules[tool].gen_schematic(self, **kwargs)
         finally:
             skidl.empty_footprint_handler = save_empty_footprint_handler
 
         active_logger.report_summary("generating schematic")
@@ -1158,11 +1164,21 @@
 
         self._preprocess()
 
         lib = SchLib(tool=SKIDL)  # Create empty library.
         for p in self.parts:
             lib += p
 
-        if not file_:
-            file_ = skidl.BACKUP_LIB_FILE_NAME
+        file_ = file_ or skidl.config.backup_lib_file_name
+
+        lib.export(libname=skidl.config.backup_lib_name, file_=file_)
 
-        lib.export(libname=skidl.BACKUP_LIB_NAME, file_=file_)
+    @property
+    def no_files(self):
+        """Prevent creation of output files (netlists, ERC, logs) by this Circuit object."""
+        return self._no_files
+
+    @no_files.setter
+    def no_files(self, stop):
+        """Don't output any files if stop is True."""
+        self._no_files = stop
+        stop_log_file_output(stop)
```

### Comparing `skidl-1.2.0/src/skidl/config.py` & `skidl-1.2.1/src/skidl/config_.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 import os.path
 from builtins import open, super
 
 from future import standard_library
 
 from .logger import active_logger
 from .part_query import footprint_cache
-from .tools import ALL_TOOLS, KICAD, SKIDL
+from .scriptinfo import get_script_name
+from .tools import ALL_TOOLS, KICAD, SKIDL, lib_suffixes
 from .tools.kicad import get_kicad_lib_tbl_dir
 from .utilities import TriggerDict, export_to_all, merge_dicts
 
 standard_library.install_aliases()
 
 
 @export_to_all
@@ -34,14 +35,26 @@
     """Class for handling configuration parameters."""
 
     def __init__(self, cfg_file_name, *dirs):
         super().__init__()
         self.cfg_file_name = cfg_file_name
         self.load(*dirs)
 
+    def __getattr__(self, key):
+        """Get the value of a Config attribute or else from the Config dictionary."""
+        try:
+            return self[key]
+        except KeyError:
+            raise AttributeError
+        
+    def __setattr__(self, key, value):
+        """Set the value of both a Config attribute and a Config dictionary entry."""
+        self.__dict__[key] = value
+        self[key] = value
+
     def merge(self, merge_dct):
         """Recurse through both dicts and updates keys."""
         for k, v in list(merge_dct.items()):
             if (
                 k in self
                 and isinstance(self[k], dict)
                 and isinstance(merge_dct[k], collections.Mapping)
@@ -74,14 +87,18 @@
 @export_to_all
 class SkidlConfig(Config):
     """Config specialized for SKiDL configuration files."""
 
     def __init__(self):
         super().__init__(".skidlcfg", "/etc", "~", ".")
 
+        # If no configuration files were found, set default backend/tool.
+        if "tool" not in self:
+            self.tool = KICAD
+
         # If no configuration files were found, set some default lib search paths.
         if "lib_search_paths" not in self:
 
             # No lib search paths, so start with the current directory for all tools.
             self["lib_search_paths"] = {tool: ["."] for tool in ALL_TOOLS}
 
             # Add the location of the default KiCad part libraries.
@@ -94,14 +111,24 @@
 
             # Add the location of the default SKiDL part libraries.
             default_skidl_libs = os.path.join(
                 os.path.dirname(os.path.abspath(__file__)), "libs"
             )
             self["lib_search_paths"][SKIDL].append(default_skidl_libs)
 
+        # If no configuration files were found, set base name of default backup part library.
+        if "backup_lib_name" not in self:
+            self.backup_lib_name = get_script_name() + "_lib"
+        if "backup_lib_file_name" not in self:
+            self.backup_lib_file_name = self.backup_lib_name + lib_suffixes[SKIDL]
+        if "query_backup_lib" not in self:
+            self.query_backup_lib = True
+        if "backup_lib" not in self:
+            self.backup_lib = None
+
         # If no configuration files were found, set some default footprint search paths.
         if "footprint_search_paths" not in self:
             dir_ = get_kicad_lib_tbl_dir()
             self["footprint_search_paths"] = {tool: [dir_] for tool in ALL_TOOLS}
 
         # Cause the footprint cache to be invalidated if the footprint search path changes.
         def invalidate_footprint_cache(self, k, v):
```

### Comparing `skidl-1.2.0/src/skidl/erc.py` & `skidl-1.2.1/src/skidl/erc.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/group.py` & `skidl-1.2.1/src/skidl/group.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/interface.py` & `skidl-1.2.1/src/skidl/interface.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/74xgxx_sklib.py` & `skidl-1.2.1/src/skidl/libs/74xgxx_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/74xx_sklib.py` & `skidl-1.2.1/src/skidl/libs/74xx_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/Altera_sklib.py` & `skidl-1.2.1/src/skidl/libs/Altera_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/ESD_Protection_sklib.py` & `skidl-1.2.1/src/skidl/libs/ESD_Protection_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/LEM_sklib.py` & `skidl-1.2.1/src/skidl/libs/LEM_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/Lattice_sklib.py` & `skidl-1.2.1/src/skidl/libs/Lattice_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/NXP_sklib.py` & `skidl-1.2.1/src/skidl/libs/NXP_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/Oscillators_sklib.py` & `skidl-1.2.1/src/skidl/libs/Oscillators_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/Power_Management_sklib.py` & `skidl-1.2.1/src/skidl/libs/Power_Management_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/RFSolutions_sklib.py` & `skidl-1.2.1/src/skidl/libs/RFSolutions_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/Worldsemi_sklib.py` & `skidl-1.2.1/src/skidl/libs/Worldsemi_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/Xicor_sklib.py` & `skidl-1.2.1/src/skidl/libs/Xicor_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/Zilog_sklib.py` & `skidl-1.2.1/src/skidl/libs/Zilog_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/ac-dc_sklib.py` & `skidl-1.2.1/src/skidl/libs/ac-dc_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/actel_sklib.py` & `skidl-1.2.1/src/skidl/libs/actel_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/adc-dac_sklib.py` & `skidl-1.2.1/src/skidl/libs/adc-dac_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/allegro_sklib.py` & `skidl-1.2.1/src/skidl/libs/allegro_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/analog_devices_sklib.py` & `skidl-1.2.1/src/skidl/libs/analog_devices_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/analog_switches_sklib.py` & `skidl-1.2.1/src/skidl/libs/analog_switches_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/atmel_sklib.py` & `skidl-1.2.1/src/skidl/libs/atmel_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/audio_sklib.py` & `skidl-1.2.1/src/skidl/libs/audio_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/battery_management_sklib.py` & `skidl-1.2.1/src/skidl/libs/battery_management_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/bbd_sklib.py` & `skidl-1.2.1/src/skidl/libs/bbd_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/bosch_sklib.py` & `skidl-1.2.1/src/skidl/libs/bosch_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/brooktre_sklib.py` & `skidl-1.2.1/src/skidl/libs/brooktre_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/cmos4000_sklib.py` & `skidl-1.2.1/src/skidl/libs/cmos4000_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/cmos_ieee_sklib.py` & `skidl-1.2.1/src/skidl/libs/cmos_ieee_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/conn_sklib.py` & `skidl-1.2.1/src/skidl/libs/conn_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/contrib_sklib.py` & `skidl-1.2.1/src/skidl/libs/contrib_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/convert_libs.py` & `skidl-1.2.1/src/skidl/libs/convert_libs.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/cypress_sklib.py` & `skidl-1.2.1/src/skidl/libs/cypress_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/dc-dc_sklib.py` & `skidl-1.2.1/src/skidl/libs/dc-dc_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/device_sklib.py` & `skidl-1.2.1/src/skidl/libs/device_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/digital-audio_sklib.py` & `skidl-1.2.1/src/skidl/libs/digital-audio_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/diode_sklib.py` & `skidl-1.2.1/src/skidl/libs/diode_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/display_sklib.py` & `skidl-1.2.1/src/skidl/libs/display_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/dsp_sklib.py` & `skidl-1.2.1/src/skidl/libs/dsp_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/elec-unifil_sklib.py` & `skidl-1.2.1/src/skidl/libs/elec-unifil_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/ftdi_sklib.py` & `skidl-1.2.1/src/skidl/libs/ftdi_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/gennum_sklib.py` & `skidl-1.2.1/src/skidl/libs/gennum_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/graphic_sklib.py` & `skidl-1.2.1/src/skidl/libs/graphic_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/hc11_sklib.py` & `skidl-1.2.1/src/skidl/libs/hc11_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/intel_sklib.py` & `skidl-1.2.1/src/skidl/libs/intel_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/interface_sklib.py` & `skidl-1.2.1/src/skidl/libs/interface_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/intersil_sklib.py` & `skidl-1.2.1/src/skidl/libs/intersil_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/ir_sklib.py` & `skidl-1.2.1/src/skidl/libs/ir_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/leds_sklib.py` & `skidl-1.2.1/src/skidl/libs/leds_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/linear_sklib.py` & `skidl-1.2.1/src/skidl/libs/linear_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/maxim_sklib.py` & `skidl-1.2.1/src/skidl/libs/maxim_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/mechanical_sklib.py` & `skidl-1.2.1/src/skidl/libs/mechanical_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/memory_sklib.py` & `skidl-1.2.1/src/skidl/libs/memory_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/microchip_dspic33dsc_sklib.py` & `skidl-1.2.1/src/skidl/libs/microchip_dspic33dsc_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/microchip_pic10mcu_sklib.py` & `skidl-1.2.1/src/skidl/libs/microchip_pic10mcu_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/microchip_pic12mcu_sklib.py` & `skidl-1.2.1/src/skidl/libs/microchip_pic12mcu_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/microchip_pic16mcu_sklib.py` & `skidl-1.2.1/src/skidl/libs/microchip_pic16mcu_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/microchip_pic18mcu_sklib.py` & `skidl-1.2.1/src/skidl/libs/microchip_pic18mcu_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/microchip_pic24mcu_sklib.py` & `skidl-1.2.1/src/skidl/libs/microchip_pic24mcu_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/microchip_pic32mcu_sklib.py` & `skidl-1.2.1/src/skidl/libs/microchip_pic32mcu_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/microchip_sklib.py` & `skidl-1.2.1/src/skidl/libs/microchip_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/microcontrollers_sklib.py` & `skidl-1.2.1/src/skidl/libs/microcontrollers_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/modules_sklib.py` & `skidl-1.2.1/src/skidl/libs/modules_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/motor_drivers_sklib.py` & `skidl-1.2.1/src/skidl/libs/motor_drivers_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/motorola_sklib.py` & `skidl-1.2.1/src/skidl/libs/motorola_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/motors_sklib.py` & `skidl-1.2.1/src/skidl/libs/motors_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/msp430_sklib.py` & `skidl-1.2.1/src/skidl/libs/msp430_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/nordicsemi_sklib.py` & `skidl-1.2.1/src/skidl/libs/nordicsemi_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/nxp_armmcu_sklib.py` & `skidl-1.2.1/src/skidl/libs/nxp_armmcu_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/onsemi_sklib.py` & `skidl-1.2.1/src/skidl/libs/onsemi_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/opto_sklib.py` & `skidl-1.2.1/src/skidl/libs/opto_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/philips_sklib.py` & `skidl-1.2.1/src/skidl/libs/philips_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/power_sklib.py` & `skidl-1.2.1/src/skidl/libs/power_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/powerint_sklib.py` & `skidl-1.2.1/src/skidl/libs/powerint_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/pspice_sklib.py` & `skidl-1.2.1/src/skidl/libs/pspice_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/pyspice_sklib.py` & `skidl-1.2.1/src/skidl/libs/pyspice_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/references_sklib.py` & `skidl-1.2.1/src/skidl/libs/references_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/regul_sklib.py` & `skidl-1.2.1/src/skidl/libs/regul_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/relays_sklib.py` & `skidl-1.2.1/src/skidl/libs/relays_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/rfcom_sklib.py` & `skidl-1.2.1/src/skidl/libs/rfcom_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/sensors_sklib.py` & `skidl-1.2.1/src/skidl/libs/sensors_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/silabs_sklib.py` & `skidl-1.2.1/src/skidl/libs/silabs_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/siliconi_sklib.py` & `skidl-1.2.1/src/skidl/libs/siliconi_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/skidl_lib_sklib.py` & `skidl-1.2.1/src/skidl/libs/skidl_lib_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/stm32_sklib.py` & `skidl-1.2.1/src/skidl/libs/stm32_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/stm8_sklib.py` & `skidl-1.2.1/src/skidl/libs/stm8_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/supertex_sklib.py` & `skidl-1.2.1/src/skidl/libs/supertex_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/switches_sklib.py` & `skidl-1.2.1/src/skidl/libs/switches_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/texas_sklib.py` & `skidl-1.2.1/src/skidl/libs/texas_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/transf_sklib.py` & `skidl-1.2.1/src/skidl/libs/transf_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/transistors_sklib.py` & `skidl-1.2.1/src/skidl/libs/transistors_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/triac_thyristor_sklib.py` & `skidl-1.2.1/src/skidl/libs/triac_thyristor_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/ttl_ieee_sklib.py` & `skidl-1.2.1/src/skidl/libs/ttl_ieee_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/valves_sklib.py` & `skidl-1.2.1/src/skidl/libs/valves_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/video_sklib.py` & `skidl-1.2.1/src/skidl/libs/video_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/wiznet_sklib.py` & `skidl-1.2.1/src/skidl/libs/wiznet_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/xilinx_sklib.py` & `skidl-1.2.1/src/skidl/libs/xilinx_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/libs/zetex_sklib.py` & `skidl-1.2.1/src/skidl/libs/zetex_sklib.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/logger.py` & `skidl-1.2.1/src/skidl/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,18 +224,19 @@
     logger.error = CountCalls(logger.error)
     logger.warning = CountCalls(logger.warning)
 
     return logger
 
 
 @export_to_all
-def stop_log_file_output():
-    """Stop loggers from creating files containing log messages."""
-    rt_logger.stop_file_output()
-    erc_logger.stop_file_output()
+def stop_log_file_output(stop=True):
+    """Permanently stop loggers from creating files containing log messages."""
+    if stop:
+        rt_logger.stop_file_output()
+        erc_logger.stop_file_output()
 
 
 ###############################################################################
 
 # Create loggers for runtime messages and ERC reports.
 rt_logger = _create_logger("skidl")
 rt_logger.set_trace_depth(2)
```

### Comparing `skidl-1.2.0/src/skidl/net.py` & `skidl-1.2.1/src/skidl/net.py`

 * *Files 1% similar despite different names*

```diff
@@ -659,15 +659,15 @@
             tool: The format for the netlist file (e.g., KICAD).
         """
 
         import skidl
 
         from .tools import tool_modules
 
-        tool = tool or skidl.get_default_tool()
+        tool = tool or skidl.config.tool
 
         self.test_validity()
 
         # Don't add anything to the netlist if no pins are on this net.
         if not self.pins:
             return
 
@@ -681,15 +681,15 @@
             tool: The format for the XML file (e.g., KICAD).
         """
 
         import skidl
 
         from .tools import tool_modules
 
-        tool = tool or skidl.get_default_tool()
+        tool = tool or skidl.config.tool
 
         self.test_validity()
 
         # Don't add anything to the XML if no pins are on this net.
         if not self.pins:
             return
 
@@ -898,20 +898,14 @@
 
         super().__init__(name=name, circuit=circuit, *pins_nets_buses, **attribs)
         self._drive = Pin.drives.NOCONNECT
         self.do_erc = False  # No need to do ERC on no-connect nets.
 
     def generate_netlist_net(self, tool=None):
         """NO_CONNECT nets don't generate anything for netlists."""
-
-        import skidl
-
-        if tool is None:
-            tool = skidl.get_default_tool()
-
         return ""
 
     @property
     def drive(self):
         """
         Get the drive strength of this net.
```

### Comparing `skidl-1.2.0/src/skidl/netclass.py` & `skidl-1.2.1/src/skidl/netclass.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/netlist_to_skidl.py` & `skidl-1.2.1/src/skidl/netlist_to_skidl.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/netpinlist.py` & `skidl-1.2.1/src/skidl/netpinlist.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/network.py` & `skidl-1.2.1/src/skidl/network.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/note.py` & `skidl-1.2.1/src/skidl/note.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/package.py` & `skidl-1.2.1/src/skidl/package.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/part.py` & `skidl-1.2.1/src/skidl/part.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     find_num_copies,
     flatten,
     from_iadd,
     get_unique_name,
     list_or_scalar,
     rmv_iadd,
     to_list,
+    Rgx,
 )
 
 standard_library.install_aliases()
 
 __all__ = ["NETLIST", "LIBRARY", "TEMPLATE", "PartTmplt"]
 
 
@@ -162,16 +163,15 @@
         import skidl
 
         from .schlib import SchLib
         from .tools import SKIDL, add_xspice_io
 
         super().__init__()
 
-        if tool is None:
-            tool = skidl.get_default_tool()
+        tool = tool or skidl.config.tool
 
         # Setup some part attributes that might be overwritten later on.
         self.do_erc = True  # Allow part to be included in ERC.
         self.unit = {}  # Dictionary for storing subunits of the part, if desired.
         self.pins = []  # Start with no pins, but a place to store them.
         self.p = PinNumberSearch(self)  # Does pin search using only pin numbers.
         self.n = PinNameSearch(self)  # Does pin search using only pin names.
@@ -186,15 +186,15 @@
             # If the lib argument is a string, then create a library using the
             # string as the library file name.
             if isinstance(lib, basestring):
                 libname = lib
                 try:
                     lib = SchLib(filename=libname, tool=tool)
                 except FileNotFoundError as e:
-                    if skidl.get_query_backup_lib():
+                    if skidl.config.query_backup_lib:
                         active_logger.warning(
                             'Could not load KiCad schematic library "{}", falling back to backup library.'.format(
                                 libname
                             )
                         )
                         lib = skidl.load_backup_lib()
                         if not lib:
@@ -671,16 +671,15 @@
 
         # Extract permission to search for regex matches in pin names/aliases.
         match_regex = criteria.pop("match_regex", False) or self.match_pin_regex
 
         # If no pin identifiers were given, then use a wildcard that will
         # select all pins.
         if not pin_ids:
-            pin_ids = [".*"]
-            match_regex = True
+            pin_ids = [Rgx(".*")]
 
         # Determine the minimum and maximum pin ids if they don't already exist.
         if "min_pin" not in dir(self) or "max_pin" not in dir(self):
             self.min_pin, self.max_pin = self._find_min_max_pins()
 
         # Go through the list of pin IDs one-by-one.
         pins = NetPinList()
@@ -1011,15 +1010,15 @@
             tool: The format for the netlist file (e.g., KICAD).
         """
 
         import skidl
 
         from .tools import tool_modules
 
-        tool = tool or skidl.get_default_tool()
+        tool = tool or skidl.config.tool
 
         # Create part value as a string so including it in netlist isn't a problem.
         self.value_str = self._value_to_str()
 
         return tool_modules[tool].gen_netlist_comp(self)
 
     def generate_xml_component(self, tool=None):
@@ -1030,15 +1029,15 @@
             tool: The format for the XML file (e.g., KICAD).
         """
 
         import skidl
 
         from .tools import tool_modules
 
-        tool = tool or skidl.get_default_tool()
+        tool = tool or skidl.config.tool
 
         # Create part value as a string so including it in XML isn't a problem.
         self.value_str = self._value_to_str()
 
         return tool_modules[tool].gen_xml_comp(self)
 
     def generate_svg_component(self, symtx="", tool=None, net_stubs=None):
@@ -1046,15 +1045,15 @@
         Generate the SVG for displaying a part in an SVG schematic.
         """
 
         import skidl
 
         from .tools import tool_modules
 
-        tool = tool or skidl.get_default_tool()
+        tool = tool or skidl.config.tool
 
         return tool_modules[tool].gen_svg_comp(self, symtx=symtx, net_stubs=net_stubs)
 
     def erc_desc(self):
         """Create description of part for ERC and other error reporting."""
         return "{p.name}/{p.ref}".format(p=self)
```

### Comparing `skidl-1.2.0/src/skidl/part_query.py` & `skidl-1.2.1/src/skidl/part_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,15 @@
     """Return a list of (lib, part) sequences that match a regex term."""
 
     import skidl
     import skidl.tools
 
     from .schlib import SchLib
 
-    if tool is None:
-        tool = skidl.get_default_tool()
+    tool = tool or skidl.config.tool
 
     terms = parse_search_terms(terms)
 
     def mk_list(l):
         """Make a list out of whatever is given."""
         if isinstance(l, (list, tuple)):
             return l
@@ -158,16 +157,16 @@
         A Part object.
     """
 
     import skidl
 
     from .part import TEMPLATE, Part
 
-    if tool is None:
-        tool = skidl.get_default_tool()
+    tool = tool or skidl.config.tool
+
     try:
         return Part(lib, re.escape(part_name), tool=tool, dest=TEMPLATE)
     except Exception:
         return None
 
 
 class FootprintCache(dict):
@@ -286,16 +285,15 @@
 
 @export_to_all
 def search_footprints_iter(terms, tool=None):
     """Return a list of (lib, footprint) sequences that match a regex term."""
 
     import skidl
 
-    if tool is None:
-        tool = skidl.get_default_tool()
+    tool = tool or skidl.config.tool
 
     terms = parse_search_terms(terms)
 
     # If the cache isn't valid, then make it valid by gathering all the
     # footprint files from all the directories in the search paths.
     if not footprint_cache.valid:
         footprint_cache.clear()
@@ -412,16 +410,15 @@
 
     Returns:
         A Part object.
     """
 
     import skidl
 
-    if tool is None:
-        tool = skidl.get_default_tool()
+    tool = tool or skidl.config.tool
 
     os.environ["KISYSMOD"] = os.pathsep.join(skidl.footprint_search_paths[tool])
     return pym.Module.from_library(lib, module_name)
 
 
 # Define some shortcuts.
 search = search_parts
```

### Comparing `skidl-1.2.0/src/skidl/pin.py` & `skidl-1.2.1/src/skidl/pin.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/protonet.py` & `skidl-1.2.1/src/skidl/protonet.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/pyspice.py` & `skidl-1.2.1/src/skidl/pyspice.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/schematics/debug_draw.py` & `skidl-1.2.1/src/skidl/schematics/debug_draw.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/schematics/gen_schematic.py` & `skidl-1.2.1/src/skidl/schematics/gen_schematic.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/schematics/geometry.py` & `skidl-1.2.1/src/skidl/schematics/geometry.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/schematics/place.py` & `skidl-1.2.1/src/skidl/schematics/place.py`

 * *Files 0% similar despite different names*

```diff
@@ -1470,15 +1470,15 @@
             options (dict): Dictionary of options and values to control placement.
         """
 
         # Inject the constants for the backend tool into this module.
         import skidl
         from skidl.tools import tool_modules
 
-        tool = tool or skidl.get_default_tool()
+        tool = tool or skidl.config.tool
         this_module = sys.modules[__name__]
         this_module.__dict__.update(tool_modules[tool].constants.__dict__)
 
         random.seed(options.get("seed"))
 
         # Store the starting attributes of the node's parts, pins, and nets.
         node.attrs = node.get_attrs()
```

### Comparing `skidl-1.2.0/src/skidl/schematics/route.py` & `skidl-1.2.1/src/skidl/schematics/route.py`

 * *Files 0% similar despite different names*

```diff
@@ -3136,15 +3136,15 @@
                 "draw_switchbox", "draw_routing", "draw_channels"
         """
 
         # Inject the constants for the backend tool into this module.
         import skidl
         from skidl.tools import tool_modules
 
-        tool = tool or skidl.get_default_tool()
+        tool = tool or skidl.config.tool
         this_module = sys.modules[__name__]
         this_module.__dict__.update(tool_modules[tool].constants.__dict__)
 
         random.seed(options.get("seed"))
 
         # Remove any stuff leftover from a previous place & route run.
         node.rmv_routing_stuff()
```

### Comparing `skidl-1.2.0/src/skidl/schlib.py` & `skidl-1.2.1/src/skidl/schlib.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from .utilities import (
     cnvt_to_var_name,
     export_to_all,
     filter_list,
     flatten,
     list_or_scalar,
     opened,
+    norecurse,
 )
 
 standard_library.install_aliases()
 
 
 @export_to_all
 class SchLib(object):
@@ -58,16 +59,15 @@
         Load the parts from a library file.
         """
 
         import skidl
 
         from .tools import tool_modules
 
-        if tool is None:
-            tool = skidl.get_default_tool()
+        tool = tool or skidl.config.tool
 
         # Library starts off empty of parts.
         self.parts = []
 
         # Attach attributes to the library.
         for k, v in list(attribs.items()):
             setattr(self, k, v)
@@ -133,22 +133,21 @@
                 the attribute name while the argument contains the desired value
                 of the attribute.
 
         Returns:
             A list of Parts that match all the criteria.
         """
 
-        from .skidl import get_query_backup_lib, load_backup_lib
+        import skidl
 
         parts = filter_list(self.parts, **criteria)
-        if not parts and use_backup_lib and get_query_backup_lib():
-            # if not parts and use_backup_lib and skidl.QUERY_BACKUP_LIB:
+        if not parts and use_backup_lib and skidl.config.query_backup_lib:
             try:
-                backup_lib_ = load_backup_lib()
-                parts = backup_lib_.get_parts(use_backup_lib=False, **criteria)
+                backup_lib = load_backup_lib()
+                parts = backup_lib.get_parts(use_backup_lib=False, **criteria)
             except AttributeError:
                 pass
         return parts
 
     def get_parts_quick(self, name):
         """Do a quick search for a part name or alias."""
         return [prt for prt in self.parts if prt.aliases == name]
@@ -255,7 +254,28 @@
             f.write(export_str)
 
     def __len__(self):
         """
         Return number of parts in library.
         """
         return len(self.parts)
+
+
+@export_to_all
+@norecurse
+def load_backup_lib():
+    """Load a backup library that stores the parts used in the circuit."""
+
+    from . import skidl
+
+    # Don't keep reloading the backup library once it's loaded.
+    if not skidl.config.backup_lib:
+        try:
+            # The backup library is a SKiDL lib stored as a Python module.
+            exec(open(skidl.config.backup_lib_file_name).read())
+            # Copy the backup library in the local storage to the global storage.
+            skidl.config.backup_lib = locals()[skidl.config.backup_lib_name]
+
+        except (FileNotFoundError, ImportError, NameError, IOError):
+            pass
+
+    return skidl.config.backup_lib
```

### Comparing `skidl-1.2.0/src/skidl/scriptinfo.py` & `skidl-1.2.1/src/skidl/scriptinfo.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/scripts/netlist_to_skidl_main.py` & `skidl-1.2.1/src/skidl/scripts/netlist_to_skidl_main.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/skidlbaseobj.py` & `skidl-1.2.1/src/skidl/skidlbaseobj.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/tools/__init__.py` & `skidl-1.2.1/src/skidl/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/tools/kicad/eeschema_v5.py` & `skidl-1.2.1/src/skidl/tools/kicad/eeschema_v5.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/tools/kicad/kicad.py` & `skidl-1.2.1/src/skidl/tools/kicad/kicad.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/tools/kicad/v5.py` & `skidl-1.2.1/src/skidl/tools/kicad/v5.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/tools/kicad/v6.py` & `skidl-1.2.1/src/skidl/tools/kicad/v6.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/tools/skidl/skidl.py` & `skidl-1.2.1/src/skidl/tools/skidl/skidl.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/tools/spice/spice.py` & `skidl-1.2.1/src/skidl/tools/spice/spice.py`

 * *Files identical despite different names*

### Comparing `skidl-1.2.0/src/skidl/utilities.py` & `skidl-1.2.1/src/skidl/utilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 import collections
 import os
 import os.path
 import re
 import sys
 import traceback
+import urllib.parse
+import urllib.request
 from builtins import chr, dict, int, open, range, str, super
 from collections import namedtuple
 from contextlib import contextmanager
 
 __all__ = ["INDEX_SEPARATOR"]
 
 
@@ -47,28 +49,36 @@
     if hasattr(mod, "__all__"):
         mod.__all__.append(fn.__name__)
     else:
         mod.__all__ = [fn.__name__]
     return fn
 
 
+class Rgx(str):
+    """Same as a string but the class makes it recognizable as as a regular expression."""
+
+    def __init__(self, s):
+        str.__init__(s)
+
+
 @export_to_all
 def sgn(x):
     """Return -1,0,1 if x<0, x==0, x>0."""
     return -1 if x < 0 else (1 if x > 0 else 0)
 
 
 @export_to_all
 def debug_trace(fn, *args, **kwargs):
     """Decorator to print tracing info when debugging execution."""
 
     def traced_fn(*args, **kwargs):
         if kwargs.get("debug_trace"):
             print("Doing {} ...".format(fn.__name__))
         return fn(*args, **kwargs)
+
     return traced_fn
 
 
 @export_to_all
 def num_to_chars(num):
     """Return a string like 'AB' when given a number like 28."""
     num -= 1
@@ -122,15 +132,15 @@
 
 
 @export_to_all
 def to_list(x):
     """
     Return x if it is already a list, or return a list containing x if x is a scalar.
     """
-    if isinstance(x, (list, tuple)):
+    if isinstance(x, (list, tuple, set)):
         return x  # Already a list, so just return it.
     return [x]  # Wasn't a list, so make it into one.
 
 
 @export_to_all
 def list_or_scalar(lst):
     """
@@ -309,15 +319,14 @@
 
     # Get the unique names used in the list.
     unique_names = set([getattr(l, attrib, None) for l in lst])
 
     # If the initial name is None, then create a name based on the prefix
     # and the smallest unused number that's available for that prefix.
     if not name:
-
         # Do a binary search for a unique name formed from the prefix + number.
         n = 1  # Starting number to append to the prefix.
         while True:
             # Step forward in larger and larger increments looking for a name
             # that isn't in the list.
             step = 1
             while prefix + str(n) in unique_names:
@@ -416,62 +425,66 @@
     extract = []
 
     for item in lst:
         # Compare an item's attributes to each of the criteria.
         # Break current_level of the criteria loop and don't add the item to the extract
         # list if *any* of the item's attributes *does not* match.
         for k, v in list(criteria.items()):
-
             try:
-                attr_val = getattr(item, k)
+                attr_val = to_list(getattr(item, k))
             except AttributeError:
                 # If the attribute doesn't exist, then that's a non-match.
                 break
 
-            if isinstance(v, (int, basestring)):
-                # Check integer or string attributes.
-
-                if isinstance(attr_val, (list, tuple, set)):
-                    # If the attribute value from the item is a list or tuple,
-                    # loop through the list of attribute values. If at least one
-                    # value matches the current criterium, then break from the
-                    # criteria loop and extract this item.
-                    for val in attr_val:
-                        if compare_func(
-                            str(v),
-                            str(val),
-                            flags=re.IGNORECASE | re.MULTILINE | re.DOTALL,
-                        ):
-                            # One of the list of values matched, so break from this
-                            # loop and do not execute the break in the
-                            # loop's else clause.
-                            break
-                    else:
-                        # If we got here, then none of the values in the attribute
-                        # list matched the current criterium. Therefore, break current_level
-                        # of the criteria loop and don't add this list item to
-                        # the extract list.
+            if isinstance(v, Rgx):
+                # Loop through the list of attribute values. If at least one
+                # value matches the current criterium, then break from the
+                # criteria loop and extract this item.
+                for val in attr_val:
+                    # This is an Rgx, so use fullmatch().
+                    if fullmatch(
+                        str(v),
+                        str(val),
+                        flags=re.IGNORECASE | re.MULTILINE | re.DOTALL,
+                    ):
+                        # One of the list of values matched, so break from this
+                        # loop and do not execute the break in the
+                        # loop's else clause.
                         break
                 else:
-                    # If the attribute value from the item in the list is a scalar,
-                    # see if the value matches the current criterium. If it doesn't,
-                    # then break from the criteria loop and don't extract this item.
-                    if not compare_func(
+                    # If we got here, then none of the values in the attribute
+                    # list matched the current criterium. Therefore, break current_level
+                    # of the criteria loop and don't add this list item to
+                    # the extract list.
+                    break
+
+            elif isinstance(v, (int, basestring)):
+                # Loop through the list of attribute values. If at least one
+                # value matches the current criterium, then break from the
+                # criteria loop and extract this item.
+                for val in attr_val:
+                    if compare_func(
                         str(v),
-                        str(attr_val),
+                        str(val),
                         flags=re.IGNORECASE | re.MULTILINE | re.DOTALL,
                     ):
+                        # One of the list of values matched, so break from this
+                        # loop and do not execute the break in the
+                        # loop's else clause.
                         break
+                else:
+                    # If we got here, then none of the values in the attribute
+                    # list matched the current criterium. Therefore, break current_level
+                    # of the criteria loop and don't add this list item to
+                    # the extract list.
+                    break
 
             else:
                 # Check non-integer, non-string attributes.
-                if isinstance(attr_val, (list, tuple)):
-                    if v not in attr_val:
-                        break
-                elif v != attr_val:
+                if v not in attr_val:
                     break
 
         else:
             # If we get here, then all the item attributes matched and the
             # for criteria loop didn't break, so add this item to the
             # extract list.
             extract.append(item)
@@ -596,14 +609,21 @@
     # Expand each index and add it to the list.
     ids = []
     for indx in flatten(indices):
         if isinstance(indx, slice):
             ids.extend(expand_slice(indx))
         elif isinstance(indx, int):
             ids.append(indx)
+        elif isinstance(indx, Rgx):
+            # Rgx might contain multiple indices with a separator.
+            for id in re.split(INDEX_SEPARATOR, indx):
+                # If the id is a valid bus expression, then the exploded bus lines
+                # are added to the list of ids. If not, the original id is
+                # added to the list.
+                ids.extend((Rgx(i) for i in explode(id.strip())))
         elif isinstance(indx, basestring):
             # String might contain multiple indices with a separator.
             for id in re.split(INDEX_SEPARATOR, indx):
                 # If the id is a valid bus expression, then the exploded bus lines
                 # are added to the list of ids. If not, the original id is
                 # added to the list.
                 ids.extend(explode(id.strip()))
@@ -724,14 +744,18 @@
     try:
         with open(filename, "rb") as fp:
             return bool(fp.read(1024).translate(None, text_chars))
     except (IOError, FileNotFoundError, TypeError):
         return False
 
 
+def is_url(s):
+    return urllib.parse.urlparse(s).scheme in {"http", "https"}
+
+
 @export_to_all
 def find_and_open_file(
     filename, paths=None, ext=None, allow_failure=False, exclude_binary=False, descend=0
 ):
     """
     Search for a file in list of paths, open it and return file pointer and full file name.
 
@@ -745,22 +769,16 @@
                  that many levels down for the file. If negative, descend into
                  subdirectories withcurrent_level limit.
 
     Returns:
         File pointer and file name or None, None if file could not be opened.
     """
 
-    import urllib.parse
-    import urllib.request
-
     from .logger import active_logger
 
-    def is_url(s):
-        return bool(urllib.parse.urlparse(s).scheme)
-
     if is_url(filename):
         # This is a URL. Use the URL path as the search path except for
         # the ending file name. Maybe not the best thing to use, but
         # os.path.dirname() will do this.
         paths = [os.path.dirname(filename)]
     elif os.path.isabs(filename):
         # Replace search paths if the file already has an absolute path.
```

### Comparing `skidl-1.2.0/src/skidl.egg-info/PKG-INFO` & `skidl-1.2.1/src/skidl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skidl
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python package for textually describing electronic circuit schematics.
 Home-page: https://github.com/devbisme/skidl
 Author: Dave Vandenbout
 Author-email: devb@xess.com
 License: MIT
 Project-URL: Documentation, https://devbisme.github.io/skidl
 Project-URL: Source, https://github.com/devbisme/skidl
@@ -207,14 +207,20 @@
     )
 
 
 
 History
 -------
 
+
+1.2.1 (2023-07-26)
+______________________
+- `is_url` function fixed to solve problems with `search` and loading libraries.
+
+
 1.2.0 (2023-07-14)
 ______________________
 
 - Added ability to generate an editable schematic from a Circuit object. (Currently only works for KiCad V5.)
 - Added Group object for creating hierarchy without using function calls.
 - `generate_pcb` now takes an optional list of footprint library directories.
 - If not explicitly declared, `Part` objects will load the default footprint from their symbol definition.
```

### Comparing `skidl-1.2.0/src/skidl.egg-info/SOURCES.txt` & `skidl-1.2.1/src/skidl.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 icons/part_fp_search_icon.png
 icons/part_fp_search_icon_master.svg
 src/skidl/__init__.py
 src/skidl/alias.py
 src/skidl/bus.py
 src/skidl/circuit.py
 src/skidl/common.py
-src/skidl/config.py
+src/skidl/config_.py
 src/skidl/erc.py
 src/skidl/group.py
 src/skidl/interface.py
 src/skidl/logger.py
 src/skidl/net.py
 src/skidl/netclass.py
 src/skidl/netlist_to_skidl.py
```

### Comparing `skidl-1.2.0/tox.ini` & `skidl-1.2.1/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -16,30 +16,47 @@
     3.8: py38
     3.9: py39
     3.10: py310
     3.11: py311
 
 
 [pytest]
-markers = spice: Run unit tests that use SPICE.
+markers = 
+    spice: Unit tests that use SPICE.
 
 
 [testenv:py{27,36,37,38,39,310,311}]
-description = test everything except SKiDL SPICE functions
+description = test everything except SKiDL SPICE functions and schematic generation
 isolated_build = True
 setenv = TOXINIDIR = {toxinidir}
 passenv = *
 extras = testing
 deps =
     pytest
     kinparse >= 0.1.0
 changedir = {toxinidir}/tests
 commands =
     pip install -e {toxinidir}
-    py.test --ignore {toxinidir}/tests/examples -m "not spice" --tb=short --color=yes
+    py.test --ignore {toxinidir}/tests/examples -m "not spice" -k "not gen_" --tb=short --color=yes
+
+
+[testenv:generate]
+basepython = python3.10
+description = test schematic generation
+isolated_build = True
+setenv = TOXINIDIR = {toxinidir}
+passenv = *
+extras = testing
+deps =
+    pytest
+    kinparse >= 0.1.0
+changedir = {toxinidir}/tests
+commands =
+    pip install -e {toxinidir}
+    py.test --ignore {toxinidir}/tests/examples -m "not spice" -k "gen_" --tb=short --color=yes
 
 
 [testenv:spice]
 basepython = python3.10
 description = test SKiDL SPICE functions
 isolated_build = True
 setenv = TOXINIDIR = {toxinidir}
```


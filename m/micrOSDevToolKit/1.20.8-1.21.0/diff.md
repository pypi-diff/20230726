# Comparing `tmp/micrOSDevToolKit-1.20.8.tar.gz` & `tmp/micrOSDevToolKit-1.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/micrOSDevToolKit-1.20.8.tar", last modified: Wed Jul 26 12:03:05 2023, max compression
+gzip compressed data, was "dist/micrOSDevToolKit-1.21.0.tar", last modified: Wed Jul 26 14:54:48 2023, max compression
```

## Comparing `micrOSDevToolKit-1.20.8.tar` & `micrOSDevToolKit-1.21.0.tar`

### file list

```diff
@@ -1,253 +1,253 @@
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.173428 micrOSDevToolKit-1.20.8/
--rw-r--r--   0 bnm        (501) staff       (20)      333 2023-07-18 21:54:39.000000 micrOSDevToolKit-1.20.8/MANIFEST.in
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-26 12:03:05.172907 micrOSDevToolKit-1.20.8/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.20.8/README.md
--rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.20.8/devToolKit.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:04.839571 micrOSDevToolKit-1.20.8/env/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.8/env/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:04.853200 micrOSDevToolKit-1.20.8/media/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.20.8/media/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/media/dnd.png
--rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.20.8/media/logo.png
--rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/media/logo_mini.png
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:04.862567 micrOSDevToolKit-1.20.8/micrOS/
--rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.20.8/micrOS/SchedulerUT.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.8/micrOS/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:04.904586 micrOSDevToolKit-1.20.8/micrOS/micropython/
--rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.8/micrOS/micropython/esp32-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.20.8/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.20.8/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
--rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.8/micrOS/micropython/tinypico-20220618-v1.19.1.bin
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:04.967218 micrOSDevToolKit-1.20.8/micrOS/source/
--rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.20.8/micrOS/source/.DS_Store
--rw-r--r--   0 bnm        (501) staff       (20)     6198 2023-07-17 14:02:35.000000 micrOSDevToolKit-1.20.8/micrOS/source/Common.py
--rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.20.8/micrOS/source/ConfigHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     6331 2023-07-17 14:19:18.000000 micrOSDevToolKit-1.20.8/micrOS/source/Debug.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.20.8/micrOS/source/Hooks.py
--rw-r--r--   0 bnm        (501) staff       (20)     6844 2023-07-22 08:28:00.000000 micrOSDevToolKit-1.20.8/micrOS/source/InterConnect.py
--rw-r--r--   0 bnm        (501) staff       (20)    11569 2023-07-26 11:40:59.000000 micrOSDevToolKit-1.20.8/micrOS/source/InterpreterShell.py
--rw-r--r--   0 bnm        (501) staff       (20)     7470 2023-07-20 09:51:20.000000 micrOSDevToolKit-1.20.8/micrOS/source/InterruptHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_L298N_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_bme280.py
--rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_buzzer.py
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_cct.py
--rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_co2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-18 21:04:59.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_dht11.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_dht22.py
--rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_ds18.py
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_genIO.py
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_intercon.py
--rw-r--r--   0 bnm        (501) staff       (20)     1618 2023-07-06 20:03:50.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_light_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2890 2023-07-18 20:07:19.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_lmpacman.py
--rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_neoeffects.py
--rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_oled.py
--rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_oled_sh1106.py
--rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-04 18:36:10.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_oled_ui.py
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_presence.py
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_rgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_roboarm.py
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_servo.py
--rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_stepper.py
--rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_switch.py
--rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_system.py
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_telegram.py
--rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_tinyrgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LP_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.20.8/micrOS/source/LP_esp32s2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.20.8/micrOS/source/LP_esp32s3.py
--rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.8/micrOS/source/LP_rp2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LP_tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.20.8/micrOS/source/LogicalPins.py
--rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.20.8/micrOS/source/Network.py
--rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.20.8/micrOS/source/Notify.py
--rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.20.8/micrOS/source/Scheduler.py
--rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-15 19:57:59.000000 micrOSDevToolKit-1.20.8/micrOS/source/SocketServer.py
--rw-r--r--   0 bnm        (501) staff       (20)    19305 2023-07-26 11:52:48.000000 micrOSDevToolKit-1.20.8/micrOS/source/TaskManager.py
--rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.20.8/micrOS/source/Time.py
--rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.8/micrOS/source/TinyPLed.py
--rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.8/micrOS/source/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.20.8/micrOS/source/micrOS.py
--rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.20.8/micrOS/source/micrOSloader.py
--rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.20.8/micrOS/source/reset.py
--rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.20.8/micrOS/source/urequests.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:04.970183 micrOSDevToolKit-1.20.8/micrOSDevToolKit.egg-info/
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-26 12:03:04.000000 micrOSDevToolKit-1.20.8/micrOSDevToolKit.egg-info/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)     8866 2023-07-26 12:03:04.000000 micrOSDevToolKit-1.20.8/micrOSDevToolKit.egg-info/SOURCES.txt
--rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-26 12:03:04.000000 micrOSDevToolKit-1.20.8/micrOSDevToolKit.egg-info/dependency_links.txt
--rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-26 12:03:04.000000 micrOSDevToolKit-1.20.8/micrOSDevToolKit.egg-info/requires.txt
--rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-26 12:03:04.000000 micrOSDevToolKit-1.20.8/micrOSDevToolKit.egg-info/top_level.txt
--rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-26 12:03:05.173567 micrOSDevToolKit-1.20.8/setup.cfg
--rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-26 12:01:34.000000 micrOSDevToolKit-1.20.8/setup.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:04.992357 micrOSDevToolKit-1.20.8/toolkit/
--rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.20.8/toolkit/DevEnvCompile.py
--rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.20.8/toolkit/DevEnvOTA.py
--rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.20.8/toolkit/DevEnvUSB.py
--rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/Gateway.py
--rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.20.8/toolkit/MicrOSDevEnv.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.022500 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/
--rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/AirQualityBME280.py
--rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/CCTDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/CCTTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/CatGame.py
--rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/Dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/GetVersion.py
--rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/MicrophoneTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/NeoEffectsDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/NeopixelTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/RGBTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/RoboArm.py
--rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/SED_test.py
--rw-r--r--   0 bnm        (501) staff       (20)    17600 2023-07-19 10:50:53.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/SystemTest.py
--rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/Template_app.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/_micPlotting.py
--rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/uLightDemo.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.031427 micrOSDevToolKit-1.20.8/toolkit/lib/
--rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.20.8/toolkit/lib/LocalMachine.py
--rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.20.8/toolkit/lib/SearchDevices.py
--rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/lib/SerialDriverHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/lib/TerminalColors.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/lib/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.20.8/toolkit/lib/micrOSClient.py
--rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.20.8/toolkit/micrOSdashboard.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.046347 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/
--rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/LP_darwin.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.103842 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5397 2023-07-15 16:13:28.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/dotstar.py
--rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/ds18x20.py
--rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/framebuf.py
--rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/machine.py
--rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/micropython.py
--rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/network.py
--rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/ntptime.py
--rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/onewire.py
--rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/sim_console.py
--rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/simgc.py
--rw-r--r--   0 bnm        (501) staff       (20)     6545 2023-07-15 16:13:22.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/simulator.py
--rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/uasyncio.py
--rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/utime.py
--rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/webrepl.py
--rwxr-xr-x   0 bnm        (501) staff       (20)    16970 2023-07-19 10:36:50.000000 micrOSDevToolKit-1.20.8/toolkit/socketClient.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.104640 micrOSDevToolKit-1.20.8/toolkit/user_data/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:50:53.000000 micrOSDevToolKit-1.20.8/toolkit/user_data/.include
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.105123 micrOSDevToolKit-1.20.8/toolkit/user_data/node_config_archive/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/user_data/node_config_archive/.include
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.105519 micrOSDevToolKit-1.20.8/toolkit/workspace/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.171430 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/
--rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Common.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/ConfigHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1927 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Debug.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      759 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Hooks.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2085 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/InterConnect.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     4174 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/InterpreterShell.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/InterruptHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      869 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_bme280.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_buzzer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_cct.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_co2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_dht11.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_dht22.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_dimmer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)      522 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_ds18.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_genIO.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)      616 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_intercon.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      512 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_light_sensor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1477 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_lmpacman.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_neoeffects.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_neopixel.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_oled.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     6082 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_oled_ui.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_presence.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_rgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_roboarm.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_servo.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_stepper.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_switch.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_system.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      872 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_telegram.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_tinyrgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      550 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LP_esp32.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      563 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LP_esp32s2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      553 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LP_esp32s3.mpy
--rw-r--r--   0 bnm        (501) staff       (20)       54 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LP_rp2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      491 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LP_tinypico.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LogicalPins.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Network.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Notify.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Scheduler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/SocketServer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     5702 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/TaskManager.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Time.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      434 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/TinyPLed.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      440 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/micrOS.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/micrOSloader.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      198 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/reset.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/urequests.mpy
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.773724 micrOSDevToolKit-1.21.0/
+-rw-r--r--   0 bnm        (501) staff       (20)      333 2023-07-18 21:54:39.000000 micrOSDevToolKit-1.21.0/MANIFEST.in
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-26 14:54:48.773220 micrOSDevToolKit-1.21.0/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.21.0/README.md
+-rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.21.0/devToolKit.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.404457 micrOSDevToolKit-1.21.0/env/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.0/env/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.409750 micrOSDevToolKit-1.21.0/media/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.21.0/media/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/media/dnd.png
+-rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.21.0/media/logo.png
+-rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/media/logo_mini.png
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.413297 micrOSDevToolKit-1.21.0/micrOS/
+-rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.21.0/micrOS/SchedulerUT.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.0/micrOS/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.466565 micrOSDevToolKit-1.21.0/micrOS/micropython/
+-rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.0/micrOS/micropython/esp32-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.21.0/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.21.0/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
+-rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.0/micrOS/micropython/tinypico-20220618-v1.19.1.bin
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.538825 micrOSDevToolKit-1.21.0/micrOS/source/
+-rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.21.0/micrOS/source/.DS_Store
+-rw-r--r--   0 bnm        (501) staff       (20)     6198 2023-07-17 14:02:35.000000 micrOSDevToolKit-1.21.0/micrOS/source/Common.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.21.0/micrOS/source/ConfigHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6331 2023-07-17 14:19:18.000000 micrOSDevToolKit-1.21.0/micrOS/source/Debug.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.21.0/micrOS/source/Hooks.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6844 2023-07-22 08:28:00.000000 micrOSDevToolKit-1.21.0/micrOS/source/InterConnect.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11569 2023-07-26 14:03:06.000000 micrOSDevToolKit-1.21.0/micrOS/source/InterpreterShell.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7470 2023-07-20 09:51:20.000000 micrOSDevToolKit-1.21.0/micrOS/source/InterruptHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_L298N_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_bme280.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_buzzer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_cct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_co2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-18 21:04:59.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_dht11.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_dht22.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_ds18.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_genIO.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_intercon.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1618 2023-07-06 20:03:50.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_light_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2890 2023-07-18 20:07:19.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_lmpacman.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_neoeffects.py
+-rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_oled.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_oled_sh1106.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19328 2023-07-26 14:42:47.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_oled_ui.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_presence.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_rgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_roboarm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_servo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_stepper.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_switch.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_system.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_telegram.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LM_tinyrgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LP_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.21.0/micrOS/source/LP_esp32s2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.21.0/micrOS/source/LP_esp32s3.py
+-rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.0/micrOS/source/LP_rp2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.21.0/micrOS/source/LP_tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.21.0/micrOS/source/LogicalPins.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.21.0/micrOS/source/Network.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.21.0/micrOS/source/Notify.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.21.0/micrOS/source/Scheduler.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-15 19:57:59.000000 micrOSDevToolKit-1.21.0/micrOS/source/SocketServer.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19349 2023-07-26 13:44:08.000000 micrOSDevToolKit-1.21.0/micrOS/source/TaskManager.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.21.0/micrOS/source/Time.py
+-rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.0/micrOS/source/TinyPLed.py
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.21.0/micrOS/source/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.21.0/micrOS/source/micrOS.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.21.0/micrOS/source/micrOSloader.py
+-rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.21.0/micrOS/source/reset.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.21.0/micrOS/source/urequests.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.544057 micrOSDevToolKit-1.21.0/micrOSDevToolKit.egg-info/
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-26 14:54:48.000000 micrOSDevToolKit-1.21.0/micrOSDevToolKit.egg-info/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)     8866 2023-07-26 14:54:48.000000 micrOSDevToolKit-1.21.0/micrOSDevToolKit.egg-info/SOURCES.txt
+-rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-26 14:54:48.000000 micrOSDevToolKit-1.21.0/micrOSDevToolKit.egg-info/dependency_links.txt
+-rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-26 14:54:48.000000 micrOSDevToolKit-1.21.0/micrOSDevToolKit.egg-info/requires.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-26 14:54:48.000000 micrOSDevToolKit-1.21.0/micrOSDevToolKit.egg-info/top_level.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-26 14:54:48.773872 micrOSDevToolKit-1.21.0/setup.cfg
+-rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-26 14:51:46.000000 micrOSDevToolKit-1.21.0/setup.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.554680 micrOSDevToolKit-1.21.0/toolkit/
+-rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.21.0/toolkit/DevEnvCompile.py
+-rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.21.0/toolkit/DevEnvOTA.py
+-rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.21.0/toolkit/DevEnvUSB.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/Gateway.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.21.0/toolkit/MicrOSDevEnv.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.572579 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/
+-rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/AirQualityBME280.py
+-rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/CCTDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/CCTTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/CatGame.py
+-rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/Dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/GetVersion.py
+-rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/MicrophoneTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/NeoEffectsDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/NeopixelTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/RGBTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/RoboArm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/SED_test.py
+-rw-r--r--   0 bnm        (501) staff       (20)    17600 2023-07-19 10:50:53.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/SystemTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/Template_app.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/_micPlotting.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/uLightDemo.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.579360 micrOSDevToolKit-1.21.0/toolkit/lib/
+-rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.21.0/toolkit/lib/LocalMachine.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.21.0/toolkit/lib/SearchDevices.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/lib/SerialDriverHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/lib/TerminalColors.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/lib/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.21.0/toolkit/lib/micrOSClient.py
+-rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.21.0/toolkit/micrOSdashboard.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.597853 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/
+-rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/LP_darwin.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.648074 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5397 2023-07-15 16:13:28.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/dotstar.py
+-rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/ds18x20.py
+-rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/framebuf.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/machine.py
+-rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/micropython.py
+-rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/network.py
+-rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/ntptime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/onewire.py
+-rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/sim_console.py
+-rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/simgc.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6545 2023-07-15 16:13:22.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/simulator.py
+-rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/uasyncio.py
+-rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/utime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/simulator_lib/webrepl.py
+-rwxr-xr-x   0 bnm        (501) staff       (20)    16970 2023-07-19 10:36:50.000000 micrOSDevToolKit-1.21.0/toolkit/socketClient.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.649109 micrOSDevToolKit-1.21.0/toolkit/user_data/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:50:53.000000 micrOSDevToolKit-1.21.0/toolkit/user_data/.include
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.649626 micrOSDevToolKit-1.21.0/toolkit/user_data/node_config_archive/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/user_data/node_config_archive/.include
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.650416 micrOSDevToolKit-1.21.0/toolkit/workspace/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 14:54:48.771650 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/
+-rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Common.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/ConfigHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1927 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Debug.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      759 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Hooks.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2085 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/InterConnect.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     4174 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/InterpreterShell.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/InterruptHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      869 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_bme280.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_buzzer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_cct.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_co2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_dht11.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_dht22.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_dimmer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)      522 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_ds18.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_genIO.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)      616 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_intercon.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      512 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_light_sensor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1477 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_lmpacman.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_neoeffects.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_neopixel.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_oled.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     6191 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_oled_ui.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_presence.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_rgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_roboarm.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_servo.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_stepper.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_switch.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_system.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      872 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_telegram.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_tinyrgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      550 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LP_esp32.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      563 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LP_esp32s2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      553 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LP_esp32s3.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)       54 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LP_rp2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      491 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LP_tinypico.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LogicalPins.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Network.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Notify.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Scheduler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/SocketServer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     5718 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/TaskManager.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Time.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      434 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/TinyPLed.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/micrOS.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/micrOSloader.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      198 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/reset.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-07-26 14:51:58.000000 micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/urequests.mpy
```

### Comparing `micrOSDevToolKit-1.20.8/PKG-INFO` & `micrOSDevToolKit-1.21.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.20.8
+Version: 1.21.0
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.20.8/README.md` & `micrOSDevToolKit-1.21.0/README.md`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/devToolKit.py` & `micrOSDevToolKit-1.21.0/devToolKit.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/media/dnd.png` & `micrOSDevToolKit-1.21.0/media/dnd.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/media/logo.png` & `micrOSDevToolKit-1.21.0/media/logo.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/media/logo_mini.png` & `micrOSDevToolKit-1.21.0/media/logo_mini.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/SchedulerUT.py` & `micrOSDevToolKit-1.21.0/micrOS/SchedulerUT.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/micropython/esp32-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.21.0/micrOS/micropython/esp32-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/micropython/esp32s2-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.21.0/micrOS/micropython/esp32s2-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin` & `micrOSDevToolKit-1.21.0/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2` & `micrOSDevToolKit-1.21.0/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/micropython/tinypico-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.21.0/micrOS/micropython/tinypico-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/.DS_Store` & `micrOSDevToolKit-1.21.0/micrOS/source/.DS_Store`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/Common.py` & `micrOSDevToolKit-1.21.0/micrOS/source/Common.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/ConfigHandler.py` & `micrOSDevToolKit-1.21.0/micrOS/source/ConfigHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/Debug.py` & `micrOSDevToolKit-1.21.0/micrOS/source/Debug.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/Hooks.py` & `micrOSDevToolKit-1.21.0/micrOS/source/Hooks.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/InterConnect.py` & `micrOSDevToolKit-1.21.0/micrOS/source/InterConnect.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/InterpreterShell.py` & `micrOSDevToolKit-1.21.0/micrOS/source/InterpreterShell.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 #################################################################
 #                  SHELL Interpreter FUNCTIONS                  #
 #################################################################
 
 class Shell:
-    MICROS_VERSION = '1.20.5-0'
+    MICROS_VERSION = '1.21.0-0'
 
     def __init__(self, msg_obj=None):
         """
         comm_obj - communication object - send messages back
                  - comm_obj.reply('msg')
         """
         self.msg_obj = msg_obj
```

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/InterruptHandler.py` & `micrOSDevToolKit-1.21.0/micrOS/source/InterruptHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_L298N_DCmotor.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_L298N_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_VL53L0X.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_bme280.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_bme280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_buzzer.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_buzzer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_catgame.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_cct.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_cct.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_co2.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_co2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_demo.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_dht11.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_dht11.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_dht22.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_dht22.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_dimmer.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_distance.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_ds18.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_ds18.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_esp32.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_genIO.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_genIO.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_i2c.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_intercon.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_intercon.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_light_sensor.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_light_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_lmpacman.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_lmpacman.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_neoeffects.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_neoeffects.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_neopixel.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_oled.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_oled.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_oled_sh1106.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_oled_sh1106.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_oled_ui.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_oled_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ConfigHandler import cfgget
-from utime import localtime
+from utime import localtime, sleep
 from network import WLAN, STA_IF
 from LogicalPins import physical_pin, pinmap_dump
 from Network import ifconfig
 from Debug import errlog_add
 from machine import Pin
 from TaskManager import exec_lm_core, Manager
 try:
@@ -271,26 +271,26 @@
                 PageUI.DISPLAY.text(self.cmd_out[char_limit:], x, y + 20)
         else:
             PageUI.DISPLAY.text(self.cmd_out, x, y + 10)
 
     #####################################
     #           PAGE GENERATORS         #
     #####################################
-    def intercon_page(self, host, cmd):
+    def intercon_page(self, host, cmd, run=False):
         """Generic interconnect page core - create multiple page with it"""
         posx, posy = 5, 12
 
         def _button():
             # BUTTON CALLBACK - INTERCONNECT execution
             self.open_intercons.append(host)
             try:
                 # Send CMD to other device & show result
                 data_meta = InterCon.send_cmd(host, cmd)
                 self.cmd_task_tag = data_meta['tag']
-                if "Busy" in data_meta['verdict']:
+                if "Task is Busy" in data_meta['verdict'] and not run:
                     self.cmd_out = data_meta['verdict']     # Otherwise the task start output not relevant on UI
             except Exception as e:
                 self.cmd_out = str(e)
             self.open_intercons.remove(host)
 
         # Check open host connection
         if host in self.open_intercons:
@@ -308,16 +308,19 @@
                 Manager().kill(tag=self.cmd_task_tag)
                 # data gathered - remove tag - skip re-read
                 self.cmd_task_tag = None
         # Show self.cmd_out value on display
         self._cmd_text(posx, posy+10)
         # Set button press callback (+draw button)
         self.set_press_callback(_button)
+        # Run button event at page init
+        if run:
+            _button()
 
-    def cmd_call_page(self, cmd):
+    def cmd_call_page(self, cmd, run=False):
         """Generic LoadModule execution page core - create multiple page with it"""
         posx, posy = 5, 12
 
         def _buffer(msg):
             try:
                 self.cmd_out = ''.join(msg.strip().split()).replace(' ', '').replace('ºC', 'C')
             except Exception:
@@ -333,14 +336,17 @@
                 self.cmd_out = str(e)
 
         # Draw host + cmd details
         PageUI.DISPLAY.text(cmd, 0, posy)
         self._cmd_text(posx, posy)
         # Set button press callback (+draw button)
         self.set_press_callback(_button)
+        # Run button event at page init
+        if run:
+            _button()
 
 
 #################################
 #        PAGE DEFINITIONS       #
 #################################
 
 def _sys_page():
@@ -352,27 +358,28 @@
     if memory_usage is not None:
         mem = memory_usage()
         PageUI.DISPLAY.text(f"  {mem['percent']}% ({int(mem['mem_used']/1000)}kb)", 0, 35)
     PageUI.DISPLAY.text(f"  V: {cfgget('version')}", 0, 45)
     return True
 
 
-def _intercon_cache():
+def _intercon_cache(line_limit=3):
     if InterCon is None:
         return False
     line_start = 15
     line_cnt = 1
-    line_limit = 3
     PageUI.DISPLAY.text("InterCon cache", 0, line_start)
     if sum([1 for _ in InterCon.dump()]) > 0:
         for key, val in InterCon.dump().items():
             key = key.split('.')[0]
             val = '.'.join(val.split('.')[-2:])
             PageUI.DISPLAY.text(" {} {}".format(val, key), 0, line_start+(line_cnt*10))
-            line_cnt = 1 if line_cnt > line_limit else line_cnt+1
+            line_cnt += 1
+            if line_cnt > line_limit:
+                break
         return True
     PageUI.DISPLAY.text("Empty", 40, line_start+20)
     return True
 
 
 def _micros_welcome():
     """Template function"""
@@ -463,51 +470,53 @@
     :param msg: message string
     """
     PageUI.PAGE_UI_OBJ.show_msg = msg
     PageUI.PAGE_UI_OBJ.show_page()
     return 'Show msg'
 
 
-def intercon_genpage(cmd=None):
+def intercon_genpage(cmd=None, run=False):
     """
     Create intercon pages dynamically :)
     - based on cmd value.
     :param cmd: 'host hello' or 'host system clock'
+    :param run: run button event at page init: True/False
     :return: page creation verdict
     """
     raw = cmd.split()
     host = raw[0]
     cmd = ' '.join(raw[1:])
     if PageUI.PAGE_UI_OBJ is None:
         # Auto init UI
         pageui()
     try:
         # Create page for intercon command
-        PageUI.PAGE_UI_OBJ.add_page(lambda: PageUI.PAGE_UI_OBJ.intercon_page(host, cmd))
+        PageUI.PAGE_UI_OBJ.add_page(lambda: PageUI.PAGE_UI_OBJ.intercon_page(host, cmd, run=run))
     except Exception as e:
         return str(e)
     return True
 
 
-def cmd_genpage(cmd=None):
+def cmd_genpage(cmd=None, run=False):
     """
     Create load module execution pages dynamically :)
     - based on cmd value: load_module function (args)
     :param cmd: 'load_module function (args)' string
+    :param run: run button event at page init: True/False
     :return: page creation verdict
     """
     if not isinstance(cmd, str):
         return False
 
     if PageUI.PAGE_UI_OBJ is None:
         # Auto init UI
         pageui()
     try:
         # Create page for intercon command
-        PageUI.PAGE_UI_OBJ.add_page(lambda: PageUI.PAGE_UI_OBJ.cmd_call_page(cmd))
+        PageUI.PAGE_UI_OBJ.add_page(lambda: PageUI.PAGE_UI_OBJ.cmd_call_page(cmd, run=run))
     except Exception as e:
         print(e)
         return str(e)
     return True
 
 
 #######################
@@ -540,10 +549,10 @@
     [i] micrOS LM naming convention
     Load Module built-in help message
     :return tuple: list of functions implemented by this application
     """
     return 'pageui page=0 pwr_sec=None/int(sec) oled_type="ssd1306 or sh1106"',\
            'control next/prev/press/on/off',\
            'msgbox "msg"',\
-           'intercon_genpage "host cmd"',\
-           'cmd_genpage "cmd"',\
-           'pinmap', 'INFO: OLED Module for SSD1306'
+           'intercon_genpage "host" "cmd" run=False',\
+           'cmd_genpage "cmd" run=False',\
+           'pinmap'
```

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_pet_feeder.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_ph_sensor.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_presence.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_presence.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_rencoder.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_rgb.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_rgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_roboarm.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_roboarm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_robustness.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_servo.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_servo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_stepper.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_stepper.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_switch.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_switch.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_system.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_system.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_telegram.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_telegram.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LM_tinyrgb.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LM_tinyrgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LP_esp32.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LP_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LP_esp32s2.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LP_esp32s2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LP_esp32s3.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LP_esp32s3.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LP_tinypico.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LP_tinypico.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/LogicalPins.py` & `micrOSDevToolKit-1.21.0/micrOS/source/LogicalPins.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/Network.py` & `micrOSDevToolKit-1.21.0/micrOS/source/Network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/Notify.py` & `micrOSDevToolKit-1.21.0/micrOS/source/Notify.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/Scheduler.py` & `micrOSDevToolKit-1.21.0/micrOS/source/Scheduler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/SocketServer.py` & `micrOSDevToolKit-1.21.0/micrOS/source/SocketServer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/TaskManager.py` & `micrOSDevToolKit-1.21.0/micrOS/source/TaskManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,19 +227,20 @@
         - Try to measure system load - based on idle task latency
         """
         # FREQUENCY OF IDLE TASK - IMPACTS IRQ TASK SCHEDULING, SMALLER IS BEST
         my_task = Task.TASKS.get('idle')
         my_task.out = f"i.d.l.e: 200ms"
         try:
             while True:
+                await asyncio.sleep_ms(300)
                 # Probe system load
                 t = ticks_ms()
-                await asyncio.sleep_ms(500)
+                await asyncio.sleep_ms(300)
                 # SysLogic block - sys load
-                delta_rate = int(((ticks_diff(ticks_ms(), t) / 500)-1) * 100)
+                delta_rate = int(((ticks_diff(ticks_ms(), t) / 300)-1) * 100)
                 Manager.OLOAD = int((Manager.OLOAD + delta_rate) / 2)       # Average - smooth
         except Exception as e:
             errlog_add(f"[ERR] Idle task exists: {e}")
         my_task.done.set()
 
     @staticmethod
     def create_task(callback, tag=None, loop=False, delay=None):
```

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/Time.py` & `micrOSDevToolKit-1.21.0/micrOS/source/Time.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/TinyPLed.py` & `micrOSDevToolKit-1.21.0/micrOS/source/TinyPLed.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/micrOS.py` & `micrOSDevToolKit-1.21.0/micrOS/source/micrOS.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/micrOSloader.py` & `micrOSDevToolKit-1.21.0/micrOS/source/micrOSloader.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOS/source/urequests.py` & `micrOSDevToolKit-1.21.0/micrOS/source/urequests.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/micrOSDevToolKit.egg-info/PKG-INFO` & `micrOSDevToolKit-1.21.0/micrOSDevToolKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.20.8
+Version: 1.21.0
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.20.8/micrOSDevToolKit.egg-info/SOURCES.txt` & `micrOSDevToolKit-1.21.0/micrOSDevToolKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/setup.py` & `micrOSDevToolKit-1.21.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # https://towardsdatascience.com/create-your-custom-python-package-that-you-can-pip-install-from-your-git-repository-f90465867893
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='micrOSDevToolKit',
-    version='1.20.8',
+    version='1.21.0',
     author='Marcell Ban',
     author_email='miros.framework@gmail.com',
     description='Development and deployment environment for micrOS, the diy micropython automation OS (IoT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/BxNxM/micrOS',
     project_urls={
```

### Comparing `micrOSDevToolKit-1.20.8/toolkit/DevEnvCompile.py` & `micrOSDevToolKit-1.21.0/toolkit/DevEnvCompile.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/DevEnvOTA.py` & `micrOSDevToolKit-1.21.0/toolkit/DevEnvOTA.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/DevEnvUSB.py` & `micrOSDevToolKit-1.21.0/toolkit/DevEnvUSB.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/Gateway.py` & `micrOSDevToolKit-1.21.0/toolkit/Gateway.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/MicrOSDevEnv.py` & `micrOSDevToolKit-1.21.0/toolkit/MicrOSDevEnv.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/AirQualityBME280.py` & `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/AirQualityBME280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/AirQualityDHT22_CO2.py` & `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/AirQualityDHT22_CO2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/CCTDemo.py` & `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/CCTDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/CCTTest.py` & `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/CCTTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/CatGame.py` & `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/CatGame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/Dimmer.py` & `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/Dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/GetVersion.py` & `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/GetVersion.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/NeoEffectsDemo.py` & `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/NeoEffectsDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/NeopixelTest.py` & `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/NeopixelTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/RGBTest.py` & `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/RGBTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/RoboArm.py` & `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/RoboArm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/SED_test.py` & `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/SED_test.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/SystemTest.py` & `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/SystemTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/Template_app.py` & `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/Template_app.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/_micPlotting.py` & `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/_micPlotting.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/uLightDemo.py` & `micrOSDevToolKit-1.21.0/toolkit/dashboard_apps/uLightDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/lib/LocalMachine.py` & `micrOSDevToolKit-1.21.0/toolkit/lib/LocalMachine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/lib/SearchDevices.py` & `micrOSDevToolKit-1.21.0/toolkit/lib/SearchDevices.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/lib/SerialDriverHandler.py` & `micrOSDevToolKit-1.21.0/toolkit/lib/SerialDriverHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/lib/TerminalColors.py` & `micrOSDevToolKit-1.21.0/toolkit/lib/TerminalColors.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/lib/micrOSClient.py` & `micrOSDevToolKit-1.21.0/toolkit/lib/micrOSClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/micrOSdashboard.py` & `micrOSDevToolKit-1.21.0/toolkit/micrOSdashboard.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/LP_darwin.py` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/LP_darwin.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/machine.py` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/machine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/micropython.py` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/micropython.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/neopixel.py` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/network.py` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/sim_console.py` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/sim_console.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/simulator.py` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/simulator.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/uasyncio.py` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/uasyncio.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/utime.py` & `micrOSDevToolKit-1.21.0/toolkit/simulator_lib/utime.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/socketClient.py` & `micrOSDevToolKit-1.21.0/toolkit/socketClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Common.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Common.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/ConfigHandler.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/ConfigHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Debug.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Debug.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Hooks.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Hooks.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/InterConnect.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/InterConnect.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/InterpreterShell.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/InterpreterShell.mpy`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6366 6770 7574 001a 436f 6e66 6967 4861  cfgput..ConfigHa
 00000050: 6e64 6c65 7200 1865 7865 635f 6c6d 5f63  ndler..exec_lm_c
 00000060: 6f72 6500 1654 6173 6b4d 616e 6167 6572  ore..TaskManager
 00000070: 001a 636f 6e73 6f6c 655f 7772 6974 6500  ..console_write.
 00000080: 1465 7272 6c6f 675f 6164 6400 0a44 6562  .errlog_add..Deb
 00000090: 7567 000a 7265 7365 7400 1473 6f66 745f  ug..reset..soft_
 000000a0: 7265 7365 7400 0e6d 6163 6869 6e65 000a  reset..machine..
-000000b0: 5368 656c 6c00 1031 2e32 302e 352d 3000  Shell..1.20.5-0.
+000000b0: 5368 656c 6c00 1031 2e32 312e 302d 3000  Shell..1.21.0-0.
 000000c0: 230e 6d73 675f 6f62 6a00 0c64 6576 6669  #.msg_obj..devfi
 000000d0: 6400 105f 5f64 6576 6669 6400 0861 7574  d..__devfid..aut
 000000e0: 6800 165f 5f61 7574 685f 6d6f 6465 000a  h..__auth_mode..
 000000f0: 6877 7569 6400 0e5f 5f68 7775 6964 0012  hwuid..__hwuid..
 00000100: 5f5f 6175 7468 5f6f 6b00 165f 5f63 6f6e  __auth_ok..__con
 00000110: 665f 6d6f 6465 000e 7665 7273 696f 6e00  f_mode..version.
 00000120: 1c4d 4943 524f 535f 5645 5253 494f 4e00  .MICROS_VERSION.
```

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/InterruptHandler.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/InterruptHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_VL53L0X.py` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_bme280.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_bme280.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_buzzer.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_buzzer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_catgame.py` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_cct.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_cct.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_co2.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_co2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_demo.py` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_dht11.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_dht11.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_dht22.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_dht22.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_dimmer.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_dimmer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_distance.py` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_ds18.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_ds18.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_esp32.py` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_genIO.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_genIO.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_i2c.py` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_intercon.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_intercon.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_light_sensor.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_light_sensor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_lmpacman.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_lmpacman.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_neoeffects.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_neoeffects.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_neopixel.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_neopixel.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_oled.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_oled.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_oled_sh1106.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_oled_sh1106.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_oled_ui.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_oled_ui.mpy`

 * *Files 22% similar despite different names*

```diff
@@ -1,381 +1,387 @@
-00000000: 4d06 001f 8138 0e1a 4c4d 5f6f 6c65 645f  M....8..LM_oled_
+00000000: 4d06 001f 813a 0f1a 4c4d 5f6f 6c65 645f  M....:..LM_oled_
 00000010: 7569 2e70 7900 0f0c 6366 6767 6574 001a  ui.py...cfgget..
 00000020: 436f 6e66 6967 4861 6e64 6c65 7200 126c  ConfigHandler..l
-00000030: 6f63 616c 7469 6d65 000a 7574 696d 6500  ocaltime..utime.
-00000040: 0857 4c41 4e00 0c53 5441 5f49 4600 0e6e  .WLAN..STA_IF..n
-00000050: 6574 776f 726b 0018 7068 7973 6963 616c  etwork..physical
-00000060: 5f70 696e 0016 7069 6e6d 6170 5f64 756d  _pin..pinmap_dum
-00000070: 7000 164c 6f67 6963 616c 5069 6e73 0010  p..LogicalPins..
-00000080: 6966 636f 6e66 6967 000e 4e65 7477 6f72  ifconfig..Networ
-00000090: 6b00 1465 7272 6c6f 675f 6164 6400 0a44  k..errlog_add..D
-000000a0: 6562 7567 0006 5069 6e00 0e6d 6163 6869  ebug..Pin..machi
-000000b0: 6e65 0018 6578 6563 5f6c 6d5f 636f 7265  ne..exec_lm_core
-000000c0: 000e 4d61 6e61 6765 7200 1654 6173 6b4d  ..Manager..TaskM
-000000d0: 616e 6167 6572 0018 6d65 6d6f 7279 5f75  anager..memory_u
-000000e0: 7361 6765 0012 4c4d 5f73 7973 7465 6d00  sage..LM_system.
-000000f0: 164c 4d5f 696e 7465 7263 6f6e 000e 6765  .LM_intercon..ge
-00000100: 745f 6164 6300 104c 4d5f 6765 6e49 4f00  t_adc..LM_genIO.
-00000110: 0c50 6167 6555 4900 0e73 7364 3133 3036  .PageUI..ssd1306
-00000120: 0081 6914 6d69 6372 4f53 206d 7367 0014  ..i.micrOS msg..
-00000130: 6f6c 6564 7569 6274 746e 0012 5f73 7973  oleduibttn.._sys
-00000140: 5f70 6167 6500 0e44 4953 504c 4159 0008  _page..DISPLAY..
-00000150: 7465 7874 000c 6465 7666 6964 0008 2020  text..devfid..  
-00000160: 7b7d 0081 290e 7065 7263 656e 7400 106d  {}..).percent..m
-00000170: 656d 5f75 7365 6400 0e20 2056 3a20 7b7d  em_used..  V: {}
-00000180: 000e 7665 7273 696f 6e00 1e5f 696e 7465  ..version.._inte
-00000190: 7263 6f6e 5f63 6163 6865 0008 6475 6d70  rcon_cache..dump
-000001a0: 0081 4d82 2302 2e00 8151 0c20 7b7d 207b  ..M.#....Q. {} {
-000001b0: 7d00 0a45 6d70 7479 001e 5f6d 6963 726f  }..Empty.._micro
-000001c0: 735f 7765 6c63 6f6d 6500 146d 6963 724f  s_welcome..micrO
-000001d0: 5320 4755 4900 1650 4147 455f 5549 5f4f  S GUI..PAGE_UI_O
-000001e0: 424a 0024 7365 745f 7072 6573 735f 6361  BJ.$set_press_ca
-000001f0: 6c6c 6261 636b 0012 5f61 6463 5f70 6167  llback.._adc_pag
-00000200: 6500 086e 756c 6c00 0876 6f6c 7400 0c67  e..null..volt..g
-00000210: 656e 6164 6300 0270 0008 7b7d 2025 0008  enadc..p..{} %..
-00000220: 7b7d 2056 000c 7061 6765 7569 0008 7061  {} V..pageui..pa
-00000230: 6765 000e 7077 725f 7365 6300 126f 6c65  ge..pwr_sec..ole
-00000240: 645f 7479 7065 0012 7368 6f77 5f70 6167  d_type..show_pag
-00000250: 6500 0e63 6f6e 7472 6f6c 000c 6d73 6762  e..control..msgb
-00000260: 6f78 0010 7368 6f77 5f6d 7367 0010 5368  ox..show_msg..Sh
-00000270: 6f77 206d 7367 0020 696e 7465 7263 6f6e  ow msg. intercon
-00000280: 5f67 656e 7061 6765 0009 1061 6464 5f70  _genpage...add_p
-00000290: 6167 6500 1663 6d64 5f67 656e 7061 6765  age..cmd_genpage
-000002a0: 000a 6c6d 6465 7000 0c70 696e 6d61 7000  ..lmdep..pinmap.
-000002b0: 823f 0868 656c 7000 2382 310e 4c4d 5f6f  .?.help.#.1.LM_o
-000002c0: 6c65 6400 1c4c 4d5f 6f6c 6564 5f73 6831  led..LM_oled_sh1
-000002d0: 3130 3600 2470 6167 655f 6361 6c6c 6261  106.$page_callba
-000002e0: 636b 5f6c 6973 7400 1661 6374 6976 655f  ck_list..active_
-000002f0: 7061 6765 000a 7769 6474 6800 0c68 6569  page..width..hei
-00000300: 6768 7400 1862 6c69 6e6b 5f65 6666 6563  ght..blink_effec
-00000310: 7400 146f 6c65 645f 7374 6174 6500 2662  t..oled_state.&b
-00000320: 7474 6e5f 7072 6573 735f 6361 6c6c 6261  ttn_press_callba
-00000330: 636b 001c 6f70 656e 5f69 6e74 6572 636f  ck..open_interco
-00000340: 6e73 0006 6e2f 6100 0e63 6d64 5f6f 7574  ns..n/a..cmd_out
-00000350: 0018 636d 645f 7461 736b 5f74 6167 000c  ..cmd_task_tag..
-00000360: 6972 715f 6f6b 0026 5f5f 6372 6561 7465  irq_ok.&__create
-00000370: 5f62 7574 746f 6e5f 6972 7100 1274 696d  _button_irq..tim
-00000380: 6972 7173 6571 001e 7077 725f 7361 7665  irqseq..pwr_save
-00000390: 725f 7374 6174 6500 1a5f 5f70 6167 655f  r_state..__page_
-000003a0: 6865 6164 6572 0006 307b 7d00 0230 000b  header..0{}..0..
-000003b0: 0221 0014 5f5f 7061 6765 5f62 6172 0008  .!..__page_bar..
-000003c0: 7265 6374 0010 5f5f 6d73 6762 6f78 000e  rect..__msgbox..
-000003d0: 706f 7765 726f 6e00 0a73 7461 7465 0004  poweron..state..
-000003e0: 494e 0012 5055 4c4c 5f44 4f57 4e00 0669  IN..PULL_DOWN..i
-000003f0: 7271 000e 7472 6967 6765 7200 1449 5251  rq..trigger..IRQ
-00000400: 5f52 4953 494e 4700 0e68 616e 646c 6572  _RISING..handler
-00000410: 0018 5f5f 706f 7765 725f 7361 7665 0006  ..__power_save..
-00000420: 6f66 6600 790a 636c 6561 6e00 0873 686f  off.y.clean..sho
-00000430: 7700 0a70 7265 7373 0024 5f70 6167 655f  w..press.$_page_
-00000440: 6275 7474 6f6e 5f70 7265 7373 0008 7072  button_press..pr
-00000450: 6576 0004 6f6e 0010 706f 7765 726f 6666  ev..on..poweroff
-00000460: 0006 533a 3100 0653 3a30 0012 5f63 6d64  ..S:1..S:0.._cmd
-00000470: 5f74 6578 7400 1a69 6e74 6572 636f 6e5f  _text..intercon_
-00000480: 7061 6765 0006 7461 6700 8203 0306 c2ba  page..tag.......
-00000490: 4300 0243 0008 6b69 6c6c 001a 636d 645f  C..C..kill..cmd_
-000004a0: 6361 6c6c 5f70 6167 6500 143c 6c69 7374  call_page..<list
-000004b0: 636f 6d70 3e00 0e5f 6275 7474 6f6e 0010  comp>.._button..
-000004c0: 4845 4c4c 4f20 3a44 0016 5f5f 7669 7375  HELLO :D..__visu
-000004d0: 616c 697a 6500 0866 696c 6c00 205f 5f72  alize..fill. __r
-000004e0: 6762 5f62 7269 6768 746e 6573 7300 0e6d  gb_brightness..m
-000004f0: 6f64 756c 6573 0006 7379 7300 0c4c 4d5f  odules..sys..LM_
-00000500: 7267 6200 8155 1462 7269 6768 746e 6573  rgb..U.brightnes
-00000510: 7300 0c73 6d6f 6f74 6800 103c 6c61 6d62  s..smooth..<lamb
-00000520: 6461 3e00 165f 5f64 7261 775f 7273 7369  da>..__draw_rssi
-00000530: 000c 7374 6174 7573 0008 7273 7369 0008  ..status..rssi..
-00000540: 6c69 6e65 0012 5f5f 7077 725f 6f66 6600  line..__pwr_off.
-00000550: 105f 5f65 6666 6563 7400 1073 656e 645f  .__effect..send_
-00000560: 636d 6400 0842 7573 7900 0e76 6572 6469  cmd..Busy..verdi
-00000570: 6374 0082 010e 5f62 7566 6665 7200 0c6d  ct...._buffer..m
-00000580: 7367 6f62 6a00 1049 6e74 6572 436f 6e00  sgobj..InterCon.
-00000590: 2f2d 3581 3d82 3349 822f 0663 6d64 0006  /-5.=.3I./.cmd..
-000005a0: 6d73 6700 8143 8177 8213 1c70 6167 655f  msg..C.w...page_
-000005b0: 6361 6c6c 6261 636b 7300 0277 0002 6800  callbacks..w..h.
-000005c0: 820d 8157 8179 0c70 696e 6b65 7900 1a70  ...W.y.pinkey..p
-000005d0: 6167 655f 6361 6c6c 6261 636b 0010 6361  age_callback..ca
-000005e0: 6c6c 6261 636b 0002 7800 0279 0008 686f  llback..x..y..ho
-000005f0: 7374 0006 7069 6e00 050c 2020 7b7d 2520  st..pin...  {}% 
-00000600: 287b 7d6b 6229 0005 0e49 6e74 6572 436f  ({}kb)...InterCo
-00000610: 6e20 6361 6368 6500 0a05 0504 6e65 7874  n cache.....next
-00000620: 0005 0470 7265 7600 0505 7072 6573 7300  ...prev...press.
-00000630: 0502 6f6e 0005 036f 6666 0005 1c49 6e76  ..on...off...Inv
-00000640: 616c 6964 2063 6f6d 6d61 6e64 207b 7d21  alid command {}!
-00000650: 2048 696e 743a 207b 7d00 0a03 0504 6f6c   Hint: {}.....ol
-00000660: 6564 0005 0869 6e74 6572 636f 6e00 0505  ed...intercon...
-00000670: 6765 6e49 4f00 0a07 0541 7061 6765 7569  genIO....Apageui
-00000680: 2070 6167 653d 3020 7077 725f 7365 633d   page=0 pwr_sec=
-00000690: 4e6f 6e65 2f69 6e74 2873 6563 2920 6f6c  None/int(sec) ol
-000006a0: 6564 5f74 7970 653d 2273 7364 3133 3036  ed_type="ssd1306
-000006b0: 206f 7220 7368 3131 3036 2200 051e 636f   or sh1106"...co
-000006c0: 6e74 726f 6c20 6e65 7874 2f70 7265 762f  ntrol next/prev/
-000006d0: 7072 6573 732f 6f6e 2f6f 6666 0005 0c6d  press/on/off...m
-000006e0: 7367 626f 7820 226d 7367 2200 051b 696e  sgbox "msg"...in
-000006f0: 7465 7263 6f6e 5f67 656e 7061 6765 2022  tercon_genpage "
-00000700: 686f 7374 2063 6d64 2200 0511 636d 645f  host cmd"...cmd_
-00000710: 6765 6e70 6167 6520 2263 6d64 2200 0506  genpage "cmd"...
-00000720: 7069 6e6d 6170 0005 1d49 4e46 4f3a 204f  pinmap...INFO: O
-00000730: 4c45 4420 4d6f 6475 6c65 2066 6f72 2053  LED Module for S
-00000740: 5344 3133 3036 000a 0205 0773 7364 3133  SD1306.....ssd13
-00000750: 3036 0005 0673 6831 3130 3600 051d 4f6c  06...sh1106...Ol
-00000760: 6564 2055 4920 756e 6b6e 6f77 6e20 6f6c  ed UI unknown ol
-00000770: 6564 5f74 7970 653a 207b 7d00 050e 7b7d  ed_type: {}...{}
-00000780: 207b 7d20 7b7d 3a7b 7d3a 7b7d 0005 165b   {} {}:{}:{}...[
-00000790: 4552 525d 2042 7574 746f 6e20 4952 513a  ERR] Button IRQ:
-000007a0: 7b7d 207b 7d00 0510 7061 6765 3a20 7b7d  {} {}...page: {}
-000007b0: 2070 7772 3a20 7b7d 000a 0207 0238 3407   pwr: {}.....84.
-000007c0: 0234 350a 0207 0135 0702 3132 0804 302e  .45....5..12..0.
-000007d0: 3031 9324 1c56 012c 2c32 322c 2c2c 3222  01.$.V.,,22,,,2"
-000007e0: 4f26 224a 2722 4f86 0799 3f84 0d84 1284  O&"J'"O...?.....
-000007f0: 0f84 2a8b 0e89 0c89 0a88 1588 1a84 0984  ..*.............
-00000800: 0c80 1002 2a01 1b03 1c02 1602 5980 1004  ....*.......Y...
-00000810: 2a01 1b05 1c04 1604 5980 1006 1007 2a02  *.......Y.....*.
-00000820: 1b08 1c06 1606 1c07 1607 5980 1009 100a  ..........Y.....
-00000830: 2a02 1b0b 1c09 1609 1c0a 160a 5980 100c  *...........Y...
-00000840: 2a01 1b0d 1c0c 160c 5980 100e 2a01 1b0f  *.......Y...*...
-00000850: 1c0e 160e 5980 1010 2a01 1b11 1c10 1610  ....Y...*.......
-00000860: 5980 1012 1013 2a02 1b14 1c12 1612 1c13  Y.....*.........
-00000870: 1613 5948 0e80 1015 2a01 1b16 1c15 1615  ..YH....*.......
-00000880: 594a 0759 5116 154a 015d 4809 8051 1b17  YJ.YQ..J.]H..Q..
-00000890: 1681 1e4a 0859 5116 811e 4a01 5d48 0e80  ...J.YQ...J.]H..
-000008a0: 1018 2a01 1b19 1c18 1618 594a 0759 5116  ..*.......YJ.YQ.
-000008b0: 184a 015d 5432 0010 1a34 0216 1a32 0116  .J.]T2...4...2..
-000008c0: 1f32 0216 2932 0316 3132 0416 3551 101b  .2..)2..12..5Q..
-000008d0: 802a 0353 3305 163c 101c 2a01 5333 0616  .*.S3..<..*.S3..
-000008e0: 4110 1d2a 0153 3307 1642 512a 0153 3308  A..*.S3..BQ*.S3.
-000008f0: 1645 512a 0153 3309 1648 320a 1649 320b  .EQ*.S3..H2..I2.
-00000900: 164a 320c 164c 5163 0d87 4c10 3e1a 8b1b  .J2..LQc..L.>...
-00000910: 2343 8b2a 8423 840a 841b 890e 840e 6460  #C.*.#........d`
-00000920: 840f 8422 840d 8413 8412 8426 1181 1f16  ...".......&....
-00000930: 8120 101a 1681 2151 1633 5116 2080 5110  . ....!Q.3Q. .Q.
-00000940: 1b2a 0353 3300 164d 3201 1660 3202 1665  .*.S3..M2..`2..e
-00000950: 3203 1667 101e 2a01 5333 0416 5d32 0516  2..g..*.S3..]2..
-00000960: 7032 0616 4732 0716 4032 0816 4132 0916  p2..G2..@2..A2..
-00000970: 7632 0a16 3432 0b16 7c32 0c16 7d32 0d16  v2..42..|2..}2..
-00000980: 8104 5163 0e8b 78db 8501 4a4d 812a 812b  ..Qc..x...JM.*.+
-00000990: 812c 812d 3d3e 3f80 1f80 082a 2a47 2547  .,.-=>?....**G%G
-000009a0: 2c2d 2424 2424 2424 4444 2525 4424 4657  ,-$$$$$$DD%%D$FW
-000009b0: b614 4e36 0023 06dd 445d b614 4e36 0010  ..N6.#..D]..N6..
-000009c0: 1bd9 4447 8051 1b4f c742 4580 511b 50c7  ..DG.Q.O.BE.Q.P.
-000009d0: b712 1a18 2042 5912 0e23 0714 24b6 3601  .... BY..#..$.6.
-000009e0: 3401 5912 8124 2307 1424 b636 0134 0159  4.Y..$#..$.6.4.Y
-000009f0: b1b0 1851 b4b0 1852 b2b0 1853 b3b0 1854  ...Q...R...S...T
-00000a00: 51b0 1843 50b0 1855 52b0 1856 51b0 1857  Q..CP..UR..VQ..W
-00000a10: 2b00 b018 5810 59b0 185a 51b0 185b 50b0  +...X.Y..ZQ..[P.
-00000a20: 185c b014 5d36 0059 b512 812e 1202 105e  .\..]6.Y.......^
-00000a30: 3401 2287 68f7 8234 02b5 2b03 b018 5fb0  4.".h..4..+..._.
-00000a40: 121a 1833 5163 8e2c 8d10 3160 812a 8049  ...3Qc.,..1`.*.I
-00000a50: 4085 0885 0922 2447 4325 1f21 1f21 1f21  @...."$GC%.!.!.!
-00000a60: 2732 3900 b020 0001 c1b0 2001 01c2 480a  '29.. .... ...H.
-00000a70: b134 0059 b234 0059 4a04 594a 015d 1204  .4.Y.4.YJ.YJ.]..
-00000a80: 3400 c312 812f 1281 25b3 7b55 3401 3401  4..../..%.{U4.4.
-00000a90: 82d7 444b 1061 1424 b37b 5536 0142 43b3  ..DK.a.$.{U6.BC.
-00000aa0: 7b55 c412 812f 1281 25b3 7c55 3401 3401  {U.../..%.|U4.4.
-00000ab0: 82d7 444b 1061 1424 b37c 5536 0142 43b3  ..DK.a.$.|U6.BC.
-00000ac0: 7c55 c512 812f 1281 25b3 7d55 3401 3401  |U.../..%.}U4.4.
-00000ad0: 82d7 444b 1061 1424 b37d 5536 0142 43b3  ..DK.a.$.}U6.BC.
-00000ae0: 7d55 c612 0c34 0080 55c7 1281 2fb7 3401  }U...4..U.../.4.
-00000af0: 80d8 4445 b780 5542 4210 62c7 2500 1357  ..DE..UBB.b.%..W
-00000b00: 51de 4444 1046 424c 2500 135c 4444 1063  Q.DD.FBL%..\DD.c
-00000b10: 4242 1064 c812 1a13 2014 2123 0814 24b7  BB.d.... .!#..$.
-00000b20: b8b4 b5b6 3605 8080 3603 5951 6302 8818  ....6...6.YQc...
-00000b30: 6114 8112 6380 4c2f 2f38 3626 1206 1207  a...c.L//86&....
-00000b40: 3401 1481 1310 8114 3601 c112 812e b122  4.......6......"
-00000b50: 805b f29e f788 f434 01c2 121a 1320 1481  .[.....4..... ..
-00000b60: 1525 0013 538a f388 2500 1353 88f3 8836  .%..S...%..S...6
-00000b70: 0459 121a 1320 1481 1525 0013 5391 f381  .Y... ...%..S...
-00000b80: 2500 1353 8136 0459 b280 425e 57c3 121a  %..S.6.Y..B^W...
-00000b90: 1320 1481 1522 8076 b3f3 88b3 f322 8078  . ...".v.....".x
-00000ba0: b3f2 88b3 f336 0459 81e5 585a d743 1d59  .....6.Y..XZ.C.Y
-00000bb0: 5951 6385 5079 1681 1663 8054 2229 2522  YQc.Py...c.T")%"
-00000bc0: 2c26 9dc1 2500 135f 3003 c2c3 c4b2 51de  ,&..%.._0.....Q.
-00000bd0: 4442 5163 1281 2eb4 b2f7 8134 0288 f4c5  DBQc.......4....
-00000be0: b580 4262 57c6 121a 1320 1481 1525 0013  ..BbW.... ...%..
-00000bf0: 53b1 f386 b6f3 2500 1353 b1f3 82f3 86b6  S.....%..S......
-00000c00: f336 0459 81e5 585a d743 1959 5951 6386  .6.Y..XZ.C.YYQc.
-00000c10: 1869 1465 812a 806c 2029 502e 5512 812f  .i.e.*.l )P.U../
-00000c20: b013 5134 01c1 1281 2212 812e b013 53b1  ..Q4....".....S.
-00000c30: f734 0134 01c2 1281 3080 b013 53b2 3403  .4.4....0...S.4.
-00000c40: 5f4b 16c3 121a 1320 1466 b3b0 1354 85f3  _K..... .f...T..
-00000c50: b281 f384 3604 5942 2812 1a13 2014 66b0  ....6.YB(... .f.
-00000c60: 1352 b2f4 81f2 b013 5484 f3b2 82f3 8236  .R......T......6
-00000c70: 0459 5163 893c 5929 6781 2a80 7665 4025  .YQc.<Y)g.*.ve@%
-00000c80: 4522 4629 4553 244a 3127 542c 00b0 2000  E"F)ES$J1'T,.. .
-00000c90: 01c1 2500 1343 c2b2 51de 4442 5063 2500  ..%..C..Q.DBPc%.
-00000ca0: 1356 434e 121a 1320 1468 3600 5952 2500  .VCN... .h6.YR%.
-00000cb0: 1856 121a 1320 1466 8a8f 2280 6ca8 1069  .V... .f..".l..i
-00000cc0: 8136 8204 59b1 3400 5912 812f b234 018a  .6..Y.4.Y../.4..
-00000cd0: d844 6c12 1a13 2014 21b2 808a 2e02 558f  .Dl... .!.....U.
-00000ce0: 9936 0359 b28a 512e 0255 c312 812f b334  .6.Y..Q..U.../.4
-00000cf0: 018c d844 48b3 518b 2e02 5542 41b3 c212  ...DH.Q...UBA...
-00000d00: 1a13 2014 21b2 8fa8 3603 5952 6301 8440  .. .!...6.YRc..@
-00000d10: 510e 8117 6380 7729 3a25 0013 55d3 2500  Q...c.w):%..U.%.
-00000d20: 1855 121a 1320 1466 2280 6a91 8985 1069  .U... .f".j....i
-00000d30: 8110 8109 2500 1355 3684 0459 121a 1320  ....%..U6..Y... 
-00000d40: 1466 2280 6a98 8989 1069 8110 8109 2500  .f".j....i....%.
-00000d50: 1355 3684 0459 5163 866c e203 215d 812a  .U6..YQc.l..!].*
-00000d60: 8131 8091 2022 5229 222f 234e 3300 4808  .1.. "R)"/#N3.H.
-00000d70: 1209 b134 01c2 4a24 5712 8124 df44 5cc3  ...4..J$W..$.D\.
-00000d80: 4912 2309 1424 b1b3 3602 c451 c212 0eb4  I.#..$..6..Q....
-00000d90: 3401 5951 51c3 2803 5d4a 015d b244 6612  4.YQQ.(.]J.].Df.
-00000da0: 10b2 1210 136a 1210 136b 3403 c5b5 146c  .....j...k4....l
-00000db0: 106d 1210 136e 106f b020 0001 3684 0059  .m...n.o. ..6..Y
-00000dc0: 5225 0018 5c51 6301 8110 220e 8111 6381  R%..\Qc..."...c.
-00000dd0: 3780 9b25 0014 4110 7536 0163 8358 3116  7..%..A.u6.c.X1.
-00000de0: 7081 2a80 9f28 4522 254a 28b0 135f 3003  p.*..(E"%J(.._0.
-00000df0: c1c2 c3b1 51de 4442 5163 b380 d844 4ab3  ....Q.DBQc...DJ.
-00000e00: b2f3 b013 5f82 5642 4eb0 1441 1071 3601  ...._.VBN..A.q6.
-00000e10: 59b1 b013 5f82 5651 6382 0022 1447 812a  Y..._.VQc..".G.*
-00000e20: 8132 80ad 2722 29b1 b013 51dd 4442 5263  .2..'")...Q.DBRc
-00000e30: b013 5114 72b1 3601 5952 6386 5821 2040  ..Q.r.6.YRc.X! @
-00000e40: 812a 80b3 2029 2626 2626 2330 4a2a 2912  .*.. )&&&&#0J*).
-00000e50: 1a13 2014 7336 0059 b014 6736 00c1 b013  .. .s6.Y..g6....
-00000e60: 5644 c280 b014 6036 0059 b014 6536 0059  VD....`6.Y..e6.Y
-00000e70: b143 64b0 1352 1281 2fb0 1351 3401 81f3  .Cd..R../..Q4...
-00000e80: d844 4ab0 1351 8055 3400 5942 4ab0 1351  .DJ..Q.U4.YBJ..Q
-00000e90: b013 5255 3400 5912 1a13 2014 7436 0059  ..RU4.Y... .t6.Y
-00000ea0: b014 7036 0059 5163 8f50 2a46 4181 2a81  ..p6.YQc.P*FA.*.
-00000eb0: 2680 c34a 442a 2029 2a20 2930 2426 2428  &..JD* )* )0$&$(
-00000ec0: 2a20 2927 2d26 2427 2a29 262a 2924 26b0  * )'-&$'*)&*)$&.
-00000ed0: 135f 8055 b013 5f82 5651 b018 43b1 144e  ._.U.._.VQ..C..N
-00000ee0: 3600 1075 d944 49b0 1476 3600 5942 a781  6..u.DI..v6.YB..
-00000ef0: b114 4e36 0010 1cd9 446f b057 1352 81e5  ..N6....Do.W.R..
-00000f00: 5a18 52b0 1352 1281 2fb0 1351 3401 81f3  Z.R..R../..Q4...
-00000f10: d844 4480 b018 52b0 1440 3600 5951 b018  .DD...R..@6.YQ..
-00000f20: 5710 59b0 185a 42ee 80b1 144e 3600 1077  W.Y..ZB....N6..w
-00000f30: d944 6eb0 5713 5281 e65a 1852 b013 5280  .Dn.W.R..Z.R..R.
-00000f40: d744 4d12 812f b013 5134 0181 f3b0 1852  .DM../..Q4.....R
-00000f50: b014 4036 0059 51b0 1857 1059 b018 5a42  ..@6.YQ..W.Y..ZB
-00000f60: 76b1 144e 3600 1078 d944 4f12 1a13 2014  v..N6..x.DO... .
-00000f70: 6836 0059 52b0 1856 425d b114 4e36 0010  h6.YR..VB]..N6..
-00000f80: 71d9 4453 121a 1320 1479 3600 5950 b018  q.DS... .y6.YP..
-00000f90: 5651 b018 5742 4023 0a14 24b0 1352 b013  VQ..WB@#..$..R..
-00000fa0: 5636 0263 8208 1114 7681 2a80 e460 4027  V6.c....v.*..`@'
-00000fb0: 4246 b013 5751 de44 4251 63b0 1457 3600  BF..WQ.DBQc..W6.
-00000fc0: 5951 b018 5751 6387 2052 2234 812a 8133  YQ..WQc. R"4.*.3
-00000fd0: 80f1 2064 2631 6d28 2628 6627 b1b0 1857  .. d&1m(&(f'...W
-00000fe0: 230b 3002 c2c3 121a 1320 1466 b283 f3b3  #.0...... .f....
-00000ff0: 83f3 ae8e 3604 5912 1a13 2014 2110 75b2  ....6.Y... .!.u.
-00001000: b336 0359 107a b013 5add 4446 52b0 1855  .6.Y.z..Z.DFR..U
-00001010: 4255 107b b013 5add 4446 50b0 1855 4247  BU.{..Z.DFP..UBG
-00001020: b013 55d3 b018 5512 1a13 2014 66b2 82f3  ..U...U... .f...
-00001030: b382 f3ac 8cb0 1355 3605 5951 638a 004b  .......U6.YQc..K
-00001040: 227c 812a 8134 8135 9004 6020 342d 3533  "|.*.4.5..` 4-53
-00001050: 5b57 1281 2212 812e b013 53b1 f388 f734  [W..".....S....4
-00001060: 0134 0181 f3c3 1281 2fb0 135a 3401 b3d8  .4....../..Z4...
-00001070: 44da 8012 1a13 2014 21b0 135a 80b3 2e02  D..... .!..Z....
-00001080: 55b1 b28a f236 0359 1281 2fb0 135a b351  U....6.Y../..Z.Q
-00001090: 2e02 5534 01b3 85f3 d844 5b12 1a13 2014  ..U4.....D[... .
-000010a0: 21b0 135a b382 b3f4 85f3 2e02 55b1 b294  !..Z........U...
-000010b0: f236 0359 4255 121a 1320 1421 b013 5ab3  .6.YBU... .!..Z.
-000010c0: 512e 0255 b1b2 94f2 3603 5942 5012 1a13  Q..U....6.YBP...
-000010d0: 2014 21b0 135a b1b2 8af2 3603 5951 638c   .!..Z....6.YQc.
-000010e0: 2463 b101 7d81 2a81 3681 2690 1620 4687  $c..}.*.6.&.. F.
-000010f0: 0e29 422d 4f2a 3e50 4f51 454b 0001 0223  .)B-O*>POQEK...#
-00001100: 0c30 02c3 c4b0 b1b2 2000 03c5 2501 2500  .0...... ...%.%.
-00001110: 1358 dd44 4251 6312 1a13 2014 2125 0180  .X.DBQc... .!%..
-00001120: b436 0359 121a 1320 1421 2502 b3b4 8af2  .6.Y... .!%.....
-00001130: 3603 5925 0013 5b51 ded3 44d3 8012 8125  6.Y%..[Q..D....%
-00001140: 1213 3400 1474 107e 2500 135b 3682 0034  ..4..t.~%..[6..4
-00001150: 0114 7f10 4610 8100 3602 c6b6 51de d344  ....F...6...Q..D
-00001160: 6f12 812f b634 0180 d844 65b6 147f 1081  o../.4...De.....
-00001170: 0110 8102 3602 2500 185a 1213 3400 1481  ....6.%..Z..4...
-00001180: 0310 7e25 0013 5b36 8200 5951 2500 185b  ..~%..[6..YQ%..[
-00001190: 2500 147c b3b4 8af2 3602 5925 0014 34b5  %..|....6.Y%..4.
-000011a0: 3601 5951 6301 8720 d302 1c81 0663 6363  6.YQc.. .....ccc
-000011b0: 901b 2b42 2d28 2b55 3325 0013 5814 7225  ..+B-(+U3%..X.r%
-000011c0: 0136 0159 482b 1281 1e14 8118 2501 2502  .6.YH+......%.%.
-000011d0: 3602 c3b3 107e 5525 0018 5b10 8119 b310  6....~U%..[.....
-000011e0: 811a 55dd 4449 b310 811a 5525 0018 5a4a  ..U.DI....U%..ZJ
-000011f0: 1d57 1281 24df 4455 c449 0b12 8125 b434  .W..$.DU.I...%.4
-00001200: 0125 0018 5a51 51c4 2804 5d4a 015d 2500  .%..ZQQ.(.]J.]%.
-00001210: 1358 1481 1b25 0136 0159 5163 844c 52a1  .X...%.6.YQc.LR.
-00001220: 0181 0481 2a81 2690 3c20 4666 6087 0a2d  ....*.&.< Ff`..-
-00001230: 4900 0105 230c 3002 c2c3 b020 0001 2705  I...#.0.... ..'.
-00001240: b0b1 b520 0103 c412 1a13 2014 2125 0180  ... ...... .!%..
-00001250: b336 0359 2500 147c b2b3 3602 5925 0014  .6.Y%..|..6.Y%..
-00001260: 34b4 3601 5951 6302 8468 3e14 811c 6381  4.6.YQc..h>...c.
-00001270: 2790 4022 1f52 4829 1081 0014 2eb1 144e  '.@".RH).......N
-00001280: 3600 142c 3600 3601 147f 1046 1081 0036  6..,6.6....F...6
-00001290: 0214 7f10 8101 1081 0236 0225 0018 5a4a  .........6.%..ZJ
-000012a0: 1457 1281 24df 444c 59b1 144e 3600 2500  .W..$.DLY..N6.%.
-000012b0: 185a 4a01 5d51 6384 40d3 0216 8106 6363  .ZJ.]Qc.@.....cc
-000012c0: 6390 4620 224b 5848 1925 0114 4e36 0014  c.F "KXH.%..N6..
-000012d0: 2c36 00c3 1212 b310 811d 2502 3482 0159  ,6........%.4..Y
-000012e0: 4a1d 5712 8124 df44 55c4 490b 1281 25b4  J.W..$.DU.I...%.
-000012f0: 3401 2500 185a 5151 c428 045d 4a01 5d51  4.%..ZQQ.(.]J.]Q
-00001300: 6387 7040 161f 905a 6031 3927 251f 2337  c.p@...Z`19'%.#7
-00001310: 121a 1320 1421 1202 1022 3401 808f 3603  ... .!..."4...6.
-00001320: 5912 1a13 2014 2110 2314 2412 0c34 0081  Y... .!.#.$..4..
-00001330: 5580 5536 0180 9936 0359 1215 51de d344  U.U6...6.Y..Q..D
-00001340: 6712 1534 00c0 121a 1320 1421 2300 1424  g..4..... .!#..$
-00001350: b010 2555 1281 22b0 1026 5522 8768 f734  ..%U.."..&U".h.4
-00001360: 0136 0280 a336 0359 121a 1320 1421 1027  .6...6.Y... .!.'
-00001370: 1424 1202 1028 3401 3601 80ad 3603 5952  .$...(4.6...6.YR
-00001380: 638a 6478 2229 9067 2722 2222 222d 3532  c.dx").g'""""-52
-00001390: 2a33 372f 222f 1281 1e51 de44 4250 638f  *37/"/...Q.DBPc.
-000013a0: c081 c183 c212 1a13 2014 2123 0180 b036  ........ .!#...6
-000013b0: 0359 1281 2332 0012 811e 142a 3600 3401  .Y..#2.....*6.4.
-000013c0: 3401 80d8 44d7 8012 811e 142a 3600 142b  4...D......*6..+
-000013d0: 3600 5f4b 4730 02c3 c4b3 142c 102d 3601  6._KG0.....,.-6.
-000013e0: 8055 c310 2d14 2eb4 142c 102d 3601 7e51  .U..-....,.-6.~Q
-000013f0: 2e02 5536 01c4 121a 1320 1421 102f 1424  ..U6..... .!./.$
-00001400: b4b3 3602 80b0 b18a f4f2 3603 59b1 b2d8  ..6.......6.Y...
-00001410: 4443 8142 43b1 81f2 c142 b77f 5263 121a  DC.BC....B..Rc..
-00001420: 1320 1421 1030 a8b0 94f2 3603 5952 6301  . .!.0....6.YRc.
-00001430: 8120 390a 8105 6390 6d2b 00b0 5f4b 06c1  . 9...c.m+.._K..
-00001440: 812f 1442 3863 843c b802 1431 9079 2063  ./.B8c.<...1.y c
-00001450: 4022 2d56 3032 00c0 4819 121a 1320 1421  @"-V02..H.... .!
-00001460: 1032 9e8f 3603 5912 1a13 3314 34b0 3601  .2..6.Y...3.4.6.
-00001470: 594a 1a57 1281 24df 4452 c149 0812 8125  YJ.W..$.DR.I...%
-00001480: b134 0163 5151 c128 015d 4a01 5d52 6301  .4.cQQ.(.]J.]Rc.
-00001490: 8208 200c 8106 907b 202e 121a 1320 1421  .. ....{ .... .!
-000014a0: 1081 07a3 9d36 0359 121a 1320 1474 3600  .....6.Y... .t6.
-000014b0: 5951 6387 4c40 1e35 9088 6083 0f83 082d  YQc.L@.5..`....-
-000014c0: 272b 2b37 3728 3200 c032 01c1 2c02 1036  '++77(2..2..,..6
-000014d0: 1025 6210 3610 3762 c212 1851 ded3 444b  .%b.6.7b...Q..DK
-000014e0: 1218 1209 1038 3401 3401 c2b0 1039 b210  .....84.4....9..
-000014f0: 2555 3482 0059 121a 1320 1421 103a 1424  %U4..Y... .!.:.$
-00001500: b210 2555 3601 2280 4194 3603 5912 1a13  ..%U6.".A.6.Y...
-00001510: 2014 2110 3b14 24b2 1037 5536 0122 8041   .!.;.$..7U6.".A
-00001520: a836 0359 b1b2 1025 5534 0159 5263 0288  .6.Y...%U4.YRc..
-00001530: 1089 101c 8108 3990 8c23 2529 4a52 292e  ......9..#%)JR).
-00001540: 2553 2232 c1b0 230d f4c2 1281 2eb2 b1f4  %S"2..#.........
-00001550: 3401 c3b3 81d7 4443 8142 41b3 c312 1a13  4.....DC.BA.....
-00001560: 2014 6680 89b3 b310 8109 5236 8204 5912   .f.......R6..Y.
-00001570: 8122 b18a f734 01c4 1281 30b4 b181 f2b4  ."...4....0.....
-00001580: 3403 5f4b 2cc5 b5b3 d744 5312 1a13 2014  4._K,....DS... .
-00001590: 6680 89b5 b510 6980 3682 0459 4251 121a  f.....i.6..YBQ..
-000015a0: 1320 1466 8089 b5b5 1069 8136 8204 5942  . .f.....i.6..YB
-000015b0: 1251 6384 3831 1481 0a25 909b 2e2c 2e25  .Qc.81...%...,.%
-000015c0: 2280 1081 0b2a 011b 810c 1c81 0bc1 5910  "....*........Y.
-000015d0: 810d b114 810e 3600 dd44 5f80 1081 0f2a  ......6..D_....*
-000015e0: 011b 810d 1c81 0fc2 59b0 51de 4442 5163  ........Y.Q.DBQc
-000015f0: b2b0 1081 1052 3482 0159 5163 8418 eb81  .....R4..YQc....
-00001600: 0116 3c3e 3f3d 90b2 8007 282b 3612 1a13  ..<>?=....(+6...
-00001610: 3351 de44 6112 1f12 2912 3512 312b 04c3  3Q.Da...).5.1+..
-00001620: 121a b322 8100 2280 4010 3db2 103e b010  ..."..".@.=..>..
-00001630: 3fb1 3486 0359 121a 1333 1440 3600 5951  ?.4..Y...3.@6.YQ
-00001640: 6382 40a9 0114 4181 2690 c060 4023 252a  c.@...A.&..`@#%*
-00001650: 2302 c1b0 b1dd 444a 121a 1333 1441 b036  #.....DJ...3.A.6
-00001660: 0163 2303 1424 b0b1 3602 6381 7891 0112  .c#..$..6.c.x...
-00001670: 4281 2790 cc60 2027 29b0 121a 1333 1843  B.'..` ')....3.C
-00001680: 121a 1333 1440 3600 5910 4463 8654 c903  ...3.@6.Y.Dc.T..
-00001690: 9e01 4581 2690 d660 6027 252e 4825 425a  ..E.&..``'%.H%BZ
-000016a0: 3000 0325 0014 2c36 00c1 b180 5527 0310  0..%..,6....U'..
-000016b0: 4614 2eb1 8151 2e02 5536 0127 0012 1a13  F....Q..U6.'....
-000016c0: 3351 de44 4512 3c34 0059 4810 121a 1333  3Q.DE.<4.YH....3
-000016d0: 1447 b0b3 2000 0236 0159 4a1a 5712 8124  .G.. ..6.YJ.W..$
-000016e0: df44 52c2 4908 1281 25b2 3401 6351 51c2  .DR.I...%.4.cQQ.
-000016f0: 2802 5d4a 015d 5263 0181 282a 0c81 1163  (.]J.]Rc..(*...c
-00001700: 6390 e412 1a13 3314 7d25 0125 0036 0263  c.....3.}%.%.6.c
-00001710: 8614 b903 1f48 8126 90eb 6060 2c42 4825  .....H.&..``,BH%
-00001720: 4259 2730 0012 8128 2500 1281 2534 0243  BY'0...(%...%4.C
-00001730: 4250 6312 1a13 3351 de44 4512 3c34 0059  BPc...3Q.DE.<4.Y
-00001740: 480f 121a 1333 1447 b020 0001 3601 594a  H....3.G. ..6.YJ
-00001750: 2157 1281 24df 4459 c149 0f12 8129 b134  !W..$.DY.I...).4
-00001760: 0159 1281 25b1 3401 6351 51c1 2801 5d4a  .Y..%.4.cQQ.(.]J
-00001770: 015d 5263 0181 1819 0a81 1163 90f9 121a  .]Rc.......c....
-00001780: 1333 1481 0425 0036 0163 5000 0a49 a005  .3...%.6.cP..I..
-00001790: 6040 2304 6382 0020 0e4a a00e 6060 292c  `@#.c.. .J..``),
-000017a0: 121a 1320 144a 3600 c0b0 144b 120a 101e  ... .J6....K....
-000017b0: 3401 3601 59b0 6350 000a 4ca0 1a60 4023  4.6.Y.cP..L..`@#
-000017c0: 0563                                     .c
+00000030: 6f63 616c 7469 6d65 000a 736c 6565 7000  ocaltime..sleep.
+00000040: 0a75 7469 6d65 0008 574c 414e 000c 5354  .utime..WLAN..ST
+00000050: 415f 4946 000e 6e65 7477 6f72 6b00 1870  A_IF..network..p
+00000060: 6879 7369 6361 6c5f 7069 6e00 1670 696e  hysical_pin..pin
+00000070: 6d61 705f 6475 6d70 0016 4c6f 6769 6361  map_dump..Logica
+00000080: 6c50 696e 7300 1069 6663 6f6e 6669 6700  lPins..ifconfig.
+00000090: 0e4e 6574 776f 726b 0014 6572 726c 6f67  .Network..errlog
+000000a0: 5f61 6464 000a 4465 6275 6700 0650 696e  _add..Debug..Pin
+000000b0: 000e 6d61 6368 696e 6500 1865 7865 635f  ..machine..exec_
+000000c0: 6c6d 5f63 6f72 6500 0e4d 616e 6167 6572  lm_core..Manager
+000000d0: 0016 5461 736b 4d61 6e61 6765 7200 186d  ..TaskManager..m
+000000e0: 656d 6f72 795f 7573 6167 6500 124c 4d5f  emory_usage..LM_
+000000f0: 7379 7374 656d 0016 4c4d 5f69 6e74 6572  system..LM_inter
+00000100: 636f 6e00 0e67 6574 5f61 6463 0010 4c4d  con..get_adc..LM
+00000110: 5f67 656e 494f 000c 5061 6765 5549 000e  _genIO..PageUI..
+00000120: 7373 6431 3330 3600 8169 146d 6963 724f  ssd1306..i.micrO
+00000130: 5320 6d73 6700 146f 6c65 6475 6962 7474  S msg..oleduibtt
+00000140: 6e00 125f 7379 735f 7061 6765 000e 4449  n.._sys_page..DI
+00000150: 5350 4c41 5900 0874 6578 7400 0c64 6576  SPLAY..text..dev
+00000160: 6669 6400 0820 207b 7d00 8129 0e70 6572  fid..  {}..).per
+00000170: 6365 6e74 0010 6d65 6d5f 7573 6564 000e  cent..mem_used..
+00000180: 2020 563a 207b 7d00 0e76 6572 7369 6f6e    V: {}..version
+00000190: 001e 5f69 6e74 6572 636f 6e5f 6361 6368  .._intercon_cach
+000001a0: 6500 0864 756d 7000 814d 8223 022e 0081  e..dump..M.#....
+000001b0: 510c 207b 7d20 7b7d 000a 456d 7074 7900  Q. {} {}..Empty.
+000001c0: 1e5f 6d69 6372 6f73 5f77 656c 636f 6d65  ._micros_welcome
+000001d0: 0014 6d69 6372 4f53 2047 5549 0016 5041  ..micrOS GUI..PA
+000001e0: 4745 5f55 495f 4f42 4a00 2473 6574 5f70  GE_UI_OBJ.$set_p
+000001f0: 7265 7373 5f63 616c 6c62 6163 6b00 125f  ress_callback.._
+00000200: 6164 635f 7061 6765 0008 6e75 6c6c 0008  adc_page..null..
+00000210: 766f 6c74 000c 6765 6e61 6463 0002 7000  volt..genadc..p.
+00000220: 087b 7d20 2500 087b 7d20 5600 0c70 6167  .{} %..{} V..pag
+00000230: 6575 6900 0870 6167 6500 0e70 7772 5f73  eui..page..pwr_s
+00000240: 6563 0012 6f6c 6564 5f74 7970 6500 1273  ec..oled_type..s
+00000250: 686f 775f 7061 6765 000e 636f 6e74 726f  how_page..contro
+00000260: 6c00 0c6d 7367 626f 7800 1073 686f 775f  l..msgbox..show_
+00000270: 6d73 6700 1053 686f 7720 6d73 6700 2069  msg..Show msg. i
+00000280: 6e74 6572 636f 6e5f 6765 6e70 6167 6500  ntercon_genpage.
+00000290: 0910 6164 645f 7061 6765 0016 636d 645f  ..add_page..cmd_
+000002a0: 6765 6e70 6167 6500 0a6c 6d64 6570 000c  genpage..lmdep..
+000002b0: 7069 6e6d 6170 0082 3f08 6865 6c70 0023  pinmap..?.help.#
+000002c0: 8231 0e4c 4d5f 6f6c 6564 001c 4c4d 5f6f  .1.LM_oled..LM_o
+000002d0: 6c65 645f 7368 3131 3036 0024 7061 6765  led_sh1106.$page
+000002e0: 5f63 616c 6c62 6163 6b5f 6c69 7374 0016  _callback_list..
+000002f0: 6163 7469 7665 5f70 6167 6500 0a77 6964  active_page..wid
+00000300: 7468 000c 6865 6967 6874 0018 626c 696e  th..height..blin
+00000310: 6b5f 6566 6665 6374 0014 6f6c 6564 5f73  k_effect..oled_s
+00000320: 7461 7465 0026 6274 746e 5f70 7265 7373  tate.&bttn_press
+00000330: 5f63 616c 6c62 6163 6b00 1c6f 7065 6e5f  _callback..open_
+00000340: 696e 7465 7263 6f6e 7300 066e 2f61 000e  intercons..n/a..
+00000350: 636d 645f 6f75 7400 1863 6d64 5f74 6173  cmd_out..cmd_tas
+00000360: 6b5f 7461 6700 0c69 7271 5f6f 6b00 265f  k_tag..irq_ok.&_
+00000370: 5f63 7265 6174 655f 6275 7474 6f6e 5f69  _create_button_i
+00000380: 7271 0012 7469 6d69 7271 7365 7100 1e70  rq..timirqseq..p
+00000390: 7772 5f73 6176 6572 5f73 7461 7465 001a  wr_saver_state..
+000003a0: 5f5f 7061 6765 5f68 6561 6465 7200 0630  __page_header..0
+000003b0: 7b7d 0002 3000 0b02 2100 145f 5f70 6167  {}..0...!..__pag
+000003c0: 655f 6261 7200 0872 6563 7400 105f 5f6d  e_bar..rect..__m
+000003d0: 7367 626f 7800 0e70 6f77 6572 6f6e 000a  sgbox..poweron..
+000003e0: 7374 6174 6500 0449 4e00 1250 554c 4c5f  state..IN..PULL_
+000003f0: 444f 574e 0006 6972 7100 0e74 7269 6767  DOWN..irq..trigg
+00000400: 6572 0014 4952 515f 5249 5349 4e47 000e  er..IRQ_RISING..
+00000410: 6861 6e64 6c65 7200 185f 5f70 6f77 6572  handler..__power
+00000420: 5f73 6176 6500 066f 6666 0079 0a63 6c65  _save..off.y.cle
+00000430: 616e 0008 7368 6f77 000a 7072 6573 7300  an..show..press.
+00000440: 245f 7061 6765 5f62 7574 746f 6e5f 7072  $_page_button_pr
+00000450: 6573 7300 0870 7265 7600 046f 6e00 1070  ess..prev..on..p
+00000460: 6f77 6572 6f66 6600 0653 3a31 0006 533a  oweroff..S:1..S:
+00000470: 3000 125f 636d 645f 7465 7874 001a 696e  0.._cmd_text..in
+00000480: 7465 7263 6f6e 5f70 6167 6500 0674 6167  tercon_page..tag
+00000490: 0082 0303 06c2 ba43 0002 4300 086b 696c  .......C..C..kil
+000004a0: 6c00 1a63 6d64 5f63 616c 6c5f 7061 6765  l..cmd_call_page
+000004b0: 0014 3c6c 6973 7463 6f6d 703e 000e 5f62  ..<listcomp>.._b
+000004c0: 7574 746f 6e00 1048 454c 4c4f 203a 4400  utton..HELLO :D.
+000004d0: 165f 5f76 6973 7561 6c69 7a65 0008 6669  .__visualize..fi
+000004e0: 6c6c 0020 5f5f 7267 625f 6272 6967 6874  ll. __rgb_bright
+000004f0: 6e65 7373 000e 6d6f 6475 6c65 7300 0673  ness..modules..s
+00000500: 7973 000c 4c4d 5f72 6762 0081 5514 6272  ys..LM_rgb..U.br
+00000510: 6967 6874 6e65 7373 000c 736d 6f6f 7468  ightness..smooth
+00000520: 0010 3c6c 616d 6264 613e 0006 7275 6e00  ..<lambda>..run.
+00000530: 165f 5f64 7261 775f 7273 7369 000c 7374  .__draw_rssi..st
+00000540: 6174 7573 0008 7273 7369 0008 6c69 6e65  atus..rssi..line
+00000550: 0012 5f5f 7077 725f 6f66 6600 105f 5f65  ..__pwr_off..__e
+00000560: 6666 6563 7400 1073 656e 645f 636d 6400  ffect..send_cmd.
+00000570: 0e76 6572 6469 6374 0082 010e 5f62 7566  .verdict...._buf
+00000580: 6665 7200 0c6d 7367 6f62 6a00 1049 6e74  fer..msgobj..Int
+00000590: 6572 436f 6e00 2f2d 3581 3d14 6c69 6e65  erCon./-5.=.line
+000005a0: 5f6c 696d 6974 0082 3349 822f 0663 6d64  _limit..3I./.cmd
+000005b0: 0006 6d73 6700 8143 8177 8213 1c70 6167  ..msg..C.w...pag
+000005c0: 655f 6361 6c6c 6261 636b 7300 0277 0002  e_callbacks..w..
+000005d0: 6800 820d 8157 8179 0c70 696e 6b65 7900  h....W.y.pinkey.
+000005e0: 1a70 6167 655f 6361 6c6c 6261 636b 0010  .page_callback..
+000005f0: 6361 6c6c 6261 636b 0002 7800 0279 0008  callback..x..y..
+00000600: 686f 7374 0006 7069 6e00 050c 2020 7b7d  host..pin...  {}
+00000610: 2520 287b 7d6b 6229 0005 0e49 6e74 6572  % ({}kb)...Inter
+00000620: 436f 6e20 6361 6368 6500 0a05 0504 6e65  Con cache.....ne
+00000630: 7874 0005 0470 7265 7600 0505 7072 6573  xt...prev...pres
+00000640: 7300 0502 6f6e 0005 036f 6666 0005 1c49  s...on...off...I
+00000650: 6e76 616c 6964 2063 6f6d 6d61 6e64 207b  nvalid command {
+00000660: 7d21 2048 696e 743a 207b 7d00 0a03 0504  }! Hint: {}.....
+00000670: 6f6c 6564 0005 0869 6e74 6572 636f 6e00  oled...intercon.
+00000680: 0505 6765 6e49 4f00 0a06 0541 7061 6765  ..genIO....Apage
+00000690: 7569 2070 6167 653d 3020 7077 725f 7365  ui page=0 pwr_se
+000006a0: 633d 4e6f 6e65 2f69 6e74 2873 6563 2920  c=None/int(sec) 
+000006b0: 6f6c 6564 5f74 7970 653d 2273 7364 3133  oled_type="ssd13
+000006c0: 3036 206f 7220 7368 3131 3036 2200 051e  06 or sh1106"...
+000006d0: 636f 6e74 726f 6c20 6e65 7874 2f70 7265  control next/pre
+000006e0: 762f 7072 6573 732f 6f6e 2f6f 6666 0005  v/press/on/off..
+000006f0: 0c6d 7367 626f 7820 226d 7367 2200 0527  .msgbox "msg"..'
+00000700: 696e 7465 7263 6f6e 5f67 656e 7061 6765  intercon_genpage
+00000710: 2022 686f 7374 2220 2263 6d64 2220 7275   "host" "cmd" ru
+00000720: 6e3d 4661 6c73 6500 051b 636d 645f 6765  n=False...cmd_ge
+00000730: 6e70 6167 6520 2263 6d64 2220 7275 6e3d  npage "cmd" run=
+00000740: 4661 6c73 6500 0506 7069 6e6d 6170 000a  False...pinmap..
+00000750: 0205 0773 7364 3133 3036 0005 0673 6831  ...ssd1306...sh1
+00000760: 3130 3600 051d 4f6c 6564 2055 4920 756e  106...Oled UI un
+00000770: 6b6e 6f77 6e20 6f6c 6564 5f74 7970 653a  known oled_type:
+00000780: 207b 7d00 050e 7b7d 207b 7d20 7b7d 3a7b   {}...{} {} {}:{
+00000790: 7d3a 7b7d 0005 165b 4552 525d 2042 7574  }:{}...[ERR] But
+000007a0: 746f 6e20 4952 513a 7b7d 207b 7d00 0510  ton IRQ:{} {}...
+000007b0: 7061 6765 3a20 7b7d 2070 7772 3a20 7b7d  page: {} pwr: {}
+000007c0: 000a 0207 0238 3407 0234 350a 0207 0135  .....84..45....5
+000007d0: 0702 3132 0804 302e 3031 050c 5461 736b  ..12..0.01..Task
+000007e0: 2069 7320 4275 7379 0094 041c 5601 2c32   is Busy....V.,2
+000007f0: 3232 2c2c 2c32 224f 2622 4a27 224f 8607  22,,,2"O&"J'"O..
+00000800: 9945 840d 8813 840f 842a 8b0e 890c 890a  .E.......*......
+00000810: 8916 891b 8409 840c 8010 022a 011b 031c  ...........*....
+00000820: 0216 0259 8010 0410 052a 021b 061c 0416  ...Y.....*......
+00000830: 041c 0516 0559 8010 0710 082a 021b 091c  .....Y.....*....
+00000840: 0716 071c 0816 0859 8010 0a10 0b2a 021b  .......Y.....*..
+00000850: 0c1c 0a16 0a1c 0b16 0b59 8010 0d2a 011b  .........Y...*..
+00000860: 0e1c 0d16 0d59 8010 0f2a 011b 101c 0f16  .....Y...*......
+00000870: 0f59 8010 112a 011b 121c 1116 1159 8010  .Y...*.......Y..
+00000880: 1310 142a 021b 151c 1316 131c 1416 1459  ...*...........Y
+00000890: 480e 8010 162a 011b 171c 1616 1659 4a07  H....*.......YJ.
+000008a0: 5951 1616 4a01 5d48 0980 511b 1816 811f  YQ..J.]H..Q.....
+000008b0: 4a08 5951 1681 1f4a 015d 480e 8010 192a  J.YQ...J.]H....*
+000008c0: 011b 1a1c 1916 1959 4a07 5951 1619 4a01  .......YJ.YQ..J.
+000008d0: 5d54 3200 101b 3402 161b 3201 1620 832a  ]T2...4...2.. .*
+000008e0: 0153 3302 162a 3203 1632 3204 1636 5110  .S3..*2..22..6Q.
+000008f0: 1c80 2a03 5333 0516 3d10 1d2a 0153 3306  ..*.S3..=..*.S3.
+00000900: 1642 101e 2a01 5333 0716 4351 502a 0253  .B..*.S3..CQP*.S
+00000910: 3308 1646 5150 2a02 5333 0916 4932 0a16  3..FQP*.S3..I2..
+00000920: 4a32 0b16 4b32 0c16 4d51 630d 880c 103e  J2..K2..MQc....>
+00000930: 1b8b 1b23 438b 2a84 2384 0a84 1b89 0e84  ...#C.*.#.......
+00000940: 0e64 6084 0f84 2284 0d84 1384 1288 2911  .d`...".......).
+00000950: 8120 1681 2110 1b16 8122 5116 3451 1621  . ..!...."Q.4Q.!
+00000960: 8051 101c 2a03 5333 0016 4e32 0116 6132  .Q..*.S3..N2..a2
+00000970: 0216 6632 0316 6810 1f2a 0153 3304 165e  ..f2..h..*.S3..^
+00000980: 3205 1671 3206 1648 3207 1641 3208 1642  2..q2..H2..A2..B
+00000990: 3209 1677 320a 1635 320b 167d 502a 0153  2..w2..52..}P*.S
+000009a0: 330c 167e 502a 0153 330d 1681 0551 630e  3..~P*.S3....Qc.
+000009b0: 8b78 db85 014a 4e81 2c81 2d81 2e81 2f3e  .x...JN.,.-.../>
+000009c0: 3f40 801f 8008 2a2a 4725 472c 2d24 2424  ?@....**G%G,-$$$
+000009d0: 2424 2444 4425 2544 2446 57b6 144f 3600  $$$DD%%D$FW..O6.
+000009e0: 2306 dd44 5db6 144f 3600 101c d944 4780  #..D]..O6....DG.
+000009f0: 511b 50c7 4245 8051 1b51 c7b7 121b 1821  Q.P.BE.Q.Q.....!
+00000a00: 4259 120f 2307 1425 b636 0134 0159 1281  BY..#..%.6.4.Y..
+00000a10: 2623 0714 25b6 3601 3401 59b1 b018 52b4  &#..%.6.4.Y...R.
+00000a20: b018 53b2 b018 54b3 b018 5551 b018 4450  ..S...T...UQ..DP
+00000a30: b018 5652 b018 5751 b018 582b 00b0 1859  ..VR..WQ..X+...Y
+00000a40: 105a b018 5b51 b018 5c50 b018 5db0 145e  .Z..[Q..\P..]..^
+00000a50: 3600 59b5 1281 3012 0210 5f34 0122 8768  6.Y...0..._4.".h
+00000a60: f782 3402 b52b 03b0 1860 b012 1b18 3451  ..4..+...`....4Q
+00000a70: 638e 2c8d 1031 6181 2c80 4940 8508 8509  c.,..1a.,.I@....
+00000a80: 2224 4743 251f 211f 211f 2127 3239 00b0  "$GC%.!.!.!'29..
+00000a90: 2000 01c1 b020 0101 c248 0ab1 3400 59b2   .... ...H..4.Y.
+00000aa0: 3400 594a 0459 4a01 5d12 0434 00c3 1281  4.YJ.YJ.]..4....
+00000ab0: 3112 8127 b37b 5534 0134 0182 d744 4b10  1..'.{U4.4...DK.
+00000ac0: 6214 25b3 7b55 3601 4243 b37b 55c4 1281  b.%.{U6.BC.{U...
+00000ad0: 3112 8127 b37c 5534 0134 0182 d744 4b10  1..'.|U4.4...DK.
+00000ae0: 6214 25b3 7c55 3601 4243 b37c 55c5 1281  b.%.|U6.BC.|U...
+00000af0: 3112 8127 b37d 5534 0134 0182 d744 4b10  1..'.}U4.4...DK.
+00000b00: 6214 25b3 7d55 3601 4243 b37d 55c6 120d  b.%.}U6.BC.}U...
+00000b10: 3400 8055 c712 8131 b734 0180 d844 45b7  4..U...1.4...DE.
+00000b20: 8055 4242 1063 c725 0013 5851 de44 4410  .UBB.c.%..XQ.DD.
+00000b30: 4742 4c25 0013 5d44 4410 6442 4210 65c8  GBL%..]DD.dBB.e.
+00000b40: 121b 1321 1422 2308 1425 b7b8 b4b5 b636  ...!."#..%.....6
+00000b50: 0580 8036 0359 5163 0288 1861 1481 1464  ...6.YQc...a...d
+00000b60: 804c 2f2f 3836 2612 0712 0834 0114 8115  .L//86&....4....
+00000b70: 1081 1636 01c1 1281 30b1 2280 5bf2 9ef7  ...6....0.".[...
+00000b80: 88f4 3401 c212 1b13 2114 8117 2500 1354  ..4.....!...%..T
+00000b90: 8af3 8825 0013 5488 f388 3604 5912 1b13  ...%..T...6.Y...
+00000ba0: 2114 8117 2500 1354 91f3 8125 0013 5481  !...%..T...%..T.
+00000bb0: 3604 59b2 8042 5e57 c312 1b13 2114 8117  6.Y..B^W....!...
+00000bc0: 2280 76b3 f388 b3f3 2280 78b3 f288 b3f3  ".v.....".x.....
+00000bd0: 3604 5981 e558 5ad7 431d 5959 5163 8550  6.Y..XZ.C.YYQc.P
+00000be0: 7916 8118 6480 5422 2925 222c 269d c125  y...d.T")%",&..%
+00000bf0: 0013 6030 03c2 c3c4 b251 de44 4251 6312  ..`0.....Q.DBQc.
+00000c00: 8130 b4b2 f781 3402 88f4 c5b5 8042 6257  .0....4......BbW
+00000c10: c612 1b13 2114 8117 2500 1354 b1f3 86b6  ....!...%..T....
+00000c20: f325 0013 54b1 f382 f386 b6f3 3604 5981  .%..T.......6.Y.
+00000c30: e558 5ad7 4319 5959 5163 8618 6914 6681  .XZ.C.YYQc..i.f.
+00000c40: 2c80 6c20 2950 2e55 1281 31b0 1352 3401  ,.l )P.U..1..R4.
+00000c50: c112 8123 1281 30b0 1354 b1f7 3401 3401  ...#..0..T..4.4.
+00000c60: c212 8132 80b0 1354 b234 035f 4b16 c312  ...2...T.4._K...
+00000c70: 1b13 2114 67b3 b013 5585 f3b2 81f3 8436  ..!.g...U......6
+00000c80: 0459 4228 121b 1321 1467 b013 53b2 f481  .YB(...!.g..S...
+00000c90: f2b0 1355 84f3 b282 f382 3604 5951 6389  ...U......6.YQc.
+00000ca0: 3c59 2968 812c 8076 6540 2545 2246 2945  <Y)h.,.ve@%E"F)E
+00000cb0: 5324 4a31 2754 2c00 b020 0001 c125 0013  S$J1'T,.. ...%..
+00000cc0: 44c2 b251 de44 4250 6325 0013 5743 4e12  D..Q.DBPc%..WCN.
+00000cd0: 1b13 2114 6936 0059 5225 0018 5712 1b13  ..!.i6.YR%..W...
+00000ce0: 2114 678a 8f22 806c a810 6a81 3682 0459  !.g..".l..j.6..Y
+00000cf0: b134 0059 1281 31b2 3401 8ad8 446c 121b  .4.Y..1.4...Dl..
+00000d00: 1321 1422 b280 8a2e 0255 8f99 3603 59b2  .!.".....U..6.Y.
+00000d10: 8a51 2e02 55c3 1281 31b3 3401 8cd8 4448  .Q..U...1.4...DH
+00000d20: b351 8b2e 0255 4241 b3c2 121b 1321 1422  .Q...UBA.....!."
+00000d30: b28f a836 0359 5263 0184 4051 0e81 1964  ...6.YRc..@Q...d
+00000d40: 8077 293a 2500 1356 d325 0018 5612 1b13  .w):%..V.%..V...
+00000d50: 2114 6722 806a 9189 8510 6a81 1081 0a25  !.g".j....j....%
+00000d60: 0013 5636 8404 5912 1b13 2114 6722 806a  ..V6..Y...!.g".j
+00000d70: 9889 8910 6a81 1081 0a25 0013 5636 8404  ....j....%..V6..
+00000d80: 5951 6386 6ce2 0321 5e81 2c81 3380 9120  YQc.l..!^.,.3.. 
+00000d90: 2252 2922 2f23 4e33 0048 0812 0ab1 3401  "R)"/#N3.H....4.
+00000da0: c24a 2457 1281 26df 445c c349 1223 0914  .J$W..&.D\.I.#..
+00000db0: 25b1 b336 02c4 51c2 120f b434 0159 5151  %..6..Q....4.YQQ
+00000dc0: c328 035d 4a01 5db2 4466 1211 b212 1113  .(.]J.].Df......
+00000dd0: 6b12 1113 6c34 03c5 b514 6d10 6e12 1113  k...l4....m.n...
+00000de0: 6f10 70b0 2000 0136 8400 5952 2500 185d  o.p. ..6..YR%..]
+00000df0: 5163 0181 1022 0e81 1264 8139 809b 2500  Qc..."...d.9..%.
+00000e00: 1442 1076 3601 6383 5831 1671 812c 809f  .B.v6.c.X1.q.,..
+00000e10: 2845 2225 4a28 b013 6030 03c1 c2c3 b151  (E"%J(..`0.....Q
+00000e20: de44 4251 63b3 80d8 444a b3b2 f3b0 1360  .DBQc...DJ.....`
+00000e30: 8256 424e b014 4210 7236 0159 b1b0 1360  .VBN..B.r6.Y...`
+00000e40: 8256 5163 8200 2214 4881 2c81 3480 ad27  .VQc..".H.,.4..'
+00000e50: 2229 b1b0 1352 dd44 4252 63b0 1352 1473  ")...R.DBRc..R.s
+00000e60: b136 0159 5263 8658 2120 4181 2c80 b320  .6.YRc.X! A.,.. 
+00000e70: 2926 2626 2623 304a 2a29 121b 1321 1474  )&&&&#0J*)...!.t
+00000e80: 3600 59b0 1468 3600 c1b0 1357 44c2 80b0  6.Y..h6....WD...
+00000e90: 1461 3600 59b0 1466 3600 59b1 4364 b013  .a6.Y..f6.Y.Cd..
+00000ea0: 5312 8131 b013 5234 0181 f3d8 444a b013  S..1..R4....DJ..
+00000eb0: 5280 5534 0059 424a b013 52b0 1353 5534  R.U4.YBJ..R..SU4
+00000ec0: 0059 121b 1321 1475 3600 59b0 1471 3600  .Y...!.u6.Y..q6.
+00000ed0: 5951 638f 502a 4642 812c 8128 80c3 4a44  YQc.P*FB.,.(..JD
+00000ee0: 2a20 292a 2029 3024 2624 282a 2029 272d  * )* )0$&$(* )'-
+00000ef0: 2624 272a 2926 2a29 2426 b013 6080 55b0  &$'*)&*)$&..`.U.
+00000f00: 1360 8256 51b0 1844 b114 4f36 0010 76d9  .`.VQ..D..O6..v.
+00000f10: 4449 b014 7736 0059 42a7 81b1 144f 3600  DI..w6.YB....O6.
+00000f20: 101d d944 6fb0 5713 5381 e55a 1853 b013  ...Do.W.S..Z.S..
+00000f30: 5312 8131 b013 5234 0181 f3d8 4444 80b0  S..1..R4....DD..
+00000f40: 1853 b014 4136 0059 51b0 1858 105a b018  .S..A6.YQ..X.Z..
+00000f50: 5b42 ee80 b114 4f36 0010 78d9 446e b057  [B....O6..x.Dn.W
+00000f60: 1353 81e6 5a18 53b0 1353 80d7 444d 1281  .S..Z.S..S..DM..
+00000f70: 31b0 1352 3401 81f3 b018 53b0 1441 3600  1..R4.....S..A6.
+00000f80: 5951 b018 5810 5ab0 185b 4276 b114 4f36  YQ..X.Z..[Bv..O6
+00000f90: 0010 79d9 444f 121b 1321 1469 3600 5952  ..y.DO...!.i6.YR
+00000fa0: b018 5742 5db1 144f 3600 1072 d944 5312  ..WB]..O6..r.DS.
+00000fb0: 1b13 2114 7a36 0059 50b0 1857 51b0 1858  ..!.z6.YP..WQ..X
+00000fc0: 4240 230a 1425 b013 53b0 1357 3602 6382  B@#..%..S..W6.c.
+00000fd0: 0811 1477 812c 80e4 6040 2742 46b0 1358  ...w.,..`@'BF..X
+00000fe0: 51de 4442 5163 b014 5836 0059 51b0 1858  Q.DBQc..X6.YQ..X
+00000ff0: 5163 8720 5222 3581 2c81 3580 f120 6426  Qc. R"5.,.5.. d&
+00001000: 316d 2826 2866 27b1 b018 5823 0b30 02c2  1m(&(f'...X#.0..
+00001010: c312 1b13 2114 67b2 83f3 b383 f3ae 8e36  ....!.g........6
+00001020: 0459 121b 1321 1422 1076 b2b3 3603 5910  .Y...!.".v..6.Y.
+00001030: 7bb0 135b dd44 4652 b018 5642 5510 7cb0  {..[.DFR..VBU.|.
+00001040: 135b dd44 4650 b018 5642 47b0 1356 d3b0  .[.DFP..VBG..V..
+00001050: 1856 121b 1321 1467 b282 f3b3 82f3 ac8c  .V...!.g........
+00001060: b013 5636 0559 5163 8a00 4b22 7d81 2c81  ..V6.YQc..K"}.,.
+00001070: 3681 3790 0460 2034 2d35 335b 5712 8123  6.7..` 4-53[W..#
+00001080: 1281 30b0 1354 b1f3 88f7 3401 3401 81f3  ..0..T....4.4...
+00001090: c312 8131 b013 5b34 01b3 d844 da80 121b  ...1..[4...D....
+000010a0: 1321 1422 b013 5b80 b32e 0255 b1b2 8af2  .!."..[....U....
+000010b0: 3603 5912 8131 b013 5bb3 512e 0255 3401  6.Y..1..[.Q..U4.
+000010c0: b385 f3d8 445b 121b 1321 1422 b013 5bb3  ....D[...!."..[.
+000010d0: 82b3 f485 f32e 0255 b1b2 94f2 3603 5942  .......U....6.YB
+000010e0: 5512 1b13 2114 22b0 135b b351 2e02 55b1  U...!."..[.Q..U.
+000010f0: b294 f236 0359 4250 121b 1321 1422 b013  ...6.YBP...!."..
+00001100: 5bb1 b28a f236 0359 5163 8d34 e805 b880  [....6.YQc.4....
+00001110: 017e 812c 8138 8128 8113 9016 2046 880e  .~.,.8.(.... F..
+00001120: 2942 2d4f 2a3f 5050 5145 4b48 2400 0102  )B-O*?PPQEKH$...
+00001130: 0323 0c30 02c4 c5b0 b1b2 b320 0004 c625  .#.0....... ...%
+00001140: 0125 0013 59dd 4442 5163 121b 1321 1422  .%..Y.DBQc...!."
+00001150: 2501 80b5 3603 5912 1b13 2114 2225 02b4  %...6.Y...!."%..
+00001160: b58a f236 0359 2500 135c 51de d344 d580  ...6.Y%..\Q..D..
+00001170: 1281 2712 1434 0014 7510 7f25 0013 5c36  ..'..4..u..%..\6
+00001180: 8200 3401 1481 0010 4710 8101 3602 c7b7  ..4.....G...6...
+00001190: 51de d344 7012 8131 b734 0180 d844 66b7  Q..Dp..1.4...Df.
+000011a0: 1481 0010 8102 1081 0336 0225 0018 5b12  .........6.%..[.
+000011b0: 1434 0014 8104 107f 2500 135c 3682 0059  .4......%..\6..Y
+000011c0: 5125 0018 5c25 0014 7db4 b58a f236 0259  Q%..\%..}....6.Y
+000011d0: 2500 1435 b636 0159 2503 4444 b634 0059  %..5.6.Y%.DD.4.Y
+000011e0: 5163 0187 40d8 061e 8107 6464 6464 901b  Qc..@.....dddd..
+000011f0: 2b42 2d28 2e55 3325 0013 5914 7325 0136  +B-(.U3%..Y.s%.6
+00001200: 0159 482e 1281 1f14 811a 2501 2502 3602  .YH.......%.%.6.
+00001210: c4b4 107f 5525 0018 5c23 0eb4 1081 1b55  ....U%..\#.....U
+00001220: dd44 4d25 0343 49b4 1081 1b55 2500 185b  .DM%.CI....U%..[
+00001230: 4a1d 5712 8126 df44 55c5 490b 1281 27b5  J.W..&.DU.I...'.
+00001240: 3401 2500 185b 5151 c528 055d 4a01 5d25  4.%..[QQ.(.]J.]%
+00001250: 0013 5914 811c 2501 3601 5951 6385 2cdb  ..Y...%.6.YQc.,.
+00001260: 01a9 0181 0581 2c81 2881 1390 3f20 4666  ......,.(...? Ff
+00001270: 6087 0a2d 4948 2300 0106 230c 3002 c3c4  `..-IH#...#.0...
+00001280: b020 0001 2706 b0b1 b620 0103 c512 1b13  . ..'.... ......
+00001290: 2114 2225 0180 b436 0359 2500 147d b3b4  !."%...6.Y%..}..
+000012a0: 3602 5925 0014 35b5 3601 59b2 4444 b534  6.Y%..5.6.Y.DD.4
+000012b0: 0059 5163 0284 783e 1481 1d64 8129 9043  .YQc..x>...d.).C
+000012c0: 221f 5448 2b10 8101 142f b114 4f36 0014  ".TH+..../..O6..
+000012d0: 2d36 0036 0114 8100 1047 1081 0136 0214  -6.6.....G...6..
+000012e0: 8100 1081 0210 8103 3602 2500 185b 4a14  ........6.%..[J.
+000012f0: 5712 8126 df44 4c59 b114 4f36 0025 0018  W..&.DLY..O6.%..
+00001300: 5b4a 015d 5163 8440 d302 1681 0764 6464  [J.]Qc.@.....ddd
+00001310: 9049 2022 4b58 4819 2501 144f 3600 142d  .I "KXH.%..O6..-
+00001320: 3600 c312 13b3 1081 1e25 0234 8201 594a  6........%.4..YJ
+00001330: 1d57 1281 26df 4455 c449 0b12 8127 b434  .W..&.DU.I...'.4
+00001340: 0125 0018 5b51 51c4 2804 5d4a 015d 5163  .%..[QQ.(.]J.]Qc
+00001350: 8770 4016 2090 6060 3139 2725 1f23 3712  .p@. .``19'%.#7.
+00001360: 1b13 2114 2212 0210 2334 0180 8f36 0359  ..!."...#4...6.Y
+00001370: 121b 1321 1422 1024 1425 120d 3400 8155  ...!.".$.%..4..U
+00001380: 8055 3601 8099 3603 5912 1651 ded3 4467  .U6...6.Y..Q..Dg
+00001390: 1216 3400 c012 1b13 2114 2223 0014 25b0  ..4.....!."#..%.
+000013a0: 1026 5512 8123 b010 2755 2287 68f7 3401  .&U..#..'U".h.4.
+000013b0: 3602 80a3 3603 5912 1b13 2114 2210 2814  6...6.Y...!.".(.
+000013c0: 2512 0210 2934 0136 0180 ad36 0359 5263  %...)4.6...6.YRc
+000013d0: 8b0c f901 282a 8124 906d 2722 2222 2d35  ....(*.$.m'"""-5
+000013e0: 322a 3337 2425 2922 2f12 811f 51de 4442  2*37$%)"/...Q.DB
+000013f0: 5063 8fc1 81c2 121b 1321 1422 2301 80b1  Pc.......!."#...
+00001400: 3603 5912 8125 3200 1281 1f14 2b36 0034  6.Y..%2.....+6.4
+00001410: 0134 0180 d844 da80 1281 1f14 2b36 0014  .4...D......+6..
+00001420: 2c36 005f 4b4a 3002 c3c4 b314 2d10 2e36  ,6._KJ0.....-..6
+00001430: 0180 55c3 102e 142f b414 2d10 2e36 017e  ..U..../..-..6.~
+00001440: 512e 0255 3601 c412 1b13 2114 2210 3014  Q..U6.....!.".0.
+00001450: 25b4 b336 0280 b1b2 8af4 f236 0359 b281  %..6.......6.Y..
+00001460: e5c2 b2b0 d844 4659 5959 5942 4342 b47f  .....DFYYYYBCB..
+00001470: 5263 121b 1321 1422 1031 a8b1 94f2 3603  Rc...!.".1....6.
+00001480: 5952 6301 8120 390a 8106 6490 722b 00b0  YRc.. 9...d.r+..
+00001490: 5f4b 06c1 812f 1442 3863 843c b802 1432  _K.../.B8c.<...2
+000014a0: 9080 2063 4022 2d56 3032 00c0 4819 121b  .. c@"-V02..H...
+000014b0: 1321 1422 1033 9e8f 3603 5912 1b13 3414  .!.".3..6.Y...4.
+000014c0: 35b0 3601 594a 1a57 1281 26df 4452 c149  5.6.YJ.W..&.DR.I
+000014d0: 0812 8127 b134 0163 5151 c128 015d 4a01  ...'.4.cQQ.(.]J.
+000014e0: 5d52 6301 8208 200c 8107 9082 202e 121b  ]Rc... ..... ...
+000014f0: 1321 1422 1081 08a3 9d36 0359 121b 1321  .!.".....6.Y...!
+00001500: 1475 3600 5951 6387 4c40 1e36 908f 6083  .u6.YQc.L@.6..`.
+00001510: 0f83 082d 272b 2b37 3728 3200 c032 01c1  ...-'++77(2..2..
+00001520: 2c02 1037 1026 6210 3710 3862 c212 1951  ,..7.&b.7.8b...Q
+00001530: ded3 444b 1219 120a 1039 3401 3401 c2b0  ..DK.....94.4...
+00001540: 103a b210 2655 3482 0059 121b 1321 1422  .:..&U4..Y...!."
+00001550: 103b 1425 b210 2655 3601 2280 4194 3603  .;.%..&U6.".A.6.
+00001560: 5912 1b13 2114 2210 3c14 25b2 1038 5536  Y...!.".<.%..8U6
+00001570: 0122 8041 a836 0359 b1b2 1026 5534 0159  .".A.6.Y...&U4.Y
+00001580: 5263 0288 1089 101c 8109 3a90 9323 2529  Rc........:..#%)
+00001590: 4a52 292e 2553 2232 c1b0 230d f4c2 1281  JR).%S"2..#.....
+000015a0: 30b2 b1f4 3401 c3b3 81d7 4443 8142 41b3  0...4.....DC.BA.
+000015b0: c312 1b13 2114 6780 89b3 b310 810a 5236  ....!.g.......R6
+000015c0: 8204 5912 8123 b18a f734 01c4 1281 32b4  ..Y..#...4....2.
+000015d0: b181 f2b4 3403 5f4b 2cc5 b5b3 d744 5312  ....4._K,....DS.
+000015e0: 1b13 2114 6780 89b5 b510 6a80 3682 0459  ..!.g.....j.6..Y
+000015f0: 4251 121b 1321 1467 8089 b5b5 106a 8136  BQ...!.g.....j.6
+00001600: 8204 5942 1251 6384 3831 1481 0b26 90a2  ..YB.Qc.81...&..
+00001610: 2e2c 2e25 2280 1081 0c2a 011b 810d 1c81  .,.%"....*......
+00001620: 0cc1 5910 810e b114 810f 3600 dd44 5f80  ..Y.......6..D_.
+00001630: 1081 102a 011b 810e 1c81 10c2 59b0 51de  ...*........Y.Q.
+00001640: 4442 5163 b2b0 1081 1152 3482 0159 5163  DBQc.....R4..YQc
+00001650: 8418 eb81 0116 3d3f 403e 90b9 8007 282b  ......=?@>....(+
+00001660: 3612 1b13 3451 de44 6112 2012 2a12 3612  6...4Q.Da. .*.6.
+00001670: 322b 04c3 121b b322 8100 2280 4010 3eb2  2+....."..".@.>.
+00001680: 103f b010 40b1 3486 0359 121b 1334 1441  .?..@.4..Y...4.A
+00001690: 3600 5951 6382 40a9 0114 4281 2890 c760  6.YQc.@...B.(..`
+000016a0: 4023 252a 2302 c1b0 b1dd 444a 121b 1334  @#%*#.....DJ...4
+000016b0: 1442 b036 0163 2303 1425 b0b1 3602 6381  .B.6.c#..%..6.c.
+000016c0: 7891 0112 4381 2990 d360 2027 29b0 121b  x...C.)..` ')...
+000016d0: 1334 1844 121b 1334 1441 3600 5910 4563  .4.D...4.A6.Y.Ec
+000016e0: 867c d282 01a3 0146 8128 8113 90dd 8007  .|.....F.(......
+000016f0: 2725 2e48 2542 5b30 0001 0425 0014 2d36  '%.H%B[0...%..-6
+00001700: 00c2 b280 5527 0410 4714 2fb2 8151 2e02  ....U'..G./..Q..
+00001710: 5536 0127 0012 1b13 3451 de44 4512 3d34  U6.'....4Q.DE.=4
+00001720: 0059 4811 121b 1334 1448 b0b1 b420 0003  .YH....4.H... ..
+00001730: 3601 594a 1a57 1281 26df 4452 c349 0812  6.YJ.W..&.DR.I..
+00001740: 8127 b334 0163 5151 c328 035d 4a01 5d52  .'.4.cQQ.(.]J.]R
+00001750: 6301 8160 430e 8112 6464 6490 ec12 1b13  c..`C...ddd.....
+00001760: 3414 7e25 0225 0010 8113 2501 3682 0263  4.~%.%....%.6..c
+00001770: 8644 c282 01a2 0149 8128 8113 90f3 8007  .D.....I.(......
+00001780: 2c42 4825 425a 2730 0001 1281 2a25 0012  ,BH%BZ'0....*%..
+00001790: 8127 3402 4342 5063 121b 1334 51de 4445  .'4.CBPc...4Q.DE
+000017a0: 123d 3400 5948 1012 1b13 3414 48b0 b120  .=4.YH....4.H.. 
+000017b0: 0002 3601 594a 2157 1281 26df 4459 c249  ..6.YJ!W..&.DY.I
+000017c0: 0f12 812b b234 0159 1281 27b2 3401 6351  ...+.4.Y..'.4.cQ
+000017d0: 51c2 2802 5d4a 015d 5263 0181 5032 0c81  Q.(.]J.]Rc..P2..
+000017e0: 1264 64a0 0212 1b13 3414 8105 2500 1081  .dd.....4...%...
+000017f0: 1325 0136 8201 6350 000a 4aa0 0e60 4023  .%.6..cP..J..`@#
+00001800: 0463 8200 200e 4ba0 1760 6029 2c12 1b13  .c.. .K..``),...
+00001810: 2114 4b36 00c0 b014 4c12 0b10 1f34 0136  !.K6....L....4.6
+00001820: 0159 b063 5000 0a4d a023 6040 2305 63    .Y.cP..M.#`@#.c
```

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_pet_feeder.py` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_ph_sensor.py` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_presence.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_presence.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_rencoder.py` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_rgb.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_rgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_roboarm.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_roboarm.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_robustness.py` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_servo.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_servo.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_stepper.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_stepper.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_switch.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_switch.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_system.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_system.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_telegram.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_telegram.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_tinyrgb.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LM_tinyrgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LP_esp32.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LP_esp32.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LP_esp32s2.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LP_esp32s2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LP_esp32s3.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LP_esp32s3.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LogicalPins.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/LogicalPins.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Network.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Network.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Notify.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Notify.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Scheduler.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Scheduler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/SocketServer.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/SocketServer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/TaskManager.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/TaskManager.mpy`

 * *Files 3% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 00000770: 7374 6f70 7065 643a 207b 7d00 0541 496e  stopped: {}..AIn
 00000780: 7661 6c69 6420 7461 736b 2063 6d64 2120  valid task cmd! 
 00000790: 4865 6c70 3a20 7461 736b 206c 6973 7420  Help: task list 
 000007a0: 2f20 6b69 6c6c 203c 7461 736b 4944 3e20  / kill <taskID> 
 000007b0: 2f20 7368 6f77 203c 7461 736b 4944 3e00  / show <taskID>.
 000007c0: 0513 5b45 5252 5d20 5461 736b 206b 696c  ..[ERR] Task kil
 000007d0: 6c3a 207b 7d00 8c54 2436 0180 0e26 2c2c  l: {}..T$6...&,,
-000007e0: 2c32 2c52 224f 278f 0789 9089 b484 1484  ,2,R"O'.........
+000007e0: 2c32 2c52 224f 278f 0789 9089 b584 1484  ,2,R"O'.........
 000007f0: 0d88 4084 5180 511b 0216 7f80 1003 2a01  ..@.Q.Q.......*.
 00000800: 1b04 1c03 1603 5980 1005 2a01 1b06 1c05  ......Y...*.....
 00000810: 1605 5980 1007 2a01 1b08 1c07 1607 5980  ..Y...*.......Y.
 00000820: 1009 100a 2a02 1b0b 1c09 1609 1c0a 160a  ....*...........
 00000830: 5980 100c 2a01 1b0d 1c0c 160c 5980 100e  Y...*.......Y...
 00000840: 100f 2a02 1b10 1c0e 160e 1c0f 160f 5948  ..*...........YH
 00000850: 0e80 1011 2a01 1b12 1c11 1611 594a 1759  ....*.......YJ.Y
@@ -184,15 +184,15 @@
 00000b70: 4218 2500 132e 1437 3600 5951 6301 8138  B.%....76.YQc..8
 00000b80: 320c 695b 8116 80a0 1281 1f25 0010 30b1  2.i[.......%..0.
 00000b90: 1468 3600 3403 6383 48c1 020e 4581 0b80  .h6.4.c.H...E...
 00000ba0: a622 5648 0cb0 1436 1046 5236 8200 594a  ."VH...6.FR6..YJ
 00000bb0: 1f57 1281 05df 4457 c149 0d12 0a23 0f14  .W....DW.I...#..
 00000bc0: 1cb1 3601 3401 5951 51c1 2801 5d4a 015d  ..6.4.YQQ.(.]J.]
 00000bd0: 5163 8a74 2039 158b b223 2843 8610 8e07  Qc.t 9...#(C....
-00000be0: 6940 890c 8915 8f0d 890f 890f 8910 8920  i@............. 
+00000be0: 6940 890c 8916 8f0d 890f 890f 8910 8920  i@............. 
 00000bf0: 890b 0011 8100 1681 0110 1516 8102 5116  ..............Q.
 00000c00: 4811 0c10 1634 0116 5180 1652 b020 0001  H....4..Q..R. ..
 00000c10: 1647 1181 0351 512a 0253 3301 3401 164a  .G...QQ*.S3.4..J
 00000c20: 1181 0332 0234 0116 4e11 8103 3203 3401  ...2.4..N...2.4.
 00000c30: 1650 1181 0332 0434 0116 4c11 8103 5150  .P...2.4..L...QP
 00000c40: 512a 0353 3305 3401 163e 1181 0332 0634  Q*.S3.4..>...2.4
 00000c50: 0116 5511 8103 3207 3401 165a 1181 0332  ..U...2.4..Z...2
@@ -208,150 +208,151 @@
 00000cf0: 3c18 064e 80d0 1281 1232 0012 1413 3314  <..N.....2....3.
 00000d00: 4f36 0034 0134 0163 0182 2849 087b 5b80  O6.4.4.c..(I.{[.
 00000d10: d02b 00b0 5f4b 1830 02c1 c2b2 132e 1435  .+.._K.0.......5
 00000d20: 3600 4331 1040 b1dd 442b 812f 1442 2663  6.C1.@..D+./.B&c
 00000d30: 8308 1810 5080 d460 402d 2b26 1215 144e  ....P..`@-+&...N
 00000d40: 3600 1215 1351 db44 5823 1114 1c12 1513  6....Q.DX#......
 00000d50: 5136 01c0 120a b034 0159 1281 05b0 3401  Q6.....4.Y....4.
-00000d60: 6551 6389 00d0 421c 4c80 e060 402b 2922  eQc...B.L..`@+)"
-00000d70: 4025 4d39 5f35 1214 1333 1434 104d 3601  @%M9_5...3.4.M6.
-00000d80: c023 1214 1c36 00b0 1830 4840 120e 3400  .#...6...0H@..4.
-00000d90: c112 7f14 4322 8374 3601 5e51 6859 1281  ....C".t6.^QhY..
-00000da0: 1312 0f12 0e34 00b1 3402 2283 74f7 81f3  .....4..4.".t...
-00000db0: 2280 64f4 3401 c212 8113 1215 1352 b2f2  ".d.4........R..
-00000dc0: 82f7 3401 1215 1852 4202 4a1f 5712 8105  ..4....RB.J.W...
-00000dd0: df44 57c3 490d 120a 2313 141c b336 0134  .DW.I...#....6.4
-00000de0: 0159 5151 c328 035d 4a01 5db0 132e 1437  .YQQ.(.]J.]....7
-00000df0: 3600 5951 6384 20d8 8501 183e 4b31 5372  6.YQc. ....>K1Sr
-00000e00: 80f5 6040 4a27 3312 8114 b012 6b34 0244  ..`@J'3.....k4.D
-00000e10: 5a12 1514 5036 0059 1214 3400 143f 104b  Z...P6.Y..4..?.K
-00000e20: b010 53b2 1054 b336 8600 6312 1434 0014  ..S..T.6..c..4..
-00000e30: 3b10 4bb0 1031 b136 8400 6387 0878 1855  ;.K..1.6..c..x.U
-00000e40: 9002 6020 2c32 2f30 2c2a 2912 1513 5112  ..` ,2/0,*)...Q.
-00000e50: 1514 4e36 00f3 c023 1423 1514 1cb0 1215  ..N6...#.#......
-00000e60: 1352 3602 2316 2b03 c112 1413 3314 4f36  .R6.#.+.....3.O6
-00000e70: 005f 4b33 3002 c2c3 b313 2e14 3536 0044  ._K30.......56.D
-00000e80: 4410 5642 4210 57c4 1022 8a12 8107 b434  D.VBB.W..".....4
-00000e90: 01f3 f4c5 1058 141c b4b5 b236 03c6 b114  .....X.....6....
-00000ea0: 59b6 3601 5942 0b12 8115 b134 0163 8708  Y.6.YB.....4.c..
-00000eb0: 611e 5a31 9011 202b 2623 282c 3c29 2a23  a.Z1.. +&#(,<)*#
-00000ec0: 2212 1413 3314 34b0 5136 02c1 b151 de44  "...3.4.Q6...Q.D
-00000ed0: cb80 2b00 c2b0 141a 1040 3601 c312 1413  ..+......@6.....
-00000ee0: 3314 2636 005f 4b26 c4b4 1418 b380 5536  3.&6._K&......U6
-00000ef0: 0144 5912 8107 b334 0181 d844 4fb3 8155  .DY....4...DO..U
-00000f00: 105b d944 47b2 1459 b436 0159 4218 1281  .[.DG..Y.6.YB...
-00000f10: 07b2 3401 80d9 4443 2b00 63b2 63b0 2b01  ..4...DC+.c.c.+.
-00000f20: 6386 3071 1c5c 3190 2060 2028 2a28 2a2b  c.0q.\1. ` (*(*+
-00000f30: 2325 3712 1514 5ab0 3601 c112 8107 b134  #%7...Z.6......4
-00000f40: 0180 d944 4823 1714 1cb0 3601 6312 8107  ...DH#....6.c...
-00000f50: b134 0181 d944 4b12 1413 33b1 8055 5513  .4...DK...3..UU.
-00000f60: 3063 2b00 c2b1 5f4b 18c3 b214 5910 5d14  0c+..._K....Y.].
-00000f70: 1cb3 1214 1333 b355 1330 3602 3601 5942  .....3.U.06.6.YB
-00000f80: 2610 5e14 23b2 3601 6388 5481 1028 5f31  &.^.#.6.c.T..(_1
-00000f90: 9030 8007 8309 2822 2a2b 2a2b 2a23 2527  .0....("*+*+*#%'
-00000fa0: 302e 3200 c112 1514 5ab0 3601 c252 c312  0.2.....Z.6..R..
-00000fb0: 8107 b234 0180 d944 4bb3 2317 141c b036  ...4...DK.#....6
-00000fc0: 012a 0263 1281 07b2 3401 81d9 4455 2318  .*.c....4...DU#.
-00000fd0: 141c b280 55b3 3602 c4b1 b280 5534 01b4  ....U.6.....U4..
-00000fe0: 2a02 632b 00c5 b25f 4b18 c6b3 b1b6 3401  *.c+..._K.....4.
-00000ff0: e2c3 b514 5910 6014 1cb6 b336 0236 0159  ....Y.`....6.6.Y
-00001000: 4226 1061 141c 1062 1423 b536 0136 01c4  B&.a...b.#.6.6..
-00001010: b3b4 2a02 6301 8458 c902 127c 8120 9038  ..*.c..X...|. .8
-00001020: 2b22 592c 1214 1333 1434 b051 3602 c148  +"Y,...3.4.Q6..H
-00001030: 0fb1 51de 4442 5063 b114 4236 0063 4a21  ..Q.DBPc..B6.cJ!
-00001040: 5712 8105 df44 59c2 490f 120a 231b 141c  W....DY.I...#...
-00001050: b236 0134 0159 5063 5151 c228 025d 4a01  .6.4.YPcQQ.(.]J.
-00001060: 5d51 6384 28b8 020e 6390 5060 2257 2c48  ]Qc.(...c.P`"W,H
-00001070: 0d12 7f14 3d36 0014 6336 0059 4a2a 5712  ....=6..c6.YJ*W.
-00001080: 8105 df44 62c0 4918 120a 2319 141c b036  ...Db.I...#....6
-00001090: 0134 0159 127f 143d 3600 1464 3600 5951  .4.Y...=6..d6.YQ
-000010a0: 51c0 2800 5d4a 015d 5163 8218 2910 6581  Q.(.]J.]Qc..).e.
-000010b0: 1690 5b2c 2522 1214 1333 1434 1066 5136  ..[,%"...3.4.fQ6
-000010c0: 02c1 b151 de44 4251 63b0 b118 3051 6387  ...Q.DBQc...0Qc.
-000010d0: 3cd1 0220 1781 0490 6660 2042 2942 3027  <.. ....f` B)B0'
-000010e0: 5a2d 2c2b 4832 b014 1810 1936 0144 4252  Z-,+H2.....6.DBR
-000010f0: 6332 00b0 141a 101b 3601 5e34 015f 4b16  c2......6.^4._K.
-00001100: c112 1eb1 3401 434c 1209 2301 141c b136  ....4.CL..#....6
-00001110: 0134 0159 4228 4a2e 5712 8105 df44 66c2  .4.YB(J.W....Df.
-00001120: 491c 1209 2302 141c b0b2 3602 3401 5912  I...#.....6.4.Y.
-00001130: 0a23 0314 1cb2 3601 3401 5950 6351 51c2  .#....6.4.YPcQQ.
-00001140: 2802 5d4a 015d 5263 0182 38b9 4008 675b  (.]J.]Rc..8.@.g[
-00001150: 906f 53b0 5353 4b18 c112 8107 b134 0180  .oS.SSK......4..
-00001160: d844 33b1 1468 3600 141a 3600 6759 4226  .D3..h6...6.gYB&
-00001170: 5163 8378 c102 161d 8104 907a 6020 2228  Qc.x.......z` "(
-00001180: 4e2c 480c 1203 1217 b034 0259 5263 4a21  N,H......4.YRcJ!
-00001190: 5712 8105 df44 59c1 490f 120a 2304 141c  W....DY.I...#...
-000011a0: b136 0134 0159 5063 5151 c128 015d 4a01  .6.4.YPcQQ.(.]J.
-000011b0: 5d51 6383 3caa 019e 011e 8106 4490 8780  ]Qc.<.......D...
-000011c0: 0726 4486 2c60 2742 0001 2501 51de 4444  .&D.,`'B..%.Q.DD
-000011d0: 3200 2701 b0b1 2001 02c2 b225 0034 0144  2.'... ....%.4.D
-000011e0: 4252 6312 1f25 0025 0134 0263 0248 090a  BRc..%.%.4.c.H..
-000011f0: 6981 1690 8f51 6395 0893 124c 6a5b 5b81  i....Qc....Lj[[.
-00001200: 1790 9247 492d 2d28 2642 2528 3026 2228  ...GI--(&B%(0&"(
-00001210: 3122 2742 5028 302e 5122 5c46 2b2e 234e  1"'BP(0.Q"\F+.#N
-00001220: 4c42 1281 07b2 3401 c310 29b2 8055 d944  LB....4...)..U.D
-00001230: f380 b382 d944 6510 6bb2 8155 d944 5d10  .....De.k..U.D].
-00001240: 5e14 2312 1514 5536 0036 01c4 106c 141c  ^.#...U6.6...l..
-00001250: b436 01c4 2501 b434 0159 5263 b382 d844  .6..%..4.YRc...D
-00001260: 7b10 5fb2 8155 d944 5812 1514 5f10 31b2  {._..U.DX..._.1.
-00001270: 8255 3682 0030 02c5 c625 01b6 3401 5952  .U6..0...%..4.YR
-00001280: 6310 5cb2 8155 d944 5325 0112 1514 5c10  c.\..U.DS%....\.
-00001290: 31b2 8255 3682 0034 0159 5263 2501 231a  1..U6..4.YRc%.#.
-000012a0: 3401 5952 63b3 82d8 449d 8110 6d25 007f  4.YRc...D...m%..
-000012b0: 55dd 4493 8125 0014 6e7f 3601 c7b7 146f  U.D..%..n.6....o
-000012c0: 106d 3601 82d9 4443 5242 4150 c8b7 1470  .m6...DCRBAP...p
-000012d0: 106d 102f 3602 1468 3600 c9b9 1471 3600  .m./6..h6....q6.
-000012e0: 4448 1281 13b9 3401 4241 51c9 4812 1215  DH....4.BAQ.H...
-000012f0: 143e 2500 1053 b810 72b9 3684 01c5 4a1b  .>%..S..r.6...J.
-00001300: 5712 8105 df44 53ca 4909 2501 ba34 0159  W....DS.I.%..4.Y
-00001310: 5263 5151 ca28 0a5d 4a01 5d10 4014 2325  RcQQ.(.]J.].@.#%
-00001320: 0080 822e 0255 3601 cbb5 444e 2501 1073  .....U6...DN%..s
-00001330: 141c bb36 0134 0159 424c 2501 1074 141c  ...6.4.YBL%..t..
-00001340: bb36 0134 0159 5263 5063 9554 9e12 4b1f  .6.4.YRcPc.T..K.
-00001350: 8106 4490 c780 0883 0d85 0f27 4d2b 1f21  ..D........'M+.!
-00001360: 6327 2d42 7d2a 4c4d 5270 492b 6f2d 562a  c'-B}*LMRpI+o-V*
-00001370: 462b 2646 0a32 00c2 ba20 0101 c3b0 7f55  F+&F.2... .....U
-00001380: 1020 d9c4 b444 48b0 807f 2e02 5542 41b0  . ...DH.....UBA.
-00001390: c512 8107 b534 0182 db44 fc81 1021 141c  .....4...D...!..
-000013a0: b580 5536 01b5 8155 b210 2214 23b5 8251  ..U6...U..".#..Q
-000013b0: 2e02 5536 0134 015b 5ac6 c7c8 4890 01b6  ..U6.4.[Z...H...
-000013c0: 1205 ddd3 444d 1281 0810 2414 1cb6 3601  ....DM....$...6.
-000013d0: 3401 5948 1212 8109 1025 141c b6b7 b836  4.YH.....%.....6
-000013e0: 0334 0127 0a4a 5057 1281 05df 44c7 80c9  .4.'.JPW....D...
-000013f0: 493d b612 810a b934 01dd 446b 120a 2305  I=.....4..Dk..#.
-00001400: 141c b636 0134 0159 1281 0810 2414 1cb6  ...6.4.Y....$...
-00001410: 3601 3401 5912 8109 1025 141c b6b7 b836  6.4.Y....%.....6
-00001420: 0334 0127 0a42 4712 8105 b934 0165 5151  .4.'.BG....4.eQQ
-00001430: c928 095d 4a01 5db3 b4b7 250a 3403 270a  .(.]J.]...%.4.'.
-00001440: b112 810a 250a 3401 3401 5952 634a 4957  ....%.4.4.YRcJIW
-00001450: 1281 05df 44c0 80c9 4936 b123 0614 1cb6  ....D...I6.#....
-00001460: b7b9 3603 3401 5923 0712 810a b934 01dd  ..6.4.Y#.....4..
-00001470: 434b 2308 1281 0ab9 3401 dd44 52b6 1205  CK#.....4..DR...
-00001480: 1426 3600 dd44 4612 05b6 535b 5650 6351  .&6..DF...S[VPcQ
-00001490: 51c9 2809 5d4a 015d b123 0934 0159 b123  Q.(.]J.].#.4.Y.#
-000014a0: 0a34 0159 5263 0287 5c59 9c01 7581 1890  .4.YRc..\Y..u...
-000014b0: d022 2e2d 3625 2d2c 2a2a 0003 51c1 1076  .".-6%-,**..Q..v
-000014c0: 2500 dd43 4710 7725 00dd 4475 3200 1281  %..CG.w%..Du2...
-000014d0: 1925 0034 0134 0127 03b0 b320 0102 1281  .%.4.4.'... ....
-000014e0: 1a80 1281 0725 0334 0182 3403 3401 c1b1  .....%.4..4.4...
-000014f0: 5f4b 0ec2 2500 1470 b210 7836 0227 0042  _K..%..p..x6.'.B
-00001500: 3025 0014 7010 2210 6236 0227 0012 8114  0%..p.".b6.'....
-00001510: b112 6b34 0244 4a25 0014 1cb1 8137 0127  ..k4.DJ%.....7.'
-00001520: 0025 0063 0282 1049 087b 5b90 d22b 00b0  .%.c...I.{[..+..
-00001530: 5f4b 1530 02c1 c2b2 1077 d943 46b2 1076  _K.0.....w.CF..v
-00001540: d944 2eb1 2f14 4229 6382 286b 0c7b 5b5b  .D../.B)c.(k.{[[
-00001550: 5b90 d32b 00b2 5f4b 16c3 2500 2501 b355  [..+.._K..%.%..U
-00001560: 2501 b381 f255 81f2 2e02 552f 1442 2863  %....U....U/.B(c
-00001570: 853c c004 2479 5b81 1b81 1c81 1d90 dd2b  .<..$y[........+
-00001580: 2346 5126 2346 2c12 8114 b312 811e 3402  #FQ&#F,.......4.
-00001590: 445a b144 4612 07b3 3401 6310 5e14 2332  DZ.DF...4.c.^.#2
-000015a0: 0025 0014 4f36 0034 0136 0163 b210 7ad9  .%..O6.4.6.c..z.
-000015b0: 4455 b144 4612 07b3 3401 6310 5e14 2332  DU.DF...4.c.^.#2
-000015c0: 01b3 3401 3601 63b3 6302 8168 5908 7b5b  ..4.6.c.c..hY.{[
-000015d0: 90e1 2b00 b05f 4b10 3002 c1c2 107d 141c  ..+.._K.0....}..
-000015e0: b1b2 3602 2f14 422e 6381 4849 087b 5b90  ..6./.B.c.HI.{[.
-000015f0: e72b 00b0 5f4b 0cc1 107e 141c b136 012f  .+.._K...~...6./
-00001600: 1442 3263 8400 c902 1627 8106 a018 6040  .B2c.....'....`@
-00001610: 2228 4e2d 480c 1203 121e b034 0259 5263  "(N-H......4.YRc
-00001620: 4a22 5712 8105 df44 5ac1 4910 120a 230b  J"W....DZ.I...#.
-00001630: 141c b0b1 3602 3401 5950 6351 51c1 2801  ....6.4.YPcQQ.(.
-00001640: 5d4a 015d 5163                           ]J.]Qc
+00000d60: 6551 638a 00d0 4220 4c80 e060 402b 2922  eQc...B L..`@+)"
+00000d70: 204d 254d 391f 4135 1214 1333 1434 104d   M%M9.A5...3.4.M
+00000d80: 3601 c023 1214 1c36 00b0 1830 484e 127f  6..#...6...0HN..
+00000d90: 1443 2282 2c36 015e 5168 5912 0e34 00c1  .C".,6.^QhY..4..
+00000da0: 127f 1443 2282 2c36 015e 5168 5912 8113  ...C".,6.^QhY...
+00000db0: 120f 120e 3400 b134 0222 822c f781 f322  ....4..4.".,..."
+00000dc0: 8064 f434 01c2 1281 1312 1513 52b2 f282  .d.4........R...
+00000dd0: f734 0112 1518 5242 b47f 4a1f 5712 8105  .4....RB..J.W...
+00000de0: df44 57c3 490d 120a 2313 141c b336 0134  .DW.I...#....6.4
+00000df0: 0159 5151 c328 035d 4a01 5db0 132e 1437  .YQQ.(.]J.]....7
+00000e00: 3600 5951 6384 20d8 8501 183e 4b31 5372  6.YQc. ....>K1Sr
+00000e10: 80f6 6040 4a27 3312 8114 b012 6b34 0244  ..`@J'3.....k4.D
+00000e20: 5a12 1514 5036 0059 1214 3400 143f 104b  Z...P6.Y..4..?.K
+00000e30: b010 53b2 1054 b336 8600 6312 1434 0014  ..S..T.6..c..4..
+00000e40: 3b10 4bb0 1031 b136 8400 6387 0878 1855  ;.K..1.6..c..x.U
+00000e50: 9003 6020 2c32 2f30 2c2a 2912 1513 5112  ..` ,2/0,*)...Q.
+00000e60: 1514 4e36 00f3 c023 1423 1514 1cb0 1215  ..N6...#.#......
+00000e70: 1352 3602 2316 2b03 c112 1413 3314 4f36  .R6.#.+.....3.O6
+00000e80: 005f 4b33 3002 c2c3 b313 2e14 3536 0044  ._K30.......56.D
+00000e90: 4410 5642 4210 57c4 1022 8a12 8107 b434  D.VBB.W..".....4
+00000ea0: 01f3 f4c5 1058 141c b4b5 b236 03c6 b114  .....X.....6....
+00000eb0: 59b6 3601 5942 0b12 8115 b134 0163 8708  Y.6.YB.....4.c..
+00000ec0: 611e 5a31 9012 202b 2623 282c 3c29 2a23  a.Z1.. +&#(,<)*#
+00000ed0: 2212 1413 3314 34b0 5136 02c1 b151 de44  "...3.4.Q6...Q.D
+00000ee0: cb80 2b00 c2b0 141a 1040 3601 c312 1413  ..+......@6.....
+00000ef0: 3314 2636 005f 4b26 c4b4 1418 b380 5536  3.&6._K&......U6
+00000f00: 0144 5912 8107 b334 0181 d844 4fb3 8155  .DY....4...DO..U
+00000f10: 105b d944 47b2 1459 b436 0159 4218 1281  .[.DG..Y.6.YB...
+00000f20: 07b2 3401 80d9 4443 2b00 63b2 63b0 2b01  ..4...DC+.c.c.+.
+00000f30: 6386 3071 1c5c 3190 2160 2028 2a28 2a2b  c.0q.\1.!` (*(*+
+00000f40: 2325 3712 1514 5ab0 3601 c112 8107 b134  #%7...Z.6......4
+00000f50: 0180 d944 4823 1714 1cb0 3601 6312 8107  ...DH#....6.c...
+00000f60: b134 0181 d944 4b12 1413 33b1 8055 5513  .4...DK...3..UU.
+00000f70: 3063 2b00 c2b1 5f4b 18c3 b214 5910 5d14  0c+..._K....Y.].
+00000f80: 1cb3 1214 1333 b355 1330 3602 3601 5942  .....3.U.06.6.YB
+00000f90: 2610 5e14 23b2 3601 6388 5481 1028 5f31  &.^.#.6.c.T..(_1
+00000fa0: 9031 8007 8309 2822 2a2b 2a2b 2a23 2527  .1....("*+*+*#%'
+00000fb0: 302e 3200 c112 1514 5ab0 3601 c252 c312  0.2.....Z.6..R..
+00000fc0: 8107 b234 0180 d944 4bb3 2317 141c b036  ...4...DK.#....6
+00000fd0: 012a 0263 1281 07b2 3401 81d9 4455 2318  .*.c....4...DU#.
+00000fe0: 141c b280 55b3 3602 c4b1 b280 5534 01b4  ....U.6.....U4..
+00000ff0: 2a02 632b 00c5 b25f 4b18 c6b3 b1b6 3401  *.c+..._K.....4.
+00001000: e2c3 b514 5910 6014 1cb6 b336 0236 0159  ....Y.`....6.6.Y
+00001010: 4226 1061 141c 1062 1423 b536 0136 01c4  B&.a...b.#.6.6..
+00001020: b3b4 2a02 6301 8458 c902 127c 8120 9039  ..*.c..X...|. .9
+00001030: 2b22 592c 1214 1333 1434 b051 3602 c148  +"Y,...3.4.Q6..H
+00001040: 0fb1 51de 4442 5063 b114 4236 0063 4a21  ..Q.DBPc..B6.cJ!
+00001050: 5712 8105 df44 59c2 490f 120a 231b 141c  W....DY.I...#...
+00001060: b236 0134 0159 5063 5151 c228 025d 4a01  .6.4.YPcQQ.(.]J.
+00001070: 5d51 6384 28b8 020e 6390 5160 2257 2c48  ]Qc.(...c.Q`"W,H
+00001080: 0d12 7f14 3d36 0014 6336 0059 4a2a 5712  ....=6..c6.YJ*W.
+00001090: 8105 df44 62c0 4918 120a 2319 141c b036  ...Db.I...#....6
+000010a0: 0134 0159 127f 143d 3600 1464 3600 5951  .4.Y...=6..d6.YQ
+000010b0: 51c0 2800 5d4a 015d 5163 8218 2910 6581  Q.(.]J.]Qc..).e.
+000010c0: 1690 5c2c 2522 1214 1333 1434 1066 5136  ..\,%"...3.4.fQ6
+000010d0: 02c1 b151 de44 4251 63b0 b118 3051 6387  ...Q.DBQc...0Qc.
+000010e0: 3cd1 0220 1781 0490 6760 2042 2942 3027  <.. ....g` B)B0'
+000010f0: 5a2d 2c2b 4832 b014 1810 1936 0144 4252  Z-,+H2.....6.DBR
+00001100: 6332 00b0 141a 101b 3601 5e34 015f 4b16  c2......6.^4._K.
+00001110: c112 1eb1 3401 434c 1209 2301 141c b136  ....4.CL..#....6
+00001120: 0134 0159 4228 4a2e 5712 8105 df44 66c2  .4.YB(J.W....Df.
+00001130: 491c 1209 2302 141c b0b2 3602 3401 5912  I...#.....6.4.Y.
+00001140: 0a23 0314 1cb2 3601 3401 5950 6351 51c2  .#....6.4.YPcQQ.
+00001150: 2802 5d4a 015d 5263 0182 38b9 4008 675b  (.]J.]Rc..8.@.g[
+00001160: 9070 53b0 5353 4b18 c112 8107 b134 0180  .pS.SSK......4..
+00001170: d844 33b1 1468 3600 141a 3600 6759 4226  .D3..h6...6.gYB&
+00001180: 5163 8378 c102 161d 8104 907b 6020 2228  Qc.x.......{` "(
+00001190: 4e2c 480c 1203 1217 b034 0259 5263 4a21  N,H......4.YRcJ!
+000011a0: 5712 8105 df44 59c1 490f 120a 2304 141c  W....DY.I...#...
+000011b0: b136 0134 0159 5063 5151 c128 015d 4a01  .6.4.YPcQQ.(.]J.
+000011c0: 5d51 6383 3caa 019e 011e 8106 4490 8880  ]Qc.<.......D...
+000011d0: 0726 4486 2c60 2742 0001 2501 51de 4444  .&D.,`'B..%.Q.DD
+000011e0: 3200 2701 b0b1 2001 02c2 b225 0034 0144  2.'... ....%.4.D
+000011f0: 4252 6312 1f25 0025 0134 0263 0248 090a  BRc..%.%.4.c.H..
+00001200: 6981 1690 9051 6395 0893 124c 6a5b 5b81  i....Qc....Lj[[.
+00001210: 1790 9347 492d 2d28 2642 2528 3026 2228  ...GI--(&B%(0&"(
+00001220: 3122 2742 5028 302e 5122 5c46 2b2e 234e  1"'BP(0.Q"\F+.#N
+00001230: 4c42 1281 07b2 3401 c310 29b2 8055 d944  LB....4...)..U.D
+00001240: f380 b382 d944 6510 6bb2 8155 d944 5d10  .....De.k..U.D].
+00001250: 5e14 2312 1514 5536 0036 01c4 106c 141c  ^.#...U6.6...l..
+00001260: b436 01c4 2501 b434 0159 5263 b382 d844  .6..%..4.YRc...D
+00001270: 7b10 5fb2 8155 d944 5812 1514 5f10 31b2  {._..U.DX..._.1.
+00001280: 8255 3682 0030 02c5 c625 01b6 3401 5952  .U6..0...%..4.YR
+00001290: 6310 5cb2 8155 d944 5325 0112 1514 5c10  c.\..U.DS%....\.
+000012a0: 31b2 8255 3682 0034 0159 5263 2501 231a  1..U6..4.YRc%.#.
+000012b0: 3401 5952 63b3 82d8 449d 8110 6d25 007f  4.YRc...D...m%..
+000012c0: 55dd 4493 8125 0014 6e7f 3601 c7b7 146f  U.D..%..n.6....o
+000012d0: 106d 3601 82d9 4443 5242 4150 c8b7 1470  .m6...DCRBAP...p
+000012e0: 106d 102f 3602 1468 3600 c9b9 1471 3600  .m./6..h6....q6.
+000012f0: 4448 1281 13b9 3401 4241 51c9 4812 1215  DH....4.BAQ.H...
+00001300: 143e 2500 1053 b810 72b9 3684 01c5 4a1b  .>%..S..r.6...J.
+00001310: 5712 8105 df44 53ca 4909 2501 ba34 0159  W....DS.I.%..4.Y
+00001320: 5263 5151 ca28 0a5d 4a01 5d10 4014 2325  RcQQ.(.]J.].@.#%
+00001330: 0080 822e 0255 3601 cbb5 444e 2501 1073  .....U6...DN%..s
+00001340: 141c bb36 0134 0159 424c 2501 1074 141c  ...6.4.YBL%..t..
+00001350: bb36 0134 0159 5263 5063 9554 9e12 4b1f  .6.4.YRcPc.T..K.
+00001360: 8106 4490 c880 0883 0d85 0f27 4d2b 1f21  ..D........'M+.!
+00001370: 6327 2d42 7d2a 4c4d 5270 492b 6f2d 562a  c'-B}*LMRpI+o-V*
+00001380: 462b 2646 0a32 00c2 ba20 0101 c3b0 7f55  F+&F.2... .....U
+00001390: 1020 d9c4 b444 48b0 807f 2e02 5542 41b0  . ...DH.....UBA.
+000013a0: c512 8107 b534 0182 db44 fc81 1021 141c  .....4...D...!..
+000013b0: b580 5536 01b5 8155 b210 2214 23b5 8251  ..U6...U..".#..Q
+000013c0: 2e02 5536 0134 015b 5ac6 c7c8 4890 01b6  ..U6.4.[Z...H...
+000013d0: 1205 ddd3 444d 1281 0810 2414 1cb6 3601  ....DM....$...6.
+000013e0: 3401 5948 1212 8109 1025 141c b6b7 b836  4.YH.....%.....6
+000013f0: 0334 0127 0a4a 5057 1281 05df 44c7 80c9  .4.'.JPW....D...
+00001400: 493d b612 810a b934 01dd 446b 120a 2305  I=.....4..Dk..#.
+00001410: 141c b636 0134 0159 1281 0810 2414 1cb6  ...6.4.Y....$...
+00001420: 3601 3401 5912 8109 1025 141c b6b7 b836  6.4.Y....%.....6
+00001430: 0334 0127 0a42 4712 8105 b934 0165 5151  .4.'.BG....4.eQQ
+00001440: c928 095d 4a01 5db3 b4b7 250a 3403 270a  .(.]J.]...%.4.'.
+00001450: b112 810a 250a 3401 3401 5952 634a 4957  ....%.4.4.YRcJIW
+00001460: 1281 05df 44c0 80c9 4936 b123 0614 1cb6  ....D...I6.#....
+00001470: b7b9 3603 3401 5923 0712 810a b934 01dd  ..6.4.Y#.....4..
+00001480: 434b 2308 1281 0ab9 3401 dd44 52b6 1205  CK#.....4..DR...
+00001490: 1426 3600 dd44 4612 05b6 535b 5650 6351  .&6..DF...S[VPcQ
+000014a0: 51c9 2809 5d4a 015d b123 0934 0159 b123  Q.(.]J.].#.4.Y.#
+000014b0: 0a34 0159 5263 0287 5c59 9c01 7581 1890  .4.YRc..\Y..u...
+000014c0: d122 2e2d 3625 2d2c 2a2a 0003 51c1 1076  .".-6%-,**..Q..v
+000014d0: 2500 dd43 4710 7725 00dd 4475 3200 1281  %..CG.w%..Du2...
+000014e0: 1925 0034 0134 0127 03b0 b320 0102 1281  .%.4.4.'... ....
+000014f0: 1a80 1281 0725 0334 0182 3403 3401 c1b1  .....%.4..4.4...
+00001500: 5f4b 0ec2 2500 1470 b210 7836 0227 0042  _K..%..p..x6.'.B
+00001510: 3025 0014 7010 2210 6236 0227 0012 8114  0%..p.".b6.'....
+00001520: b112 6b34 0244 4a25 0014 1cb1 8137 0127  ..k4.DJ%.....7.'
+00001530: 0025 0063 0282 1049 087b 5b90 d32b 00b0  .%.c...I.{[..+..
+00001540: 5f4b 1530 02c1 c2b2 1077 d943 46b2 1076  _K.0.....w.CF..v
+00001550: d944 2eb1 2f14 4229 6382 286b 0c7b 5b5b  .D../.B)c.(k.{[[
+00001560: 5b90 d42b 00b2 5f4b 16c3 2500 2501 b355  [..+.._K..%.%..U
+00001570: 2501 b381 f255 81f2 2e02 552f 1442 2863  %....U....U/.B(c
+00001580: 853c c004 2479 5b81 1b81 1c81 1d90 de2b  .<..$y[........+
+00001590: 2346 5126 2346 2c12 8114 b312 811e 3402  #FQ&#F,.......4.
+000015a0: 445a b144 4612 07b3 3401 6310 5e14 2332  DZ.DF...4.c.^.#2
+000015b0: 0025 0014 4f36 0034 0136 0163 b210 7ad9  .%..O6.4.6.c..z.
+000015c0: 4455 b144 4612 07b3 3401 6310 5e14 2332  DU.DF...4.c.^.#2
+000015d0: 01b3 3401 3601 63b3 6302 8168 5908 7b5b  ..4.6.c.c..hY.{[
+000015e0: 90e2 2b00 b05f 4b10 3002 c1c2 107d 141c  ..+.._K.0....}..
+000015f0: b1b2 3602 2f14 422e 6381 4849 087b 5b90  ..6./.B.c.HI.{[.
+00001600: e82b 00b0 5f4b 0cc1 107e 141c b136 012f  .+.._K...~...6./
+00001610: 1442 3263 8400 c902 1627 8106 a019 6040  .B2c.....'....`@
+00001620: 2228 4e2d 480c 1203 121e b034 0259 5263  "(N-H......4.YRc
+00001630: 4a22 5712 8105 df44 5ac1 4910 120a 230b  J"W....DZ.I...#.
+00001640: 141c b0b1 3602 3401 5950 6351 51c1 2801  ....6.4.YPcQQ.(.
+00001650: 5d4a 015d 5163                           ]J.]Qc
```

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Time.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/Time.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/micrOS.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/micrOS.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/micrOSloader.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/micrOSloader.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/urequests.mpy` & `micrOSDevToolKit-1.21.0/toolkit/workspace/precompiled/urequests.mpy`

 * *Files identical despite different names*


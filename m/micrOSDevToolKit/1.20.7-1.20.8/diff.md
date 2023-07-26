# Comparing `tmp/micrOSDevToolKit-1.20.7.tar.gz` & `tmp/micrOSDevToolKit-1.20.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/micrOSDevToolKit-1.20.7.tar", last modified: Sat Jul 22 08:34:21 2023, max compression
+gzip compressed data, was "dist/micrOSDevToolKit-1.20.8.tar", last modified: Wed Jul 26 12:03:05 2023, max compression
```

## Comparing `micrOSDevToolKit-1.20.7.tar` & `micrOSDevToolKit-1.20.8.tar`

### file list

```diff
@@ -1,253 +1,253 @@
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.939029 micrOSDevToolKit-1.20.7/
--rw-r--r--   0 bnm        (501) staff       (20)      333 2023-07-18 21:54:39.000000 micrOSDevToolKit-1.20.7/MANIFEST.in
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-22 08:34:21.938478 micrOSDevToolKit-1.20.7/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.20.7/README.md
--rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.20.7/devToolKit.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.603584 micrOSDevToolKit-1.20.7/env/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.7/env/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.607276 micrOSDevToolKit-1.20.7/media/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.20.7/media/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/media/dnd.png
--rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.20.7/media/logo.png
--rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/media/logo_mini.png
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.609053 micrOSDevToolKit-1.20.7/micrOS/
--rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.20.7/micrOS/SchedulerUT.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.7/micrOS/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.647185 micrOSDevToolKit-1.20.7/micrOS/micropython/
--rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.7/micrOS/micropython/esp32-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.20.7/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.20.7/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
--rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.7/micrOS/micropython/tinypico-20220618-v1.19.1.bin
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.700945 micrOSDevToolKit-1.20.7/micrOS/source/
--rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.20.7/micrOS/source/.DS_Store
--rw-r--r--   0 bnm        (501) staff       (20)     6198 2023-07-17 14:02:35.000000 micrOSDevToolKit-1.20.7/micrOS/source/Common.py
--rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.20.7/micrOS/source/ConfigHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     6331 2023-07-17 14:19:18.000000 micrOSDevToolKit-1.20.7/micrOS/source/Debug.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.20.7/micrOS/source/Hooks.py
--rw-r--r--   0 bnm        (501) staff       (20)     6844 2023-07-22 08:28:00.000000 micrOSDevToolKit-1.20.7/micrOS/source/InterConnect.py
--rw-r--r--   0 bnm        (501) staff       (20)    11569 2023-07-22 08:22:13.000000 micrOSDevToolKit-1.20.7/micrOS/source/InterpreterShell.py
--rw-r--r--   0 bnm        (501) staff       (20)     7470 2023-07-20 09:51:20.000000 micrOSDevToolKit-1.20.7/micrOS/source/InterruptHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_L298N_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_bme280.py
--rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_buzzer.py
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_cct.py
--rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_co2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-18 21:04:59.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_dht11.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_dht22.py
--rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_ds18.py
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_genIO.py
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_intercon.py
--rw-r--r--   0 bnm        (501) staff       (20)     1618 2023-07-06 20:03:50.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_light_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2890 2023-07-18 20:07:19.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_lmpacman.py
--rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_neoeffects.py
--rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_oled.py
--rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_oled_sh1106.py
--rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-04 18:36:10.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_oled_ui.py
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_presence.py
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_rgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_roboarm.py
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_servo.py
--rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_stepper.py
--rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_switch.py
--rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_system.py
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_telegram.py
--rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LM_tinyrgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LP_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.20.7/micrOS/source/LP_esp32s2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.20.7/micrOS/source/LP_esp32s3.py
--rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.7/micrOS/source/LP_rp2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.7/micrOS/source/LP_tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.20.7/micrOS/source/LogicalPins.py
--rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.20.7/micrOS/source/Network.py
--rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.20.7/micrOS/source/Notify.py
--rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.20.7/micrOS/source/Scheduler.py
--rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-15 19:57:59.000000 micrOSDevToolKit-1.20.7/micrOS/source/SocketServer.py
--rw-r--r--   0 bnm        (501) staff       (20)    19574 2023-07-17 15:01:38.000000 micrOSDevToolKit-1.20.7/micrOS/source/TaskManager.py
--rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.20.7/micrOS/source/Time.py
--rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.7/micrOS/source/TinyPLed.py
--rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.7/micrOS/source/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.20.7/micrOS/source/micrOS.py
--rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.20.7/micrOS/source/micrOSloader.py
--rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.20.7/micrOS/source/reset.py
--rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.20.7/micrOS/source/urequests.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.703552 micrOSDevToolKit-1.20.7/micrOSDevToolKit.egg-info/
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-22 08:34:21.000000 micrOSDevToolKit-1.20.7/micrOSDevToolKit.egg-info/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)     8866 2023-07-22 08:34:21.000000 micrOSDevToolKit-1.20.7/micrOSDevToolKit.egg-info/SOURCES.txt
--rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-22 08:34:21.000000 micrOSDevToolKit-1.20.7/micrOSDevToolKit.egg-info/dependency_links.txt
--rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-22 08:34:21.000000 micrOSDevToolKit-1.20.7/micrOSDevToolKit.egg-info/requires.txt
--rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-22 08:34:21.000000 micrOSDevToolKit-1.20.7/micrOSDevToolKit.egg-info/top_level.txt
--rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-22 08:34:21.939251 micrOSDevToolKit-1.20.7/setup.cfg
--rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-22 08:33:36.000000 micrOSDevToolKit-1.20.7/setup.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.711568 micrOSDevToolKit-1.20.7/toolkit/
--rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.20.7/toolkit/DevEnvCompile.py
--rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.20.7/toolkit/DevEnvOTA.py
--rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.20.7/toolkit/DevEnvUSB.py
--rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/Gateway.py
--rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.20.7/toolkit/MicrOSDevEnv.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.726819 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/
--rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/AirQualityBME280.py
--rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/CCTDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/CCTTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/CatGame.py
--rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/Dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/GetVersion.py
--rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/MicrophoneTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/NeoEffectsDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/NeopixelTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/RGBTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/RoboArm.py
--rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/SED_test.py
--rw-r--r--   0 bnm        (501) staff       (20)    17600 2023-07-19 10:50:53.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/SystemTest.py
--rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/Template_app.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/_micPlotting.py
--rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/uLightDemo.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.732144 micrOSDevToolKit-1.20.7/toolkit/lib/
--rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.20.7/toolkit/lib/LocalMachine.py
--rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.20.7/toolkit/lib/SearchDevices.py
--rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/lib/SerialDriverHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/lib/TerminalColors.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/lib/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.20.7/toolkit/lib/micrOSClient.py
--rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.20.7/toolkit/micrOSdashboard.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.749579 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/
--rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/LP_darwin.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.779128 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5397 2023-07-15 16:13:28.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/dotstar.py
--rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/ds18x20.py
--rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/framebuf.py
--rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/machine.py
--rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/micropython.py
--rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/network.py
--rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/ntptime.py
--rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/onewire.py
--rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/sim_console.py
--rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/simgc.py
--rw-r--r--   0 bnm        (501) staff       (20)     6545 2023-07-15 16:13:22.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/simulator.py
--rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/uasyncio.py
--rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/utime.py
--rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/simulator_lib/webrepl.py
--rwxr-xr-x   0 bnm        (501) staff       (20)    16970 2023-07-19 10:36:50.000000 micrOSDevToolKit-1.20.7/toolkit/socketClient.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.780040 micrOSDevToolKit-1.20.7/toolkit/user_data/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:50:53.000000 micrOSDevToolKit-1.20.7/toolkit/user_data/.include
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.780453 micrOSDevToolKit-1.20.7/toolkit/user_data/node_config_archive/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/user_data/node_config_archive/.include
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.780890 micrOSDevToolKit-1.20.7/toolkit/workspace/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-22 08:34:21.934938 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/
--rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Common.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/ConfigHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1927 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Debug.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      759 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Hooks.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2085 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/InterConnect.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     4174 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/InterpreterShell.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/InterruptHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      869 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_bme280.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_buzzer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_cct.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_co2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_dht11.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_dht22.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_dimmer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)      522 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_ds18.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_genIO.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)      616 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_intercon.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      512 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_light_sensor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1477 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_lmpacman.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_neoeffects.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_neopixel.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_oled.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     6082 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_oled_ui.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_presence.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_rgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_roboarm.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_servo.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_stepper.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_switch.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_system.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      872 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_telegram.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_tinyrgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      550 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LP_esp32.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      563 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LP_esp32s2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      553 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LP_esp32s3.mpy
--rw-r--r--   0 bnm        (501) staff       (20)       54 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LP_rp2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      491 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LP_tinypico.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LogicalPins.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Network.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Notify.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Scheduler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/SocketServer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     5760 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/TaskManager.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Time.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      434 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/TinyPLed.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      440 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/micrOS.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/micrOSloader.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      198 2023-07-22 08:28:42.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/reset.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-07-22 08:28:43.000000 micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/urequests.mpy
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.173428 micrOSDevToolKit-1.20.8/
+-rw-r--r--   0 bnm        (501) staff       (20)      333 2023-07-18 21:54:39.000000 micrOSDevToolKit-1.20.8/MANIFEST.in
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-26 12:03:05.172907 micrOSDevToolKit-1.20.8/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.20.8/README.md
+-rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.20.8/devToolKit.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:04.839571 micrOSDevToolKit-1.20.8/env/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.8/env/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:04.853200 micrOSDevToolKit-1.20.8/media/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.20.8/media/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/media/dnd.png
+-rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.20.8/media/logo.png
+-rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/media/logo_mini.png
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:04.862567 micrOSDevToolKit-1.20.8/micrOS/
+-rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.20.8/micrOS/SchedulerUT.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.8/micrOS/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:04.904586 micrOSDevToolKit-1.20.8/micrOS/micropython/
+-rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.8/micrOS/micropython/esp32-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.20.8/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.20.8/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
+-rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.8/micrOS/micropython/tinypico-20220618-v1.19.1.bin
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:04.967218 micrOSDevToolKit-1.20.8/micrOS/source/
+-rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.20.8/micrOS/source/.DS_Store
+-rw-r--r--   0 bnm        (501) staff       (20)     6198 2023-07-17 14:02:35.000000 micrOSDevToolKit-1.20.8/micrOS/source/Common.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.20.8/micrOS/source/ConfigHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6331 2023-07-17 14:19:18.000000 micrOSDevToolKit-1.20.8/micrOS/source/Debug.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.20.8/micrOS/source/Hooks.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6844 2023-07-22 08:28:00.000000 micrOSDevToolKit-1.20.8/micrOS/source/InterConnect.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11569 2023-07-26 11:40:59.000000 micrOSDevToolKit-1.20.8/micrOS/source/InterpreterShell.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7470 2023-07-20 09:51:20.000000 micrOSDevToolKit-1.20.8/micrOS/source/InterruptHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_L298N_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_bme280.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_buzzer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_cct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_co2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-18 21:04:59.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_dht11.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_dht22.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_ds18.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_genIO.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_intercon.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1618 2023-07-06 20:03:50.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_light_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2890 2023-07-18 20:07:19.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_lmpacman.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_neoeffects.py
+-rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_oled.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_oled_sh1106.py
+-rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-04 18:36:10.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_oled_ui.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_presence.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_rgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_roboarm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_servo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_stepper.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_switch.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_system.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_telegram.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LM_tinyrgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LP_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.20.8/micrOS/source/LP_esp32s2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.20.8/micrOS/source/LP_esp32s3.py
+-rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.8/micrOS/source/LP_rp2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.8/micrOS/source/LP_tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.20.8/micrOS/source/LogicalPins.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.20.8/micrOS/source/Network.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.20.8/micrOS/source/Notify.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.20.8/micrOS/source/Scheduler.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-15 19:57:59.000000 micrOSDevToolKit-1.20.8/micrOS/source/SocketServer.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19305 2023-07-26 11:52:48.000000 micrOSDevToolKit-1.20.8/micrOS/source/TaskManager.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.20.8/micrOS/source/Time.py
+-rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.8/micrOS/source/TinyPLed.py
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.8/micrOS/source/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.20.8/micrOS/source/micrOS.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.20.8/micrOS/source/micrOSloader.py
+-rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.20.8/micrOS/source/reset.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.20.8/micrOS/source/urequests.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:04.970183 micrOSDevToolKit-1.20.8/micrOSDevToolKit.egg-info/
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-26 12:03:04.000000 micrOSDevToolKit-1.20.8/micrOSDevToolKit.egg-info/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)     8866 2023-07-26 12:03:04.000000 micrOSDevToolKit-1.20.8/micrOSDevToolKit.egg-info/SOURCES.txt
+-rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-26 12:03:04.000000 micrOSDevToolKit-1.20.8/micrOSDevToolKit.egg-info/dependency_links.txt
+-rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-26 12:03:04.000000 micrOSDevToolKit-1.20.8/micrOSDevToolKit.egg-info/requires.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-26 12:03:04.000000 micrOSDevToolKit-1.20.8/micrOSDevToolKit.egg-info/top_level.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-26 12:03:05.173567 micrOSDevToolKit-1.20.8/setup.cfg
+-rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-26 12:01:34.000000 micrOSDevToolKit-1.20.8/setup.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:04.992357 micrOSDevToolKit-1.20.8/toolkit/
+-rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.20.8/toolkit/DevEnvCompile.py
+-rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.20.8/toolkit/DevEnvOTA.py
+-rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.20.8/toolkit/DevEnvUSB.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/Gateway.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.20.8/toolkit/MicrOSDevEnv.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.022500 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/
+-rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/AirQualityBME280.py
+-rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/CCTDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/CCTTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/CatGame.py
+-rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/Dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/GetVersion.py
+-rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/MicrophoneTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/NeoEffectsDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/NeopixelTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/RGBTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/RoboArm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/SED_test.py
+-rw-r--r--   0 bnm        (501) staff       (20)    17600 2023-07-19 10:50:53.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/SystemTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/Template_app.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/_micPlotting.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/uLightDemo.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.031427 micrOSDevToolKit-1.20.8/toolkit/lib/
+-rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.20.8/toolkit/lib/LocalMachine.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.20.8/toolkit/lib/SearchDevices.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/lib/SerialDriverHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/lib/TerminalColors.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/lib/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.20.8/toolkit/lib/micrOSClient.py
+-rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.20.8/toolkit/micrOSdashboard.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.046347 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/
+-rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/LP_darwin.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.103842 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5397 2023-07-15 16:13:28.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/dotstar.py
+-rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/ds18x20.py
+-rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/framebuf.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/machine.py
+-rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/micropython.py
+-rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/network.py
+-rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/ntptime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/onewire.py
+-rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/sim_console.py
+-rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/simgc.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6545 2023-07-15 16:13:22.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/simulator.py
+-rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/uasyncio.py
+-rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/utime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/simulator_lib/webrepl.py
+-rwxr-xr-x   0 bnm        (501) staff       (20)    16970 2023-07-19 10:36:50.000000 micrOSDevToolKit-1.20.8/toolkit/socketClient.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.104640 micrOSDevToolKit-1.20.8/toolkit/user_data/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:50:53.000000 micrOSDevToolKit-1.20.8/toolkit/user_data/.include
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.105123 micrOSDevToolKit-1.20.8/toolkit/user_data/node_config_archive/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-18 21:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/user_data/node_config_archive/.include
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.105519 micrOSDevToolKit-1.20.8/toolkit/workspace/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-26 12:03:05.171430 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/
+-rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Common.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/ConfigHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1927 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Debug.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      759 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Hooks.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2085 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/InterConnect.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     4174 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/InterpreterShell.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/InterruptHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      869 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_bme280.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_buzzer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_cct.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_co2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1952 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_dht11.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_dht22.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_dimmer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)      522 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_ds18.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_genIO.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)      616 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_intercon.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      512 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_light_sensor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1477 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_lmpacman.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_neoeffects.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_neopixel.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_oled.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     6082 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_oled_ui.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_presence.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_rgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_roboarm.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_servo.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_stepper.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_switch.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_system.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      872 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_telegram.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_tinyrgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      550 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LP_esp32.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      563 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LP_esp32s2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      553 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LP_esp32s3.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)       54 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LP_rp2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      491 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LP_tinypico.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LogicalPins.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Network.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Notify.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Scheduler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/SocketServer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     5702 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/TaskManager.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Time.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      434 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/TinyPLed.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-07-26 11:57:14.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/micrOS.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/micrOSloader.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      198 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/reset.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-07-26 11:57:13.000000 micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/urequests.mpy
```

### Comparing `micrOSDevToolKit-1.20.7/PKG-INFO` & `micrOSDevToolKit-1.20.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.20.7
+Version: 1.20.8
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.20.7/README.md` & `micrOSDevToolKit-1.20.8/README.md`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/devToolKit.py` & `micrOSDevToolKit-1.20.8/devToolKit.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/media/dnd.png` & `micrOSDevToolKit-1.20.8/media/dnd.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/media/logo.png` & `micrOSDevToolKit-1.20.8/media/logo.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/media/logo_mini.png` & `micrOSDevToolKit-1.20.8/media/logo_mini.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/SchedulerUT.py` & `micrOSDevToolKit-1.20.8/micrOS/SchedulerUT.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/micropython/esp32-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.20.8/micrOS/micropython/esp32-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/micropython/esp32s2-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.20.8/micrOS/micropython/esp32s2-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin` & `micrOSDevToolKit-1.20.8/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2` & `micrOSDevToolKit-1.20.8/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/micropython/tinypico-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.20.8/micrOS/micropython/tinypico-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/.DS_Store` & `micrOSDevToolKit-1.20.8/micrOS/source/.DS_Store`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/Common.py` & `micrOSDevToolKit-1.20.8/micrOS/source/Common.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/ConfigHandler.py` & `micrOSDevToolKit-1.20.8/micrOS/source/ConfigHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/Debug.py` & `micrOSDevToolKit-1.20.8/micrOS/source/Debug.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/Hooks.py` & `micrOSDevToolKit-1.20.8/micrOS/source/Hooks.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/InterConnect.py` & `micrOSDevToolKit-1.20.8/micrOS/source/InterConnect.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/InterpreterShell.py` & `micrOSDevToolKit-1.20.8/micrOS/source/InterpreterShell.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 #################################################################
 #                  SHELL Interpreter FUNCTIONS                  #
 #################################################################
 
 class Shell:
-    MICROS_VERSION = '1.20.4-0'
+    MICROS_VERSION = '1.20.5-0'
 
     def __init__(self, msg_obj=None):
         """
         comm_obj - communication object - send messages back
                  - comm_obj.reply('msg')
         """
         self.msg_obj = msg_obj
```

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/InterruptHandler.py` & `micrOSDevToolKit-1.20.8/micrOS/source/InterruptHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_L298N_DCmotor.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_L298N_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_VL53L0X.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_bme280.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_bme280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_buzzer.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_buzzer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_catgame.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_cct.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_cct.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_co2.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_co2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_demo.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_dht11.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_dht11.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_dht22.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_dht22.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_dimmer.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_distance.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_ds18.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_ds18.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_esp32.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_genIO.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_genIO.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_i2c.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_intercon.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_intercon.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_light_sensor.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_light_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_lmpacman.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_lmpacman.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_neoeffects.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_neoeffects.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_neopixel.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_oled.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_oled.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_oled_sh1106.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_oled_sh1106.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_oled_ui.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_oled_ui.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_pet_feeder.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_ph_sensor.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_presence.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_presence.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_rencoder.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_rgb.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_rgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_roboarm.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_roboarm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_robustness.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_servo.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_servo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_stepper.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_stepper.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_switch.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_switch.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_system.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_system.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_telegram.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_telegram.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LM_tinyrgb.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LM_tinyrgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LP_esp32.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LP_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LP_esp32s2.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LP_esp32s2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LP_esp32s3.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LP_esp32s3.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LP_tinypico.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LP_tinypico.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/LogicalPins.py` & `micrOSDevToolKit-1.20.8/micrOS/source/LogicalPins.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/Network.py` & `micrOSDevToolKit-1.20.8/micrOS/source/Network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/Notify.py` & `micrOSDevToolKit-1.20.8/micrOS/source/Notify.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/Scheduler.py` & `micrOSDevToolKit-1.20.8/micrOS/source/Scheduler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/SocketServer.py` & `micrOSDevToolKit-1.20.8/micrOS/source/SocketServer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/TaskManager.py` & `micrOSDevToolKit-1.20.8/micrOS/source/TaskManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,23 +227,19 @@
         - Try to measure system load - based on idle task latency
         """
         # FREQUENCY OF IDLE TASK - IMPACTS IRQ TASK SCHEDULING, SMALLER IS BEST
         my_task = Task.TASKS.get('idle')
         my_task.out = f"i.d.l.e: 200ms"
         try:
             while True:
-                await asyncio.sleep_ms(200)     # 0.2s wake, irq
-                await asyncio.sleep_ms(200)     # 0.4s wake
-                await asyncio.sleep_ms(200)     # 0.6s wake
-                await asyncio.sleep_ms(200)     # 0.8s wake
                 # Probe system load
                 t = ticks_ms()
-                await asyncio.sleep_ms(200)     # 1.0s measure load
+                await asyncio.sleep_ms(500)
                 # SysLogic block - sys load
-                delta_rate = int(((ticks_diff(ticks_ms(), t) / 200)-1) * 100)
+                delta_rate = int(((ticks_diff(ticks_ms(), t) / 500)-1) * 100)
                 Manager.OLOAD = int((Manager.OLOAD + delta_rate) / 2)       # Average - smooth
         except Exception as e:
             errlog_add(f"[ERR] Idle task exists: {e}")
         my_task.done.set()
 
     @staticmethod
     def create_task(callback, tag=None, loop=False, delay=None):
```

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/Time.py` & `micrOSDevToolKit-1.20.8/micrOS/source/Time.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/TinyPLed.py` & `micrOSDevToolKit-1.20.8/micrOS/source/TinyPLed.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/micrOS.py` & `micrOSDevToolKit-1.20.8/micrOS/source/micrOS.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/micrOSloader.py` & `micrOSDevToolKit-1.20.8/micrOS/source/micrOSloader.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOS/source/urequests.py` & `micrOSDevToolKit-1.20.8/micrOS/source/urequests.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/micrOSDevToolKit.egg-info/PKG-INFO` & `micrOSDevToolKit-1.20.8/micrOSDevToolKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.20.7
+Version: 1.20.8
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.20.7/micrOSDevToolKit.egg-info/SOURCES.txt` & `micrOSDevToolKit-1.20.8/micrOSDevToolKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/setup.py` & `micrOSDevToolKit-1.20.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # https://towardsdatascience.com/create-your-custom-python-package-that-you-can-pip-install-from-your-git-repository-f90465867893
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='micrOSDevToolKit',
-    version='1.20.7',
+    version='1.20.8',
     author='Marcell Ban',
     author_email='miros.framework@gmail.com',
     description='Development and deployment environment for micrOS, the diy micropython automation OS (IoT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/BxNxM/micrOS',
     project_urls={
```

### Comparing `micrOSDevToolKit-1.20.7/toolkit/DevEnvCompile.py` & `micrOSDevToolKit-1.20.8/toolkit/DevEnvCompile.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/DevEnvOTA.py` & `micrOSDevToolKit-1.20.8/toolkit/DevEnvOTA.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/DevEnvUSB.py` & `micrOSDevToolKit-1.20.8/toolkit/DevEnvUSB.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/Gateway.py` & `micrOSDevToolKit-1.20.8/toolkit/Gateway.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/MicrOSDevEnv.py` & `micrOSDevToolKit-1.20.8/toolkit/MicrOSDevEnv.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/AirQualityBME280.py` & `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/AirQualityBME280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/AirQualityDHT22_CO2.py` & `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/AirQualityDHT22_CO2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/CCTDemo.py` & `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/CCTDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/CCTTest.py` & `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/CCTTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/CatGame.py` & `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/CatGame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/Dimmer.py` & `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/Dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/GetVersion.py` & `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/GetVersion.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/NeoEffectsDemo.py` & `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/NeoEffectsDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/NeopixelTest.py` & `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/NeopixelTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/RGBTest.py` & `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/RGBTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/RoboArm.py` & `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/RoboArm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/SED_test.py` & `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/SED_test.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/SystemTest.py` & `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/SystemTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/Template_app.py` & `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/Template_app.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/_micPlotting.py` & `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/_micPlotting.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/dashboard_apps/uLightDemo.py` & `micrOSDevToolKit-1.20.8/toolkit/dashboard_apps/uLightDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/lib/LocalMachine.py` & `micrOSDevToolKit-1.20.8/toolkit/lib/LocalMachine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/lib/SearchDevices.py` & `micrOSDevToolKit-1.20.8/toolkit/lib/SearchDevices.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/lib/SerialDriverHandler.py` & `micrOSDevToolKit-1.20.8/toolkit/lib/SerialDriverHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/lib/TerminalColors.py` & `micrOSDevToolKit-1.20.8/toolkit/lib/TerminalColors.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/lib/micrOSClient.py` & `micrOSDevToolKit-1.20.8/toolkit/lib/micrOSClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/micrOSdashboard.py` & `micrOSDevToolKit-1.20.8/toolkit/micrOSdashboard.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/LP_darwin.py` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/LP_darwin.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/machine.py` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/machine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/micropython.py` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/micropython.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/neopixel.py` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/network.py` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/sim_console.py` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/sim_console.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/simulator.py` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/simulator.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/uasyncio.py` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/uasyncio.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/simulator_lib/utime.py` & `micrOSDevToolKit-1.20.8/toolkit/simulator_lib/utime.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/socketClient.py` & `micrOSDevToolKit-1.20.8/toolkit/socketClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Common.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Common.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/ConfigHandler.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/ConfigHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Debug.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Debug.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Hooks.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Hooks.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/InterConnect.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/InterConnect.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/InterpreterShell.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/InterpreterShell.mpy`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6366 6770 7574 001a 436f 6e66 6967 4861  cfgput..ConfigHa
 00000050: 6e64 6c65 7200 1865 7865 635f 6c6d 5f63  ndler..exec_lm_c
 00000060: 6f72 6500 1654 6173 6b4d 616e 6167 6572  ore..TaskManager
 00000070: 001a 636f 6e73 6f6c 655f 7772 6974 6500  ..console_write.
 00000080: 1465 7272 6c6f 675f 6164 6400 0a44 6562  .errlog_add..Deb
 00000090: 7567 000a 7265 7365 7400 1473 6f66 745f  ug..reset..soft_
 000000a0: 7265 7365 7400 0e6d 6163 6869 6e65 000a  reset..machine..
-000000b0: 5368 656c 6c00 1031 2e32 302e 342d 3000  Shell..1.20.4-0.
+000000b0: 5368 656c 6c00 1031 2e32 302e 352d 3000  Shell..1.20.5-0.
 000000c0: 230e 6d73 675f 6f62 6a00 0c64 6576 6669  #.msg_obj..devfi
 000000d0: 6400 105f 5f64 6576 6669 6400 0861 7574  d..__devfid..aut
 000000e0: 6800 165f 5f61 7574 685f 6d6f 6465 000a  h..__auth_mode..
 000000f0: 6877 7569 6400 0e5f 5f68 7775 6964 0012  hwuid..__hwuid..
 00000100: 5f5f 6175 7468 5f6f 6b00 165f 5f63 6f6e  __auth_ok..__con
 00000110: 665f 6d6f 6465 000e 7665 7273 696f 6e00  f_mode..version.
 00000120: 1c4d 4943 524f 535f 5645 5253 494f 4e00  .MICROS_VERSION.
```

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/InterruptHandler.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/InterruptHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_VL53L0X.py` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_bme280.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_bme280.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_buzzer.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_buzzer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_catgame.py` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_cct.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_cct.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_co2.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_co2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_demo.py` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_dht11.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_dht11.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_dht22.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_dht22.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_dimmer.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_dimmer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_distance.py` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_ds18.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_ds18.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_esp32.py` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_genIO.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_genIO.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_i2c.py` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_intercon.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_intercon.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_light_sensor.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_light_sensor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_lmpacman.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_lmpacman.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_neoeffects.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_neoeffects.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_neopixel.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_neopixel.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_oled.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_oled.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_oled_sh1106.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_oled_sh1106.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_oled_ui.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_oled_ui.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_pet_feeder.py` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_ph_sensor.py` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_presence.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_presence.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_rencoder.py` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_rgb.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_rgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_roboarm.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_roboarm.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_robustness.py` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_servo.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_servo.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_stepper.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_stepper.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_switch.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_switch.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_system.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_system.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_telegram.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_telegram.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LM_tinyrgb.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LM_tinyrgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LP_esp32.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LP_esp32.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LP_esp32s2.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LP_esp32s2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LP_esp32s3.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LP_esp32s3.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/LogicalPins.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/LogicalPins.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Network.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Network.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Notify.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Notify.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Scheduler.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Scheduler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/SocketServer.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/SocketServer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/TaskManager.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/TaskManager.mpy`

 * *Files 4% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 00000770: 7374 6f70 7065 643a 207b 7d00 0541 496e  stopped: {}..AIn
 00000780: 7661 6c69 6420 7461 736b 2063 6d64 2120  valid task cmd! 
 00000790: 4865 6c70 3a20 7461 736b 206c 6973 7420  Help: task list 
 000007a0: 2f20 6b69 6c6c 203c 7461 736b 4944 3e20  / kill <taskID> 
 000007b0: 2f20 7368 6f77 203c 7461 736b 4944 3e00  / show <taskID>.
 000007c0: 0513 5b45 5252 5d20 5461 736b 206b 696c  ..[ERR] Task kil
 000007d0: 6c3a 207b 7d00 8c54 2436 0180 0e26 2c2c  l: {}..T$6...&,,
-000007e0: 2c32 2c52 224f 278f 0789 9089 b884 1484  ,2,R"O'.........
+000007e0: 2c32 2c52 224f 278f 0789 9089 b484 1484  ,2,R"O'.........
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
-00000be0: 6940 890c 8919 8f0d 890f 890f 8910 8920  i@............. 
+00000be0: 6940 890c 8915 8f0d 890f 890f 8910 8920  i@............. 
 00000bf0: 890b 0011 8100 1681 0110 1516 8102 5116  ..............Q.
 00000c00: 4811 0c10 1634 0116 5180 1652 b020 0001  H....4..Q..R. ..
 00000c10: 1647 1181 0351 512a 0253 3301 3401 164a  .G...QQ*.S3.4..J
 00000c20: 1181 0332 0234 0116 4e11 8103 3203 3401  ...2.4..N...2.4.
 00000c30: 1650 1181 0332 0434 0116 4c11 8103 5150  .P...2.4..L...QP
 00000c40: 512a 0353 3305 3401 163e 1181 0332 0634  Q*.S3.4..>...2.4
 00000c50: 0116 5511 8103 3207 3401 165a 1181 0332  ..U...2.4..Z...2
@@ -208,153 +208,150 @@
 00000cf0: 3c18 064e 80d0 1281 1232 0012 1413 3314  <..N.....2....3.
 00000d00: 4f36 0034 0134 0163 0182 2849 087b 5b80  O6.4.4.c..(I.{[.
 00000d10: d02b 00b0 5f4b 1830 02c1 c2b2 132e 1435  .+.._K.0.......5
 00000d20: 3600 4331 1040 b1dd 442b 812f 1442 2663  6.C1.@..D+./.B&c
 00000d30: 8308 1810 5080 d460 402d 2b26 1215 144e  ....P..`@-+&...N
 00000d40: 3600 1215 1351 db44 5823 1114 1c12 1513  6....Q.DX#......
 00000d50: 5136 01c0 120a b034 0159 1281 05b0 3401  Q6.....4.Y....4.
-00000d60: 6551 638c 50d0 4226 4c80 e060 402b 2922  eQc.P.B&L..`@+)"
-00000d70: 202d 2d2d 4d25 4d39 1f41 3512 1413 3314   ---M%M9.A5...3.
-00000d80: 3410 4d36 01c0 2312 141c 3600 b018 3048  4.M6..#...6...0H
-00000d90: 7512 7f14 4322 8148 3601 5e51 6859 127f  u...C".H6.^QhY..
-00000da0: 1443 2281 4836 015e 5168 5912 7f14 4322  .C".H6.^QhY...C"
-00000db0: 8148 3601 5e51 6859 127f 1443 2281 4836  .H6.^QhY...C".H6
-00000dc0: 015e 5168 5912 0e34 00c1 127f 1443 2281  .^QhY..4.....C".
-00000dd0: 4836 015e 5168 5912 8113 120f 120e 3400  H6.^QhY.......4.
-00000de0: b134 0222 8148 f781 f322 8064 f434 01c2  .4.".H...".d.4..
-00000df0: 1281 1312 1513 52b2 f282 f734 0112 1518  ......R....4....
-00000e00: 5242 8d7f 4a1f 5712 8105 df44 57c3 490d  RB..J.W....DW.I.
-00000e10: 120a 2313 141c b336 0134 0159 5151 c328  ..#....6.4.YQQ.(
-00000e20: 035d 4a01 5db0 132e 1437 3600 5951 6384  .]J.]....76.YQc.
-00000e30: 20d8 8501 183e 4b31 5372 80f9 6040 4a27   ....>K1Sr..`@J'
-00000e40: 3312 8114 b012 6b34 0244 5a12 1514 5036  3.....k4.DZ...P6
-00000e50: 0059 1214 3400 143f 104b b010 53b2 1054  .Y..4..?.K..S..T
-00000e60: b336 8600 6312 1434 0014 3b10 4bb0 1031  .6..c..4..;.K..1
-00000e70: b136 8400 6387 0878 1855 9006 6020 2c32  .6..c..x.U..` ,2
-00000e80: 2f30 2c2a 2912 1513 5112 1514 4e36 00f3  /0,*)...Q...N6..
-00000e90: c023 1423 1514 1cb0 1215 1352 3602 2316  .#.#.......R6.#.
-00000ea0: 2b03 c112 1413 3314 4f36 005f 4b33 3002  +.....3.O6._K30.
-00000eb0: c2c3 b313 2e14 3536 0044 4410 5642 4210  ......56.DD.VBB.
-00000ec0: 57c4 1022 8a12 8107 b434 01f3 f4c5 1058  W..".....4.....X
-00000ed0: 141c b4b5 b236 03c6 b114 59b6 3601 5942  .....6....Y.6.YB
-00000ee0: 0b12 8115 b134 0163 8708 611e 5a31 9015  .....4.c..a.Z1..
-00000ef0: 202b 2623 282c 3c29 2a23 2212 1413 3314   +&#(,<)*#"...3.
-00000f00: 34b0 5136 02c1 b151 de44 cb80 2b00 c2b0  4.Q6...Q.D..+...
-00000f10: 141a 1040 3601 c312 1413 3314 2636 005f  ...@6.....3.&6._
-00000f20: 4b26 c4b4 1418 b380 5536 0144 5912 8107  K&......U6.DY...
-00000f30: b334 0181 d844 4fb3 8155 105b d944 47b2  .4...DO..U.[.DG.
-00000f40: 1459 b436 0159 4218 1281 07b2 3401 80d9  .Y.6.YB.....4...
-00000f50: 4443 2b00 63b2 63b0 2b01 6386 3071 1c5c  DC+.c.c.+.c.0q.\
-00000f60: 3190 2460 2028 2a28 2a2b 2325 3712 1514  1.$` (*(*+#%7...
-00000f70: 5ab0 3601 c112 8107 b134 0180 d944 4823  Z.6......4...DH#
-00000f80: 1714 1cb0 3601 6312 8107 b134 0181 d944  ....6.c....4...D
-00000f90: 4b12 1413 33b1 8055 5513 3063 2b00 c2b1  K...3..UU.0c+...
-00000fa0: 5f4b 18c3 b214 5910 5d14 1cb3 1214 1333  _K....Y.]......3
-00000fb0: b355 1330 3602 3601 5942 2610 5e14 23b2  .U.06.6.YB&.^.#.
-00000fc0: 3601 6388 5481 1028 5f31 9034 8007 8309  6.c.T..(_1.4....
-00000fd0: 2822 2a2b 2a2b 2a23 2527 302e 3200 c112  ("*+*+*#%'0.2...
-00000fe0: 1514 5ab0 3601 c252 c312 8107 b234 0180  ..Z.6..R.....4..
-00000ff0: d944 4bb3 2317 141c b036 012a 0263 1281  .DK.#....6.*.c..
-00001000: 07b2 3401 81d9 4455 2318 141c b280 55b3  ..4...DU#.....U.
-00001010: 3602 c4b1 b280 5534 01b4 2a02 632b 00c5  6.....U4..*.c+..
-00001020: b25f 4b18 c6b3 b1b6 3401 e2c3 b514 5910  ._K.....4.....Y.
-00001030: 6014 1cb6 b336 0236 0159 4226 1061 141c  `....6.6.YB&.a..
-00001040: 1062 1423 b536 0136 01c4 b3b4 2a02 6301  .b.#.6.6....*.c.
-00001050: 8458 c902 127c 8120 903c 2b22 592c 1214  .X...|. .<+"Y,..
-00001060: 1333 1434 b051 3602 c148 0fb1 51de 4442  .3.4.Q6..H..Q.DB
-00001070: 5063 b114 4236 0063 4a21 5712 8105 df44  Pc..B6.cJ!W....D
-00001080: 59c2 490f 120a 231b 141c b236 0134 0159  Y.I...#....6.4.Y
-00001090: 5063 5151 c228 025d 4a01 5d51 6384 28b8  PcQQ.(.]J.]Qc.(.
-000010a0: 020e 6390 5460 2257 2c48 0d12 7f14 3d36  ..c.T`"W,H....=6
-000010b0: 0014 6336 0059 4a2a 5712 8105 df44 62c0  ..c6.YJ*W....Db.
-000010c0: 4918 120a 2319 141c b036 0134 0159 127f  I...#....6.4.Y..
-000010d0: 143d 3600 1464 3600 5951 51c0 2800 5d4a  .=6..d6.YQQ.(.]J
-000010e0: 015d 5163 8218 2910 6581 1690 5f2c 2522  .]Qc..).e..._,%"
-000010f0: 1214 1333 1434 1066 5136 02c1 b151 de44  ...3.4.fQ6...Q.D
-00001100: 4251 63b0 b118 3051 6387 3cd1 0220 1781  BQc...0Qc.<.. ..
-00001110: 0490 6a60 2042 2942 3027 5a2d 2c2b 4832  ..j` B)B0'Z-,+H2
-00001120: b014 1810 1936 0144 4252 6332 00b0 141a  .....6.DBRc2....
-00001130: 101b 3601 5e34 015f 4b16 c112 1eb1 3401  ..6.^4._K.....4.
-00001140: 434c 1209 2301 141c b136 0134 0159 4228  CL..#....6.4.YB(
-00001150: 4a2e 5712 8105 df44 66c2 491c 1209 2302  J.W....Df.I...#.
-00001160: 141c b0b2 3602 3401 5912 0a23 0314 1cb2  ....6.4.Y..#....
-00001170: 3601 3401 5950 6351 51c2 2802 5d4a 015d  6.4.YPcQQ.(.]J.]
-00001180: 5263 0182 38b9 4008 675b 9073 53b0 5353  Rc..8.@.g[.sS.SS
-00001190: 4b18 c112 8107 b134 0180 d844 33b1 1468  K......4...D3..h
-000011a0: 3600 141a 3600 6759 4226 5163 8378 c102  6...6.gYB&Qc.x..
-000011b0: 161d 8104 907e 6020 2228 4e2c 480c 1203  .....~` "(N,H...
-000011c0: 1217 b034 0259 5263 4a21 5712 8105 df44  ...4.YRcJ!W....D
-000011d0: 59c1 490f 120a 2304 141c b136 0134 0159  Y.I...#....6.4.Y
-000011e0: 5063 5151 c128 015d 4a01 5d51 6383 3caa  PcQQ.(.]J.]Qc.<.
-000011f0: 019e 011e 8106 4490 8b80 0726 4486 2c60  ......D....&D.,`
-00001200: 2742 0001 2501 51de 4444 3200 2701 b0b1  'B..%.Q.DD2.'...
-00001210: 2001 02c2 b225 0034 0144 4252 6312 1f25   ....%.4.DBRc..%
-00001220: 0025 0134 0263 0248 090a 6981 1690 9351  .%.4.c.H..i....Q
-00001230: 6395 0893 124c 6a5b 5b81 1790 9647 492d  c....Lj[[....GI-
-00001240: 2d28 2642 2528 3026 2228 3122 2742 5028  -(&B%(0&"(1"'BP(
-00001250: 302e 5122 5c46 2b2e 234e 4c42 1281 07b2  0.Q"\F+.#NLB....
-00001260: 3401 c310 29b2 8055 d944 f380 b382 d944  4...)..U.D.....D
-00001270: 6510 6bb2 8155 d944 5d10 5e14 2312 1514  e.k..U.D].^.#...
-00001280: 5536 0036 01c4 106c 141c b436 01c4 2501  U6.6...l...6..%.
-00001290: b434 0159 5263 b382 d844 7b10 5fb2 8155  .4.YRc...D{._..U
-000012a0: d944 5812 1514 5f10 31b2 8255 3682 0030  .DX..._.1..U6..0
-000012b0: 02c5 c625 01b6 3401 5952 6310 5cb2 8155  ...%..4.YRc.\..U
-000012c0: d944 5325 0112 1514 5c10 31b2 8255 3682  .DS%....\.1..U6.
-000012d0: 0034 0159 5263 2501 231a 3401 5952 63b3  .4.YRc%.#.4.YRc.
-000012e0: 82d8 449d 8110 6d25 007f 55dd 4493 8125  ..D...m%..U.D..%
-000012f0: 0014 6e7f 3601 c7b7 146f 106d 3601 82d9  ..n.6....o.m6...
-00001300: 4443 5242 4150 c8b7 1470 106d 102f 3602  DCRBAP...p.m./6.
-00001310: 1468 3600 c9b9 1471 3600 4448 1281 13b9  .h6....q6.DH....
-00001320: 3401 4241 51c9 4812 1215 143e 2500 1053  4.BAQ.H....>%..S
-00001330: b810 72b9 3684 01c5 4a1b 5712 8105 df44  ..r.6...J.W....D
-00001340: 53ca 4909 2501 ba34 0159 5263 5151 ca28  S.I.%..4.YRcQQ.(
-00001350: 0a5d 4a01 5d10 4014 2325 0080 822e 0255  .]J.].@.#%.....U
-00001360: 3601 cbb5 444e 2501 1073 141c bb36 0134  6...DN%..s...6.4
-00001370: 0159 424c 2501 1074 141c bb36 0134 0159  .YBL%..t...6.4.Y
-00001380: 5263 5063 9554 9e12 4b1f 8106 4490 cb80  RcPc.T..K...D...
-00001390: 0883 0d85 0f27 4d2b 1f21 6327 2d42 7d2a  .....'M+.!c'-B}*
-000013a0: 4c4d 5270 492b 6f2d 562a 462b 2646 0a32  LMRpI+o-V*F+&F.2
-000013b0: 00c2 ba20 0101 c3b0 7f55 1020 d9c4 b444  ... .....U. ...D
-000013c0: 48b0 807f 2e02 5542 41b0 c512 8107 b534  H.....UBA......4
-000013d0: 0182 db44 fc81 1021 141c b580 5536 01b5  ...D...!....U6..
-000013e0: 8155 b210 2214 23b5 8251 2e02 5536 0134  .U..".#..Q..U6.4
-000013f0: 015b 5ac6 c7c8 4890 01b6 1205 ddd3 444d  .[Z...H.......DM
-00001400: 1281 0810 2414 1cb6 3601 3401 5948 1212  ....$...6.4.YH..
-00001410: 8109 1025 141c b6b7 b836 0334 0127 0a4a  ...%.....6.4.'.J
-00001420: 5057 1281 05df 44c7 80c9 493d b612 810a  PW....D...I=....
-00001430: b934 01dd 446b 120a 2305 141c b636 0134  .4..Dk..#....6.4
-00001440: 0159 1281 0810 2414 1cb6 3601 3401 5912  .Y....$...6.4.Y.
-00001450: 8109 1025 141c b6b7 b836 0334 0127 0a42  ...%.....6.4.'.B
-00001460: 4712 8105 b934 0165 5151 c928 095d 4a01  G....4.eQQ.(.]J.
-00001470: 5db3 b4b7 250a 3403 270a b112 810a 250a  ]...%.4.'.....%.
-00001480: 3401 3401 5952 634a 4957 1281 05df 44c0  4.4.YRcJIW....D.
-00001490: 80c9 4936 b123 0614 1cb6 b7b9 3603 3401  ..I6.#......6.4.
-000014a0: 5923 0712 810a b934 01dd 434b 2308 1281  Y#.....4..CK#...
-000014b0: 0ab9 3401 dd44 52b6 1205 1426 3600 dd44  ..4..DR....&6..D
-000014c0: 4612 05b6 535b 5650 6351 51c9 2809 5d4a  F...S[VPcQQ.(.]J
-000014d0: 015d b123 0934 0159 b123 0a34 0159 5263  .].#.4.Y.#.4.YRc
-000014e0: 0287 5c59 9c01 7581 1890 d422 2e2d 3625  ..\Y..u....".-6%
-000014f0: 2d2c 2a2a 0003 51c1 1076 2500 dd43 4710  -,**..Q..v%..CG.
-00001500: 7725 00dd 4475 3200 1281 1925 0034 0134  w%..Du2....%.4.4
-00001510: 0127 03b0 b320 0102 1281 1a80 1281 0725  .'... .........%
-00001520: 0334 0182 3403 3401 c1b1 5f4b 0ec2 2500  .4..4.4..._K..%.
-00001530: 1470 b210 7836 0227 0042 3025 0014 7010  .p..x6.'.B0%..p.
-00001540: 2210 6236 0227 0012 8114 b112 6b34 0244  ".b6.'......k4.D
-00001550: 4a25 0014 1cb1 8137 0127 0025 0063 0282  J%.....7.'.%.c..
-00001560: 1049 087b 5b90 d62b 00b0 5f4b 1530 02c1  .I.{[..+.._K.0..
-00001570: c2b2 1077 d943 46b2 1076 d944 2eb1 2f14  ...w.CF..v.D../.
-00001580: 4229 6382 286b 0c7b 5b5b 5b90 d72b 00b2  B)c.(k.{[[[..+..
-00001590: 5f4b 16c3 2500 2501 b355 2501 b381 f255  _K..%.%..U%....U
-000015a0: 81f2 2e02 552f 1442 2863 853c c004 2479  ....U/.B(c.<..$y
-000015b0: 5b81 1b81 1c81 1d90 e12b 2346 5126 2346  [........+#FQ&#F
-000015c0: 2c12 8114 b312 811e 3402 445a b144 4612  ,.......4.DZ.DF.
-000015d0: 07b3 3401 6310 5e14 2332 0025 0014 4f36  ..4.c.^.#2.%..O6
-000015e0: 0034 0136 0163 b210 7ad9 4455 b144 4612  .4.6.c..z.DU.DF.
-000015f0: 07b3 3401 6310 5e14 2332 01b3 3401 3601  ..4.c.^.#2..4.6.
-00001600: 63b3 6302 8168 5908 7b5b 90e5 2b00 b05f  c.c..hY.{[..+.._
-00001610: 4b10 3002 c1c2 107d 141c b1b2 3602 2f14  K.0....}....6./.
-00001620: 422e 6381 4849 087b 5b90 eb2b 00b0 5f4b  B.c.HI.{[..+.._K
-00001630: 0cc1 107e 141c b136 012f 1442 3263 8400  ...~...6./.B2c..
-00001640: c902 1627 8106 a01c 6040 2228 4e2d 480c  ...'....`@"(N-H.
-00001650: 1203 121e b034 0259 5263 4a22 5712 8105  .....4.YRcJ"W...
-00001660: df44 5ac1 4910 120a 230b 141c b0b1 3602  .DZ.I...#.....6.
-00001670: 3401 5950 6351 51c1 2801 5d4a 015d 5163  4.YPcQQ.(.]J.]Qc
+00000d60: 6551 6389 00d0 421c 4c80 e060 402b 2922  eQc...B.L..`@+)"
+00000d70: 4025 4d39 5f35 1214 1333 1434 104d 3601  @%M9_5...3.4.M6.
+00000d80: c023 1214 1c36 00b0 1830 4840 120e 3400  .#...6...0H@..4.
+00000d90: c112 7f14 4322 8374 3601 5e51 6859 1281  ....C".t6.^QhY..
+00000da0: 1312 0f12 0e34 00b1 3402 2283 74f7 81f3  .....4..4.".t...
+00000db0: 2280 64f4 3401 c212 8113 1215 1352 b2f2  ".d.4........R..
+00000dc0: 82f7 3401 1215 1852 4202 4a1f 5712 8105  ..4....RB.J.W...
+00000dd0: df44 57c3 490d 120a 2313 141c b336 0134  .DW.I...#....6.4
+00000de0: 0159 5151 c328 035d 4a01 5db0 132e 1437  .YQQ.(.]J.]....7
+00000df0: 3600 5951 6384 20d8 8501 183e 4b31 5372  6.YQc. ....>K1Sr
+00000e00: 80f5 6040 4a27 3312 8114 b012 6b34 0244  ..`@J'3.....k4.D
+00000e10: 5a12 1514 5036 0059 1214 3400 143f 104b  Z...P6.Y..4..?.K
+00000e20: b010 53b2 1054 b336 8600 6312 1434 0014  ..S..T.6..c..4..
+00000e30: 3b10 4bb0 1031 b136 8400 6387 0878 1855  ;.K..1.6..c..x.U
+00000e40: 9002 6020 2c32 2f30 2c2a 2912 1513 5112  ..` ,2/0,*)...Q.
+00000e50: 1514 4e36 00f3 c023 1423 1514 1cb0 1215  ..N6...#.#......
+00000e60: 1352 3602 2316 2b03 c112 1413 3314 4f36  .R6.#.+.....3.O6
+00000e70: 005f 4b33 3002 c2c3 b313 2e14 3536 0044  ._K30.......56.D
+00000e80: 4410 5642 4210 57c4 1022 8a12 8107 b434  D.VBB.W..".....4
+00000e90: 01f3 f4c5 1058 141c b4b5 b236 03c6 b114  .....X.....6....
+00000ea0: 59b6 3601 5942 0b12 8115 b134 0163 8708  Y.6.YB.....4.c..
+00000eb0: 611e 5a31 9011 202b 2623 282c 3c29 2a23  a.Z1.. +&#(,<)*#
+00000ec0: 2212 1413 3314 34b0 5136 02c1 b151 de44  "...3.4.Q6...Q.D
+00000ed0: cb80 2b00 c2b0 141a 1040 3601 c312 1413  ..+......@6.....
+00000ee0: 3314 2636 005f 4b26 c4b4 1418 b380 5536  3.&6._K&......U6
+00000ef0: 0144 5912 8107 b334 0181 d844 4fb3 8155  .DY....4...DO..U
+00000f00: 105b d944 47b2 1459 b436 0159 4218 1281  .[.DG..Y.6.YB...
+00000f10: 07b2 3401 80d9 4443 2b00 63b2 63b0 2b01  ..4...DC+.c.c.+.
+00000f20: 6386 3071 1c5c 3190 2060 2028 2a28 2a2b  c.0q.\1. ` (*(*+
+00000f30: 2325 3712 1514 5ab0 3601 c112 8107 b134  #%7...Z.6......4
+00000f40: 0180 d944 4823 1714 1cb0 3601 6312 8107  ...DH#....6.c...
+00000f50: b134 0181 d944 4b12 1413 33b1 8055 5513  .4...DK...3..UU.
+00000f60: 3063 2b00 c2b1 5f4b 18c3 b214 5910 5d14  0c+..._K....Y.].
+00000f70: 1cb3 1214 1333 b355 1330 3602 3601 5942  .....3.U.06.6.YB
+00000f80: 2610 5e14 23b2 3601 6388 5481 1028 5f31  &.^.#.6.c.T..(_1
+00000f90: 9030 8007 8309 2822 2a2b 2a2b 2a23 2527  .0....("*+*+*#%'
+00000fa0: 302e 3200 c112 1514 5ab0 3601 c252 c312  0.2.....Z.6..R..
+00000fb0: 8107 b234 0180 d944 4bb3 2317 141c b036  ...4...DK.#....6
+00000fc0: 012a 0263 1281 07b2 3401 81d9 4455 2318  .*.c....4...DU#.
+00000fd0: 141c b280 55b3 3602 c4b1 b280 5534 01b4  ....U.6.....U4..
+00000fe0: 2a02 632b 00c5 b25f 4b18 c6b3 b1b6 3401  *.c+..._K.....4.
+00000ff0: e2c3 b514 5910 6014 1cb6 b336 0236 0159  ....Y.`....6.6.Y
+00001000: 4226 1061 141c 1062 1423 b536 0136 01c4  B&.a...b.#.6.6..
+00001010: b3b4 2a02 6301 8458 c902 127c 8120 9038  ..*.c..X...|. .8
+00001020: 2b22 592c 1214 1333 1434 b051 3602 c148  +"Y,...3.4.Q6..H
+00001030: 0fb1 51de 4442 5063 b114 4236 0063 4a21  ..Q.DBPc..B6.cJ!
+00001040: 5712 8105 df44 59c2 490f 120a 231b 141c  W....DY.I...#...
+00001050: b236 0134 0159 5063 5151 c228 025d 4a01  .6.4.YPcQQ.(.]J.
+00001060: 5d51 6384 28b8 020e 6390 5060 2257 2c48  ]Qc.(...c.P`"W,H
+00001070: 0d12 7f14 3d36 0014 6336 0059 4a2a 5712  ....=6..c6.YJ*W.
+00001080: 8105 df44 62c0 4918 120a 2319 141c b036  ...Db.I...#....6
+00001090: 0134 0159 127f 143d 3600 1464 3600 5951  .4.Y...=6..d6.YQ
+000010a0: 51c0 2800 5d4a 015d 5163 8218 2910 6581  Q.(.]J.]Qc..).e.
+000010b0: 1690 5b2c 2522 1214 1333 1434 1066 5136  ..[,%"...3.4.fQ6
+000010c0: 02c1 b151 de44 4251 63b0 b118 3051 6387  ...Q.DBQc...0Qc.
+000010d0: 3cd1 0220 1781 0490 6660 2042 2942 3027  <.. ....f` B)B0'
+000010e0: 5a2d 2c2b 4832 b014 1810 1936 0144 4252  Z-,+H2.....6.DBR
+000010f0: 6332 00b0 141a 101b 3601 5e34 015f 4b16  c2......6.^4._K.
+00001100: c112 1eb1 3401 434c 1209 2301 141c b136  ....4.CL..#....6
+00001110: 0134 0159 4228 4a2e 5712 8105 df44 66c2  .4.YB(J.W....Df.
+00001120: 491c 1209 2302 141c b0b2 3602 3401 5912  I...#.....6.4.Y.
+00001130: 0a23 0314 1cb2 3601 3401 5950 6351 51c2  .#....6.4.YPcQQ.
+00001140: 2802 5d4a 015d 5263 0182 38b9 4008 675b  (.]J.]Rc..8.@.g[
+00001150: 906f 53b0 5353 4b18 c112 8107 b134 0180  .oS.SSK......4..
+00001160: d844 33b1 1468 3600 141a 3600 6759 4226  .D3..h6...6.gYB&
+00001170: 5163 8378 c102 161d 8104 907a 6020 2228  Qc.x.......z` "(
+00001180: 4e2c 480c 1203 1217 b034 0259 5263 4a21  N,H......4.YRcJ!
+00001190: 5712 8105 df44 59c1 490f 120a 2304 141c  W....DY.I...#...
+000011a0: b136 0134 0159 5063 5151 c128 015d 4a01  .6.4.YPcQQ.(.]J.
+000011b0: 5d51 6383 3caa 019e 011e 8106 4490 8780  ]Qc.<.......D...
+000011c0: 0726 4486 2c60 2742 0001 2501 51de 4444  .&D.,`'B..%.Q.DD
+000011d0: 3200 2701 b0b1 2001 02c2 b225 0034 0144  2.'... ....%.4.D
+000011e0: 4252 6312 1f25 0025 0134 0263 0248 090a  BRc..%.%.4.c.H..
+000011f0: 6981 1690 8f51 6395 0893 124c 6a5b 5b81  i....Qc....Lj[[.
+00001200: 1790 9247 492d 2d28 2642 2528 3026 2228  ...GI--(&B%(0&"(
+00001210: 3122 2742 5028 302e 5122 5c46 2b2e 234e  1"'BP(0.Q"\F+.#N
+00001220: 4c42 1281 07b2 3401 c310 29b2 8055 d944  LB....4...)..U.D
+00001230: f380 b382 d944 6510 6bb2 8155 d944 5d10  .....De.k..U.D].
+00001240: 5e14 2312 1514 5536 0036 01c4 106c 141c  ^.#...U6.6...l..
+00001250: b436 01c4 2501 b434 0159 5263 b382 d844  .6..%..4.YRc...D
+00001260: 7b10 5fb2 8155 d944 5812 1514 5f10 31b2  {._..U.DX..._.1.
+00001270: 8255 3682 0030 02c5 c625 01b6 3401 5952  .U6..0...%..4.YR
+00001280: 6310 5cb2 8155 d944 5325 0112 1514 5c10  c.\..U.DS%....\.
+00001290: 31b2 8255 3682 0034 0159 5263 2501 231a  1..U6..4.YRc%.#.
+000012a0: 3401 5952 63b3 82d8 449d 8110 6d25 007f  4.YRc...D...m%..
+000012b0: 55dd 4493 8125 0014 6e7f 3601 c7b7 146f  U.D..%..n.6....o
+000012c0: 106d 3601 82d9 4443 5242 4150 c8b7 1470  .m6...DCRBAP...p
+000012d0: 106d 102f 3602 1468 3600 c9b9 1471 3600  .m./6..h6....q6.
+000012e0: 4448 1281 13b9 3401 4241 51c9 4812 1215  DH....4.BAQ.H...
+000012f0: 143e 2500 1053 b810 72b9 3684 01c5 4a1b  .>%..S..r.6...J.
+00001300: 5712 8105 df44 53ca 4909 2501 ba34 0159  W....DS.I.%..4.Y
+00001310: 5263 5151 ca28 0a5d 4a01 5d10 4014 2325  RcQQ.(.]J.].@.#%
+00001320: 0080 822e 0255 3601 cbb5 444e 2501 1073  .....U6...DN%..s
+00001330: 141c bb36 0134 0159 424c 2501 1074 141c  ...6.4.YBL%..t..
+00001340: bb36 0134 0159 5263 5063 9554 9e12 4b1f  .6.4.YRcPc.T..K.
+00001350: 8106 4490 c780 0883 0d85 0f27 4d2b 1f21  ..D........'M+.!
+00001360: 6327 2d42 7d2a 4c4d 5270 492b 6f2d 562a  c'-B}*LMRpI+o-V*
+00001370: 462b 2646 0a32 00c2 ba20 0101 c3b0 7f55  F+&F.2... .....U
+00001380: 1020 d9c4 b444 48b0 807f 2e02 5542 41b0  . ...DH.....UBA.
+00001390: c512 8107 b534 0182 db44 fc81 1021 141c  .....4...D...!..
+000013a0: b580 5536 01b5 8155 b210 2214 23b5 8251  ..U6...U..".#..Q
+000013b0: 2e02 5536 0134 015b 5ac6 c7c8 4890 01b6  ..U6.4.[Z...H...
+000013c0: 1205 ddd3 444d 1281 0810 2414 1cb6 3601  ....DM....$...6.
+000013d0: 3401 5948 1212 8109 1025 141c b6b7 b836  4.YH.....%.....6
+000013e0: 0334 0127 0a4a 5057 1281 05df 44c7 80c9  .4.'.JPW....D...
+000013f0: 493d b612 810a b934 01dd 446b 120a 2305  I=.....4..Dk..#.
+00001400: 141c b636 0134 0159 1281 0810 2414 1cb6  ...6.4.Y....$...
+00001410: 3601 3401 5912 8109 1025 141c b6b7 b836  6.4.Y....%.....6
+00001420: 0334 0127 0a42 4712 8105 b934 0165 5151  .4.'.BG....4.eQQ
+00001430: c928 095d 4a01 5db3 b4b7 250a 3403 270a  .(.]J.]...%.4.'.
+00001440: b112 810a 250a 3401 3401 5952 634a 4957  ....%.4.4.YRcJIW
+00001450: 1281 05df 44c0 80c9 4936 b123 0614 1cb6  ....D...I6.#....
+00001460: b7b9 3603 3401 5923 0712 810a b934 01dd  ..6.4.Y#.....4..
+00001470: 434b 2308 1281 0ab9 3401 dd44 52b6 1205  CK#.....4..DR...
+00001480: 1426 3600 dd44 4612 05b6 535b 5650 6351  .&6..DF...S[VPcQ
+00001490: 51c9 2809 5d4a 015d b123 0934 0159 b123  Q.(.]J.].#.4.Y.#
+000014a0: 0a34 0159 5263 0287 5c59 9c01 7581 1890  .4.YRc..\Y..u...
+000014b0: d022 2e2d 3625 2d2c 2a2a 0003 51c1 1076  .".-6%-,**..Q..v
+000014c0: 2500 dd43 4710 7725 00dd 4475 3200 1281  %..CG.w%..Du2...
+000014d0: 1925 0034 0134 0127 03b0 b320 0102 1281  .%.4.4.'... ....
+000014e0: 1a80 1281 0725 0334 0182 3403 3401 c1b1  .....%.4..4.4...
+000014f0: 5f4b 0ec2 2500 1470 b210 7836 0227 0042  _K..%..p..x6.'.B
+00001500: 3025 0014 7010 2210 6236 0227 0012 8114  0%..p.".b6.'....
+00001510: b112 6b34 0244 4a25 0014 1cb1 8137 0127  ..k4.DJ%.....7.'
+00001520: 0025 0063 0282 1049 087b 5b90 d22b 00b0  .%.c...I.{[..+..
+00001530: 5f4b 1530 02c1 c2b2 1077 d943 46b2 1076  _K.0.....w.CF..v
+00001540: d944 2eb1 2f14 4229 6382 286b 0c7b 5b5b  .D../.B)c.(k.{[[
+00001550: 5b90 d32b 00b2 5f4b 16c3 2500 2501 b355  [..+.._K..%.%..U
+00001560: 2501 b381 f255 81f2 2e02 552f 1442 2863  %....U....U/.B(c
+00001570: 853c c004 2479 5b81 1b81 1c81 1d90 dd2b  .<..$y[........+
+00001580: 2346 5126 2346 2c12 8114 b312 811e 3402  #FQ&#F,.......4.
+00001590: 445a b144 4612 07b3 3401 6310 5e14 2332  DZ.DF...4.c.^.#2
+000015a0: 0025 0014 4f36 0034 0136 0163 b210 7ad9  .%..O6.4.6.c..z.
+000015b0: 4455 b144 4612 07b3 3401 6310 5e14 2332  DU.DF...4.c.^.#2
+000015c0: 01b3 3401 3601 63b3 6302 8168 5908 7b5b  ..4.6.c.c..hY.{[
+000015d0: 90e1 2b00 b05f 4b10 3002 c1c2 107d 141c  ..+.._K.0....}..
+000015e0: b1b2 3602 2f14 422e 6381 4849 087b 5b90  ..6./.B.c.HI.{[.
+000015f0: e72b 00b0 5f4b 0cc1 107e 141c b136 012f  .+.._K...~...6./
+00001600: 1442 3263 8400 c902 1627 8106 a018 6040  .B2c.....'....`@
+00001610: 2228 4e2d 480c 1203 121e b034 0259 5263  "(N-H......4.YRc
+00001620: 4a22 5712 8105 df44 5ac1 4910 120a 230b  J"W....DZ.I...#.
+00001630: 141c b0b1 3602 3401 5950 6351 51c1 2801  ....6.4.YPcQQ.(.
+00001640: 5d4a 015d 5163                           ]J.]Qc
```

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/Time.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/Time.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/micrOS.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/micrOS.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/micrOSloader.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/micrOSloader.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.7/toolkit/workspace/precompiled/urequests.mpy` & `micrOSDevToolKit-1.20.8/toolkit/workspace/precompiled/urequests.mpy`

 * *Files identical despite different names*


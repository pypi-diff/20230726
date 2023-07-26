# Comparing `tmp/onoffmonitordevice-0.2.0-py3-none-any.whl.zip` & `tmp/onoffmonitordevice-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6466 bytes, number of entries: 11
+Zip file size: 7550 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-06 16:55 onoffmonitordevice/__init__.py
 -rw-r--r--  2.0 unx     1523 b- defN 23-Jul-24 15:42 onoffmonitordevice/__main__.py
--rw-r--r--  2.0 unx     1776 b- defN 23-Jul-25 10:45 onoffmonitordevice/device.py
+-rw-r--r--  2.0 unx     1904 b- defN 23-Jul-26 16:08 onoffmonitordevice/device.py
 -rw-r--r--  2.0 unx       43 b- defN 23-Jul-06 16:55 onoffmonitordevice/exceptions.py
--rw-r--r--  2.0 unx     4280 b- defN 23-Jul-24 15:37 onoffmonitordevice/monitor.py
--rw-r--r--  2.0 unx     1687 b- defN 23-Jul-25 10:53 onoffmonitordevice-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1112 b- defN 23-Jul-25 10:53 onoffmonitordevice-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 10:53 onoffmonitordevice-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       66 b- defN 23-Jul-25 10:53 onoffmonitordevice-0.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-25 10:53 onoffmonitordevice-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      976 b- defN 23-Jul-25 10:53 onoffmonitordevice-0.2.0.dist-info/RECORD
-11 files, 11574 bytes uncompressed, 4780 bytes compressed:  58.7%
+-rw-r--r--  2.0 unx     5076 b- defN 23-Jul-26 16:04 onoffmonitordevice/monitor.py
+-rw-r--r--  2.0 unx     1687 b- defN 23-Jul-26 16:12 onoffmonitordevice-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3065 b- defN 23-Jul-26 16:12 onoffmonitordevice-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-26 16:12 onoffmonitordevice-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       66 b- defN 23-Jul-26 16:12 onoffmonitordevice-0.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-26 16:12 onoffmonitordevice-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jul-26 16:12 onoffmonitordevice-0.3.0.dist-info/RECORD
+11 files, 14451 bytes uncompressed, 5864 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: onoffmonitordevice/exceptions.py
 Comment: 
 
 Filename: onoffmonitordevice/monitor.py
 Comment: 
 
-Filename: onoffmonitordevice-0.2.0.dist-info/LICENSE
+Filename: onoffmonitordevice-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: onoffmonitordevice-0.2.0.dist-info/METADATA
+Filename: onoffmonitordevice-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: onoffmonitordevice-0.2.0.dist-info/WHEEL
+Filename: onoffmonitordevice-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: onoffmonitordevice-0.2.0.dist-info/entry_points.txt
+Filename: onoffmonitordevice-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: onoffmonitordevice-0.2.0.dist-info/top_level.txt
+Filename: onoffmonitordevice-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: onoffmonitordevice-0.2.0.dist-info/RECORD
+Filename: onoffmonitordevice-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## onoffmonitordevice/device.py

```diff
@@ -1,21 +1,27 @@
+'''
+Module for managing a device
+'''
 # pylint:disable=no-member
 import logging
 from typing import Callable
 
 import RPi.GPIO as gpio
 
 from .exceptions import ValidationError
 
 
 class Device:
+    '''
+    Manage the state, GPIO pin(s), and events of a device
+    '''
     _logger = logging.getLogger(__name__)
 
     def __init__(self, setup: dict):
-        self._logger.debug('Initialising (%s)', str(setup))
+        self._logger.debug('Initialising (%s)', setup)
         if (
             isinstance(setup, dict)
             and isinstance(setup.get('id'), int)
             and isinstance(setup.get('gpio_input'), int)
         ):
             self._device_id: int = setup['id']
             self._input: int = setup['gpio_input']
@@ -35,20 +41,23 @@
         print(self._state, gpio.input(pin))
         if self._led is not None:
             gpio.output(self._led, self._state)
         if self._event is not None:
             self._event({'device': self._device_id, 'status': self._state})
 
     def begin(self, event: Callable):
+        '''
+        Set up the GPIO pin(s) and add events
+        '''
         self._logger.debug('Pin %i: begin', self._input)
         self._event = event
-        gpio.setup(self._input, gpio.IN)  # type: ignore
+        gpio.setup(self._input, gpio.IN)
         if self._led is not None:
             gpio.setup(self._led, gpio.OUT)
-        gpio.add_event_detect(  # type: ignore
+        gpio.add_event_detect(
             self._input,
-            gpio.BOTH,  # type: ignore
+            gpio.BOTH,
             callback=self._on_state_change
         )
 
     def __repr__(self):
         return f"Device({{'id': {self._device_id}, 'gpio_input': {self._input}, 'gpio_led': {self._led}}})"
```

## onoffmonitordevice/monitor.py

```diff
@@ -1,10 +1,11 @@
 """
 Module containing the main monitor program
 """
+# pylint:disable=no-member
 import getpass
 import json
 import logging
 from time import sleep
 from pathlib import Path
 
 import keyring
@@ -17,26 +18,31 @@
 
 class Monitor:
     """
     Starts a new monitor program
     """
     keyring_service = 'onoffmonitor'
     _logger = logging.getLogger(__name__)
+    gpio_modes = (gpio.BOARD, gpio.BCM)
 
     def __init__(self, settings_path: str):
         self._logger.debug('Initialising (%s)', settings_path)
         path = self._get_path(settings_path)
         self._request_headers = {}
         self._devices: list[Device] = []
+        self._gpio_mode = gpio.BOARD
         self._process_settings(json.loads(path.read_text()))
 
     def run(self):
+        '''
+        Start running this Monitor
+        '''
         self._logger.debug('Running')
         self._login()
-        self._fetch_devices()
+        self._fetch_conf()
         self._monitor()
 
     @staticmethod
     def _get_path(settings_path: str):
         path = Path(settings_path)
         if not path.exists():
             raise ValidationError(f'The file {settings_path} doesn\'t exist')
@@ -56,61 +62,88 @@
         if len(errors) != 0:
             raise ValidationError(*errors)
         self._host = settings['host']
         self._username = settings['username']
         self._monitor_id = settings['id']
         self._monitor_path = settings.get('monitorapi', '/api/onoffmonitor/')
         self._login_path = settings.get('loginapi', '/api/')
+        self._status_path = f'{self._host}{self._monitor_path}status/'
 
     def _login(self):
         self._logger.debug('Logging in')
         password = keyring.get_password(self.keyring_service, self._username)
         while True:
             if password is None:
                 password = getpass.getpass(
                     f'Enter password for {self._username}: ')
             request = requests.post(
-                self._host + self._login_path + 'login/', auth=(self._username, password), timeout=10)
+                f'{self._host}{self._login_path}login/',
+                auth=(self._username, password),
+                timeout=10
+            )
             response = request.json()
             if 'token' in response:
                 self._request_headers['Authorization'] = f'Token {response["token"]}'
                 keyring.set_password(self.keyring_service,
                                      self._username, password)
                 self._logger.info('Logged in as %s', self._username)
                 break
             password = None
             if 'detail' in response:
                 self._logger.error(response['detail'])
             else:
                 self._logger.error('Response from server: %s', response)
 
-    def _fetch_devices(self):
-        self._logger.debug('Fetching device configuration')
-        request = requests.get('%s%smonitor/%i/conf/' % (self._host, self._monitor_path, self._monitor_id), headers=self._request_headers)
+    def _fetch_conf(self):
+        self._logger.debug('Fetching monitor configuration')
+        request = requests.get(
+            f'{self._host}{self._monitor_path}monitor/{self._monitor_id}/conf/',
+            headers=self._request_headers,
+            timeout=10
+        )
         response = request.json()
-        for device in response:
+        gpio_mode = response.get('gpio_mode')
+        if isinstance(gpio_mode, int) and 0 <= gpio_mode < len(self.gpio_modes):
+            self._gpio_mode = self.gpio_modes[gpio_mode]
+        self._logger.debug('GPIO mode: %i', self._gpio_mode)
+        for device in response.get('devices', []):
             self._devices.append(Device(device))
-        self._logger.debug('Devices: %s', str(self._devices))
+        self._logger.debug('Devices: %s', self._devices)
 
     def _monitor(self):
-        gpio.setmode(gpio.BOARD)
+        gpio.setmode(self._gpio_mode)
         for device in self._devices:
             device.begin(self.on_device_state_change)
         print('Sleeping')
         sleep(20)
 
     def on_device_state_change(self, data):
-        self._logger.debug('Sending %s', str(data))
-        request = requests.post(self._host + self._monitor_path + 'status/', json=data, headers=self._request_headers)
+        '''
+        Event handler for device state change
+        '''
+        self._logger.debug('Sending %s', data)
+        request = requests.post(
+            self._status_path,
+            json=data,
+            headers=self._request_headers,
+            timeout=10
+        )
         self._logger.debug(request.text)
 
     def stop(self):
+        '''
+        Stop running this Monitor
+        '''
         self._logger.debug('Stopping')
+        gpio.cleanup()
         self._logout()
 
     def _logout(self):
         if 'Authorization' not in self._request_headers:
             self._logger.debug('Already logged out')
             return
         self._logger.debug('Logging out')
-        requests.post(self._host + self._login_path + 'logout/', headers=self._request_headers)
-        self._request_headers.clear()
+        requests.post(
+            f'{self._host}{self._login_path}logout/',
+            headers=self._request_headers,
+            timeout=10
+        )
```

## Comparing `onoffmonitordevice-0.2.0.dist-info/LICENSE` & `onoffmonitordevice-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `onoffmonitordevice-0.2.0.dist-info/RECORD` & `onoffmonitordevice-0.3.0.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 onoffmonitordevice/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 onoffmonitordevice/__main__.py,sha256=NlqTgn9mqnJAkXj40l-KU5b_CN75ED3epYxzJXCb1BQ,1523
-onoffmonitordevice/device.py,sha256=GyuBeZ9Osb12JXzyXLeeVxjRoUqvg4RxOnzYAUstzz0,1776
+onoffmonitordevice/device.py,sha256=46FANpxeaiAqVFIDtoBzz8dTqohZDYYQ0cY73Mmdbzw,1904
 onoffmonitordevice/exceptions.py,sha256=ifvhlxVWqvNDv8EGYdTGuvYwVV-s0K_mbbwL7vBZiHk,43
-onoffmonitordevice/monitor.py,sha256=E6W_8DvNxNrpwW_J1vHn5DEXAjNlr9-lC1W9qxfTgmc,4280
-onoffmonitordevice-0.2.0.dist-info/LICENSE,sha256=EauXk7lwd6z-a8bJgvo3A7hc81tjj_NBScbdp-ON9mA,1687
-onoffmonitordevice-0.2.0.dist-info/METADATA,sha256=l8KRPdYC5YwjSpJvISmjLPux-Cc4dGko8ePMWgTp7gE,1112
-onoffmonitordevice-0.2.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-onoffmonitordevice-0.2.0.dist-info/entry_points.txt,sha256=bHUy4t3W6x822izmj0ZlnD7pslK3Mpm58vdcFv9LsMU,66
-onoffmonitordevice-0.2.0.dist-info/top_level.txt,sha256=y1P0gLW_WugW-4aoqMBNPYlXJl6DEsrWSgwUONzFjH0,19
-onoffmonitordevice-0.2.0.dist-info/RECORD,,
+onoffmonitordevice/monitor.py,sha256=TDOOUcmQzZCvyerV-csfoy-NMHFc7lwL4S37e11L668,5076
+onoffmonitordevice-0.3.0.dist-info/LICENSE,sha256=EauXk7lwd6z-a8bJgvo3A7hc81tjj_NBScbdp-ON9mA,1687
+onoffmonitordevice-0.3.0.dist-info/METADATA,sha256=-7lN5rBHYJh17SU3oy5XdUJpRN0u8VLSM8bU0mkI9jk,3065
+onoffmonitordevice-0.3.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+onoffmonitordevice-0.3.0.dist-info/entry_points.txt,sha256=bHUy4t3W6x822izmj0ZlnD7pslK3Mpm58vdcFv9LsMU,66
+onoffmonitordevice-0.3.0.dist-info/top_level.txt,sha256=y1P0gLW_WugW-4aoqMBNPYlXJl6DEsrWSgwUONzFjH0,19
+onoffmonitordevice-0.3.0.dist-info/RECORD,,
```


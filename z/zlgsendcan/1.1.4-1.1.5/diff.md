# Comparing `tmp/zlgsendcan-1.1.4.tar.gz` & `tmp/zlgsendcan-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlgsendcan-1.1.4.tar", last modified: Wed Jul 26 09:43:01 2023, max compression
+gzip compressed data, was "zlgsendcan-1.1.5.tar", last modified: Wed Jul 26 12:21:36 2023, max compression
```

## Comparing `zlgsendcan-1.1.4.tar` & `zlgsendcan-1.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 09:43:01.279761 zlgsendcan-1.1.4/
--rw-rw-rw-   0        0        0      220 2023-07-26 09:43:01.279761 zlgsendcan-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-26 09:43:01.280761 zlgsendcan-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      463 2023-07-26 09:42:56.000000 zlgsendcan-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:43:01.269755 zlgsendcan-1.1.4/zlgsendcan/
--rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.1.4/zlgsendcan/__init__.py
--rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.1.4/zlgsendcan/frozen_dir.py
--rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.1.4/zlgsendcan/get_conf_info.py
--rw-rw-rw-   0        0        0     5211 2023-07-19 02:48:32.000000 zlgsendcan-1.1.4/zlgsendcan/parseDBC.py
--rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.1.4/zlgsendcan/yaml_util.py
--rw-rw-rw-   0        0        0    25077 2023-07-26 09:27:40.000000 zlgsendcan-1.1.4/zlgsendcan/zlgcan1.py
--rw-rw-rw-   0        0        0    18584 2023-07-26 09:42:40.000000 zlgsendcan-1.1.4/zlgsendcan/zlgserver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:43:01.277760 zlgsendcan-1.1.4/zlgsendcan.egg-info/
--rw-rw-rw-   0        0        0      220 2023-07-26 09:43:01.000000 zlgsendcan-1.1.4/zlgsendcan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-07-26 09:43:01.000000 zlgsendcan-1.1.4/zlgsendcan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 09:43:01.000000 zlgsendcan-1.1.4/zlgsendcan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-26 09:43:01.000000 zlgsendcan-1.1.4/zlgsendcan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-26 09:43:01.000000 zlgsendcan-1.1.4/zlgsendcan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 12:21:36.533149 zlgsendcan-1.1.5/
+-rw-rw-rw-   0        0        0      220 2023-07-26 12:21:36.532149 zlgsendcan-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-26 12:21:36.533149 zlgsendcan-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      463 2023-07-26 12:21:23.000000 zlgsendcan-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:21:36.524149 zlgsendcan-1.1.5/zlgsendcan/
+-rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.1.5/zlgsendcan/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.1.5/zlgsendcan/frozen_dir.py
+-rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.1.5/zlgsendcan/get_conf_info.py
+-rw-rw-rw-   0        0        0     5262 2023-07-26 12:12:26.000000 zlgsendcan-1.1.5/zlgsendcan/parseDBC.py
+-rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.1.5/zlgsendcan/yaml_util.py
+-rw-rw-rw-   0        0        0    26010 2023-07-26 12:01:29.000000 zlgsendcan-1.1.5/zlgsendcan/zlgcan1.py
+-rw-rw-rw-   0        0        0    18925 2023-07-26 12:20:21.000000 zlgsendcan-1.1.5/zlgsendcan/zlgserver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:21:36.531149 zlgsendcan-1.1.5/zlgsendcan.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-07-26 12:21:36.000000 zlgsendcan-1.1.5/zlgsendcan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-07-26 12:21:36.000000 zlgsendcan-1.1.5/zlgsendcan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 12:21:36.000000 zlgsendcan-1.1.5/zlgsendcan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-26 12:21:36.000000 zlgsendcan-1.1.5/zlgsendcan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-26 12:21:36.000000 zlgsendcan-1.1.5/zlgsendcan.egg-info/top_level.txt
```

### Comparing `zlgsendcan-1.1.4/zlgsendcan/get_conf_info.py` & `zlgsendcan-1.1.5/zlgsendcan/get_conf_info.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.4/zlgsendcan/parseDBC.py` & `zlgsendcan-1.1.5/zlgsendcan/parseDBC.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
 
 class GlobleValue:
     thread_obj = {}
     global_msg = {}
     global_msg2 = {}
     global_msg3 = {}
-    chanl=0
+    can_conf={'can_type':'can','chan':0,'zcy':None,'sjy':None}
     zlginit = None
     dbc_path = None
     thread_run = False
     flag_trace = False
     thread_sigchange_flag = False
     data_log = []
     sql_flag = False
```

### Comparing `zlgsendcan-1.1.4/zlgsendcan/yaml_util.py` & `zlgsendcan-1.1.5/zlgsendcan/yaml_util.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.4/zlgsendcan/zlgcan1.py` & `zlgsendcan-1.1.5/zlgsendcan/zlgcan1.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 #  Author : guochuangjian    
 #  Last change: 21.02.2019
 #
 #  Language: Python 2.7, 3.6
 #  ------------------------------------------------------------------
 #
 import os
+import re
 import sys
 from ctypes import *
 import platform
-from zlgsendcan import frozen_dir
-import pkg_resources
+import frozen_dir
 
 SETUP_DIR = frozen_dir.app_path() + r'\zlgcan_1.dll'
 sys.path.append(SETUP_DIR)
 
 ZCAN_DEVICE_TYPE = c_uint
 
 INVALID_DEVICE_HANDLE = 0
@@ -323,18 +323,17 @@
 
 class ZCAN(object):
     def __init__(self):
         if platform.system() == "Windows":
             try:
                 base_path = sys._MEIPASS
             except Exception:
-                base_path = os.path.abspath('..')
-            dll_path = os.path.join(base_path, 'zlgcan_1.dll')
-            # dll_path = os.path.join('D:\\auto-qt\\newauto\zlgcan_1.dll')
-            dll_path = pkg_resources.resource_filename('zlgsendcan', 'zlgcan_1.dll')
+                base_path = os.path.abspath('.')
+            # dll_path = os.path.join(base_path, 'zlgcan_1.dll')
+            dll_path = os.path.join('D:\\auto-qt\\newauto\zlgcan_1.dll')
             self.__dll = windll.LoadLibrary(dll_path)
 
         else:
             print("No support now!")
         if self.__dll == None:
             print("DLL couldn't be loaded!")
 
@@ -510,36 +509,55 @@
             raise
 
 
 ###############################################################################
 '''
 USBCANFD-MINI Demo
 '''
+def convert_speed(speed):
+    # 通过正则表达式提取数字和单位
+    match = re.match(r'(\d+(\.\d+)?)\s*(kbps|Mbps)', speed, re.IGNORECASE)
+    if match:
+        value = float(match.group(1))  # 提取数值部分
+        unit = match.group(3).lower()  # 提取单位并转换为小写
+
+        # 根据单位进行转换
+        if unit == 'kbps':
+            value *= 1000
+        elif unit == 'mbps':
+            value *= 1000000
 
+        return str(value)  # 返回转换后的速度值
+
+    return None  # 如果无法匹配，则返回None
 
 def canfd_start(zcanlib, device_handle, chn, data):
-    init_conf = data['can初始化配置']
+    # init_conf = data['can初始化配置']
+    init_conf = data
     ip = zcanlib.GetIProperty(device_handle)
-    if init_conf['仲裁域'][0] == '自定义':
-        ret = zcanlib.SetValue(ip, str(chn) + "/baud_rate_custom", init_conf['自定义波特率'])
+    # if init_conf['仲裁域'][0] == '自定义':
+    #     ret = zcanlib.SetValue(ip, str(chn) + "/baud_rate_custom", init_conf['自定义波特率'])
+    if init_conf['zcy'] == '自定义':
+        ret = zcanlib.SetValue(ip, str(chn) + "/baud_rate_custom", init_conf['sjy'])
     else:
 
         ret = zcanlib.SetValue(ip, str(chn) + "/clock", "60000000")
         # print("ret", ret, ip)
         if ret != ZCAN_STATUS_OK:
             print("Set CH%d CANFD clock failed!" % (chn))
         ret = zcanlib.SetValue(ip, str(chn) + "/canfd_standard", "0")
         if ret != ZCAN_STATUS_OK:
             print("Set CH%d CANFD standard failed!" % (chn))
         ret = zcanlib.SetValue(ip, str(chn) + "/initenal_resistance", "1")
         if ret != ZCAN_STATUS_OK:
             print("Open CH%d resistance failed!" % (chn))
         # 500Kbps(85%),2.0Mbps(80%),(20,00000520,00000106)
-        ret = zcanlib.SetValue(ip, str(chn) + "/canfd_abit_baud_rate", "500000")  # 设置波特率
-        ret = zcanlib.SetValue(ip, str(chn) + "/canfd_dbit_baud_rate", "2000000")
+
+        ret = zcanlib.SetValue(ip, str(chn) + "/canfd_abit_baud_rate", convert_speed(init_conf['zcy']))  # 设置波特率
+        ret = zcanlib.SetValue(ip, str(chn) + "/canfd_dbit_baud_rate", convert_speed(init_conf['sjy']))
         if ret != ZCAN_STATUS_OK:
             print("Set CH%d baud failed!" % (chn))
 
     # ret = zcanlib.SetValue(ip, "0/set_cn","A001")
     # if ret == ZCAN_STATUS_OK:
     #     t = zcanlib.GetValue(ip, "0/get_cn/1")
     ret = zcanlib.SetValue(ip, str(chn) + "/set_device_recv_merge", "1")
@@ -597,118 +615,118 @@
       print("Apply CH%d USBCANFD AutoSend failed!" %(chn))'''
 
     zcanlib.ReleaseIProperty(ip)
     return chn_handle
 
 
 if __name__ == "__main__":
-
-    zcanlib = ZCAN()
-    # testcantype =0 #0:CAN; 1:canfd
-    handle = zcanlib.OpenDevice(ZCAN_USBCANFD_200U, 0, 0)
-    if handle == INVALID_DEVICE_HANDLE:
-        print("Open CANFD Device failed!")
-
-    print("device handle:%d." % (handle))
-
-    info = zcanlib.GetDeviceInf(handle)
-    print("Device Information:\n%s" % (info))
-
-    # set auto send obj
-
-    # AutoCAN_A    =  ZCAN_AUTO_TRANSMIT_OBJ()
-    # AutoCAN_B    =  ZCAN_AUTO_TRANSMIT_OBJ()
-    # AutoCAN_A.enable                    = 1  #enable
-    # AutoCAN_A.index                     = 0
-    # AutoCAN_A.interval                  = 200  #ms
-    # AutoCAN_A.obj.frame.can_id          = 0x100
-    # AutoCAN_A.obj.transmit_type         = 0
-    # AutoCAN_A.obj.frame.eff             = 0
-    # AutoCAN_A.obj.frame.rtr             = 0
-    # AutoCAN_A.obj.frame.can_dlc         = 8
-    # for j in range(AutoCAN_A.obj.frame.can_dlc):
-    #     AutoCAN_A.obj.frame.data[j] = j
-    #
-    # AutoCAN_B.enable                    = 1  #enable
-    # AutoCAN_B.index                     = 1
-    # AutoCAN_B.interval                  = 200  #ms
-    # AutoCAN_B.obj.frame.can_id          = 0x300
-    # AutoCAN_B.obj.transmit_type         = 0
-    # AutoCAN_B.obj.frame.eff             = 0
-    # AutoCAN_B.obj.frame.rtr             = 0
-    # AutoCAN_B.obj.frame.can_dlc         = 8
-    # for j in range(AutoCAN_B.obj.frame.can_dlc):
-    #     AutoCAN_B.obj.frame.data[j] = j
-    #
-    # AutoCAN_B_delay=ZCANFD_AUTO_TRANSMIT_OBJ_PARAM()
-    # AutoCAN_B_delay.index = AutoCAN_B.index
-    # AutoCAN_B_delay.type  = 1
-    # AutoCAN_B_delay.value = 100
-
-    # Start CAN
-
-    chn_handle = canfd_start(zcanlib, handle, 0)
-    print("channel handle:%d." % (chn_handle))
-
-    # Send CAN Messages
-
-    DataObj = (ZCANDataObj * 2)()
-    for i in range(1):
-        DataObj[i].dataType = 1  # can/canfd frame
-        DataObj[i].chnl = 0  # can_channel
-        DataObj[i].zcanfddata.flag.frameType = 1  # 0-can,1-canfd
-        DataObj[i].zcanfddata.flag.txDelay = 0  # 不添加延迟
-        DataObj[i].zcanfddata.flag.transmitType = 0  # 发送方式，0-正常发送
-        DataObj[i].zcanfddata.flag.txEchoRequest = 1  # 发送回显请求，0-不回显，1-回显
-        DataObj[i].zcanfddata.frame.can_id = 793
-        DataObj[i].zcanfddata.frame.len = 16
-        a = [0, 0, 64, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
-        for j in range(DataObj[i].zcanfddata.frame.len):
-            DataObj[i].zcanfddata.frame.data[j] = a[j]
-    ret = zcanlib.TransmitData(chn_handle, DataObj, 1)
-
-    # print("Tranmit Num: %d." % ret)
-
-    # thread=threading.Thread(target=input_thread)
-    # thread.start()
-
-    # Receive Messages
-    while True:
-        rcv_num = zcanlib.GetReceiveNum(chn_handle, ZCAN_TYPE_CAN)
-        rcv_canfd_num = zcanlib.GetReceiveNum(chn_handle, ZCAN_TYPE_CANFD)
-        if rcv_num:
-            print("Receive CAN message number:%d" % rcv_num)
-            rcv_msg, rcv_num = zcanlib.Receive(chn_handle, rcv_num)
-            for i in range(rcv_num):
-                print("[%d]:timestamps:%d,type:CAN, id:%s, dlc:%d, eff:%d, rtr:%d, data:%s" % (i, rcv_msg[i].timestamp,
-                                                                                               hex(rcv_msg[
-                                                                                                       i].frame.can_id),
-                                                                                               rcv_msg[i].frame.can_dlc,
-                                                                                               rcv_msg[i].frame.eff,
-                                                                                               rcv_msg[i].frame.rtr,
-                                                                                               ''.join(hex(rcv_msg[
-                                                                                                               i].frame.data[
-                                                                                                               j]) + ' '
-                                                                                                       for j in range(
-                                                                                                   rcv_msg[
-                                                                                                       i].frame.can_dlc))))
-        elif rcv_canfd_num:
-            print("Receive CANFD message number:%d" % rcv_canfd_num)
-            rcv_canfd_msgs, rcv_canfd_num = zcanlib.ReceiveFD(chn_handle, rcv_canfd_num, 1000)
-            for i in range(rcv_canfd_num):
-                print("[%d]:timestamp:%d,type:canfd, id:%s, len:%d, eff:%d, rtr:%d, esi:%d, brs: %d, data:%s" % (
-                    i, rcv_canfd_msgs[i].timestamp, hex(rcv_canfd_msgs[i].frame.can_id), rcv_canfd_msgs[i].frame.len,
-                    rcv_canfd_msgs[i].frame.eff, rcv_canfd_msgs[i].frame.rtr,
-                    rcv_canfd_msgs[i].frame.esi, rcv_canfd_msgs[i].frame.brs,
-                    ''.join(hex(rcv_canfd_msgs[i].frame.data[j]) + ' ' for j in range(rcv_canfd_msgs[i].frame.len))))
-        # else:
-        #     if thread.is_alive() == False:
-        #         break
-
-    # Close CAN
-    ret = zcanlib.ResetCAN(chn_handle)
-    if ret == 1:
-        print("ResetCAN success! ")
-    # Close Device
-    ret = zcanlib.CloseDevice(handle)
-    if ret == 1:
-        print("CloseDevice success! ")
+    print(convert_speed('5Mbps 80%'))
+    # zcanlib = ZCAN()
+    # # testcantype =0 #0:CAN; 1:canfd
+    # handle = zcanlib.OpenDevice(ZCAN_USBCANFD_200U, 0, 0)
+    # if handle == INVALID_DEVICE_HANDLE:
+    #     print("Open CANFD Device failed!")
+    #
+    # print("device handle:%d." % (handle))
+    #
+    # info = zcanlib.GetDeviceInf(handle)
+    # print("Device Information:\n%s" % (info))
+    #
+    # # set auto send obj
+    #
+    # # AutoCAN_A    =  ZCAN_AUTO_TRANSMIT_OBJ()
+    # # AutoCAN_B    =  ZCAN_AUTO_TRANSMIT_OBJ()
+    # # AutoCAN_A.enable                    = 1  #enable
+    # # AutoCAN_A.index                     = 0
+    # # AutoCAN_A.interval                  = 200  #ms
+    # # AutoCAN_A.obj.frame.can_id          = 0x100
+    # # AutoCAN_A.obj.transmit_type         = 0
+    # # AutoCAN_A.obj.frame.eff             = 0
+    # # AutoCAN_A.obj.frame.rtr             = 0
+    # # AutoCAN_A.obj.frame.can_dlc         = 8
+    # # for j in range(AutoCAN_A.obj.frame.can_dlc):
+    # #     AutoCAN_A.obj.frame.data[j] = j
+    # #
+    # # AutoCAN_B.enable                    = 1  #enable
+    # # AutoCAN_B.index                     = 1
+    # # AutoCAN_B.interval                  = 200  #ms
+    # # AutoCAN_B.obj.frame.can_id          = 0x300
+    # # AutoCAN_B.obj.transmit_type         = 0
+    # # AutoCAN_B.obj.frame.eff             = 0
+    # # AutoCAN_B.obj.frame.rtr             = 0
+    # # AutoCAN_B.obj.frame.can_dlc         = 8
+    # # for j in range(AutoCAN_B.obj.frame.can_dlc):
+    # #     AutoCAN_B.obj.frame.data[j] = j
+    # #
+    # # AutoCAN_B_delay=ZCANFD_AUTO_TRANSMIT_OBJ_PARAM()
+    # # AutoCAN_B_delay.index = AutoCAN_B.index
+    # # AutoCAN_B_delay.type  = 1
+    # # AutoCAN_B_delay.value = 100
+    #
+    # # Start CAN
+    #
+    # chn_handle = canfd_start(zcanlib, handle, 0)
+    # print("channel handle:%d." % (chn_handle))
+    #
+    # # Send CAN Messages
+    #
+    # DataObj = (ZCANDataObj * 2)()
+    # for i in range(1):
+    #     DataObj[i].dataType = 1  # can/canfd frame
+    #     DataObj[i].chnl = 0  # can_channel
+    #     DataObj[i].zcanfddata.flag.frameType = 1  # 0-can,1-canfd
+    #     DataObj[i].zcanfddata.flag.txDelay = 0  # 不添加延迟
+    #     DataObj[i].zcanfddata.flag.transmitType = 0  # 发送方式，0-正常发送
+    #     DataObj[i].zcanfddata.flag.txEchoRequest = 1  # 发送回显请求，0-不回显，1-回显
+    #     DataObj[i].zcanfddata.frame.can_id = 793
+    #     DataObj[i].zcanfddata.frame.len = 16
+    #     a = [0, 0, 64, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
+    #     for j in range(DataObj[i].zcanfddata.frame.len):
+    #         DataObj[i].zcanfddata.frame.data[j] = a[j]
+    # ret = zcanlib.TransmitData(chn_handle, DataObj, 1)
+    #
+    # # print("Tranmit Num: %d." % ret)
+    #
+    # # thread=threading.Thread(target=input_thread)
+    # # thread.start()
+    #
+    # # Receive Messages
+    # while True:
+    #     rcv_num = zcanlib.GetReceiveNum(chn_handle, ZCAN_TYPE_CAN)
+    #     rcv_canfd_num = zcanlib.GetReceiveNum(chn_handle, ZCAN_TYPE_CANFD)
+    #     if rcv_num:
+    #         print("Receive CAN message number:%d" % rcv_num)
+    #         rcv_msg, rcv_num = zcanlib.Receive(chn_handle, rcv_num)
+    #         for i in range(rcv_num):
+    #             print("[%d]:timestamps:%d,type:CAN, id:%s, dlc:%d, eff:%d, rtr:%d, data:%s" % (i, rcv_msg[i].timestamp,
+    #                                                                                            hex(rcv_msg[
+    #                                                                                                    i].frame.can_id),
+    #                                                                                            rcv_msg[i].frame.can_dlc,
+    #                                                                                            rcv_msg[i].frame.eff,
+    #                                                                                            rcv_msg[i].frame.rtr,
+    #                                                                                            ''.join(hex(rcv_msg[
+    #                                                                                                            i].frame.data[
+    #                                                                                                            j]) + ' '
+    #                                                                                                    for j in range(
+    #                                                                                                rcv_msg[
+    #                                                                                                    i].frame.can_dlc))))
+    #     elif rcv_canfd_num:
+    #         print("Receive CANFD message number:%d" % rcv_canfd_num)
+    #         rcv_canfd_msgs, rcv_canfd_num = zcanlib.ReceiveFD(chn_handle, rcv_canfd_num, 1000)
+    #         for i in range(rcv_canfd_num):
+    #             print("[%d]:timestamp:%d,type:canfd, id:%s, len:%d, eff:%d, rtr:%d, esi:%d, brs: %d, data:%s" % (
+    #                 i, rcv_canfd_msgs[i].timestamp, hex(rcv_canfd_msgs[i].frame.can_id), rcv_canfd_msgs[i].frame.len,
+    #                 rcv_canfd_msgs[i].frame.eff, rcv_canfd_msgs[i].frame.rtr,
+    #                 rcv_canfd_msgs[i].frame.esi, rcv_canfd_msgs[i].frame.brs,
+    #                 ''.join(hex(rcv_canfd_msgs[i].frame.data[j]) + ' ' for j in range(rcv_canfd_msgs[i].frame.len))))
+    #     # else:
+    #     #     if thread.is_alive() == False:
+    #     #         break
+    #
+    # # Close CAN
+    # ret = zcanlib.ResetCAN(chn_handle)
+    # if ret == 1:
+    #     print("ResetCAN success! ")
+    # # Close Device
+    # ret = zcanlib.CloseDevice(handle)
+    # if ret == 1:
+    #     print("CloseDevice success! ")
```

### Comparing `zlgsendcan-1.1.4/zlgsendcan/zlgserver.py` & `zlgsendcan-1.1.5/zlgsendcan/zlgserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 import copy
 import importlib
 import time
 from PyQt5.QtWidgets import QMessageBox
-from zlgsendcan.parseDBC import GlobleValue, DbcInit
+from parseDBC import GlobleValue, DbcInit
 from zlgsendcan.zlgcan1 import *
 import threading
-from zlgsendcan.get_conf_info import GetBaseInfo
+from get_conf_info import GetBaseInfo
+
 data_ = GetBaseInfo().get_base_config()
 condition = threading.Condition()
 
 
 class MessageDate:
-    def __init__(self):
-        data_ = GetBaseInfo().get_base_config()
+    def __init__(self,can_type,chanl,brate:dict):
+        """
+
+        :param can_type: 1、can 2、canfd
+        :param chanl: 0,1
+        :param brate: {'zcy':'500kbps 80%','sjy':'2Mbps 80%‘}注意如果自定义波特率格式如下
+                        {'zcy':'自定义','sjy':‘500Kbps(85%),2.0Mbps(80%),(20,00000520,00000106)’}
+        """
+        GlobleValue.can_conf['chan'] = chanl
+        GlobleValue.can_conf['zcy'] = brate['zcy']
+        GlobleValue.can_conf['can_type'] = can_type
+        GlobleValue.can_conf['sjy']=brate['sjy']
+
         self.zcanlib = ZCAN()
         # self.testcantype = 1  # 0:CAN; 1:canfd
         self.handle = self.zcanlib.OpenDevice(ZCAN_USBCANFD_200U, 0, 0)
         if self.handle == INVALID_DEVICE_HANDLE:
             msgbox = QMessageBox(QMessageBox.Critical, '错误', "请检查周立功是否连接或重复开启！")
             msgbox.adjustSize()
             msgbox.show()
@@ -24,15 +36,15 @@
             print("Open CANFD Device failed!")
             # exit(0)
         print("device handle:%d." % (self.handle))
         info = self.zcanlib.GetDeviceInf(self.handle)
         print("Device Information:\n%s" % (info))
 
         # Start CAN
-        self.chn_handle = canfd_start(self.zcanlib, self.handle, int(GlobleValue.chanl), data_)
+        self.chn_handle = canfd_start(self.zcanlib, self.handle, int(GlobleValue.can_conf['chan']), GlobleValue.can_conf)
         print("channel handle:%d." % (self.chn_handle))
 
     # 检查设备是否在线
     def check_device_online(self):
         return self.zcanlib.DeviceOnLine(self.handle)
 
     def clear_buffer(self):
@@ -84,17 +96,16 @@
         data_len = len(data)
         # print('=============',data_len)
         canfd_msgs = (ZCANDataObj * data_len)()
         # memset(byref(canfd_msgs), 0, sizeof(canfd_msgs))
         # canfd_msgs = (ZCAN_TransmitFD_Data * 10)()
         for i in range(data_len):
             canfd_msgs[i].dataType = 1  # can/canfd frame
-            canfd_msgs[i].chnl = int(GlobleValue.chanl)  # can_channel
-            canfd_msgs[i].zcanfddata.flag.frameType = 1 if data_['can初始化配置']['协议']['周立功'][
-                                                               0] == 'canfd' else 0  # 0-can,1-canfd
+            canfd_msgs[i].chnl = int(GlobleValue.can_conf['chan'])  # can_channel
+            canfd_msgs[i].zcanfddata.flag.frameType = 1 if GlobleValue.can_conf['can_type'] == 'canfd' else 0  # 0-can,1-canfd
             # canfd_msgs[i].zcanfddata.frame.eff = 0
             # canfd_msgs[i].zcanfddata.frame.rtr = 0
             # canfd_msgs[i].zcanfddata.frame.brs = 1
             # canfd_msgs[i].zcanfddata.frame.esi = 0
             # canfd_msgs[i].zcanfddata.frame.__pad = 0x20  # 队列发送，当值为0x20时，单位为ms;  当值为0x30时，单位是100us。
             # canfd_msgs[i].zcanfddata.frame.__res0 = 0x1388  # 帧间隔低位,定时100ms
             # canfd_msgs[i].zcanfddata.frame.__res1 = 0x00  # 帧间隔高位
@@ -114,17 +125,16 @@
 
 # 普通发送
 def canfd_msg_power(idx, data):
     data_ = GetBaseInfo().get_base_config()
     canfd_msgs = (ZCANDataObj * 1)()
     for i in range(1):
         canfd_msgs[i].dataType = 1  # can/canfd frame
-        canfd_msgs[i].chnl = int(data_['can初始化配置']['通道'][0])  # can_channel
-        canfd_msgs[i].zcanfddata.flag.frameType = 1 if data_['can初始化配置']['协议'][
-                                                           0] == 'canfd' else 0  # 0-can,1-canfd
+        canfd_msgs[i].chnl = int(GlobleValue.can_conf['chan']) # can_channel
+        canfd_msgs[i].zcanfddata.flag.frameType = 1 if GlobleValue.can_conf['can_type'] == 'canfd' else 0  # 0-can,1-canfd
         canfd_msgs[i].zcanfddata.flag.txDelay = 0  # 不添加延迟
         canfd_msgs[i].zcanfddata.flag.transmitType = 0  # 发送方式，0-正常发送
         canfd_msgs[i].zcanfddata.flag.txEchoRequest = 1  # 发送回显请求，0-不回显，1-回显
         canfd_msgs[i].zcanfddata.frame.can_id = int(idx, 16)
         canfd_msgs[i].zcanfddata.frame.len = 8
         canfd_msgs[i].zcanfddata.flag.txEchoed = 1  # 0发送txEchoed
         for j in range(8):
```


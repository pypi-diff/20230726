# Comparing `tmp/ait_core-2.4.0.tar.gz` & `tmp/ait_core-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ait_core-2.4.0.tar", max compression
+gzip compressed data, was "ait_core-2.5.0.tar", max compression
```

## Comparing `ait_core-2.4.0.tar` & `ait_core-2.5.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0     1074 2019-09-05 22:56:36.307419 ait_core-2.4.0/LICENSE.txt
--rw-r--r--   0        0        0     9771 2023-01-24 21:55:05.782828 ait_core-2.4.0/README.rst
--rw-r--r--   0        0        0     2087 2022-01-04 19:26:54.297651 ait_core-2.4.0/ait/core/__init__.py
--rw-r--r--   0        0        0    28617 2022-12-14 23:21:45.201945 ait_core-2.4.0/ait/core/api.py
--rw-r--r--   0        0        0      769 2021-10-04 23:43:07.249128 ait_core-2.4.0/ait/core/bin/__init__.py
--rwxr-xr-x   0        0        0     2921 2022-01-04 19:26:54.301179 ait_core-2.4.0/ait/core/bin/ait_bsc.py
--rwxr-xr-x   0        0        0     3217 2022-01-04 19:26:54.302677 ait_core-2.4.0/ait/core/bin/ait_bsc_create_handler.py
--rwxr-xr-x   0        0        0     1773 2022-01-04 19:26:54.304174 ait_core-2.4.0/ait/core/bin/ait_bsc_stop_handler.py
--rwxr-xr-x   0        0        0     1376 2022-01-04 19:26:54.305407 ait_core-2.4.0/ait/core/bin/ait_ccsds_send_example.py
--rwxr-xr-x   0        0        0      699 2022-01-04 19:26:54.307041 ait_core-2.4.0/ait/core/bin/ait_cmd_hist.py
--rwxr-xr-x   0        0        0     4160 2022-01-04 19:26:54.308362 ait_core-2.4.0/ait/core/bin/ait_cmd_send.py
--rwxr-xr-x   0        0        0     6639 2022-01-04 19:26:54.309397 ait_core-2.4.0/ait/core/bin/ait_create_dirs.py
--rwxr-xr-x   0        0        0     2685 2022-01-04 19:26:54.310609 ait_core-2.4.0/ait/core/bin/ait_dict_writer.py
--rw-r--r--   0        0        0     4860 2022-01-04 19:26:54.311688 ait_core-2.4.0/ait/core/bin/ait_limits_find_dn.py
--rw-r--r--   0        0        0     6136 2022-01-04 19:26:54.312758 ait_core-2.4.0/ait/core/bin/ait_mps_seq_convert.py
--rwxr-xr-x   0        0        0     4411 2022-01-04 19:26:54.313601 ait_core-2.4.0/ait/core/bin/ait_pcap.py
--rw-r--r--   0        0        0     3163 2022-01-04 19:26:54.314381 ait_core-2.4.0/ait/core/bin/ait_pcap_segment.py
--rwxr-xr-x   0        0        0     2564 2022-01-04 19:26:54.315298 ait_core-2.4.0/ait/core/bin/ait_seq_decode.py
--rwxr-xr-x   0        0        0     2961 2022-01-04 19:26:54.317780 ait_core-2.4.0/ait/core/bin/ait_seq_encode.py
--rwxr-xr-x   0        0        0     2346 2022-01-04 19:26:54.319863 ait_core-2.4.0/ait/core/bin/ait_seq_print.py
--rwxr-xr-x   0        0        0     4794 2022-01-04 19:26:54.320727 ait_core-2.4.0/ait/core/bin/ait_seq_send.py
--rwxr-xr-x   0        0        0      482 2022-01-04 19:26:54.322331 ait_core-2.4.0/ait/core/bin/ait_server.py
--rwxr-xr-x   0        0        0     2583 2022-01-04 19:26:54.323362 ait_core-2.4.0/ait/core/bin/ait_table_decode.py
--rwxr-xr-x   0        0        0     2353 2022-01-04 19:26:54.324307 ait_core-2.4.0/ait/core/bin/ait_table_encode.py
--rwxr-xr-x   0        0        0     7832 2022-01-04 19:26:54.325362 ait_core-2.4.0/ait/core/bin/ait_tlm_csv.py
--rwxr-xr-x   0        0        0     4091 2022-01-04 19:26:54.326118 ait_core-2.4.0/ait/core/bin/ait_tlm_db_insert.py
--rwxr-xr-x   0        0        0     3176 2022-01-04 19:26:54.327357 ait_core-2.4.0/ait/core/bin/ait_tlm_send.py
--rw-r--r--   0        0        0     2732 2022-01-04 19:26:54.328830 ait_core-2.4.0/ait/core/bin/ait_tlm_simulate.py
--rwxr-xr-x   0        0        0     6555 2022-01-04 19:26:54.330356 ait_core-2.4.0/ait/core/bin/ait_yaml_validate.py
--rw-r--r--   0        0        0    28665 2022-01-04 19:26:54.332049 ait_core-2.4.0/ait/core/bsc.py
--rw-r--r--   0        0        0     3657 2022-01-04 19:26:54.333240 ait_core-2.4.0/ait/core/ccsds.py
--rw-r--r--   0        0        0    14177 2022-10-13 18:10:11.522503 ait_core-2.4.0/ait/core/cfg.py
--rw-r--r--   0        0        0    17765 2022-10-13 18:17:19.236632 ait_core-2.4.0/ait/core/cmd.py
--rw-r--r--   0        0        0     3210 2022-01-04 19:26:54.336724 ait_core-2.4.0/ait/core/coord.py
--rw-r--r--   0        0        0     4950 2020-12-16 17:03:34.395919 ait_core-2.4.0/ait/core/data/cmd_schema.json
--rw-r--r--   0        0        0      732 2019-09-05 22:56:36.324196 ait_core-2.4.0/ait/core/data/evr_schema.json
--rw-r--r--   0        0        0     2163 2019-09-05 22:56:36.324532 ait_core-2.4.0/ait/core/data/limits_schema.json
--rw-r--r--   0        0        0     2638 2022-01-04 19:26:54.337772 ait_core-2.4.0/ait/core/data/table_schema.json
--rw-r--r--   0        0        0     6906 2019-09-05 22:56:36.325199 ait_core-2.4.0/ait/core/data/tlm_schema.json
--rw-r--r--   0        0        0    32471 2022-10-13 18:10:11.522965 ait_core-2.4.0/ait/core/db.py
--rw-r--r--   0        0        0    12158 2022-01-04 19:26:54.339836 ait_core-2.4.0/ait/core/dmc.py
--rw-r--r--   0        0        0    26135 2022-12-21 17:41:53.495338 ait_core-2.4.0/ait/core/dtype.py
--rw-r--r--   0        0        0     8049 2022-01-04 19:26:54.341657 ait_core-2.4.0/ait/core/evr.py
--rw-r--r--   0        0        0     4708 2022-01-04 19:26:54.342628 ait_core-2.4.0/ait/core/gds.py
--rwxr-xr-x   0        0        0    20575 2022-01-04 19:26:54.344426 ait_core-2.4.0/ait/core/geom.py
--rw-r--r--   0        0        0     3725 2022-12-14 23:21:45.202583 ait_core-2.4.0/ait/core/json.py
--rw-r--r--   0        0        0     7286 2022-01-04 19:26:54.347326 ait_core-2.4.0/ait/core/limits.py
--rw-r--r--   0        0        0     9316 2023-02-03 17:20:30.334138 ait_core-2.4.0/ait/core/log.py
--rw-r--r--   0        0        0     3314 2022-01-04 19:26:54.350055 ait_core-2.4.0/ait/core/notify.py
--rw-r--r--   0        0        0    19602 2022-10-13 18:10:11.523208 ait_core-2.4.0/ait/core/pcap.py
--rw-r--r--   0        0        0        0 2023-01-24 22:50:52.581099 ait_core-2.4.0/ait/core/py.typed
--rw-r--r--   0        0        0    23095 2022-01-04 19:26:54.353077 ait_core-2.4.0/ait/core/seq.py
--rw-r--r--   0        0        0      227 2022-10-13 18:10:11.523588 ait_core-2.4.0/ait/core/server/__init__.py
--rw-r--r--   0        0        0     6610 2022-10-13 18:17:19.237065 ait_core-2.4.0/ait/core/server/broker.py
--rw-r--r--   0        0        0     5942 2022-10-13 18:10:11.523934 ait_core-2.4.0/ait/core/server/client.py
--rw-r--r--   0        0        0      356 2022-10-13 18:10:11.524023 ait_core-2.4.0/ait/core/server/config.py
--rwxr-xr-x   0        0        0     1589 2022-01-04 19:26:54.360135 ait_core-2.4.0/ait/core/server/handler.py
--rw-r--r--   0        0        0       82 2022-01-04 19:26:54.361724 ait_core-2.4.0/ait/core/server/handlers/__init__.py
--rw-r--r--   0        0        0     4832 2022-10-13 18:17:19.237705 ait_core-2.4.0/ait/core/server/handlers/ccsds_packet_handler.py
--rw-r--r--   0        0        0     1733 2022-10-13 18:17:19.238252 ait_core-2.4.0/ait/core/server/handlers/packet_handler.py
--rw-r--r--   0        0        0     7759 2022-10-13 18:10:11.524184 ait_core-2.4.0/ait/core/server/plugin.py
--rw-r--r--   0        0        0     1785 2022-03-30 22:19:26.637280 ait_core-2.4.0/ait/core/server/plugins/PacketAccumulator.py
--rw-r--r--   0        0        0      717 2022-03-30 22:19:26.637965 ait_core-2.4.0/ait/core/server/plugins/PacketPadder.py
--rw-r--r--   0        0        0      104 2022-01-04 19:26:54.367862 ait_core-2.4.0/ait/core/server/plugins/__init__.py
--rw-r--r--   0        0        0     7576 2022-10-13 18:10:11.524307 ait_core-2.4.0/ait/core/server/plugins/apid_routing.py
--rw-r--r--   0        0        0     3646 2022-01-04 19:26:54.369049 ait_core-2.4.0/ait/core/server/plugins/data_archive.py
--rw-r--r--   0        0        0     4015 2022-01-04 19:26:54.370926 ait_core-2.4.0/ait/core/server/plugins/limit_monitor.py
--rw-r--r--   0        0        0    45038 2022-10-13 18:10:11.525270 ait_core-2.4.0/ait/core/server/plugins/openmct.py
--rw-r--r--   0        0        0     8885 2022-10-13 18:10:11.525465 ait_core-2.4.0/ait/core/server/process.py
--rw-r--r--   0        0        0    18532 2022-10-13 18:17:19.238632 ait_core-2.4.0/ait/core/server/server.py
--rw-r--r--   0        0        0     4644 2022-01-04 19:26:54.377250 ait_core-2.4.0/ait/core/server/stream.py
--rw-r--r--   0        0        0     1937 2022-01-04 19:26:54.379289 ait_core-2.4.0/ait/core/server/utils.py
--rw-r--r--   0        0        0    18960 2022-10-13 18:10:11.525953 ait_core-2.4.0/ait/core/table.py
--rw-r--r--   0        0        0    35308 2022-12-14 23:21:45.203312 ait_core-2.4.0/ait/core/tlm.py
--rwxr-xr-x   0        0        0    17740 2022-12-14 23:34:20.207415 ait_core-2.4.0/ait/core/util.py
--rw-r--r--   0        0        0    35471 2022-12-14 23:34:20.208130 ait_core-2.4.0/ait/core/val.py
--rw-r--r--   0        0        0       45 2022-01-04 19:26:54.386170 ait_core-2.4.0/ait/data/settings.yaml
--rw-r--r--   0        0        0     3230 2022-12-21 17:41:53.503688 ait_core-2.4.0/pyproject.toml
--rw-r--r--   0        0        0    13077 1970-01-01 00:00:00.000000 ait_core-2.4.0/setup.py
--rw-r--r--   0        0        0    10917 1970-01-01 00:00:00.000000 ait_core-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2019-09-05 22:56:36.307419 ait_core-2.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     9771 2023-01-24 21:55:05.782828 ait_core-2.5.0/README.rst
+-rw-r--r--   0        0        0     2087 2022-01-04 19:26:54.297651 ait_core-2.5.0/ait/core/__init__.py
+-rw-r--r--   0        0        0    28617 2022-12-14 23:21:45.201945 ait_core-2.5.0/ait/core/api.py
+-rw-r--r--   0        0        0      769 2021-10-04 23:43:07.249128 ait_core-2.5.0/ait/core/bin/__init__.py
+-rwxr-xr-x   0        0        0     2921 2022-01-04 19:26:54.301179 ait_core-2.5.0/ait/core/bin/ait_bsc.py
+-rwxr-xr-x   0        0        0     3217 2022-01-04 19:26:54.302677 ait_core-2.5.0/ait/core/bin/ait_bsc_create_handler.py
+-rwxr-xr-x   0        0        0     1773 2022-01-04 19:26:54.304174 ait_core-2.5.0/ait/core/bin/ait_bsc_stop_handler.py
+-rwxr-xr-x   0        0        0     1376 2022-01-04 19:26:54.305407 ait_core-2.5.0/ait/core/bin/ait_ccsds_send_example.py
+-rwxr-xr-x   0        0        0      699 2022-01-04 19:26:54.307041 ait_core-2.5.0/ait/core/bin/ait_cmd_hist.py
+-rwxr-xr-x   0        0        0     4160 2022-01-04 19:26:54.308362 ait_core-2.5.0/ait/core/bin/ait_cmd_send.py
+-rwxr-xr-x   0        0        0     6639 2022-01-04 19:26:54.309397 ait_core-2.5.0/ait/core/bin/ait_create_dirs.py
+-rwxr-xr-x   0        0        0     2685 2022-01-04 19:26:54.310609 ait_core-2.5.0/ait/core/bin/ait_dict_writer.py
+-rw-r--r--   0        0        0     4860 2022-01-04 19:26:54.311688 ait_core-2.5.0/ait/core/bin/ait_limits_find_dn.py
+-rw-r--r--   0        0        0     6136 2022-01-04 19:26:54.312758 ait_core-2.5.0/ait/core/bin/ait_mps_seq_convert.py
+-rwxr-xr-x   0        0        0     4411 2022-01-04 19:26:54.313601 ait_core-2.5.0/ait/core/bin/ait_pcap.py
+-rw-r--r--   0        0        0     3163 2022-01-04 19:26:54.314381 ait_core-2.5.0/ait/core/bin/ait_pcap_segment.py
+-rwxr-xr-x   0        0        0     2564 2022-01-04 19:26:54.315298 ait_core-2.5.0/ait/core/bin/ait_seq_decode.py
+-rwxr-xr-x   0        0        0     2961 2022-01-04 19:26:54.317780 ait_core-2.5.0/ait/core/bin/ait_seq_encode.py
+-rwxr-xr-x   0        0        0     2346 2022-01-04 19:26:54.319863 ait_core-2.5.0/ait/core/bin/ait_seq_print.py
+-rwxr-xr-x   0        0        0     4794 2022-01-04 19:26:54.320727 ait_core-2.5.0/ait/core/bin/ait_seq_send.py
+-rwxr-xr-x   0        0        0      482 2022-01-04 19:26:54.322331 ait_core-2.5.0/ait/core/bin/ait_server.py
+-rwxr-xr-x   0        0        0     2583 2022-01-04 19:26:54.323362 ait_core-2.5.0/ait/core/bin/ait_table_decode.py
+-rwxr-xr-x   0        0        0     2353 2022-01-04 19:26:54.324307 ait_core-2.5.0/ait/core/bin/ait_table_encode.py
+-rwxr-xr-x   0        0        0     7832 2022-01-04 19:26:54.325362 ait_core-2.5.0/ait/core/bin/ait_tlm_csv.py
+-rwxr-xr-x   0        0        0     4091 2022-01-04 19:26:54.326118 ait_core-2.5.0/ait/core/bin/ait_tlm_db_insert.py
+-rwxr-xr-x   0        0        0     3176 2022-01-04 19:26:54.327357 ait_core-2.5.0/ait/core/bin/ait_tlm_send.py
+-rw-r--r--   0        0        0     2732 2022-01-04 19:26:54.328830 ait_core-2.5.0/ait/core/bin/ait_tlm_simulate.py
+-rwxr-xr-x   0        0        0     6555 2022-01-04 19:26:54.330356 ait_core-2.5.0/ait/core/bin/ait_yaml_validate.py
+-rw-r--r--   0        0        0    28665 2022-01-04 19:26:54.332049 ait_core-2.5.0/ait/core/bsc.py
+-rw-r--r--   0        0        0     3657 2022-01-04 19:26:54.333240 ait_core-2.5.0/ait/core/ccsds.py
+-rw-r--r--   0        0        0    14177 2022-10-13 18:10:11.522503 ait_core-2.5.0/ait/core/cfg.py
+-rw-r--r--   0        0        0    17765 2022-10-13 18:17:19.236632 ait_core-2.5.0/ait/core/cmd.py
+-rw-r--r--   0        0        0     3210 2022-01-04 19:26:54.336724 ait_core-2.5.0/ait/core/coord.py
+-rw-r--r--   0        0        0     4950 2020-12-16 17:03:34.395919 ait_core-2.5.0/ait/core/data/cmd_schema.json
+-rw-r--r--   0        0        0      732 2019-09-05 22:56:36.324196 ait_core-2.5.0/ait/core/data/evr_schema.json
+-rw-r--r--   0        0        0     2163 2019-09-05 22:56:36.324532 ait_core-2.5.0/ait/core/data/limits_schema.json
+-rw-r--r--   0        0        0     2638 2022-01-04 19:26:54.337772 ait_core-2.5.0/ait/core/data/table_schema.json
+-rw-r--r--   0        0        0     6906 2019-09-05 22:56:36.325199 ait_core-2.5.0/ait/core/data/tlm_schema.json
+-rw-r--r--   0        0        0    32471 2022-10-13 18:10:11.522965 ait_core-2.5.0/ait/core/db.py
+-rw-r--r--   0        0        0    12158 2022-01-04 19:26:54.339836 ait_core-2.5.0/ait/core/dmc.py
+-rw-r--r--   0        0        0    26135 2022-12-21 17:41:53.495338 ait_core-2.5.0/ait/core/dtype.py
+-rw-r--r--   0        0        0     8049 2022-01-04 19:26:54.341657 ait_core-2.5.0/ait/core/evr.py
+-rw-r--r--   0        0        0     4708 2022-01-04 19:26:54.342628 ait_core-2.5.0/ait/core/gds.py
+-rwxr-xr-x   0        0        0    20575 2022-01-04 19:26:54.344426 ait_core-2.5.0/ait/core/geom.py
+-rw-r--r--   0        0        0     3725 2022-12-14 23:21:45.202583 ait_core-2.5.0/ait/core/json.py
+-rw-r--r--   0        0        0     7286 2022-01-04 19:26:54.347326 ait_core-2.5.0/ait/core/limits.py
+-rw-r--r--   0        0        0     9316 2023-02-03 17:20:30.334138 ait_core-2.5.0/ait/core/log.py
+-rw-r--r--   0        0        0     3314 2022-01-04 19:26:54.350055 ait_core-2.5.0/ait/core/notify.py
+-rw-r--r--   0        0        0    19602 2022-10-13 18:10:11.523208 ait_core-2.5.0/ait/core/pcap.py
+-rw-r--r--   0        0        0        0 2023-01-24 22:50:52.581099 ait_core-2.5.0/ait/core/py.typed
+-rw-r--r--   0        0        0    23095 2022-01-04 19:26:54.353077 ait_core-2.5.0/ait/core/seq.py
+-rw-r--r--   0        0        0      227 2022-10-13 18:10:11.523588 ait_core-2.5.0/ait/core/server/__init__.py
+-rw-r--r--   0        0        0     6610 2022-10-13 18:17:19.237065 ait_core-2.5.0/ait/core/server/broker.py
+-rw-r--r--   0        0        0     5942 2022-10-13 18:10:11.523934 ait_core-2.5.0/ait/core/server/client.py
+-rw-r--r--   0        0        0      356 2022-10-13 18:10:11.524023 ait_core-2.5.0/ait/core/server/config.py
+-rwxr-xr-x   0        0        0     1589 2022-01-04 19:26:54.360135 ait_core-2.5.0/ait/core/server/handler.py
+-rw-r--r--   0        0        0       82 2022-01-04 19:26:54.361724 ait_core-2.5.0/ait/core/server/handlers/__init__.py
+-rw-r--r--   0        0        0     4832 2022-10-13 18:17:19.237705 ait_core-2.5.0/ait/core/server/handlers/ccsds_packet_handler.py
+-rw-r--r--   0        0        0     1733 2022-10-13 18:17:19.238252 ait_core-2.5.0/ait/core/server/handlers/packet_handler.py
+-rw-r--r--   0        0        0     7759 2022-10-13 18:10:11.524184 ait_core-2.5.0/ait/core/server/plugin.py
+-rw-r--r--   0        0        0     1785 2022-03-30 22:19:26.637280 ait_core-2.5.0/ait/core/server/plugins/PacketAccumulator.py
+-rw-r--r--   0        0        0      717 2022-03-30 22:19:26.637965 ait_core-2.5.0/ait/core/server/plugins/PacketPadder.py
+-rw-r--r--   0        0        0      104 2022-01-04 19:26:54.367862 ait_core-2.5.0/ait/core/server/plugins/__init__.py
+-rw-r--r--   0        0        0     7576 2022-10-13 18:10:11.524307 ait_core-2.5.0/ait/core/server/plugins/apid_routing.py
+-rw-r--r--   0        0        0     3646 2022-01-04 19:26:54.369049 ait_core-2.5.0/ait/core/server/plugins/data_archive.py
+-rw-r--r--   0        0        0     4015 2022-01-04 19:26:54.370926 ait_core-2.5.0/ait/core/server/plugins/limit_monitor.py
+-rw-r--r--   0        0        0    45038 2022-10-13 18:10:11.525270 ait_core-2.5.0/ait/core/server/plugins/openmct.py
+-rw-r--r--   0        0        0     8885 2022-10-13 18:10:11.525465 ait_core-2.5.0/ait/core/server/process.py
+-rw-r--r--   0        0        0    18532 2022-10-13 18:17:19.238632 ait_core-2.5.0/ait/core/server/server.py
+-rw-r--r--   0        0        0     4644 2022-01-04 19:26:54.377250 ait_core-2.5.0/ait/core/server/stream.py
+-rw-r--r--   0        0        0     1937 2022-01-04 19:26:54.379289 ait_core-2.5.0/ait/core/server/utils.py
+-rw-r--r--   0        0        0    18960 2022-10-13 18:10:11.525953 ait_core-2.5.0/ait/core/table.py
+-rw-r--r--   0        0        0    35308 2022-12-14 23:21:45.203312 ait_core-2.5.0/ait/core/tlm.py
+-rwxr-xr-x   0        0        0    17740 2022-12-14 23:34:20.207415 ait_core-2.5.0/ait/core/util.py
+-rw-r--r--   0        0        0    35471 2022-12-14 23:34:20.208130 ait_core-2.5.0/ait/core/val.py
+-rw-r--r--   0        0        0       45 2022-01-04 19:26:54.386170 ait_core-2.5.0/ait/data/settings.yaml
+-rw-r--r--   0        0        0     3310 2023-07-26 20:53:39.484939 ait_core-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0    13070 1970-01-01 00:00:00.000000 ait_core-2.5.0/setup.py
+-rw-r--r--   0        0        0    10910 1970-01-01 00:00:00.000000 ait_core-2.5.0/PKG-INFO
```

### Comparing `ait_core-2.4.0/LICENSE.txt` & `ait_core-2.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/README.rst` & `ait_core-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/__init__.py` & `ait_core-2.5.0/ait/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/api.py` & `ait_core-2.5.0/ait/core/api.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/__init__.py` & `ait_core-2.5.0/ait/core/bin/__init__.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_bsc.py` & `ait_core-2.5.0/ait/core/bin/ait_bsc.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_bsc_create_handler.py` & `ait_core-2.5.0/ait/core/bin/ait_bsc_create_handler.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_bsc_stop_handler.py` & `ait_core-2.5.0/ait/core/bin/ait_bsc_stop_handler.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_ccsds_send_example.py` & `ait_core-2.5.0/ait/core/bin/ait_ccsds_send_example.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_cmd_hist.py` & `ait_core-2.5.0/ait/core/bin/ait_cmd_hist.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_cmd_send.py` & `ait_core-2.5.0/ait/core/bin/ait_cmd_send.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_create_dirs.py` & `ait_core-2.5.0/ait/core/bin/ait_create_dirs.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_dict_writer.py` & `ait_core-2.5.0/ait/core/bin/ait_dict_writer.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_limits_find_dn.py` & `ait_core-2.5.0/ait/core/bin/ait_limits_find_dn.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_mps_seq_convert.py` & `ait_core-2.5.0/ait/core/bin/ait_mps_seq_convert.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_pcap.py` & `ait_core-2.5.0/ait/core/bin/ait_pcap.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_pcap_segment.py` & `ait_core-2.5.0/ait/core/bin/ait_pcap_segment.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_seq_decode.py` & `ait_core-2.5.0/ait/core/bin/ait_seq_decode.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_seq_encode.py` & `ait_core-2.5.0/ait/core/bin/ait_seq_encode.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_seq_print.py` & `ait_core-2.5.0/ait/core/bin/ait_seq_print.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_seq_send.py` & `ait_core-2.5.0/ait/core/bin/ait_seq_send.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_table_decode.py` & `ait_core-2.5.0/ait/core/bin/ait_table_decode.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_table_encode.py` & `ait_core-2.5.0/ait/core/bin/ait_table_encode.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_tlm_csv.py` & `ait_core-2.5.0/ait/core/bin/ait_tlm_csv.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_tlm_db_insert.py` & `ait_core-2.5.0/ait/core/bin/ait_tlm_db_insert.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_tlm_send.py` & `ait_core-2.5.0/ait/core/bin/ait_tlm_send.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_tlm_simulate.py` & `ait_core-2.5.0/ait/core/bin/ait_tlm_simulate.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bin/ait_yaml_validate.py` & `ait_core-2.5.0/ait/core/bin/ait_yaml_validate.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/bsc.py` & `ait_core-2.5.0/ait/core/bsc.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/ccsds.py` & `ait_core-2.5.0/ait/core/ccsds.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/cfg.py` & `ait_core-2.5.0/ait/core/cfg.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/cmd.py` & `ait_core-2.5.0/ait/core/cmd.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/coord.py` & `ait_core-2.5.0/ait/core/coord.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/data/cmd_schema.json` & `ait_core-2.5.0/ait/core/data/cmd_schema.json`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/data/evr_schema.json` & `ait_core-2.5.0/ait/core/data/evr_schema.json`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/data/limits_schema.json` & `ait_core-2.5.0/ait/core/data/limits_schema.json`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/data/table_schema.json` & `ait_core-2.5.0/ait/core/data/table_schema.json`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/data/tlm_schema.json` & `ait_core-2.5.0/ait/core/data/tlm_schema.json`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/db.py` & `ait_core-2.5.0/ait/core/db.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/dmc.py` & `ait_core-2.5.0/ait/core/dmc.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/dtype.py` & `ait_core-2.5.0/ait/core/dtype.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/evr.py` & `ait_core-2.5.0/ait/core/evr.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/gds.py` & `ait_core-2.5.0/ait/core/gds.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/geom.py` & `ait_core-2.5.0/ait/core/geom.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/json.py` & `ait_core-2.5.0/ait/core/json.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/limits.py` & `ait_core-2.5.0/ait/core/limits.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/log.py` & `ait_core-2.5.0/ait/core/log.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/notify.py` & `ait_core-2.5.0/ait/core/notify.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/pcap.py` & `ait_core-2.5.0/ait/core/pcap.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/seq.py` & `ait_core-2.5.0/ait/core/seq.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/server/broker.py` & `ait_core-2.5.0/ait/core/server/broker.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/server/client.py` & `ait_core-2.5.0/ait/core/server/client.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/server/handler.py` & `ait_core-2.5.0/ait/core/server/handler.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/server/handlers/ccsds_packet_handler.py` & `ait_core-2.5.0/ait/core/server/handlers/ccsds_packet_handler.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/server/handlers/packet_handler.py` & `ait_core-2.5.0/ait/core/server/handlers/packet_handler.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/server/plugin.py` & `ait_core-2.5.0/ait/core/server/plugin.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/server/plugins/PacketAccumulator.py` & `ait_core-2.5.0/ait/core/server/plugins/PacketAccumulator.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/server/plugins/PacketPadder.py` & `ait_core-2.5.0/ait/core/server/plugins/PacketPadder.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/server/plugins/apid_routing.py` & `ait_core-2.5.0/ait/core/server/plugins/apid_routing.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/server/plugins/data_archive.py` & `ait_core-2.5.0/ait/core/server/plugins/data_archive.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/server/plugins/limit_monitor.py` & `ait_core-2.5.0/ait/core/server/plugins/limit_monitor.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/server/plugins/openmct.py` & `ait_core-2.5.0/ait/core/server/plugins/openmct.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/server/process.py` & `ait_core-2.5.0/ait/core/server/process.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/server/server.py` & `ait_core-2.5.0/ait/core/server/server.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/server/stream.py` & `ait_core-2.5.0/ait/core/server/stream.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/server/utils.py` & `ait_core-2.5.0/ait/core/server/utils.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/table.py` & `ait_core-2.5.0/ait/core/table.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/tlm.py` & `ait_core-2.5.0/ait/core/tlm.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/util.py` & `ait_core-2.5.0/ait/core/util.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/ait/core/val.py` & `ait_core-2.5.0/ait/core/val.py`

 * *Files identical despite different names*

### Comparing `ait_core-2.4.0/pyproject.toml` & `ait_core-2.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name         = 'ait-core'
-version      = '2.4.0'
+version      = '2.5.0'
 description  = "NASA JPL's Ground Data System toolkit for Instrument and CubeSat Missions"
 license = 'MIT'
 readme = 'README.rst'
 homepage = 'https://github.com/NASA-AMMOS/AIT-Core'
 repository = 'https://github.com/NASA-AMMOS/AIT-Core'
 documentation = 'https://ait-core.readthedocs.io/en/latest'
 authors       = ['AMMOS Instrument Toolkit Development Team <ait-pmc@googlegroups.com>']
@@ -21,15 +21,15 @@
     "ait/core/data/*.json"
 ]
 
 [tool.poetry.dependencies]
 python           = '>= 3.7 < 3.11'
 bottle           = '0.12.23'
 jsonschema       = '3.0.2'
-pyyaml           = '^5.1.2'
+pyyaml           = '5.3.1'  # Temporarily pinning this to 5.3.1 because pyyaml and Cython 3 don't get along
 requests         = '>= 2.22.0'
 greenlet         = '1.1.3'
 gevent           = '*'
 gevent-websocket = '0.10.1'
 pyzmq            = '24.0.0'
 gipc             = "^1.1.0"
 setproctitle = "^1.2.3"
```

### Comparing `ait_core-2.4.0/setup.py` & `ait_core-2.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 install_requires = \
 ['bottle==0.12.23',
  'gevent',
  'gevent-websocket==0.10.1',
  'gipc>=1.1.0,<2.0.0',
  'greenlet==1.1.3',
  'jsonschema==3.0.2',
- 'pyyaml>=5.1.2,<6.0.0',
+ 'pyyaml==5.3.1',
  'pyzmq==24.0.0',
  'requests>=2.22.0',
  'setproctitle>=1.2.3,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['ait-bsc = ait.core.bin.ait_bsc:main',
                      'ait-bsc-create-handler = '
@@ -54,15 +54,15 @@
                      'ait-tlm-send = ait.core.bin.ait_tlm_send:main',
                      'ait-tlm-simulate = ait.core.bin.ait_tlm_simulate:main',
                      'ait-yaml-validate = ait.core.bin.ait_yaml_validate:main',
                      'build_sphinx = poetry_cli.build_sphinx:main']}
 
 setup_kwargs = {
     'name': 'ait-core',
-    'version': '2.4.0',
+    'version': '2.5.0',
     'description': "NASA JPL's Ground Data System toolkit for Instrument and CubeSat Missions",
     'long_description': '\n.. image:: https://github.com/NASA-AMMOS/AIT-Core/actions/workflows/full_build.yaml/badge.svg?branch=master\n   :target: https://github.com/NASA-AMMOS/AIT-Core/actions\n   :alt: Build and Lint Status\n\n.. image:: https://readthedocs.org/projects/ait-core/badge/?version=latest\n    :target: https://ait-core.readthedocs.io/en/latest/?badge=latest\n    :alt: Documentation Status\n\nThe AMMOS Instrument Toolkit (Formerly the Bespoke Links to Instruments\nfor Surface and Space (BLISS)) is a Python-based software suite\ndeveloped to handle Ground Data System (GDS), Electronic Ground Support\nEquipment (EGSE), commanding, telemetry uplink/downlink, and sequencing\nfor instrument and CubeSat Missions. It is a generalization and expansion\nof tools developed for a number of ISS\nmissions.\n\nGetting Started\n===============\n\nYou can read through the `Installation and Configuration\nPage <http://ait-core.readthedocs.io/en/latest/installation.html>`__ for\ninstruction on how to install AIT Core.\n\nYou can read through the `New Project Setup\nPage <http://ait-core.readthedocs.io/en/latest/project_setup.html>`__\nfor instructions on how to use AIT on your next project.\n\nJoin the Community\n==================\n\nThe project\'s `User and Developer Mailing List <https://groups.google.com/forum/#!forum/ait-dev>`__ is the best way to communicate with the team, ask questions, brainstorm plans for future changes, and help contribute to the project.\n\nThis project exists thanks to the dedicated users, contributors, committers, and project management committee members. If you\'d like to learn more about how the project is organized and how to become a part of the team please check out the `Project Structure and Governance <https://github.com/NASA-AMMOS/AIT-Core/wiki/Project-Structure-and-Governance>`__ documentation.\n\nContributing\n============\n\nThank you for your interest in contributing to AIT! We welcome contributions from people of all backgrounds and disciplines. While much of the focus of our project is software, we believe that many of the most critical contributions come in the form of documentation improvements, asset generation, user testing and feedback, and community involvement. So if you\'re interested and want to help out please don\'t hesitate! Send us an email on the public mailing list below, introduce yourself, and join the community.\n\nCommunication\n-------------\nAll project communication happens via mailing lists. Discussions related to development should happen on the public `Developer and User Mailing List <https://groups.google.com/forum/#!forum/ait-dev>`__. If you\'re new to the community make sure to introduce yourself as well!\n\nDev Installation\n----------------\nAs always, we encourage you to install AIT into a virtual environment of your choosing when you set up your development environment. AIT uses `poetry` for package management. Before setting up your development environment you will need the following installed and ready to use:\n\n- A virtual environment "manager" of your choosing with a configured and activated virtual environment. Since AIT uses `poetry` you can consider leveraging its `environment management <https://python-poetry.org/docs/managing-environments/>`__ functionality as well.\n    - Using `poetry shell` is also very convenient for development testing and simplifying environment management. You should make sure to install the package into the shell to get access to the development dependencies as well. It\'s recommended that you use `poetry shell` when running the tox builds because other virtual environment managers will often prevent tox from accessing `pyenv`-installed Python versions.\n- `pyenv <https://github.com/pyenv/pyenv>`__ so you can easily install different Python versions\n- `poetry <https://python-poetry.org/docs/#installation>`__ installed either to your specific virtual environment or system-wide, whichever you prefer.\n\nInstall the package in "editable" mode with all the development dependencies by running the following::\n\n    poetry install\n\nAs with a normal installation you will need to point `AIT_CONFIG` at the primary configuration file. You should consider saving this in your shell RC file or your virtual environment configuration files so you don\'t have to reset with every new shell::\n\n    export AIT_CONFIG=/path/to/ait-core/config/config.yaml\n\nYou should configure `pre-commit` by running the following. This will install our pre-commit and pre-push hooks::\n\n    pre-commit install && pre-commit install -t pre-push\n\nFinally, you should install the different Python versions that the project supports so they\'re accessible to `tox`. Using `pyenv` is the easiest way to accomplish this::\n\n    cat .python-version | xargs -I{} pyenv install --skip-existing {}\n\nDev Tools\n---------\n\nTox\n~~~\nUse `tox` to run a thorough build of the toolkit that checks test execution across different Python versions, verifies the docs build, runs the linting pipeline, and checks that the repo packages cleanly. Make sure you run `tox` in Poetry\'s `shell` without another virtual environment active to avoid problems with `tox` finding different python versions for the tests. You can run all of the development tools with::\n\n    tox\n\nYou can see the available `tox` test environments by passing `-l` and execute a specific one by passing its name to `-e`. Run `tox -h` for more info.\n\nTests\n~~~~~\n\nUse `pytest` to manually run the test suite::\n\n    pytest\n\nOr via `tox` for a specific python version::\n\n    tox -e py310\n\n\nCode Checks\n~~~~~~~~~~~\nWe run ``black``, ``flake8``, ``mypy``, and a few other minor checkers on the code base. Our linting and code check pipeline is run whenever you commit or push. If you\'d like to run it manually you can do so with the following::\n\n    pre_commit run --color=always {posargs:--all}\n\nIndividual calls to the tools are configured in ``.pre-commit-config.yaml``. If you\'d like to run a specific tool on its own you can see how we call them there.\n\nYou can run all the linting tools with tox as well::\n\n    tox -e lint\n\n\nDocumentation\n~~~~~~~~~~~~~\n\nAIT uses Sphinx to build its documentation. You can build the documentation with::\n\n    poetry run build_sphinx\n\nTo view the documentation, open ``doc/build/html/index.html`` in a web browser. If you just want to check that the docs build is working you can use tox::\n\n    tox -e docs\n\nIf you need to update the auto-generated documentation you can run the following command to rebuild all of the package documentation::\n\n    sphinx-apidoc --separate --force --no-toc -o doc/source ait --implicit-namespaces\n\nPlease make sure to update the docs if changes in a ticket result in the documentation being out of date.\n\n\nProject Workflow\n----------------\nIssue Tracking\n~~~~~~~~~~~~~~\nAll changes need to be made against one or more tickets for tracking purposes. AIT uses GitHub Issues along with Zenhub to track issue in the project. All tickets should have (outside of rare edge-cases):\n\n- A concise title\n- An in-depth description of the problem / request. If reporting a bug, the description should include information on how to reproduce the bug. Also include the version of the code where you’re seeing the bug.\n\nIf you’re going to begin work on a ticket make sure to progress the ticket through the various Pipeline steps as appropriate as well as assigning yourself as an Assignee. If you lack sufficient permissions to do so you can post on the ticket asking for the above to be done for you.\n\nCommit Messages\n~~~~~~~~~~~~~~~\nAIT projects take a fairly standard approach to commit message formatting. You can checkout Tim Pope\'s blog for a good starting point to figuring out how to format your commit messages. All commit messages should reference a ticket in their title / summary line::\n\n    Issue #248 - Show an example commit message title\n\nThis makes sure that tickets are updated on GitHub with references to commits that are related to them.\n\nCommit should always be atomic. Keep solutions isolated whenever possible. Filler commits such as "clean up white space" or "fix typo" should be rebased out before making a pull request. Please ensure your commit history is clean and meaningful!\n\nCode Formatting and Style\n~~~~~~~~~~~~~~~~~~~~~~~~~\nAIT makes a best-effort attempt at sticking with PEP-8 conventions. This is enforced automatically by ``black`` and checked by ``flake8``. You should run the ``pre-commit`` linting pipeline on any changes you make.\n\nTesting\n~~~~~~~\nWe do our best to make sure that all of our changes are tested. If you\'re fixing a bug you should always have an accompanying unit test to ensure we don\'t regress!\n\nCheck the Developer Tips section below for information on running each repository\'s test suite.\n\nPull Requests and Feature Branches\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\nAll changes should be isolated to a feature branch that links to a ticket. The standard across AIT projects is to use issue-### for branch names where ### is the issue number found on GitHub.\n\nThe title of a pull request should include a reference to the ticket being fixed as mentioned for commit messages. The description of a pull request should provide an in-depth explanation of the changes present. Note, if you wrote good commit messages this step should be easy!\n\nAny tickets that are resolved by the pull request should be referenced with GitHub\'s syntax for closing out tickets. Assuming the above ticket we would have the following in a pull request description:\n\nChanges are required to be reviewed by at least one member of the AIT PMC/Committers groups, tests must pass, and the branch must be up to date with master before changes will be merged. If changes are made as part of code review please ensure your commit history is cleaned up.\n\nResolve #248\n--------------\n',
     'author': 'AMMOS Instrument Toolkit Development Team',
     'author_email': 'ait-pmc@googlegroups.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/NASA-AMMOS/AIT-Core',
```

### Comparing `ait_core-2.4.0/PKG-INFO` & `ait_core-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ait-core
-Version: 2.4.0
+Version: 2.5.0
 Summary: NASA JPL's Ground Data System toolkit for Instrument and CubeSat Missions
 Home-page: https://github.com/NASA-AMMOS/AIT-Core
 License: MIT
 Author: AMMOS Instrument Toolkit Development Team
 Author-email: ait-pmc@googlegroups.com
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: bottle (==0.12.23)
 Requires-Dist: gevent
 Requires-Dist: gevent-websocket (==0.10.1)
 Requires-Dist: gipc (>=1.1.0,<2.0.0)
 Requires-Dist: greenlet (==1.1.3)
 Requires-Dist: jsonschema (==3.0.2)
-Requires-Dist: pyyaml (>=5.1.2,<6.0.0)
+Requires-Dist: pyyaml (==5.3.1)
 Requires-Dist: pyzmq (==24.0.0)
 Requires-Dist: requests (>=2.22.0)
 Requires-Dist: setproctitle (>=1.2.3,<2.0.0)
 Project-URL: Documentation, https://ait-core.readthedocs.io/en/latest
 Project-URL: Repository, https://github.com/NASA-AMMOS/AIT-Core
 Description-Content-Type: text/x-rst
```


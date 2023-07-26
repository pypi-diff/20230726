# Comparing `tmp/goplus-0.1.4.tar.gz` & `tmp/goplus-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goplus-0.1.4.tar", last modified: Thu Jul  6 10:46:47 2023, max compression
+gzip compressed data, was "goplus-0.1.5.tar", last modified: Wed Jul 26 10:39:12 2023, max compression
```

## Comparing `goplus-0.1.4.tar` & `goplus-0.1.5.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:46:47.936354 goplus-0.1.4/
--rw-r--r--   0 cong       (501) staff       (20)    11357 2023-04-27 08:29:42.000000 goplus-0.1.4/LICENSE
--rw-r--r--   0 cong       (501) staff       (20)      837 2023-07-06 10:46:47.936240 goplus-0.1.4/PKG-INFO
--rw-r--r--   0 cong       (501) staff       (20)      359 2023-07-06 10:35:12.000000 goplus-0.1.4/README.md
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:46:47.925484 goplus-0.1.4/goplus/
--rw-r--r--   0 cong       (501) staff       (20)      590 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)      654 2023-07-06 10:45:38.000000 goplus-0.1.4/goplus/__version__.py
--rw-r--r--   0 cong       (501) staff       (20)     1135 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/address.py
--rw-r--r--   0 cong       (501) staff       (20)     2227 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/approve.py
--rw-r--r--   0 cong       (501) staff       (20)     1481 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/auth.py
--rw-r--r--   0 cong       (501) staff       (20)      840 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/base.py
--rw-r--r--   0 cong       (501) staff       (20)      864 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/chain.py
--rw-r--r--   0 cong       (501) staff       (20)      982 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/dapp.py
--rw-r--r--   0 cong       (501) staff       (20)     1302 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/decode.py
--rw-r--r--   0 cong       (501) staff       (20)     1096 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/errocode.py
--rw-r--r--   0 cong       (501) staff       (20)     1092 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/nft.py
--rw-r--r--   0 cong       (501) staff       (20)     1002 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/phishing_site.py
--rw-r--r--   0 cong       (501) staff       (20)     1144 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/rug_pull.py
--rw-r--r--   0 cong       (501) staff       (20)     1453 2023-05-30 08:01:30.000000 goplus-0.1.4/goplus/token.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:46:47.925948 goplus-0.1.4/goplus.egg-info/
--rw-r--r--   0 cong       (501) staff       (20)      837 2023-07-06 10:46:47.000000 goplus-0.1.4/goplus.egg-info/PKG-INFO
--rw-r--r--   0 cong       (501) staff       (20)     4153 2023-07-06 10:46:47.000000 goplus-0.1.4/goplus.egg-info/SOURCES.txt
--rw-r--r--   0 cong       (501) staff       (20)        1 2023-07-06 10:46:47.000000 goplus-0.1.4/goplus.egg-info/dependency_links.txt
--rw-r--r--   0 cong       (501) staff       (20)       67 2023-07-06 10:46:47.000000 goplus-0.1.4/goplus.egg-info/requires.txt
--rw-r--r--   0 cong       (501) staff       (20)       22 2023-07-06 10:46:47.000000 goplus-0.1.4/goplus.egg-info/top_level.txt
--rw-r--r--   0 cong       (501) staff       (20)       38 2023-07-06 10:46:47.936387 goplus-0.1.4/setup.cfg
--rw-r--r--   0 cong       (501) staff       (20)     3592 2023-05-10 02:53:37.000000 goplus-0.1.4/setup.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:46:47.926786 goplus-0.1.4/swagger_client/
--rw-r--r--   0 cong       (501) staff       (20)     6427 2023-07-06 10:45:21.000000 goplus-0.1.4/swagger_client/__init__.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:46:47.928649 goplus-0.1.4/swagger_client/api/
--rw-r--r--   0 cong       (501) staff       (20)      761 2023-05-30 06:06:21.000000 goplus-0.1.4/swagger_client/api/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)    10919 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api/approve_controller_v_1_api.py
--rw-r--r--   0 cong       (501) staff       (20)    15210 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api/approve_controller_v_2_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4981 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api/contract_abi_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4471 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api/dapp_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     5548 2023-06-21 02:21:31.000000 goplus-0.1.4/swagger_client/api/defi_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     5833 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api/nft_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4282 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api/token_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)    10150 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api/token_controller_v_1_api.py
--rw-r--r--   0 cong       (501) staff       (20)     4726 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api/website_controller_api.py
--rw-r--r--   0 cong       (501) staff       (20)    25084 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/api_client.py
--rw-r--r--   0 cong       (501) staff       (20)     8010 2023-05-30 08:59:54.000000 goplus-0.1.4/swagger_client/configuration.py
-drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-06 10:46:47.936076 goplus-0.1.4/swagger_client/models/
--rw-r--r--   0 cong       (501) staff       (20)     5601 2023-07-06 10:45:21.000000 goplus-0.1.4/swagger_client/models/__init__.py
--rw-r--r--   0 cong       (501) staff       (20)     7936 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/abi_address_info.py
--rw-r--r--   0 cong       (501) staff       (20)     5536 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/abi_param_info.py
--rw-r--r--   0 cong       (501) staff       (20)    10427 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/approve_address_info.py
--rw-r--r--   0 cong       (501) staff       (20)     7889 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/approve_erc1155_result.py
--rw-r--r--   0 cong       (501) staff       (20)    10642 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/approve_nft1155_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)    10461 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/approve_nft_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     9647 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/approve_result.py
--rw-r--r--   0 cong       (501) staff       (20)    11415 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/approve_token_out_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     8748 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/approve_token_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4933 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/audit_info.py
--rw-r--r--   0 cong       (501) staff       (20)    15392 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/contract_approve_response.py
--rw-r--r--   0 cong       (501) staff       (20)    11564 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/contracts.py
--rw-r--r--   0 cong       (501) staff       (20)     4468 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/contracts_security.py
--rw-r--r--   0 cong       (501) staff       (20)     9038 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/dapp_contract_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5447 2023-07-06 10:35:12.000000 goplus-0.1.4/swagger_client/models/get_access_token_request.py
--rw-r--r--   0 cong       (501) staff       (20)     4144 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/get_access_token_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4619 2023-06-21 02:21:31.000000 goplus-0.1.4/swagger_client/models/get_defi_info_response.py
--rw-r--r--   0 cong       (501) staff       (20)    12280 2023-06-21 02:21:31.000000 goplus-0.1.4/swagger_client/models/get_defi_info_response_result.py
--rw-r--r--   0 cong       (501) staff       (20)     5765 2023-06-21 02:21:31.000000 goplus-0.1.4/swagger_client/models/get_defi_info_response_result_owner.py
--rw-r--r--   0 cong       (501) staff       (20)     2684 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     2704 2023-06-21 02:21:31.000000 goplus-0.1.4/swagger_client/models/map_string_string.py
--rw-r--r--   0 cong       (501) staff       (20)     8209 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/parse_abi_data_request.py
--rw-r--r--   0 cong       (501) staff       (20)    10371 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/parse_abi_data_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4828 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_address_contract.py
--rw-r--r--   0 cong       (501) staff       (20)    23058 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_address_contract_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4917 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_contract_approve_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5012 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_dapp_contract_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4898 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_get_access_token_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4733 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info.py
--rw-r--r--   0 cong       (501) staff       (20)    42552 2023-06-02 06:08:47.000000 goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result.py
--rw-r--r--   0 cong       (501) staff       (20)     7031 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py
--rw-r--r--   0 cong       (501) staff       (20)     7079 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py
--rw-r--r--   0 cong       (501) staff       (20)     7605 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py
--rw-r--r--   0 cong       (501) staff       (20)     6999 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py
--rw-r--r--   0 cong       (501) staff       (20)     7175 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py
--rw-r--r--   0 cong       (501) staff       (20)     4767 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     5132 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5056 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_list_approve_nft_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     5151 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4960 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_list_get_chains_list.py
--rw-r--r--   0 cong       (501) staff       (20)     4008 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_list_get_chains_list_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4828 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_list_json_object.py
--rw-r--r--   0 cong       (501) staff       (20)     4838 2023-06-21 02:21:31.000000 goplus-0.1.4/swagger_client/models/response_wrapper_map_string_string.py
--rw-r--r--   0 cong       (501) staff       (20)     4860 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_parse_abi_data_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4771 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_phishing_site.py
--rw-r--r--   0 cong       (501) staff       (20)     4798 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_phishing_site_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4917 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_ta_token_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)     4899 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_token_security.py
--rw-r--r--   0 cong       (501) staff       (20)     4905 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_token_security_dex.py
--rw-r--r--   0 cong       (501) staff       (20)     5269 2023-07-06 10:45:21.000000 goplus-0.1.4/swagger_client/models/response_wrapper_token_security_locked_detail.py
--rw-r--r--   0 cong       (501) staff       (20)    10070 2023-07-06 10:45:21.000000 goplus-0.1.4/swagger_client/models/response_wrapper_token_security_lp_holders.py
--rw-r--r--   0 cong       (501) staff       (20)    70422 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapper_token_security_result.py
--rw-r--r--   0 cong       (501) staff       (20)     4670 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/response_wrapperobject.py
--rw-r--r--   0 cong       (501) staff       (20)     3194 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/models/ta_token_security_response.py
--rw-r--r--   0 cong       (501) staff       (20)    13036 2023-05-30 06:06:46.000000 goplus-0.1.4/swagger_client/rest.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-26 10:39:12.078513 goplus-0.1.5/
+-rw-r--r--   0 cong       (501) staff       (20)    11357 2023-04-27 08:29:42.000000 goplus-0.1.5/LICENSE
+-rw-r--r--   0 cong       (501) staff       (20)      837 2023-07-26 10:39:12.078374 goplus-0.1.5/PKG-INFO
+-rw-r--r--   0 cong       (501) staff       (20)      359 2023-07-06 10:35:12.000000 goplus-0.1.5/README.md
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-26 10:39:12.061404 goplus-0.1.5/goplus/
+-rw-r--r--   0 cong       (501) staff       (20)      590 2023-05-30 08:01:30.000000 goplus-0.1.5/goplus/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)      654 2023-07-26 10:36:23.000000 goplus-0.1.5/goplus/__version__.py
+-rw-r--r--   0 cong       (501) staff       (20)     1135 2023-05-30 08:01:30.000000 goplus-0.1.5/goplus/address.py
+-rw-r--r--   0 cong       (501) staff       (20)     2227 2023-05-30 08:01:30.000000 goplus-0.1.5/goplus/approve.py
+-rw-r--r--   0 cong       (501) staff       (20)     1481 2023-05-30 08:01:30.000000 goplus-0.1.5/goplus/auth.py
+-rw-r--r--   0 cong       (501) staff       (20)      840 2023-05-30 08:01:30.000000 goplus-0.1.5/goplus/base.py
+-rw-r--r--   0 cong       (501) staff       (20)      864 2023-05-30 08:01:30.000000 goplus-0.1.5/goplus/chain.py
+-rw-r--r--   0 cong       (501) staff       (20)      982 2023-05-30 08:01:30.000000 goplus-0.1.5/goplus/dapp.py
+-rw-r--r--   0 cong       (501) staff       (20)     1302 2023-05-30 08:01:30.000000 goplus-0.1.5/goplus/decode.py
+-rw-r--r--   0 cong       (501) staff       (20)     1096 2023-05-30 08:01:30.000000 goplus-0.1.5/goplus/errocode.py
+-rw-r--r--   0 cong       (501) staff       (20)     1092 2023-05-30 08:01:30.000000 goplus-0.1.5/goplus/nft.py
+-rw-r--r--   0 cong       (501) staff       (20)     1002 2023-05-30 08:01:30.000000 goplus-0.1.5/goplus/phishing_site.py
+-rw-r--r--   0 cong       (501) staff       (20)     1144 2023-05-30 08:01:30.000000 goplus-0.1.5/goplus/rug_pull.py
+-rw-r--r--   0 cong       (501) staff       (20)     1453 2023-05-30 08:01:30.000000 goplus-0.1.5/goplus/token.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-26 10:39:12.062048 goplus-0.1.5/goplus.egg-info/
+-rw-r--r--   0 cong       (501) staff       (20)      837 2023-07-26 10:39:12.000000 goplus-0.1.5/goplus.egg-info/PKG-INFO
+-rw-r--r--   0 cong       (501) staff       (20)     4153 2023-07-26 10:39:12.000000 goplus-0.1.5/goplus.egg-info/SOURCES.txt
+-rw-r--r--   0 cong       (501) staff       (20)        1 2023-07-26 10:39:12.000000 goplus-0.1.5/goplus.egg-info/dependency_links.txt
+-rw-r--r--   0 cong       (501) staff       (20)       67 2023-07-26 10:39:12.000000 goplus-0.1.5/goplus.egg-info/requires.txt
+-rw-r--r--   0 cong       (501) staff       (20)       22 2023-07-26 10:39:12.000000 goplus-0.1.5/goplus.egg-info/top_level.txt
+-rw-r--r--   0 cong       (501) staff       (20)       38 2023-07-26 10:39:12.078550 goplus-0.1.5/setup.cfg
+-rw-r--r--   0 cong       (501) staff       (20)     3592 2023-05-10 02:53:37.000000 goplus-0.1.5/setup.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-26 10:39:12.063281 goplus-0.1.5/swagger_client/
+-rw-r--r--   0 cong       (501) staff       (20)     6427 2023-07-06 10:45:21.000000 goplus-0.1.5/swagger_client/__init__.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-26 10:39:12.068627 goplus-0.1.5/swagger_client/api/
+-rw-r--r--   0 cong       (501) staff       (20)      761 2023-05-30 06:06:21.000000 goplus-0.1.5/swagger_client/api/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)    10907 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/api/approve_controller_v_1_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    15204 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/api/approve_controller_v_2_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4979 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/api/contract_abi_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4469 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/api/dapp_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     5546 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/api/defi_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     5831 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/api/nft_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4282 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/api/token_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    10138 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/api/token_controller_v_1_api.py
+-rw-r--r--   0 cong       (501) staff       (20)     4724 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/api/website_controller_api.py
+-rw-r--r--   0 cong       (501) staff       (20)    25084 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/api_client.py
+-rw-r--r--   0 cong       (501) staff       (20)     8009 2023-07-26 10:36:07.000000 goplus-0.1.5/swagger_client/configuration.py
+drwxr-xr-x   0 cong       (501) staff       (20)        0 2023-07-26 10:39:12.078090 goplus-0.1.5/swagger_client/models/
+-rw-r--r--   0 cong       (501) staff       (20)     5601 2023-07-06 10:45:21.000000 goplus-0.1.5/swagger_client/models/__init__.py
+-rw-r--r--   0 cong       (501) staff       (20)     7936 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/abi_address_info.py
+-rw-r--r--   0 cong       (501) staff       (20)     5536 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/abi_param_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    10427 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/approve_address_info.py
+-rw-r--r--   0 cong       (501) staff       (20)     7889 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/approve_erc1155_result.py
+-rw-r--r--   0 cong       (501) staff       (20)    10642 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/approve_nft1155_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    10461 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/approve_nft_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     9647 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/approve_result.py
+-rw-r--r--   0 cong       (501) staff       (20)    11415 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/approve_token_out_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     8748 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/approve_token_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4933 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/audit_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    15388 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/contract_approve_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    11564 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/contracts.py
+-rw-r--r--   0 cong       (501) staff       (20)     4468 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/contracts_security.py
+-rw-r--r--   0 cong       (501) staff       (20)     9038 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/dapp_contract_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5447 2023-07-06 10:35:12.000000 goplus-0.1.5/swagger_client/models/get_access_token_request.py
+-rw-r--r--   0 cong       (501) staff       (20)     4144 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/get_access_token_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4617 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/get_defi_info_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    12268 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/get_defi_info_response_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     5765 2023-06-21 02:21:31.000000 goplus-0.1.5/swagger_client/models/get_defi_info_response_result_owner.py
+-rw-r--r--   0 cong       (501) staff       (20)     2684 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     2704 2023-06-21 02:21:31.000000 goplus-0.1.5/swagger_client/models/map_string_string.py
+-rw-r--r--   0 cong       (501) staff       (20)     8209 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/parse_abi_data_request.py
+-rw-r--r--   0 cong       (501) staff       (20)    10371 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/parse_abi_data_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4826 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_address_contract.py
+-rw-r--r--   0 cong       (501) staff       (20)    23056 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_address_contract_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4915 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_contract_approve_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5010 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_dapp_contract_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4896 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_get_access_token_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4731 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_get_nft_info.py
+-rw-r--r--   0 cong       (501) staff       (20)    42512 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_get_nft_info_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     7031 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py
+-rw-r--r--   0 cong       (501) staff       (20)     7079 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py
+-rw-r--r--   0 cong       (501) staff       (20)     7605 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py
+-rw-r--r--   0 cong       (501) staff       (20)     6999 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py
+-rw-r--r--   0 cong       (501) staff       (20)     7175 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py
+-rw-r--r--   0 cong       (501) staff       (20)     4765 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     5130 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5054 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_list_approve_nft_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     5149 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4958 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_list_get_chains_list.py
+-rw-r--r--   0 cong       (501) staff       (20)     4008 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/response_wrapper_list_get_chains_list_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4826 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_list_json_object.py
+-rw-r--r--   0 cong       (501) staff       (20)     4836 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_map_string_string.py
+-rw-r--r--   0 cong       (501) staff       (20)     4858 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_parse_abi_data_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4769 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_phishing_site.py
+-rw-r--r--   0 cong       (501) staff       (20)     4798 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/response_wrapper_phishing_site_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4915 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_ta_token_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)     4897 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_token_security.py
+-rw-r--r--   0 cong       (501) staff       (20)     4905 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/response_wrapper_token_security_dex.py
+-rw-r--r--   0 cong       (501) staff       (20)     5269 2023-07-06 10:45:21.000000 goplus-0.1.5/swagger_client/models/response_wrapper_token_security_locked_detail.py
+-rw-r--r--   0 cong       (501) staff       (20)    10066 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_token_security_lp_holders.py
+-rw-r--r--   0 cong       (501) staff       (20)    70400 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapper_token_security_result.py
+-rw-r--r--   0 cong       (501) staff       (20)     4668 2023-07-21 07:25:36.000000 goplus-0.1.5/swagger_client/models/response_wrapperobject.py
+-rw-r--r--   0 cong       (501) staff       (20)     3194 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/models/ta_token_security_response.py
+-rw-r--r--   0 cong       (501) staff       (20)    13036 2023-05-30 06:06:46.000000 goplus-0.1.5/swagger_client/rest.py
```

### Comparing `goplus-0.1.4/LICENSE` & `goplus-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/PKG-INFO` & `goplus-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goplus
-Version: 0.1.4
+Version: 0.1.5
 Summary: GoPlus SDK
 Home-page: https://github.com/GoPlusSecurity/goplus-sdk-python
 Author: GoPlus
 Author-email: service@gopluslabs.io
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `goplus-0.1.4/goplus/__init__.py` & `goplus-0.1.5/goplus/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/goplus/__version__.py` & `goplus-0.1.5/goplus/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-VERSION = (0, 1, 4)
+VERSION = (0, 1, 5)
 
 __version__ = ".".join(map(str, VERSION))
```

### Comparing `goplus-0.1.4/goplus/address.py` & `goplus-0.1.5/goplus/address.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/goplus/approve.py` & `goplus-0.1.5/goplus/approve.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/goplus/auth.py` & `goplus-0.1.5/goplus/auth.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/goplus/base.py` & `goplus-0.1.5/goplus/base.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/goplus/chain.py` & `goplus-0.1.5/goplus/chain.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/goplus/dapp.py` & `goplus-0.1.5/goplus/dapp.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/goplus/decode.py` & `goplus-0.1.5/goplus/decode.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/goplus/errocode.py` & `goplus-0.1.5/goplus/errocode.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/goplus/nft.py` & `goplus-0.1.5/goplus/nft.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/goplus/phishing_site.py` & `goplus-0.1.5/goplus/phishing_site.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/goplus/rug_pull.py` & `goplus-0.1.5/goplus/rug_pull.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/goplus/token.py` & `goplus-0.1.5/goplus/token.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/goplus.egg-info/PKG-INFO` & `goplus-0.1.5/goplus.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goplus
-Version: 0.1.4
+Version: 0.1.5
 Summary: GoPlus SDK
 Home-page: https://github.com/GoPlusSecurity/goplus-sdk-python
 Author: GoPlus
 Author-email: service@gopluslabs.io
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `goplus-0.1.4/goplus.egg-info/SOURCES.txt` & `goplus-0.1.5/goplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/setup.py` & `goplus-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/__init__.py` & `goplus-0.1.5/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/api/__init__.py` & `goplus-0.1.5/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/api/approve_controller_v_1_api.py` & `goplus-0.1.5/swagger_client/api/approve_controller_v_1_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,16 +38,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.address_contract_using_get1(address, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str address: address (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
-        :param str chain_id: The chain_id of the blockchain. \"1\" means Ethereum;  \"10\" means Optimism; “25” means Cronos; \"56\" means BSC;  “66” means OKC; \"100\" means Gnosis; \"128\" means HECO;  \"137\" means Polygon;  \"250\" means Fantom; \"321\" means KCC; \"324\" means zkSync Era; \"10001\" means ETHW; \"201022\" means FON; \"42161\" means Arbitrum;  \"43114\" means Avalanche; \"59140\" means Linea; \"1666600000\" means Harmony; \"tron\" means Tron.
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str chain_id: The chain_id of the blockchain. \"1\" means Ethereum;  \"10\" means Optimism; \"25\" means Cronos; \"56\" means BSC;  \"66\" means OKC; \"100\" means Gnosis; \"128\" means HECO;  \"137\" means Polygon;  \"250\" means Fantom; \"321\" means KCC; \"324\" means zkSync Era; \"10001\" means ETHW; \"201022\" means FON; \"42161\" means Arbitrum;  \"43114\" means Avalanche; \"59140\" means Linea; \"1666600000\" means Harmony; \"tron\" means Tron.
         :return: ResponseWrapperAddressContract
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.address_contract_using_get1_with_http_info(address, **kwargs)  # noqa: E501
@@ -61,16 +61,16 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.address_contract_using_get1_with_http_info(address, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str address: address (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
-        :param str chain_id: The chain_id of the blockchain. \"1\" means Ethereum;  \"10\" means Optimism; “25” means Cronos; \"56\" means BSC;  “66” means OKC; \"100\" means Gnosis; \"128\" means HECO;  \"137\" means Polygon;  \"250\" means Fantom; \"321\" means KCC; \"324\" means zkSync Era; \"10001\" means ETHW; \"201022\" means FON; \"42161\" means Arbitrum;  \"43114\" means Avalanche; \"59140\" means Linea; \"1666600000\" means Harmony; \"tron\" means Tron.
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str chain_id: The chain_id of the blockchain. \"1\" means Ethereum;  \"10\" means Optimism; \"25\" means Cronos; \"56\" means BSC;  \"66\" means OKC; \"100\" means Gnosis; \"128\" means HECO;  \"137\" means Polygon;  \"250\" means Fantom; \"321\" means KCC; \"324\" means zkSync Era; \"10001\" means ETHW; \"201022\" means FON; \"42161\" means Arbitrum;  \"43114\" means Avalanche; \"59140\" means Linea; \"1666600000\" means Harmony; \"tron\" means Tron.
         :return: ResponseWrapperAddressContract
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['address', 'authorization', 'chain_id']  # noqa: E501
         all_params.append('async_req')
@@ -140,15 +140,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.approval_contract_using_get(chain_id, contract_addresses, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str chain_id: Chain id, (ETH: 1,  BSC: 56, OKC: 66, Heco: 128, Polygon: 137, Fantom:250, Arbitrum: 42161, Avalanche: 43114) (required)
         :param str contract_addresses: Contract needs to be detected (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :return: ResponseWrapperContractApproveResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.approval_contract_using_get_with_http_info(chain_id, contract_addresses, **kwargs)  # noqa: E501
@@ -163,15 +163,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.approval_contract_using_get_with_http_info(chain_id, contract_addresses, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str chain_id: Chain id, (ETH: 1,  BSC: 56, OKC: 66, Heco: 128, Polygon: 137, Fantom:250, Arbitrum: 42161, Avalanche: 43114) (required)
         :param str contract_addresses: Contract needs to be detected (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :return: ResponseWrapperContractApproveResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['chain_id', 'contract_addresses', 'authorization']  # noqa: E501
         all_params.append('async_req')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/api/approve_controller_v_2_api.py` & `goplus-0.1.5/swagger_client/api/approve_controller_v_2_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.address_nft1155_approve_list_using_get1(addresses, chain_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str addresses: contract address (required)
         :param str chain_id: chain id (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :return: ResponseWrapperListApproveNFT1155ListResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.address_nft1155_approve_list_using_get1_with_http_info(addresses, chain_id, **kwargs)  # noqa: E501
@@ -62,15 +62,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.address_nft1155_approve_list_using_get1_with_http_info(addresses, chain_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str addresses: contract address (required)
         :param str chain_id: chain id (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :return: ResponseWrapperListApproveNFT1155ListResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['addresses', 'chain_id', 'authorization']  # noqa: E501
         all_params.append('async_req')
@@ -144,15 +144,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.address_nft721_approve_list_using_get1(addresses, chain_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str addresses: contract address (required)
         :param str chain_id: chain id (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :return: ResponseWrapperListApproveNFTListResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.address_nft721_approve_list_using_get1_with_http_info(addresses, chain_id, **kwargs)  # noqa: E501
@@ -167,15 +167,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.address_nft721_approve_list_using_get1_with_http_info(addresses, chain_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str addresses: contract address (required)
         :param str chain_id: chain id (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :return: ResponseWrapperListApproveNFTListResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['addresses', 'chain_id', 'authorization']  # noqa: E501
         all_params.append('async_req')
@@ -249,15 +249,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.address_token_approve_list_using_get1(addresses, chain_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str addresses: contract address (required)
         :param str chain_id: chain id (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :return: ResponseWrapperListApproveTokenOutListResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.address_token_approve_list_using_get1_with_http_info(addresses, chain_id, **kwargs)  # noqa: E501
@@ -272,15 +272,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.address_token_approve_list_using_get1_with_http_info(addresses, chain_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str addresses: contract address (required)
         :param str chain_id: chain id (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :return: ResponseWrapperListApproveTokenOutListResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['addresses', 'chain_id', 'authorization']  # noqa: E501
         all_params.append('async_req')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/api/contract_abi_controller_api.py` & `goplus-0.1.5/swagger_client/api/contract_abi_controller_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_abi_data_info_using_post(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param ParseAbiDataRequest body: abiDataRequest (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :return: ResponseWrapperParseAbiDataResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_abi_data_info_using_post_with_http_info(body, **kwargs)  # noqa: E501
@@ -60,15 +60,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_abi_data_info_using_post_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param ParseAbiDataRequest body: abiDataRequest (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :return: ResponseWrapperParseAbiDataResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['body', 'authorization']  # noqa: E501
         all_params.append('async_req')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/api/dapp_controller_api.py` & `goplus-0.1.5/swagger_client/api/dapp_controller_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_dapp_info_using_get(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :param str url: Url or domain
         :return: ResponseWrapperDappContractSecurityResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -59,15 +59,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_dapp_info_using_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :param str url: Url or domain
         :return: ResponseWrapperDappContractSecurityResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['authorization', 'url']  # noqa: E501
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/api/defi_controller_api.py` & `goplus-0.1.5/swagger_client/api/defi_controller_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_defi_info_using_get(contract_addresses, chain_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str contract_addresses: Defi protocol address (required)
         :param str chain_id: Chain id, (eth: 1, bsc: 56) (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :return: GetDefiInfoResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_defi_info_using_get_with_http_info(contract_addresses, chain_id, **kwargs)  # noqa: E501
@@ -62,15 +62,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_defi_info_using_get_with_http_info(contract_addresses, chain_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str contract_addresses: Defi protocol address (required)
         :param str chain_id: Chain id, (eth: 1, bsc: 56) (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :return: GetDefiInfoResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['contract_addresses', 'chain_id', 'authorization']  # noqa: E501
         all_params.append('async_req')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/api/nft_controller_api.py` & `goplus-0.1.5/swagger_client/api/nft_controller_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_nft_info_using_get1(chain_id, contract_addresses, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str chain_id: Chain id, (eth: 1, bsc: 56, Polygon: 137, Avalanche: 43114) (required)
         :param str contract_addresses: NFT contract address (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :param str token_id: tokenId
         :return: ResponseWrapperGetNftInfo
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -63,15 +63,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_nft_info_using_get1_with_http_info(chain_id, contract_addresses, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str chain_id: Chain id, (eth: 1, bsc: 56, Polygon: 137, Avalanche: 43114) (required)
         :param str contract_addresses: NFT contract address (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :param str token_id: tokenId
         :return: ResponseWrapperGetNftInfo
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['chain_id', 'contract_addresses', 'authorization', 'token_id']  # noqa: E501
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/api/token_controller_api.py` & `goplus-0.1.5/swagger_client/api/token_controller_api.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/api/token_controller_v_1_api.py` & `goplus-0.1.5/swagger_client/api/token_controller_v_1_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_chains_list_using_get(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :param str name: API name.
         :return: ResponseWrapperListGetChainsList
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -59,15 +59,15 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_chains_list_using_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :param str name: API name.
         :return: ResponseWrapperListGetChainsList
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['authorization', 'name']  # noqa: E501
@@ -130,17 +130,17 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.token_security_using_get1(chain_id, contract_addresses, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str chain_id: The chain_id of the blockchain. \"1\" means Ethereum;  \"10\" means Optimism; “25” means Cronos; \"56\" means BSC;  “66” means OKC; \"100\" means Gnosis; \"128\" means HECO;  \"137\" means Polygon;  \"250\" means Fantom; \"321\" means KCC; \"324\" means zkSync Era; \"10001\" means ETHW; \"201022\" means FON; \"42161\" means Arbitrum;  \"43114\" means Avalanche; \"59140\" means Linea; \"1666600000\" means Harmony; \"tron\" means Tron. (required)
+        :param str chain_id: The chain_id of the blockchain. \"1\" means Ethereum;  \"10\" means Optimism; \"25\" means Cronos; \"56\" means BSC;  \"66\" means OKC; \"100\" means Gnosis; \"128\" means HECO;  \"137\" means Polygon;  \"250\" means Fantom; \"321\" means KCC; \"324\" means zkSync Era; \"10001\" means ETHW; \"201022\" means FON; \"42161\" means Arbitrum;  \"43114\" means Avalanche; \"59140\" means Linea; \"1666600000\" means Harmony; \"tron\" means Tron. (required)
         :param str contract_addresses: The contract address of tokens. (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :return: ResponseWrapperTokenSecurity
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.token_security_using_get1_with_http_info(chain_id, contract_addresses, **kwargs)  # noqa: E501
@@ -153,17 +153,17 @@
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.token_security_using_get1_with_http_info(chain_id, contract_addresses, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str chain_id: The chain_id of the blockchain. \"1\" means Ethereum;  \"10\" means Optimism; “25” means Cronos; \"56\" means BSC;  “66” means OKC; \"100\" means Gnosis; \"128\" means HECO;  \"137\" means Polygon;  \"250\" means Fantom; \"321\" means KCC; \"324\" means zkSync Era; \"10001\" means ETHW; \"201022\" means FON; \"42161\" means Arbitrum;  \"43114\" means Avalanche; \"59140\" means Linea; \"1666600000\" means Harmony; \"tron\" means Tron. (required)
+        :param str chain_id: The chain_id of the blockchain. \"1\" means Ethereum;  \"10\" means Optimism; \"25\" means Cronos; \"56\" means BSC;  \"66\" means OKC; \"100\" means Gnosis; \"128\" means HECO;  \"137\" means Polygon;  \"250\" means Fantom; \"321\" means KCC; \"324\" means zkSync Era; \"10001\" means ETHW; \"201022\" means FON; \"42161\" means Arbitrum;  \"43114\" means Avalanche; \"59140\" means Linea; \"1666600000\" means Harmony; \"tron\" means Tron. (required)
         :param str contract_addresses: The contract address of tokens. (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :return: ResponseWrapperTokenSecurity
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['chain_id', 'contract_addresses', 'authorization']  # noqa: E501
         all_params.append('async_req')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/api/website_controller_api.py` & `goplus-0.1.5/swagger_client/api/website_controller_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.phishing_site_using_get(url, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str url: Url (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :return: ResponseWrapperPhishingSite
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.phishing_site_using_get_with_http_info(url, **kwargs)  # noqa: E501
@@ -60,15 +60,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.phishing_site_using_get_with_http_info(url, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str url: Url (required)
-        :param str authorization: Authorization (test：Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
+        :param str authorization: Authorization (test: Bearer 81|9ihH8JzEuFu4MQ9DjWmH5WrNCPW...)
         :return: ResponseWrapperPhishingSite
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['url', 'authorization']  # noqa: E501
         all_params.append('async_req')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/api_client.py` & `goplus-0.1.5/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/configuration.py` & `goplus-0.1.5/swagger_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     Ref: https://github.com/swagger-api/swagger-codegen
     Do not edit the class manually.
     """
 
     def __init__(self):
         """Constructor"""
         # Default Base url
-        self.host = "https://api.gopluslabs.io/"
+        self.host = "https://api.gopluslabs.io"
         # Temp file folder for downloading files
         self.temp_folder_path = None
 
         # Authentication Settings
         # dict to store API key(s)
         self.api_key = {}
         # dict to store API prefix (e.g. Bearer)
```

### Comparing `goplus-0.1.4/swagger_client/models/__init__.py` & `goplus-0.1.5/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/abi_address_info.py` & `goplus-0.1.5/swagger_client/models/abi_address_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/abi_param_info.py` & `goplus-0.1.5/swagger_client/models/abi_param_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/approve_address_info.py` & `goplus-0.1.5/swagger_client/models/approve_address_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/approve_erc1155_result.py` & `goplus-0.1.5/swagger_client/models/approve_erc1155_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/approve_nft1155_list_response.py` & `goplus-0.1.5/swagger_client/models/approve_nft1155_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/approve_nft_list_response.py` & `goplus-0.1.5/swagger_client/models/approve_nft_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/approve_result.py` & `goplus-0.1.5/swagger_client/models/approve_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/approve_token_out_list_response.py` & `goplus-0.1.5/swagger_client/models/approve_token_out_list_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/approve_token_result.py` & `goplus-0.1.5/swagger_client/models/approve_token_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/audit_info.py` & `goplus-0.1.5/swagger_client/models/audit_info.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/contract_approve_response.py` & `goplus-0.1.5/swagger_client/models/contract_approve_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,26 +248,26 @@
 
         self._is_proxy = is_proxy
 
     @property
     def malicious_behavior(self):
         """Gets the malicious_behavior of this ContractApproveResponse.  # noqa: E501
 
-        It describes specific malicious behaviors. \"honeypot_related_address\" means that the address is related to honeypot tokens or has created scam tokens. \"phishing_activities\" means that this address has implemented phishing activities. \"blackmail_activities\" means that this address has implemented blackmail activities. \"stealing_attack\" means that this address has implemented stealing attacks. \"fake_kyc\" means that this address is involved in fake KYC. \"malicious_mining_activities\" means that this address is involved in malicious mining activities. \"darkweb_transactions\" means that this address is involved in darkweb transactions. \"cybercrime\" means that this address is involved in cybercrime. \"money_laundering\" means that this address is involved in money laundering. \"financial_crime\" means that this address is involved in financial crime. “blacklist_doubt” means that the address is suspected of malicious behavior and is therefore blacklisted.(Notice:Returning an empty array means that no malicious behavior was found at that address.)  # noqa: E501
+        It describes specific malicious behaviors. \"honeypot_related_address\" means that the address is related to honeypot tokens or has created scam tokens. \"phishing_activities\" means that this address has implemented phishing activities. \"blackmail_activities\" means that this address has implemented blackmail activities. \"stealing_attack\" means that this address has implemented stealing attacks. \"fake_kyc\" means that this address is involved in fake KYC. \"malicious_mining_activities\" means that this address is involved in malicious mining activities. \"darkweb_transactions\" means that this address is involved in darkweb transactions. \"cybercrime\" means that this address is involved in cybercrime. \"money_laundering\" means that this address is involved in money laundering. \"financial_crime\" means that this address is involved in financial crime. \"blacklist_doubt\" means that the address is suspected of malicious behavior and is therefore blacklisted.(Notice:Returning an empty array means that no malicious behavior was found at that address.)  # noqa: E501
 
         :return: The malicious_behavior of this ContractApproveResponse.  # noqa: E501
         :rtype: list[str]
         """
         return self._malicious_behavior
 
     @malicious_behavior.setter
     def malicious_behavior(self, malicious_behavior):
         """Sets the malicious_behavior of this ContractApproveResponse.
 
-        It describes specific malicious behaviors. \"honeypot_related_address\" means that the address is related to honeypot tokens or has created scam tokens. \"phishing_activities\" means that this address has implemented phishing activities. \"blackmail_activities\" means that this address has implemented blackmail activities. \"stealing_attack\" means that this address has implemented stealing attacks. \"fake_kyc\" means that this address is involved in fake KYC. \"malicious_mining_activities\" means that this address is involved in malicious mining activities. \"darkweb_transactions\" means that this address is involved in darkweb transactions. \"cybercrime\" means that this address is involved in cybercrime. \"money_laundering\" means that this address is involved in money laundering. \"financial_crime\" means that this address is involved in financial crime. “blacklist_doubt” means that the address is suspected of malicious behavior and is therefore blacklisted.(Notice:Returning an empty array means that no malicious behavior was found at that address.)  # noqa: E501
+        It describes specific malicious behaviors. \"honeypot_related_address\" means that the address is related to honeypot tokens or has created scam tokens. \"phishing_activities\" means that this address has implemented phishing activities. \"blackmail_activities\" means that this address has implemented blackmail activities. \"stealing_attack\" means that this address has implemented stealing attacks. \"fake_kyc\" means that this address is involved in fake KYC. \"malicious_mining_activities\" means that this address is involved in malicious mining activities. \"darkweb_transactions\" means that this address is involved in darkweb transactions. \"cybercrime\" means that this address is involved in cybercrime. \"money_laundering\" means that this address is involved in money laundering. \"financial_crime\" means that this address is involved in financial crime. \"blacklist_doubt\" means that the address is suspected of malicious behavior and is therefore blacklisted.(Notice:Returning an empty array means that no malicious behavior was found at that address.)  # noqa: E501
 
         :param malicious_behavior: The malicious_behavior of this ContractApproveResponse.  # noqa: E501
         :type: list[str]
         """
 
         self._malicious_behavior = malicious_behavior
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/contracts.py` & `goplus-0.1.5/swagger_client/models/contracts.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/contracts_security.py` & `goplus-0.1.5/swagger_client/models/contracts_security.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/dapp_contract_security_response.py` & `goplus-0.1.5/swagger_client/models/dapp_contract_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/get_access_token_request.py` & `goplus-0.1.5/swagger_client/models/get_access_token_request.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/get_access_token_response.py` & `goplus-0.1.5/swagger_client/models/get_access_token_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/get_defi_info_response.py` & `goplus-0.1.5/swagger_client/models/get_defi_info_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if result is not None:
             self.result = result
 
     @property
     def code(self):
         """Gets the code of this GetDefiInfoResponse.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this GetDefiInfoResponse.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this GetDefiInfoResponse.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this GetDefiInfoResponse.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/get_defi_info_response_result.py` & `goplus-0.1.5/swagger_client/models/get_defi_info_response_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,72 +218,72 @@
 
         self._contract_name = contract_name
 
     @property
     def selfdestruct(self):
         """Gets the selfdestruct of this GetDefiInfoResponseResult.  # noqa: E501
 
-        It describes whether this contract can self destruct. \"1\" means true;  \"0\" means false; “-1” means unknown.  # noqa: E501
+        It describes whether this contract can self destruct. \"1\" means true;  \"0\" means false; \"-1\" means unknown.  # noqa: E501
 
         :return: The selfdestruct of this GetDefiInfoResponseResult.  # noqa: E501
         :rtype: int
         """
         return self._selfdestruct
 
     @selfdestruct.setter
     def selfdestruct(self, selfdestruct):
         """Sets the selfdestruct of this GetDefiInfoResponseResult.
 
-        It describes whether this contract can self destruct. \"1\" means true;  \"0\" means false; “-1” means unknown.  # noqa: E501
+        It describes whether this contract can self destruct. \"1\" means true;  \"0\" means false; \"-1\" means unknown.  # noqa: E501
 
         :param selfdestruct: The selfdestruct of this GetDefiInfoResponseResult.  # noqa: E501
         :type: int
         """
 
         self._selfdestruct = selfdestruct
 
     @property
     def is_proxy(self):
         """Gets the is_proxy of this GetDefiInfoResponseResult.  # noqa: E501
 
-        It describes whether this contract has a proxy contract.  \"1\" means true;  \"0\" means false; “-1” means unknown.  # noqa: E501
+        It describes whether this contract has a proxy contract.  \"1\" means true;  \"0\" means false; \"-1\" means unknown.  # noqa: E501
 
         :return: The is_proxy of this GetDefiInfoResponseResult.  # noqa: E501
         :rtype: int
         """
         return self._is_proxy
 
     @is_proxy.setter
     def is_proxy(self, is_proxy):
         """Sets the is_proxy of this GetDefiInfoResponseResult.
 
-        It describes whether this contract has a proxy contract.  \"1\" means true;  \"0\" means false; “-1” means unknown.  # noqa: E501
+        It describes whether this contract has a proxy contract.  \"1\" means true;  \"0\" means false; \"-1\" means unknown.  # noqa: E501
 
         :param is_proxy: The is_proxy of this GetDefiInfoResponseResult.  # noqa: E501
         :type: int
         """
 
         self._is_proxy = is_proxy
 
     @property
     def approval_abuse(self):
         """Gets the approval_abuse of this GetDefiInfoResponseResult.  # noqa: E501
 
-        It describes whether the owner can spend the allowance that obtained by the contract. If so, this function could potentially be abused to steal user assets. \"1\" means true;  \"0\" means false; “-1” means unknown.  # noqa: E501
+        It describes whether the owner can spend the allowance that obtained by the contract. If so, this function could potentially be abused to steal user assets. \"1\" means true;  \"0\" means false; \"-1\" means unknown.  # noqa: E501
 
         :return: The approval_abuse of this GetDefiInfoResponseResult.  # noqa: E501
         :rtype: int
         """
         return self._approval_abuse
 
     @approval_abuse.setter
     def approval_abuse(self, approval_abuse):
         """Sets the approval_abuse of this GetDefiInfoResponseResult.
 
-        It describes whether the owner can spend the allowance that obtained by the contract. If so, this function could potentially be abused to steal user assets. \"1\" means true;  \"0\" means false; “-1” means unknown.  # noqa: E501
+        It describes whether the owner can spend the allowance that obtained by the contract. If so, this function could potentially be abused to steal user assets. \"1\" means true;  \"0\" means false; \"-1\" means unknown.  # noqa: E501
 
         :param approval_abuse: The approval_abuse of this GetDefiInfoResponseResult.  # noqa: E501
         :type: int
         """
 
         self._approval_abuse = approval_abuse
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/get_defi_info_response_result_owner.py` & `goplus-0.1.5/swagger_client/models/get_defi_info_response_result_owner.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/json_object.py` & `goplus-0.1.5/swagger_client/models/json_object.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/map_string_string.py` & `goplus-0.1.5/swagger_client/models/map_string_string.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/parse_abi_data_request.py` & `goplus-0.1.5/swagger_client/models/parse_abi_data_request.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/parse_abi_data_response.py` & `goplus-0.1.5/swagger_client/models/parse_abi_data_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_address_contract.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_address_contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if result is not None:
             self.result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperAddressContract.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this ResponseWrapperAddressContract.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this ResponseWrapperAddressContract.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this ResponseWrapperAddressContract.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_address_contract_result.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_address_contract_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,26 +324,26 @@
 
         self._blacklist_doubt = blacklist_doubt
 
     @property
     def data_source(self):
         """Gets the data_source of this ResponseWrapperAddressContractResult.  # noqa: E501
 
-        It describes the data source for this address information. For example：GoPlus/SlowMist  # noqa: E501
+        It describes the data source for this address information. For example: GoPlus/SlowMist  # noqa: E501
 
         :return: The data_source of this ResponseWrapperAddressContractResult.  # noqa: E501
         :rtype: str
         """
         return self._data_source
 
     @data_source.setter
     def data_source(self, data_source):
         """Sets the data_source of this ResponseWrapperAddressContractResult.
 
-        It describes the data source for this address information. For example：GoPlus/SlowMist  # noqa: E501
+        It describes the data source for this address information. For example: GoPlus/SlowMist  # noqa: E501
 
         :param data_source: The data_source of this ResponseWrapperAddressContractResult.  # noqa: E501
         :type: str
         """
 
         self._data_source = data_source
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_contract_approve_response.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_contract_approve_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if result is not None:
             self.result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperContractApproveResponse.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this ResponseWrapperContractApproveResponse.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this ResponseWrapperContractApproveResponse.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this ResponseWrapperContractApproveResponse.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_dapp_contract_security_response.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_dapp_contract_security_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if result is not None:
             self.result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperDappContractSecurityResponse.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this ResponseWrapperDappContractSecurityResponse.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this ResponseWrapperDappContractSecurityResponse.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this ResponseWrapperDappContractSecurityResponse.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_get_access_token_response.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_get_access_token_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,26 +73,26 @@
 
         self._result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperGetAccessTokenResponse.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this ResponseWrapperGetAccessTokenResponse.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this ResponseWrapperGetAccessTokenResponse.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this ResponseWrapperGetAccessTokenResponse.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_get_nft_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if result is not None:
             self.result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperGetNftInfo.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this ResponseWrapperGetNftInfo.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this ResponseWrapperGetNftInfo.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this ResponseWrapperGetNftInfo.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_get_nft_info_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,26 +376,26 @@
 
         self._transfer_without_approval = transfer_without_approval
 
     @property
     def discord_url(self):
         """Gets the discord_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
-        It describes the discord url of the NFT. Return “null” means there is no discord url or didn't find the discord url.  # noqa: E501
+        It describes the discord url of the NFT. Return \"null\" means there is no discord url or didn't find the discord url.  # noqa: E501
 
         :return: The discord_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._discord_url
 
     @discord_url.setter
     def discord_url(self, discord_url):
         """Sets the discord_url of this ResponseWrapperGetNftInfoResult.
 
-        It describes the discord url of the NFT. Return “null” means there is no discord url or didn't find the discord url.  # noqa: E501
+        It describes the discord url of the NFT. Return \"null\" means there is no discord url or didn't find the discord url.  # noqa: E501
 
         :param discord_url: The discord_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._discord_url = discord_url
 
@@ -581,49 +581,49 @@
 
         self._nft_erc = nft_erc
 
     @property
     def creator_address(self):
         """Gets the creator_address of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
-        It describes the creator address of the NFT. Example: \"creator_address\": \"0x1ee0af784b96bb55ece98c9b15675726b0da1b6b\"; Return “null” means that we didn't find the creator address.  # noqa: E501
+        It describes the creator address of the NFT. Example: \"creator_address\": \"0x1ee0af784b96bb55ece98c9b15675726b0da1b6b\"; Return \"null\" means that we didn't find the creator address.  # noqa: E501
 
         :return: The creator_address of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._creator_address
 
     @creator_address.setter
     def creator_address(self, creator_address):
         """Sets the creator_address of this ResponseWrapperGetNftInfoResult.
 
-        It describes the creator address of the NFT. Example: \"creator_address\": \"0x1ee0af784b96bb55ece98c9b15675726b0da1b6b\"; Return “null” means that we didn't find the creator address.  # noqa: E501
+        It describes the creator address of the NFT. Example: \"creator_address\": \"0x1ee0af784b96bb55ece98c9b15675726b0da1b6b\"; Return \"null\" means that we didn't find the creator address.  # noqa: E501
 
         :param creator_address: The creator_address of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._creator_address = creator_address
 
     @property
     def medium_url(self):
         """Gets the medium_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
-        It describes the medium url of the NFT. Return “null” means there is no medium url or didn't find the medium url.  # noqa: E501
+        It describes the medium url of the NFT. Return \"null\" means there is no medium url or didn't find the medium url.  # noqa: E501
 
         :return: The medium_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._medium_url
 
     @medium_url.setter
     def medium_url(self, medium_url):
         """Sets the medium_url of this ResponseWrapperGetNftInfoResult.
 
-        It describes the medium url of the NFT. Return “null” means there is no medium url or didn't find the medium url.  # noqa: E501
+        It describes the medium url of the NFT. Return \"null\" means there is no medium url or didn't find the medium url.  # noqa: E501
 
         :param medium_url: The medium_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._medium_url = medium_url
 
@@ -671,26 +671,26 @@
 
         self._privileged_burn = privileged_burn
 
     @property
     def twitter_url(self):
         """Gets the twitter_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
-        It describes the twitter url of the NFT. Return “null” means there is no twitter url or didn't find the twitter url.  # noqa: E501
+        It describes the twitter url of the NFT. Return \"null\" means there is no twitter url or didn't find the twitter url.  # noqa: E501
 
         :return: The twitter_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._twitter_url
 
     @twitter_url.setter
     def twitter_url(self, twitter_url):
         """Sets the twitter_url of this ResponseWrapperGetNftInfoResult.
 
-        It describes the twitter url of the NFT. Return “null” means there is no twitter url or didn't find the twitter url.  # noqa: E501
+        It describes the twitter url of the NFT. Return \"null\" means there is no twitter url or didn't find the twitter url.  # noqa: E501
 
         :param twitter_url: The twitter_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._twitter_url = twitter_url
 
@@ -717,26 +717,26 @@
 
         self._nft_symbol = nft_symbol
 
     @property
     def nft_description(self):
         """Gets the nft_description of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
-        It describes the introduction of the NFT. Return “null” means there is no description of the NFT.  # noqa: E501
+        It describes the introduction of the NFT. Return \"null\" means there is no description of the NFT.  # noqa: E501
 
         :return: The nft_description of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._nft_description
 
     @nft_description.setter
     def nft_description(self, nft_description):
         """Sets the nft_description of this ResponseWrapperGetNftInfoResult.
 
-        It describes the introduction of the NFT. Return “null” means there is no description of the NFT.  # noqa: E501
+        It describes the introduction of the NFT. Return \"null\" means there is no description of the NFT.  # noqa: E501
 
         :param nft_description: The nft_description of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._nft_description = nft_description
 
@@ -876,26 +876,26 @@
 
         self._nft_items = nft_items
 
     @property
     def oversupply_minting(self):
         """Gets the oversupply_minting of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
-        It describes whether this NFT owner can bypass the maximum amount of minting specified in the contract, and continue to mint NFTs beyond this limit.  \"1\" means true;  \"0\" means false;  \"Null\" means unknown.(Notice:Oversupply minting refers to the existence of a special mint method in the NFT contract — the owner can bypass the maximum amount of minting specified in the contract, and continue to mint NFTs beyond this limit.)  # noqa: E501
+        It describes whether this NFT owner can bypass the maximum amount of minting specified in the contract, and continue to mint NFTs beyond this limit.  \"1\" means true;  \"0\" means false;  \"Null\" means unknown.(Notice:Oversupply minting refers to the existence of a special mint method in the NFT contract - the owner can bypass the maximum amount of minting specified in the contract, and continue to mint NFTs beyond this limit.)  # noqa: E501
 
         :return: The oversupply_minting of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: int
         """
         return self._oversupply_minting
 
     @oversupply_minting.setter
     def oversupply_minting(self, oversupply_minting):
         """Sets the oversupply_minting of this ResponseWrapperGetNftInfoResult.
 
-        It describes whether this NFT owner can bypass the maximum amount of minting specified in the contract, and continue to mint NFTs beyond this limit.  \"1\" means true;  \"0\" means false;  \"Null\" means unknown.(Notice:Oversupply minting refers to the existence of a special mint method in the NFT contract — the owner can bypass the maximum amount of minting specified in the contract, and continue to mint NFTs beyond this limit.)  # noqa: E501
+        It describes whether this NFT owner can bypass the maximum amount of minting specified in the contract, and continue to mint NFTs beyond this limit.  \"1\" means true;  \"0\" means false;  \"Null\" means unknown.(Notice:Oversupply minting refers to the existence of a special mint method in the NFT contract - the owner can bypass the maximum amount of minting specified in the contract, and continue to mint NFTs beyond this limit.)  # noqa: E501
 
         :param oversupply_minting: The oversupply_minting of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: int
         """
 
         self._oversupply_minting = oversupply_minting
 
@@ -922,72 +922,72 @@
 
         self._nft_name = nft_name
 
     @property
     def website_url(self):
         """Gets the website_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
-        It describes the website url of the NFT. Return “null” means there is no website url or didn't find the website url.  # noqa: E501
+        It describes the website url of the NFT. Return \"null\" means there is no website url or didn't find the website url.  # noqa: E501
 
         :return: The website_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._website_url
 
     @website_url.setter
     def website_url(self, website_url):
         """Sets the website_url of this ResponseWrapperGetNftInfoResult.
 
-        It describes the website url of the NFT. Return “null” means there is no website url or didn't find the website url.  # noqa: E501
+        It describes the website url of the NFT. Return \"null\" means there is no website url or didn't find the website url.  # noqa: E501
 
         :param website_url: The website_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._website_url = website_url
 
     @property
     def github_url(self):
         """Gets the github_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
-        It describes the github url of the NFT. Return “null” means there is no github url or didn't find the github url.  # noqa: E501
+        It describes the github url of the NFT. Return \"null\" means there is no github url or didn't find the github url.  # noqa: E501
 
         :return: The github_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._github_url
 
     @github_url.setter
     def github_url(self, github_url):
         """Sets the github_url of this ResponseWrapperGetNftInfoResult.
 
-        It describes the github url of the NFT. Return “null” means there is no github url or didn't find the github url.  # noqa: E501
+        It describes the github url of the NFT. Return \"null\" means there is no github url or didn't find the github url.  # noqa: E501
 
         :param github_url: The github_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._github_url = github_url
 
     @property
     def telegram_url(self):
         """Gets the telegram_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
-        It describes the telegram url of the NFT. Return “null” means there is no telegram url or didn't find the telegram url.  # noqa: E501
+        It describes the telegram url of the NFT. Return \"null\" means there is no telegram url or didn't find the telegram url.  # noqa: E501
 
         :return: The telegram_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: str
         """
         return self._telegram_url
 
     @telegram_url.setter
     def telegram_url(self, telegram_url):
         """Sets the telegram_url of this ResponseWrapperGetNftInfoResult.
 
-        It describes the telegram url of the NFT. Return “null” means there is no telegram url or didn't find the telegram url.  # noqa: E501
+        It describes the telegram url of the NFT. Return \"null\" means there is no telegram url or didn't find the telegram url.  # noqa: E501
 
         :param telegram_url: The telegram_url of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: str
         """
 
         self._telegram_url = telegram_url
 
@@ -1014,26 +1014,26 @@
 
         self._sales_24h = sales_24h
 
     @property
     def create_block_number(self):
         """Gets the create_block_number of this ResponseWrapperGetNftInfoResult.  # noqa: E501
 
-        It describes the number of blocks created for the NFT. Return “null” means that we didn't find the number of blocks created for the NFT.  # noqa: E501
+        It describes the number of blocks created for the NFT. Return \"null\" means that we didn't find the number of blocks created for the NFT.  # noqa: E501
 
         :return: The create_block_number of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :rtype: int
         """
         return self._create_block_number
 
     @create_block_number.setter
     def create_block_number(self, create_block_number):
         """Sets the create_block_number of this ResponseWrapperGetNftInfoResult.
 
-        It describes the number of blocks created for the NFT. Return “null” means that we didn't find the number of blocks created for the NFT.  # noqa: E501
+        It describes the number of blocks created for the NFT. Return \"null\" means that we didn't find the number of blocks created for the NFT.  # noqa: E501
 
         :param create_block_number: The create_block_number of this ResponseWrapperGetNftInfoResult.  # noqa: E501
         :type: int
         """
 
         self._create_block_number = create_block_number
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_get_nft_info_result_privileged_burn.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_get_nft_info_result_privileged_minting.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_get_nft_info_result_same_nfts.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_get_nft_info_result_self_destruct.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_get_nft_info_result_transfer_without_approval.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_json_object.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_json_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if result is not None:
             self.result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperJSONObject.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this ResponseWrapperJSONObject.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this ResponseWrapperJSONObject.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this ResponseWrapperJSONObject.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_list_approve_nft1155_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if result is not None:
             self.result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperListApproveNFT1155ListResponse.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this ResponseWrapperListApproveNFT1155ListResponse.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this ResponseWrapperListApproveNFT1155ListResponse.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this ResponseWrapperListApproveNFT1155ListResponse.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_list_approve_nft_list_response.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_list_approve_nft_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if result is not None:
             self.result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperListApproveNFTListResponse.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this ResponseWrapperListApproveNFTListResponse.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this ResponseWrapperListApproveNFTListResponse.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this ResponseWrapperListApproveNFTListResponse.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_list_approve_token_out_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if result is not None:
             self.result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this ResponseWrapperListApproveTokenOutListResponse.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this ResponseWrapperListApproveTokenOutListResponse.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_list_get_chains_list.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_list_get_chains_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if result is not None:
             self.result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperListGetChainsList.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this ResponseWrapperListGetChainsList.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this ResponseWrapperListGetChainsList.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this ResponseWrapperListGetChainsList.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_list_get_chains_list_result.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_list_get_chains_list_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_list_json_object.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_list_json_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if result is not None:
             self.result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperListJSONObject.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this ResponseWrapperListJSONObject.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this ResponseWrapperListJSONObject.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this ResponseWrapperListJSONObject.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_map_string_string.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_map_string_string.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if result is not None:
             self.result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperMapStringString.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this ResponseWrapperMapStringString.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this ResponseWrapperMapStringString.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this ResponseWrapperMapStringString.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_parse_abi_data_response.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_parse_abi_data_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if result is not None:
             self.result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperParseAbiDataResponse.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this ResponseWrapperParseAbiDataResponse.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this ResponseWrapperParseAbiDataResponse.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this ResponseWrapperParseAbiDataResponse.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_phishing_site.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_phishing_site.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if result is not None:
             self.result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperPhishingSite.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this ResponseWrapperPhishingSite.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this ResponseWrapperPhishingSite.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this ResponseWrapperPhishingSite.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_phishing_site_result.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_phishing_site_result.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_ta_token_security_response.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_ta_token_security_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if result is not None:
             self.result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this ResponseWrapperTaTokenSecurityResponse.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this ResponseWrapperTaTokenSecurityResponse.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_token_security.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_token_security.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if result is not None:
             self.result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperTokenSecurity.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this ResponseWrapperTokenSecurity.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this ResponseWrapperTokenSecurity.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this ResponseWrapperTokenSecurity.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_token_security_dex.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_token_security_dex.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_token_security_locked_detail.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_token_security_locked_detail.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_token_security_lp_holders.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_token_security_lp_holders.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,26 +72,26 @@
         if percent is not None:
             self.percent = percent
 
     @property
     def is_locked(self):
         """Gets the is_locked of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
 
-        It describes whether the tokens owned by the holder are locked \"1\" means true; \"0\" means false;  (3) “tag” describes the address's public tag. Example:Burn (Notice:About \"locked\": We only support the token lock addresses or black hole addresses that we have included. )  # noqa: E501
+        It describes whether the tokens owned by the holder are locked \"1\" means true; \"0\" means false;  (3) \"tag\" describes the address's public tag. Example:Burn (Notice:About \"locked\": We only support the token lock addresses or black hole addresses that we have included. )  # noqa: E501
 
         :return: The is_locked of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
         :rtype: int
         """
         return self._is_locked
 
     @is_locked.setter
     def is_locked(self, is_locked):
         """Sets the is_locked of this ResponseWrapperTokenSecurityLpHolders.
 
-        It describes whether the tokens owned by the holder are locked \"1\" means true; \"0\" means false;  (3) “tag” describes the address's public tag. Example:Burn (Notice:About \"locked\": We only support the token lock addresses or black hole addresses that we have included. )  # noqa: E501
+        It describes whether the tokens owned by the holder are locked \"1\" means true; \"0\" means false;  (3) \"tag\" describes the address's public tag. Example:Burn (Notice:About \"locked\": We only support the token lock addresses or black hole addresses that we have included. )  # noqa: E501
 
         :param is_locked: The is_locked of this ResponseWrapperTokenSecurityLpHolders.  # noqa: E501
         :type: int
         """
 
         self._is_locked = is_locked
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapper_token_security_result.py` & `goplus-0.1.5/swagger_client/models/response_wrapper_token_security_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,26 +247,26 @@
         if token_symbol is not None:
             self.token_symbol = token_symbol
 
     @property
     def note(self):
         """Gets the note of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
-        It describes whether the contract has other things investors need to know.  Example:  \"note”: “Contract owner is a multisign contract.”(Notice:(1) If we haven't found any other thing which is valuable yet, there will be no return.  (2) Type: string.)  # noqa: E501
+        It describes whether the contract has other things investors need to know.  Example:  \"note\": \"Contract owner is a multisign contract.\"(Notice:(1) If we haven't found any other thing which is valuable yet, there will be no return.  (2) Type: string.)  # noqa: E501
 
         :return: The note of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._note
 
     @note.setter
     def note(self, note):
         """Sets the note of this ResponseWrapperTokenSecurityResult.
 
-        It describes whether the contract has other things investors need to know.  Example:  \"note”: “Contract owner is a multisign contract.”(Notice:(1) If we haven't found any other thing which is valuable yet, there will be no return.  (2) Type: string.)  # noqa: E501
+        It describes whether the contract has other things investors need to know.  Example:  \"note\": \"Contract owner is a multisign contract.\"(Notice:(1) If we haven't found any other thing which is valuable yet, there will be no return.  (2) Type: string.)  # noqa: E501
 
         :param note: The note of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._note = note
 
@@ -339,26 +339,26 @@
 
         self._is_airdrop_scam = is_airdrop_scam
 
     @property
     def other_potential_risks(self):
         """Gets the other_potential_risks of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
-        It describes whether the contract has other potential risks. Example: “other_potential_risks”: “Owner can set different transaction taxes for each user, which can trigger serious losses.”(Notice:(1) If we haven't found any other potential risk yet, there will be no return.  (2) Type: string.)  # noqa: E501
+        It describes whether the contract has other potential risks. Example: \"other_potential_risks\": \"Owner can set different transaction taxes for each user, which can trigger serious losses.\"(Notice:(1) If we haven't found any other potential risk yet, there will be no return.  (2) Type: string.)  # noqa: E501
 
         :return: The other_potential_risks of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._other_potential_risks
 
     @other_potential_risks.setter
     def other_potential_risks(self, other_potential_risks):
         """Sets the other_potential_risks of this ResponseWrapperTokenSecurityResult.
 
-        It describes whether the contract has other potential risks. Example: “other_potential_risks”: “Owner can set different transaction taxes for each user, which can trigger serious losses.”(Notice:(1) If we haven't found any other potential risk yet, there will be no return.  (2) Type: string.)  # noqa: E501
+        It describes whether the contract has other potential risks. Example: \"other_potential_risks\": \"Owner can set different transaction taxes for each user, which can trigger serious losses.\"(Notice:(1) If we haven't found any other potential risk yet, there will be no return.  (2) Type: string.)  # noqa: E501
 
         :param other_potential_risks: The other_potential_risks of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._other_potential_risks = other_potential_risks
 
@@ -408,26 +408,26 @@
 
         self._trading_cooldown = trading_cooldown
 
     @property
     def hidden_owner(self):
         """Gets the hidden_owner of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
-        It describes whether the contract has hidden owners. For contract with a hidden owner, developer can still manipulate the contract even if the ownership has been abandoned. “1” means true; \"0\" means false; No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Hidden owner is often used by developers to hide ownership and is often accompanied by malicious functionality. When the hidden owner exists, it is assumed that ownership has not been abandoned.)  # noqa: E501
+        It describes whether the contract has hidden owners. For contract with a hidden owner, developer can still manipulate the contract even if the ownership has been abandoned. \"1\" means true; \"0\" means false; No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Hidden owner is often used by developers to hide ownership and is often accompanied by malicious functionality. When the hidden owner exists, it is assumed that ownership has not been abandoned.)  # noqa: E501
 
         :return: The hidden_owner of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._hidden_owner
 
     @hidden_owner.setter
     def hidden_owner(self, hidden_owner):
         """Sets the hidden_owner of this ResponseWrapperTokenSecurityResult.
 
-        It describes whether the contract has hidden owners. For contract with a hidden owner, developer can still manipulate the contract even if the ownership has been abandoned. “1” means true; \"0\" means false; No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Hidden owner is often used by developers to hide ownership and is often accompanied by malicious functionality. When the hidden owner exists, it is assumed that ownership has not been abandoned.)  # noqa: E501
+        It describes whether the contract has hidden owners. For contract with a hidden owner, developer can still manipulate the contract even if the ownership has been abandoned. \"1\" means true; \"0\" means false; No return means unknown.(Notice:(1) When \"is_open_source\": \"0\", there will be no return.  (2) Sometimes, when \"is_proxy\": \"1\", there will be no return.  (3) Hidden owner is often used by developers to hide ownership and is often accompanied by malicious functionality. When the hidden owner exists, it is assumed that ownership has not been abandoned.)  # noqa: E501
 
         :param hidden_owner: The hidden_owner of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._hidden_owner = hidden_owner
 
@@ -1144,26 +1144,26 @@
 
         self._owner_change_balance = owner_change_balance
 
     @property
     def cannot_buy(self):
         """Gets the cannot_buy of this ResponseWrapperTokenSecurityResult.  # noqa: E501
 
-        It deiscribes whether the Token can be bought. \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) Generally, \"cannot_buy\": \"1\" would be found in Reward Tokens. Such Tokens are issued as rewards for some on-chain applications and cannot be bought directly by users. (2) Sometimes token's anti-bot mechanism would affect our sandbox system, causing the display of \"buy_tax\": \"1\". (3) When “cannot_buy”: \"1\", our sandbox system might be bloked, causing the display of \"buy_tax\": \"1\" and \"sell_tax\": \"1\")  # noqa: E501
+        It deiscribes whether the Token can be bought. \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) Generally, \"cannot_buy\": \"1\" would be found in Reward Tokens. Such Tokens are issued as rewards for some on-chain applications and cannot be bought directly by users. (2) Sometimes token's anti-bot mechanism would affect our sandbox system, causing the display of \"buy_tax\": \"1\". (3) When \"cannot_buy\": \"1\", our sandbox system might be bloked, causing the display of \"buy_tax\": \"1\" and \"sell_tax\": \"1\")  # noqa: E501
 
         :return: The cannot_buy of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :rtype: str
         """
         return self._cannot_buy
 
     @cannot_buy.setter
     def cannot_buy(self, cannot_buy):
         """Sets the cannot_buy of this ResponseWrapperTokenSecurityResult.
 
-        It deiscribes whether the Token can be bought. \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) Generally, \"cannot_buy\": \"1\" would be found in Reward Tokens. Such Tokens are issued as rewards for some on-chain applications and cannot be bought directly by users. (2) Sometimes token's anti-bot mechanism would affect our sandbox system, causing the display of \"buy_tax\": \"1\". (3) When “cannot_buy”: \"1\", our sandbox system might be bloked, causing the display of \"buy_tax\": \"1\" and \"sell_tax\": \"1\")  # noqa: E501
+        It deiscribes whether the Token can be bought. \"1\" means true;  \"0\" means false;  No return means unknown.(Notice:(1) Generally, \"cannot_buy\": \"1\" would be found in Reward Tokens. Such Tokens are issued as rewards for some on-chain applications and cannot be bought directly by users. (2) Sometimes token's anti-bot mechanism would affect our sandbox system, causing the display of \"buy_tax\": \"1\". (3) When \"cannot_buy\": \"1\", our sandbox system might be bloked, causing the display of \"buy_tax\": \"1\" and \"sell_tax\": \"1\")  # noqa: E501
 
         :param cannot_buy: The cannot_buy of this ResponseWrapperTokenSecurityResult.  # noqa: E501
         :type: str
         """
 
         self._cannot_buy = cannot_buy
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/response_wrapperobject.py` & `goplus-0.1.5/swagger_client/models/response_wrapperobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if result is not None:
             self.result = result
 
     @property
     def code(self):
         """Gets the code of this ResponseWrapperobject.  # noqa: E501
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :return: The code of this ResponseWrapperobject.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
         """Sets the code of this ResponseWrapperobject.
 
-        Code 1：Success  # noqa: E501
+        Code 1: Success  # noqa: E501
 
         :param code: The code of this ResponseWrapperobject.  # noqa: E501
         :type: int
         """
 
         self._code = code
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `goplus-0.1.4/swagger_client/models/ta_token_security_response.py` & `goplus-0.1.5/swagger_client/models/ta_token_security_response.py`

 * *Files identical despite different names*

### Comparing `goplus-0.1.4/swagger_client/rest.py` & `goplus-0.1.5/swagger_client/rest.py`

 * *Files identical despite different names*


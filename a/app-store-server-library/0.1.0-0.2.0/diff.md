# Comparing `tmp/app-store-server-library-0.1.0.tar.gz` & `tmp/app-store-server-library-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app-store-server-library-0.1.0.tar", last modified: Thu Jun  8 15:16:15 2023, max compression
+gzip compressed data, was "app-store-server-library-0.2.0.tar", last modified: Wed Jul 26 00:37:53 2023, max compression
```

## Comparing `app-store-server-library-0.1.0.tar` & `app-store-server-library-0.2.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 alexbaker   (501) staff       (20)        0 2023-06-08 15:16:15.772448 app-store-server-library-0.1.0/
-drwxr-xr-x   0 alexbaker   (501) staff       (20)        0 2023-06-08 15:16:15.734982 app-store-server-library-0.1.0/App_Store_Server_Library.egg-info/
--rw-r--r--   0 alexbaker   (501) staff       (20)     4988 2023-06-08 15:16:15.000000 app-store-server-library-0.1.0/App_Store_Server_Library.egg-info/PKG-INFO
--rw-r--r--   0 alexbaker   (501) staff       (20)     3490 2023-06-08 15:16:15.000000 app-store-server-library-0.1.0/App_Store_Server_Library.egg-info/SOURCES.txt
--rw-r--r--   0 alexbaker   (501) staff       (20)        1 2023-06-08 15:16:15.000000 app-store-server-library-0.1.0/App_Store_Server_Library.egg-info/dependency_links.txt
--rw-r--r--   0 alexbaker   (501) staff       (20)      124 2023-06-08 15:16:15.000000 app-store-server-library-0.1.0/App_Store_Server_Library.egg-info/requires.txt
--rw-r--r--   0 alexbaker   (501) staff       (20)       28 2023-06-08 15:16:15.000000 app-store-server-library-0.1.0/App_Store_Server_Library.egg-info/top_level.txt
--rw-r--r--   0 alexbaker   (501) staff       (20)     1049 2023-06-03 04:20:29.000000 app-store-server-library-0.1.0/LICENSE.txt
--rw-r--r--   0 alexbaker   (501) staff       (20)       17 2023-06-03 04:20:25.000000 app-store-server-library-0.1.0/MANIFEST.in
--rw-r--r--   0 alexbaker   (501) staff       (20)    37755 2023-06-03 04:20:25.000000 app-store-server-library-0.1.0/NOTICE.txt
--rw-r--r--   0 alexbaker   (501) staff       (20)     4988 2023-06-08 15:16:15.772155 app-store-server-library-0.1.0/PKG-INFO
--rw-r--r--   0 alexbaker   (501) staff       (20)     4763 2023-06-08 15:15:44.000000 app-store-server-library-0.1.0/README.md
-drwxr-xr-x   0 alexbaker   (501) staff       (20)        0 2023-06-08 15:16:15.738757 app-store-server-library-0.1.0/appstoreserverlibrary/
--rw-r--r--   0 alexbaker   (501) staff       (20)        0 2023-06-03 04:20:29.000000 app-store-server-library-0.1.0/appstoreserverlibrary/__init__.py
--rw-r--r--   0 alexbaker   (501) staff       (20)    19163 2023-06-06 20:47:13.000000 app-store-server-library-0.1.0/appstoreserverlibrary/api_client.py
-drwxr-xr-x   0 alexbaker   (501) staff       (20)        0 2023-06-08 15:16:15.770042 app-store-server-library-0.1.0/appstoreserverlibrary/models/
--rw-r--r--   0 alexbaker   (501) staff       (20)      557 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/AccountTenure.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     2965 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/AppTransaction.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      297 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/AutoRenewStatus.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     1077 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/CheckTestNotificationResponse.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     3522 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/ConsumptionRequest.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      399 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/ConsumptionStatus.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     1686 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/Data.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      573 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/DeliveryStatus.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      319 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/Environment.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      416 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/ExpirationIntent.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      397 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/ExtendReasonCode.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     1119 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/ExtendRenewalDateRequest.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     1282 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/ExtendRenewalDateResponse.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      788 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/FirstSendAttemptResult.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     1705 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/HistoryResponse.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      377 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/InAppOwnershipType.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     3933 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/JWSRenewalInfoDecodedPayload.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     6125 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/JWSTransactionDecodedPayload.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     1366 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/LastTransactionsItem.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      844 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/LifetimeDollarsPurchased.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      855 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/LifetimeDollarsRefunded.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     1710 2023-06-06 18:38:32.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/MassExtendRenewalDateRequest.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      643 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/MassExtendRenewalDateResponse.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     1715 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/MassExtendRenewalDateStatusResponse.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     2889 2023-06-06 18:37:13.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/NotificationHistoryRequest.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     1072 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/NotificationHistoryResponse.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     1079 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/NotificationHistoryResponseItem.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      938 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/NotificationTypeV2.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      324 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/OfferType.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      853 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/OrderLookupResponse.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      335 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/OrderLookupStatus.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      321 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/Platform.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      510 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/PlayTime.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      426 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/PriceIncreaseStatus.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     1087 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/RefundHistoryResponse.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      609 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/ResponseBodyV2.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     2451 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/ResponseBodyV2DecodedPayload.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      324 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/RevocationReason.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      941 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/SendAttemptItem.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      771 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/SendAttemptResult.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      574 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/SendTestNotificationResponse.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      345 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/Status.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     1335 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/StatusResponse.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      998 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/SubscriptionGroupIdentifierItem.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      824 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/Subtype.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     2261 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/Summary.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     3043 2023-06-06 18:29:06.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/TransactionHistoryRequest.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      593 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/TransactionInfoResponse.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      440 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/TransactionReason.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      452 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/Type.py
--rw-r--r--   0 alexbaker   (501) staff       (20)      355 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/UserStatus.py
--rw-r--r--   0 alexbaker   (501) staff       (20)        0 2023-06-04 21:45:31.000000 app-store-server-library-0.1.0/appstoreserverlibrary/models/__init__.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     2112 2023-06-03 04:20:29.000000 app-store-server-library-0.1.0/appstoreserverlibrary/promotional_offer.py
--rw-r--r--   0 alexbaker   (501) staff       (20)     4372 2023-06-03 04:20:29.000000 app-store-server-library-0.1.0/appstoreserverlibrary/receipt_utility.py
--rw-r--r--   0 alexbaker   (501) staff       (20)    15166 2023-06-03 04:20:29.000000 app-store-server-library-0.1.0/appstoreserverlibrary/signed_data_verifier.py
--rw-r--r--   0 alexbaker   (501) staff       (20)       38 2023-06-08 15:16:15.772540 app-store-server-library-0.1.0/setup.cfg
--rw-r--r--   0 alexbaker   (501) staff       (20)      750 2023-06-08 15:15:55.000000 app-store-server-library-0.1.0/setup.py
-drwxr-xr-x   0 alexbaker   (501) staff       (20)        0 2023-06-08 15:16:15.771608 app-store-server-library-0.1.0/tests/
--rw-r--r--   0 alexbaker   (501) staff       (20)        0 2023-06-03 04:20:25.000000 app-store-server-library-0.1.0/tests/__init__.py
--rw-r--r--   0 alexbaker   (501) staff       (20)    16754 2023-06-06 19:17:56.000000 app-store-server-library-0.1.0/tests/test_payload_verification.py
--rw-r--r--   0 alexbaker   (501) staff       (20)    12131 2023-06-03 04:20:25.000000 app-store-server-library-0.1.0/tests/test_x509_verifiction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:37:53.196481 app-store-server-library-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    37755 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-26 00:37:53.196481 app-store-server-library-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:37:53.184481 app-store-server-library-0.2.0/app_store_server_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-26 00:37:53.000000 app-store-server-library-0.2.0/app_store_server_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-26 00:37:53.000000 app-store-server-library-0.2.0/app_store_server_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 00:37:53.000000 app-store-server-library-0.2.0/app_store_server_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-26 00:37:53.000000 app-store-server-library-0.2.0/app_store_server_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 00:37:53.000000 app-store-server-library-0.2.0/app_store_server_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:37:53.184481 app-store-server-library-0.2.0/appstoreserverlibrary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19137 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:37:53.196481 app-store-server-library-0.2.0/appstoreserverlibrary/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/AccountTenure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/AppTransaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/AutoRenewStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/CheckTestNotificationResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/ConsumptionRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/ConsumptionStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/DeliveryStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/Environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/ExpirationIntent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/ExtendReasonCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/ExtendRenewalDateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/ExtendRenewalDateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/FirstSendAttemptResult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/HistoryResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/InAppOwnershipType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/JWSRenewalInfoDecodedPayload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/JWSTransactionDecodedPayload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/LastTransactionsItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/LifetimeDollarsPurchased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/LifetimeDollarsRefunded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/MassExtendRenewalDateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/MassExtendRenewalDateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/MassExtendRenewalDateStatusResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/NotificationHistoryRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/NotificationHistoryResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/NotificationHistoryResponseItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/NotificationTypeV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/OfferType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/OrderLookupResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/OrderLookupStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/Platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/PlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/PriceIncreaseStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/RefundHistoryResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/ResponseBodyV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/ResponseBodyV2DecodedPayload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/RevocationReason.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/SendAttemptItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/SendAttemptResult.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/SendTestNotificationResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/Status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/StatusResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/SubscriptionGroupIdentifierItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/Subtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/Summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/TransactionHistoryRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/TransactionInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/TransactionReason.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/Type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/UserStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/promotional_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/receipt_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/appstoreserverlibrary/signed_data_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 00:37:53.196481 app-store-server-library-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:37:53.196481 app-store-server-library-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/tests/test_payload_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-07-26 00:37:41.000000 app-store-server-library-0.2.0/tests/test_x509_verifiction.py
```

### Comparing `app-store-server-library-0.1.0/App_Store_Server_Library.egg-info/PKG-INFO` & `app-store-server-library-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app-store-server-library
-Version: 0.1.0
+Version: 0.2.0
 Summary: The App Store Server Library
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
 # Apple App Store Server Python Library
```

### Comparing `app-store-server-library-0.1.0/App_Store_Server_Library.egg-info/SOURCES.txt` & `app-store-server-library-0.2.0/app_store_server_library.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 NOTICE.txt
 README.md
 setup.py
-App_Store_Server_Library.egg-info/PKG-INFO
-App_Store_Server_Library.egg-info/SOURCES.txt
-App_Store_Server_Library.egg-info/dependency_links.txt
-App_Store_Server_Library.egg-info/requires.txt
-App_Store_Server_Library.egg-info/top_level.txt
 app_store_server_library.egg-info/PKG-INFO
 app_store_server_library.egg-info/SOURCES.txt
 app_store_server_library.egg-info/dependency_links.txt
 app_store_server_library.egg-info/requires.txt
 app_store_server_library.egg-info/top_level.txt
 appstoreserverlibrary/__init__.py
 appstoreserverlibrary/api_client.py
```

### Comparing `app-store-server-library-0.1.0/LICENSE.txt` & `app-store-server-library-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `app-store-server-library-0.1.0/NOTICE.txt` & `app-store-server-library-0.2.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `app-store-server-library-0.1.0/PKG-INFO` & `app-store-server-library-0.2.0/app_store_server_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app-store-server-library
-Version: 0.1.0
+Version: 0.2.0
 Summary: The App Store Server Library
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
 # Apple App Store Server Python Library
```

### Comparing `app-store-server-library-0.1.0/README.md` & `app-store-server-library-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/api_client.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,119 +137,119 @@
                 errorValue = APIError(response_body['errorCode'])
                 raise APIException(response.status_code, errorValue)
             except APIException as e:
                 raise e
             except Exception:
                 raise APIException(response.status_code)
 
-    
+
     def extend_renewal_date_for_all_active_subscribers(self, mass_extend_renewal_date_request: MassExtendRenewalDateRequest) -> MassExtendRenewalDateResponse: 
         """
         Uses a subscription's product identifier to extend the renewal date for all of its eligible active subscribers.
-        
-        :param mass_extend_renewal_date_request The request body for extending a subscription renewal date for all of its active subscribers.
-        :return A response that indicates the server successfully received the subscription-renewal-date extension request.
-        :throws APIException If a response was returned indicating the request could not be processed
         https://developer.apple.com/documentation/appstoreserverapi/extend_subscription_renewal_dates_for_all_active_subscribers
+        
+        :param mass_extend_renewal_date_request: The request body for extending a subscription renewal date for all of its active subscribers.
+        :return: A response that indicates the server successfully received the subscription-renewal-date extension request.
+        :throws APIException: If a response was returned indicating the request could not be processed
         """
         return self._make_request("/inApps/v1/subscriptions/extend/mass/", "POST", {}, mass_extend_renewal_date_request, MassExtendRenewalDateResponse)
 
     def extend_subscription_renewal_date(self, original_transaction_id: str, extend_renewal_date_request: ExtendRenewalDateRequest) -> ExtendRenewalDateResponse:
         """
         Extends the renewal date of a customer's active subscription using the original transaction identifier.
-        
-        :param original_transaction_id    The original transaction identifier of the subscription receiving a renewal date extension.
-        :param extend_renewal_date_request The request body containing subscription-renewal-extension data.
-        :return A response that indicates whether an individual renewal-date extension succeeded, and related details.
-        :throws APIException If a response was returned indicating the request could not be processed
         https://developer.apple.com/documentation/appstoreserverapi/extend_a_subscription_renewal_date
+        
+        :param original_transaction_id:    The original transaction identifier of the subscription receiving a renewal date extension.
+        :param extend_renewal_date_request: The request body containing subscription-renewal-extension data.
+        :return: A response that indicates whether an individual renewal-date extension succeeded, and related details.
+        :throws APIException: If a response was returned indicating the request could not be processed
         """
         return self._make_request("/inApps/v1/subscriptions/extend/" + original_transaction_id, "PUT", {}, extend_renewal_date_request, ExtendRenewalDateResponse)
     
     def get_all_subscription_statuses(self, transaction_id: str, status: List[Status] = None) -> StatusResponse:
         """
         Get the statuses for all of a customer's auto-renewable subscriptions in your app.
-        
-        :param transaction_id The identifier of a transaction that belongs to the customer, and which may be an original transaction identifier.
-        :param status An optional filter that indicates the status of subscriptions to include in the response. Your query may specify more than one status query parameter.
-        :return A response that contains status information for all of a customer's auto-renewable subscriptions in your app.
-        :throws APIException If a response was returned indicating the request could not be processed
         https://developer.apple.com/documentation/appstoreserverapi/get_all_subscription_statuses
+        
+        :param transaction_id: The identifier of a transaction that belongs to the customer, and which may be an original transaction identifier.
+        :param status: An optional filter that indicates the status of subscriptions to include in the response. Your query may specify more than one status query parameter.
+        :return: A response that contains status information for all of a customer's auto-renewable subscriptions in your app.
+        :throws APIException: If a response was returned indicating the request could not be processed
         """
         queryParameters: Dict[str, List[str]] = dict()
         if status != None:
             queryParameters["status"] = [s.value for s in status]
         
         return self._make_request("/inApps/v1/subscriptions/" + transaction_id, "GET", queryParameters, None, StatusResponse)
     
     def get_refund_history(self, transaction_id: str, revision: str) -> RefundHistoryResponse:
         """
         Get a paginated list of all of a customer's refunded in-app purchases for your app.
-        
-        :param transaction_id The identifier of a transaction that belongs to the customer, and which may be an original transaction identifier.
-        :param revision              A token you provide to get the next set of up to 20 transactions. All responses include a revision token. Use the revision token from the previous RefundHistoryResponse.
-        :return A response that contains status information for all of a customer's auto-renewable subscriptions in your app.
-        :throws APIException If a response was returned indicating the request could not be processed
         https://developer.apple.com/documentation/appstoreserverapi/get_refund_history
+
+        :param transaction_id: The identifier of a transaction that belongs to the customer, and which may be an original transaction identifier.
+        :param revision:              A token you provide to get the next set of up to 20 transactions. All responses include a revision token. Use the revision token from the previous RefundHistoryResponse.
+        :return: A response that contains status information for all of a customer's auto-renewable subscriptions in your app.
+        :throws APIException: If a response was returned indicating the request could not be processed
         """
 
         queryParameters: Dict[str, List[str]] = dict()
         if revision != None:
             queryParameters["revision"] = [revision]
         
         return self._make_request("/inApps/v2/refund/lookup/" + transaction_id, "GET", queryParameters, None, RefundHistoryResponse)
     
     def get_status_of_subscription_renewal_date_extensions(self, request_identifier: str, product_id: str) -> MassExtendRenewalDateStatusResponse:
         """
         Checks whether a renewal date extension request completed, and provides the final count of successful or failed extensions.
-        
-        :param request_identifier The UUID that represents your request to the Extend Subscription Renewal Dates for All Active Subscribers endpoint.
-        :param product_id         The product identifier of the auto-renewable subscription that you request a renewal-date extension for.
-        :return A response that indicates the current status of a request to extend the subscription renewal date to all eligible subscribers.
-        :throws APIException If a response was returned indicating the request could not be processed
         https://developer.apple.com/documentation/appstoreserverapi/get_status_of_subscription_renewal_date_extensions
+
+        :param request_identifier: The UUID that represents your request to the Extend Subscription Renewal Dates for All Active Subscribers endpoint.
+        :param product_id:         The product identifier of the auto-renewable subscription that you request a renewal-date extension for.
+        :return: A response that indicates the current status of a request to extend the subscription renewal date to all eligible subscribers.
+        :throws APIException: If a response was returned indicating the request could not be processed
         """
         return self._make_request("/inApps/v1/subscriptions/extend/mass/" + product_id + "/" + request_identifier, "GET", {}, None, MassExtendRenewalDateStatusResponse)
     
     def get_test_notification_status(self, test_notification_token: str) -> CheckTestNotificationResponse:
         """
         Check the status of the test App Store server notification sent to your server.
-        
-        :param test_notification_token The test notification token received from the Request a Test Notification endpoint
-        :return A response that contains the contents of the test notification sent by the App Store server and the result from your server.
-        :throws APIException If a response was returned indicating the request could not be processed
         https://developer.apple.com/documentation/appstoreserverapi/get_test_notification_status
+
+        :param test_notification_token: The test notification token received from the Request a Test Notification endpoint
+        :return: A response that contains the contents of the test notification sent by the App Store server and the result from your server.
+        :throws APIException: If a response was returned indicating the request could not be processed
         """
         return self._make_request("/inApps/v1/notifications/test/" + test_notification_token, "GET", {}, None, CheckTestNotificationResponse)
     
     def get_notification_history(self, pagination_token: str, notification_history_request: NotificationHistoryRequest) -> NotificationHistoryResponse:
         """
         Get a list of notifications that the App Store server attempted to send to your server.
-
-        :param pagination_token An optional token you use to get the next set of up to 20 notification history records. All responses that have more records available include a paginationToken. Omit this parameter the first time you call this endpoint.
-        :param notification_history_request The request body that includes the start and end dates, and optional query constraints.
-        :return A response that contains the App Store Server Notifications history for your app.
-        :throws APIException If a response was returned indicating the request could not be processed
         https://developer.apple.com/documentation/appstoreserverapi/get_notification_history
+
+        :param pagination_token: An optional token you use to get the next set of up to 20 notification history records. All responses that have more records available include a paginationToken. Omit this parameter the first time you call this endpoint.
+        :param notification_history_request: The request body that includes the start and end dates, and optional query constraints.
+        :return: A response that contains the App Store Server Notifications history for your app.
+        :throws APIException: If a response was returned indicating the request could not be processed
         """
         queryParameters: Dict[str, List[str]] = dict()
         if pagination_token != None:
             queryParameters["paginationToken"] = [pagination_token]
         
         return self._make_request("/inApps/v1/notifications/history", "POST", queryParameters, notification_history_request, NotificationHistoryResponse)
 
     def get_transaction_history(self, transaction_id: str, revision: Optional[str], transaction_history_request: TransactionHistoryRequest) -> HistoryResponse:
         """
         Get a customer's in-app purchase transaction history for your app.
-        
-        :param transaction_id The identifier of a transaction that belongs to the customer, and which may be an original transaction identifier.
-        :param revision              A token you provide to get the next set of up to 20 transactions. All responses include a revision token. Note: For requests that use the revision token, include the same query parameters from the initial request. Use the revision token from the previous HistoryResponse.
-        :return A response that contains the customer's transaction history for an app.
-        :throws APIException If a response was returned indicating the request could not be processed
         https://developer.apple.com/documentation/appstoreserverapi/get_transaction_history
+
+        :param transaction_id: The identifier of a transaction that belongs to the customer, and which may be an original transaction identifier.
+        :param revision:              A token you provide to get the next set of up to 20 transactions. All responses include a revision token. Note: For requests that use the revision token, include the same query parameters from the initial request. Use the revision token from the previous HistoryResponse.
+        :return: A response that contains the customer's transaction history for an app.
+        :throws APIException: If a response was returned indicating the request could not be processed
         """
         queryParameters: Dict[str, List[str]] = dict()
         if revision != None:
             queryParameters["revision"] = [revision]
         
         if transaction_history_request.startDate != None:
             queryParameters["startDate"] = [str(transaction_history_request.startDate)]
@@ -276,46 +276,45 @@
             queryParameters["revoked"] = [str(transaction_history_request.revoked)]
         
         return self._make_request("/inApps/v1/history/" + transaction_id, "GET", queryParameters, None, HistoryResponse)
     
     def get_transaction_info(self, transaction_id: str) -> TransactionInfoResponse:
         """
         Get information about a single transaction for your app.
+        https://developer.apple.com/documentation/appstoreserverapi/get_transaction_info
         
         :param transaction_id The identifier of a transaction that belongs to the customer, and which may be an original transaction identifier.
-        :return A response that contains signed transaction information for a single transaction.
-        :throws APIException If a response was returned indicating the request could not be processed
-        https://developer.apple.com/documentation/appstoreserverapi/get_transaction_info
+        :return: A response that contains signed transaction information for a single transaction.
+        :throws APIException: If a response was returned indicating the request could not be processed
         """
         return self._make_request("/inApps/v1/transactions/" + transaction_id, "GET", {}, None, TransactionInfoResponse)
 
     def look_up_order_id(self, order_id: str) -> OrderLookupResponse:
         """
         Get a customer's in-app purchases from a receipt using the order ID.
-        
-        :param order_id The order ID for in-app purchases that belong to the customer.
-        :return A response that includes the order lookup status and an array of signed transactions for the in-app purchases in the order.
-        :throws APIException If a response was returned indicating the request could not be processed
         https://developer.apple.com/documentation/appstoreserverapi/look_up_order_id
+        
+        :param order_id: The order ID for in-app purchases that belong to the customer.
+        :return: A response that includes the order lookup status and an array of signed transactions for the in-app purchases in the order.
+        :throws APIException: If a response was returned indicating the request could not be processed
         """
         return self._make_request("/inApps/v1/lookup/" + order_id, "GET", {}, None, OrderLookupResponse)
     def request_test_notification(self) -> SendTestNotificationResponse:
         """
         Ask App Store Server Notifications to send a test notification to your server.
-        
-        :return A response that contains the test notification token.
-        :throws APIException If a response was returned indicating the request could not be processed
         https://developer.apple.com/documentation/appstoreserverapi/request_a_test_notification
+
+        :return: A response that contains the test notification token.
+        :throws APIException: If a response was returned indicating the request could not be processed
         """
         return self._make_request("/inApps/v1/notifications/test", "POST", {}, None, SendTestNotificationResponse)
-        
+
     def send_consumption_data(self, transaction_id: str, consumption_request: ConsumptionRequest):
         """
         Send consumption information about a consumable in-app purchase to the App Store after your server receives a consumption request notification.
-        
-        :param transaction_id The transaction identifier for which you’re providing consumption information. You receive this identifier in the CONSUMPTION_REQUEST notification the App Store sends to your server.
-        :param consumption_request    The request body containing consumption information.
-        :throws APIException If a response was returned indicating the request could not be processed
         https://developer.apple.com/documentation/appstoreserverapi/send_consumption_information
+
+        :param transaction_id: The transaction identifier for which you're providing consumption information. You receive this identifier in the CONSUMPTION_REQUEST notification the App Store sends to your server.
+        :param consumption_request:    The request body containing consumption information.
+        :raises APIException: If a response was returned indicating the request could not be processed
         """
         self._make_request("/inApps/v1/transactions/consumption/" + transaction_id, "PUT", {}, consumption_request, None)
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/AccountTenure.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/AccountTenure.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/AppTransaction.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/AppTransaction.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,91 +1,92 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional
 
 from attr import define
 import attr
 
 from .Environment import Environment
 
 @define
 class AppTransaction: 
     """
     Information that represents the customer’s purchase of the app, cryptographically signed by the App Store.
     
     https://developer.apple.com/documentation/storekit/apptransaction
     """
 
-    receiptType: Environment = attr.ib(default=None)
+    receiptType: Optional[Environment] = attr.ib(default=None)
     """
     The server environment that signs the app transaction.
     
     https://developer.apple.com/documentation/storekit/apptransaction/3963901-environment
     """
 
-    appAppleId: int = attr.ib(default=None)
+    appAppleId: Optional[int] = attr.ib(default=None)
     """
     The unique identifier the App Store uses to identify the app.
     
     https://developer.apple.com/documentation/storekit/apptransaction/3954436-appid
     """
 
-    bundleId: str = attr.ib(default=None)
+    bundleId: Optional[str] = attr.ib(default=None)
     """
     The bundle identifier that the app transaction applies to.
     
     https://developer.apple.com/documentation/storekit/apptransaction/3954439-bundleid
     """
 
-    applicationVersion: str = attr.ib(default=None)
+    applicationVersion: Optional[str] = attr.ib(default=None)
     """
     The app version that the app transaction applies to.
     
     https://developer.apple.com/documentation/storekit/apptransaction/3954437-appversion
     """
 
-    versionExternalIdentifier: int = attr.ib(default=None)
+    versionExternalIdentifier: Optional[int] = attr.ib(default=None)
     """
     The version external identifier of the app
     
     https://developer.apple.com/documentation/storekit/apptransaction/3954438-appversionid
     """
 
-    receiptCreationDate: int = attr.ib(default=None)
+    receiptCreationDate: Optional[int] = attr.ib(default=None)
     """
     The date that the App Store signed the JWS app transaction.
     
     https://developer.apple.com/documentation/storekit/apptransaction/3954449-signeddate
     """
 
-    originalPurchaseDate: int = attr.ib(default=None)
+    originalPurchaseDate: Optional[int] = attr.ib(default=None)
     """
     The date the user originally purchased the app from the App Store.
     
     https://developer.apple.com/documentation/storekit/apptransaction/3954448-originalpurchasedate
     """
 
-    originalApplicationVersion: str = attr.ib(default=None)
+    originalApplicationVersion: Optional[str] = attr.ib(default=None)
     """
     The app version that the user originally purchased from the App Store.
     
     https://developer.apple.com/documentation/storekit/apptransaction/3954447-originalappversion
     """
 
-    deviceVerification: str = attr.ib(default=None)
+    deviceVerification: Optional[str] = attr.ib(default=None)
     """
     The Base64 device verification value to use to verify whether the app transaction belongs to the device.
     
     https://developer.apple.com/documentation/storekit/apptransaction/3954441-deviceverification
     """
 
-    deviceVerificationNonce: str = attr.ib(default=None)
+    deviceVerificationNonce: Optional[str] = attr.ib(default=None)
     """
     The UUID used to compute the device verification value.
     
     https://developer.apple.com/documentation/storekit/apptransaction/3954442-deviceverificationnonce
     """
 
-    preorderDate: int = attr.ib(default=None)
+    preorderDate: Optional[int] = attr.ib(default=None)
     """
     The date the customer placed an order for the app before it's available in the App Store.
     
     https://developer.apple.com/documentation/storekit/apptransaction/4013175-preorderdate
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/CheckTestNotificationResponse.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/CheckTestNotificationResponse.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import List, Optional
 
 from attr import define
 import attr
 
 from .SendAttemptItem import SendAttemptItem
 
 @define
 class CheckTestNotificationResponse: 
     """
     A response that contains the contents of the test notification sent by the App Store server and the result from your server.
     
     https://developer.apple.com/documentation/appstoreserverapi/checktestnotificationresponse
     """
 
-    signedPayload: str = attr.ib(default=None)
+    signedPayload: Optional[str] = attr.ib(default=None)
     """
     A cryptographically signed payload, in JSON Web Signature (JWS) format, containing the response body for a version 2 notification.
     
     https://developer.apple.com/documentation/appstoreservernotifications/signedpayload
     """
 
-    sendAttempts: "list[SendAttemptItem]" = attr.ib(default=None)
+    sendAttempts: Optional[List[SendAttemptItem]] = attr.ib(default=None)
     """
     An array of information the App Store server records for its attempts to send the TEST notification to your server. The array may contain a maximum of six sendAttemptItem objects.
     
     https://developer.apple.com/documentation/appstoreserverapi/sendattemptitem
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/ConsumptionRequest.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/ConsumptionRequest.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional
 
 from attr import define
 import attr
 from .AccountTenure import AccountTenure
 
 from .ConsumptionStatus import ConsumptionStatus
 from .DeliveryStatus import DeliveryStatus
@@ -16,83 +17,83 @@
 class ConsumptionRequest: 
     """
     The request body containing consumption information.
     
     https://developer.apple.com/documentation/appstoreserverapi/consumptionrequest
     """
 
-    customerConsented: bool = attr.ib(default=None)
+    customerConsented: Optional[bool] = attr.ib(default=None)
     """
     A Boolean value that indicates whether the customer consented to provide consumption data to the App Store.
     
     https://developer.apple.com/documentation/appstoreserverapi/customerconsented
     """
 
-    consumptionStatus: ConsumptionStatus = attr.ib(default=None)
+    consumptionStatus: Optional[ConsumptionStatus] = attr.ib(default=None)
     """
     A value that indicates the extent to which the customer consumed the in-app purchase.
     
     https://developer.apple.com/documentation/appstoreserverapi/consumptionstatus
     """
 
-    platform: Platform = attr.ib(default=None)
+    platform: Optional[Platform] = attr.ib(default=None)
     """
     A value that indicates the platform on which the customer consumed the in-app purchase.
     
     https://developer.apple.com/documentation/appstoreserverapi/platform
     """
 
-    sampleContentProvided: bool = attr.ib(default=None)
+    sampleContentProvided: Optional[bool] = attr.ib(default=None)
     """
     A Boolean value that indicates whether you provided, prior to its purchase, a free sample or trial of the content, or information about its functionality.
     
     https://developer.apple.com/documentation/appstoreserverapi/samplecontentprovided
     """
 
-    deliveryStatus: DeliveryStatus = attr.ib(default=None)
+    deliveryStatus: Optional[DeliveryStatus] = attr.ib(default=None)
     """
     A value that indicates whether the app successfully delivered an in-app purchase that works properly.
     
     https://developer.apple.com/documentation/appstoreserverapi/deliverystatus
     """
 
-    appAccountToken: str = attr.ib(default=None)
+    appAccountToken: Optional[str] = attr.ib(default=None)
     """
     The UUID that an app optionally generates to map a customer's in-app purchase with its resulting App Store transaction.
     
     https://developer.apple.com/documentation/appstoreserverapi/appaccounttoken
     """
 
-    accountTenure: AccountTenure = attr.ib(default=None)
+    accountTenure: Optional[AccountTenure] = attr.ib(default=None)
     """
     The age of the customer's account.
     
     https://developer.apple.com/documentation/appstoreserverapi/accounttenure
     """
 
-    playTime: PlayTime = attr.ib(default=None)
+    playTime: Optional[PlayTime] = attr.ib(default=None)
     """
     A value that indicates the amount of time that the customer used the app.
     
     https://developer.apple.com/documentation/appstoreserverapi/consumptionrequest
     """
 
-    lifetimeDollarsRefunded: LifetimeDollarsRefunded = attr.ib(default=None)
+    lifetimeDollarsRefunded: Optional[LifetimeDollarsRefunded] = attr.ib(default=None)
     """
     A value that indicates the total amount, in USD, of refunds the customer has received, in your app, across all platforms.
     
     https://developer.apple.com/documentation/appstoreserverapi/lifetimedollarsrefunded
     """
 
-    lifetimeDollarsPurchased: LifetimeDollarsPurchased = attr.ib(default=None)
+    lifetimeDollarsPurchased: Optional[LifetimeDollarsPurchased] = attr.ib(default=None)
     """
     A value that indicates the total amount, in USD, of in-app purchases the customer has made in your app, across all platforms.
     
     https://developer.apple.com/documentation/appstoreserverapi/lifetimedollarspurchased
     """
 
-    userStatus: UserStatus = attr.ib(default=None)
+    userStatus: Optional[UserStatus] = attr.ib(default=None)
     """
     The status of the customer's account.
     
     https://developer.apple.com/documentation/appstoreserverapi/userstatus
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/Data.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/Data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional
 
 from attr import define
 import attr
 
 from .Environment import Environment
 
 @define
 class Data: 
     """
     The app metadata and the signed renewal and transaction information.
     
     https://developer.apple.com/documentation/appstoreservernotifications/data
     """
 
-    environment: Environment = attr.ib(default=None)
+    environment: Optional[Environment] = attr.ib(default=None)
     """
     The server environment that the notification applies to, either sandbox or production.
     
     https://developer.apple.com/documentation/appstoreservernotifications/environment
     """
 
-    appAppleId: int = attr.ib(default=None)
+    appAppleId: Optional[int] = attr.ib(default=None)
     """
     The unique identifier of an app in the App Store.
     
     https://developer.apple.com/documentation/appstoreservernotifications/appappleid
     """
 
-    bundleId: str = attr.ib(default=None)
+    bundleId: Optional[str] = attr.ib(default=None)
     """
     The bundle identifier of an app.
     
     https://developer.apple.com/documentation/appstoreserverapi/bundleid
     """
 
-    bundleVersion: str = attr.ib(default=None)
+    bundleVersion: Optional[str] = attr.ib(default=None)
     """
     The version of the build that identifies an iteration of the bundle.
     
     https://developer.apple.com/documentation/appstoreservernotifications/bundleversion
     """
 
-    signedTransactionInfo: str = attr.ib(default=None)
+    signedTransactionInfo: Optional[str] = attr.ib(default=None)
     """
     Transaction information signed by the App Store, in JSON Web Signature (JWS) format.
     
     https://developer.apple.com/documentation/appstoreserverapi/jwstransaction
     """
 
-    signedRenewalInfo: str = attr.ib(default=None)
+    signedRenewalInfo: Optional[str] = attr.ib(default=None)
     """
     Subscription renewal information, signed by the App Store, in JSON Web Signature (JWS) format.
     
     https://developer.apple.com/documentation/appstoreserverapi/jwsrenewalinfo
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/DeliveryStatus.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/DeliveryStatus.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/ExtendRenewalDateRequest.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/ExtendRenewalDateRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional
 
 from attr import define
 import attr
 
 from .ExtendReasonCode import ExtendReasonCode
 
 @define
 class ExtendRenewalDateRequest: 
     """
     The request body that contains subscription-renewal-extension data for an individual subscription.
     
     https://developer.apple.com/documentation/appstoreserverapi/extendrenewaldaterequest
     """
 
-    extendByDays: int = attr.ib(default=None)
+    extendByDays: Optional[int] = attr.ib(default=None)
     """
     The number of days to extend the subscription renewal date.
     
     https://developer.apple.com/documentation/appstoreserverapi/extendbydays
     maximum: 90
     """
 
-    extendReasonCode: ExtendReasonCode = attr.ib(default=None)
+    extendReasonCode: Optional[ExtendReasonCode] = attr.ib(default=None)
     """
     The reason code for the subscription date extension
     
     https://developer.apple.com/documentation/appstoreserverapi/extendreasoncode
     """
 
-    requestIdentifier: str = attr.ib(default=None)
+    requestIdentifier: Optional[str] = attr.ib(default=None)
     """
     A string that contains a unique identifier you provide to track each subscription-renewal-date extension request.
     
     https://developer.apple.com/documentation/appstoreserverapi/requestidentifier
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/ExtendRenewalDateResponse.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/ExtendRenewalDateResponse.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional
 
 from attr import define
 import attr
 
 @define
 class ExtendRenewalDateResponse: 
     """
     A response that indicates whether an individual renewal-date extension succeeded, and related details.
     
     https://developer.apple.com/documentation/appstoreserverapi/extendrenewaldateresponse
     """
 
-    originalTransactionId: str = attr.ib(default=None)
+    originalTransactionId: Optional[str] = attr.ib(default=None)
     """
     The original transaction identifier of a purchase.
     
     https://developer.apple.com/documentation/appstoreserverapi/originaltransactionid
     """
 
-    webOrderLineItemId: str = attr.ib(default=None)
+    webOrderLineItemId: Optional[str] = attr.ib(default=None)
     """
     The unique identifier of subscription-purchase events across devices, including renewals.
     
     https://developer.apple.com/documentation/appstoreserverapi/weborderlineitemid
     """
 
-    success: bool = attr.ib(default=None)
+    success: Optional[bool] = attr.ib(default=None)
     """
     A Boolean value that indicates whether the subscription-renewal-date extension succeeded.
     
     https://developer.apple.com/documentation/appstoreserverapi/success
     """
 
-    effectiveDate: int = attr.ib(default=None)
+    effectiveDate: Optional[int] = attr.ib(default=None)
     """
     The new subscription expiration date for a subscription-renewal extension.
     
     https://developer.apple.com/documentation/appstoreserverapi/effectivedate
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/FirstSendAttemptResult.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/FirstSendAttemptResult.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/HistoryResponse.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/HistoryResponse.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
 
 from attr import define
-from typing import List
+from typing import List, Optional
 import attr
 
 from .Environment import Environment
 
 @define
 class HistoryResponse: 
     """
     A response that contains the customer's transaction history for an app.
     
     https://developer.apple.com/documentation/appstoreserverapi/historyresponse
     """
 
-    revision: str = attr.ib(default=None)
+    revision: Optional[str] = attr.ib(default=None)
     """
     A token you use in a query to request the next set of transactions for the customer.
     
     https://developer.apple.com/documentation/appstoreserverapi/revision
     """
 
-    hasMore: bool = attr.ib(default=None)
+    hasMore: Optional[bool] = attr.ib(default=None)
     """
     A Boolean value indicating whether the App Store has more transaction data.
     
     https://developer.apple.com/documentation/appstoreserverapi/hasmore
     """
 
-    bundleId: str = attr.ib(default=None)
+    bundleId: Optional[str] = attr.ib(default=None)
     """
     The bundle identifier of an app.
     
     https://developer.apple.com/documentation/appstoreserverapi/bundleid
     """
 
-    appAppleId: int = attr.ib(default=None)
+    appAppleId: Optional[int] = attr.ib(default=None)
     """
     The unique identifier of an app in the App Store.
     
     https://developer.apple.com/documentation/appstoreservernotifications/appappleid
     """
 
-    environment: Environment = attr.ib(default=None)
+    environment: Optional[Environment] = attr.ib(default=None)
     """
     The server environment in which you're making the request, whether sandbox or production.
     
     https://developer.apple.com/documentation/appstoreserverapi/environment
     """
 
-    signedTransactions: "List[str]" = attr.ib(default=None)
+    signedTransactions: Optional[List[str]] = attr.ib(default=None)
     """
     An array of in-app purchase transactions for the customer, signed by Apple, in JSON Web Signature format.
     
     https://developer.apple.com/documentation/appstoreserverapi/jwstransaction
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/JWSRenewalInfoDecodedPayload.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/JWSRenewalInfoDecodedPayload.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional
 
 from attr import define
 import attr
 from .AutoRenewStatus import AutoRenewStatus
 from .Environment import Environment
 
 from .ExpirationIntent import ExpirationIntent
@@ -13,104 +14,104 @@
 class JWSRenewalInfoDecodedPayload: 
     """
     A decoded payload containing subscription renewal information for an auto-renewable subscription.
     
     https://developer.apple.com/documentation/appstoreserverapi/jwsrenewalinfodecodedpayload
     """
 
-    expirationIntent: ExpirationIntent = attr.ib(default=None)
+    expirationIntent: Optional[ExpirationIntent] = attr.ib(default=None)
     """
     The reason the subscription expired.
     
     https://developer.apple.com/documentation/appstoreserverapi/expirationintent
     """
 
-    originalTransactionId: str = attr.ib(default=None)
+    originalTransactionId: Optional[str] = attr.ib(default=None)
     """
     The original transaction identifier of a purchase.
     
     https://developer.apple.com/documentation/appstoreserverapi/originaltransactionid
     """
 
-    autoRenewProductId: str = attr.ib(default=None)
+    autoRenewProductId: Optional[str] = attr.ib(default=None)
     """
     The product identifier of the product that will renew at the next billing period.
     
     https://developer.apple.com/documentation/appstoreserverapi/autorenewproductid
     """
 
-    productId: str = attr.ib(default=None)
+    productId: Optional[str] = attr.ib(default=None)
     """
     The unique identifier for the product, that you create in App Store Connect.
     
     https://developer.apple.com/documentation/appstoreserverapi/productid
     """
 
-    autoRenewStatus: AutoRenewStatus = attr.ib(default=None)
+    autoRenewStatus: Optional[AutoRenewStatus] = attr.ib(default=None)
     """
     The renewal status of the auto-renewable subscription.
     
     https://developer.apple.com/documentation/appstoreserverapi/autorenewstatus
     """
 
-    isInBillingRetryPeriod: bool = attr.ib(default=None)
+    isInBillingRetryPeriod: Optional[bool] = attr.ib(default=None)
     """
     A Boolean value that indicates whether the App Store is attempting to automatically renew an expired subscription.
     
     https://developer.apple.com/documentation/appstoreserverapi/isinbillingretryperiod
     """
 
-    priceIncreaseStatus: PriceIncreaseStatus = attr.ib(default=None)
+    priceIncreaseStatus: Optional[PriceIncreaseStatus] = attr.ib(default=None)
     """
     The status that indicates whether the auto-renewable subscription is subject to a price increase.
     
     https://developer.apple.com/documentation/appstoreserverapi/priceincreasestatus
     """
 
-    gracePeriodExpiresDate: int = attr.ib(default=None)
+    gracePeriodExpiresDate: Optional[int] = attr.ib(default=None)
     """
     The time when the billing grace period for subscription renewals expires.
     
     https://developer.apple.com/documentation/appstoreserverapi/graceperiodexpiresdate
     """
 
-    offerType: OfferType = attr.ib(default=None)
+    offerType: Optional[OfferType] = attr.ib(default=None)
     """
     The type of the subscription offer.
     
     https://developer.apple.com/documentation/appstoreserverapi/offertype
     """
 
-    offerIdentifier: str = attr.ib(default=None)
+    offerIdentifier: Optional[str] = attr.ib(default=None)
     """
     The identifier that contains the promo code or the promotional offer identifier.
     
     https://developer.apple.com/documentation/appstoreserverapi/offeridentifier
     """
 
-    signedDate: int = attr.ib(default=None)
+    signedDate: Optional[int] = attr.ib(default=None)
     """
     The UNIX time, in milliseconds, that the App Store signed the JSON Web Signature data.
     
     https://developer.apple.com/documentation/appstoreserverapi/signeddate
     """
 
-    environment: Environment = attr.ib(default=None)
+    environment: Optional[Environment] = attr.ib(default=None)
     """
     The server environment, either sandbox or production.
     
     https://developer.apple.com/documentation/appstoreserverapi/environment
     """
 
-    recentSubscriptionStartDate: int = attr.ib(default=None)
+    recentSubscriptionStartDate: Optional[int] = attr.ib(default=None)
     """
     The earliest start date of a subscription in a series of auto-renewable subscription purchases that ignores all lapses of paid service shorter than 60 days.
     
     https://developer.apple.com/documentation/appstoreserverapi/recentsubscriptionstartdate
     """
 
-    renewalDate: int = attr.ib(default=None)
+    renewalDate: Optional[int] = attr.ib(default=None)
     """
     The UNIX time, in milliseconds, that the most recent auto-renewable subscription purchase expires.
     
     https://developer.apple.com/documentation/appstoreserverapi/renewaldate
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/JWSTransactionDecodedPayload.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/JWSTransactionDecodedPayload.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional
 
 from attr import define
 import attr
 from .Environment import Environment
 from .InAppOwnershipType import InAppOwnershipType
 from .OfferType import OfferType
 from .RevocationReason import RevocationReason
@@ -14,167 +15,167 @@
 class JWSTransactionDecodedPayload: 
     """
     A decoded payload containing transaction information.
     
     https://developer.apple.com/documentation/appstoreserverapi/jwstransactiondecodedpayload
     """
 
-    originalTransactionId: str = attr.ib(default=None)
+    originalTransactionId: Optional[str] = attr.ib(default=None)
     """
     The original transaction identifier of a purchase.
     
     https://developer.apple.com/documentation/appstoreserverapi/originaltransactionid
     """
 
-    transactionId: str = attr.ib(default=None)
+    transactionId: Optional[str] = attr.ib(default=None)
     """
     The unique identifier for a transaction such as an in-app purchase, restored in-app purchase, or subscription renewal.
     
     https://developer.apple.com/documentation/appstoreserverapi/transactionid
     """
 
-    webOrderLineItemId: str = attr.ib(default=None)
+    webOrderLineItemId: Optional[str] = attr.ib(default=None)
     """
     The unique identifier of subscription-purchase events across devices, including renewals.
     
     https://developer.apple.com/documentation/appstoreserverapi/weborderlineitemid
     """
 
-    bundleId: str = attr.ib(default=None)
+    bundleId: Optional[str] = attr.ib(default=None)
     """
     The bundle identifier of an app.
     
     https://developer.apple.com/documentation/appstoreserverapi/bundleid
     """
 
-    productId: str = attr.ib(default=None)
+    productId: Optional[str] = attr.ib(default=None)
     """
     The unique identifier for the product, that you create in App Store Connect.
     
     https://developer.apple.com/documentation/appstoreserverapi/productid
     """    
 
-    subscriptionGroupIdentifier: str = attr.ib(default=None)
+    subscriptionGroupIdentifier: Optional[str] = attr.ib(default=None)
     """
     The identifier of the subscription group that the subscription belongs to.
     
     https://developer.apple.com/documentation/appstoreserverapi/subscriptiongroupidentifier
     """
 
-    purchaseDate: int = attr.ib(default=None)
+    purchaseDate: Optional[int] = attr.ib(default=None)
     """
     The time that the App Store charged the user's account for an in-app purchase, a restored in-app purchase, a subscription, or a subscription renewal after a lapse.
     
     https://developer.apple.com/documentation/appstoreserverapi/purchasedate
     """
 
-    originalPurchaseDate: int = attr.ib(default=None)
+    originalPurchaseDate: Optional[int] = attr.ib(default=None)
     """
     The purchase date of the transaction associated with the original transaction identifier.
     
     https://developer.apple.com/documentation/appstoreserverapi/originalpurchasedate
     """
 
-    expiresDate: int = attr.ib(default=None)
+    expiresDate: Optional[int] = attr.ib(default=None)
     """
     The UNIX time, in milliseconds, an auto-renewable subscription expires or renews.
     
     https://developer.apple.com/documentation/appstoreserverapi/expiresdate
     """
 
-    quantity: int = attr.ib(default=None)
+    quantity: Optional[int] = attr.ib(default=None)
     """
     The number of consumable products purchased.
     
     https://developer.apple.com/documentation/appstoreserverapi/quantity
     """
 
-    type: Type = attr.ib(default=None)
+    type: Optional[Type] = attr.ib(default=None)
     """
     The type of the in-app purchase.
     
     https://developer.apple.com/documentation/appstoreserverapi/type
     """
 
-    appAccountToken: str = attr.ib(default=None)
+    appAccountToken: Optional[str] = attr.ib(default=None)
     """
     The UUID that an app optionally generates to map a customer's in-app purchase with its resulting App Store transaction.
     
     https://developer.apple.com/documentation/appstoreserverapi/appaccounttoken
     """
 
-    inAppOwnershipType: InAppOwnershipType = attr.ib(default=None)
+    inAppOwnershipType: Optional[InAppOwnershipType] = attr.ib(default=None)
     """
     A string that describes whether the transaction was purchased by the user, or is available to them through Family Sharing.
     
     https://developer.apple.com/documentation/appstoreserverapi/inappownershiptype
     """
 
-    signedDate: int = attr.ib(default=None)
+    signedDate: Optional[int] = attr.ib(default=None)
     """
     The UNIX time, in milliseconds, that the App Store signed the JSON Web Signature data.
     
     https://developer.apple.com/documentation/appstoreserverapi/signeddate
     """
 
-    revocationReason: RevocationReason = attr.ib(default=None)
+    revocationReason: Optional[RevocationReason] = attr.ib(default=None)
     """
     The reason that the App Store refunded the transaction or revoked it from family sharing.
     
     https://developer.apple.com/documentation/appstoreserverapi/revocationreason
     """
 
-    revocationDate: int = attr.ib(default=None)
+    revocationDate: Optional[int] = attr.ib(default=None)
     """
     The UNIX time, in milliseconds, that Apple Support refunded a transaction.
     
     https://developer.apple.com/documentation/appstoreserverapi/revocationdate
     """    
 
-    isUpgraded: bool = attr.ib(default=None)
+    isUpgraded: Optional[bool] = attr.ib(default=None)
     """
     The Boolean value that indicates whether the user upgraded to another subscription.
     
     https://developer.apple.com/documentation/appstoreserverapi/isupgraded
     """
 
-    offerType: OfferType = attr.ib(default=None)
+    offerType: Optional[OfferType] = attr.ib(default=None)
     """
     A value that represents the promotional offer type.
     
     https://developer.apple.com/documentation/appstoreserverapi/offertype
     """
 
-    offerIdentifier: str = attr.ib(default=None)
+    offerIdentifier: Optional[str] = attr.ib(default=None)
     """
     The identifier that contains the promo code or the promotional offer identifier.
     
     https://developer.apple.com/documentation/appstoreserverapi/offeridentifier
     """
 
-    environment: Environment = attr.ib(default=None)
+    environment: Optional[Environment] = attr.ib(default=None)
     """
     The server environment, either sandbox or production.
     
     https://developer.apple.com/documentation/appstoreserverapi/environment
     """
 
-    storefront: str = attr.ib(default=None)
+    storefront: Optional[str] = attr.ib(default=None)
     """
     The three-letter code that represents the country or region associated with the App Store storefront for the purchase.
     
     https://developer.apple.com/documentation/appstoreserverapi/storefront
     """
 
-    storefrontId: str = attr.ib(default=None)
+    storefrontId: Optional[str] = attr.ib(default=None)
     """
     An Apple-defined value that uniquely identifies the App Store storefront associated with the purchase.
     
     https://developer.apple.com/documentation/appstoreserverapi/storefrontid
     """
 
-    transactionReason: TransactionReason = attr.ib(default=None)
+    transactionReason: Optional[TransactionReason] = attr.ib(default=None)
     """
     The reason for the purchase transaction, which indicates whether it's a customer's purchase or a renewal for an auto-renewable subscription that the system initates.
     
     https://developer.apple.com/documentation/appstoreserverapi/transactionreason
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/LastTransactionsItem.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/MassExtendRenewalDateRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
 
 from attr import define
+from typing import List, Optional
 import attr
 
-from appstoreserverlibrary.signed_data_verifier import VerificationStatus
+from .ExtendReasonCode import ExtendReasonCode
 
 @define
-class LastTransactionsItem: 
+class MassExtendRenewalDateRequest: 
     """
-    The most recent App Store-signed transaction information and App Store-signed renewal information for an auto-renewable subscription.
+    The request body that contains subscription-renewal-extension data to apply for all eligible active subscribers.
     
-    https://developer.apple.com/documentation/appstoreserverapi/lasttransactionsitem
+    https://developer.apple.com/documentation/appstoreserverapi/massextendrenewaldaterequest
     """
 
-    status: VerificationStatus = attr.ib(default=None)
+    extendByDays: Optional[int] = attr.ib(default=None)
     """
-    The status of the auto-renewable subscription.
+    The number of days to extend the subscription renewal date.
     
-    https://developer.apple.com/documentation/appstoreserverapi/status
+    https://developer.apple.com/documentation/appstoreserverapi/extendbydays
+    maximum: 90
     """
 
-    originalTransactionId: str = attr.ib(default=None)
+    extendReasonCode: Optional[ExtendReasonCode] = attr.ib(default=None)
     """
-    The original transaction identifier of a purchase.
+    The reason code for the subscription-renewal-date extension.
     
-    https://developer.apple.com/documentation/appstoreserverapi/originaltransactionid
+    https://developer.apple.com/documentation/appstoreserverapi/extendreasoncode
+    """    
+
+    requestIdentifier: Optional[str] = attr.ib(default=None)
+    """
+    A string that contains a unique identifier you provide to track each subscription-renewal-date extension request.
+    
+    https://developer.apple.com/documentation/appstoreserverapi/requestidentifier
     """
 
-    signedTransactionInfo: str = attr.ib(default=None)
+    storefrontCountryCodes: Optional[List[str]] = attr.ib(default=None)
     """
-    Transaction information signed by the App Store, in JSON Web Signature (JWS) format.
+    A list of storefront country codes you provide to limit the storefronts for a subscription-renewal-date extension.
     
-    https://developer.apple.com/documentation/appstoreserverapi/jwstransaction
+    https://developer.apple.com/documentation/appstoreserverapi/storefrontcountrycodes
     """
 
-    signedRenewalInfo: str = attr.ib(default=None)
+    productId: Optional[str] = attr.ib(default=None)
     """
-    Subscription renewal information, signed by the App Store, in JSON Web Signature (JWS) format.
+    The unique identifier for the product, that you create in App Store Connect.
     
-    https://developer.apple.com/documentation/appstoreserverapi/jwsrenewalinfo
+    https://developer.apple.com/documentation/appstoreserverapi/productid
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/LifetimeDollarsPurchased.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/LifetimeDollarsPurchased.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/LifetimeDollarsRefunded.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/LifetimeDollarsRefunded.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/MassExtendRenewalDateResponse.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/MassExtendRenewalDateResponse.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional
 
 from attr import define
 import attr
 
 @define
 class MassExtendRenewalDateResponse: 
     """
     A response that indicates the server successfully received the subscription-renewal-date extension request.
     
     https://developer.apple.com/documentation/appstoreserverapi/massextendrenewaldateresponse
     """
 
-    requestIdentifier: str = attr.ib(default=None)
+    requestIdentifier: Optional[str] = attr.ib(default=None)
     """
     A string that contains a unique identifier you provide to track each subscription-renewal-date extension request.
     
     https://developer.apple.com/documentation/appstoreserverapi/requestidentifier
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/MassExtendRenewalDateStatusResponse.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/MassExtendRenewalDateStatusResponse.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional
 
 from attr import define
 import attr
 
 @define
 class MassExtendRenewalDateStatusResponse: 
     """
     A response that indicates the current status of a request to extend the subscription renewal date to all eligible subscribers.
     
     https://developer.apple.com/documentation/appstoreserverapi/massextendrenewaldatestatusresponse
     """
 
-    requestIdentifier: str = attr.ib(default=None)
+    requestIdentifier: Optional[str] = attr.ib(default=None)
     """
     A string that contains a unique identifier you provide to track each subscription-renewal-date extension request.
     
     https://developer.apple.com/documentation/appstoreserverapi/requestidentifier
     """
 
-    complete: bool = attr.ib(default=None)
+    complete: Optional[bool] = attr.ib(default=None)
     """
     A Boolean value that indicates whether the App Store completed the request to extend a subscription renewal date to active subscribers.
     
     https://developer.apple.com/documentation/appstoreserverapi/complete
     """
 
-    completeDate: int = attr.ib(default=None)
+    completeDate: Optional[int] = attr.ib(default=None)
     """
     The UNIX time, in milliseconds, that the App Store completes a request to extend a subscription renewal date for eligible subscribers.
     
     https://developer.apple.com/documentation/appstoreserverapi/completedate
     """
 
-    succeededCount: int = attr.ib(default=None)
+    succeededCount: Optional[int] = attr.ib(default=None)
     """
     The count of subscriptions that successfully receive a subscription-renewal-date extension.
     
     https://developer.apple.com/documentation/appstoreserverapi/succeededcount
     """
 
-    failedCount: int = attr.ib(default=None)
+    failedCount: Optional[int] = attr.ib(default=None)
     """
     The count of subscriptions that fail to receive a subscription-renewal-date extension.
     
     https://developer.apple.com/documentation/appstoreserverapi/failedcount
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/NotificationHistoryRequest.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/NotificationHistoryRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 class NotificationHistoryRequest: 
     """
     The request body for notification history.
     
     https://developer.apple.com/documentation/appstoreserverapi/notificationhistoryrequest
     """
 
-    startDate: int = attr.ib(default=None)
+    startDate: Optional[int] = attr.ib(default=None)
     """
     The start date of the timespan for the requested App Store Server Notification history records. The startDate needs to precede the endDate. Choose a startDate that's within the past 180 days from the current date.
     
     https://developer.apple.com/documentation/appstoreserverapi/startdate
     """
 
-    endDate: int = attr.ib(default=None)
+    endDate: Optional[int] = attr.ib(default=None)
     """
     The end date of the timespan for the requested App Store Server Notification history records. Choose an endDate that's later than the startDate. If you choose an endDate in the future, the endpoint automatically uses the current date as the endDate.
     
     https://developer.apple.com/documentation/appstoreserverapi/enddate
     """
 
     notificationType: Optional[NotificationTypeV2] = attr.ib(default=None)
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/NotificationHistoryResponse.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/NotificationHistoryResponse.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional, List
 
 from attr import define
 import attr
 
 from .NotificationHistoryResponseItem import NotificationHistoryResponseItem
 
 @define
 class NotificationHistoryResponse: 
     """
     A response that contains the App Store Server Notifications history for your app.
     
     https://developer.apple.com/documentation/appstoreserverapi/notificationhistoryresponse
     """
 
-    paginationToken: str = attr.ib(default=None)
+    paginationToken: Optional[str] = attr.ib(default=None)
     """
     A pagination token that you return to the endpoint on a subsequent call to receive the next set of results.
     
     https://developer.apple.com/documentation/appstoreserverapi/paginationtoken
     """
 
-    hasMore: bool = attr.ib(default=None)
+    hasMore: Optional[bool] = attr.ib(default=None)
     """
     A Boolean value indicating whether the App Store has more transaction data.
     
     https://developer.apple.com/documentation/appstoreserverapi/hasmore
     """
 
-    notificationHistory: "list[NotificationHistoryResponseItem]" = attr.ib(default=None)
+    notificationHistory: Optional[List[NotificationHistoryResponseItem]] = attr.ib(default=None)
     """
     An array of App Store server notification history records.
     
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/NotificationHistoryResponseItem.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/NotificationHistoryResponseItem.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional, List
 
 from attr import define
 import attr
 
 from .SendAttemptItem import SendAttemptItem
 
 @define
 class NotificationHistoryResponseItem: 
     """
     The App Store server notification history record, including the signed notification payload and the result of the server's first send attempt.
     
     https://developer.apple.com/documentation/appstoreserverapi/notificationhistoryresponseitem
     """
 
-    signedPayload: str = attr.ib(default=None)
+    signedPayload: Optional[str] = attr.ib(default=None)
     """
     A cryptographically signed payload, in JSON Web Signature (JWS) format, containing the response body for a version 2 notification.
     
     https://developer.apple.com/documentation/appstoreservernotifications/signedpayload
     """
 
-    sendAttempts: "list[SendAttemptItem]" = attr.ib(default=None)
+    sendAttempts: Optional[List[SendAttemptItem]] = attr.ib(default=None)
     """
     An array of information the App Store server records for its attempts to send a notification to your server. The maximum number of entries in the array is six.
     
     https://developer.apple.com/documentation/appstoreserverapi/sendattemptitem
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/NotificationTypeV2.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/NotificationTypeV2.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/OrderLookupResponse.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/OrderLookupResponse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
 
 from attr import define
-from typing import List
+from typing import List, Optional
 import attr
 
 from .OrderLookupStatus import OrderLookupStatus
 
 @define
 class OrderLookupResponse: 
     """
     A response that includes the order lookup status and an array of signed transactions for the in-app purchases in the order.
     
     https://developer.apple.com/documentation/appstoreserverapi/orderlookupresponse
     """
 
-    status: OrderLookupStatus = attr.ib(default=None)
+    status: Optional[OrderLookupStatus] = attr.ib(default=None)
     """
     The status that indicates whether the order ID is valid.
     
     https://developer.apple.com/documentation/appstoreserverapi/orderlookupstatus
     """
 
-    signedTransactions: "List[str]" = attr.ib(default=None)
+    signedTransactions: Optional[List[str]] = attr.ib(default=None)
     """
     An array of in-app purchase transactions that are part of order, signed by Apple, in JSON Web Signature format.
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/RefundHistoryResponse.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/RefundHistoryResponse.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
 
 from attr import define
-from typing import List
+from typing import List, Optional
 import attr
 
 @define
 class RefundHistoryResponse: 
     """
     A response that contains an array of signed JSON Web Signature (JWS) refunded transactions, and paging information.
     
     https://developer.apple.com/documentation/appstoreserverapi/refundhistoryresponse
     """
 
-    signedTransactions: "List[str]" = attr.ib(default=None)
+    signedTransactions: Optional[List[str]] = attr.ib(default=None)
     """
     A list of up to 20 JWS transactions, or an empty array if the customer hasn't received any refunds in your app. The transactions are sorted in ascending order by revocationDate.
     """
 
-    revision: str = attr.ib(default=None)
+    revision: Optional[str] = attr.ib(default=None)
     """
     A token you use in a query to request the next set of transactions for the customer.
     
     https://developer.apple.com/documentation/appstoreserverapi/revision
     """
 
-    hasMore: bool = attr.ib(default=None)
+    hasMore: Optional[bool] = attr.ib(default=None)
     """
     A Boolean value indicating whether the App Store has more transaction data.
     
     https://developer.apple.com/documentation/appstoreserverapi/hasmore
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/ResponseBodyV2.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/ResponseBodyV2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional
 
 from attr import define
 import attr
 
 @define
 class ResponseBodyV2:
     """
     The response body the App Store sends in a version 2 server notification.
 
     https://developer.apple.com/documentation/appstoreservernotifications/responsebodyv2
     """
      
-    signedPayload: str = attr.ib(default=None)
+    signedPayload: Optional[str] = attr.ib(default=None)
     """
     A cryptographically signed payload, in JSON Web Signature (JWS) format, containing the response body for a version 2 notification.
     
     https://developer.apple.com/documentation/appstoreservernotifications/signedpayload
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/ResponseBodyV2DecodedPayload.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/ResponseBodyV2DecodedPayload.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional
 
 from attr import define
 import attr
 from .Data import Data
 
 from .NotificationTypeV2 import NotificationTypeV2
 from .Subtype import Subtype
@@ -13,57 +14,57 @@
 class ResponseBodyV2DecodedPayload: 
     """
     A decoded payload containing the version 2 notification data.
     
     https://developer.apple.com/documentation/appstoreservernotifications/responsebodyv2decodedpayload
     """
 
-    notificationType: NotificationTypeV2 = attr.ib(default=None)
+    notificationType: Optional[NotificationTypeV2] = attr.ib(default=None)
     """
     The in-app purchase event for which the App Store sends this version 2 notification.
     
     https://developer.apple.com/documentation/appstoreservernotifications/notificationtype
     """
 
-    subtype: Subtype = attr.ib(default=None)
+    subtype: Optional[Subtype] = attr.ib(default=None)
     """
     Additional information that identifies the notification event. The subtype field is present only for specific version 2 notifications.
     
     https://developer.apple.com/documentation/appstoreservernotifications/subtype
     """
 
-    notificationUUID: str = attr.ib(default=None)
+    notificationUUID: Optional[str] = attr.ib(default=None)
     """
     A unique identifier for the notification.
     
     https://developer.apple.com/documentation/appstoreservernotifications/notificationuuid
     """
 
-    data: Data = attr.ib(default=None)
+    data: Optional[Data] = attr.ib(default=None)
     """
     The object that contains the app metadata and signed renewal and transaction information.
     The data and summary fields are mutually exclusive. The payload contains one of the fields, but not both.
     
     https://developer.apple.com/documentation/appstoreservernotifications/data
     """
 
-    version: str = attr.ib(default=None)
+    version: Optional[str] = attr.ib(default=None)
     """
     A string that indicates the notification's App Store Server Notifications version number.
     
     https://developer.apple.com/documentation/appstoreservernotifications/version
     """
 
-    signedDate: int = attr.ib(default=None)
+    signedDate: Optional[int] = attr.ib(default=None)
     """
     The UNIX time, in milliseconds, that the App Store signed the JSON Web Signature data.
     
     https://developer.apple.com/documentation/appstoreserverapi/signeddate
     """
 
-    summary: Summary = attr.ib(default=None)
+    summary: Optional[Summary] = attr.ib(default=None)
     """
     The summary data that appears when the App Store server completes your request to extend a subscription renewal date for eligible subscribers.
     The data and summary fields are mutually exclusive. The payload contains one of the fields, but not both.
     
     https://developer.apple.com/documentation/appstoreservernotifications/summary
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/SendAttemptItem.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/SendAttemptItem.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional
 
 from attr import define
 import attr
 
 from .SendAttemptResult import SendAttemptResult
 
 @define
 class SendAttemptItem: 
     """
     The success or error information and the date the App Store server records when it attempts to send a server notification to your server.
     
     https://developer.apple.com/documentation/appstoreserverapi/sendattemptitem
     """
 
-    attemptDate: int = attr.ib(default=None)
+    attemptDate: Optional[int] = attr.ib(default=None)
     """
     The date the App Store server attempts to send a notification.
     
     https://developer.apple.com/documentation/appstoreserverapi/attemptdate
     """
 
-    sendAttemptResult: SendAttemptResult = attr.ib(default=None)
+    sendAttemptResult: Optional[SendAttemptResult] = attr.ib(default=None)
     """
     The success or error information the App Store server records when it attempts to send an App Store server notification to your server.
     
     https://developer.apple.com/documentation/appstoreserverapi/sendattemptresult
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/SendAttemptResult.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/SendAttemptResult.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/SendTestNotificationResponse.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/SendTestNotificationResponse.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional
 
 from attr import define
 import attr
 
 @define
 class SendTestNotificationResponse: 
     """
     A response that contains the test notification token.
     
     https://developer.apple.com/documentation/appstoreserverapi/sendtestnotificationresponse
     """
 
-    testNotificationToken: str = attr.ib(default=None)
+    testNotificationToken: Optional[str] = attr.ib(default=None)
     """
     A unique identifier for a notification test that the App Store server sends to your server.
     
     https://developer.apple.com/documentation/appstoreserverapi/testnotificationtoken
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/StatusResponse.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/StatusResponse.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional, List
 
 from attr import define
 import attr
 from .Environment import Environment
 from .SubscriptionGroupIdentifierItem import SubscriptionGroupIdentifierItem
 
 @define
 class StatusResponse: 
     """
     A response that contains status information for all of a customer's auto-renewable subscriptions in your app.
     
     https://developer.apple.com/documentation/appstoreserverapi/statusresponse
     """
 
-    environment: Environment = attr.ib(default=None)
+    environment: Optional[Environment] = attr.ib(default=None)
     """
     The server environment, sandbox or production, in which the App Store generated the response.
     
     https://developer.apple.com/documentation/appstoreserverapi/environment
     """
 
-    bundleId: str = attr.ib(default=None)
+    bundleId: Optional[str] = attr.ib(default=None)
     """
     The bundle identifier of an app.
     
     https://developer.apple.com/documentation/appstoreserverapi/bundleid
     """
 
-    appAppleId: int = attr.ib(default=None)
+    appAppleId: Optional[int] = attr.ib(default=None)
     """
     The unique identifier of an app in the App Store.
     
     https://developer.apple.com/documentation/appstoreservernotifications/appappleid
     """
 
-    data: "list[SubscriptionGroupIdentifierItem]" = attr.ib(default=None)
+    data: Optional[List[SubscriptionGroupIdentifierItem]] = attr.ib(default=None)
     """
     An array of information for auto-renewable subscriptions, including App Store-signed transaction information and App Store-signed renewal information.
     
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/SubscriptionGroupIdentifierItem.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/SubscriptionGroupIdentifierItem.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional, List
 
 from attr import define
 import attr
 
 from .LastTransactionsItem import LastTransactionsItem
 
 @define
 class SubscriptionGroupIdentifierItem: 
     """
     Information for auto-renewable subscriptions, including signed transaction information and signed renewal information, for one subscription group.
     
     https://developer.apple.com/documentation/appstoreserverapi/subscriptiongroupidentifieritem
     """
 
-    subscriptionGroupIdentifier: str = attr.ib(default=None)
+    subscriptionGroupIdentifier: Optional[str] = attr.ib(default=None)
     """
     The identifier of the subscription group that the subscription belongs to.
     
     https://developer.apple.com/documentation/appstoreserverapi/subscriptiongroupidentifier
     """    
 
-    lastTransactions: "list[LastTransactionsItem]" = attr.ib(default=None)
+    lastTransactions: Optional[List[LastTransactionsItem]] = attr.ib(default=None)
     """
     An array of the most recent App Store-signed transaction information and App Store-signed renewal information for all auto-renewable subscriptions in the subscription group.
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/Subtype.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/Subtype.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/Summary.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/Summary.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
 
 from attr import define
-from typing import List
+from typing import List, Optional
 import attr
 from .Environment import Environment
 
 @define
 class Summary: 
     """
     The payload data for a subscription-renewal-date extension notification.
     
     https://developer.apple.com/documentation/appstoreservernotifications/summary
     """
 
-    environment: Environment = attr.ib(default=None)
+    environment: Optional[Environment] = attr.ib(default=None)
     """
     The server environment that the notification applies to, either sandbox or production.
     
     https://developer.apple.com/documentation/appstoreservernotifications/environment
     """
 
-    appAppleId: int = attr.ib(default=None)
+    appAppleId: Optional[int] = attr.ib(default=None)
     """
     The unique identifier of an app in the App Store.
     
     https://developer.apple.com/documentation/appstoreservernotifications/appappleid
     """
 
-    bundleId: str = attr.ib(default=None)
+    bundleId: Optional[str] = attr.ib(default=None)
     """
     The bundle identifier of an app.
     
     https://developer.apple.com/documentation/appstoreserverapi/bundleid
     """
 
-    productId: str = attr.ib(default=None)
+    productId: Optional[str] = attr.ib(default=None)
     """
     The unique identifier for the product, that you create in App Store Connect.
     
     https://developer.apple.com/documentation/appstoreserverapi/productid
     """    
 
-    requestIdentifier: str = attr.ib(default=None)
+    requestIdentifier: Optional[str] = attr.ib(default=None)
     """
     A string that contains a unique identifier you provide to track each subscription-renewal-date extension request.
     
     https://developer.apple.com/documentation/appstoreserverapi/requestidentifier
     """
 
-    storefrontCountryCodes: "List[str]" = attr.ib(default=None)
+    storefrontCountryCodes: Optional[List[str]] = attr.ib(default=None)
     """
     A list of storefront country codes you provide to limit the storefronts for a subscription-renewal-date extension.
     
     https://developer.apple.com/documentation/appstoreserverapi/storefrontcountrycodes
     """
 
-    succeededCount: int = attr.ib(default=None)
+    succeededCount: Optional[int] = attr.ib(default=None)
     """
     The count of subscriptions that successfully receive a subscription-renewal-date extension.
     
     https://developer.apple.com/documentation/appstoreserverapi/succeededcount
     """
 
-    failedCount: int = attr.ib(default=None)
+    failedCount: Optional[int] = attr.ib(default=None)
     """
     The count of subscriptions that fail to receive a subscription-renewal-date extension.
     
     https://developer.apple.com/documentation/appstoreserverapi/failedcount
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/TransactionHistoryRequest.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/TransactionHistoryRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
 
 from enum import Enum
-from typing import List
+from typing import List, Optional
 import attr
 
 
 from .InAppOwnershipType import InAppOwnershipType
 
 class ProductType(Enum):
     AUTO_RENEWABLE = "AUTO_RENEWABLE"
@@ -15,56 +15,56 @@
 
 class Order(Enum):
     ASCENDING = "ASCENDING"
     DESCENDING = "DESCENDING"
 
 @attr.define
 class TransactionHistoryRequest:
-    startDate: int = attr.ib(default=None)
+    startDate: Optional[int] = attr.ib(default=None)
     """
     An optional start date of the timespan for the transaction history records you're requesting. The startDate must precede the endDate if you specify both dates. To be included in results, the transaction's purchaseDate must be equal to or greater than the startDate.
     
     https://developer.apple.com/documentation/appstoreserverapi/startdate
     """
     
-    endDate: int = attr.ib(default=None)
+    endDate: Optional[int] = attr.ib(default=None)
     """
     An optional end date of the timespan for the transaction history records you're requesting. Choose an endDate that's later than the startDate if you specify both dates. Using an endDate in the future is valid. To be included in results, the transaction's purchaseDate must be less than the endDate.
     
     https://developer.apple.com/documentation/appstoreserverapi/enddate
     """
 
-    productIds: "List[str]" = attr.ib(default=None)
+    productIds: Optional[List[str]] = attr.ib(default=None)
     """
     An optional filter that indicates the product identifier to include in the transaction history. Your query may specify more than one productID.
     
     https://developer.apple.com/documentation/appstoreserverapi/productid
     """    
 
-    productTypes: "List[ProductType]" = attr.ib(default=None)
+    productTypes: Optional[List[ProductType]] = attr.ib(default=None)
     """
     An optional filter that indicates the product type to include in the transaction history. Your query may specify more than one productType.
     """
     
-    sort: Order = attr.ib(default=None)
+    sort: Optional[Order] = attr.ib(default=None)
     """
     An optional sort order for the transaction history records. The response sorts the transaction records by their recently modified date. The default value is ASCENDING, so you receive the oldest records first.
     """
 
-    subscriptionGroupIdentifiers: "list[str]" = attr.ib(default=None)
+    subscriptionGroupIdentifiers: Optional[List[str]] = attr.ib(default=None)
     """
     An optional filter that indicates the subscription group identifier to include in the transaction history. Your query may specify more than one subscriptionGroupIdentifier.
     
     https://developer.apple.com/documentation/appstoreserverapi/subscriptiongroupidentifier
     """
 
-    inAppOwnershipType: InAppOwnershipType = attr.ib(default=None)
+    inAppOwnershipType: Optional[InAppOwnershipType] = attr.ib(default=None)
     """
     An optional filter that limits the transaction history by the in-app ownership type.
     
     https://developer.apple.com/documentation/appstoreserverapi/inappownershiptype
     """
    
-    revoked: bool = attr.ib(default=None)
+    revoked: Optional[bool] = attr.ib(default=None)
     """
     An optional Boolean value that indicates whether the response includes only revoked transactions when the value is true, or contains only nonrevoked transactions when the value is false. By default, the request doesn't include this parameter.
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/models/TransactionInfoResponse.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/models/TransactionInfoResponse.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright (c) 2023 Apple Inc. Licensed under MIT License.
+from typing import Optional
 
 from attr import define
 import attr
 
 @define
 class TransactionInfoResponse:
     """
     A response that contains signed transaction information for a single transaction.
     
     https://developer.apple.com/documentation/appstoreserverapi/transactioninforesponse
     """
     
-    signedTransactionInfo: str = attr.ib(default=None)
+    signedTransactionInfo: Optional[str] = attr.ib(default=None)
     """
     A customer’s in-app purchase transaction, signed by Apple, in JSON Web Signature (JWS) format.
     
     https://developer.apple.com/documentation/appstoreserverapi/jwstransaction
     """
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/promotional_offer.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/promotional_offer.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
        self._bundle_id = bundle_id
     def create_signature(self, product_identifier: str, subscription_offer_id: str, application_username: str, nonce: uuid, timestamp: int):
         """
         Return the Base64 encoded signature
 
         https://developer.apple.com/documentation/storekit/in-app_purchase/original_api_for_in-app_purchase/subscriptions_and_offers/generating_a_signature_for_promotional_offers
 
-        :param product_identifier The subscription product identifier
-        :param subscription_offer_id The subscription discount identifier
-        :param application_username An optional string value that you define; may be an empty string
-        :param nonce A one-time UUID value that your server generates. Generate a new nonce for every signature.
-        :param timestamp A timestamp your server generates in UNIX time format, in milliseconds. The timestamp keeps the offer active for 24 hours.
-        :return The Base64 encoded signature
+        :param product_identifier: The subscription product identifier
+        :param subscription_offer_id: The subscription discount identifier
+        :param application_username: An optional string value that you define; may be an empty string
+        :param nonce: A one-time UUID value that your server generates. Generate a new nonce for every signature.
+        :param timestamp: A timestamp your server generates in UNIX time format, in milliseconds. The timestamp keeps the offer active for 24 hours.
+        :return: The Base64 encoded signature
         """
         payload = self._bundle_id + '\u2063' + \
             self._key_id + '\u2063' + \
             product_identifier + '\u2063' + \
             subscription_offer_id + '\u2063' + \
             application_username.lower()  + '\u2063'+ \
             str(nonce).lower() + '\u2063' + \
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/receipt_utility.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/receipt_utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 class ReceiptUtility:
     def extract_transaction_id_from_app_receipt(self, app_receipt: str) -> Optional[str]:
         """
         Extracts a transaction id from an encoded App Receipt. Throws if the receipt does not match the expected format.
         *NO validation* is performed on the receipt, and any data returned should only be used to call the App Store Server API.
 
-        :param appReceipt The unmodified app receipt
-        :returns A transaction id from the array of in-app purchases, null if the receipt contains no in-app purchases
+        :param appReceipt: The unmodified app receipt
+        :return: A transaction id from the array of in-app purchases, null if the receipt contains no in-app purchases
         """
         decoder = asn1.Decoder()
         decoder.start(b64decode(app_receipt, validate=True))
         tag = decoder.peek()
         if tag.typ != asn1.Types.Constructed or tag.nr != asn1.Numbers.Sequence:
             raise ValueError()
         decoder.enter()
@@ -78,16 +78,16 @@
             decoder.leave()
         return None
     
     def extract_transaction_id_from_transaction_receipt(self, transaction_receipt: str) -> Optional[str]:
         """
         Extracts a transaction id from an encoded transactional receipt. Throws if the receipt does not match the expected format.
         *NO validation* is performed on the receipt, and any data returned should only be used to call the App Store Server API.
-        :param transactionReceipt The unmodified transactionReceipt
-        :returns A transaction id, or null if no transactionId is found in the receipt
+        :param transactionReceipt: The unmodified transactionReceipt
+        :return: A transaction id, or null if no transactionId is found in the receipt
         """
         decoded_top_level = base64.b64decode(transaction_receipt).decode('utf-8')
         matching_result = re.search('"purchase-info"\s+=\s+"([a-zA-Z0-9+/=]+)";', decoded_top_level)
         if matching_result:
             decoded_inner_level = base64.b64decode(matching_result.group(1)).decode('utf-8')
             inner_matching_result = re.search('"transaction-id"\s+=\s+"([a-zA-Z0-9+/=]+)";', decoded_inner_level)
             if inner_matching_result:
```

### Comparing `app-store-server-library-0.1.0/appstoreserverlibrary/signed_data_verifier.py` & `app-store-server-library-0.2.0/appstoreserverlibrary/signed_data_verifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,42 +43,42 @@
         self._app_apple_id = app_apple_id
         self._enable_online_checks = enable_online_checks
 
     def verify_and_decode_renewal_info(self, signed_renewal_info: str) -> JWSRenewalInfoDecodedPayload:
         """
         Verifies and decodes a signedRenewalInfo obtained from the App Store Server API, an App Store Server Notification, or from a device
 
-        :param signed_renewal_info The signedRenewalInfo field
-        :return The decoded renewal info after verification
-        :throws VerificationException Thrown if the data could not be verified
+        :param signed_renewal_info: The signedRenewalInfo field
+        :return: The decoded renewal info after verification
+        :throws VerificationException: Thrown if the data could not be verified
         """
         return cattrs.structure(self._decode_signed_object(signed_renewal_info), JWSRenewalInfoDecodedPayload)
 
     def verify_and_decode_signed_transaction(self, signed_transaction: str) -> JWSTransactionDecodedPayload:
         """
         Verifies and decodes a signedTransaction obtained from the App Store Server API, an App Store Server Notification, or from a device
 
-        :param signed_transaction The signedRenewalInfo field
-        :return The decoded transaction info after verification
-        :throws VerificationException Thrown if the data could not be verified
+        :param signed_transaction: The signedRenewalInfo field
+        :return: The decoded transaction info after verification
+        :throws VerificationException: Thrown if the data could not be verified
         """
         decoded_transaction_info = cattrs.structure(self._decode_signed_object(signed_transaction), JWSTransactionDecodedPayload)
         if decoded_transaction_info.bundleId != self._bundle_id:
             raise VerificationException(VerificationStatus.INVALID_APP_IDENTIFIER)
         if decoded_transaction_info.environment != self._environment:
             raise VerificationException(VerificationStatus.INVALID_ENVIRONMENT)
         return decoded_transaction_info
 
     def verify_and_decode_notification(self, signed_payload: str) -> ResponseBodyV2DecodedPayload:
         """
         Verifies and decodes an App Store Server Notification signedPayload
 
-        :param signedPayload The payload received by your server
-        :return The decoded payload after verification
-        :throws VerificationException Thrown if the data could not be verified
+        :param signedPayload: The payload received by your server
+        :return: The decoded payload after verification
+        :throws VerificationException: Thrown if the data could not be verified
         """
         decoded_dict = self._decode_signed_object(signed_payload)
         decoded_signed_notification = cattrs.structure(decoded_dict, ResponseBodyV2DecodedPayload)
         bundle_id = None
         app_apple_id = None
         environment = None
         if decoded_signed_notification.data:
@@ -95,17 +95,17 @@
             raise VerificationException(VerificationStatus.INVALID_ENVIRONMENT)
         return decoded_signed_notification
 
     def verify_and_decode_app_transaction(self, signed_app_transaction: str) -> AppTransaction:
         """
         Verifies and decodes a signed AppTransaction
 
-        :param signed_app_transaction The signed AppTransaction
-        :return The decoded AppTransaction after validation
-        :throws VerificationException Thrown if the data could not be verified
+        :param signed_app_transaction: The signed AppTransaction
+        :return: The decoded AppTransaction after validation
+        :throws VerificationException: Thrown if the data could not be verified
         """
         decoded_dict = self._decode_signed_object(signed_app_transaction)
         decoded_app_transaction = cattrs.structure(decoded_dict, AppTransaction)
         environment = decoded_app_transaction.receiptType
         if decoded_app_transaction.bundleId != self._bundle_id or (self._environment == Environment.PRODUCTION and decoded_app_transaction.appAppleId != self._app_apple_id):
             raise VerificationException(VerificationStatus.INVALID_APP_IDENTIFIER)
         if environment != self._environment:
```

### Comparing `app-store-server-library-0.1.0/setup.py` & `app-store-server-library-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="app-store-server-library",
-    version="0.1.0",
+    version="0.2.0",
     description="The App Store Server Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     python_requires=">=3.7, <4",
     install_requires=["attrs >= 21.3.0", 'PyJWT >= 2.6.0, < 3', 'requests >= 2.28.0, < 3', 'cryptography >= 40.0.0, < 42', 'pyOpenSSL >= 23.1.1, < 24', 'asn1==2.7.0', 'cattrs==23.1.2'],
     package_data={"appstoreserverlibrary": ["py.typed"]},
```

### Comparing `app-store-server-library-0.1.0/tests/test_payload_verification.py` & `app-store-server-library-0.2.0/tests/test_payload_verification.py`

 * *Files identical despite different names*

### Comparing `app-store-server-library-0.1.0/tests/test_x509_verifiction.py` & `app-store-server-library-0.2.0/tests/test_x509_verifiction.py`

 * *Files identical despite different names*


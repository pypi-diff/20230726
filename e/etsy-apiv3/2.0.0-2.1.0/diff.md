# Comparing `tmp/etsy-apiv3-2.0.0.tar.gz` & `tmp/etsy-apiv3-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etsy-apiv3-2.0.0.tar", last modified: Wed Jul 19 15:41:29 2023, max compression
+gzip compressed data, was "etsy-apiv3-2.1.0.tar", last modified: Wed Jul 26 11:39:22 2023, max compression
```

## Comparing `etsy-apiv3-2.0.0.tar` & `etsy-apiv3-2.1.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 15:41:29.289707 etsy-apiv3-2.0.0/
--rw-rw-rw-   0        0        0     1089 2022-11-29 15:57:22.000000 etsy-apiv3-2.0.0/LICENSE
--rw-rw-rw-   0        0        0      342 2023-07-19 15:41:29.289707 etsy-apiv3-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1120 2022-12-02 14:38:46.000000 etsy-apiv3-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 15:41:29.199039 etsy-apiv3-2.0.0/etsy_apiv3/
--rw-rw-rw-   0        0        0       23 2023-07-19 15:41:23.000000 etsy-apiv3-2.0.0/etsy_apiv3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 15:41:29.217133 etsy-apiv3-2.0.0/etsy_apiv3/exceptions/
--rw-rw-rw-   0        0        0      549 2023-05-15 08:29:30.000000 etsy-apiv3-2.0.0/etsy_apiv3/exceptions/TokenExpiredError.py
--rw-rw-rw-   0        0        0        0 2023-05-20 08:39:21.000000 etsy-apiv3-2.0.0/etsy_apiv3/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 15:41:29.249387 etsy-apiv3-2.0.0/etsy_apiv3/models/
--rw-rw-rw-   0        0        0      126 2023-01-05 12:58:42.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/Auth.py
--rw-rw-rw-   0        0        0      293 2023-01-05 11:18:24.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/File.py
--rw-rw-rw-   0        0        0      604 2022-06-06 13:20:33.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/ListingImageModel.py
--rw-rw-rw-   0        0        0     4001 2023-07-08 15:18:46.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/ListingModel.py
--rw-rw-rw-   0        0        0      293 2022-04-23 21:35:29.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/ListingPropertyModel.py
--rw-rw-rw-   0        0        0      255 2022-11-29 15:27:15.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/OfferingModel.py
--rw-rw-rw-   0        0        0     2124 2023-01-12 13:28:51.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/PaymentModel.py
--rw-rw-rw-   0        0        0      116 2022-04-04 14:44:43.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/PriceModel.py
--rw-rw-rw-   0        0        0      334 2022-11-29 15:27:25.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/ProductModel.py
--rw-rw-rw-   0        0        0      143 2022-04-05 14:24:47.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/ProductionPartnerModel.py
--rw-rw-rw-   0        0        0      303 2022-07-02 07:06:56.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/PropertyValueModel.py
--rw-rw-rw-   0        0        0     1961 2022-11-29 15:27:49.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/ReceiptModel.py
--rw-rw-rw-   0        0        0      199 2022-11-29 15:27:55.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/RefundModel.py
--rw-rw-rw-   0        0        0      245 2023-01-05 13:51:36.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/ReturnPolicyModel.py
--rw-rw-rw-   0        0        0      394 2022-04-23 16:26:45.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/ReviewModel.py
--rw-rw-rw-   0        0        0      254 2022-10-15 18:09:39.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/ShipmentModel.py
--rw-rw-rw-   0        0        0      293 2023-01-06 08:26:38.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/ShippingCarrierModel.py
--rw-rw-rw-   0        0        0      537 2023-01-28 10:35:20.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/ShippingProfileDestinationModel.py
--rw-rw-rw-   0        0        0      698 2022-11-29 15:28:16.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/ShippingProfileModel.py
--rw-rw-rw-   0        0        0      420 2023-07-19 15:34:54.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/ShippingProfileUpgradeModel.py
--rw-rw-rw-   0        0        0     1609 2022-07-02 07:49:17.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/ShopModel.py
--rw-rw-rw-   0        0        0      171 2023-01-05 13:22:47.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/ShopSection.py
--rw-rw-rw-   0        0        0      930 2023-01-06 07:39:02.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/TaxonomyModel.py
--rw-rw-rw-   0        0        0      146 2023-05-15 08:25:27.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/TokenModel.py
--rw-rw-rw-   0        0        0      974 2023-02-18 13:56:54.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/TransactionModel.py
--rw-rw-rw-   0        0        0      187 2022-04-05 14:20:33.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/TranslationModel.py
--rw-rw-rw-   0        0        0      728 2023-01-05 12:33:05.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/UserModel.py
--rw-rw-rw-   0        0        0      202 2022-04-05 14:03:40.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/VariationModel.py
--rw-rw-rw-   0        0        0     1224 2023-01-06 12:04:29.000000 etsy-apiv3-2.0.0/etsy_apiv3/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 15:41:29.257407 etsy-apiv3-2.0.0/etsy_apiv3/resources/
--rw-rw-rw-   0        0        0    17850 2023-07-19 12:23:15.000000 etsy-apiv3-2.0.0/etsy_apiv3/resources/ListingResource.py
--rw-rw-rw-   0        0        0     2645 2023-05-20 08:40:36.000000 etsy-apiv3-2.0.0/etsy_apiv3/resources/PaymentResource.py
--rw-rw-rw-   0        0        0     5940 2023-05-20 08:40:46.000000 etsy-apiv3-2.0.0/etsy_apiv3/resources/ReceiptResource.py
--rw-rw-rw-   0        0        0     1395 2023-05-20 08:41:00.000000 etsy-apiv3-2.0.0/etsy_apiv3/resources/ReviewResource.py
--rw-rw-rw-   0        0        0     6087 2023-05-20 08:41:07.000000 etsy-apiv3-2.0.0/etsy_apiv3/resources/ShippingProfileResource.py
--rw-rw-rw-   0        0        0     2792 2023-05-20 08:41:16.000000 etsy-apiv3-2.0.0/etsy_apiv3/resources/ShopPolicyResource.py
--rw-rw-rw-   0        0        0     3810 2023-05-20 08:41:27.000000 etsy-apiv3-2.0.0/etsy_apiv3/resources/ShopResource.py
--rw-rw-rw-   0        0        0      190 2023-01-06 12:19:53.000000 etsy-apiv3-2.0.0/etsy_apiv3/resources/UserResource.py
--rw-rw-rw-   0        0        0      222 2023-01-12 13:29:03.000000 etsy-apiv3-2.0.0/etsy_apiv3/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 15:41:29.279613 etsy-apiv3-2.0.0/etsy_apiv3/utils/
--rw-rw-rw-   0        0        0     4091 2023-04-06 13:41:59.000000 etsy-apiv3-2.0.0/etsy_apiv3/utils/APIV3.py
--rw-rw-rw-   0        0        0     5971 2023-07-19 15:41:08.000000 etsy-apiv3-2.0.0/etsy_apiv3/utils/EtsyOauth2Session.py
--rw-rw-rw-   0        0        0      474 2022-04-22 20:27:32.000000 etsy-apiv3-2.0.0/etsy_apiv3/utils/RequestException.py
--rw-rw-rw-   0        0        0      218 2022-07-02 14:30:58.000000 etsy-apiv3-2.0.0/etsy_apiv3/utils/Response.py
--rw-rw-rw-   0        0        0      154 2023-05-20 08:15:27.000000 etsy-apiv3-2.0.0/etsy_apiv3/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 15:41:29.207103 etsy-apiv3-2.0.0/etsy_apiv3.egg-info/
--rw-rw-rw-   0        0        0      342 2023-07-19 15:41:28.000000 etsy-apiv3-2.0.0/etsy_apiv3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1962 2023-07-19 15:41:29.000000 etsy-apiv3-2.0.0/etsy_apiv3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 15:41:28.000000 etsy-apiv3-2.0.0/etsy_apiv3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-07-19 15:41:28.000000 etsy-apiv3-2.0.0/etsy_apiv3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-19 15:41:28.000000 etsy-apiv3-2.0.0/etsy_apiv3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 15:41:29.289707 etsy-apiv3-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      746 2023-02-18 14:12:46.000000 etsy-apiv3-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 15:41:29.289707 etsy-apiv3-2.0.0/tests/
--rw-rw-rw-   0        0        0     2246 2023-01-12 13:49:46.000000 etsy-apiv3-2.0.0/tests/Payment.py
--rw-rw-rw-   0        0        0     3880 2023-03-15 09:02:53.000000 etsy-apiv3-2.0.0/tests/Receipt.py
--rw-rw-rw-   0        0        0        0 2023-03-15 09:02:44.000000 etsy-apiv3-2.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0      539 2023-01-13 08:43:06.000000 etsy-apiv3-2.0.0/tests/taxonomy_test.py
--rw-rw-rw-   0        0        0      426 2023-01-12 11:25:14.000000 etsy-apiv3-2.0.0/tests/test_credentials.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:39:22.034169 etsy-apiv3-2.1.0/
+-rw-rw-rw-   0        0        0     1089 2022-11-29 15:57:22.000000 etsy-apiv3-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0      342 2023-07-26 11:39:22.034169 etsy-apiv3-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1120 2022-12-02 14:38:46.000000 etsy-apiv3-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 11:39:21.765090 etsy-apiv3-2.1.0/etsy_apiv3/
+-rw-rw-rw-   0        0        0       23 2023-07-26 11:39:13.000000 etsy-apiv3-2.1.0/etsy_apiv3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:39:21.802406 etsy-apiv3-2.1.0/etsy_apiv3/exceptions/
+-rw-rw-rw-   0        0        0      549 2023-05-15 08:29:30.000000 etsy-apiv3-2.1.0/etsy_apiv3/exceptions/TokenExpiredError.py
+-rw-rw-rw-   0        0        0        0 2023-05-20 08:39:21.000000 etsy-apiv3-2.1.0/etsy_apiv3/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:39:21.949538 etsy-apiv3-2.1.0/etsy_apiv3/models/
+-rw-rw-rw-   0        0        0      126 2023-01-05 12:58:42.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/Auth.py
+-rw-rw-rw-   0        0        0      293 2023-01-05 11:18:24.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/File.py
+-rw-rw-rw-   0        0        0      604 2022-06-06 13:20:33.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/ListingImageModel.py
+-rw-rw-rw-   0        0        0     4001 2023-07-08 15:18:46.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/ListingModel.py
+-rw-rw-rw-   0        0        0      293 2022-04-23 21:35:29.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/ListingPropertyModel.py
+-rw-rw-rw-   0        0        0      255 2022-11-29 15:27:15.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/OfferingModel.py
+-rw-rw-rw-   0        0        0     2124 2023-01-12 13:28:51.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/PaymentModel.py
+-rw-rw-rw-   0        0        0      116 2022-04-04 14:44:43.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/PriceModel.py
+-rw-rw-rw-   0        0        0      334 2022-11-29 15:27:25.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/ProductModel.py
+-rw-rw-rw-   0        0        0      143 2022-04-05 14:24:47.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/ProductionPartnerModel.py
+-rw-rw-rw-   0        0        0      303 2022-07-02 07:06:56.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/PropertyValueModel.py
+-rw-rw-rw-   0        0        0     1961 2022-11-29 15:27:49.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/ReceiptModel.py
+-rw-rw-rw-   0        0        0      199 2022-11-29 15:27:55.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/RefundModel.py
+-rw-rw-rw-   0        0        0      245 2023-01-05 13:51:36.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/ReturnPolicyModel.py
+-rw-rw-rw-   0        0        0      394 2022-04-23 16:26:45.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/ReviewModel.py
+-rw-rw-rw-   0        0        0      254 2022-10-15 18:09:39.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/ShipmentModel.py
+-rw-rw-rw-   0        0        0      293 2023-01-06 08:26:38.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/ShippingCarrierModel.py
+-rw-rw-rw-   0        0        0      537 2023-01-28 10:35:20.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/ShippingProfileDestinationModel.py
+-rw-rw-rw-   0        0        0      698 2022-11-29 15:28:16.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/ShippingProfileModel.py
+-rw-rw-rw-   0        0        0      440 2023-07-26 11:39:05.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/ShippingProfileUpgradeModel.py
+-rw-rw-rw-   0        0        0     1609 2022-07-02 07:49:17.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/ShopModel.py
+-rw-rw-rw-   0        0        0      171 2023-01-05 13:22:47.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/ShopSection.py
+-rw-rw-rw-   0        0        0      930 2023-01-06 07:39:02.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/TaxonomyModel.py
+-rw-rw-rw-   0        0        0      146 2023-05-15 08:25:27.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/TokenModel.py
+-rw-rw-rw-   0        0        0      974 2023-02-18 13:56:54.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/TransactionModel.py
+-rw-rw-rw-   0        0        0      187 2022-04-05 14:20:33.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/TranslationModel.py
+-rw-rw-rw-   0        0        0      728 2023-01-05 12:33:05.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/UserModel.py
+-rw-rw-rw-   0        0        0      202 2022-04-05 14:03:40.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/VariationModel.py
+-rw-rw-rw-   0        0        0     1224 2023-01-06 12:04:29.000000 etsy-apiv3-2.1.0/etsy_apiv3/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:39:21.996406 etsy-apiv3-2.1.0/etsy_apiv3/resources/
+-rw-rw-rw-   0        0        0    17850 2023-07-19 12:23:15.000000 etsy-apiv3-2.1.0/etsy_apiv3/resources/ListingResource.py
+-rw-rw-rw-   0        0        0     2645 2023-05-20 08:40:36.000000 etsy-apiv3-2.1.0/etsy_apiv3/resources/PaymentResource.py
+-rw-rw-rw-   0        0        0     5940 2023-05-20 08:40:46.000000 etsy-apiv3-2.1.0/etsy_apiv3/resources/ReceiptResource.py
+-rw-rw-rw-   0        0        0     1395 2023-05-20 08:41:00.000000 etsy-apiv3-2.1.0/etsy_apiv3/resources/ReviewResource.py
+-rw-rw-rw-   0        0        0     6087 2023-05-20 08:41:07.000000 etsy-apiv3-2.1.0/etsy_apiv3/resources/ShippingProfileResource.py
+-rw-rw-rw-   0        0        0     2792 2023-05-20 08:41:16.000000 etsy-apiv3-2.1.0/etsy_apiv3/resources/ShopPolicyResource.py
+-rw-rw-rw-   0        0        0     3810 2023-05-20 08:41:27.000000 etsy-apiv3-2.1.0/etsy_apiv3/resources/ShopResource.py
+-rw-rw-rw-   0        0        0      190 2023-01-06 12:19:53.000000 etsy-apiv3-2.1.0/etsy_apiv3/resources/UserResource.py
+-rw-rw-rw-   0        0        0      222 2023-01-12 13:29:03.000000 etsy-apiv3-2.1.0/etsy_apiv3/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:39:22.002916 etsy-apiv3-2.1.0/etsy_apiv3/utils/
+-rw-rw-rw-   0        0        0     4091 2023-04-06 13:41:59.000000 etsy-apiv3-2.1.0/etsy_apiv3/utils/APIV3.py
+-rw-rw-rw-   0        0        0     5971 2023-07-19 15:41:08.000000 etsy-apiv3-2.1.0/etsy_apiv3/utils/EtsyOauth2Session.py
+-rw-rw-rw-   0        0        0      474 2022-04-22 20:27:32.000000 etsy-apiv3-2.1.0/etsy_apiv3/utils/RequestException.py
+-rw-rw-rw-   0        0        0      218 2022-07-02 14:30:58.000000 etsy-apiv3-2.1.0/etsy_apiv3/utils/Response.py
+-rw-rw-rw-   0        0        0      154 2023-05-20 08:15:27.000000 etsy-apiv3-2.1.0/etsy_apiv3/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:39:21.796312 etsy-apiv3-2.1.0/etsy_apiv3.egg-info/
+-rw-rw-rw-   0        0        0      342 2023-07-26 11:39:21.000000 etsy-apiv3-2.1.0/etsy_apiv3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1962 2023-07-26 11:39:21.000000 etsy-apiv3-2.1.0/etsy_apiv3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 11:39:21.000000 etsy-apiv3-2.1.0/etsy_apiv3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-07-26 11:39:21.000000 etsy-apiv3-2.1.0/etsy_apiv3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 11:39:21.000000 etsy-apiv3-2.1.0/etsy_apiv3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 11:39:22.034169 etsy-apiv3-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      746 2023-02-18 14:12:46.000000 etsy-apiv3-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:39:22.034169 etsy-apiv3-2.1.0/tests/
+-rw-rw-rw-   0        0        0     2246 2023-01-12 13:49:46.000000 etsy-apiv3-2.1.0/tests/Payment.py
+-rw-rw-rw-   0        0        0     3880 2023-03-15 09:02:53.000000 etsy-apiv3-2.1.0/tests/Receipt.py
+-rw-rw-rw-   0        0        0        0 2023-03-15 09:02:44.000000 etsy-apiv3-2.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      539 2023-01-13 08:43:06.000000 etsy-apiv3-2.1.0/tests/taxonomy_test.py
+-rw-rw-rw-   0        0        0      426 2023-01-12 11:25:14.000000 etsy-apiv3-2.1.0/tests/test_credentials.py
```

### Comparing `etsy-apiv3-2.0.0/LICENSE` & `etsy-apiv3-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/README.md` & `etsy-apiv3-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/exceptions/TokenExpiredError.py` & `etsy-apiv3-2.1.0/etsy_apiv3/exceptions/TokenExpiredError.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/models/ListingImageModel.py` & `etsy-apiv3-2.1.0/etsy_apiv3/models/ListingImageModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/models/ListingModel.py` & `etsy-apiv3-2.1.0/etsy_apiv3/models/ListingModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/models/PaymentModel.py` & `etsy-apiv3-2.1.0/etsy_apiv3/models/PaymentModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/models/ReceiptModel.py` & `etsy-apiv3-2.1.0/etsy_apiv3/models/ReceiptModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/models/ShippingProfileDestinationModel.py` & `etsy-apiv3-2.1.0/etsy_apiv3/models/ShippingProfileDestinationModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/models/ShippingProfileModel.py` & `etsy-apiv3-2.1.0/etsy_apiv3/models/ShippingProfileModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/models/ShopModel.py` & `etsy-apiv3-2.1.0/etsy_apiv3/models/ShopModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/models/TaxonomyModel.py` & `etsy-apiv3-2.1.0/etsy_apiv3/models/TaxonomyModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/models/TransactionModel.py` & `etsy-apiv3-2.1.0/etsy_apiv3/models/TransactionModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/models/UserModel.py` & `etsy-apiv3-2.1.0/etsy_apiv3/models/UserModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/models/__init__.py` & `etsy-apiv3-2.1.0/etsy_apiv3/models/__init__.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/resources/ListingResource.py` & `etsy-apiv3-2.1.0/etsy_apiv3/resources/ListingResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/resources/PaymentResource.py` & `etsy-apiv3-2.1.0/etsy_apiv3/resources/PaymentResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/resources/ReceiptResource.py` & `etsy-apiv3-2.1.0/etsy_apiv3/resources/ReceiptResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/resources/ReviewResource.py` & `etsy-apiv3-2.1.0/etsy_apiv3/resources/ReviewResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/resources/ShippingProfileResource.py` & `etsy-apiv3-2.1.0/etsy_apiv3/resources/ShippingProfileResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/resources/ShopPolicyResource.py` & `etsy-apiv3-2.1.0/etsy_apiv3/resources/ShopPolicyResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/resources/ShopResource.py` & `etsy-apiv3-2.1.0/etsy_apiv3/resources/ShopResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/utils/APIV3.py` & `etsy-apiv3-2.1.0/etsy_apiv3/utils/APIV3.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3/utils/EtsyOauth2Session.py` & `etsy-apiv3-2.1.0/etsy_apiv3/utils/EtsyOauth2Session.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/etsy_apiv3.egg-info/SOURCES.txt` & `etsy-apiv3-2.1.0/etsy_apiv3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/setup.py` & `etsy-apiv3-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/tests/Payment.py` & `etsy-apiv3-2.1.0/tests/Payment.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/tests/Receipt.py` & `etsy-apiv3-2.1.0/tests/Receipt.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-2.0.0/tests/taxonomy_test.py` & `etsy-apiv3-2.1.0/tests/taxonomy_test.py`

 * *Files identical despite different names*


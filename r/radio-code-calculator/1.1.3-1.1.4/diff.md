# Comparing `tmp/radio_code_calculator-1.1.3.tar.gz` & `tmp/radio_code_calculator-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radio_code_calculator-1.1.3.tar", last modified: Sat Mar 18 17:54:56 2023, max compression
+gzip compressed data, was "radio_code_calculator-1.1.4.tar", last modified: Wed Jul 26 18:06:38 2023, max compression
```

## Comparing `radio_code_calculator-1.1.3.tar` & `radio_code_calculator-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-18 17:54:58.000000 radio_code_calculator-1.1.3/
--rw-rw-rw-   0        0        0    24332 2023-03-18 17:54:58.000000 radio_code_calculator-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    19799 2023-03-18 17:51:46.000000 radio_code_calculator-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-18 17:54:58.000000 radio_code_calculator-1.1.3/radio_code_calculator/
--rw-rw-rw-   0        0        0       59 2023-02-08 21:29:14.000000 radio_code_calculator-1.1.3/radio_code_calculator/__init__.py
--rw-rw-rw-   0        0        0    12104 2023-03-18 17:51:46.000000 radio_code_calculator-1.1.3/radio_code_calculator/radio_code_calculator.py
-drwxrwxrwx   0        0        0        0 2023-03-18 17:54:58.000000 radio_code_calculator-1.1.3/radio_code_calculator.egg-info/
--rw-rw-rw-   0        0        0    24332 2023-03-18 17:54:58.000000 radio_code_calculator-1.1.3/radio_code_calculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-03-18 17:54:58.000000 radio_code_calculator-1.1.3/radio_code_calculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-18 17:54:58.000000 radio_code_calculator-1.1.3/radio_code_calculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-18 17:54:58.000000 radio_code_calculator-1.1.3/radio_code_calculator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-03-18 17:54:58.000000 radio_code_calculator-1.1.3/radio_code_calculator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-03-18 17:54:58.000000 radio_code_calculator-1.1.3/radio_code_calculator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-18 17:54:58.000000 radio_code_calculator-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1242 2023-03-18 17:51:54.000000 radio_code_calculator-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:06:40.000000 radio_code_calculator-1.1.4/
+-rw-rw-rw-   0        0        0    24439 2023-07-26 18:06:40.000000 radio_code_calculator-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    19898 2023-07-26 17:55:12.000000 radio_code_calculator-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 18:06:40.000000 radio_code_calculator-1.1.4/radio_code_calculator/
+-rw-rw-rw-   0        0        0       59 2023-02-08 20:29:14.000000 radio_code_calculator-1.1.4/radio_code_calculator/__init__.py
+-rw-rw-rw-   0        0        0    12185 2023-07-26 17:54:48.000000 radio_code_calculator-1.1.4/radio_code_calculator/radio_code_calculator.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:06:40.000000 radio_code_calculator-1.1.4/radio_code_calculator.egg-info/
+-rw-rw-rw-   0        0        0    24439 2023-07-26 18:06:40.000000 radio_code_calculator-1.1.4/radio_code_calculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-07-26 18:06:40.000000 radio_code_calculator-1.1.4/radio_code_calculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 18:06:40.000000 radio_code_calculator-1.1.4/radio_code_calculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-26 18:06:40.000000 radio_code_calculator-1.1.4/radio_code_calculator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-26 18:06:40.000000 radio_code_calculator-1.1.4/radio_code_calculator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-26 18:06:40.000000 radio_code_calculator-1.1.4/radio_code_calculator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 18:06:40.000000 radio_code_calculator-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1242 2023-07-26 17:59:10.000000 radio_code_calculator-1.1.4/setup.py
```

### Comparing `radio_code_calculator-1.1.3/PKG-INFO` & `radio_code_calculator-1.1.4/radio_code_calculator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: radio_code_calculator
-Version: 1.1.3
+Name: radio-code-calculator
+Version: 1.1.4
 Summary: Radio Code Calculator is an online service along with Web API and SDK for generating car radio unlock codes for popular vehicle brands.
 Home-page: https://www.pelock.com/products/radio-code-calculator
 Author: Bartosz Wójcik
 Author-email: support@pelock.com
 License: Apache-2.0
 Description: # Radio Code Calculator Online & SDK for Python
         
@@ -35,14 +35,15 @@
         * [Ford V Serial](https://www.pelock.com/products/ford-radio-code-v-serial-calculator-generator)
         * [Ford TravelPilot EX, FX & NX](https://www.pelock.com/products/ford-travelpilot-ex-fx-nx-radio-code-generator-calculator)
         * [Chrysler Panasonic TM9](https://www.pelock.com/products/chrysler-panasonic-tm9-car-radio-code-calculator-generator)
         * [Fiat Stilo & Bravo Visteon](https://www.pelock.com/products/fiat-stilo-bravo-visteon-radio-code-calculator-generator)
         * [Fiat DAIICHI MOPAR](https://www.pelock.com/products/fiat-daiichi-radio-code-calculator-generator)
         * [Nissan Glove Box Immobiliser PIN](https://www.pelock.com/products/nissan-glove-box-pin-code-calculator)
         * [Eclipse ESN Unlock Code Calculator](https://www.pelock.com/products/eclipse-esn-unlock-code-calculator)
+        * [Jaguar Alpine](https://www.pelock.com/products/jaguar-alpine-car-radio-unlock-code-calculator)
         
         ## Use of radio code calculator
         
         Where and who can use the radio code generation service and make money from code generation?
         
         ### ![Android](https://www.pelock.com/img/en/icons/android-32.png) App developers 
         The main audience for our software is clearly developers and programmers, either of mobile or desktop applications.
@@ -110,15 +111,15 @@
         ###############################################################################
         #
         # Radio Code Calculator API - WebApi interface usage example
         #
         # In this example, we will demonstrate how to generate a code for a specific
         # type of car radio.
         #
-        # Version        : v1.1.3
+        # Version        : v1.1.4
         # Language       : Python
         # Author         : Bartosz Wójcik
         # Project        : https://www.pelock.com/products/radio-code-calculator
         # Homepage       : https://www.pelock.com
         #
         ###############################################################################
         
@@ -178,15 +179,15 @@
         #
         # Radio Code Calculator API - WebApi interface usage example
         #
         # In this example, we will demonstrate how to generate a code for a specific
         # type of car radio. This example shows how to use an extended offline
         # validation.
         #
-        # Version        : v1.1.3
+        # Version        : v1.1.4
         # Language       : Python
         # Author         : Bartosz Wójcik
         # Project        : https://www.pelock.com/products/radio-code-calculator
         # Homepage       : https://www.pelock.com
         #
         ###############################################################################
         
@@ -288,15 +289,15 @@
         #
         # Radio Code Calculator API - WebApi interface usage example
         #
         # In this example we will list all the available calculators and, their
         # parameters like name, maximum length of the radio serial number and its
         # regex pattern.
         #
-        # Version        : v1.1.3
+        # Version        : v1.1.4
         # Language       : Python
         # Author         : Bartosz Wójcik
         # Project        : https://www.pelock.com/products/radio-code-calculator
         # Homepage       : https://www.pelock.com
         #
         ###############################################################################
         
@@ -349,15 +350,15 @@
         ###############################################################################
         #
         # Radio Code Calculator API - WebApi interface usage example
         #
         # In this example, we will demonstrate how to get information about the
         # specific radio calculator and its parameters (max. length & regex pattern).
         #
-        # Version        : v1.1.3
+        # Version        : v1.1.4
         # Language       : Python
         # Author         : Bartosz Wójcik
         # Project        : https://www.pelock.com/products/radio-code-calculator
         # Homepage       : https://www.pelock.com
         #
         ###############################################################################
         
@@ -405,15 +406,15 @@
         
         ###############################################################################
         #
         # Radio Code Calculator API - WebApi interface usage example
         #
         # In this example we will verify our activation key status.
         #
-        # Version        : v1.1.3
+        # Version        : v1.1.4
         # Language       : Python
         # Author         : Bartosz Wójcik
         # Project        : https://www.pelock.com/products/radio-code-calculator
         # Homepage       : https://www.pelock.com
         #
         ###############################################################################
```

### Comparing `radio_code_calculator-1.1.3/README.md` & `radio_code_calculator-1.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 * [Ford V Serial](https://www.pelock.com/products/ford-radio-code-v-serial-calculator-generator)
 * [Ford TravelPilot EX, FX & NX](https://www.pelock.com/products/ford-travelpilot-ex-fx-nx-radio-code-generator-calculator)
 * [Chrysler Panasonic TM9](https://www.pelock.com/products/chrysler-panasonic-tm9-car-radio-code-calculator-generator)
 * [Fiat Stilo & Bravo Visteon](https://www.pelock.com/products/fiat-stilo-bravo-visteon-radio-code-calculator-generator)
 * [Fiat DAIICHI MOPAR](https://www.pelock.com/products/fiat-daiichi-radio-code-calculator-generator)
 * [Nissan Glove Box Immobiliser PIN](https://www.pelock.com/products/nissan-glove-box-pin-code-calculator)
 * [Eclipse ESN Unlock Code Calculator](https://www.pelock.com/products/eclipse-esn-unlock-code-calculator)
+* [Jaguar Alpine](https://www.pelock.com/products/jaguar-alpine-car-radio-unlock-code-calculator)
 
 ## Use of radio code calculator
 
 Where and who can use the radio code generation service and make money from code generation?
 
 ### ![Android](https://www.pelock.com/img/en/icons/android-32.png) App developers 
 The main audience for our software is clearly developers and programmers, either of mobile or desktop applications.
@@ -102,15 +103,15 @@
 ###############################################################################
 #
 # Radio Code Calculator API - WebApi interface usage example
 #
 # In this example, we will demonstrate how to generate a code for a specific
 # type of car radio.
 #
-# Version        : v1.1.3
+# Version        : v1.1.4
 # Language       : Python
 # Author         : Bartosz Wójcik
 # Project        : https://www.pelock.com/products/radio-code-calculator
 # Homepage       : https://www.pelock.com
 #
 ###############################################################################
 
@@ -170,15 +171,15 @@
 #
 # Radio Code Calculator API - WebApi interface usage example
 #
 # In this example, we will demonstrate how to generate a code for a specific
 # type of car radio. This example shows how to use an extended offline
 # validation.
 #
-# Version        : v1.1.3
+# Version        : v1.1.4
 # Language       : Python
 # Author         : Bartosz Wójcik
 # Project        : https://www.pelock.com/products/radio-code-calculator
 # Homepage       : https://www.pelock.com
 #
 ###############################################################################
 
@@ -280,15 +281,15 @@
 #
 # Radio Code Calculator API - WebApi interface usage example
 #
 # In this example we will list all the available calculators and, their
 # parameters like name, maximum length of the radio serial number and its
 # regex pattern.
 #
-# Version        : v1.1.3
+# Version        : v1.1.4
 # Language       : Python
 # Author         : Bartosz Wójcik
 # Project        : https://www.pelock.com/products/radio-code-calculator
 # Homepage       : https://www.pelock.com
 #
 ###############################################################################
 
@@ -341,15 +342,15 @@
 ###############################################################################
 #
 # Radio Code Calculator API - WebApi interface usage example
 #
 # In this example, we will demonstrate how to get information about the
 # specific radio calculator and its parameters (max. length & regex pattern).
 #
-# Version        : v1.1.3
+# Version        : v1.1.4
 # Language       : Python
 # Author         : Bartosz Wójcik
 # Project        : https://www.pelock.com/products/radio-code-calculator
 # Homepage       : https://www.pelock.com
 #
 ###############################################################################
 
@@ -397,15 +398,15 @@
 
 ###############################################################################
 #
 # Radio Code Calculator API - WebApi interface usage example
 #
 # In this example we will verify our activation key status.
 #
-# Version        : v1.1.3
+# Version        : v1.1.4
 # Language       : Python
 # Author         : Bartosz Wójcik
 # Project        : https://www.pelock.com/products/radio-code-calculator
 # Homepage       : https://www.pelock.com
 #
 ###############################################################################
```

### Comparing `radio_code_calculator-1.1.3/radio_code_calculator/radio_code_calculator.py` & `radio_code_calculator-1.1.4/radio_code_calculator/radio_code_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ###############################################################################
 #
 # Radio Code Calculator API - WebApi interface
 #
 # Generate radio unlocking codes for various radio players.
 #
-# Version      : v1.1.3
+# Version      : v1.1.4
 # Python       : Python v3
 # Dependencies : requests (https://pypi.python.org/pypi/requests/)
 # Author       : Bartosz Wójcik (support@pelock.com)
 # Project      : https://www.pelock.com/products/radio-code-calculator
 # Homepage     : https://www.pelock.com
 #
 ###############################################################################
@@ -156,14 +156,15 @@
     FORD_TRAVELPILOT: RadioModel = RadioModel("ford-travelpilot", 7, r"^([0-9]{7})$")
     FIAT_STILO_BRAVO_VISTEON: RadioModel = RadioModel("fiat-stilo-bravo-visteon", 6, r"^([a-zA-Z0-9]{6})$")
     FIAT_DAIICHI: RadioModel = RadioModel("fiat-daiichi", 4, r"^([a-zA-Z0-9]{4})$")
     TOYOTA_ERC: RadioModel = RadioModel("toyota-erc", 16, r"^([a-zA-Z0-9]{16})$")
     JEEP_CHEROKEE: RadioModel = RadioModel("jeep-cherokee", 14, r"^([a-zA-Z0-9]{10}[0-9]{4})$")
     NISSAN_GLOVE_BOX: RadioModel = RadioModel("nissan-glove-box", 12, r"^([a-zA-Z0-9]{12})$")
     ECLIPSE_ESN: RadioModel = RadioModel("eclipse-esn", 6, r"^([a-zA-Z0-9]{6})$")
+    JAGUAR_ALPINE: RadioModel = RadioModel("jaguar-alpine", 5, r"^([0-9]{5})$")
 
 
 class RadioCodeCalculator(object):
     """Radio Code Calculator API module"""
 
     # 
     # @var string default Radio Code Calculator API WebApi endpoint
```

### Comparing `radio_code_calculator-1.1.3/radio_code_calculator.egg-info/PKG-INFO` & `radio_code_calculator-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: radio-code-calculator
-Version: 1.1.3
+Name: radio_code_calculator
+Version: 1.1.4
 Summary: Radio Code Calculator is an online service along with Web API and SDK for generating car radio unlock codes for popular vehicle brands.
 Home-page: https://www.pelock.com/products/radio-code-calculator
 Author: Bartosz Wójcik
 Author-email: support@pelock.com
 License: Apache-2.0
 Description: # Radio Code Calculator Online & SDK for Python
         
@@ -35,14 +35,15 @@
         * [Ford V Serial](https://www.pelock.com/products/ford-radio-code-v-serial-calculator-generator)
         * [Ford TravelPilot EX, FX & NX](https://www.pelock.com/products/ford-travelpilot-ex-fx-nx-radio-code-generator-calculator)
         * [Chrysler Panasonic TM9](https://www.pelock.com/products/chrysler-panasonic-tm9-car-radio-code-calculator-generator)
         * [Fiat Stilo & Bravo Visteon](https://www.pelock.com/products/fiat-stilo-bravo-visteon-radio-code-calculator-generator)
         * [Fiat DAIICHI MOPAR](https://www.pelock.com/products/fiat-daiichi-radio-code-calculator-generator)
         * [Nissan Glove Box Immobiliser PIN](https://www.pelock.com/products/nissan-glove-box-pin-code-calculator)
         * [Eclipse ESN Unlock Code Calculator](https://www.pelock.com/products/eclipse-esn-unlock-code-calculator)
+        * [Jaguar Alpine](https://www.pelock.com/products/jaguar-alpine-car-radio-unlock-code-calculator)
         
         ## Use of radio code calculator
         
         Where and who can use the radio code generation service and make money from code generation?
         
         ### ![Android](https://www.pelock.com/img/en/icons/android-32.png) App developers 
         The main audience for our software is clearly developers and programmers, either of mobile or desktop applications.
@@ -110,15 +111,15 @@
         ###############################################################################
         #
         # Radio Code Calculator API - WebApi interface usage example
         #
         # In this example, we will demonstrate how to generate a code for a specific
         # type of car radio.
         #
-        # Version        : v1.1.3
+        # Version        : v1.1.4
         # Language       : Python
         # Author         : Bartosz Wójcik
         # Project        : https://www.pelock.com/products/radio-code-calculator
         # Homepage       : https://www.pelock.com
         #
         ###############################################################################
         
@@ -178,15 +179,15 @@
         #
         # Radio Code Calculator API - WebApi interface usage example
         #
         # In this example, we will demonstrate how to generate a code for a specific
         # type of car radio. This example shows how to use an extended offline
         # validation.
         #
-        # Version        : v1.1.3
+        # Version        : v1.1.4
         # Language       : Python
         # Author         : Bartosz Wójcik
         # Project        : https://www.pelock.com/products/radio-code-calculator
         # Homepage       : https://www.pelock.com
         #
         ###############################################################################
         
@@ -288,15 +289,15 @@
         #
         # Radio Code Calculator API - WebApi interface usage example
         #
         # In this example we will list all the available calculators and, their
         # parameters like name, maximum length of the radio serial number and its
         # regex pattern.
         #
-        # Version        : v1.1.3
+        # Version        : v1.1.4
         # Language       : Python
         # Author         : Bartosz Wójcik
         # Project        : https://www.pelock.com/products/radio-code-calculator
         # Homepage       : https://www.pelock.com
         #
         ###############################################################################
         
@@ -349,15 +350,15 @@
         ###############################################################################
         #
         # Radio Code Calculator API - WebApi interface usage example
         #
         # In this example, we will demonstrate how to get information about the
         # specific radio calculator and its parameters (max. length & regex pattern).
         #
-        # Version        : v1.1.3
+        # Version        : v1.1.4
         # Language       : Python
         # Author         : Bartosz Wójcik
         # Project        : https://www.pelock.com/products/radio-code-calculator
         # Homepage       : https://www.pelock.com
         #
         ###############################################################################
         
@@ -405,15 +406,15 @@
         
         ###############################################################################
         #
         # Radio Code Calculator API - WebApi interface usage example
         #
         # In this example we will verify our activation key status.
         #
-        # Version        : v1.1.3
+        # Version        : v1.1.4
         # Language       : Python
         # Author         : Bartosz Wójcik
         # Project        : https://www.pelock.com/products/radio-code-calculator
         # Homepage       : https://www.pelock.com
         #
         ###############################################################################
```

### Comparing `radio_code_calculator-1.1.3/setup.py` & `radio_code_calculator-1.1.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='radio_code_calculator',
 
-    version='1.1.3',
+    version='1.1.4',
 
     description='Radio Code Calculator is an online service along with Web API and SDK for generating car radio unlock codes for popular vehicle brands.',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     keywords="radio code navigation calculator generator vehicle car automotive radiocode radiocodes api",
```


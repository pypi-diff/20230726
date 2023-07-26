# Comparing `tmp/visualtest_python-1.5.1-py3-none-any.whl.zip` & `tmp/visualtest_python-1.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20781 bytes, number of entries: 11
--rw-r--r--  2.0 unx      121 b- defN 23-Jul-18 11:44 sbvt/__init__.py
--rw-r--r--  2.0 unx     7694 b- defN 23-Jul-11 11:50 sbvt/api.py
--rw-r--r--  2.0 unx    36548 b- defN 23-Jul-11 11:50 sbvt/browser.py
--rw-r--r--  2.0 unx     6269 b- defN 23-Jun-09 14:01 sbvt/imagetools.py
--rw-r--r--  2.0 unx      548 b- defN 23-May-11 09:06 sbvt/timer.py
--rw-r--r--  2.0 unx    16070 b- defN 23-Jul-18 11:45 sbvt/visualtest.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Jul-18 11:46 visualtest_python-1.5.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3876 b- defN 23-Jul-18 11:46 visualtest_python-1.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-18 11:46 visualtest_python-1.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-18 11:46 visualtest_python-1.5.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      868 b- defN 23-Jul-18 11:46 visualtest_python-1.5.1.dist-info/RECORD
-11 files, 73164 bytes uncompressed, 19323 bytes compressed:  73.6%
+Zip file size: 21109 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      121 b- defN 23-Jul-26 16:43 sbvt/__init__.py
+-rw-r--r--  2.0 unx     9505 b- defN 23-Jul-25 22:59 sbvt/api.py
+-rw-r--r--  2.0 unx    36548 b- defN 23-Jul-20 21:49 sbvt/browser.py
+-rw-r--r--  2.0 unx     6269 b- defN 23-Jun-01 20:43 sbvt/imagetools.py
+-rw-r--r--  2.0 unx      548 b- defN 23-May-08 21:54 sbvt/timer.py
+-rw-r--r--  2.0 unx    16511 b- defN 23-Jul-25 22:59 sbvt/visualtest.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jul-26 16:45 visualtest_python-1.5.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3876 b- defN 23-Jul-26 16:45 visualtest_python-1.5.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-26 16:45 visualtest_python-1.5.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-26 16:45 visualtest_python-1.5.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      868 b- defN 23-Jul-26 16:45 visualtest_python-1.5.2.dist-info/RECORD
+11 files, 75416 bytes uncompressed, 19651 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: sbvt/timer.py
 Comment: 
 
 Filename: sbvt/visualtest.py
 Comment: 
 
-Filename: visualtest_python-1.5.1.dist-info/LICENSE
+Filename: visualtest_python-1.5.2.dist-info/LICENSE
 Comment: 
 
-Filename: visualtest_python-1.5.1.dist-info/METADATA
+Filename: visualtest_python-1.5.2.dist-info/METADATA
 Comment: 
 
-Filename: visualtest_python-1.5.1.dist-info/WHEEL
+Filename: visualtest_python-1.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: visualtest_python-1.5.1.dist-info/top_level.txt
+Filename: visualtest_python-1.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: visualtest_python-1.5.1.dist-info/RECORD
+Filename: visualtest_python-1.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbvt/__init__.py

```diff
@@ -1,4 +1,4 @@
 # this import statement is here for context.py in tests folder
 from .visualtest import VisualTest
 
-__version__ = '1.5.1'
+__version__ = '1.5.2'
```

## sbvt/api.py

```diff
@@ -118,45 +118,83 @@
         })
         if response.status_code in range(200, 300):
             return response.json()
         else:
             log.error(f'Failed to create testRun. HTTP Response: {response.json()}')
             raise Exception(f'Failed to create testRun. HTTP Response: {response.json()}')
 
-    def saveImage(self, testRunName, imageData, imageBinary):
+    def saveImage(self, testRunName, imageData, imageBinary, domString):
         log.info(f'Saving image for testRunName: {testRunName}')
 
-        # TODO add this logic later with a flag
         # check if testRun already exists, if not create one
         if not self.testRun:
             self.testRun = self.createTestRun(testRunName)
 
+        # create image on backend via API
         url = f'{Api.baseUrl}/projects/{self.projectId}/testruns/{self.testRun["testRunId"]}/images'
         log.info(f'calling API to save image: {url}')
         log.debug(f'imageData: {imageData}')
 
         response = api.post(url, json=imageData)
         log.info(f'create image response: {response}')
 
         if response.status_code in range(200, 300):
             result = response.json()
         else:
             log.error(f'Failed to create image. HTTP Response: {response.json()}')
             raise Exception(f'Failed to create image. HTTP Response: {response.json()}')
 
-        log.info(f'uploading image to: {result["uploadUrl"]}')
 
+        # Upload DOM file to S3
+        log.info(f'uploading DOM to S3: {result["domUploadUrl"]}')
+        try:
+            if 'domUploadUrl' not in result:
+                raise Exception(f'No domUploadUrl received from POST to /images API')
+            else:
+                response = s3.put(result['domUploadUrl'], data=domString.encode())
+                log.info(f'upload DOM to S3 response: {response.status_code}')
+                if not response.status_code in range(200, 300):
+                    log.error(f'Failed to upload DOM to S3.')
+                    raise Exception(f'{response.text}')
+
+        except Exception as e:
+            log.debug(f'error: {e.__str__()}')
+            errorMessage = {"errorMessage": e.__str__()}
+            url = f'{Api.baseUrl}/projects/{self.projectId}/testruns/{self.testRun["testRunId"]}/images/{result["imageId"]}'
+
+            response = api.patch(url, json=errorMessage)
+            log.info(f'calling API to add error: {url}')
+            log.debug(f'errorMessage: {errorMessage}')
+
+            if response.status_code in range(200, 300):
+                log.debug(f'errorResult: {response.json()}')
+            else:
+                log.error(
+                    f'Failed to send error. HTTP Response: {response.text}')
+                raise Exception(
+                    f'Failed to send error. HTTP Response: {response.text}')
+        
+        # Call API to set domCaptured=true
+        url = f'{Api.baseUrl}/projects/{self.projectId}/testruns/{self.testRun["testRunId"]}/images/{result["imageId"]}'
+        log.info(f'calling API to PATCH image with domCaptured=true: {url}')
+
+        response = api.patch(url, json={'domCaptured': True})
+        log.info(f'patch image response: {response}')
+
+       
+        # Upload image to S3
+        log.info(f'uploading image to S3: {result["uploadUrl"]}')
         try:
             response = s3.put(result['uploadUrl'], data=imageBinary)
-            log.info(f'upload image response: {response.status_code}')
+            log.info(f'upload image to S3 response: {response.status_code}')
 
             if response.status_code in range(200, 300):
                 return result
             else:
-                log.error(f'Failed to upload image.')
+                log.error(f'Failed to upload image to S3.')
                 raise Exception(f'{response.text}')
 
         except Exception as e:
             log.debug(f'error: {e.__str__()}')
             errorMessage = {"errorMessage": e.__str__()}
             url = f'{Api.baseUrl}/projects/{self.projectId}/testruns/{self.testRun["testRunId"]}/images/{result["imageId"]}'
```

## sbvt/visualtest.py

```diff
@@ -291,61 +291,63 @@
                 if type(options['lazyload']) != int or options['lazyload'] < 0 or options['lazyload'] > 10000:
                     raise Exception('"lazyload" value must be an integer between 0 and 10000 ms!')
 
             screenshotResult = self.browser.takeFullpageScreenshot(name, options)
 
             imageType = 'fullpage'
         
+        
+         # save final image to debug file
+        if self._debug:
+            fileDir = os.path.join(self._debugDir, f'{name}-{imageType}')
+            os.makedirs(fileDir, exist_ok=True)
+            imagePath = os.path.join(fileDir, f'{name}.png')
+            domPath = os.path.join(fileDir, f'{name}.json')
+
+            with open(imagePath, 'wb') as outfile:
+                outfile.write(screenshotResult['imageBinary'])
+                outfile.close()
+            with open(domPath, 'w') as outfile:
+                json.dump(self.browser.dom, outfile, indent=4)
+
+        # save final image to saveTo location
+        if self.saveTo is not None:
+            current_time = time.strftime('%H-%M-%S', time.localtime())
+            saveToFile = os.path.join(self._settings['saveTo'], f'{name}-{imageType}_{current_time}.png')
+            screenshotResult['imagePath'] = saveToFile
+            with open(saveToFile, 'wb') as outfile:
+                outfile.write(screenshotResult['imageBinary'])
+                outfile.close()
+        
+        
         # save image to server
         imageData = {
             'sessionId': self._sessionId,
             'imageName': name,
             'imageType': imageType,
             'imageExt': 'png',
             'testUrl': self.browser._driver.current_url,
             'viewportWidth': self.browser.viewportWidth,
             'viewportHeight': self.browser.viewportHeight,
             'imageWidth': screenshotResult['imageSize']['width'],
             'imageHeight': screenshotResult['imageSize']['height'],
-            'dom': json.dumps(self.browser.dom),
             'ignoredElements': json.dumps(self.browser.dom['ignoredElementsData']),
             'comparisonMode': comparisonMode,
             'sensitivity': sensitivity,
-            'headless': self.browser._headless
+            'headless': self.browser._headless,
+            'sdkDomUpload': True # SDKs will upload dom to S3 directly and receive presigned URL if this flag is set
         }
         imageData.update(self.browser._deviceInfo) # required information about device/os/browser
 
         # these two are informational and just used to store - not required
         imageData.update({'driverCapabilities': json.dumps(self.browser.capabilities)})
         imageData.update({'userAgentInfo': json.dumps(self.browser._userAgentInfo)})
 
         # post the image, creating testrun if new
-        imageApiResult = self._api.saveImage(self._settings['testRunName'], imageData, screenshotResult['imageBinary'])
-
-        # save final image to debug file
-        if self._debug:
-            fileDir = os.path.join(self._debugDir, f'{name}-{imageType}')
-            os.makedirs(fileDir, exist_ok=True)
-            imagePath = os.path.join(fileDir, f'{name}.png')
-            domPath = os.path.join(fileDir, f'{name}.json')
-
-            with open(imagePath, 'wb') as outfile:
-                outfile.write(screenshotResult['imageBinary'])
-                outfile.close()
-            with open(domPath, 'w') as outfile:
-                json.dump(self.browser.dom, outfile, indent=4)
-
-        # save final image to saveTo location
-        if self.saveTo is not None:
-            current_time = time.strftime('%H-%M-%S', time.localtime())
-            saveToFile = os.path.join(self._settings['saveTo'], f'{name}-{imageType}_{current_time}.png')
-            screenshotResult['imagePath'] = saveToFile
-            with open(saveToFile, 'wb') as outfile:
-                outfile.write(screenshotResult['imageBinary'])
-                outfile.close()
+        imageApiResult = self._api.saveImage(self._settings['testRunName'], imageData, screenshotResult['imageBinary'], json.dumps(self.browser.dom))
 
         # do not return the binary to the results
         del screenshotResult['imageBinary']
 
         return {
             'screenshotResult': screenshotResult,
             'imageApiResult': imageApiResult,
@@ -376,7 +378,16 @@
 
     def getTestRunResult(self):
         comparisons = self._api.getTestRunResult()
         return {
             'passed' : comparisons['aggregate']['passed'], 
             'failed' : comparisons['aggregate']['failed']
             }
+
+    def setDeviceName(self, deviceName):
+        if(type(deviceName) == str ):
+            self.browser._deviceInfo["deviceName"] = deviceName
+        else:
+            raise Exception('"deviceName" should be a str type.')
+        
+    def getDeviceName(self):
+        return self.browser._deviceInfo["deviceName"]
```

## Comparing `visualtest_python-1.5.1.dist-info/LICENSE` & `visualtest_python-1.5.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `visualtest_python-1.5.1.dist-info/METADATA` & `visualtest_python-1.5.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualtest-python
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python SDK for SmartBear VisualTest via Selenium WebDriver
 Home-page: https://github.com/SmartBear/visualtest-python
 Author: Luke Kende
 Author-email: luke.kende@smartbear.com
 Keywords: visual testing,UI testing,GUI testing,UX testing,screenshots,full page screenshots,image comparisons,regression testing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

## Comparing `visualtest_python-1.5.1.dist-info/RECORD` & `visualtest_python-1.5.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-sbvt/__init__.py,sha256=z2qB8PVChPeAEsGkTW8LK7eUB9L2oxzWDEF6Lut2y4A,121
-sbvt/api.py,sha256=oI9IYHNk4wlBV1bjqx3C4cT3HOlkvErstnAf_YyN8gA,7694
+sbvt/__init__.py,sha256=m2Ckp3NiBlT0nI5TeMGh6WBZH3MF3D3yTMuSU5d3SaY,121
+sbvt/api.py,sha256=NhRYkNZch-QCz5bQswEiz-RC52o7Iiavbz_iWtqNvH4,9505
 sbvt/browser.py,sha256=PuZS51EiOfTXS14q4G2YgVOG7SH7eUtRtw07SuJaX3o,36548
 sbvt/imagetools.py,sha256=rZjArTuJkuSZOeuGWccRwyBsBxJMdvaWRwTxZuh0O-g,6269
 sbvt/timer.py,sha256=ciQJQUYSTChdIbsLiYiEzPa6yw8YwSqaeWc7DU4gSrE,548
-sbvt/visualtest.py,sha256=r1ubD4j6sJd5E4rMNLb4RjTOV6xCba923iKn7PKZnuQ,16070
-visualtest_python-1.5.1.dist-info/LICENSE,sha256=8vhEBNg7g2MxrQdwP-_ugxe3PDk5EbsBeMa--tc1xEA,1073
-visualtest_python-1.5.1.dist-info/METADATA,sha256=PaC6_Z4gFC4ZPRPDDsjJqzW32__DmvyBGNWvXC-imTI,3876
-visualtest_python-1.5.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-visualtest_python-1.5.1.dist-info/top_level.txt,sha256=t2tNJSI9vPU6KzikQCU2NYIJmbBaVTvOSJajc6IoRD0,5
-visualtest_python-1.5.1.dist-info/RECORD,,
+sbvt/visualtest.py,sha256=j6iWf7hszbEDkOZyZdjxhpLQawG9Gm0PMG34Idzm6_w,16511
+visualtest_python-1.5.2.dist-info/LICENSE,sha256=8vhEBNg7g2MxrQdwP-_ugxe3PDk5EbsBeMa--tc1xEA,1073
+visualtest_python-1.5.2.dist-info/METADATA,sha256=-tQTq4TqAOSVl4-0Krq0xVi9_eSfhpHmQ9p0OoGOmnI,3876
+visualtest_python-1.5.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+visualtest_python-1.5.2.dist-info/top_level.txt,sha256=t2tNJSI9vPU6KzikQCU2NYIJmbBaVTvOSJajc6IoRD0,5
+visualtest_python-1.5.2.dist-info/RECORD,,
```


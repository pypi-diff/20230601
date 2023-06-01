# Comparing `tmp/visualtest_python-1.3.2-py3-none-any.whl.zip` & `tmp/visualtest_python-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20590 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1129 b- defN 23-May-01 23:30 sbvt/__init__.py
--rw-r--r--  2.0 unx     9114 b- defN 23-Apr-26 16:54 sbvt/api.py
--rw-r--r--  2.0 unx    35178 b- defN 23-May-01 22:54 sbvt/browser.py
--rw-r--r--  2.0 unx     5981 b- defN 22-Sep-26 14:39 sbvt/imagetools.py
--rw-r--r--  2.0 unx      548 b- defN 22-Sep-26 14:39 sbvt/timer.py
--rw-r--r--  2.0 unx    11283 b- defN 23-May-01 22:55 sbvt/visualtest.py
--rw-r--r--  2.0 unx     1073 b- defN 23-May-02 18:15 visualtest_python-1.3.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3876 b- defN 23-May-02 18:15 visualtest_python-1.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 18:15 visualtest_python-1.3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-02 18:15 visualtest_python-1.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      869 b- defN 23-May-02 18:15 visualtest_python-1.3.2.dist-info/RECORD
-11 files, 69148 bytes uncompressed, 19132 bytes compressed:  72.3%
+Zip file size: 20358 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      121 b- defN 23-Jun-01 20:43 sbvt/__init__.py
+-rw-r--r--  2.0 unx     8453 b- defN 23-May-26 19:46 sbvt/api.py
+-rw-r--r--  2.0 unx    35100 b- defN 23-Jun-01 20:43 sbvt/browser.py
+-rw-r--r--  2.0 unx     6269 b- defN 23-Jun-01 20:43 sbvt/imagetools.py
+-rw-r--r--  2.0 unx      548 b- defN 23-May-08 21:54 sbvt/timer.py
+-rw-r--r--  2.0 unx    14314 b- defN 23-Jun-01 20:43 sbvt/visualtest.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jun-01 20:44 visualtest_python-1.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3876 b- defN 23-Jun-01 20:44 visualtest_python-1.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 20:44 visualtest_python-1.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-01 20:44 visualtest_python-1.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      868 b- defN 23-Jun-01 20:44 visualtest_python-1.4.0.dist-info/RECORD
+11 files, 70719 bytes uncompressed, 18900 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: sbvt/timer.py
 Comment: 
 
 Filename: sbvt/visualtest.py
 Comment: 
 
-Filename: visualtest_python-1.3.2.dist-info/LICENSE
+Filename: visualtest_python-1.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: visualtest_python-1.3.2.dist-info/METADATA
+Filename: visualtest_python-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: visualtest_python-1.3.2.dist-info/WHEEL
+Filename: visualtest_python-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: visualtest_python-1.3.2.dist-info/top_level.txt
+Filename: visualtest_python-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: visualtest_python-1.3.2.dist-info/RECORD
+Filename: visualtest_python-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbvt/__init__.py

```diff
@@ -1,35 +1,4 @@
-import logging
-import os.path
-
 # this import statement is here for context.py in tests folder
 from .visualtest import VisualTest
 
-__version__ = '1.3.2'
-
-logPath = 'logs'
-if not os.path.exists(logPath):
-    os.makedirs(logPath)
-
-# By generating a new logger as 'vt' we don't affect global logging from other packages
-# Each logger created in our package should be a child by prefacing with 'vt.childname'
-logger = logging.getLogger('vt')
-formatter = logging.Formatter('%(asctime)s [%(name)s][%(levelname)s] %(message)s')
-
-fileHandler = logging.FileHandler(os.path.join(logPath,'info.log'), mode='w')
-fileHandler.setFormatter(formatter)
-logger.addHandler(fileHandler)
-
-if "LOGGER_LEVEL" in os.environ:
-    LOGGER_LEVEL = os.environ["PROJECT_TOKEN"]
-    print(f'LOGGER_LEVEL: {LOGGER_LEVEL}')
-    logger.setLevel(level=LOGGER_LEVEL)
-else:
-    logger.setLevel(level='INFO')
-
-# decided to only add console logging from instantiation of VisualTesting class
-# - see visualtest.py
-# consoleHandler = logging.StreamHandler()
-# consoleHandler.setFormatter(formatter)
-# logger.addHandler(consoleHandler)
-# logger.setLevel(logging.WARNING)
-
+__version__ = '1.4.0'
```

## sbvt/api.py

```diff
@@ -9,30 +9,14 @@
 from requests.packages.urllib3.util.retry import Retry
 from dotenv import load_dotenv
 from colorama import Fore, Style
 
 load_dotenv()
 
 log = logging.getLogger(f'vt.{os.path.basename(__file__)}')
-env = os.environ["VT_ENV"].upper() if "VT_ENV" in os.environ else 'PROD'
-if env == "PROD":
-    host = "https://api.visualtest.io"
-    webUrl = "https://app.visualtest.io"
-    cdnUrl = "https://cdn.visualtest.io/browser-toolkit"
-elif env == "DEV":
-    host = "https://api.dev.visualtest.io"
-    webUrl = "https://app.dev.visualtest.io"
-    cdnUrl = "https://cdn.dev.visualtest.io/browser-toolkit"
-elif env == "INT":
-    host = "https://api.int.visualtest.io"
-    webUrl = "https://app.int.visualtest.io"
-    cdnUrl = "https://cdn.int.visualtest.io/browser-toolkit"
-else:
-    log.error(f'Invalid VT_ENV param: {env}. Please use DEV or INT')
-    raise Exception(f'Invalid VT_ENV param: {env}. Please use DEV or INT')
 
 api = requests.Session()
 s3 = requests.Session()
 
 
 # from https://findwork.dev/blog/advanced-usage-python-requests-timeouts-retries-hooks/
 class TimeoutHTTPAdapter(HTTPAdapter):
@@ -59,27 +43,40 @@
 api.mount("http://", adapter)
 s3.mount("https://", adapter)
 
 s3.headers.update({"Content-Type": "application/octet-stream"})
 
 class Api:
 
-    baseUrl = f'{host}/api/v1'
-    testRuns = []
+    baseUrl = None
+    webUrl = None
+    cdnUrl = None
+
+    @staticmethod
+    def setEnv(env):
+        if env != "prod":
+            print(f'overwritten env is: {env}')
+            Api.baseUrl = f'https://api.{env}.visualtest.io/api/v1'
+            Api.webUrl = f"https://app.{env}.visualtest.io"
+            Api.cdnUrl = f"https://cdn.{env}.visualtest.io/browser-toolkit"
+        else:
+            Api.baseUrl = 'https://api.visualtest.io/api/v1'
+            Api.webUrl = 'https://app.visualtest.io'
+            Api.cdnUrl = 'https://cdn.visualtest.io/browser-toolkit'
 
     def __init__(self, projectToken=None):
         self.projectToken = None
         self.projectId = None
         if projectToken:
             self.projectToken = projectToken
             self.projectId = projectToken.split("/")[0]
             api.headers.update({
                 'Authorization': f'Bearer {projectToken}',
                 'sbvt-client': 'sdk',
-                'sbvt-sdk': 'python', 
+                'sbvt-sdk': 'python',
                 'sbvt-sdk-version': sbvt.__version__
             })
         self.testRun = None
 
     def getDeviceInfo(self, userAgentInfo, driverCapabilities):
 
         url = f'{Api.baseUrl}/device-info/'
@@ -121,93 +118,85 @@
         })
         if response.status_code in range(200, 300):
             return response.json()
         else:
             log.error(f'Failed to create testRun. HTTP Response: {response.json()}')
             raise Exception(f'Failed to create testRun. HTTP Response: {response.json()}')
 
-    def saveImage(self, testRunName, imageData, filePath):
+    def saveImage(self, testRunName, imageData, imageBinary):
         log.info(f'Saving image for testRunName: {testRunName}')
 
         # TODO add this logic later with a flag
         # check if testRun already exists, if not create one
         if not self.testRun:
             self.testRun = self.createTestRun(testRunName)
-            Api.testRuns.append({"projectId": self.projectId, "testRunId": self.testRun["testRunId"] })
 
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
 
-        imageBinary = open(filePath, "rb")
         log.info(f'uploading image to: {result["uploadUrl"]}')
 
         response = s3.put(result['uploadUrl'], data=imageBinary)
         log.info(f'upload image response: {response}')
-        imageBinary.close()
 
         if response.status_code in range(200, 300):
             return result
         else:
             log.error(f'Failed to upload image. HTTP Response: {response.json()}')
             raise Exception(f'Failed to upload image. HTTP Response: {response.json()}')
 
     @staticmethod
     def getToolkit(scriptName=None):
-        if scriptName in ['user-agent','dom-capture','freeze-page','chrome-os-version']:
-            url = f'{cdnUrl}/{scriptName}.min.js'
+        if scriptName in ['user-agent','dom-capture','freeze-page','chrome-os-version','detect-chrome-headless']:
+            url = f'{Api.cdnUrl}/{scriptName}.min.js'
             response = api.get(url)
             return response.text
         else:
             log.error(f'Invalid scriptName for getToolkit from cdn: {scriptName}')
             raise Exception(f'Invalid scriptName for getToolkit from cdn: {scriptName}')
 
-    @staticmethod
-    def printReport():
+    def printReport(self):
+
+        url = f'{Api.baseUrl}/projects/{self.projectId}/testruns/{self.testRun["testRunId"]}/images'
+        response = api.get(url).json()
+        imageCount = response["page"]["totalItems"]
+        print(f'View your {imageCount} {"capture" if imageCount == 1 else "captures"} here: ' + Fore.BLUE + f'{Api.webUrl}/projects/{response["items"][0]["projectId"]}/testruns/{response["items"][0]["testRunId"]}/comparisons'+ Style.RESET_ALL)
+
+        comparisonUrl = f'{Api.baseUrl}/projects/{self.projectId}/testruns/{self.testRun["testRunId"]}?expand=comparison-totals'
+        comparisons = {"complete": 0}
+        maxLoops = 20
+        countLoops = 0
+        while comparisons["complete"] != imageCount and countLoops <= maxLoops:
+            time.sleep(0.25)
+            log.info(f'imageCount: {imageCount} != comparisonTotal: {comparisons["complete"]} -- mismatch... running again for testRun {self.testRun} countLoops: {countLoops}')
+            comparisonResult = api.get(comparisonUrl).json()
+            comparisons = comparisonResult["comparisons"]
+            countLoops += 1
+
+        try:
+            # print(f'Comparisons: {str(comparisons)}')
+            new = comparisons["status"]["new_image"]
+            failed = comparisons["status"]["unreviewed"]
+            passed = comparisons["status"]["passed"]
+
+            if new:
+                print(Style.BRIGHT + Fore.YELLOW + f'\t{new} new base {"image" if new == 1 else "images"}' + Style.RESET_ALL)
+            if failed:
+                print(Style.BRIGHT + Fore.RED + f'\t{failed} image comparison {"failure" if failed == 1 else "failures"} to review' + Style.RESET_ALL)
+            if passed:
+                print(Style.RESET_ALL + Style.BRIGHT + Fore.GREEN + f'\t{passed} image comparisons passed' + Style.RESET_ALL)
+            if comparisons["complete"] != imageCount:
+                print(Style.BRIGHT + Fore.MAGENTA + f'\tTimed out getting comparisons results' + Style.RESET_ALL)
+        except Exception as e:
+            print(Style.BRIGHT + Fore.MAGENTA + f'\tError getting comparisons results: {str(e)}' + Style.RESET_ALL)
 
-        for testRun in Api.testRuns:
-            if not testRun["testRunId"]:  # logic to check if the users tests failed before a 'saveImage'
-                continue
-
-            url = f'{Api.baseUrl}/projects/{testRun["projectId"]}/testruns/{testRun["testRunId"]}/images'
-            response = api.get(url).json()
-            imageCount = response["page"]["totalItems"]
-            print(f'View your {imageCount} {"capture" if imageCount == 1 else "captures"} here: ' + Fore.BLUE + f'{webUrl}/projects/{response["items"][0]["projectId"]}/testruns/{response["items"][0]["testRunId"]}/comparisons'+ Style.RESET_ALL)
-
-            comparisonUrl = f'{Api.baseUrl}/projects/{testRun["projectId"]}/testruns/{testRun["testRunId"]}?expand=comparison-totals'
-            comparisons = {"complete": 0}
-            maxLoops = 20
-            countLoops = 0
-            while comparisons["complete"] != imageCount and countLoops <= maxLoops:
-                time.sleep(0.25)
-                log.info(f'imageCount: {imageCount} != comparisonTotal: {comparisons["complete"]} -- mismatch... running again for testRun {testRun} countLoops: {countLoops}')
-                comparisonResult = api.get(comparisonUrl).json()
-                comparisons = comparisonResult["comparisons"]
-                countLoops += 1
-
-            try:
-                # print(f'Comparisons: {str(comparisons)}')
-                new = comparisons["status"]["new_image"]
-                failed = comparisons["status"]["unreviewed"]
-                passed = comparisons["status"]["passed"]
-
-                if new:
-                    print(Style.BRIGHT + Fore.YELLOW + f'\t{new} new base {"image" if new == 1 else "images"}' + Style.RESET_ALL)
-                if failed:
-                    print(Style.BRIGHT + Fore.RED + f'\t{failed} image comparison {"failure" if failed == 1 else "failures"} to review' + Style.RESET_ALL)
-                if passed:
-                    print(Style.RESET_ALL + Style.BRIGHT + Fore.GREEN + f'\t{passed} image comparisons passed' + Style.RESET_ALL)
-                if comparisons["complete"] != imageCount:
-                    print(Style.BRIGHT + Fore.MAGENTA + f'\tTimed out getting comparisons results' + Style.RESET_ALL)
-            except Exception as e:
-                print(Style.BRIGHT + Fore.MAGENTA + f'\tError getting comparisons results: {str(e)}' + Style.RESET_ALL)
 
-atexit.register(Api.printReport)
```

## sbvt/browser.py

```diff
@@ -1,13 +1,14 @@
 import os
 import time
 import shutil
 import math
 import logging
 import json
+from sys import getsizeof
 from .imagetools import ImageTools
 from .timer import StopWatch
 from .api import Api
 from selenium.webdriver.common.by import By
 
 log = logging.getLogger(f'vt.{os.path.basename(__file__)}')
 
@@ -27,48 +28,43 @@
             - MAX_TIME_MIN (float): Max time to create fullpage image.  Default is 3.5 minutes. Can be set to a max of 10 minutes. 
     Returns:
         Class instance
     """
 
     def __init__(self, driver, limits: dict = {}):
 
-        if not driver:
-            raise Exception('driver argument is required!')
-
-        if not driver.session_id:
-            raise Exception('driver argument does not have a session_id!')
-
-        if not driver.capabilities:
-            raise Exception('driver argument does not have capabilities!')
-
         # setup api
         self._userAgentScript = Api.getToolkit('user-agent')
         self._domCaptureScript = Api.getToolkit('dom-capture')
         self._freezePageScript = Api.getToolkit('freeze-page')
         self._chromeOsVersion = Api.getToolkit('chrome-os-version')
+        self._detectChromeHeadless = Api.getToolkit('detect-chrome-headless')
         self._api = Api()
         log.info(f'Capabilities from driver: {driver.capabilities}')
         self._driver = driver
         self._userAgentInfo = self.getNavigatorUserAgentData(self._driver)
         self._deviceInfo = self._api.getDeviceInfo(self._userAgentInfo, driver.capabilities)
         log.info(f'Final device info: {self._deviceInfo}')
 
+        # check browser running in headless mode or not after getting user-agent script
+        self._headless = self.detectHeadlessMode(driver)
+
         log.info(f'limits: {limits}')
         if 'MAX_IMAGE_PIXELS' in limits:
             ImageTools.setMaxImagePixels(limits['MAX_IMAGE_PIXELS'])
 
         if 'MAX_TIME_MIN' in limits:
             self.MAX_TIME_MIN = limits['MAX_TIME_MIN']
         else:
             self._MAX_TIME_MIN = DEFAULT_MAX_TIME_MIN
 
         # default options
         self._scrollMethod = 'CSS_TRANSLATE'
-        self._debugImages = False
-        self._saveDOM = False
+        self._debug = False
+        self._debugDir = None
 
     @property
     def scrollMethod(self):
         return self._scrollMethod
 
     @scrollMethod.setter
     def scrollMethod(self, s):
@@ -79,32 +75,33 @@
             raise Exception(f'Invalid scrollMethod: "{s}". Options are {str(scroll_options)}')
 
     @property
     def capabilities(self):
         return self._driver.capabilities
 
     @property
-    def debugImages(self):
-        return self._debugImages
+    def debugDir(self):
+        return self._debugDir
 
-    @debugImages.setter
-    def debugImages(self, debug):
-        if type(debug) == bool:
-            self._debugImages = debug
+    @debugDir.setter
+    def debugDir(self, debugDir):
+        
+        if type(debugDir) == str or debugDir == None:
+            self._debugDir = debugDir
         else:
-            raise Exception(f'Argument must be a boolean!')
+            raise Exception(f'Argument must be a string!')
 
     @property
-    def saveDOM(self):
-        return self._saveDOM
+    def debug(self):
+        return self._debug
 
-    @saveDOM.setter
-    def saveDOM(self, save):
-        if type(save) == bool:
-            self._saveDOM = save
+    @debug.setter
+    def debug(self, debug):
+        if type(debug) == bool:
+            self._debug = debug
         else:
             raise Exception(f'Argument must be a boolean!')
 
     @property
     def MAX_TIME_MIN(self):
         return self._MAX_TIME_MIN
 
@@ -125,28 +122,35 @@
             osVersion = driver.execute_async_script(self._chromeOsVersion)
             if osVersion:
                 agent['osVersion'] = osVersion
             log.info(f'osVersion for chrome-based browser: {agent["osVersion"]}')
 
         return agent
 
-    def captureDom(self, driver, path, type=""):
+    def detectHeadlessMode(self, driver):
+        headless = None
+        agent = self._userAgentInfo
+        if 'browserName' in agent and agent['browserName'] in ['chrome', 'edge', 'opera', 'samsunginternet']:
+            headless = driver.execute_script(f'return {self._detectChromeHeadless};')
+            log.info(f'headless flag for chrome-based browser: {headless}')
+        if driver.capabilities['browserName'] == 'firefox' and driver.capabilities['moz:headless']:
+            headless = driver.capabilities['moz:headless']
+            log.info(f'headless flag for firefox browser: {headless}')
+        return headless
+
+    def captureDom(self, driver, type=""):
         """ Using a custom predefined script, capture the webpage's DOM element information """
         domString = driver.execute_script(f'return {self._domCaptureScript};')
 
         # add screenshot type and dump back to JSON string
         dom = json.loads(domString)
         dom['screenshotType'] = type
         domString = json.dumps(dom)
         # log.debug(f'Dom-capture: {dom}')
 
-        if self._saveDOM: # save at same location and filename as screenshot
-            with open(path.replace('.png','.json'), 'w') as outfile:
-                json.dump(dom, outfile, indent=4)
-
         return dom
 
     def _findElement(self, cssSelector):
         return self._driver.find_element(By.CSS_SELECTOR, cssSelector)
 
     def _clearIgnoreElements(self):
         script = 'delete window.sbvt'
@@ -196,17 +200,16 @@
         self.viewportWidth = dimensions['windowInner']['width']
         self.fullpageHeight = dimensions['fullpage']['height']
         self.fullpageWidth = dimensions['fullpage']['width']
         self.devicePixelRatio = dimensions['devicePixelRatio']
         log.info(f'devicePixelRatio: {self.devicePixelRatio}')
         # validate the viewport from javascript matches 
         # what we actually get from a png
-        file = os.path.join(self.tmpDir, f'size-test.png')
-        self._driver.save_screenshot(file)
-        testImageWidth, testImageHeight = ImageTools.getImageSize(file)
+        imageBinary = self._driver.get_screenshot_as_png()
+        testImageWidth, testImageHeight = ImageTools.getImageSize(imageBinary)
         log.info(f'Size Test: image dimensions: {testImageWidth}x{testImageHeight}')
 
         self._cropEachBottom = None
         self._cropEachTop = None
 
         expectedWidth = math.ceil(self.viewportWidth * self.devicePixelRatio)
         expectedHeight = math.ceil(self.viewportHeight * self.devicePixelRatio)
@@ -383,52 +386,40 @@
             term = 'grew' if newFullpageHeight > self.fullpageHeight else 'shrank'
             log.info(f'Fullpage height {term}, was {self.fullpageHeight}, now is {newFullpageHeight}')
             self.fullpageHeight = newFullpageHeight
             changed = True
 
         return changed
 
-    def _createTmpDir(self, path, screenshotType):
-        current_time = time.strftime("%H-%M-%S", time.localtime()) # removed the ":" because throw error with windows
-        self.tmpDir = os.path.join(path, f'.temp-images-{screenshotType}-{current_time}')
-        os.makedirs(self.tmpDir)
-        log.info(f'Made tmp images directory for {screenshotType} screenshot: {self.tmpDir}')
-
-    def _deleteTmpDir(self):
-        # there can only be one screenshot happening at a time,
-        # hence there can only be one tmpDir referenced on self
-        try:
-            shutil.rmtree(self.tmpDir)
-            log.info(f'Deleted tmp images directory: {self.tmpDir}')
-            self.tmpDir = None
-        except OSError as e:
-            log.warning(f'Error deleting tmp directory: {e.filename} - {e.strerror}.')
-
-    def takeFullpageScreenshot(self, path: str, options):
+    def takeFullpageScreenshot(self, name, options):
         """
         Will take a fullpage screenshot and place the image at the path provided. \n
         Note this places a temporary folder at the current directory with the name sbTemp-{time}
         Args:
             path (str): the directory for where to save the image
             lazyload (int): if set, will scroll the page to load any content first and wait the number of milliseconds provided between each scroll
         """
+        imageBinary = bytearray()  # New empty byte array
 
         if self._deviceInfo['osName'] == 'ios':
             raise Exception('iOS devices do no currently support fullpage screenshots.')
 
         log.info(f'Taking full page screenshot at URL: {self._driver.current_url}')
-        if '.png' not in path:
-            raise Exception('Fullpage Screenshot path must end in a .png')
 
         # limit how long we let a screenshot run
         self.fullpageStopWatch = StopWatch()
         self.fullpageStopWatch.start()
 
-        # create tmp directory for storing images that will be stitched together
-        self._createTmpDir(os.path.dirname(path), 'fullpage')
+        # create images directory for debug
+        debugImageDir = None
+        debugImageName = None
+        debugImagePath = None
+        if self._debug and self._debugDir:
+            debugImageDir = os.path.join(self._debugDir, f'{name}-fullpage')
+            os.makedirs(debugImageDir)
 
         # get initial page state for returning to later (must do before hiding scrollbar)
         self._getInitialPageState()
 
         # hide scroll bar for accurate dimensions
         hideScrollBarResult = self._driver.execute_script('return document.body.style.overflow="hidden";')
         log.info(f'PREP: Hide scrollbar result: {hideScrollBarResult}')
@@ -455,29 +446,33 @@
             freezePageResult = None
             if 'freezePage' in options:
                 if options['freezePage']:
                     freezePageResult = self._freezePage()
             else:
                 freezePageResult = self._freezePage()
 
-            file = os.path.join(self.tmpDir, f'0.png')
-            self._driver.save_screenshot(file)
+            imageBinary = self._driver.get_screenshot_as_png()
 
-            if self._cropEachBottom:
-                file = ImageTools.cropBottom(file, self._cropEachBottom)
+            if self._debug:
+                debugImageName = '0.png'
+                debugImagePath = os.path.join(debugImageDir, debugImageName)
+                with open(debugImagePath, 'wb') as outfile:
+                    outfile.write(imageBinary)
+                    outfile.close()
 
+            if self._cropEachBottom:
+                imageBinary = ImageTools.cropBottom(imageBinary, self._cropEachBottom, debugImagePath)
+                
             if self._cropEachTop:
-                file = ImageTools.cropTop(file, self._cropEachTop)
+                imageBinary = ImageTools.cropTop(imageBinary, self._cropEachTop, debugImagePath)
 
-            # copy file to save path
-            shutil.copy(file, path)
             reasonStopped = 'IS_SINGLE_PAGE'
 
             # capture dom AFTER creating screenshot but BEFORE displaying scrollbar again (else get vertical offset on dom elements to image)
-            self.dom = self.captureDom(self._driver, path, 'fullpage')
+            self.dom = self.captureDom(self._driver, 'fullpage')
 
             log.info(f'Setting document.body.style.overflow back to initial state: {self.initialPageState["overflow"]}')
             self._driver.execute_script(f'document.body.style.overflow="{self.initialPageState["overflow"]}"')
 
             pageTime = pageStopWatch.stop()
             averagePageTime = round(pageTime, 2)
 
@@ -535,22 +530,28 @@
                             # handles infinite-scroll or lazy loaded content
                             self._scrollPage(pageIndex)
 
                 # check if we should stop scrolling due to a limit
                 hitLimit, reasonStopped = self._checkScrollingLimits(pageIndex, totalPages)
 
                 # take the selenium screenshot
-                file = os.path.join(self.tmpDir, f'{pageIndex}.png')
-                self._driver.save_screenshot(file)
+                viewportImage = self._driver.get_screenshot_as_png()
+
+                if self._debug:
+                    debugImageName = f'{pageIndex}.png'
+                    debugImagePath = os.path.join(debugImageDir, debugImageName)
+                    with open(debugImagePath, 'wb') as outfile:
+                        outfile.write(viewportImage)
+                        outfile.close()
 
                 if self._cropEachBottom:
-                    file = ImageTools.cropBottom(file, self._cropEachBottom)
+                    viewportImage = ImageTools.cropBottom(viewportImage, self._cropEachBottom, debugImagePath)
 
                 if self._cropEachTop:
-                    file = ImageTools.cropTop(file, self._cropEachTop)
+                    viewportImage = ImageTools.cropTop(viewportImage, self._cropEachTop, debugImagePath)
 
                 # crop image as necessary
                 if self._scrollMethod == 'CSS_TRANSLATE':
 
                     """
                     When using translate, the last page will be shifted up past the true
                     bottom of the page. We need to crop off the extra "white" space that 
@@ -564,15 +565,15 @@
                     """
 
                     cropHeight = self.viewportHeight - (self.fullpageHeight % self.viewportHeight)
                     numPixels = cropHeight * self.devicePixelRatio
 
                     if pageIndex == totalPages - 1 and numPixels > 0:
                         log.info(f'Cropping bottom of last image: {numPixels}px')
-                        file = ImageTools.cropBottom(file, numPixels)  # will reference cropped file
+                        viewportImage = ImageTools.cropBottom(viewportImage, numPixels, debugImagePath)  # will reference cropped file
 
                 elif self._scrollMethod == 'JS_SCROLL':
 
                     """
                     When using window.scrollTo(), the last page will not scroll a full
                     viewport and our last image will have content at the top that duplicates
                     content from previous screenshot. So, we need to crop the top of the image
@@ -581,18 +582,18 @@
                     To calculate, subtract the scrolled offset from total viewports scrolled
                     and multiply by devicePixelRatio to get the actual pixels for image crop.
                     """
                     cropHeight = pageIndex * self.viewportHeight - self._getScrollOffset()
                     numPixels = cropHeight * self.devicePixelRatio
                     if hitLimit and reasonStopped == 'HIT_BOTTOM' and numPixels > 0:
                         log.info(f'Cropping top of last image: {numPixels}px')
-                        file = ImageTools.cropTop(file, numPixels)  # will reference cropped file
+                        viewportImage = ImageTools.cropTop(viewportImage, numPixels, debugImagePath)  # will reference cropped file
 
-                screenshots.append(file)
-                self.approxDiskSize += os.path.getsize(file)
+                screenshots.append(viewportImage)
+                self.approxDiskSize += getsizeof(viewportImage)
 
                 # we are done if we didn't actually scroll or hit a scrolling limit
                 done = not scrolled or hitLimit
                 pageTime = pageStopWatch.stop()
                 totalPageTime += pageTime
                 log.debug(f'Scroll and capture page time: {pageTime}s')
 
@@ -607,15 +608,15 @@
 
             elif self._scrollMethod == 'JS_SCROLL':
                 #scroll back to the top
                 self._driver.execute_script('window.scrollTo(0,0)')
                 time.sleep(0.75) # wait a half sec to allow dom to settle before capturing
 
             # capture dom AFTER creating screenshot but BEFORE setting back to initial states
-            self.dom = self.captureDom(self._driver, path, 'fullpage')
+            self.dom = self.captureDom(self._driver, 'fullpage')
 
             # Setting document.body.style.transform back
             log.info(f'Setting document.body.style.transform back to initial state: {self.initialPageState["transform"]}')
             self._driver.execute_script(f'document.body.style.transform="{self.initialPageState["transform"]}"')
             
             # Setting scroll position back
             log.info(f'Scrolling back to initial scroll offset ({self.initialPageState["scrollX"]},{self.initialPageState["scrollY"]})')
@@ -626,27 +627,27 @@
             log.info(f'Setting document.body.style.overflow back to initial state: {self.initialPageState["overflow"]}')
             self._driver.execute_script(f'document.body.style.overflow="{self.initialPageState["overflow"]}"')
 
             # TODO: technically we could return control back to user here??
 
             # build the fullpage image from individual screenshots
             log.info(f'Stitching screenshots for final fullpage image')
-            ImageTools.stitchImages(screenshots, path)
+            imageBinary = ImageTools.stitchImages(screenshots)
         
 
         # validate final fullpage image dimensions
-        imageWidth, imageHeight = ImageTools.getImageSize(path)
+        imageWidth, imageHeight = ImageTools.getImageSize(imageBinary)
 
         expectedImageWidth = self.fullpageWidth * self.devicePixelRatio
         expectedImageHeight = self.fullpageHeight * self.devicePixelRatio
 
         totalFullpageTime = self.fullpageStopWatch.stop()
         log.info(f'Total fullpage time duration: {totalFullpageTime} seconds')
         result = {
-            'imagePath': path,
+            'imagePath': None,
             'imageSize': {
                 'width': imageWidth,
                 'height': imageHeight
             },
             'expectedSize': {
                 'width': expectedImageWidth,
                 'height': expectedImageHeight
@@ -657,34 +658,30 @@
             'averagePageTime': f'{averagePageTime} seconds',
             'url': self._driver.current_url,
             'freezePageResult': freezePageResult
         }
 
         log.info(f'Result: {result}')
         result['dom'] = self.dom #add dom after logging result
-
-        # delete the temp screenshot images used to build fullpage
-        if not self._debugImages:
-            self._deleteTmpDir()
+        result['imageBinary'] = imageBinary
 
         return result
 
-    def takeElementScreenshot(self, path, options):
+    def takeElementScreenshot(self, options):
         """
         Will take an element screenshot and place the image at the path provided. \n
         Args:
             element (WebElement): The reference to the Selenium WebElement to capture a screenshot of
             path (str): the directory for where to save the image
         """
         # measure how long it takes
         self.watch = StopWatch()
         self.watch.start()
 
-        # create tmp directory for storing images that will be stitched together
-        self._createTmpDir(os.path.dirname(path), 'element')
+        imageBinary = bytearray()  # New empty byte array
 
         # freezePage script
         freezePageResult = None
         if 'freezePage' in options:
             if options['freezePage']:
                 freezePageResult = self._freezePage()
         else:
@@ -692,56 +689,53 @@
 
         # update the dimensions of the browser window and webpage
         self._getPageDimensions()
 
         # selenium.webdriver.firefox.webelement.FirefoxWebElement
         log.debug(f'type of element is {type(options["element"])}')
         log.info(f'Taking element screenshot of element')
-        options["element"].screenshot(path)
+        imageBinary = options["element"].screenshot_as_png
 
         # capture dom AFTER creating screenshot
-        self.dom = self.captureDom(self._driver, path, 'element')
+        self.dom = self.captureDom(self._driver, 'element')
 
         # validate final fullpage image dimensions
-        imageWidth, imageHeight = ImageTools.getImageSize(path)
+        imageWidth, imageHeight = ImageTools.getImageSize(imageBinary)
 
         totalTime = self.watch.stop()
         result = {
-            'imagePath': path,
+            'imagePath': None,
             'imageSize': {
                 'width': imageWidth,
                 'height': imageHeight
             },
             'duration': f'{totalTime} seconds',
             'url': self._driver.current_url,
             'freezePageResult': freezePageResult
         }
 
         log.info(f'Result: {result}')
         result['dom'] = self.dom #add dom after logging result
-
-        if not self._debugImages:
-            self._deleteTmpDir()
+        result['imageBinary'] = imageBinary
 
         return result
 
-    def takeViewportScreenshot(self, path, options):
+    def takeViewportScreenshot(self, options):
         """
         Will take a screenshot of the browser viewport and place the image at the path provided. \n
         Args:
             path (str): the directory for where to save the image
         """
         log.info(f'Taking screenshot of viewport')
 
         # measure how long it takes
         self.watch = StopWatch()
         self.watch.start()
 
-        # create tmp directory for storing images that will be stitched together
-        self._createTmpDir(os.path.dirname(path), 'viewport')
+        imageBinary = bytearray()  # New empty byte array
 
         # freezePage script
         freezePageResult = None
         if 'freezePage' in options:
             if options['freezePage']:
                 freezePageResult = self._freezePage()
         else:
@@ -753,42 +747,38 @@
         # hide scroll bar for accurate dimensions
         hideScrollBarResult = self._driver.execute_script('return document.body.style.overflow="hidden";')
         log.info(f'PREP: Hide scrollbar result: {hideScrollBarResult}')
 
         # update the dimensions of the browser window and webpage
         self._getPageDimensions()
 
-        file = os.path.join(self.tmpDir, f'viewport.png')
-        self._driver.save_screenshot(file)
+        imageBinary = self._driver.get_screenshot_as_png()
 
         if self._cropEachBottom:
-            file = ImageTools.cropBottom(file, self._cropEachBottom)
+            imageBinary = ImageTools.cropBottom(imageBinary, self._cropEachBottom)
 
         if self._cropEachTop:
-            file = ImageTools.cropTop(file, self._cropEachTop)
-
-        # copy file to save path
-        shutil.copy(file, path)
+            imageBinary = ImageTools.cropTop(imageBinary, self._cropEachTop)
 
         # capture dom AFTER creating screenshot but BEFORE displaying scrollbar again (else get vertical offset on dom elements to image)
-        self.dom = self.captureDom(self._driver, path, 'viewport')
+        self.dom = self.captureDom(self._driver, 'viewport')
 
         log.info(f'Setting document.body.style.overflow back to initial state: {self.initialPageState["overflow"]}')
         self._driver.execute_script(f'document.body.style.overflow="{self.initialPageState["overflow"]}"')
 
         # validate final fullpage image dimensions
-        imageWidth, imageHeight = ImageTools.getImageSize(path)
+        imageWidth, imageHeight = ImageTools.getImageSize(imageBinary)
 
         expectedImageWidth = self.viewportWidth * self.devicePixelRatio
         expectedImageHeight = self.viewportHeight * self.devicePixelRatio
 
         totalTime = self.watch.stop()
         log.info(f'Total viewport capture time duration: {totalTime} seconds')
         result = {
-            'imagePath': path,
+            'imagePath': None,
             'imageSize': {
                 'width': imageWidth,
                 'height': imageHeight
             },
             'expectedSize': {
                 'width': expectedImageWidth,
                 'height': expectedImageHeight
@@ -797,12 +787,9 @@
             'duration': f'{totalTime} seconds',
             'url': self._driver.current_url,
             'freezePageResult': freezePageResult
         }
 
         log.info(f'Result: {result}')
         result['dom'] = self.dom #add dom after logging result
-
-        if not self._debugImages:
-            self._deleteTmpDir()
-
+        result['imageBinary'] = imageBinary
         return result
```

## sbvt/imagetools.py

```diff
@@ -1,10 +1,11 @@
+import io
 import os
 import logging
-from pathlib import Path
+from io import BytesIO
 from PIL import Image, ImageChops
 import numpy
 
 log = logging.getLogger(f'vt.{os.path.basename(__file__)}')
 
 class ImageTools:
 
@@ -38,82 +39,85 @@
 
         result = Image.new('RGB', (result_width, result_height))
         result.paste(im=image1, box=(0, 0))
         result.paste(im=image2, box=(0, height1))
         return result
 
     @staticmethod
-    def stitchImages(images, outputFile):
+    def stitchImages(images):
 
         if len(images) == 0:
             log.error('Could not stitch files as none were found.')
             return
 
-        bigImage = Image.open(images[0])
+        bigImage = Image.open(BytesIO(images[0]))
 
         for i in range(1,len(images)):
-            if os.path.exists(images[i]):
-                nextImage = Image.open(images[i])
-            else:
-                raise Exception(f'Image reference did not exist in temp images folder: {images[i]}')
+            nextImage = Image.open(BytesIO(images[i]))
             bigImage = ImageTools.mergeImages(bigImage, nextImage)
             nextImage.close()
 
-        bigImage.save(outputFile)
+        imageBuffer = io.BytesIO()
+        bigImage.save(imageBuffer, format='png')
         bigImage.close()
+        return imageBuffer.getvalue()
 
     @staticmethod
     def getImageSize(imagePath):
-        image = Image.open(imagePath)
+        image = Image.open(BytesIO(imagePath))
         size = image.size
         image.close()
         return size
 
     @staticmethod
-    def cropTop(imagePath, numPixels):
+    def cropTop(imageBinary, numPixels, debugImagePath=None):
         if numPixels == 0:
-            return imagePath
+            return imageBinary
 
-        image = Image.open(imagePath)
+        image = Image.open(BytesIO(imageBinary))
         width, height = image.size
-        croppedImagePath = imagePath.replace('.png', '_cropped_top.png')
-        image.crop((0, numPixels, width, height)).save(croppedImagePath)
+        imageBuffer = io.BytesIO()
+        image.crop((0, numPixels, width, height)).save(imageBuffer, format='png')
+        if debugImagePath: 
+            image.crop((0, numPixels, width, height)).save(debugImagePath.replace('.png', '_cropped_top.png'))
         image.close()
-        return croppedImagePath
+        return imageBuffer.getvalue()
 
     @staticmethod
-    def cropBottom(imagePath, numPixels):
+    def cropBottom(imageBinary, numPixels, debugImagePath=None):
         if numPixels == 0:
-            return imagePath
+            return imageBinary
 
-        image = Image.open(imagePath)
+        image = Image.open(BytesIO(imageBinary))
         width, height = image.size
-        croppedImagePath = imagePath.replace('.png', '_cropped_bottom.png')
-        image.crop((0, 0, width, height-numPixels)).save(croppedImagePath)
+        imageBuffer = io.BytesIO()
+        image.crop((0, 0, width, height-numPixels)).save(imageBuffer, format='png')
+        if debugImagePath: 
+            image.crop((0, 0, width, height-numPixels)).save(debugImagePath.replace('.png', '_cropped_bottom.png'))
         image.close()
-        return croppedImagePath
+        return imageBuffer.getvalue()
 
     @staticmethod
     def imagesMatch(pathOne, pathTwo):
-        imageOne = Image.open(pathOne)
-        imageTwo = Image.open(pathTwo)
+        imageOne = Image.open(BytesIO(pathOne))
+        imageTwo = Image.open(BytesIO(pathTwo))
 
         diff = ImageChops.difference(imageOne, imageTwo)
         imageOne.close()
         imageTwo.close()
 
         if diff.getbbox():
             return False
         else:
             return True
 
     @staticmethod
     def imageDiff(pathOne, pathTwo):
-        imageOne = Image.open(pathOne)
-        imageTwo = Image.open(pathTwo)
+        imageOne = Image.open(BytesIO(pathOne))
+        imageTwo = Image.open(BytesIO(pathTwo))
 
         diff = ImageChops.difference(imageOne, imageTwo)
         imageOne.close()
         imageTwo.close()
 
         return diff
```

## sbvt/visualtest.py

```diff
@@ -1,11 +1,12 @@
 import json
 import os
 import logging
-from pathlib import Path
+import time
+
 from .browser import Browser
 from .imagetools import ImageTools
 from .api import Api
 
 log = logging.getLogger(f'vt.{os.path.basename(__file__)}')
 
 class VisualTest:
@@ -15,66 +16,90 @@
     Args:
         driver: Selenium webdriver with active session
         settings: Dictionary of user settings
             - projectToken (str): Unique API token for your project. (required)
             - testRunName (str): Test Run Name - defaults to OS / Browser versions if not provided (optional)
             - saveTo (str): The directory to which images should be saved. (default is your working directory/results/)
         settings: Dictionary of developer settings
-            - debugLogs (bool): Prints logs to stdout in addition to log file
-            - debugImages (bool): Keeps temp folder of images used to build fullpage screenshots
-            - saveDOM (bool): Saves DOM JSON file to same saveTo location
+            - debug (bool): 
+                Creates sbvt_debug folder with log file
+                Keeps temp folder of images used to build fullpage screenshots
+                Saves DOM JSON file
         limits: Dictionary of values to change default limits during creation fullpage images (not recommended)
             - MAX_IMAGE_PIXELS (int): Max fullpage image size. (default INT32 or 2^31)
             - MAX_TIME_MIN (float): Max time to create fullpage image.  Default is 3.5 minutes. Can be set to a max of 10 minutes. 
     Returns:
         Class instance
     """
 
-    # imitate static variable across instances
-    _consoleLogHandler = None
-
     def __init__(self, driver, settings: dict={}, limits: dict={}):
-        log.info(f'Instantiated with settings: {settings}, limits: {limits}')
 
+        if not driver:
+            raise Exception('driver argument is required!')
+
+        if not driver.session_id:
+            raise Exception('driver argument does not have a session_id!')
+
+        if not driver.capabilities:
+            raise Exception('driver argument does not have capabilities!')
+        
         # must do this first to get debug logs
-        if 'debugLogs' in settings and type(settings['debugLogs']) == bool:
-            self._handleLoggerSetting(settings['debugLogs'])
+        self._debug = False
+        self._debugDir = None
+        if 'debug' in settings:
+            if (type(settings['debug']) == bool):
+                if (settings['debug']):
+                    self._debug = True
+                    subfolder = time.strftime("%m-%d_%H-%M-%S", time.localtime()) + "_" + driver.session_id
+                    self._debugDir = os.path.join('sbvt_debug',  subfolder)
+                    os.makedirs(self._debugDir, exist_ok=True)
+                    self._startLogger(self._debugDir)
+            else:
+                raise Exception('debug argument must be a boolean')
+
+        log.info(f'Instantiated with settings: {settings}, limits: {limits}')
+
+        if 'projectToken' in settings:
+            if '_' in settings['projectToken']:
+                projectToken = settings['projectToken']
+                env = projectToken.split('_')[1]
+            else:
+                env = "prod"
+            Api.setEnv(env)
 
         self.browser = Browser(driver, limits)
+        self.browser.debug =  self._debug
+        self.browser.debugDir =  self._debugDir
         self._sessionId = driver.session_id
         self._settings = {
             'projectToken': None,
             'testRunName': None,
             'saveTo': None
         }
 
         # user-configurable project information
         if not 'projectToken' in settings:
             raise Exception('"projectToken" property in settings is required!')
         self._settings['projectToken'] = settings['projectToken']
+        
         if 'testRunName' in settings:
             self._settings['testRunName'] = settings['testRunName']
         else:
             if self.browser._deviceInfo["osName"] == 'macos':
                 osNamePretty = 'macOS'
             else:
                 osNamePretty = self.browser._deviceInfo["osName"].capitalize()
             self._settings['testRunName'] = f'{osNamePretty} {self.browser._deviceInfo["osVersion"]} / {self.browser._deviceInfo["browserName"].capitalize()} {self.browser._deviceInfo["browserVersion"]}'
 
         if 'saveTo' in settings:
             self.saveTo = os.path.join(settings['saveTo'])
-        else:
-            self.saveTo = os.path.join(os.getcwd(),'results')
-        
-        if 'debugImages' in settings and type(settings['debugImages']) == bool:
-            self.browser.debugImages = settings['debugImages']
-        
-        if 'saveDOM' in settings and type(settings['saveDOM']) == bool:
-            self.browser.saveDOM = settings['saveDOM']
-        
+
+        if 'debug' in settings and type(settings['debug']) == bool:
+            self.browser.debug = settings['debug']
+
         # setup api
         self._api = Api(self._settings['projectToken'])
         
         log.info(f'final instance settings: {self._settings}')
 
     @property
     def projectToken(self):
@@ -159,27 +184,21 @@
         """
         return self.browser.MAX_TIME_MIN
 
     @MAX_TIME_MIN.setter
     def MAX_TIME_MIN(self, minutes):
         self.browser.MAX_TIME_MIN = minutes
 
-    def _handleLoggerSetting(self, enableDebugLogs):
-        ClassName = type(self)
-        if enableDebugLogs == True:
-            if ClassName._consoleLogHandler == None:
-                logger = logging.getLogger('vt') #top-level logger created in __init__.py
-                ClassName._consoleLogHandler = logging.StreamHandler()
-                ClassName._consoleLogHandler.setFormatter(logging.Formatter('[VisualTesting][%(levelname)s] %(message)s'))
-                logger.addHandler(ClassName._consoleLogHandler)
-                logger.setLevel(logging.DEBUG)
-        else:
-            if ClassName._consoleLogHandler != None:
-                logger = logging.getLogger('vt') #top-level logger created in __init__.py
-                logger.removeHandler(ClassName._consoleLogHandler)
+    def _startLogger(self, logPath):
+        logger = logging.getLogger('vt')
+        formatter = logging.Formatter('%(asctime)s [%(name)s][%(levelname)s] %(message)s')
+        fileHandler = logging.FileHandler(os.path.join(logPath, 'debug.log'), mode='w')
+        fileHandler.setFormatter(formatter)
+        logger.addHandler(fileHandler)
+        logger.setLevel(logging.DEBUG)
 
     def capture(self, name, options: dict={}):
         """
         Capture a screenshot from the browser under test
         
         Args:
             name: the unique name used both in naming the file, and identifying the visual test image 
@@ -198,15 +217,14 @@
 
         if type(name) != str:
             raise Exception(f'Name argument must be a string')
 
         if len(name) > 100:
             raise Exception(f'Name argument cannot be greater than 100 characters')
 
-        filePath = os.path.join(self._settings['saveTo'],f'{name}.png')
         imageType = None
 
         self.browser._clearIgnoreElements() #clear the window from previous ignoredElements
         if 'ignoreElements' in options:
             if not isinstance(options['ignoreElements'], list):
                 raise Exception(f'ignoreElements must be of type "list"')
             if not all(isinstance(item, str) for item in options['ignoreElements']):
@@ -224,50 +242,105 @@
             else:
                 self.browser._injectIgnoreElements(options['ignoreElements'])
 
         if 'freezePage' in options:
             if not isinstance(options['freezePage'], bool):
                 raise Exception(f'freezePage must be of type "bool"')
 
+        comparisonMode = None
+        sensitivity = None
+        if 'comparisonMode' in options:
+            if not isinstance(options['comparisonMode'], str):
+                raise Exception(f'comparisonMode must be of type "str"')
+            if options['comparisonMode'] == 'detailed':
+                comparisonMode = 'detailed'
+            elif options['comparisonMode'] == 'layout':
+                comparisonMode = 'layout'
+                if 'sensitivity' in options:
+                    if not isinstance(options['sensitivity'], str):
+                        raise Exception(f'sensitivity must be of type "str"')
+                    if options['sensitivity'] in ['low', 'medium', 'high']:
+                        if options['sensitivity'].__eq__('low'):
+                            sensitivity = 0
+                        elif options['sensitivity'].__eq__('medium'):
+                            sensitivity = 1
+                        elif options['sensitivity'].__eq__('high'):
+                            sensitivity = 2
+                    else:
+                        raise Exception(f'sensitivity value should be "low", "medium" or "high".')
+                else:
+                    raise Exception(f'sensitivity value should be set to "low", "medium" or "high" when passing comparisonMode="layout".')
+            else:
+                raise Exception(f'comparisonMode value should be "detailed" or "layout" mode.')
+
         if 'element' in options:
-            screenshotResult = self.browser.takeElementScreenshot(filePath, options)
+            screenshotResult = self.browser.takeElementScreenshot(options)
             imageType = 'element'
         elif 'viewport' in options and options['viewport'] == True:
-            screenshotResult = self.browser.takeViewportScreenshot(filePath, options)
+            screenshotResult = self.browser.takeViewportScreenshot(options)
             imageType = 'viewport'
         else:
             if 'lazyload' in options:
                 if type(options['lazyload']) != int or options['lazyload'] < 0 or options['lazyload'] > 10000:
                     raise Exception('"lazyload" value must be an integer between 0 and 10000 ms!')
 
-            screenshotResult = self.browser.takeFullpageScreenshot(filePath, options)
+            screenshotResult = self.browser.takeFullpageScreenshot(name, options)
             imageType = 'fullpage'
         
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
             'dom': json.dumps(self.browser.dom),
-            'ignoredElements': json.dumps(self.browser.dom['ignoredElementsData'])
+            'ignoredElements': json.dumps(self.browser.dom['ignoredElementsData']),
+            'comparisonMode': comparisonMode,
+            'sensitivity': sensitivity,
+            'headless': self.browser._headless
         }
         imageData.update(self.browser._deviceInfo) # required information about device/os/browser
 
         # these two are informational and just used to store - not required
         imageData.update({'driverCapabilities': json.dumps(self.browser.capabilities)})
         imageData.update({'userAgentInfo': json.dumps(self.browser._userAgentInfo)})
 
         # post the image, creating testrun if new
-        imageApiResult = self._api.saveImage(self._settings['testRunName'], imageData, filePath)
+        imageApiResult = self._api.saveImage(self._settings['testRunName'], imageData, screenshotResult['imageBinary'])
+
+        # save final image to debug file
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
+        # do not return the binary to the results
+        del screenshotResult['imageBinary']
 
         return {
             'screenshotResult': screenshotResult,
             'imageApiResult': imageApiResult,
         }
 
-
+    def printReport(self):
+        return self._api.printReport()
```

## Comparing `visualtest_python-1.3.2.dist-info/LICENSE` & `visualtest_python-1.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `visualtest_python-1.3.2.dist-info/METADATA` & `visualtest_python-1.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualtest-python
-Version: 1.3.2
+Version: 1.4.0
 Summary: Python SDK for SmartBear VisualTest via Selenium WebDriver
 Home-page: https://github.com/SmartBear/visualtest-python
 Author: Luke Kende
 Author-email: luke.kende@smartbear.com
 Keywords: visual testing,UI testing,GUI testing,UX testing,screenshots,full page screenshots,image comparisons,regression testing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```


# Comparing `tmp/wlkatapython-0.0.1.tar.gz` & `tmp/wlkatapython-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlkatapython-0.0.1.tar", last modified: Thu May 18 07:38:32 2023, max compression
+gzip compressed data, was "wlkatapython-0.0.2.tar", last modified: Thu Jun  1 12:18:01 2023, max compression
```

## Comparing `wlkatapython-0.0.1.tar` & `wlkatapython-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 07:38:32.021383 wlkatapython-0.0.1/
--rw-rw-rw-   0        0        0      213 2023-05-18 07:38:32.021383 wlkatapython-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-18 07:38:32.021383 wlkatapython-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      290 2023-05-18 07:32:31.000000 wlkatapython-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 07:38:32.019384 wlkatapython-0.0.1/wlkatapython.egg-info/
--rw-rw-rw-   0        0        0      213 2023-05-18 07:38:31.000000 wlkatapython-0.0.1/wlkatapython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-05-18 07:38:32.000000 wlkatapython-0.0.1/wlkatapython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 07:38:31.000000 wlkatapython-0.0.1/wlkatapython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-18 07:38:31.000000 wlkatapython-0.0.1/wlkatapython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8771 2023-05-18 07:22:33.000000 wlkatapython-0.0.1/wlkatapython.py
+drwxrwxrwx   0        0        0        0 2023-06-01 12:18:01.268404 wlkatapython-0.0.2/
+-rw-rw-rw-   0        0        0      213 2023-06-01 12:18:01.268404 wlkatapython-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-01 12:18:01.268404 wlkatapython-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      290 2023-06-01 11:49:15.000000 wlkatapython-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 12:18:01.267403 wlkatapython-0.0.2/wlkatapython.egg-info/
+-rw-rw-rw-   0        0        0      213 2023-06-01 12:18:01.000000 wlkatapython-0.0.2/wlkatapython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-06-01 12:18:01.000000 wlkatapython-0.0.2/wlkatapython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 12:18:01.000000 wlkatapython-0.0.2/wlkatapython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-01 12:18:01.000000 wlkatapython-0.0.2/wlkatapython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10136 2023-06-01 11:48:59.000000 wlkatapython-0.0.2/wlkatapython.py
```

### Comparing `wlkatapython-0.0.1/wlkatapython.py` & `wlkatapython-0.0.2/wlkatapython.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 wlkata python库包含USB口控制和RS485控制
-版本号0.0.1
+版本号0.0.2
 '''
 import serial
 import time
 import re
 
 class Wlkata_UART:
     def __init__(self):
@@ -101,14 +101,56 @@
         self.num = "M3 S" + str(num)
         self.sendMsg(self.num)
 
     # 初始位置
     def zero(self):
         self.sendMsg("M21 G90 G00 X0 Y0 Z0 A0 B0 C00")
 
+    #笛卡尔坐标控制
+    def writecoordinate(self,motion,position,x,y,z,a,b,c):
+        self.motion=motion
+        self.position=position
+        self.coordinate="X"+str(x)+"Y"+str(y)+"Z"+str(z)+"A"+str(a)+"B"+str(b)+"C"+str(c)
+        if self.motion==0:
+            self.motion="G00"
+        elif self.motion==1:
+            self.motion="G01"
+        elif self.motion==2:
+            self.motion="G05"
+        else:
+            self.motion = "G00"
+
+        if self.position==0:
+            self.position="G90"
+        elif self.position==1:
+            self.position="G91"
+        else:
+            self.position = "G90"
+        self.coordinate="M20"+str(self.position)+str(self.motion)+self.coordinate
+        self.sendMsg(self.coordinate)
+
+    #速度设置
+    def speed(self,num):
+        self.num="F"+str(num)
+        self.sendMsg(self.num)
+
+    #角度设置
+    def writeangle(self,position,x,y,z,a,b,c):
+        self.position=position
+        self.coordinate="X"+str(x)+"Y"+str(y)+"Z"+str(z)+"A"+str(a)+"B"+str(b)+"C"+str(c)
+        if self.position==0:
+            self.position="G90"
+        elif self.position==1:
+            self.position="G91"
+        else:
+            self.position = "G90"
+        self.coordinate="M21"+str(self.position)+"G00"+self.coordinate
+        self.sendMsg(self.coordinate)
+
+
     #重启设备
     def restart(self):
         self.sendMsg("o100")
 
     #查询版本信息
     def version(self):
         self.lina = ""  # 初始化为字符串
```


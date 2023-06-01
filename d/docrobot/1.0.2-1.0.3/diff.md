# Comparing `tmp/docrobot-1.0.2.tar.gz` & `tmp/docrobot-1.0.3.tar.gz`

## Comparing `docrobot-1.0.2.tar` & `docrobot-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,13 @@
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 docrobot-1.0.2/convert.ps1
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 docrobot-1.0.2/requirements.txt
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 docrobot-1.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.0.2/src/docrobot/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 docrobot-1.0.2/src/docrobot/config.ini
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 docrobot-1.0.2/src/docrobot/form.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 docrobot-1.0.2/src/docrobot/form.ui
--rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 docrobot-1.0.2/src/docrobot/guimain.pyw
--rw-r--r--   0        0        0    11201 2020-02-02 00:00:00.000000 docrobot-1.0.2/src/docrobot/util.py
--rw-r--r--   0        0        0    27599 2020-02-02 00:00:00.000000 docrobot-1.0.2/temple/logo.png
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 docrobot-1.0.2/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 docrobot-1.0.2/LICENSE
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 docrobot-1.0.2/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 docrobot-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 docrobot-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 docrobot-1.0.3/convert.ps1
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 docrobot-1.0.3/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 docrobot-1.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.0.3/src/docrobot/__init__.py
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 docrobot-1.0.3/src/docrobot/form.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 docrobot-1.0.3/src/docrobot/form.ui
+-rw-r--r--   0        0        0    10924 2020-02-02 00:00:00.000000 docrobot-1.0.3/src/docrobot/guimain.pyw
+-rw-r--r--   0        0        0    10945 2020-02-02 00:00:00.000000 docrobot-1.0.3/src/docrobot/util.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 docrobot-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 docrobot-1.0.3/LICENSE
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 docrobot-1.0.3/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 docrobot-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 docrobot-1.0.3/PKG-INFO
```

### Comparing `docrobot-1.0.2/src/docrobot/form.py` & `docrobot-1.0.3/src/docrobot/form.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-# -*- coding: utf-8 -*-
-
-################################################################################
-## Form generated from reading UI file 'form.ui'
-##
-## Created by: Qt User Interface Compiler version 6.4.1
-##
-## WARNING! All changes made in this file will be lost when recompiling UI file!
-################################################################################
-
-from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
-    QMetaObject, QObject, QPoint, QRect,
-    QSize, QTime, QUrl, Qt)
-from PySide6.QtGui import (QAction, QBrush, QColor, QConicalGradient,
-    QCursor, QFont, QFontDatabase, QGradient,
-    QIcon, QImage, QKeySequence, QLinearGradient,
-    QPainter, QPalette, QPixmap, QRadialGradient,
-    QTransform)
-from PySide6.QtWidgets import (QApplication, QLabel, QLineEdit, QMainWindow,
-    QMenu, QMenuBar, QSizePolicy, QStatusBar,
-    QTextEdit, QWidget)
-
-class Ui_MainWindow(object):
-    def setupUi(self, MainWindow):
-        if not MainWindow.objectName():
-            MainWindow.setObjectName(u"MainWindow")
-        MainWindow.resize(800, 600)
-        self.actionSelect_Dir = QAction(MainWindow)
-        self.actionSelect_Dir.setObjectName(u"actionSelect_Dir")
-        self.actioncheck = QAction(MainWindow)
-        self.actioncheck.setObjectName(u"actioncheck")
-        self.actionreplace = QAction(MainWindow)
-        self.actionreplace.setObjectName(u"actionreplace")
-        self.actioncheckall = QAction(MainWindow)
-        self.actioncheckall.setObjectName(u"actioncheckall")
-        self.centralwidget = QWidget(MainWindow)
-        self.centralwidget.setObjectName(u"centralwidget")
-        self.textEdit = QTextEdit(self.centralwidget)
-        self.textEdit.setObjectName(u"textEdit")
-        self.textEdit.setGeometry(QRect(10, 40, 781, 521))
-        self.label = QLabel(self.centralwidget)
-        self.label.setObjectName(u"label")
-        self.label.setGeometry(QRect(10, 10, 91, 16))
-        self.lineEdit = QLineEdit(self.centralwidget)
-        self.lineEdit.setObjectName(u"lineEdit")
-        self.lineEdit.setGeometry(QRect(100, 10, 691, 20))
-        MainWindow.setCentralWidget(self.centralwidget)
-        self.menubar = QMenuBar(MainWindow)
-        self.menubar.setObjectName(u"menubar")
-        self.menubar.setGeometry(QRect(0, 0, 800, 26))
-        self.menu = QMenu(self.menubar)
-        self.menu.setObjectName(u"menu")
-        self.menu_2 = QMenu(self.menubar)
-        self.menu_2.setObjectName(u"menu_2")
-        self.menu_3 = QMenu(self.menubar)
-        self.menu_3.setObjectName(u"menu_3")
-        self.menu_4 = QMenu(self.menubar)
-        self.menu_4.setObjectName(u"menu_4")
-        MainWindow.setMenuBar(self.menubar)
-        self.statusbar = QStatusBar(MainWindow)
-        self.statusbar.setObjectName(u"statusbar")
-        MainWindow.setStatusBar(self.statusbar)
-
-        self.menubar.addAction(self.menu.menuAction())
-        self.menubar.addAction(self.menu_4.menuAction())
-        self.menubar.addAction(self.menu_2.menuAction())
-        self.menubar.addAction(self.menu_3.menuAction())
-        self.menu.addAction(self.actionSelect_Dir)
-        self.menu_2.addAction(self.actionreplace)
-        self.menu_3.addAction(self.actioncheck)
-        self.menu_4.addSeparator()
-        self.menu_4.addAction(self.actioncheckall)
-
-        self.retranslateUi(MainWindow)
-
-        QMetaObject.connectSlotsByName(MainWindow)
-    # setupUi
-
-    def retranslateUi(self, MainWindow):
-        MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", u"MainWindow", None))
-        self.actionSelect_Dir.setText(QCoreApplication.translate("MainWindow", u"Select Dir", None))
-        self.actioncheck.setText(QCoreApplication.translate("MainWindow", u"\u68c0\u67e5", None))
-        self.actionreplace.setText(QCoreApplication.translate("MainWindow", u"\u6279\u91cf\u66ff\u6362", None))
-        self.actioncheckall.setText(QCoreApplication.translate("MainWindow", u"\u68c0\u67e5\u6240\u6709\u9879", None))
-        self.label.setText(QCoreApplication.translate("MainWindow", u"\u5f53\u524d\u5904\u7406\u76ee\u5f55\uff1a", None))
-        self.menu.setTitle(QCoreApplication.translate("MainWindow", u"\u8bbe\u7f6e", None))
-        self.menu_2.setTitle(QCoreApplication.translate("MainWindow", u"\u9879\u76ee", None))
-        self.menu_3.setTitle(QCoreApplication.translate("MainWindow", u"\u4e13\u5229", None))
-        self.menu_4.setTitle(QCoreApplication.translate("MainWindow", u"\u68c0\u67e5", None))
-    # retranslateUi
-
+# -*- coding: utf-8 -*-
+
+################################################################################
+## Form generated from reading UI file 'form.ui'
+##
+## Created by: Qt User Interface Compiler version 6.4.1
+##
+## WARNING! All changes made in this file will be lost when recompiling UI file!
+################################################################################
+
+from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
+    QMetaObject, QObject, QPoint, QRect,
+    QSize, QTime, QUrl, Qt)
+from PySide6.QtGui import (QAction, QBrush, QColor, QConicalGradient,
+    QCursor, QFont, QFontDatabase, QGradient,
+    QIcon, QImage, QKeySequence, QLinearGradient,
+    QPainter, QPalette, QPixmap, QRadialGradient,
+    QTransform)
+from PySide6.QtWidgets import (QApplication, QLabel, QLineEdit, QMainWindow,
+    QMenu, QMenuBar, QSizePolicy, QStatusBar,
+    QTextEdit, QWidget)
+
+class Ui_MainWindow(object):
+    def setupUi(self, MainWindow):
+        if not MainWindow.objectName():
+            MainWindow.setObjectName(u"MainWindow")
+        MainWindow.resize(800, 600)
+        self.actionSelect_Dir = QAction(MainWindow)
+        self.actionSelect_Dir.setObjectName(u"actionSelect_Dir")
+        self.actioncheck = QAction(MainWindow)
+        self.actioncheck.setObjectName(u"actioncheck")
+        self.actionreplace = QAction(MainWindow)
+        self.actionreplace.setObjectName(u"actionreplace")
+        self.actioncheckall = QAction(MainWindow)
+        self.actioncheckall.setObjectName(u"actioncheckall")
+        self.centralwidget = QWidget(MainWindow)
+        self.centralwidget.setObjectName(u"centralwidget")
+        self.textEdit = QTextEdit(self.centralwidget)
+        self.textEdit.setObjectName(u"textEdit")
+        self.textEdit.setGeometry(QRect(10, 40, 781, 521))
+        self.label = QLabel(self.centralwidget)
+        self.label.setObjectName(u"label")
+        self.label.setGeometry(QRect(10, 10, 91, 16))
+        self.lineEdit = QLineEdit(self.centralwidget)
+        self.lineEdit.setObjectName(u"lineEdit")
+        self.lineEdit.setGeometry(QRect(100, 10, 691, 20))
+        MainWindow.setCentralWidget(self.centralwidget)
+        self.menubar = QMenuBar(MainWindow)
+        self.menubar.setObjectName(u"menubar")
+        self.menubar.setGeometry(QRect(0, 0, 800, 26))
+        self.menu = QMenu(self.menubar)
+        self.menu.setObjectName(u"menu")
+        self.menu_2 = QMenu(self.menubar)
+        self.menu_2.setObjectName(u"menu_2")
+        self.menu_3 = QMenu(self.menubar)
+        self.menu_3.setObjectName(u"menu_3")
+        self.menu_4 = QMenu(self.menubar)
+        self.menu_4.setObjectName(u"menu_4")
+        MainWindow.setMenuBar(self.menubar)
+        self.statusbar = QStatusBar(MainWindow)
+        self.statusbar.setObjectName(u"statusbar")
+        MainWindow.setStatusBar(self.statusbar)
+
+        self.menubar.addAction(self.menu.menuAction())
+        self.menubar.addAction(self.menu_4.menuAction())
+        self.menubar.addAction(self.menu_2.menuAction())
+        self.menubar.addAction(self.menu_3.menuAction())
+        self.menu.addAction(self.actionSelect_Dir)
+        self.menu_2.addAction(self.actionreplace)
+        self.menu_3.addAction(self.actioncheck)
+        self.menu_4.addSeparator()
+        self.menu_4.addAction(self.actioncheckall)
+
+        self.retranslateUi(MainWindow)
+
+        QMetaObject.connectSlotsByName(MainWindow)
+    # setupUi
+
+    def retranslateUi(self, MainWindow):
+        MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", u"MainWindow", None))
+        self.actionSelect_Dir.setText(QCoreApplication.translate("MainWindow", u"Select Dir", None))
+        self.actioncheck.setText(QCoreApplication.translate("MainWindow", u"\u68c0\u67e5", None))
+        self.actionreplace.setText(QCoreApplication.translate("MainWindow", u"\u6279\u91cf\u66ff\u6362", None))
+        self.actioncheckall.setText(QCoreApplication.translate("MainWindow", u"\u68c0\u67e5\u6240\u6709\u9879", None))
+        self.label.setText(QCoreApplication.translate("MainWindow", u"\u5f53\u524d\u5904\u7406\u76ee\u5f55\uff1a", None))
+        self.menu.setTitle(QCoreApplication.translate("MainWindow", u"\u8bbe\u7f6e", None))
+        self.menu_2.setTitle(QCoreApplication.translate("MainWindow", u"\u9879\u76ee", None))
+        self.menu_3.setTitle(QCoreApplication.translate("MainWindow", u"\u4e13\u5229", None))
+        self.menu_4.setTitle(QCoreApplication.translate("MainWindow", u"\u68c0\u67e5", None))
+    # retranslateUi
+
```

### Comparing `docrobot-1.0.2/src/docrobot/form.ui` & `docrobot-1.0.3/src/docrobot/form.ui`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, Unicode text, UTF-8 text, with CRLF line terminators*

 * *Files 27% similar despite different names*

```diff
@@ -1,177 +1,170 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0d0a 3c75 6920 7665 7273  F-8"?>..<ui vers
-00000030: 696f 6e3d 2234 2e30 223e 0d0a 203c 636c  ion="4.0">.. <cl
-00000040: 6173 733e 4d61 696e 5769 6e64 6f77 3c2f  ass>MainWindow</
-00000050: 636c 6173 733e 0d0a 203c 7769 6467 6574  class>.. <widget
-00000060: 2063 6c61 7373 3d22 514d 6169 6e57 696e   class="QMainWin
-00000070: 646f 7722 206e 616d 653d 224d 6169 6e57  dow" name="MainW
-00000080: 696e 646f 7722 3e0d 0a20 203c 7072 6f70  indow">..  <prop
-00000090: 6572 7479 206e 616d 653d 2267 656f 6d65  erty name="geome
-000000a0: 7472 7922 3e0d 0a20 2020 3c72 6563 743e  try">..   <rect>
-000000b0: 0d0a 2020 2020 3c78 3e30 3c2f 783e 0d0a  ..    <x>0</x>..
-000000c0: 2020 2020 3c79 3e30 3c2f 793e 0d0a 2020      <y>0</y>..  
-000000d0: 2020 3c77 6964 7468 3e38 3030 3c2f 7769    <width>800</wi
-000000e0: 6474 683e 0d0a 2020 2020 3c68 6569 6768  dth>..    <heigh
-000000f0: 743e 3630 303c 2f68 6569 6768 743e 0d0a  t>600</height>..
-00000100: 2020 203c 2f72 6563 743e 0d0a 2020 3c2f     </rect>..  </
-00000110: 7072 6f70 6572 7479 3e0d 0a20 203c 7072  property>..  <pr
-00000120: 6f70 6572 7479 206e 616d 653d 2277 696e  operty name="win
-00000130: 646f 7754 6974 6c65 223e 0d0a 2020 203c  dowTitle">..   <
-00000140: 7374 7269 6e67 3e4d 6169 6e57 696e 646f  string>MainWindo
-00000150: 773c 2f73 7472 696e 673e 0d0a 2020 3c2f  w</string>..  </
-00000160: 7072 6f70 6572 7479 3e0d 0a20 203c 7769  property>..  <wi
-00000170: 6467 6574 2063 6c61 7373 3d22 5157 6964  dget class="QWid
-00000180: 6765 7422 206e 616d 653d 2263 656e 7472  get" name="centr
-00000190: 616c 7769 6467 6574 223e 0d0a 2020 203c  alwidget">..   <
-000001a0: 7769 6467 6574 2063 6c61 7373 3d22 5154  widget class="QT
-000001b0: 6578 7445 6469 7422 206e 616d 653d 2274  extEdit" name="t
-000001c0: 6578 7445 6469 7422 3e0d 0a20 2020 203c  extEdit">..    <
-000001d0: 7072 6f70 6572 7479 206e 616d 653d 2267  property name="g
-000001e0: 656f 6d65 7472 7922 3e0d 0a20 2020 2020  eometry">..     
-000001f0: 3c72 6563 743e 0d0a 2020 2020 2020 3c78  <rect>..      <x
-00000200: 3e31 303c 2f78 3e0d 0a20 2020 2020 203c  >10</x>..      <
-00000210: 793e 3430 3c2f 793e 0d0a 2020 2020 2020  y>40</y>..      
-00000220: 3c77 6964 7468 3e37 3831 3c2f 7769 6474  <width>781</widt
-00000230: 683e 0d0a 2020 2020 2020 3c68 6569 6768  h>..      <heigh
-00000240: 743e 3532 313c 2f68 6569 6768 743e 0d0a  t>521</height>..
-00000250: 2020 2020 203c 2f72 6563 743e 0d0a 2020       </rect>..  
-00000260: 2020 3c2f 7072 6f70 6572 7479 3e0d 0a20    </property>.. 
-00000270: 2020 3c2f 7769 6467 6574 3e0d 0a20 2020    </widget>..   
-00000280: 3c77 6964 6765 7420 636c 6173 733d 2251  <widget class="Q
-00000290: 4c61 6265 6c22 206e 616d 653d 226c 6162  Label" name="lab
-000002a0: 656c 223e 0d0a 2020 2020 3c70 726f 7065  el">..    <prope
-000002b0: 7274 7920 6e61 6d65 3d22 6765 6f6d 6574  rty name="geomet
-000002c0: 7279 223e 0d0a 2020 2020 203c 7265 6374  ry">..     <rect
-000002d0: 3e0d 0a20 2020 2020 203c 783e 3130 3c2f  >..      <x>10</
-000002e0: 783e 0d0a 2020 2020 2020 3c79 3e31 303c  x>..      <y>10<
-000002f0: 2f79 3e0d 0a20 2020 2020 203c 7769 6474  /y>..      <widt
-00000300: 683e 3931 3c2f 7769 6474 683e 0d0a 2020  h>91</width>..  
-00000310: 2020 2020 3c68 6569 6768 743e 3136 3c2f      <height>16</
-00000320: 6865 6967 6874 3e0d 0a20 2020 2020 3c2f  height>..     </
-00000330: 7265 6374 3e0d 0a20 2020 203c 2f70 726f  rect>..    </pro
-00000340: 7065 7274 793e 0d0a 2020 2020 3c70 726f  perty>..    <pro
-00000350: 7065 7274 7920 6e61 6d65 3d22 7465 7874  perty name="text
-00000360: 223e 0d0a 2020 2020 203c 7374 7269 6e67  ">..     <string
-00000370: 3ee5 bd93 e589 8de5 a484 e790 86e7 9bae  >...............
-00000380: e5bd 95ef bc9a 3c2f 7374 7269 6e67 3e0d  ......</string>.
-00000390: 0a20 2020 203c 2f70 726f 7065 7274 793e  .    </property>
-000003a0: 0d0a 2020 203c 2f77 6964 6765 743e 0d0a  ..   </widget>..
-000003b0: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
-000003c0: 3d22 514c 696e 6545 6469 7422 206e 616d  ="QLineEdit" nam
-000003d0: 653d 226c 696e 6545 6469 7422 3e0d 0a20  e="lineEdit">.. 
-000003e0: 2020 203c 7072 6f70 6572 7479 206e 616d     <property nam
-000003f0: 653d 2267 656f 6d65 7472 7922 3e0d 0a20  e="geometry">.. 
-00000400: 2020 2020 3c72 6563 743e 0d0a 2020 2020      <rect>..    
-00000410: 2020 3c78 3e31 3030 3c2f 783e 0d0a 2020    <x>100</x>..  
-00000420: 2020 2020 3c79 3e31 303c 2f79 3e0d 0a20      <y>10</y>.. 
-00000430: 2020 2020 203c 7769 6474 683e 3639 313c       <width>691<
-00000440: 2f77 6964 7468 3e0d 0a20 2020 2020 203c  /width>..      <
-00000450: 6865 6967 6874 3e32 303c 2f68 6569 6768  height>20</heigh
-00000460: 743e 0d0a 2020 2020 203c 2f72 6563 743e  t>..     </rect>
-00000470: 0d0a 2020 2020 3c2f 7072 6f70 6572 7479  ..    </property
-00000480: 3e0d 0a20 2020 3c2f 7769 6467 6574 3e0d  >..   </widget>.
-00000490: 0a20 203c 2f77 6964 6765 743e 0d0a 2020  .  </widget>..  
-000004a0: 3c77 6964 6765 7420 636c 6173 733d 2251  <widget class="Q
-000004b0: 4d65 6e75 4261 7222 206e 616d 653d 226d  MenuBar" name="m
-000004c0: 656e 7562 6172 223e 0d0a 2020 203c 7072  enubar">..   <pr
-000004d0: 6f70 6572 7479 206e 616d 653d 2267 656f  operty name="geo
-000004e0: 6d65 7472 7922 3e0d 0a20 2020 203c 7265  metry">..    <re
-000004f0: 6374 3e0d 0a20 2020 2020 3c78 3e30 3c2f  ct>..     <x>0</
-00000500: 783e 0d0a 2020 2020 203c 793e 303c 2f79  x>..     <y>0</y
-00000510: 3e0d 0a20 2020 2020 3c77 6964 7468 3e38  >..     <width>8
-00000520: 3030 3c2f 7769 6474 683e 0d0a 2020 2020  00</width>..    
-00000530: 203c 6865 6967 6874 3e32 363c 2f68 6569   <height>26</hei
-00000540: 6768 743e 0d0a 2020 2020 3c2f 7265 6374  ght>..    </rect
-00000550: 3e0d 0a20 2020 3c2f 7072 6f70 6572 7479  >..   </property
-00000560: 3e0d 0a20 2020 3c77 6964 6765 7420 636c  >..   <widget cl
-00000570: 6173 733d 2251 4d65 6e75 2220 6e61 6d65  ass="QMenu" name
-00000580: 3d22 6d65 6e75 223e 0d0a 2020 2020 3c70  ="menu">..    <p
-00000590: 726f 7065 7274 7920 6e61 6d65 3d22 7469  roperty name="ti
-000005a0: 746c 6522 3e0d 0a20 2020 2020 3c73 7472  tle">..     <str
-000005b0: 696e 673e e8ae bee7 bdae 3c2f 7374 7269  ing>......</stri
-000005c0: 6e67 3e0d 0a20 2020 203c 2f70 726f 7065  ng>..    </prope
-000005d0: 7274 793e 0d0a 2020 2020 3c61 6464 6163  rty>..    <addac
-000005e0: 7469 6f6e 206e 616d 653d 2261 6374 696f  tion name="actio
-000005f0: 6e53 656c 6563 745f 4469 7222 2f3e 0d0a  nSelect_Dir"/>..
-00000600: 2020 203c 2f77 6964 6765 743e 0d0a 2020     </widget>..  
-00000610: 203c 7769 6467 6574 2063 6c61 7373 3d22   <widget class="
-00000620: 514d 656e 7522 206e 616d 653d 226d 656e  QMenu" name="men
-00000630: 755f 3222 3e0d 0a20 2020 203c 7072 6f70  u_2">..    <prop
-00000640: 6572 7479 206e 616d 653d 2274 6974 6c65  erty name="title
-00000650: 223e 0d0a 2020 2020 203c 7374 7269 6e67  ">..     <string
-00000660: 3ee9 a1b9 e79b ae3c 2f73 7472 696e 673e  >......</string>
-00000670: 0d0a 2020 2020 3c2f 7072 6f70 6572 7479  ..    </property
-00000680: 3e0d 0a20 2020 203c 6164 6461 6374 696f  >..    <addactio
-00000690: 6e20 6e61 6d65 3d22 6163 7469 6f6e 7265  n name="actionre
-000006a0: 706c 6163 6522 2f3e 0d0a 2020 203c 2f77  place"/>..   </w
-000006b0: 6964 6765 743e 0d0a 2020 203c 7769 6467  idget>..   <widg
-000006c0: 6574 2063 6c61 7373 3d22 514d 656e 7522  et class="QMenu"
-000006d0: 206e 616d 653d 226d 656e 755f 3322 3e0d   name="menu_3">.
-000006e0: 0a20 2020 203c 7072 6f70 6572 7479 206e  .    <property n
-000006f0: 616d 653d 2274 6974 6c65 223e 0d0a 2020  ame="title">..  
-00000700: 2020 203c 7374 7269 6e67 3ee4 b893 e588     <string>.....
-00000710: a93c 2f73 7472 696e 673e 0d0a 2020 2020  .</string>..    
-00000720: 3c2f 7072 6f70 6572 7479 3e0d 0a20 2020  </property>..   
-00000730: 203c 6164 6461 6374 696f 6e20 6e61 6d65   <addaction name
-00000740: 3d22 6163 7469 6f6e 6368 6563 6b22 2f3e  ="actioncheck"/>
-00000750: 0d0a 2020 203c 2f77 6964 6765 743e 0d0a  ..   </widget>..
-00000760: 2020 203c 7769 6467 6574 2063 6c61 7373     <widget class
-00000770: 3d22 514d 656e 7522 206e 616d 653d 226d  ="QMenu" name="m
-00000780: 656e 755f 3422 3e0d 0a20 2020 203c 7072  enu_4">..    <pr
-00000790: 6f70 6572 7479 206e 616d 653d 2274 6974  operty name="tit
-000007a0: 6c65 223e 0d0a 2020 2020 203c 7374 7269  le">..     <stri
-000007b0: 6e67 3ee6 a380 e69f a53c 2f73 7472 696e  ng>......</strin
-000007c0: 673e 0d0a 2020 2020 3c2f 7072 6f70 6572  g>..    </proper
-000007d0: 7479 3e0d 0a20 2020 203c 6164 6461 6374  ty>..    <addact
-000007e0: 696f 6e20 6e61 6d65 3d22 7365 7061 7261  ion name="separa
-000007f0: 746f 7222 2f3e 0d0a 2020 2020 3c61 6464  tor"/>..    <add
-00000800: 6163 7469 6f6e 206e 616d 653d 2261 6374  action name="act
-00000810: 696f 6e63 6865 636b 616c 6c22 2f3e 0d0a  ioncheckall"/>..
-00000820: 2020 203c 2f77 6964 6765 743e 0d0a 2020     </widget>..  
-00000830: 203c 6164 6461 6374 696f 6e20 6e61 6d65   <addaction name
-00000840: 3d22 6d65 6e75 222f 3e0d 0a20 2020 3c61  ="menu"/>..   <a
-00000850: 6464 6163 7469 6f6e 206e 616d 653d 226d  ddaction name="m
-00000860: 656e 755f 3422 2f3e 0d0a 2020 203c 6164  enu_4"/>..   <ad
-00000870: 6461 6374 696f 6e20 6e61 6d65 3d22 6d65  daction name="me
-00000880: 6e75 5f32 222f 3e0d 0a20 2020 3c61 6464  nu_2"/>..   <add
-00000890: 6163 7469 6f6e 206e 616d 653d 226d 656e  action name="men
-000008a0: 755f 3322 2f3e 0d0a 2020 3c2f 7769 6467  u_3"/>..  </widg
-000008b0: 6574 3e0d 0a20 203c 7769 6467 6574 2063  et>..  <widget c
-000008c0: 6c61 7373 3d22 5153 7461 7475 7342 6172  lass="QStatusBar
-000008d0: 2220 6e61 6d65 3d22 7374 6174 7573 6261  " name="statusba
-000008e0: 7222 2f3e 0d0a 2020 3c61 6374 696f 6e20  r"/>..  <action 
-000008f0: 6e61 6d65 3d22 6163 7469 6f6e 5365 6c65  name="actionSele
-00000900: 6374 5f44 6972 223e 0d0a 2020 203c 7072  ct_Dir">..   <pr
-00000910: 6f70 6572 7479 206e 616d 653d 2274 6578  operty name="tex
-00000920: 7422 3e0d 0a20 2020 203c 7374 7269 6e67  t">..    <string
-00000930: 3e53 656c 6563 7420 4469 723c 2f73 7472  >Select Dir</str
-00000940: 696e 673e 0d0a 2020 203c 2f70 726f 7065  ing>..   </prope
-00000950: 7274 793e 0d0a 2020 3c2f 6163 7469 6f6e  rty>..  </action
-00000960: 3e0d 0a20 203c 6163 7469 6f6e 206e 616d  >..  <action nam
-00000970: 653d 2261 6374 696f 6e63 6865 636b 223e  e="actioncheck">
-00000980: 0d0a 2020 203c 7072 6f70 6572 7479 206e  ..   <property n
-00000990: 616d 653d 2274 6578 7422 3e0d 0a20 2020  ame="text">..   
-000009a0: 203c 7374 7269 6e67 3ee6 a380 e69f a53c   <string>......<
-000009b0: 2f73 7472 696e 673e 0d0a 2020 203c 2f70  /string>..   </p
-000009c0: 726f 7065 7274 793e 0d0a 2020 3c2f 6163  roperty>..  </ac
-000009d0: 7469 6f6e 3e0d 0a20 203c 6163 7469 6f6e  tion>..  <action
-000009e0: 206e 616d 653d 2261 6374 696f 6e72 6570   name="actionrep
-000009f0: 6c61 6365 223e 0d0a 2020 203c 7072 6f70  lace">..   <prop
-00000a00: 6572 7479 206e 616d 653d 2274 6578 7422  erty name="text"
-00000a10: 3e0d 0a20 2020 203c 7374 7269 6e67 3ee6  >..    <string>.
-00000a20: 89b9 e987 8fe6 9bbf e68d a23c 2f73 7472  ...........</str
-00000a30: 696e 673e 0d0a 2020 203c 2f70 726f 7065  ing>..   </prope
-00000a40: 7274 793e 0d0a 2020 3c2f 6163 7469 6f6e  rty>..  </action
-00000a50: 3e0d 0a20 203c 6163 7469 6f6e 206e 616d  >..  <action nam
-00000a60: 653d 2261 6374 696f 6e63 6865 636b 616c  e="actioncheckal
-00000a70: 6c22 3e0d 0a20 2020 3c70 726f 7065 7274  l">..   <propert
-00000a80: 7920 6e61 6d65 3d22 7465 7874 223e 0d0a  y name="text">..
-00000a90: 2020 2020 3c73 7472 696e 673e e6a3 80e6      <string>....
-00000aa0: 9fa5 e689 80e6 9c89 e9a1 b93c 2f73 7472  ...........</str
-00000ab0: 696e 673e 0d0a 2020 203c 2f70 726f 7065  ing>..   </prope
-00000ac0: 7274 793e 0d0a 2020 3c2f 6163 7469 6f6e  rty>..  </action
-00000ad0: 3e0d 0a20 3c2f 7769 6467 6574 3e0d 0a20  >.. </widget>.. 
-00000ae0: 3c72 6573 6f75 7263 6573 2f3e 0d0a 203c  <resources/>.. <
-00000af0: 636f 6e6e 6563 7469 6f6e 732f 3e0d 0a3c  connections/>..<
-00000b00: 2f75 693e 0d0a                           /ui>..
+00000020: 462d 3822 3f3e 0a3c 7569 2076 6572 7369  F-8"?>.<ui versi
+00000030: 6f6e 3d22 342e 3022 3e0a 203c 636c 6173  on="4.0">. <clas
+00000040: 733e 4d61 696e 5769 6e64 6f77 3c2f 636c  s>MainWindow</cl
+00000050: 6173 733e 0a20 3c77 6964 6765 7420 636c  ass>. <widget cl
+00000060: 6173 733d 2251 4d61 696e 5769 6e64 6f77  ass="QMainWindow
+00000070: 2220 6e61 6d65 3d22 4d61 696e 5769 6e64  " name="MainWind
+00000080: 6f77 223e 0a20 203c 7072 6f70 6572 7479  ow">.  <property
+00000090: 206e 616d 653d 2267 656f 6d65 7472 7922   name="geometry"
+000000a0: 3e0a 2020 203c 7265 6374 3e0a 2020 2020  >.   <rect>.    
+000000b0: 3c78 3e30 3c2f 783e 0a20 2020 203c 793e  <x>0</x>.    <y>
+000000c0: 303c 2f79 3e0a 2020 2020 3c77 6964 7468  0</y>.    <width
+000000d0: 3e38 3030 3c2f 7769 6474 683e 0a20 2020  >800</width>.   
+000000e0: 203c 6865 6967 6874 3e36 3030 3c2f 6865   <height>600</he
+000000f0: 6967 6874 3e0a 2020 203c 2f72 6563 743e  ight>.   </rect>
+00000100: 0a20 203c 2f70 726f 7065 7274 793e 0a20  .  </property>. 
+00000110: 203c 7072 6f70 6572 7479 206e 616d 653d   <property name=
+00000120: 2277 696e 646f 7754 6974 6c65 223e 0a20  "windowTitle">. 
+00000130: 2020 3c73 7472 696e 673e 4d61 696e 5769    <string>MainWi
+00000140: 6e64 6f77 3c2f 7374 7269 6e67 3e0a 2020  ndow</string>.  
+00000150: 3c2f 7072 6f70 6572 7479 3e0a 2020 3c77  </property>.  <w
+00000160: 6964 6765 7420 636c 6173 733d 2251 5769  idget class="QWi
+00000170: 6467 6574 2220 6e61 6d65 3d22 6365 6e74  dget" name="cent
+00000180: 7261 6c77 6964 6765 7422 3e0a 2020 203c  ralwidget">.   <
+00000190: 7769 6467 6574 2063 6c61 7373 3d22 5154  widget class="QT
+000001a0: 6578 7445 6469 7422 206e 616d 653d 2274  extEdit" name="t
+000001b0: 6578 7445 6469 7422 3e0a 2020 2020 3c70  extEdit">.    <p
+000001c0: 726f 7065 7274 7920 6e61 6d65 3d22 6765  roperty name="ge
+000001d0: 6f6d 6574 7279 223e 0a20 2020 2020 3c72  ometry">.     <r
+000001e0: 6563 743e 0a20 2020 2020 203c 783e 3130  ect>.      <x>10
+000001f0: 3c2f 783e 0a20 2020 2020 203c 793e 3430  </x>.      <y>40
+00000200: 3c2f 793e 0a20 2020 2020 203c 7769 6474  </y>.      <widt
+00000210: 683e 3738 313c 2f77 6964 7468 3e0a 2020  h>781</width>.  
+00000220: 2020 2020 3c68 6569 6768 743e 3532 313c      <height>521<
+00000230: 2f68 6569 6768 743e 0a20 2020 2020 3c2f  /height>.     </
+00000240: 7265 6374 3e0a 2020 2020 3c2f 7072 6f70  rect>.    </prop
+00000250: 6572 7479 3e0a 2020 203c 2f77 6964 6765  erty>.   </widge
+00000260: 743e 0a20 2020 3c77 6964 6765 7420 636c  t>.   <widget cl
+00000270: 6173 733d 2251 4c61 6265 6c22 206e 616d  ass="QLabel" nam
+00000280: 653d 226c 6162 656c 223e 0a20 2020 203c  e="label">.    <
+00000290: 7072 6f70 6572 7479 206e 616d 653d 2267  property name="g
+000002a0: 656f 6d65 7472 7922 3e0a 2020 2020 203c  eometry">.     <
+000002b0: 7265 6374 3e0a 2020 2020 2020 3c78 3e31  rect>.      <x>1
+000002c0: 303c 2f78 3e0a 2020 2020 2020 3c79 3e31  0</x>.      <y>1
+000002d0: 303c 2f79 3e0a 2020 2020 2020 3c77 6964  0</y>.      <wid
+000002e0: 7468 3e39 313c 2f77 6964 7468 3e0a 2020  th>91</width>.  
+000002f0: 2020 2020 3c68 6569 6768 743e 3136 3c2f      <height>16</
+00000300: 6865 6967 6874 3e0a 2020 2020 203c 2f72  height>.     </r
+00000310: 6563 743e 0a20 2020 203c 2f70 726f 7065  ect>.    </prope
+00000320: 7274 793e 0a20 2020 203c 7072 6f70 6572  rty>.    <proper
+00000330: 7479 206e 616d 653d 2274 6578 7422 3e0a  ty name="text">.
+00000340: 2020 2020 203c 7374 7269 6e67 3ee5 bd93       <string>...
+00000350: e589 8de5 a484 e790 86e7 9bae e5bd 95ef  ................
+00000360: bc9a 3c2f 7374 7269 6e67 3e0a 2020 2020  ..</string>.    
+00000370: 3c2f 7072 6f70 6572 7479 3e0a 2020 203c  </property>.   <
+00000380: 2f77 6964 6765 743e 0a20 2020 3c77 6964  /widget>.   <wid
+00000390: 6765 7420 636c 6173 733d 2251 4c69 6e65  get class="QLine
+000003a0: 4564 6974 2220 6e61 6d65 3d22 6c69 6e65  Edit" name="line
+000003b0: 4564 6974 223e 0a20 2020 203c 7072 6f70  Edit">.    <prop
+000003c0: 6572 7479 206e 616d 653d 2267 656f 6d65  erty name="geome
+000003d0: 7472 7922 3e0a 2020 2020 203c 7265 6374  try">.     <rect
+000003e0: 3e0a 2020 2020 2020 3c78 3e31 3030 3c2f  >.      <x>100</
+000003f0: 783e 0a20 2020 2020 203c 793e 3130 3c2f  x>.      <y>10</
+00000400: 793e 0a20 2020 2020 203c 7769 6474 683e  y>.      <width>
+00000410: 3639 313c 2f77 6964 7468 3e0a 2020 2020  691</width>.    
+00000420: 2020 3c68 6569 6768 743e 3230 3c2f 6865    <height>20</he
+00000430: 6967 6874 3e0a 2020 2020 203c 2f72 6563  ight>.     </rec
+00000440: 743e 0a20 2020 203c 2f70 726f 7065 7274  t>.    </propert
+00000450: 793e 0a20 2020 3c2f 7769 6467 6574 3e0a  y>.   </widget>.
+00000460: 2020 3c2f 7769 6467 6574 3e0a 2020 3c77    </widget>.  <w
+00000470: 6964 6765 7420 636c 6173 733d 2251 4d65  idget class="QMe
+00000480: 6e75 4261 7222 206e 616d 653d 226d 656e  nuBar" name="men
+00000490: 7562 6172 223e 0a20 2020 3c70 726f 7065  ubar">.   <prope
+000004a0: 7274 7920 6e61 6d65 3d22 6765 6f6d 6574  rty name="geomet
+000004b0: 7279 223e 0a20 2020 203c 7265 6374 3e0a  ry">.    <rect>.
+000004c0: 2020 2020 203c 783e 303c 2f78 3e0a 2020       <x>0</x>.  
+000004d0: 2020 203c 793e 303c 2f79 3e0a 2020 2020     <y>0</y>.    
+000004e0: 203c 7769 6474 683e 3830 303c 2f77 6964   <width>800</wid
+000004f0: 7468 3e0a 2020 2020 203c 6865 6967 6874  th>.     <height
+00000500: 3e32 363c 2f68 6569 6768 743e 0a20 2020  >26</height>.   
+00000510: 203c 2f72 6563 743e 0a20 2020 3c2f 7072   </rect>.   </pr
+00000520: 6f70 6572 7479 3e0a 2020 203c 7769 6467  operty>.   <widg
+00000530: 6574 2063 6c61 7373 3d22 514d 656e 7522  et class="QMenu"
+00000540: 206e 616d 653d 226d 656e 7522 3e0a 2020   name="menu">.  
+00000550: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+00000560: 3d22 7469 746c 6522 3e0a 2020 2020 203c  ="title">.     <
+00000570: 7374 7269 6e67 3ee8 aebe e7bd ae3c 2f73  string>......</s
+00000580: 7472 696e 673e 0a20 2020 203c 2f70 726f  tring>.    </pro
+00000590: 7065 7274 793e 0a20 2020 203c 6164 6461  perty>.    <adda
+000005a0: 6374 696f 6e20 6e61 6d65 3d22 6163 7469  ction name="acti
+000005b0: 6f6e 5365 6c65 6374 5f44 6972 222f 3e0a  onSelect_Dir"/>.
+000005c0: 2020 203c 2f77 6964 6765 743e 0a20 2020     </widget>.   
+000005d0: 3c77 6964 6765 7420 636c 6173 733d 2251  <widget class="Q
+000005e0: 4d65 6e75 2220 6e61 6d65 3d22 6d65 6e75  Menu" name="menu
+000005f0: 5f32 223e 0a20 2020 203c 7072 6f70 6572  _2">.    <proper
+00000600: 7479 206e 616d 653d 2274 6974 6c65 223e  ty name="title">
+00000610: 0a20 2020 2020 3c73 7472 696e 673e e9a1  .     <string>..
+00000620: b9e7 9bae 3c2f 7374 7269 6e67 3e0a 2020  ....</string>.  
+00000630: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
+00000640: 2020 3c61 6464 6163 7469 6f6e 206e 616d    <addaction nam
+00000650: 653d 2261 6374 696f 6e72 6570 6c61 6365  e="actionreplace
+00000660: 222f 3e0a 2020 203c 2f77 6964 6765 743e  "/>.   </widget>
+00000670: 0a20 2020 3c77 6964 6765 7420 636c 6173  .   <widget clas
+00000680: 733d 2251 4d65 6e75 2220 6e61 6d65 3d22  s="QMenu" name="
+00000690: 6d65 6e75 5f33 223e 0a20 2020 203c 7072  menu_3">.    <pr
+000006a0: 6f70 6572 7479 206e 616d 653d 2274 6974  operty name="tit
+000006b0: 6c65 223e 0a20 2020 2020 3c73 7472 696e  le">.     <strin
+000006c0: 673e e4b8 93e5 88a9 3c2f 7374 7269 6e67  g>......</string
+000006d0: 3e0a 2020 2020 3c2f 7072 6f70 6572 7479  >.    </property
+000006e0: 3e0a 2020 2020 3c61 6464 6163 7469 6f6e  >.    <addaction
+000006f0: 206e 616d 653d 2261 6374 696f 6e63 6865   name="actionche
+00000700: 636b 222f 3e0a 2020 203c 2f77 6964 6765  ck"/>.   </widge
+00000710: 743e 0a20 2020 3c77 6964 6765 7420 636c  t>.   <widget cl
+00000720: 6173 733d 2251 4d65 6e75 2220 6e61 6d65  ass="QMenu" name
+00000730: 3d22 6d65 6e75 5f34 223e 0a20 2020 203c  ="menu_4">.    <
+00000740: 7072 6f70 6572 7479 206e 616d 653d 2274  property name="t
+00000750: 6974 6c65 223e 0a20 2020 2020 3c73 7472  itle">.     <str
+00000760: 696e 673e e6a3 80e6 9fa5 3c2f 7374 7269  ing>......</stri
+00000770: 6e67 3e0a 2020 2020 3c2f 7072 6f70 6572  ng>.    </proper
+00000780: 7479 3e0a 2020 2020 3c61 6464 6163 7469  ty>.    <addacti
+00000790: 6f6e 206e 616d 653d 2273 6570 6172 6174  on name="separat
+000007a0: 6f72 222f 3e0a 2020 2020 3c61 6464 6163  or"/>.    <addac
+000007b0: 7469 6f6e 206e 616d 653d 2261 6374 696f  tion name="actio
+000007c0: 6e63 6865 636b 616c 6c22 2f3e 0a20 2020  ncheckall"/>.   
+000007d0: 3c2f 7769 6467 6574 3e0a 2020 203c 6164  </widget>.   <ad
+000007e0: 6461 6374 696f 6e20 6e61 6d65 3d22 6d65  daction name="me
+000007f0: 6e75 222f 3e0a 2020 203c 6164 6461 6374  nu"/>.   <addact
+00000800: 696f 6e20 6e61 6d65 3d22 6d65 6e75 5f34  ion name="menu_4
+00000810: 222f 3e0a 2020 203c 6164 6461 6374 696f  "/>.   <addactio
+00000820: 6e20 6e61 6d65 3d22 6d65 6e75 5f32 222f  n name="menu_2"/
+00000830: 3e0a 2020 203c 6164 6461 6374 696f 6e20  >.   <addaction 
+00000840: 6e61 6d65 3d22 6d65 6e75 5f33 222f 3e0a  name="menu_3"/>.
+00000850: 2020 3c2f 7769 6467 6574 3e0a 2020 3c77    </widget>.  <w
+00000860: 6964 6765 7420 636c 6173 733d 2251 5374  idget class="QSt
+00000870: 6174 7573 4261 7222 206e 616d 653d 2273  atusBar" name="s
+00000880: 7461 7475 7362 6172 222f 3e0a 2020 3c61  tatusbar"/>.  <a
+00000890: 6374 696f 6e20 6e61 6d65 3d22 6163 7469  ction name="acti
+000008a0: 6f6e 5365 6c65 6374 5f44 6972 223e 0a20  onSelect_Dir">. 
+000008b0: 2020 3c70 726f 7065 7274 7920 6e61 6d65    <property name
+000008c0: 3d22 7465 7874 223e 0a20 2020 203c 7374  ="text">.    <st
+000008d0: 7269 6e67 3e53 656c 6563 7420 4469 723c  ring>Select Dir<
+000008e0: 2f73 7472 696e 673e 0a20 2020 3c2f 7072  /string>.   </pr
+000008f0: 6f70 6572 7479 3e0a 2020 3c2f 6163 7469  operty>.  </acti
+00000900: 6f6e 3e0a 2020 3c61 6374 696f 6e20 6e61  on>.  <action na
+00000910: 6d65 3d22 6163 7469 6f6e 6368 6563 6b22  me="actioncheck"
+00000920: 3e0a 2020 203c 7072 6f70 6572 7479 206e  >.   <property n
+00000930: 616d 653d 2274 6578 7422 3e0a 2020 2020  ame="text">.    
+00000940: 3c73 7472 696e 673e e6a3 80e6 9fa5 3c2f  <string>......</
+00000950: 7374 7269 6e67 3e0a 2020 203c 2f70 726f  string>.   </pro
+00000960: 7065 7274 793e 0a20 203c 2f61 6374 696f  perty>.  </actio
+00000970: 6e3e 0a20 203c 6163 7469 6f6e 206e 616d  n>.  <action nam
+00000980: 653d 2261 6374 696f 6e72 6570 6c61 6365  e="actionreplace
+00000990: 223e 0a20 2020 3c70 726f 7065 7274 7920  ">.   <property 
+000009a0: 6e61 6d65 3d22 7465 7874 223e 0a20 2020  name="text">.   
+000009b0: 203c 7374 7269 6e67 3ee6 89b9 e987 8fe6   <string>.......
+000009c0: 9bbf e68d a23c 2f73 7472 696e 673e 0a20  .....</string>. 
+000009d0: 2020 3c2f 7072 6f70 6572 7479 3e0a 2020    </property>.  
+000009e0: 3c2f 6163 7469 6f6e 3e0a 2020 3c61 6374  </action>.  <act
+000009f0: 696f 6e20 6e61 6d65 3d22 6163 7469 6f6e  ion name="action
+00000a00: 6368 6563 6b61 6c6c 223e 0a20 2020 3c70  checkall">.   <p
+00000a10: 726f 7065 7274 7920 6e61 6d65 3d22 7465  roperty name="te
+00000a20: 7874 223e 0a20 2020 203c 7374 7269 6e67  xt">.    <string
+00000a30: 3ee6 a380 e69f a5e6 8980 e69c 89e9 a1b9  >...............
+00000a40: 3c2f 7374 7269 6e67 3e0a 2020 203c 2f70  </string>.   </p
+00000a50: 726f 7065 7274 793e 0a20 203c 2f61 6374  roperty>.  </act
+00000a60: 696f 6e3e 0a20 3c2f 7769 6467 6574 3e0a  ion>. </widget>.
+00000a70: 203c 7265 736f 7572 6365 732f 3e0a 203c   <resources/>. <
+00000a80: 636f 6e6e 6563 7469 6f6e 732f 3e0a 3c2f  connections/>.</
+00000a90: 7569 3e0a                                ui>.
```

### Comparing `docrobot-1.0.2/src/docrobot/guimain.pyw` & `docrobot-1.0.3/src/docrobot/guimain.pyw`

 * *Files 22% similar despite different names*

```diff
@@ -1,260 +1,271 @@
-import os
-import re
-import sys
-from configparser import ConfigParser
-
-from PySide6 import QtCore
-from PySide6.QtCore import QEventLoop, QTimer
-from PySide6.QtWidgets import QApplication, QMainWindow, QFileDialog
-from docx import Document
-from docx.opc.exceptions import PackageNotFoundError
-from openpyxl.reader.excel import load_workbook
-from win32com.client import Dispatch
-
-from docrobot import util
-from docrobot.form import Ui_MainWindow
-
-
-class EmittingStr(QtCore.QObject):
-    textWritten = QtCore.Signal(str)
-
-    def write(self, text):
-        self.textWritten.emit(str(text))
-        loop = QEventLoop()
-        QTimer.singleShot(100, loop.quit)
-        loop.exec()
-        QApplication.processEvents()
-
-
-class MainWindow(Ui_MainWindow, QMainWindow):
-    workdir = ''
-    file_prj = ''
-    file_pat = ''
-    pat_dict = {}  # 专利->序号字典
-    pat_dict2 = {}  # 专利->专利编号字典
-    arr_prj = []
-
-    def __init__(self):
-        super(MainWindow, self).__init__()
-        self.setupUi(self)
-        sys.stdout = EmittingStr()
-        sys.stdout.textWritten.connect(self.outputWritten)
-        sys.stderr = EmittingStr()
-        sys.stderr.textWritten.connect(self.outputWritten)
-
-        self.actionSelect_Dir.triggered.connect(self.setDocUrl)
-        self.actioncheck.triggered.connect(lambda: self.checkpatent(True))
-        self.actionreplace.triggered.connect(lambda: self.replaceprj(True))
-        self.actioncheckall.triggered.connect(self.checkall)
-
-        self.config = ConfigParser()
-        try:
-            self.config.read('config.ini', encoding='UTF-8')
-            self.workdir = self.config['config']['lasting']
-        except KeyError:
-            self.config.add_section('config')
-        try:
-            if self.workdir != '':
-                self.onchangeworkdir()
-        except FileNotFoundError as e:
-            self.textEdit.append('路径错误：' + e.filename)
-            self.workdir = ''
-        self.lineEdit.setText(self.workdir)
-
-    def outputWritten(self, text):
-        # cursor = self.textEdit.textCursor()
-        # cursor.movePosition(QTextCursor.End)
-        # cursor.insertText(text)
-        # self.textEdit.setTextCursor(cursor)
-        # self.textEdit.ensureCursorVisible()
-        self.textEdit.append(text)
-
-    def setDocUrl(self):
-        # 重新选择输入和输出目录时，进度条设置为0，文本框的内容置空
-        tempdir = QFileDialog.getExistingDirectory(self, "选中项目所在目录", r"")
-        if tempdir != '':
-            self.workdir = tempdir
-            self.onchangeworkdir()
-            with open('config.ini', 'w', encoding='utf-8') as file:
-                self.config['config']['lasting'] = self.workdir
-                self.config.write(file)  # 数据写入配置文件
-
-    def onchangeworkdir(self):
-        self.lineEdit.setText(self.workdir)
-        for file_sum in os.listdir(self.workdir):
-            if file_sum.endswith('立项报告汇总表.xlsx') and not file_sum.startswith('~$'):
-                self.file_prj = self.workdir + '/' + file_sum
-            if file_sum.endswith('知识产权汇总表.xlsx') and not file_sum.startswith('~$'):
-                self.file_pat = self.workdir + '/' + file_sum
-        if self.file_prj == '':
-            self.textEdit.append('没找到：' + '立项报告汇总表.xlsx')
-        if self.file_pat == '':
-            self.textEdit.append('没找到：' + '知识产权汇总表.xlsx')
-
-    def replaceprj(self, modify=False):
-        if modify:
-            self.textEdit.setText('')
-            self.update_data()
-
-        for project in self.arr_prj:
-            # self.textEdit.append(project.p_order + ' 项目开始处理...')
-            match = 0  # 已匹配条目数
-            doc_name = ''
-            try:
-                doc_name = self.workdir + '/RD' + project.p_order + project.p_name + '.docx'
-                document = Document(doc_name)
-                # debug_doc(document)
-                # TODO to be fixed
-                # replace_header(document)
-                match = match + util.first_table(document, project)
-                match = match + util.start_time(document, project)
-                match = match + util.second_table(document, project)
-                match = match + util.third_table(document, project)
-
-                match = match + self.checkpat2(document, project)
-
-                if modify:
-                    document.save(doc_name)
-            except PackageNotFoundError:
-                self.textEdit.append('Error打开文件错误：' + doc_name)
-            except PermissionError:
-                self.textEdit.append('Error 保存文件错误，可能是文件已被打开：' + doc_name)
-            self.textEdit.append(project.p_order + ' 项目：处理完成。 <font color="green"><b>'
-                                 + str(match) + ' </b></font> 项条目匹配。')
-
-    def checkpatent(self, modify=False):
-        if modify:
-            self.textEdit.setText('')
-            self.update_data()
-
-        match = 0  # 已匹配条目数
-        changed = False
-        wb = load_workbook(self.file_prj)
-        ws = wb.active
-        max_row_num = ws.max_row
-        range_cell = ws[f'A3:P{max_row_num}']
-        i: int = 0
-        for r in range_cell:
-            if r[11].value is None:
-                break
-            pat_name = str(r[11].value).strip()
-
-            if pat_name == '无':
-                if r[14].value != '无':
-                    self.textEdit.append(str(i + 3) + ' 行: ' + str(r[14].value) + ' 替换为 ' + '无')
-                    r[14].value = pat_name
-                    changed |= True
-                else:
-                    match = match + 1
-            else:
-                lst = pat_name.splitlines()
-                rep = [self.pat_dict[x] if x in self.pat_dict else x for x in lst]
-                for element in rep:
-                    if re.search('^\d\d$', element) is None:
-                        self.textEdit.append('专利IP错误：' + element)
-                rep = map(lambda e: 'IP' + e, rep)
-                new_ip = ';'.join(rep)
-                if r[14].value != new_ip:
-                    self.textEdit.append(str(i + 3) + ' 行: ' + str(r[14].value) + ' 替换为 ' + new_ip)
-                    r[14].value = new_ip
-                    changed |= True
-                else:
-                    match = match + 1
-            i = i + 1
-        try:
-            if changed and modify:
-                wb.save(self.file_prj)
-                xl_app = Dispatch("Excel.Application")
-                xl_app.Visible = False
-                xl_app.DisplayAlerts = False
-                xl_book = xl_app.Workbooks.Open(self.file_prj)
-                xl_book.Close(True)
-        except PermissionError:
-            self.textEdit.append('写文件失败，关闭其他占用该文件的程序.' + self.file_prj)
-        wb.close()
-        self.textEdit.append('项目立项表IP更新完成。 <font color="green"><b>' + str(match) + ' </b></font> 项条目匹配。')
-
-
-    def checkpat2(self, doc, prj):
-        match = 0
-        lst = prj.pat_list.splitlines()
-        for pat_name in lst:
-            if pat_name in self.pat_dict2:
-                pat_num = self.pat_dict2[pat_name]
-                found = False
-                regex = pat_name.replace('[', r'\[').replace(']', r'\]'.replace('(', r'\(').replace(')', r'\)'))
-                for i, para in enumerate(doc.tables[2].rows[4].cells[0].paragraphs):
-                    if re.search(regex + '，.*号：', para.text):
-                        found |= True
-                        result = re.search(regex + '，.*号：' + pat_num, para.text)
-                        if result is None:
-                            self.textEdit.append('专利名和编号不匹配：' + pat_name + ' , ' + pat_num)
-                            self.textEdit.append('文档内容：' + para.text)
-                        else:
-                            match = match + 1
-                if not found:
-                    self.textEdit.append('全文找不到：' + pat_name)
-            else:
-                self.textEdit.append('Error没有找到专利：' + pat_name)
-        return match
-
-    def update_data(self):
-        self.pat_dict.clear()
-        self.pat_dict2.clear()
-        wb = load_workbook(self.file_pat, read_only=True, data_only=True)
-        ws = wb.active
-        max_row_num = ws.max_row
-        range_cell = ws[f'A3:D{max_row_num}']
-        for r in range_cell:
-            if r[0].value is None:
-                break
-            p_order = str(r[0].value).strip().zfill(2)
-            p_name = str(r[1].value).strip()
-            p_patnum = str(r[3].value).strip()
-            self.pat_dict[p_name] = p_order
-            self.pat_dict2[p_name] = p_patnum
-        wb.close()
-
-        self.arr_prj.clear()
-        com_name = 'XX公司'
-        wb = load_workbook(self.file_prj, read_only=True, data_only=True)
-        ws = wb.active
-        if str(ws['A1'].value).find(u'公司') != -1:
-            com_name = str(ws['A1'].value).split("公司")[0] + '公司'
-        else:
-            print("Error: 找不到 公司名")
-        max_row_num = ws.max_row
-        range_cell = ws[f'A3:P{max_row_num}']
-        for r in range_cell:
-            if r[0].value is None:
-                break
-            project = util.Project()
-            project.p_comname = com_name
-            project.p_order = str(r[0].value).strip().zfill(2)
-            project.p_name = str(r[1].value).strip()  # 项目名称
-            project.p_start = r[2].value.strftime('%Y-%m-%d')
-            project.p_end = r[3].value.strftime('%Y-%m-%d')
-            project.p_cost = str(r[5].value).strip()
-            project.p_people = str(r[6].value).strip()  # 人数
-            project.p_owner = str(r[7].value).strip()  # 项目负责人
-            project.p_rnd = str(r[8].value).strip()  # 研发人员
-            project.p_money = str(r[9].value).strip()  # 总预算
-            project.pat_list = str(r[11].value).strip()  # 知识产权名称
-            project.ip_list = str(r[14].value).strip()  # IP
-            self.arr_prj.append(project)
-        wb.close()
-
-    def checkall(self):
-        self.textEdit.setText('')
-        self.update_data()
-
-        self.checkpatent(False)
-        self.replaceprj(False)
-
-
-
-if __name__ == "__main__":
-    app = QApplication(sys.argv)
-    window = MainWindow()
-    window.show()
-    sys.exit(app.exec())
+import io
+import os
+import re
+import sys
+from configparser import ConfigParser
+
+from PySide6 import QtCore
+from PySide6.QtCore import QEventLoop, QTimer
+from PySide6.QtWidgets import QApplication, QMainWindow, QFileDialog
+from docx import Document
+from docx.opc.exceptions import PackageNotFoundError
+from openpyxl.reader.excel import load_workbook
+from win32com.client import DispatchEx
+
+from docrobot import util
+from docrobot.form import Ui_MainWindow
+
+
+class EmittingStr(QtCore.QObject):
+    textWritten = QtCore.Signal(str)
+
+    def write(self, text):
+        self.textWritten.emit(str(text))
+        loop = QEventLoop()
+        QTimer.singleShot(100, loop.quit)
+        loop.exec()
+        QApplication.processEvents()
+
+
+class MainWindow(Ui_MainWindow, QMainWindow):
+    workdir = ''
+    file_prj = ''
+    file_pat = ''
+    pat_dict = {}  # 专利->序号字典
+    pat_dict2 = {}  # 专利->专利编号字典
+    arr_prj = []
+
+    def __init__(self):
+        super(MainWindow, self).__init__()
+        self.setupUi(self)
+        sys.stdout = EmittingStr()
+        sys.stdout.textWritten.connect(self.outputWritten)
+        sys.stderr = EmittingStr()
+        sys.stderr.textWritten.connect(self.outputWritten)
+
+        self.actionSelect_Dir.triggered.connect(self.setDocUrl)
+        self.actioncheck.triggered.connect(lambda: self.checkpatent(True))
+        self.actionreplace.triggered.connect(lambda: self.replaceprj(True))
+        self.actioncheckall.triggered.connect(self.checkall)
+
+        self.config = ConfigParser()
+        try:
+            self.config.read('config.ini', encoding='UTF-8')
+            self.workdir = self.config['config']['lasting']
+        except KeyError:
+            self.config.add_section('config')
+        try:
+            if self.workdir != '':
+                self.onchangeworkdir()
+        except FileNotFoundError as e:
+            self.textEdit.append('路径错误：' + e.filename)
+            self.workdir = ''
+        self.lineEdit.setText(self.workdir)
+
+    def outputWritten(self, text):
+        # cursor = self.textEdit.textCursor()
+        # cursor.movePosition(QTextCursor.End)
+        # cursor.insertText(text)
+        # self.textEdit.setTextCursor(cursor)
+        # self.textEdit.ensureCursorVisible()
+        self.textEdit.append(text)
+
+    def setDocUrl(self):
+        # 重新选择输入和输出目录时，进度条设置为0，文本框的内容置空
+        tempdir = QFileDialog.getExistingDirectory(self, "选中项目所在目录", r"")
+        if tempdir != '':
+            self.workdir = tempdir
+            self.onchangeworkdir()
+            with open('config.ini', 'w', encoding='utf-8') as file:
+                self.config['config']['lasting'] = self.workdir
+                self.config.write(file)  # 数据写入配置文件
+
+    def onchangeworkdir(self):
+        self.lineEdit.setText(self.workdir)
+        for file_sum in os.listdir(self.workdir):
+            if file_sum.endswith('立项报告汇总表.xlsx') and not file_sum.startswith('~$'):
+                self.file_prj = self.workdir + '/' + file_sum
+            if file_sum.endswith('知识产权汇总表.xlsx') and not file_sum.startswith('~$'):
+                self.file_pat = self.workdir + '/' + file_sum
+        if self.file_prj == '':
+            self.textEdit.append('没找到：' + '立项报告汇总表.xlsx')
+        if self.file_pat == '':
+            self.textEdit.append('没找到：' + '知识产权汇总表.xlsx')
+
+    def replaceprj(self, modify=False):
+        if modify:
+            self.textEdit.setText('')
+            self.update_data()
+
+        for project in self.arr_prj:
+            # self.textEdit.append(project.p_order + ' 项目开始处理...')
+            match = 0  # 已匹配条目数
+            doc_name = ''
+            try:
+                doc_name = self.workdir + '/RD' + project.p_order + project.p_name + '.docx'
+                document = Document(doc_name)
+                # debug_doc(document)
+                # TODO to be fixed
+                # replace_header(document)
+                match = match + util.first_table(document, project)
+                match = match + util.start_time(document, project)
+                match = match + util.second_table(document, project)
+                match = match + util.third_table(document, project)
+
+                match = match + self.checkpat2(document, project)
+
+                if modify:
+                    document.save(doc_name)
+            except PackageNotFoundError:
+                self.textEdit.append('Error打开文件错误：' + doc_name)
+            except PermissionError:
+                self.textEdit.append('Error 保存文件错误，可能是文件已被打开：' + doc_name)
+            self.textEdit.append(project.p_order + ' 项目：处理完成。 <font color="green"><b>'
+                                 + str(match) + ' </b></font> 项条目匹配。')
+
+    def checkpatent(self, modify=False):
+        if modify:
+            self.textEdit.setText('')
+            self.update_data()
+
+        match = 0  # 已匹配条目数
+        changed = False
+        wb = load_workbook(self.file_prj)
+        ws = wb.active
+        max_row_num = ws.max_row
+        range_cell = ws[f'A3:P{max_row_num}']
+        i: int = 0
+        for r in range_cell:
+            if r[11].value is None:
+                break
+            pat_name = str(r[11].value).strip()
+
+            if pat_name == '无':
+                if r[14].value != '无':
+                    self.textEdit.append(str(i + 3) + ' 行: ' + str(r[14].value) + ' 替换为 ' + '无')
+                    r[14].value = pat_name
+                    changed |= True
+                else:
+                    match = match + 1
+            else:
+                lst = pat_name.splitlines()
+                rep = [self.pat_dict[x] if x in self.pat_dict else x for x in lst]
+                for element in rep:
+                    if re.search('^\d\d$', element) is None:
+                        self.textEdit.append('专利IP错误：' + element)
+                rep = map(lambda e: 'IP' + e, rep)
+                new_ip = ';'.join(rep)
+                if r[14].value != new_ip:
+                    self.textEdit.append(str(i + 3) + ' 行: ' + str(r[14].value) + ' 替换为 ' + new_ip)
+                    r[14].value = new_ip
+                    changed |= True
+                else:
+                    match = match + 1
+            i = i + 1
+        try:
+            if changed and modify:
+                wb.save(self.file_prj)
+                xl_app = DispatchEx("Excel.Application")
+                xl_app.Visible = False
+                xl_app.DisplayAlerts = False
+                xl_book = xl_app.Workbooks.Open(self.file_prj)
+                xl_book.Saved = False
+                xl_book.Close(True)
+                xl_book = None
+                xl_app.Quit()
+                xl_app = None
+        except PermissionError:
+            self.textEdit.append('写文件失败，关闭其他占用该文件的程序.' + self.file_prj)
+        wb.close()
+        self.textEdit.append('项目立项表IP更新完成。 <font color="green"><b>' + str(match) + ' </b></font> 项条目匹配。')
+
+
+    def checkpat2(self, doc, prj):
+        match = 0
+        lst = prj.pat_list.splitlines()
+        for pat_name in lst:
+            if pat_name in self.pat_dict2:
+                pat_num = self.pat_dict2[pat_name]
+                found = False
+                regex = pat_name.replace('[', r'\[').replace(']', r'\]'.replace('(', r'\(').replace(')', r'\)'))
+                for i, para in enumerate(doc.tables[2].rows[4].cells[0].paragraphs):
+                    if re.search(regex + '，.*号：', para.text):
+                        found |= True
+                        result = re.search(regex + '，.*号：' + pat_num, para.text)
+                        if result is None:
+                            self.textEdit.append('专利名和编号不匹配：' + pat_name + ' , ' + pat_num)
+                            self.textEdit.append('文档内容：' + para.text)
+                        else:
+                            match = match + 1
+                if not found:
+                    self.textEdit.append('全文找不到：' + pat_name)
+            else:
+                self.textEdit.append('Error没有找到专利：' + pat_name)
+        return match
+
+    def update_data(self):
+        self.pat_dict.clear()
+        self.pat_dict2.clear()
+        with open(self.file_pat, "rb") as f:
+            in_mem_file = io.BytesIO(f.read())
+        wb = load_workbook(in_mem_file, read_only=True, data_only=True)
+        ws = wb.active
+        max_row_num = ws.max_row
+        range_cell = ws[f'A3:D{max_row_num}']
+        for r in range_cell:
+            if r[0].value is None:
+                break
+            p_order = str(r[0].value).strip().zfill(2)
+            p_name = str(r[1].value).strip()
+            p_patnum = str(r[3].value).strip()
+            self.pat_dict[p_name] = p_order
+            self.pat_dict2[p_name] = p_patnum
+        wb.close()
+
+        self.arr_prj.clear()
+        com_name = 'XX公司'
+        with open(self.file_prj, "rb") as f:
+            in_mem_file = io.BytesIO(f.read())
+        wb = load_workbook(in_mem_file, read_only=True, data_only=True)
+        ws = wb.active
+        if str(ws['A1'].value).find(u'公司') != -1:
+            com_name = str(ws['A1'].value).split("公司")[0] + '公司'
+        else:
+            print("Error: 找不到 公司名")
+        max_row_num = ws.max_row
+        range_cell = ws[f'A3:P{max_row_num}']
+        for r in range_cell:
+            if r[0].value is None:
+                break
+            project = util.Project()
+            project.p_comname = com_name
+            project.p_order = str(r[0].value).strip().zfill(2)
+            project.p_name = str(r[1].value).strip()  # 项目名称
+            project.p_start = r[2].value.strftime('%Y-%m-%d')
+            project.p_end = r[3].value.strftime('%Y-%m-%d')
+            project.p_cost = str(r[5].value).strip()
+            project.p_people = str(r[6].value).strip()  # 人数
+            project.p_owner = str(r[7].value).strip()  # 项目负责人
+            project.p_rnd = str(r[8].value).strip()  # 研发人员
+            project.p_money = str(r[9].value).strip()  # 总预算
+            project.pat_list = str(r[11].value).strip()  # 知识产权名称
+            project.ip_list = str(r[14].value).strip()  # IP
+            self.arr_prj.append(project)
+        wb.close()
+        if len(self.arr_prj) == 0:
+            print("Error: 立项汇总表错误，使用Excel重新保存.")
+
+    def checkall(self):
+        self.textEdit.setText('')
+        self.update_data()
+
+        self.checkpatent(False)
+        self.replaceprj(False)
+
+
+
+if __name__ == "__main__":
+    app = QApplication(sys.argv)
+    window = MainWindow()
+    window.show()
+    sys.exit(app.exec())
```

### Comparing `docrobot-1.0.2/src/docrobot/util.py` & `docrobot-1.0.3/src/docrobot/util.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,256 +1,256 @@
-import os
-import re
-import sys
-from configparser import ConfigParser
-from docx import Document
-from docx.opc.exceptions import PackageNotFoundError
-from openpyxl import load_workbook
-from colorama import init, Fore
-
-
-class Project(object):
-    p_comname = ''  # 公司名称
-    p_order = ''  # 序号
-    p_name = ''  # 项目名
-    p_start = ''
-    p_end = ''
-    p_cost = ''
-    p_people = ''  # 人数
-    p_owner = ''  # 项目负责人
-    p_rnd = ''  # 研发人员
-    p_money = ''  # 总预算
-
-
-def check_and_change(doc, replace):
-    """
-    遍历word中的所有 paragraphs，在每一段中发现含有key 的内容，就替换为 value 。
-    （key 和 value 都是replace_dict中的键值对。）
-    """
-    for para in doc.paragraphs:
-        for i in range(len(para.runs)):
-            # print(">>>" + para.runs[i].text)
-            for key, value in replace.items():
-                if key in para.runs[i].text:
-                    print(key + "-->" + value)
-                    para.runs[i].text = para.runs[i].text.replace(key, value)
-    return doc
-
-
-def replace_tables(doc, replace):
-    for table in doc.tables:
-        for row in table.rows:
-            for cell in row.cells:
-                for para in cell.paragraphs:
-                    for i in range(len(para.runs)):
-                        # print(">>>" + para.runs[i].text)
-                        for key, value in replace.items():
-                            if key in para.runs[i].text:
-                                print(key + "-->" + value)
-                                para.runs[i].text = para.runs[i].text.replace(key, value)
-    return doc
-
-
-def clear_runs(runs):
-    for i, run in enumerate(runs):
-        if i > 0:
-            run.clear()
-    return runs
-
-
-def debug_doc(doc):
-    for i, sect in enumerate(doc.sections):
-        for j, para in enumerate(sect.header.paragraphs):
-            print(f'Sec.{i} Para.{j} : ', para.text, sep='')
-            for k, run in enumerate(para.runs):
-                print(f'Sec.{i} Para.{j} Run{k}: ', run.text, sep='')
-    for i, para in enumerate(doc.paragraphs):
-        print(f'Para.{i} : ', para.text, sep='')
-        for j, run in enumerate(para.runs):
-            print(f'Para.{i} Run{j}: ', run.text, sep='')
-    for k, table in enumerate(doc.tables):
-        for l, row in enumerate(table.rows):
-            for m, cell in enumerate(row.cells):
-                for i, para in enumerate(cell.paragraphs):
-                    print(f'Table.{k} Row.{l} Cell{m} Para.{i} : ', para.text, sep='')
-                    # for j, run in enumerate(para.runs):
-                    #     print(f'Para.{i} Run{j}: ', run.text, sep='')
-
-
-def replace_header(doc, prj):
-    check_replace(doc.sections[0].header.paragraphs, '.*公司', prj.com_name)
-
-
-def first_table(doc, prj):
-    match = 0
-    if doc.tables[0].rows[0].cells[0].paragraphs[0].text == '项目名称：':
-        doc.tables[0].rows[0].cells[1].paragraphs[0].runs[0].text = prj.p_name
-        clear_runs(doc.tables[0].rows[0].cells[1].paragraphs[0].runs)
-        match = match + 1
-    if doc.tables[0].rows[1].cells[0].paragraphs[0].text == '项目编号：':
-        doc.tables[0].rows[1].cells[1].paragraphs[0].runs[0].text = prj.p_start[0:4] + 'RD' + prj.p_order
-        clear_runs(doc.tables[0].rows[1].cells[1].paragraphs[0].runs)
-        match = match + 1
-    if doc.tables[0].rows[2].cells[0].paragraphs[0].text == '项目负责人：' and prj.p_owner != 'None':
-        doc.tables[0].rows[2].cells[1].paragraphs[0].runs[0].text = prj.p_owner
-        clear_runs(doc.tables[0].rows[2].cells[1].paragraphs[0].runs)
-        match = match + 1
-    if doc.tables[0].rows[3].cells[0].paragraphs[0].text == '项目周期：':
-        doc.tables[0].rows[3].cells[1].paragraphs[0].runs[0].text = prj.p_start + '至' + prj.p_end
-        clear_runs(doc.tables[0].rows[3].cells[1].paragraphs[0].runs)
-        match = match + 1
-    return match
-
-
-def start_time(doc, prj):
-    match = check_replace(doc.paragraphs, '申请立项时间：\d{4}[-/]\d{1,2}[-/]\d{1,2}', '申请立项时间：' + prj.p_start)
-    return match
-
-
-def second_table(doc, prj):
-    match = 0
-    if doc.tables[1].rows[0].cells[0].paragraphs[0].text == '项目立项名称':
-        doc.tables[1].rows[0].cells[1].paragraphs[0].runs[0].text = prj.p_name
-        clear_runs(doc.tables[1].rows[0].cells[1].paragraphs[0].runs)
-        match = match + 1
-
-    match = match + check_replace(doc.tables[1].rows[1].cells[1].paragraphs
-                                  , '项目团队由(.*)人组成，项目实施周期为(.*)个月。'
-                                  , '项目团队由' + prj.p_people + '人组成，项目实施周期为' + prj.p_cost + '个月。')
-    match = match + check_replace(doc.tables[1].rows[6].cells[1].paragraphs
-                                  , '\d{4}[-/]\d{1,2}[-/]\d{1,2}至\d{4}[-/]\d{1,2}[-/]\d{1,2}',
-                                  prj.p_start + '至' + prj.p_end)
-    match = match + check_replace(doc.tables[1].rows[7].cells[1].paragraphs
-                                  , '项目总资金预算.*万元', '项目总资金预算' + prj.p_money + '万元')
-
-    match = match + check_replace(doc.tables[1].rows[8].cells[1].paragraphs
-                                  , '项目总人数：.*人', '项目总人数：' + prj.p_people + '人')
-    if prj.p_owner != 'None':
-        match = match + check_replace(doc.tables[1].rows[8].cells[1].paragraphs, '项目负责人：.*',
-                                      '项目负责人：' + prj.p_owner)
-    if prj.p_rnd != 'None':
-        match = match + check_replace(doc.tables[1].rows[8].cells[1].paragraphs, '研发成员：.*', '研发成员：' + prj.p_rnd)
-    match = match + check_replace(doc.tables[1].rows[9].cells[1].paragraphs, '\d{4}[-/]\d{1,2}[-/]\d{1,2}', prj.p_start)
-
-    return match
-
-
-def check_replace(paras, regex, dst):
-    match = 0
-    for i, para in enumerate(paras):
-        result = re.search(regex, para.text)
-        if result is not None:
-            if result.group() != dst:
-                print(result.group() + ' 被替换为 ' + dst)
-                para.runs[0].text = re.sub(regex, dst,
-                                           para.text)
-                clear_runs(para.runs)
-            match = match + 1
-            break  # 只替换一次就够用
-    return match
-
-
-def third_table(doc, prj):
-    match = 0
-    if doc.tables[2].rows[0].cells[0].paragraphs[0].text == '项目名称':
-        doc.tables[2].rows[0].cells[1].paragraphs[0].runs[0].text = prj.p_name
-        clear_runs(doc.tables[1].rows[0].cells[1].paragraphs[0].runs)
-        match = match + 1
-    match = match + check_replace(doc.tables[2].rows[1].cells[1].paragraphs
-                  , '\d{4}[-/]\d{1,2}[-/]\d{1,2}', prj.p_end)
-    match = match + check_replace(doc.tables[2].rows[2].cells[1].paragraphs
-                  , '\d{4}[-/]\d{1,2}[-/]\d{1,2}至\d{4}[-/]\d{1,2}[-/]\d{1,2}', prj.p_start + '至' + prj.p_end)
-
-    if prj.p_owner != 'None':
-        doc.tables[2].rows[3].cells[1].paragraphs[0].runs[0].text = prj.p_owner
-        clear_runs(doc.tables[2].rows[3].cells[1].paragraphs[0].runs)
-        match = match + 1
-    return match
-
-
-if __name__ == '__main__':
-    init(autoreset=True)
-    workdir = ''
-    workdir_change = False
-    config = ConfigParser()
-    try:
-        config.read('config.ini', encoding='UTF-8')
-        workdir = config['config']['lasting']
-    except:
-        config.add_section('config')
-        pass
-    print('上次处理文件夹: ' + Fore.RED + workdir)
-    yesno = input("直接回车继续处理。否则请输入新的路径：")
-    if yesno != '':
-        workdir_change = True
-        workdir = yesno
-        config['config']['lasting'] = yesno
-    print('开始处理文件夹: ' + workdir)
-    if not os.path.exists(workdir + '_bak'):
-        print('''
-        !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-        !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-        !!                                                           !!
-        !! 该文件夹的文件会被自动修改，强烈建议备份文件，否则可能存在数据丢失风险  !!
-        !!        备份文件夹以原名称加_bak扩展时不再提示该告警!              !!
-        !!                                                           !!
-        !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-        !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-        ''')
-    input("输入回车开始执行修改文件,或者关闭该程序")
-
-    for file_sum in os.listdir(workdir):
-        if file_sum.endswith('立项报告汇总表.xlsx') and not file_sum.startswith('~$'):
-            print(f"找到 {file_sum}, 开始处理.")
-            break
-    if not file_sum.endswith('立项报告汇总表.xlsx'):
-        print("Error: 找不到 立项报告汇总表")
-        sys.exit(-1)
-
-    wb = load_workbook(workdir + '/' + file_sum, data_only=True)
-    ws = wb.active
-    if str(ws['A1'].value).find(u'公司') != -1:
-        com_name = str(ws['A1'].value).split("公司")[0] + '公司'
-    else:
-        print("Error: 找不到 公司名")
-        sys.exit(-2)
-
-    max_row_num = ws.max_row
-    rangeCell = ws[f'A3:P{max_row_num}']
-    for r in rangeCell:
-        if r[0].value is None:
-            break
-        project = Project()
-        project.p_comname = com_name
-        project.p_order = str(r[0].value).strip().zfill(2)
-        project.p_name = str(r[1].value).strip()
-        project.p_start = r[2].value.strftime('%Y-%m-%d')
-        project.p_end = r[3].value.strftime('%Y-%m-%d')
-        project.p_cost = str(r[5].value).strip()
-        project.p_people = str(r[6].value).strip()  # 人数
-        project.p_owner = str(r[7].value).strip()  # 项目负责人
-        project.p_rnd = str(r[8].value).strip()  # 研发人员
-        project.p_money = str(r[9].value).strip()  # 总预算
-
-        try:
-            doc_name = workdir + '/RD' + project.p_order + project.p_name + '.docx'
-            document = Document(doc_name)
-            # debug_doc(document)
-            # TODO to be fixed
-            # replace_header(document, project)
-            first_table(document, project)
-            start_time(document, project)
-            second_table(document, project)
-            third_table(document, project)
-            document.save(doc_name)
-        except PackageNotFoundError:
-            print(Fore.RED + '打开文件错误：' + doc_name)
-
-    #         document = replace_header(document, company)
-    #         document = check_and_change(document, replace_dict)
-    #         document = replace_tables(document, replace_dict)
-
-    if workdir_change:
-        with open('../../config.ini', 'w', encoding='utf-8') as file:
-            config = ConfigParser()
-            config.write(file)  # 数据写入配置文件
-    input("处理完成.")
+import os
+import re
+import sys
+from configparser import ConfigParser
+from docx import Document
+from docx.opc.exceptions import PackageNotFoundError
+from openpyxl import load_workbook
+from colorama import init, Fore
+
+
+class Project(object):
+    p_comname = ''  # 公司名称
+    p_order = ''  # 序号
+    p_name = ''  # 项目名
+    p_start = ''
+    p_end = ''
+    p_cost = ''
+    p_people = ''  # 人数
+    p_owner = ''  # 项目负责人
+    p_rnd = ''  # 研发人员
+    p_money = ''  # 总预算
+
+
+def check_and_change(doc, replace):
+    """
+    遍历word中的所有 paragraphs，在每一段中发现含有key 的内容，就替换为 value 。
+    （key 和 value 都是replace_dict中的键值对。）
+    """
+    for para in doc.paragraphs:
+        for i in range(len(para.runs)):
+            # print(">>>" + para.runs[i].text)
+            for key, value in replace.items():
+                if key in para.runs[i].text:
+                    print(key + "-->" + value)
+                    para.runs[i].text = para.runs[i].text.replace(key, value)
+    return doc
+
+
+def replace_tables(doc, replace):
+    for table in doc.tables:
+        for row in table.rows:
+            for cell in row.cells:
+                for para in cell.paragraphs:
+                    for i in range(len(para.runs)):
+                        # print(">>>" + para.runs[i].text)
+                        for key, value in replace.items():
+                            if key in para.runs[i].text:
+                                print(key + "-->" + value)
+                                para.runs[i].text = para.runs[i].text.replace(key, value)
+    return doc
+
+
+def clear_runs(runs):
+    for i, run in enumerate(runs):
+        if i > 0:
+            run.clear()
+    return runs
+
+
+def debug_doc(doc):
+    for i, sect in enumerate(doc.sections):
+        for j, para in enumerate(sect.header.paragraphs):
+            print(f'Sec.{i} Para.{j} : ', para.text, sep='')
+            for k, run in enumerate(para.runs):
+                print(f'Sec.{i} Para.{j} Run{k}: ', run.text, sep='')
+    for i, para in enumerate(doc.paragraphs):
+        print(f'Para.{i} : ', para.text, sep='')
+        for j, run in enumerate(para.runs):
+            print(f'Para.{i} Run{j}: ', run.text, sep='')
+    for k, table in enumerate(doc.tables):
+        for l, row in enumerate(table.rows):
+            for m, cell in enumerate(row.cells):
+                for i, para in enumerate(cell.paragraphs):
+                    print(f'Table.{k} Row.{l} Cell{m} Para.{i} : ', para.text, sep='')
+                    # for j, run in enumerate(para.runs):
+                    #     print(f'Para.{i} Run{j}: ', run.text, sep='')
+
+
+def replace_header(doc, prj):
+    check_replace(doc.sections[0].header.paragraphs, '.*公司', prj.com_name)
+
+
+def first_table(doc, prj):
+    match = 0
+    if doc.tables[0].rows[0].cells[0].paragraphs[0].text == '项目名称：':
+        doc.tables[0].rows[0].cells[1].paragraphs[0].runs[0].text = prj.p_name
+        clear_runs(doc.tables[0].rows[0].cells[1].paragraphs[0].runs)
+        match = match + 1
+    if doc.tables[0].rows[1].cells[0].paragraphs[0].text == '项目编号：':
+        doc.tables[0].rows[1].cells[1].paragraphs[0].runs[0].text = prj.p_start[0:4] + 'RD' + prj.p_order
+        clear_runs(doc.tables[0].rows[1].cells[1].paragraphs[0].runs)
+        match = match + 1
+    if doc.tables[0].rows[2].cells[0].paragraphs[0].text == '项目负责人：' and prj.p_owner != 'None':
+        doc.tables[0].rows[2].cells[1].paragraphs[0].runs[0].text = prj.p_owner
+        clear_runs(doc.tables[0].rows[2].cells[1].paragraphs[0].runs)
+        match = match + 1
+    if doc.tables[0].rows[3].cells[0].paragraphs[0].text == '项目周期：':
+        doc.tables[0].rows[3].cells[1].paragraphs[0].runs[0].text = prj.p_start + '至' + prj.p_end
+        clear_runs(doc.tables[0].rows[3].cells[1].paragraphs[0].runs)
+        match = match + 1
+    return match
+
+
+def start_time(doc, prj):
+    match = check_replace(doc.paragraphs, '申请立项时间：\d{4}[-/]\d{1,2}[-/]\d{1,2}', '申请立项时间：' + prj.p_start)
+    return match
+
+
+def second_table(doc, prj):
+    match = 0
+    if doc.tables[1].rows[0].cells[0].paragraphs[0].text == '项目立项名称':
+        doc.tables[1].rows[0].cells[1].paragraphs[0].runs[0].text = prj.p_name
+        clear_runs(doc.tables[1].rows[0].cells[1].paragraphs[0].runs)
+        match = match + 1
+
+    match = match + check_replace(doc.tables[1].rows[1].cells[1].paragraphs
+                                  , '项目团队由(.*)人组成，项目实施周期为(.*)个月。'
+                                  , '项目团队由' + prj.p_people + '人组成，项目实施周期为' + prj.p_cost + '个月。')
+    match = match + check_replace(doc.tables[1].rows[6].cells[1].paragraphs
+                                  , '\d{4}[-/]\d{1,2}[-/]\d{1,2}至\d{4}[-/]\d{1,2}[-/]\d{1,2}',
+                                  prj.p_start + '至' + prj.p_end)
+    match = match + check_replace(doc.tables[1].rows[7].cells[1].paragraphs
+                                  , '项目总资金预算.*万元', '项目总资金预算' + prj.p_money + '万元')
+
+    match = match + check_replace(doc.tables[1].rows[8].cells[1].paragraphs
+                                  , '项目总人数：.*人', '项目总人数：' + prj.p_people + '人')
+    if prj.p_owner != 'None':
+        match = match + check_replace(doc.tables[1].rows[8].cells[1].paragraphs, '项目负责人：.*',
+                                      '项目负责人：' + prj.p_owner)
+    if prj.p_rnd != 'None':
+        match = match + check_replace(doc.tables[1].rows[8].cells[1].paragraphs, '研发成员：.*', '研发成员：' + prj.p_rnd)
+    match = match + check_replace(doc.tables[1].rows[9].cells[1].paragraphs, '\d{4}[-/]\d{1,2}[-/]\d{1,2}', prj.p_start)
+
+    return match
+
+
+def check_replace(paras, regex, dst):
+    match = 0
+    for i, para in enumerate(paras):
+        result = re.search(regex, para.text)
+        if result is not None:
+            if result.group() != dst:
+                print(result.group() + ' 被替换为 ' + dst)
+                para.runs[0].text = re.sub(regex, dst,
+                                           para.text)
+                clear_runs(para.runs)
+            match = match + 1
+            break  # 只替换一次就够用
+    return match
+
+
+def third_table(doc, prj):
+    match = 0
+    if doc.tables[2].rows[0].cells[0].paragraphs[0].text == '项目名称':
+        doc.tables[2].rows[0].cells[1].paragraphs[0].runs[0].text = prj.p_name
+        clear_runs(doc.tables[1].rows[0].cells[1].paragraphs[0].runs)
+        match = match + 1
+    match = match + check_replace(doc.tables[2].rows[1].cells[1].paragraphs
+                  , '\d{4}[-/]\d{1,2}[-/]\d{1,2}', prj.p_end)
+    match = match + check_replace(doc.tables[2].rows[2].cells[1].paragraphs
+                  , '\d{4}[-/]\d{1,2}[-/]\d{1,2}至\d{4}[-/]\d{1,2}[-/]\d{1,2}', prj.p_start + '至' + prj.p_end)
+
+    if prj.p_owner != 'None':
+        doc.tables[2].rows[3].cells[1].paragraphs[0].runs[0].text = prj.p_owner
+        clear_runs(doc.tables[2].rows[3].cells[1].paragraphs[0].runs)
+        match = match + 1
+    return match
+
+
+if __name__ == '__main__':
+    init(autoreset=True)
+    workdir = ''
+    workdir_change = False
+    config = ConfigParser()
+    try:
+        config.read('config.ini', encoding='UTF-8')
+        workdir = config['config']['lasting']
+    except:
+        config.add_section('config')
+        pass
+    print('上次处理文件夹: ' + Fore.RED + workdir)
+    yesno = input("直接回车继续处理。否则请输入新的路径：")
+    if yesno != '':
+        workdir_change = True
+        workdir = yesno
+        config['config']['lasting'] = yesno
+    print('开始处理文件夹: ' + workdir)
+    if not os.path.exists(workdir + '_bak'):
+        print('''
+        !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+        !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+        !!                                                           !!
+        !! 该文件夹的文件会被自动修改，强烈建议备份文件，否则可能存在数据丢失风险  !!
+        !!        备份文件夹以原名称加_bak扩展时不再提示该告警!              !!
+        !!                                                           !!
+        !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+        !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+        ''')
+    input("输入回车开始执行修改文件,或者关闭该程序")
+
+    for file_sum in os.listdir(workdir):
+        if file_sum.endswith('立项报告汇总表.xlsx') and not file_sum.startswith('~$'):
+            print(f"找到 {file_sum}, 开始处理.")
+            break
+    if not file_sum.endswith('立项报告汇总表.xlsx'):
+        print("Error: 找不到 立项报告汇总表")
+        sys.exit(-1)
+
+    wb = load_workbook(workdir + '/' + file_sum, data_only=True)
+    ws = wb.active
+    if str(ws['A1'].value).find(u'公司') != -1:
+        com_name = str(ws['A1'].value).split("公司")[0] + '公司'
+    else:
+        print("Error: 找不到 公司名")
+        sys.exit(-2)
+
+    max_row_num = ws.max_row
+    rangeCell = ws[f'A3:P{max_row_num}']
+    for r in rangeCell:
+        if r[0].value is None:
+            break
+        project = Project()
+        project.p_comname = com_name
+        project.p_order = str(r[0].value).strip().zfill(2)
+        project.p_name = str(r[1].value).strip()
+        project.p_start = r[2].value.strftime('%Y-%m-%d')
+        project.p_end = r[3].value.strftime('%Y-%m-%d')
+        project.p_cost = str(r[5].value).strip()
+        project.p_people = str(r[6].value).strip()  # 人数
+        project.p_owner = str(r[7].value).strip()  # 项目负责人
+        project.p_rnd = str(r[8].value).strip()  # 研发人员
+        project.p_money = str(r[9].value).strip()  # 总预算
+
+        try:
+            doc_name = workdir + '/RD' + project.p_order + project.p_name + '.docx'
+            document = Document(doc_name)
+            # debug_doc(document)
+            # TODO to be fixed
+            # replace_header(document, project)
+            first_table(document, project)
+            start_time(document, project)
+            second_table(document, project)
+            third_table(document, project)
+            document.save(doc_name)
+        except PackageNotFoundError:
+            print(Fore.RED + '打开文件错误：' + doc_name)
+
+    #         document = replace_header(document, company)
+    #         document = check_and_change(document, replace_dict)
+    #         document = replace_tables(document, replace_dict)
+
+    if workdir_change:
+        with open('../../config.ini', 'w', encoding='utf-8') as file:
+            config = ConfigParser()
+            config.write(file)  # 数据写入配置文件
+    input("处理完成.")
```

### Comparing `docrobot-1.0.2/PKG-INFO` & `docrobot-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrobot
-Version: 1.0.2
+Version: 1.0.3
 Summary: 一个文档自动化处理工具
 Project-URL: Homepage, https://github.com/icehong/docrobot
 Project-URL: Bug Tracker, https://github.com/icehong/docrobot/issues
 Author-email: Xu Hong <icehong@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```


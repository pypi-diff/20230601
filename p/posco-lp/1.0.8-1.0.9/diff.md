# Comparing `tmp/posco-lp-1.0.8.tar.gz` & `tmp/posco-lp-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posco-lp-1.0.8.tar", last modified: Thu Mar 30 01:14:40 2023, max compression
+gzip compressed data, was "posco-lp-1.0.9.tar", last modified: Thu Jun  1 05:51:30 2023, max compression
```

## Comparing `posco-lp-1.0.8.tar` & `posco-lp-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 01:14:40.097595 posco-lp-1.0.8/
--rw-rw-rw-   0        0        0       32 2023-03-15 04:39:47.000000 posco-lp-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      752 2023-03-30 01:14:40.097595 posco-lp-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-03-30 01:12:00.000000 posco-lp-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 01:14:40.088619 posco-lp-1.0.8/posco_lp.egg-info/
--rw-rw-rw-   0        0        0      752 2023-03-30 01:14:40.000000 posco-lp-1.0.8/posco_lp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-03-30 01:14:40.000000 posco-lp-1.0.8/posco_lp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 01:14:40.000000 posco-lp-1.0.8/posco_lp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-03-30 01:14:40.000000 posco-lp-1.0.8/posco_lp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-30 01:14:40.000000 posco-lp-1.0.8/posco_lp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-30 01:14:40.094605 posco-lp-1.0.8/poscolp/
--rw-rw-rw-   0        0        0    29498 2023-03-30 01:11:29.000000 posco-lp-1.0.8/poscolp/__init__.py
--rw-rw-rw-   0        0        0       21 2023-03-30 01:11:37.000000 posco-lp-1.0.8/poscolp/__version__.py
--rw-rw-rw-   0        0        0       86 2023-03-30 01:14:40.100597 posco-lp-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1035 2023-03-30 01:12:42.000000 posco-lp-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 05:51:30.577559 posco-lp-1.0.9/
+-rw-rw-rw-   0        0        0       32 2023-03-15 04:39:47.000000 posco-lp-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      752 2023-06-01 05:51:30.577559 posco-lp-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-03-30 01:12:00.000000 posco-lp-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 05:51:30.567558 posco-lp-1.0.9/posco_lp.egg-info/
+-rw-rw-rw-   0        0        0      752 2023-06-01 05:51:30.000000 posco-lp-1.0.9/posco_lp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-06-01 05:51:30.000000 posco-lp-1.0.9/posco_lp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 05:51:30.000000 posco-lp-1.0.9/posco_lp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-01 05:51:30.000000 posco-lp-1.0.9/posco_lp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-01 05:51:30.000000 posco-lp-1.0.9/posco_lp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 05:51:30.575575 posco-lp-1.0.9/poscolp/
+-rw-rw-rw-   0        0        0    29631 2023-06-01 05:48:55.000000 posco-lp-1.0.9/poscolp/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-06-01 05:49:02.000000 posco-lp-1.0.9/poscolp/__version__.py
+-rw-rw-rw-   0        0        0       86 2023-06-01 05:51:30.579561 posco-lp-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2023-06-01 05:51:08.000000 posco-lp-1.0.9/setup.py
```

### Comparing `posco-lp-1.0.8/PKG-INFO` & `posco-lp-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posco-lp
-Version: 1.0.8
+Version: 1.0.9
 Summary: POSCO Learning Platform Crawling Code Library
 Home-page: https://github.com/hrdkdh
 Author: Duhwan Kim
 Author-email: hrdkdh@naver.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hrdkdh
 Keywords: POSCO,learning platform,lp
```

### Comparing `posco-lp-1.0.8/posco_lp.egg-info/PKG-INFO` & `posco-lp-1.0.9/posco_lp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posco-lp
-Version: 1.0.8
+Version: 1.0.9
 Summary: POSCO Learning Platform Crawling Code Library
 Home-page: https://github.com/hrdkdh
 Author: Duhwan Kim
 Author-email: hrdkdh@naver.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hrdkdh
 Keywords: POSCO,learning platform,lp
```

### Comparing `posco-lp-1.0.8/poscolp/__init__.py` & `posco-lp-1.0.9/poscolp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 from datetime import datetime
 from bs4 import BeautifulSoup
 from urllib3.exceptions import InsecureRequestWarning
 
 class LP():
     def __init__(self, lp_id=None, lp_pw=None):
         """
-        2023-03-30 V1.0.8, 김두환
+        2023-06-01 V1.0.9, 김두환
 
         LP 크롤링을 위한 다양한 기능을 하나로 묶은 클래스입니다.
         2개의 생성자를 입력해(생략가능) 호출하면 LP 객체를 생성합니다.
 
         lp_id : (str) 관리자 권한이 있는 lp 아이디를 입력합니다.
         lp_pw : (str) lp 아이디에 맞는 비밀번호를 입력합니다.
 
         생성자 미입력해 호출하면 아이디와 비밀번호를 묻는 프롬프트창이 뜹니다.
 
         ※업데이트 이력
             - V1.0.8 : getSurveyAnswerList() 메소드 추가, 저장할 파일명에 확장자(xlsx) 누락 시 자동으로 확장자 입력되도록 변경
+            - V1.0.9 : getChaList() 메소드 결과에 교육지역 정보 추가
         """
         if lp_id is None or lp_pw is None:
             self.lp_id=pag.prompt("관리자 권한이 있는 LP 아이디를 입력해 주세요", "LP 아이디 입력")
             self.lp_pw=pag.prompt("LP 비밀번호를 입력해 주세요", "LP 비밀번호 입력")
         else:
             self.lp_id = lp_id
             self.lp_pw = lp_pw
@@ -277,14 +278,15 @@
                 "courseCsName" : "차수명",
                 "courseSeq" : "과정ID",
                 "courseCsSeq" : "차수ID",
                 "eduMngtDeptName" : "담당부서",
                 "managerName" : "담당자",
                 "eduStartDt" : "교육시작일",
                 "eduEndDt" : "교육종료일",
+                "eduAreaName" : "교육지역",
                 "studentCnt" : "정원",
                 "studentCntApply" : "신청",
                 "studentCntConfirm" : "확정",
                 "studentCntWait" : "대기",
                 "studentCntComplete" : "수료"
             }
             df = df[kv_dict.keys()]
```

### Comparing `posco-lp-1.0.8/setup.py` & `posco-lp-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="posco-lp", # Replace with your own username
-    version="1.0.8",
+    version="1.0.9",
     author="Duhwan Kim",
     author_email="hrdkdh@naver.com",
     description="POSCO Learning Platform Crawling Code Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hrdkdh",
     project_urls={
```


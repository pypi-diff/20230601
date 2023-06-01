# Comparing `tmp/jmcomic-2.0.1.tar.gz` & `tmp/jmcomic-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-rs7emeuk/jmcomic-2.0.1.tar", last modified: Wed May 17 15:51:44 2023, max compression
+gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-6nshgqpf/jmcomic-2.0.3.tar", last modified: Thu Jun  1 06:55:02 2023, max compression
```

## Comparing `jmcomic-2.0.1.tar` & `jmcomic-2.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:51:44.000000 jmcomic-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 15:51:34.000000 jmcomic-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-17 15:51:44.000000 jmcomic-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-17 15:51:34.000000 jmcomic-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 15:51:44.000000 jmcomic-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-17 15:51:34.000000 jmcomic-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:51:44.000000 jmcomic-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:51:44.000000 jmcomic-2.0.1/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 15:51:34.000000 jmcomic-2.0.1/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-17 15:51:34.000000 jmcomic-2.0.1/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-05-17 15:51:34.000000 jmcomic-2.0.1/src/jmcomic/jm_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-05-17 15:51:34.000000 jmcomic-2.0.1/src/jmcomic/jm_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-17 15:51:34.000000 jmcomic-2.0.1/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-05-17 15:51:34.000000 jmcomic-2.0.1/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-05-17 15:51:34.000000 jmcomic-2.0.1/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-05-17 15:51:34.000000 jmcomic-2.0.1/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:51:44.000000 jmcomic-2.0.1/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-17 15:51:44.000000 jmcomic-2.0.1/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-17 15:51:44.000000 jmcomic-2.0.1/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:51:44.000000 jmcomic-2.0.1/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-17 15:51:44.000000 jmcomic-2.0.1/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 15:51:44.000000 jmcomic-2.0.1/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:55:02.000000 jmcomic-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 06:54:50.000000 jmcomic-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-01 06:55:02.000000 jmcomic-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-01 06:54:50.000000 jmcomic-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 06:55:02.000000 jmcomic-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-01 06:54:50.000000 jmcomic-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:55:02.000000 jmcomic-2.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:55:02.000000 jmcomic-2.0.3/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 06:54:50.000000 jmcomic-2.0.3/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-01 06:54:50.000000 jmcomic-2.0.3/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-06-01 06:54:50.000000 jmcomic-2.0.3/src/jmcomic/jm_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-01 06:54:50.000000 jmcomic-2.0.3/src/jmcomic/jm_client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-01 06:54:50.000000 jmcomic-2.0.3/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-06-01 06:54:50.000000 jmcomic-2.0.3/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-06-01 06:54:50.000000 jmcomic-2.0.3/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-06-01 06:54:50.000000 jmcomic-2.0.3/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:55:02.000000 jmcomic-2.0.3/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-01 06:55:02.000000 jmcomic-2.0.3/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-01 06:55:02.000000 jmcomic-2.0.3/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 06:55:02.000000 jmcomic-2.0.3/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 06:55:02.000000 jmcomic-2.0.3/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 06:55:02.000000 jmcomic-2.0.3/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-2.0.1/LICENSE` & `jmcomic-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.1/PKG-INFO` & `jmcomic-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.0.1
+Version: 2.0.3
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-2.0.1/README.md` & `jmcomic-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.1/setup.py` & `jmcomic-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.1/src/jmcomic/api.py` & `jmcomic-2.0.3/src/jmcomic/api.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.1/src/jmcomic/jm_client_impl.py` & `jmcomic-2.0.3/src/jmcomic/jm_client_impl.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             url = self.of_api_url(url, domain)
             jm_debug('api', url)
 
         if domain_index != 0 and retry_count != 0:
             jm_debug(
                 f'请求重试',
                 ', '.join([
-                    f'次数: [{retry_count + 1}/{self.retry_times}]',
+                    f'次数: [{retry_count}/{self.retry_times}]',
                     f'域名: [{domain} ({domain_index}/{len(self.domain_list)})]',
                     f'路径: [{url}]',
                     f'参数: [{kwargs if "login" not in url else "#login_form#"}]'
                 ])
             )
 
         try:
@@ -190,64 +190,90 @@
         """
         请求禁漫网页的入口
         """
         resp = self.get(url, **kwargs)
 
         if require_200 is True and resp.status_code != 200:
             write_text('./resp.html', resp.text)
-            self.check_special_http_code(resp.status_code, url)
-            raise AssertionError(f"请求失败，"
-                                 f"响应状态码为{resp.status_code}，"
-                                 f"URL=[{resp.url}]，"
-                                 + (f"响应文本=[{resp.text}]" if len(resp.text) < 50 else
-                                    f'响应文本过长(len={len(resp.text)})，不打印')
-                                 )
+            self.check_special_http_code(resp)
+            self.raise_request_error(resp)
+
         # 检查请求是否成功
-        self.require_resp_success_else_raise(resp)
+        self.require_resp_success_else_raise(resp, url)
 
         return resp
 
+    @classmethod
+    def raise_request_error(cls, resp, msg: Optional[str] = None):
+        """
+        请求如果失败，统一由该方法抛出异常
+        """
+        if msg is None:
+            msg = f"请求失败，" \
+                  f"响应状态码为{resp.status_code}，" \
+                  f"URL=[{resp.url}]，" \
+                  + (f"响应文本=[{resp.text}]" if len(resp.text) < 200 else
+                     f'响应文本过长(len={len(resp.text)})，不打印'
+                     )
+        raise AssertionError(msg)
+
     def get_jm_image(self, img_url) -> JmImageResp:
         return JmImageResp(self.get(img_url))
 
     @classmethod
-    def require_resp_success_else_raise(cls, resp):
-        # 1. 是否 album_missing
-        resp_url = resp.url
-        if resp_url.endswith('/error/album_missing'):
-            raise AssertionError(f'请求的本子不存在！({resp_url})\n'
-                                 '原因可能为:\n'
-                                 '1. id有误，检查你的本子/章节id\n'
-                                 '2. 该漫画只对登录用户可见，请配置你的cookies\n')
+    def require_resp_success_else_raise(cls, resp, req_url):
+        # 1. 检查是否 album_missing
+        error_album_missing = '/error/album_missing'
+        if resp.url.endswith(error_album_missing) and not req_url.endswith(error_album_missing):
+            cls.raise_request_error(
+                resp,
+                f'请求的本子不存在！({req_url})\n'
+                '原因可能为:\n'
+                '1. id有误，检查你的本子/章节id\n'
+                '2. 该漫画只对登录用户可见，请配置你的cookies\n'
+            )
 
-        # 2. 是否是错误html页
-        cls.check_error_html(resp.text.strip(), resp_url)
+        # 2. 是否是特殊的内容
+        cls.check_special_text(resp)
 
     @classmethod
-    def check_error_html(cls, html: str, url=None):
-        html = html.strip()
-        error_msg = JmModuleConfig.JM_ERROR_RESPONSE_HTML.get(html, None)
-        if error_msg is None:
+    def check_special_text(cls, resp):
+        html = resp.text
+        url = resp.url
+
+        if len(html) > 500:
             return
 
-        write_text('./resp.html', html)
-        raise AssertionError(f'{error_msg}'
-                             + (f': {url}' if url is not None else ''))
+        for content, reason in JmModuleConfig.JM_ERROR_RESPONSE_TEXT.items():
+            if content not in html:
+                continue
+
+            write_text('./resp.html', html)
+            cls.raise_request_error(
+                resp,
+                f'{reason}'
+                + (f': {url}' if url is not None else '')
+            )
 
     @classmethod
-    def check_special_http_code(cls, code, url=None):
+    def check_special_http_code(cls, resp):
+        code = resp.status_code
+        url = resp.url
+
         error_msg = JmModuleConfig.JM_ERROR_STATUS_CODE.get(int(code), None)
         if error_msg is None:
             return
 
-        raise AssertionError(f"请求失败，"
-                             f"响应状态码为{code}，"
-                             f'原因为: [{error_msg}], '
-                             + (f'URL=[{url}]' if url is not None else '')
-                             )
+        cls.raise_request_error(
+            resp,
+            f"请求失败，"
+            f"响应状态码为{code}，"
+            f'原因为: [{error_msg}], '
+            + (f'URL=[{url}]' if url is not None else '')
+        )
 
 
 class JmApiClient(AbstractJmClient):
     API_SEARCH = '/search'
 
     def search_album(self, search_query: str, main_tag=0) -> JmApiResp:
         """
```

### Comparing `jmcomic-2.0.1/src/jmcomic/jm_client_interface.py` & `jmcomic-2.0.3/src/jmcomic/jm_client_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,9 +204,10 @@
         return data_original.endswith('.gif')
 
 
 class JmcomicClient(
     JmImageClient,
     JmDetailClient,
     JmUserClient,
+    Postman,
 ):
     pass
```

### Comparing `jmcomic-2.0.1/src/jmcomic/jm_config.py` & `jmcomic-2.0.3/src/jmcomic/jm_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,28 @@
     from common import format_ts
     print(f'{format_ts()}:【{topic}】{msg}')
 
 
 class JmModuleConfig:
     # 网站相关
     PROT = "https://"
-    _DOMAIN = None
+    DOMAIN = None
     JM_REDIRECT_URL = f'{PROT}jm365.xyz/3YeBdF'  # 永久網域，怕走失的小伙伴收藏起来
     JM_PUB_URL = f'{PROT}jmcomic1.bet'
     JM_CDN_IMAGE_URL_TEMPLATE = PROT + 'cdn-msp.{domain}/media/photos/{photo_id}/{index:05}{suffix}'  # index 从1开始
     JM_IMAGE_SUFFIX = ['.jpg', '.webp', '.png', '.gif']
 
     # 访问JM可能会遇到的异常网页
-    JM_ERROR_RESPONSE_HTML = {
+    JM_ERROR_RESPONSE_TEXT = {
         "Could not connect to mysql! Please check your database settings!": "禁漫服务器内部报错",
         "Restricted Access!": "禁漫拒绝你所在ip地区的访问，你可以选择: 换域名/换代理",
     }
 
     JM_ERROR_STATUS_CODE = {
+        403: 'ip地区禁止访问/爬虫被识别',
         520: '520: Web server is returning an unknown error (禁漫服务器内部报错)',
         524: '524: The origin web server timed out responding to this request. (禁漫服务器处理超时)',
     }
 
     # 图片分隔相关
     SCRAMBLE_0 = 220980
     SCRAMBLE_10 = 268850
@@ -43,33 +44,34 @@
     @classmethod
     def domain(cls, postman=None):
         """
         由于禁漫的域名经常变化，调用此方法可以获取一个当前可用的最新的域名 domain，
         并且设置把 domain 设置为禁漫模块的默认域名。
         这样一来，配置文件也不用配置域名了，一切都在运行时动态获取。
         """
-        if cls._DOMAIN is None:
+        if cls.DOMAIN is None:
             from .jm_toolkit import JmcomicText
-            cls._DOMAIN = JmcomicText.parse_to_jm_domain(cls.get_jmcomic_url(postman))
+            cls.DOMAIN = JmcomicText.parse_to_jm_domain(cls.get_jmcomic_url(postman))
 
-        return cls._DOMAIN  # jmcomic默认域名
+        return cls.DOMAIN  # jmcomic默认域名
 
     @classmethod
     def headers(cls, authority=None):
         return {
             'authority': authority or '18comic.vip',
             'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,'
                       'application/signed-exchange;v=b3;q=0.7',
             'accept-language': 'zh-CN,zh;q=0.9',
+            'referer': 'https://18comic.vip',
             'sec-ch-ua': '"Google Chrome";v="111", "Not(A:Brand";v="8", "Chromium";v="111"',
             'sec-ch-ua-mobile': '?0',
             'sec-ch-ua-platform': '"Windows"',
             'sec-fetch-dest': 'document',
             'sec-fetch-mode': 'navigate',
-            'sec-fetch-site': 'none',
+            'sec-fetch-site': 'same-origin',
             'sec-fetch-user': '?1',
             'upgrade-insecure-requests': '1',
             'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 '
                           'Safari/537.36',
         }
 
     # noinspection PyUnusedLocal
```

### Comparing `jmcomic-2.0.1/src/jmcomic/jm_entity.py` & `jmcomic-2.0.3/src/jmcomic/jm_entity.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.1/src/jmcomic/jm_option.py` & `jmcomic-2.0.3/src/jmcomic/jm_option.py`

 * *Files 4% similar despite different names*

```diff
@@ -308,28 +308,36 @@
     # 缓存
     cache_jm_client = True
     jm_client_impl_mapping: Dict[str, Type[AbstractJmClient]] = {
         'html': JmHtmlClient,
         'api': JmApiClient,
     }
 
-    def build_jm_client(self) -> JmcomicClient:
+    def build_jm_client(self, **kwargs) -> JmcomicClient:
         if self.cache_jm_client is not True:
-            return self.new_jm_client()
+            return self.new_jm_client(**kwargs)
 
         client = self.jm_client_cache
         if client is None:
-            client = self.new_jm_client()
+            client = self.new_jm_client(**kwargs)
             self.jm_client_cache = client
 
         return client
 
-    def new_jm_client(self) -> JmcomicClient:
+    def new_jm_client(self, **kwargs) -> JmcomicClient:
+        postman_conf: dict = self.client.postman.src_dict
+
+        # support overwrite meta_data
+        if len(kwargs) != 0:
+            meta_data = postman_conf.get('meta_data', {})
+            meta_data.update(kwargs)
+            postman_conf['meta_data'] = meta_data
+
         # postman
-        postman = Postmans.create(data=self.client.postman)
+        postman = Postmans.create(data=postman_conf)
 
         # domain_list
         domain_list = self.client.domain
         if len(domain_list) == 0:
             domain_list = JmModuleConfig.get_jmcomic_domain_all(postman)[:-1]
 
         # client
```

### Comparing `jmcomic-2.0.1/src/jmcomic/jm_toolkit.py` & `jmcomic-2.0.3/src/jmcomic/jm_toolkit.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.1/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-2.0.3/src/jmcomic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.0.1
+Version: 2.0.3
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```


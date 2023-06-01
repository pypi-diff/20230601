# Comparing `tmp/general_calculator_zsd-1.1.5.tar.gz` & `tmp/general_calculator_zsd-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "general_calculator_zsd-1.1.5.tar", last modified: Thu Apr 20 05:22:07 2023, max compression
+gzip compressed data, was "general_calculator_zsd-1.2.0.tar", last modified: Thu Jun  1 09:11:42 2023, max compression
```

## Comparing `general_calculator_zsd-1.1.5.tar` & `general_calculator_zsd-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 05:22:07.797138 general_calculator_zsd-1.1.5/
--rw-rw-rw-   0        0        0     1089 2022-11-17 02:56:12.000000 general_calculator_zsd-1.1.5/LICENSE
--rw-rw-rw-   0        0        0      418 2023-04-20 05:22:07.797138 general_calculator_zsd-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-03-30 02:25:01.000000 general_calculator_zsd-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 05:22:07.787098 general_calculator_zsd-1.1.5/general_calculator_zsd/
--rw-rw-rw-   0        0        0        0 2022-11-16 09:26:23.000000 general_calculator_zsd-1.1.5/general_calculator_zsd/__init__.py
--rw-rw-rw-   0        0        0    47345 2023-04-20 05:20:08.000000 general_calculator_zsd-1.1.5/general_calculator_zsd/general_calculator.py
--rw-rw-rw-   0        0        0    60050 2023-04-19 03:08:55.000000 general_calculator_zsd-1.1.5/general_calculator_zsd/mysql_transmit_data4all.py
-drwxrwxrwx   0        0        0        0 2023-04-20 05:22:07.795121 general_calculator_zsd-1.1.5/general_calculator_zsd.egg-info/
--rw-rw-rw-   0        0        0      418 2023-04-20 05:22:06.000000 general_calculator_zsd-1.1.5/general_calculator_zsd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-04-20 05:22:07.000000 general_calculator_zsd-1.1.5/general_calculator_zsd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 05:22:06.000000 general_calculator_zsd-1.1.5/general_calculator_zsd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-20 05:22:06.000000 general_calculator_zsd-1.1.5/general_calculator_zsd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 05:22:07.797138 general_calculator_zsd-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      531 2023-04-20 05:21:14.000000 general_calculator_zsd-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:11:42.354030 general_calculator_zsd-1.2.0/
+-rw-rw-rw-   0        0        0     1089 2022-11-17 02:56:12.000000 general_calculator_zsd-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      418 2023-06-01 09:11:42.338411 general_calculator_zsd-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-03-30 02:25:01.000000 general_calculator_zsd-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 09:11:42.275925 general_calculator_zsd-1.2.0/general_calculator_zsd/
+-rw-rw-rw-   0        0        0        0 2022-11-16 09:26:23.000000 general_calculator_zsd-1.2.0/general_calculator_zsd/__init__.py
+-rw-rw-rw-   0        0        0    48475 2023-06-01 05:36:17.000000 general_calculator_zsd-1.2.0/general_calculator_zsd/general_calculator.py
+-rw-rw-rw-   0        0        0    65572 2023-06-01 05:20:50.000000 general_calculator_zsd-1.2.0/general_calculator_zsd/mysql_transmit_data4all.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:11:42.338411 general_calculator_zsd-1.2.0/general_calculator_zsd.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-06-01 09:11:41.000000 general_calculator_zsd-1.2.0/general_calculator_zsd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-06-01 09:11:41.000000 general_calculator_zsd-1.2.0/general_calculator_zsd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 09:11:41.000000 general_calculator_zsd-1.2.0/general_calculator_zsd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-01 09:11:41.000000 general_calculator_zsd-1.2.0/general_calculator_zsd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 09:11:42.354030 general_calculator_zsd-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      531 2023-06-01 09:10:40.000000 general_calculator_zsd-1.2.0/setup.py
```

### Comparing `general_calculator_zsd-1.1.5/LICENSE` & `general_calculator_zsd-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `general_calculator_zsd-1.1.5/general_calculator_zsd/general_calculator.py` & `general_calculator_zsd-1.2.0/general_calculator_zsd/general_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 import re
 import requests as req
 import sys
 from selenium import webdriver
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.keys import Keys
 import pickle
-
+from textrank4zh import TextRank4Keyword
+import cpca
 
 # 读取json文件变成字典
 def read_json(json_file):
     with open(json_file, 'r', encoding='utf-8') as load_f:
         data = json.load(load_f)
     return data
 
@@ -549,15 +550,15 @@
     # 连接导入数据库
     cursor, conn = get_cursor_times(db_config[db], 10)
 
     if len(cols) > 0:
         col_sql = ','.join(cols)
     else:
         col_sql = '*'
-    sql = 'select ' + col_sql + ' from ' + tbl + ' ' + condition
+    sql = 'select ' + col_sql + ' from ' + tbl + ' tbl ' + condition
     cursor.execute(sql)
     results = cursor.fetchall()  # 用于返回多条数据
     df = pd.DataFrame(list(results))
     if len(df) == 0:
         cursor.close()
         return df
     else:
@@ -1132,40 +1133,31 @@
         else:
             country_name = None
     except:
         prov_name = word2none(name)
         country_name = name
     return prov_name, country_name
 
+# 根据输入的文本，找出其中的国家、省份及城市
+# def find_country_and_province(text):
+#     if text is None:
+#         return None, None, None
+#     # 数据处理，将繁体统一为简体
+#     
+#     elif text.lower() in ['', '其他', '其它', '地区未知', 'other']:
+#         country = province = None
+#     else:
+#         # 判断是否是英文，如果是英文，则默认是只去匹配国家；如果匹配的是中国，则再匹配一轮省份
+#         if text.replace(' ', '').encode('utf-8').isalpha():
+#         location_df = cpca.transform([text], index=0)
+#         province = location_df.loc[0, '省']
+#         if province is None:
+#             country = '海外'
+        
 
-# 修正微博用户信息user_info中的地址信息
-# def fix_prov_n_city4weibo(location):
-#     province = None
-#     city = None
-#     pc_list = location.split(" ")
-#     if len(pc_list) == 1:
-#         if pc_list[0] != '其他':
-#             province = pc_list[0]
-#             if (pc_list[0] in zhixia_list) or pc_list[0] == '海外':
-#                 province = city = pc_list[0]
-#     elif len(pc_list) == 2:
-#         if pc_list[0] in zhixia_list:
-#             province = city = pc_list[0]
-#         else:
-#             province = pc_list[0]
-#             city = pc_list[1]
-#     elif len(pc_list) > 2:
-#         print('全新命名？？？？？？')
-#     if province != '海外':
-#         city = fix_city_name(city)
-#         province = fix_province_name(province)
-#     if province == '台湾省':
-#         city = '台湾省'
-#
-#     return province, city
 
 def create_task_id(task_owner, db_config, platform):
     task_owner_str = '|'.join(task_owner)
     db = 'BA_USING'
     cursor, conn = get_cursor_times(db_config[db], 10)
     sql = 'select max(task_id) as max_id from log_task_info'
     cursor.execute(sql)
@@ -1210,15 +1202,16 @@
             brand_id = row["brand_id"]
             series_id = row["series_id"]
             series_keyword = row[col_word].split('、')
             dict_out[str(account_id)]["car_list"][str(series_id)] = {"series_keyword": series_keyword}
         dict_out[str(account_id)]["brand_id"] = brand_id
     return dict_out
 
-sp_list = {'车险销售': ['车险', '汽车保险'], '车品销售': ['车品', '内饰', '汽车用品', '车辆用品'], '车膜销售': ['车膜', '贴膜', '车衣'], '轮毂销售': ['轮毂'], '二手车车商': ['二手车']}
+sp_list = {'车险销售': ['车险', '汽车保险'], '车品销售': ['车品', '内饰', '汽车用品', '车辆用品'], '车膜销售': ['车膜', '贴膜', '车衣'],
+           '轮毂销售': ['轮毂'], '二手车车商': ['二手车']}
 def speacial_identify_summmary(text):
     if (type(text) is not str) or text == '':
         return None, None
     for i in list(sp_list.keys()):
         for keyword in sp_list[i]:
             if keyword in text:
                 return keyword, i
@@ -1231,14 +1224,18 @@
 def find_emotion_by_api(TEXT):
     # 接口地址
     url = "http://ltpapi.xfyun.cn/v2/sa"
     # 开放平台应用ID
     x_appid = "d98c93ce"
     # 开放平台应用接口秘钥
     api_key = "9ed34088080000bf82286f25f6702a36"
+    # # 开放平台应用ID
+    # x_appid = "f74adea1"
+    # # 开放平台应用接口秘钥
+    # api_key = "6bfb1da8c4ad2b0cbf28a0c829228db7"
     body = urllib.parse.urlencode({'text': TEXT}).encode('utf-8')
     param = {"type": "dependent"}
     x_param = base64.b64encode(json.dumps(param).replace(' ', '').encode('utf-8'))
     x_time = str(int(time.time()))
     x_checksum = hashlib.md5(api_key.encode('utf-8') + str(x_time).encode('utf-8') + x_param).hexdigest()
     x_header = {'X-Appid': x_appid,
                 'X-CurTime': x_time,
@@ -1272,15 +1269,15 @@
             next_idx = idx + 1
             if not content[next_idx] in end_flag:
                 sentences.append(tmp_char)
                 tmp_char = ''
     return sentences
 
 def calculate_emotion_score(text):
-    if text == '' or (text.__contains__('互赞|回赞|已赞|求赞') and len(text) <= 15):
+    if text.replace(' ', '') == '' or (text.__contains__('互赞|回赞|已赞|求赞') and len(text) <= 15):
         final_sen = 0.50
     else:
         try:
             res = find_emotion_by_api(text)
             res = json.loads(res)
             if res['code'] != "0":
                 text_list = cut_sentences(text)
@@ -1311,8 +1308,38 @@
             final_sen = 0.5
     if final_sen < emo_neg:
         emo_pn = -1
     elif final_sen > emo_pos:
         emo_pn = 1
     else:
         emo_pn = 0
-    return final_sen, emo_pn
+    return final_sen, emo_pn
+
+emo_pos_paddle = 0.8
+emo_neg_paddle = 0.2
+def calculate_emotion_score_by_paddle(text, model):
+    if text.replace(' ', '') == '' or (text.__contains__('互赞|回赞|已赞|求赞') and len(text) <= 15):
+        final_sen_neg = final_sen_pos = 0.50
+    else:
+        try:
+            text_list = [text]
+            text_dict = {'text': text_list}
+            results = model.sentiment_classify(data=text_dict)
+            result = results[0]
+            final_sen_neg = result['negative_probs']
+            final_sen_pos = result['positive_probs']
+        except Exception as e:
+            final_sen_neg = final_sen_pos = 0.5
+    final_sen = final_sen_pos
+    if final_sen < emo_neg_paddle:
+        emo_pn = -1
+    elif final_sen > emo_pos_paddle:
+        emo_pn = 1
+    else:
+        emo_pn = 0
+    return final_sen, emo_pn
+
+def keywords_extraction(text, keyword_cnt):
+    tr4w = TextRank4Keyword()
+    tr4w.analyze(text=text, lower=True)
+    keywords = tr4w.get_keywords(num=keyword_cnt, word_min_len=1)
+    return keywords
```

### Comparing `general_calculator_zsd-1.1.5/general_calculator_zsd/mysql_transmit_data4all.py` & `general_calculator_zsd-1.2.0/general_calculator_zsd/mysql_transmit_data4all.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,55 +6,28 @@
 import numpy as np
 from tqdm import tqdm
 import jieba
 import time
 import datetime
 import re
 import warnings
+from bs4 import BeautifulSoup
+import general_calculator_zsd.general_calculator as gc
+global true, false, null
+false = False
+true = True
+null = ''
 
 warnings.filterwarnings("ignore")
 # 如果数据库改了，就要修改这里
 ip_database = {"localhost": "wom_db_local", "BA_USING": "BA_USING", "BI_READ": "bi"}  # 需修改本地数据库名
 dic_connet = {"localhost": {'host': 'localhost', 'port': 3306, 'user': 'root', 'password': 'zwp650811', 'database': 'wom_db_local'},
               "BA_USING": {'host': '10.26.241.164', 'port': 3306, 'user': 'BA_USING', 'password': 'BA_USING@2022', 'database': ip_database["BA_USING"]},
               "BI_READ": {'host': '10.26.241.164', 'port': 3306, 'user': 'BI_READ', 'password': 'Bireader@1027', 'database': ip_database["BI_READ"]}}
 
-# insert_table与select_table对应关系
-insert_map = {
-    'autohome_wenzhang_post': 'etl_post',
-    'autohome_luntan_post': 'etl_post',
-    'autohome_koubei_post': 'etl_post',
-    'autohome_wenzhang_comment': 'etl_comment',
-    'autohome_luntan_comment': 'etl_comment',
-    'autohome_koubei_comment': 'etl_comment',
-    'autohome_user_info': 'etl_user',
-    'dongchedi_wenzhang_post': 'etl_post',
-    'dongchedi_cheyouquan_post': 'etl_post',
-    'dongchedi_koubei_post': 'etl_post',
-    'dongchedi_wenzhang_comment': 'etl_comment',
-    'dongchedi_cheyouquan_comment': 'etl_comment',
-    'dongchedi_koubei_comment': 'etl_comment',
-    'dongchedi_user_info': 'etl_user',
-    'bilibili_video_post': 'etl_post',
-    'bilibili_video_comment': 'etl_comment',
-    'bilibili_video_danmu': 'etl_comment',
-    'bilibili_user_info': 'etl_user',
-    'weibo_auth_post': 'etl_post',
-    'weibo_search_post': 'etl_post',
-    'weibo_user_info': 'etl_user',
-    'weibo_comment': 'etl_comment',
-    'xiaohongshu_search_post': 'etl_post',
-    'xiaohongshu_comment': 'etl_comment',
-    'xiaohongshu_user_info': 'etl_user',
-    'moment': 'etl_post',
-    'momentcomment': 'etl_comment',
-    'user_base': 'etl_user',
-    'smart_tucaoba_comment': 'etl_comment'
-}
-
 insert_map_detail = {
     'weibo_auth_post': ['etl_post', 'id', 100, 'BA_USING'],
     'weibo_search_post': ['etl_post', 'id', 100, 'BA_USING'],
     'weibo_user_info': ['etl_user', 'user_id', 100, 'BA_USING'],
     'weibo_comment': ['etl_comment', 'comment_id', 100, 'BA_USING'],
     'autohome_wenzhang_post': ['etl_post', 'wenzhang_id', 200, 'BA_USING'],
     'autohome_luntan_post': ['etl_post', 'tiezi_id', 200, 'BA_USING'],
@@ -69,33 +42,63 @@
     'bilibili_user_info': ['etl_user', 'user_id', 300, 'BA_USING'],
     'xiaohongshu_search_post': ['etl_post', 'note_id', 400, 'BA_USING'],
     'xiaohongshu_comment': ['etl_comment', 'comment_id', 400, 'BA_USING'],
     'xiaohongshu_user_info': ['etl_user', 'user_id', 400, 'BA_USING'],
     'moment': ['etl_post', 'id', 500, 'BA_USING'],
     'momentcomment': ['etl_comment', 'id', 500, 'BA_USING'],
     'user_base': ['etl_user', 'user_id', 500, 'BI_READ'],
-    'smart_tucaoba_comment': ['etl_comment', 'comment_id', 500, 'BA_USING']
+    'smart_tucaoba_comment': ['etl_comment', 'comment_id', 500, 'BA_USING'],
     'dongchedi_wenzhang_post': ['etl_post', 'wenzhang_id', 600, 'BA_USING'],
     'dongchedi_cheyouquan_post': ['etl_post', 'post_id', 600, 'BA_USING'],
     'dongchedi_koubei_post': ['etl_post', 'post_id', 600, 'BA_USING'],
     'dongchedi_wenzhang_comment': ['etl_comment', 'comment_id', 600, 'BA_USING'],
     'dongchedi_cheyouquan_comment': ['etl_comment', 'comment_id', 600, 'BA_USING'],
     'dongchedi_koubei_comment': ['etl_comment', 'comment_id', 600, 'BA_USING'],
     'dongchedi_user_info': ['etl_user', 'user_id', 600, 'BA_USING'],
+    'xinchuxing_community_post': ['etl_post', 'post_id', 700, 'BA_USING'],
+    'xinchuxing_comment': ['etl_comment', 'comment_id', 700, 'BA_USING'],
+    'xinchuxing_user_info': ['etl_user', 'user_id', 700, 'BA_USING'],
+    '42hao_community_post': ['etl_post', 'post_id', 800, 'BA_USING'],
+    '42hao_comment': ['etl_comment', 'comment_id', 800, 'BA_USING'],
+    '42hao_user_info': ['etl_user', 'user_id', 800, 'BA_USING']
 }
 
 # insert_table与select_table对应关系
 post_list = ['autohome_wenzhang_post', 'autohome_luntan_post', 'autohome_koubei_post','dongchedi_wenzhang_post',
              'dongchedi_cheyouquan_post', 'dongchedi_koubei_post', 'bilibili_video_post',
-             'weibo_auth_post', 'weibo_search_post', 'xiaohongshu_search_post', 'moment']
+             'weibo_auth_post', 'weibo_search_post', 'xiaohongshu_search_post', 'moment', 'xinchuxing_community_post',
+             '42hao_community_post']
 cmt_list = ['autohome_wenzhang_comment', 'autohome_luntan_comment', 'autohome_koubei_comment',
             'dongchedi_wenzhang_comment', 'dongchedi_cheyouquan_comment', 'dongchedi_koubei_comment',
             'bilibili_video_comment','bilibili_video_danmu', 'weibo_comment', 'xiaohongshu_comment',
-            'momentcomment', 'smart_tucaoba_comment']
-user_list = ['autohome_user_info', 'dongchedi_user_info', 'weibo_user_info', 'xiaohongshu_user_info', 'bilibili_user_info', 'user_base']
+            'momentcomment', 'smart_tucaoba_comment', 'xinchuxing_comment', '42hao_comment']
+user_list = ['autohome_user_info', 'dongchedi_user_info', 'weibo_user_info', 'xiaohongshu_user_info', 
+             'bilibili_user_info', 'user_base', 'xinchuxing_user_info', '42hao_user_info']
+
+hobby_eng2chn = {
+    'cheyouhui': '车友会',
+    'finance': '金融',
+    'play_car': '玩车',
+    'parenting': '亲子',
+    'read': '读书',
+    'photography': '摄影',
+    'home_furnishing': '家居',
+    'cute_pet': '萌宠',
+    'delicious_food': '美食',
+    'movie': '影视',
+    'create_together': '共创',
+    'protection': '环保',
+    'sports_fitness': '运动健身',
+    'fashion_beauty': '时尚美妆',
+    'art_design': '艺术设计',
+    'e_sports': '游戏电竞',
+    'technology': '科技数码',
+    'travel': '旅行',
+    'listen_music': '音乐'
+}
 
 def get_datetime_now():
     return datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
 
 def combine_text(df):
     data_list = df.tolist()
     return '\n'.join(i for i in data_list if i is not None)
@@ -117,97 +120,39 @@
                  'comment_count','spider_datetime','brand_id','series_id', 'post_id', 'post_type']]
         df_after = pd.concat([df_before, df_tmp], axis=0, join='inner').reset_index()
     else:
         df_after = pd.DataFrame()
 
     return df_after
 
-def select_sql_json_bak(select_ip, select_table, start_datetime):  # sql 执行数据库语句，预计将删除
-    if select_table == 'moment':
-        select_sql = """
-            select * from {table} 
-            where createtime > '{create_datetime}'
-            and id not in (
-                select post_id from etl_post 
-                where platform_id >=500 and platform_id < 600
-                and post_datetime  > '2022-04-25');
-            """.format(table=select_table, create_datetime=start_datetime)
-    elif select_table == 'momentcomment':
-        select_sql = """
-            select mc.id id , mc.momentid momentid, mc.createtime createtime, mc.content content, mc.root root, 
-            mc.rootid rootid, mc.createdby createdby, m.source from {table} mc
-            left join moment m on m.id=mc.momentid where mc.createtime > '{create_datetime}';
-            """.format(table=select_table, create_datetime=start_datetime)
-
-    elif select_table == 'bilibili_video_comment':
-        select_sql = """
-            select c.*, p.video_id from {table} c
-            left join bilibili_video_post p on c.vid=p.video_bvid where c.spider_datetime >'{time}'
-            order by time desc
-            """.format(table=select_table, time=start_datetime)
-    elif select_table == 'user_base':
-        select_sql = """
-                select u.user_id as user_id, u.nick_name as user_nickname, u.sex as user_gender, u.province_name as user_province,
-                u.city_name as user_city, u.birthday as user_birth_date, u.signature as user_summary, u.badges as verified_reason,
-                u.role as user_label, DATE_FORMAT(u.create_time,'%Y-%m-%d') as register_date
-                from bi.{table} u
-                LEFT JOIN bi.member_info mi on u.user_id=mi.smart_id
-                LEFT JOIN bi.member_integral_info m2 on mi.id=m2.member_id
-                where (m2.points_status='enable' or m2.points_status is null)
-                and left(user_id,4) != '9999'
-                and date_format(u.create_time,'%Y-%m-%d') < current_date
-                and update_time > '{create_datetime}';
-                """.format(table=select_table, create_datetime=start_datetime)
-    else:
-        select_sql = """
-        select * from {table} where spider_datetime>'{time}';
-        """.format(table=select_table, time=start_datetime)
-    lst = []
-    try:  # 调用函数建立连接
-        conn = pymysql.connect(host=dic_connet[select_ip]['host'], port=dic_connet[select_ip]['port'],
-                               user=dic_connet[select_ip]['user'], password=dic_connet[select_ip]['password'],
-                               db=dic_connet[select_ip]['database'])
-        df = pd.read_sql(select_sql, conn)  # DataFrame转为ndarray
-        if select_table == "autohome_koubei_post":
-            df = fix_koubei_post(df)
-        df1 = np.array(df)  # 获取列名
-        column_list = list(df.columns)
-        for row in df1:  # 循环每一行数据，组装成一个字典，然后得到字典的列表
-            lst.append(dict(zip(column_list, list(row))))
-        conn.close() # 关闭数据库连接
-    except Exception as ex:
-        print(ex)
-    return lst
-
 def select_sql_json(select_ip, select_table, start_datetime, end_datetime):  # sql 执行数据库语句
     if select_table == 'moment':
         select_sql = """
             select * from {table} 
             where createtime >= '{start_datetime}' and createtime < '{end_datetime}';
             """.format(table=select_table, start_datetime=start_datetime, end_datetime=end_datetime)
     elif select_table == 'momentcomment':
         select_sql = """
             select mc.id id , mc.momentid momentid, mc.createtime createtime, mc.content content, mc.root root, 
             mc.rootid rootid, mc.createdby createdby, mc.commentscount commentscount, m.source from {table} mc
             left join moment m on m.id=mc.momentid where mc.createtime >= '{start_datetime}' 
             and mc.createtime < '{end_datetime}';
             """.format(table=select_table, start_datetime=start_datetime, end_datetime=end_datetime)
-
     elif select_table == 'bilibili_video_comment':
         select_sql = """
             select c.*, p.video_id from {table} c
             left join bilibili_video_post p on c.vid=p.video_bvid where c.spider_datetime >='{start_datetime}'
             and c.spider_datetime < '{end_datetime}'
             order by time desc
             """.format(table=select_table, start_datetime=start_datetime, end_datetime=end_datetime)
     elif select_table == 'user_base':
         select_sql = """
                 select u.user_id as user_id, u.nick_name as user_nickname, u.sex as user_gender, u.province_name as user_province,
                 u.city_name as user_city, u.birthday as user_birth_date, u.signature as user_summary, u.badges as verified_reason,
-                u.role as user_label, DATE_FORMAT(u.create_time,'%Y-%m-%d') as register_date
+                u.role as user_label, DATE_FORMAT(u.create_time,'%Y-%m-%d') as register_date, u.hobby as user_interests
                 from bi.{table} u
                 LEFT JOIN bi.member_info mi on u.user_id=mi.smart_id
                 LEFT JOIN bi.member_integral_info m2 on mi.id=m2.member_id
                 where (m2.points_status='enable' or m2.points_status is null)
                 and left(user_id,4) != '9999'
                 and date_format(u.create_time,'%Y-%m-%d') < current_date
                 and update_time >= '{start_datetime}' and update_time < '{end_datetime}';
@@ -258,15 +203,15 @@
                 left join bilibili_video_post p on c.vid=p.video_bvid where {select_key} not in 
                 (select {goal_key} from {goal_table} where platform_id >={plat_low} and platform_id < {plat_high});
                 """
     elif select_table == 'user_base':
         select_sql = f"""
                 select u.user_id as user_id, u.nick_name as user_nickname, u.sex as user_gender, u.province_name as user_province,
                 u.city_name as user_city, u.birthday as user_birth_date, u.signature as user_summary, u.badges as verified_reason,
-                u.role as user_label, DATE_FORMAT(u.create_time,'%Y-%m-%d') as register_date
+                u.role as user_label, DATE_FORMAT(u.create_time,'%Y-%m-%d') as register_date, u.hobby as user_interests
                 from bi.{select_table} u
                 LEFT JOIN bi.member_info mi on u.user_id=mi.smart_id
                 LEFT JOIN bi.member_integral_info m2 on mi.id=m2.member_id
                 where (m2.points_status='enable' or m2.points_status is null)
                 and left(user_id,4) != '9999'
                 and date_format(u.create_time,'%Y-%m-%d') < current_date
                 and {select_key} not in (select {goal_key} from ba_using.{goal_table} where media_id >={plat_low} 
@@ -329,14 +274,34 @@
         ls = eval((value))
         res = []
         for item in ls:
             hashtag = item["subject"]
             res.append(hashtag)
         result = ",".join(i for i in res)
         return result
+    else:
+        return None
+    
+def get_content4moment(content_data):
+    if content_data is not None:
+        ls = eval(content_data)
+        word_list = []
+        img_list = []
+        for content_dict in ls:
+            if content_dict['type'] == 'txt':
+                soup = BeautifulSoup(content_dict['data'], 'lxml')
+                if soup.text != '':
+                    word_list.append(soup.text)
+            elif content_dict['type'] == 'img':
+                img_list.append(content_dict['data'])
+            else:
+                print('存在其他type种类!!!')
+        return '。'.join(word_list), str(img_list)
+    else:
+        return None, '[]'
 
 def get_province(value):  # 从文本中解析城市信息
     province_list = ["北京", "天津", "上海", "重庆", "河北", "山西", "辽宁", "吉林", "黑龙江", "江苏", "浙江", "安徽", "福建", "江西", "山东", "河南", "湖北", "湖南", "广东", "海南", "四川", "贵州", "云南", "陕西", "甘肃", "青海", "台湾", "内蒙古", "广西", "西藏", "宁夏", "新疆", "香港", "澳门"]
     fenci = jieba.cut(value, cut_all=True)
     res = list(set(province_list) & set(fenci))
     if res:
         return res[0]
@@ -348,16 +313,30 @@
     fenci = jieba.cut(value, cut_all=True)
     res = list(set(city_list) & set(fenci))
     if res:
         return res[0]
     else:
         return None
 
+def sort_user_base_interests(text):
+    hobby_list_chn = []
+    if text is not None:
+        hobby_list_eng = eval(text)
+        for hobby_eng in hobby_list_eng:
+            try:
+                hobby_list_chn.append(hobby_eng2chn[hobby_eng])
+            except:
+                print(hobby_eng)
+    hobby_str = '|'.join(hobby_list_chn)
+    if hobby_str == '':
+        hobby_str = None 
+    return hobby_str
 
-def insert_json_sql(json_data, insert_ip, insert_table, select_table, update_flag):  # sql 执行数据库语句
+
+def insert_json_sql(json_data, insert_ip, insert_table, select_table, cover_flag):  # sql 执行数据库语句
     # 连接导入数据库
     insert_conn = pymysql.connect(host=dic_connet[insert_ip]['host'], port=dic_connet[insert_ip]['port'], user=dic_connet[insert_ip]['user'], password=dic_connet[insert_ip]['password'], db=dic_connet[insert_ip]['database'])
     insert_cursor = insert_conn.cursor()
     insert_data = {}
     insert_data["upload_datetime"] = get_datetime_now()
     # 自定义部分——导入数据预处理（手动填写需要导入的字段名 及 对应的上游数据字段名）
     if select_table == 'autohome_wenzhang_comment':
@@ -462,15 +441,15 @@
         insert_data["hot_degree"] = int(json_data["read_count"]) + 72*int(json_data["comment_count"])
     elif select_table == 'autohome_koubei_post':
         insert_data["platform_id"] = json_data["platform_id"]
         insert_data["post_id"] = json_data["post_id"]
         insert_data["user_id"] = json_data["user_id"]
         insert_data["post_datetime"] = json_data["post_datetime"]
         insert_data["post_content"] = json_data["post_content"]
-        # insert_data["post_subject"] = json_data["tiezi_subject"]
+        insert_data["post_subject"] = None
         insert_data["post_type"] = json_data["post_type"]
         insert_data["like_count"] = json_data["like_count"]
         insert_data["read_count"] = json_data["read_count"]
         insert_data["comment_count"] = json_data["comment_count"]
         insert_data["spider_datetime"] = json_data["spider_datetime"]
         # insert_data["keyword"] = json_data["keyword"]
         # insert_data["account_name"] = json_data["account_name"]
@@ -496,15 +475,15 @@
         insert_data["user_post_count"] = json_data["tiezi_count"]
         insert_data["following_count"] = json_data["following_count"]
         insert_data["follower_count"] = json_data["follower_count"]
         insert_data["user_level"] = json_data["vip_level"]
         insert_data["register_date"] = json_data["register_date"]
         insert_data["spider_datetime"] = json_data["spider_datetime"]
     elif select_table == 'bilibili_video_post':
-        insert_data["platform_id"] = 300
+        insert_data["platform_id"] = 301
         insert_data["post_id"] = json_data["video_id"]
         insert_data["user_id"] = json_data["user_id"]
         insert_data["post_datetime"] = json_data["video_pubdate"]
         insert_data["post_content"] = json_data["video_summary"]
         insert_data["post_subject"] = json_data["video_title"]
         insert_data["post_hashtag"] = json_data["video_tag"]
         # insert_data["publish_province"] = ""
@@ -520,30 +499,30 @@
         insert_data["account_name"] = "搜索"
         # insert_data["brand_id"] = get_brand_id(json_data["video_summary"])
         # insert_data["series_id"] = get_series_id(json_data["video_summary"])
         insert_data["brand_id"] = json_data["brand_id"]
         insert_data["series_id"] = json_data["series_id"]
         insert_data["hot_degree"] = 2*json_data["like_count"] + 15*json_data["favorite_count"] + 10*json_data["comment_count"]
     elif select_table == 'bilibili_video_comment':
-        insert_data["platform_id"] = 300
+        insert_data["platform_id"] = 301
         insert_data["comment_id"] = json_data["rpid"]
         insert_data["user_id"] = json_data["uid"]
         insert_data["comment_datetime"] = json_data["time"]
         insert_data["comment_country"] = json_data["comment_country"]
         insert_data["comment_province"] = json_data["comment_province"]
         insert_data["comment_content"] = json_data["content"]
         insert_data["comment_like_count"] = json_data["star"]
         insert_data["comment_reply_count"] = json_data["reply"]
         insert_data["comment_main_flag"] = json_data['main_flag']
         insert_data["comment_main_id"] = json_data['main_id']
         insert_data["post_id"] = json_data["video_id"]
         insert_data["spider_datetime"] = json_data["spider_datetime"]
         insert_data["hot_degree"] = 1*int(json_data["star"]) + 6*int(json_data["reply"])
     elif select_table == 'bilibili_video_danmu':
-        insert_data["platform_id"] = 301
+        insert_data["platform_id"] = 302
         insert_data["comment_id"] = json_data["danmu_comment_id"]
         insert_data["user_id"] = json_data["user_id"]
         insert_data["comment_datetime"] = json_data["pub_datetime"]
         # insert_data["comment_province"] = ""
         insert_data["comment_content"] = json_data["danmu_content"]
         # insert_data["comment_like_count"] = json_data["star"]
         # insert_data["comment_reply_count"] = json_data["reply"]
@@ -559,15 +538,16 @@
         insert_data["spider_datetime"] = json_data["spider_datetime"]
         insert_data["user_summary"] = None
     elif select_table == 'moment':
         insert_data["platform_id"] = get_platform_id(json_data["source"])
         insert_data["post_id"] = json_data["id"]
         insert_data["user_id"] = int(json_data["createdby"].replace("CMS", "9999999999").replace("smarter_unknown", "1111111111"))
         insert_data["post_datetime"] = json_data["createtime"]
-        insert_data["post_content"] = json_data["content"]
+        insert_data["post_content"], insert_data['post_image'] = get_content4moment(json_data["contentdata"])
+        # insert_data["post_content"] = json_data["content"]
         if json_data["subject"] == '无命名':
             insert_data["post_subject"] = ''
         else:
             insert_data["post_subject"] = json_data["subject"]
         insert_data["post_hashtag"] = get_hashtag(json_data["topics"])
         # insert_data["publish_province"] = ""
         # insert_data["publish_city"] = ""
@@ -581,14 +561,16 @@
         # insert_data["keyword"] = ""
         insert_data["account_name"] = json_data["source"]
         insert_data["brand_id"] = 45
         if any(word if word in (json_data["subject"]+json_data["content"]) else False for word in ['#3', '三号', '3号', '精灵3', '精灵三']):
             insert_data["series_id"] = 7044
         elif any(word if word in (json_data["subject"]+json_data["content"]) else False for word in ['#1', '一号', '1号', '精灵1', '精灵一']):
             insert_data["series_id"] = 6369
+        else:
+            insert_data["series_id"] = 999999
         insert_data["hot_degree"] = 50*int(json_data["favoritescount"]) + 8*int(json_data["commentscount"]) + 5*int(json_data["likescount"]) + 20*int(json_data["sharecount"])
     elif select_table == 'momentcomment':
         insert_data["platform_id"] = get_platform_id(json_data["source"])
         insert_data["comment_id"] = json_data["id"]
         insert_data["user_id"] = json_data["createdby"]
         insert_data["comment_datetime"] = json_data["createtime"]
         # insert_data["comment_province"] = ""
@@ -597,15 +579,15 @@
         # insert_data["comment_reply_count"] = None
         insert_data["comment_main_flag"] = get_flag(json_data["root"])
         insert_data["comment_main_id"] = json_data["rootid"]
         insert_data["post_id"] = int(json_data["momentid"])
         insert_data["spider_datetime"] = time.strftime('%Y-%m-%d %H:%M:%S', time.localtime(time.time()))
         insert_data["hot_degree"] = int(json_data["commentscount"])
     elif select_table == 'weibo_auth_post' or select_table == 'weibo_search_post':
-        insert_data["platform_id"] = 100
+        insert_data["platform_id"] = 101
         insert_data["post_id"] = json_data["id"]
         insert_data["user_id"] = json_data["user_id"]
         insert_data["account_name"] = json_data['screen_name']
         insert_data["post_datetime"] = json_data["created_at"]
         insert_data["post_content"] = json_data["text"]
         insert_data["post_subject"] = None
         insert_data["post_hashtag"] = json_data["topics"]
@@ -622,16 +604,18 @@
         insert_data["series_id"] = json_data["series_id"]
         if "search" in select_table:
             insert_data["keyword"] = json_data["search_keyword"]
             insert_data["hot_degree"] = json_data["attitudes_count"] + 4*json_data["comments_count"]
         else:
             insert_data["keyword"] = None
             insert_data["hot_degree"] = json_data["attitudes_count"] + 8*json_data["comments_count"]
+        img_list = json_data["pics"].split(',')
+        insert_data["post_image"] = str(img_list)
     elif select_table == 'weibo_comment':
-        insert_data["platform_id"] = 100
+        insert_data["platform_id"] = 101
         insert_data["comment_id"] = json_data["comment_id"]
         insert_data["user_id"] = json_data["comment_user_id"]
         insert_data["comment_datetime"] = json_data["comment_publish_time"]
         insert_data["comment_country"] = json_data["comment_user_country"]
         insert_data["comment_province"] = json_data["comment_user_province"]
         insert_data["comment_content"] = json_data["comment_content"]
         insert_data["comment_like_count"] = json_data["comment_like_count"]
@@ -675,16 +659,18 @@
         if gender == 'M':
             insert_data["user_gender"] = '男'
         elif gender == 'F':
             insert_data["user_gender"] = '女'
         else:
             insert_data["user_gender"] = None
         insert_data["user_country"] = '中国'
-        insert_data["user_province"] = json_data["user_province"]
-        insert_data["user_city"] = json_data["user_city"]
+        if json_data["user_province"] in ['上海', '北京', '天津','重庆']:
+            insert_data["user_province"] = json_data["user_province"] + '市'
+        if json_data["user_city"] in ['上海市', '北京市', '天津市', '重庆市']:
+            insert_data["user_city"] = json_data["user_city"].replace('市', '城区')
         try:
             insert_data["user_birth_date"] = json_data["user_birth_date"].strftime('%Y-%m-%d')
         except:
             insert_data["user_birth_date"] = None
         # insert_data["user_education"] = json_data["user_education"]
         # insert_data["user_work"] = json_data["user_work"]
         insert_data["user_summary"] = json_data["user_summary"]
@@ -693,18 +679,21 @@
         insert_data["verified_reason"] = json_data["verified_reason"]
         insert_data["user_label"] = json_data["user_label"]
         # insert_data["user_post_count"] = json_data["weibo_count"]
         # insert_data["following_count"] = json_data["following_count"]
         # insert_data["follower_count"] = json_data["follower_count"]
         # insert_data["user_level"] = json_data["vip_level"]
         insert_data["register_date"] = json_data["register_date"]
+        insert_data["user_interests"] = sort_user_base_interests(json_data["user_interests"])
         insert_data["spider_datetime"] = time.strftime('%Y-%m-%d %H:%M:%S', time.localtime(time.time()))
     elif select_table == 'xiaohongshu_user_info':
         insert_data["media_id"] = 400
         insert_data["user_id"] = json_data["user_id"]
+        if str(json_data["user_id"]) == '4001002859':
+            print()
         insert_data["user_nickname"] = json_data["user_nickname"]
         if json_data['user_gender'] == '1':
             insert_data["user_gender"] = "女"
         elif json_data['user_gender'] == '0':
             insert_data["user_gender"] = "男"
         else:
             insert_data["user_gender"] = None
@@ -844,15 +833,15 @@
         insert_data["hot_degree"] = 0
     elif select_table == 'dongchedi_koubei_post':
         insert_data["platform_id"] = json_data["platform_id"]
         insert_data["post_id"] = json_data["post_id"]
         insert_data["user_id"] = json_data["user_id"]
         insert_data["post_datetime"] = json_data["post_datetime"]
         insert_data["post_content"] = json_data["post_content"]
-        # insert_data["post_subject"] = json_data["tiezi_subject"]
+        insert_data["post_subject"] = None
         # insert_data["post_type"] = json_data["post_type"]
         # insert_data["like_count"] = json_data["like_count"]
         insert_data["read_count"] = json_data["read_count"]
         insert_data["comment_count"] = json_data["comment_count"]
         insert_data["spider_datetime"] = json_data["spider_datetime"]
         # insert_data["keyword"] = json_data["keyword"]
         # insert_data["account_name"] = json_data["account_name"]
@@ -890,81 +879,192 @@
         # insert_data["user_label"] = json_data["tiezi_datetime"]
         insert_data["user_post_count"] = json_data["post_count"]
         insert_data["following_count"] = json_data["following_count"]
         insert_data["follower_count"] = json_data["follower_count"]
         insert_data["user_level"] = json_data["vip_level"]
         insert_data["register_date"] = json_data["register_date"]
         insert_data["spider_datetime"] = json_data["spider_datetime"]
+    elif select_table == 'xinchuxing_community_post':
+        insert_data["platform_id"] = json_data["platform_id"]
+        insert_data["post_id"] = json_data["post_id"]
+        insert_data["user_id"] = json_data["user_id"]
+        insert_data["post_datetime"] = json_data["post_datetime"]
+        insert_data["post_content"] = json_data["content"]
+        insert_data["post_subject"] = json_data["post_title"]
+        insert_data["read_count"] = json_data["read_count"]
+        insert_data["comment_count"] = json_data["comment_count"]
+        insert_data["spider_datetime"] = json_data["spider_datetime"]
+        insert_data["brand_id"] = json_data["brand_id"]
+        insert_data["series_id"] = json_data["series_id"]
+        insert_data["hot_degree"] = 3*json_data["comment_count"] + 4*json_data["like_count"]  # 要优化
+    elif select_table == 'xinchuxing_comment':
+        insert_data["platform_id"] = json_data["platform_id"]
+        insert_data["comment_id"] = json_data["comment_id"]
+        insert_data["user_id"] = json_data["user_id"]
+        insert_data["comment_datetime"] = json_data["comment_datetime"]
+        insert_data["comment_content"] = json_data["comment_content"]
+        insert_data["comment_main_flag"] = json_data["comment_main_flag"]
+        insert_data["comment_main_id"] = json_data["comment_main_id"]
+        insert_data["post_id"] = json_data["post_id"]
+        insert_data["comment_like_count"] = json_data["like_count"]
+        insert_data["spider_datetime"] = json_data["spider_datetime"]
+        insert_data["hot_degree"] = json_data["like_count"]
+    elif select_table == 'xinchuxing_user_info':
+        insert_data["media_id"] = json_data["platform_id"]
+        insert_data["user_id"] = json_data["user_id"]
+        insert_data["user_nickname"] = json_data["user_nickname"]
+        insert_data["user_gender"] = json_data["user_gender"]
+        insert_data["user_country"] = json_data["user_country"]
+        insert_data["user_province"] = json_data["user_province"]
+        insert_data["user_city"] = json_data["user_city"]
+        insert_data["user_summary"] = json_data['introduce']
+        insert_data["user_post_count"] = json_data["post_count"]
+        insert_data["following_count"] = json_data["following_count"]
+        insert_data["follower_count"] = json_data["follower_count"]
+        insert_data["user_level"] = json_data["vip_level"]
+        insert_data["spider_datetime"] = json_data["spider_datetime"]
+    elif select_table == '42hao_community_post':
+        insert_data["platform_id"] = json_data["platform_id"]
+        insert_data["post_id"] = json_data["post_id"]
+        insert_data["user_id"] = json_data["user_id"]
+        insert_data["post_datetime"] = json_data["post_datetime"]
+        insert_data["post_content"] = json_data["content"]
+        insert_data["post_subject"] = json_data["post_title"]
+        insert_data["post_hashtag"] = json_data["labels"]
+        insert_data["like_count"] = json_data["like_count"]
+        insert_data["comment_count"] = json_data["comment_count"]
+        insert_data["spider_datetime"] = json_data["spider_datetime"]
+        insert_data["brand_id"] = json_data["brand_id"]
+        insert_data["series_id"] = json_data["series_id"]
+        insert_data["post_image"] = json_data["pic_url"]
+        insert_data["hot_degree"] = 1*insert_data["like_count"] + 2*insert_data["comment_count"]  # 这里要修改
+    elif select_table == '42hao_comment':
+        insert_data["platform_id"] = json_data["platform_id"]
+        insert_data["comment_id"] = json_data["comment_id"]
+        insert_data["user_id"] = json_data["user_id"]
+        insert_data["comment_datetime"] = json_data["comment_datetime"]
+        insert_data["comment_content"] = json_data["comment_content"]
+        insert_data["comment_main_flag"] = json_data["comment_main_flag"]
+        insert_data["comment_main_id"] = json_data["comment_main_id"]
+        insert_data["post_id"] = json_data["post_id"]
+        insert_data["spider_datetime"] = json_data["spider_datetime"]
+        insert_data["hot_degree"] = json_data["like_count"]
+    elif select_table == '42hao_user_info':
+        insert_data["media_id"] = 800
+        insert_data["user_id"] = json_data["user_id"]
+        insert_data["user_nickname"] = json_data["user_nickname"]
+        insert_data["user_gender"] = json_data["user_gender"]
+        insert_data["user_country"] = json_data["user_country"]
+        insert_data["user_province"] = json_data["user_province"]
+        insert_data["user_city"] = json_data["user_city"]
+        insert_data["user_summary"] = json_data['introduce']
+        # insert_data["user_post_count"] = json_data["post_count"]
+        insert_data["following_count"] = json_data["following_count"]
+        insert_data["follower_count"] = json_data["follower_count"]
+        insert_data["spider_datetime"] = json_data["spider_datetime"]
+        insert_data["user_car_owned"] = json_data["author_car_info_paid"]
+        insert_data["user_car_interested"] = json_data["author_car_info_intention"]
     else:
         sys.exit()
-    # 判断用户类型
-    # if select_table in user_list:
-    #     # 检查方式1：检查昵称中是否包含某个异常类型关键词
-    #     keyword, user_type1 = gc.speacial_identify_summmary(insert_data['user_nickname'])
-    #     if user_type1:
-    #         feature_list.append('昵称中包含"{}"'.format(keyword))
-    #         type_list.append(user_type1)
-    #     # 检查方式2：检查简介中是否包含某个异常类型关键词
-    #     keyword, user_type2 = gc.speacial_identify_summmary(insert_data['user_summary'])
-    #     if user_type2 and user_type1 != user_type2:
-    #         feature_list.append('简介中包含"{}"'.format(keyword))
-    #         type_list.append(user_type2)
-    #     insert_data['user_feature'] = '|'.join(feature_list)
-    #     insert_data['user_type'] = '|'.join(type_list)
+    # 判断用户类型，抽取用户简介中的关键词
+    feature_list = []
+    type_list = []
+    if select_table in user_list:
+        # 检查方式1：检查昵称中是否包含某个异常类型关键词
+        keyword, user_type1 = gc.speacial_identify_summmary(insert_data['user_nickname'])
+        if user_type1:
+            feature_list.append('昵称中包含"{}"'.format(keyword))
+            type_list.append(user_type1)
+        # 检查方式2：检查简介中是否包含某个异常类型关键词
+        keyword, user_type2 = gc.speacial_identify_summmary(insert_data['user_summary'])
+        if user_type2 and user_type1 != user_type2:
+            feature_list.append('简介中包含"{}"'.format(keyword))
+            type_list.append(user_type2)
+        insert_data['user_feature'] = '|'.join(feature_list)
+        insert_data['user_type'] = '|'.join(type_list)
+        # 用户简介的关键词提取
+        try:
+            keyword_list = []
+            user_summary = insert_data["user_summary"]
+            keyword_out = gc.keywords_extraction(user_summary, 3)
+            for word_score in keyword_out:
+                keyword_list.append(word_score['word'])
+            insert_data['summary_keyword'] = '|'.join(keyword_list)
+        except:
+            insert_data['summary_keyword'] = ''
+    # 当前只对本品进行情感打分
+    # if select_table in post_list and insert_data["brand_id"] == 45:
+    #     text_all = ''
+    #     if (insert_data["post_content"] is not None) and insert_data["post_content"] != '':
+    #         text_all += insert_data["post_content"]
+    #     if (insert_data["post_subject"] is not None) and insert_data["post_subject"] != '':
+    #         text_all += insert_data["post_subject"]
+    #     emo_score, emo_pn = gc.calculate_emotion_score(text_all)
+    #     insert_data['emo_score_neg'] = round(1 - emo_score, 2)
+    #     insert_data['emo_score_pos'] = round(emo_score, 2)
+    #     insert_data['emo_pn'] = emo_pn
+    # # comment因为架构很难改，所以暂时是对所有的文本做情感分析，有可能造成接口调用次数超过20000
+    # if select_table in cmt_list:
+    #     text_all = ''
+    #     if (insert_data["comment_content"] is not None) and insert_data["comment_content"] != '':
+    #         text_all += insert_data["comment_content"]
+    #     emo_score, emo_pn = gc.calculate_emotion_score(text_all)
+    #     insert_data['emo_score_neg'] = round(1 - emo_score, 2)
+    #     insert_data['emo_score_pos'] = round(emo_score, 2)
+    #     insert_data['emo_pn'] = emo_pn
     # 写入数据库
     keys = ", ".join(insert_data.keys())
     values = ", ".join(['%s'] * len(insert_data.keys()))
-    if update_flag:
+    if cover_flag:
         insert_sql = '''INSERT INTO {table}({keys}) VALUES ({values}) ON DUPLICATE KEY UPDATE'''.format(table=insert_table,
                                                                                                         keys=keys,
                                                                                                         values=values)
         update = ','.join([" {key} = values({key})".format(key=key) for key in insert_data])
         insert_sql += update
         insert_cursor.execute(insert_sql, tuple(insert_data.values()))
     else:
         insert_sql = """
                     INSERT ignore INTO {table}({keys}) VALUES ({values})
                     """.format(table=insert_table, keys=keys, values=values)
         # print(insert_sql)
         insert_cursor.executemany(insert_sql, [tuple(insert_data.values())])
     insert_conn.commit()
 
-def start_sql_insert_process(select_tbl, start_dt, end_dt):
+def start_sql_insert_process(select_tbl, start_dt, end_dt, mode='all'):
     insert_tbl = insert_map_detail[select_tbl][0]
-    print(f'\n-----当前将{select_tbl}导入{insert_tbl}中-----')
-    if select_tbl == 'user_base':
-        select_ip = 'BI_READ'
-        insert_ip = 'BA_USING'
-    else:
-        select_ip = 'BA_USING'
-        insert_ip = 'BA_USING'
-    res = select_sql_json(select_ip, select_tbl, start_dt, end_dt)
+    print(f'\n-----当前将{select_tbl}导入{insert_tbl}中-----')  
+    select_ip = insert_map_detail[select_tbl][3]
+    insert_ip = 'BA_USING'
+    if mode == 'all':
+        res = select_sql_json(select_ip, select_tbl, start_dt, end_dt)
+    elif mode == 'loss':
+        res = select_sql_json4loss(select_ip, select_tbl)
     for data in tqdm(res, desc=f'当前将{select_tbl}导入{insert_tbl}中' ,ncols=100):
         for (k, v) in data.items():
             try:
                 if np.isnan(data[k]):
                     data[k] = None
             except:
                 continue
         try:
-            insert_json_sql(data, insert_ip, insert_tbl, select_tbl, update_flag=True)
+            insert_json_sql(data, insert_ip, insert_tbl, select_tbl, cover_flag=True)
         except:
             print('数据插入失败：', data)
 
-def mysql_transmit_data(select_ip, insert_ip, select_tbl, start_datetime, end_datetime, update_flag):
+def mysql_transmit_data(select_ip, insert_ip, select_tbl, start_datetime, end_datetime, cover_flag):
     insert_tbl = insert_map_detail[select_tbl][0]
     print(f'\n-----当前将{select_tbl}导入{insert_tbl}中-----')
     res = select_sql_json(select_ip, select_tbl, start_datetime, end_datetime)
     if len(res) == 0:
         print('此次数据库查询无数据...')
     else:
-        for data in tqdm(res, desc=f'当前将{select_tbl}导入{insert_tbl}中',ncols=100):
+        for data in tqdm(res, desc=f'当前将{select_tbl}导入{insert_tbl}中', ncols=100):
             for (k, v) in data.items():
                 try:
                     if np.isnan(data[k]):
                         data[k] = None
                 except:
                     continue
             try:
-                insert_json_sql(data, insert_ip, insert_tbl, select_tbl, update_flag)
+                insert_json_sql(data, insert_ip, insert_tbl, select_tbl, cover_flag)
             except:
                 print('数据插入失败：', data)
```

### Comparing `general_calculator_zsd-1.1.5/setup.py` & `general_calculator_zsd-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='general_calculator_zsd',
-    version='1.1.5',
+    version='1.2.0',
     author='colin zhang',
     author_email='zsd0830@163.com',
     description='通用脚本及数据导入脚本，不定期按需更新。',
     long_description_content_type="""text/markdown""",
     url='',
     packages=find_packages(),
     classifiers=[
```


# Comparing `tmp/mypylib-0.1.74.tar.gz` & `tmp/mypylib-0.1.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypylib-0.1.74.tar", last modified: Mon May 22 15:57:12 2023, max compression
+gzip compressed data, was "mypylib-0.1.75.tar", last modified: Thu Jun  1 05:04:55 2023, max compression
```

## Comparing `mypylib-0.1.74.tar` & `mypylib-0.1.75.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-22 15:57:12.892549 mypylib-0.1.74/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-05-22 15:57:12.892310 mypylib-0.1.74/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.74/README.md
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-22 15:57:12.890273 mypylib-0.1.74/mypylib/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.74/mypylib/MP_shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    46940 2023-05-22 15:56:47.000000 mypylib-0.1.74/mypylib/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.74/mypylib/binance_copy_bot.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.74/mypylib/binance_copy_bot_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.74/mypylib/chdbif.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.74/mypylib/crypto.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.74/mypylib/finmind.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.74/mypylib/libexcel.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    24314 2023-05-22 15:55:11.000000 mypylib-0.1.74/mypylib/mvp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.74/mypylib/mytest.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.74/mypylib/option_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.74/mypylib/shioaji_history_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.74/mypylib/shioaji_kline.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.74/mypylib/shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.74/mypylib/sjtools.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.74/mypylib/tLineNotify.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7316 2023-05-17 12:26:48.000000 mypylib-0.1.74/mypylib/ti.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-22 15:57:12.891915 mypylib-0.1.74/mypylib/tmpDevelopment/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.74/mypylib/tmpDevelopment/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.74/mypylib/tmpDevelopment/warrant_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2023-04-27 13:08:02.000000 mypylib-0.1.74/mypylib/tplaysound.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8467 2023-01-12 13:51:57.000000 mypylib-0.1.74/mypylib/tredis.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8184 2023-04-11 13:54:33.000000 mypylib-0.1.74/mypylib/warrant.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-22 15:57:12.891359 mypylib-0.1.74/mypylib.egg-info/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-05-22 15:57:12.000000 mypylib-0.1.74/mypylib.egg-info/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      654 2023-05-22 15:57:12.000000 mypylib-0.1.74/mypylib.egg-info/SOURCES.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-05-22 15:57:12.000000 mypylib-0.1.74/mypylib.egg-info/dependency_links.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-05-22 15:57:12.000000 mypylib-0.1.74/mypylib.egg-info/top_level.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-05-22 15:57:12.892668 mypylib-0.1.74/setup.cfg
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.74/setup.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-06-01 05:04:55.744047 mypylib-0.1.75/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-06-01 05:04:55.743722 mypylib-0.1.75/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.75/README.md
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-06-01 05:04:55.741049 mypylib-0.1.75/mypylib/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.75/mypylib/MP_shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    46987 2023-06-01 05:04:09.000000 mypylib-0.1.75/mypylib/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.75/mypylib/binance_copy_bot.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.75/mypylib/binance_copy_bot_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.75/mypylib/chdbif.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.75/mypylib/crypto.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.75/mypylib/finmind.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.75/mypylib/libexcel.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    24435 2023-06-01 04:56:52.000000 mypylib-0.1.75/mypylib/mvp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.75/mypylib/mytest.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.75/mypylib/option_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.75/mypylib/shioaji_history_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.75/mypylib/shioaji_kline.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.75/mypylib/shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.75/mypylib/sjtools.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.75/mypylib/tLineNotify.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7735 2023-06-01 04:56:52.000000 mypylib-0.1.75/mypylib/ti.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-06-01 05:04:55.743161 mypylib-0.1.75/mypylib/tmpDevelopment/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.75/mypylib/tmpDevelopment/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.75/mypylib/tmpDevelopment/warrant_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2023-04-27 13:08:02.000000 mypylib-0.1.75/mypylib/tplaysound.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8467 2023-01-12 13:51:57.000000 mypylib-0.1.75/mypylib/tredis.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8184 2023-04-11 13:54:33.000000 mypylib-0.1.75/mypylib/warrant.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-06-01 05:04:55.742422 mypylib-0.1.75/mypylib.egg-info/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-06-01 05:04:55.000000 mypylib-0.1.75/mypylib.egg-info/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      654 2023-06-01 05:04:55.000000 mypylib-0.1.75/mypylib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-06-01 05:04:55.000000 mypylib-0.1.75/mypylib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-06-01 05:04:55.000000 mypylib-0.1.75/mypylib.egg-info/top_level.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-06-01 05:04:55.744161 mypylib-0.1.75/setup.cfg
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.75/setup.py
```

### Comparing `mypylib-0.1.74/README.md` & `mypylib-0.1.75/README.md`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/MP_shioaji_ticks.py` & `mypylib-0.1.75/mypylib/MP_shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/__init__.py` & `mypylib-0.1.75/mypylib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import requests
 
 ssl._create_default_https_context = ssl._create_unverified_context
 from termcolor import cprint
 from inspect import currentframe
 
-__version__ = '0.1.74'
+
 
 __info__ = {
     '2022/01/04: 0.1.18 加入 __info__。',
     '2022/01/04: 0.1.18 Carey修改 MVP的部分。',
     '2022/01/05: 0.1.19 add check_place_cover 預防漲停鎖住',
     '2022/01/06: 0.1.20 add get_stock_future_data(). 用來抓取每天股票期貨資料',
     '2022/01/06: 0.1.20 add get_stock_future_snapshot(). 用來抓每天股票、股票期貨漲停、跌停價格',
@@ -62,18 +62,20 @@
     '2023/02/23: 0.1.67 get_new_warrant_list() 元富修改網站，封鎖 read_html()',
     '2023/03/15: 0.1.68 修正一些宣告',
     '2023/04/11: 0.1.69 換成shioaji 1.0 API',
     '2023/04/18: 0.1.70 Market() 增加 ask bid information',
     '2023/04/27: 0.1.71 tplaysound 減少buffer音量以免很吵',
     '2023/05/10: 0.1.72 改用shioaji API',
     '2023/05/17: 0.1.73 shioaji 1.0 改 Mmvp.py & ti.py',
-    '2023/05/22: 0.1.74 mvp() 不繼承 base class。因為shioaji升級的關係。先可以跑再說'
-
+    '2023/05/22: 0.1.74 mvp() 不繼承 base class。因為shioaji升級的關係。先可以跑再說',
+    '2023/06/01: 0.1.75 Apply Carey change',
 }
 
+__version__ = '0.1.75'
+
 request_headers = {
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
 }
 
 path_cronlog = 'cronlog'
 
 toggle_btn_off = b'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'
```

### Comparing `mypylib-0.1.74/mypylib/binance_copy_bot.py` & `mypylib-0.1.75/mypylib/binance_copy_bot.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/binance_copy_bot_test.py` & `mypylib-0.1.75/mypylib/binance_copy_bot_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/chdbif.py` & `mypylib-0.1.75/mypylib/chdbif.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/crypto.py` & `mypylib-0.1.75/mypylib/crypto.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/finmind.py` & `mypylib-0.1.75/mypylib/finmind.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/libexcel.py` & `mypylib-0.1.75/mypylib/libexcel.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/mvp.py` & `mypylib-0.1.75/mypylib/mvp.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 
 matplotlib.use('PS')
 import matplotlib.pyplot as plt
 import gc
 import plotly.express as px
 
 
-class mvp:
+class mvp(Base_Technical_Indicator):
     class w:
         stop_trading_already = 'stop trading already'
 
     def __init__(self, symbol='', date='', period_seconds=10, volume_burst=1000.0, volume_lot=1000.0, volume_moving=1000.0, yesterday_close=0.0, volume_burst_30s=1000.0, volume_lot_30s=1000.0,
                  rule=1):
         cprint(f'MVP: symbol: {symbol}, '
                f'date: {date}, '
                f'period second: {period_seconds}, '
                f'volume burst: {volume_burst}, '
                f'volume burst_30s: {volume_burst_30s}, '
                f'volume lot: {volume_lot}, '
                f'volume moving: {volume_moving}',
                'yellow')
 
-        # super().__init__(symbol, date, period_seconds=period_seconds)
+        super().__init__(symbol, date, period_seconds=period_seconds)
 
         self.symbol = symbol
 
         self.rule = rule
 
         # Percentage
         self.percentage_trigger_and_down_tolerance = 0.99
@@ -72,38 +72,38 @@
         self.mvp_tmp = {'ts': [],
                         'close': [],
                         'volume': []
                         }
 
     def period_accumulate(self, tick: Tick):
         # print(f'acc: {tick.ts} {tick.close} {tick.volume}')
-        # super().period_accumulate(tick)
+        super().period_accumulate(tick)
 
         self.mvp_tmp['ts'].append(tick.datetime)
         self.mvp_tmp['close'].append(tick.close)
         self.mvp_tmp['volume'].append(tick.volume)
         self.volume_current = sum(self.mvp_tmp['volume'])
         if self.price_open == 0:
             self.price_open = tick.close
 
     def period_calculate(self, tick: Tick):
         # print(f'cal: {tick.ts} {tick.close} {tick.volume}')
-        # super().period_calculate(tick)
+        super().period_calculate(tick)
 
         self.add_mvp_index()
 
         self.mvp_tmp['ts'].clear()
         self.mvp_tmp['close'].clear()
         self.mvp_tmp['volume'].clear()
 
     def push(self, tick: Tick):
         if self.bool_stop_trading_already:
             return
 
-        # super().push(tick)
+        super().push(tick)
 
     def check_place_cover(self, tick: Tick, price) -> bool:
         index = self.mvp_index.shape[0] - 1
         cur_mvp = self.mvp_index.iloc[index]
         pre1_mvp = self.mvp_index.iloc[index - 1]
         pre2_mvp = self.mvp_index.iloc[index - 3]
         ts = cur_mvp['ts']
@@ -156,21 +156,21 @@
     def add_mvp_index(self):
 
         if len(self.mvp_tmp['ts']) == 0:
             return
         # print(f"{self.burst_volume}, {self.lot_volume}")
         volume = sum(self.mvp_tmp['volume'])
         self.volume_previous = volume
-        close = self.mvp_tmp['close'][-1]
+        close = float(self.mvp_tmp['close'][-1])
         high = max(self.mvp_tmp['close'])
         low = min(self.mvp_tmp['close'])
         burst = 0
         lot = 0
         if self.mvp_index.shape[0] == 0:
-            close = self.mvp_tmp['close'][0]
+            close = float(self.mvp_tmp['close'][0])
             ratio = round(100 * ((close / self.price_yesterday_close) - 1), 2)
             if volume > self.volume_burst_30s:
                 if close < self.price_yesterday_close:
                     burst = -1
                 elif close > self.price_yesterday_close:
                     burst = 1
             self.mvp_index = pd.DataFrame({'ts': [self.mvp_tmp['ts'][0]],
@@ -219,16 +219,20 @@
             {'ts': [self.mvp_tmp['ts'][0]], 'volume': [volume], 'high': [high], 'low': [low], 'close': [close], 'score': [score], 'ratio': [ratio], 'mvp_ratio': [mvp_ratio], 'burst': [burst],
              'lot': [lot]})
         self.mvp_index = pd.concat([self.mvp_index, df_tmp], axis=0, ignore_index=True)
         # print(tmp_df)
 
     def check_mvp(self, bool_put: bool = True):
         index = self.mvp_index.shape[0] - 1
-        if 0 < self.price_limit_up_stop_lose <= self.mvp_index['high'].max():
-            return self.w.stop_trading_already
+        try:
+            if 0 < self.price_limit_up_stop_lose <= self.mvp_index['high'].max():
+                return self.w.stop_trading_already
+        except:
+            print(self.mvp_index)
+            exit(0)
 
         if self.volume_moving / 1000 < 1000:
             cprint(f'{int(self.volume_moving / 1000)} volume low', 'blue')
             # return True
             return self.w.stop_trading_already
 
         if index < 6:
@@ -348,15 +352,15 @@
                 return True
             if -0.1 < mvp_ratio < pre1_mvp_ratio < pre2_mvp_ratio and mvp_score < 0:
                 return False
 
         return False
 
     def draw(self, symbol, date, filename):
-        # super(mvp, self).draw(symbol, date, filename)
+        super(mvp, self).draw(symbol, date, filename)
         folder = '../png/png_test'
         if not os.path.exists(folder):
             os.makedirs(folder)
         # print(self.mvp_index)
         print(f'draw {symbol} {date}')
         # Draw of MVP
         df_ticks_10s = self.mvp_index
```

### Comparing `mypylib-0.1.74/mypylib/mytest.py` & `mypylib-0.1.75/mypylib/mytest.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/option_test.py` & `mypylib-0.1.75/mypylib/option_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/shioaji_history_ticks.py` & `mypylib-0.1.75/mypylib/shioaji_history_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/shioaji_kline.py` & `mypylib-0.1.75/mypylib/shioaji_kline.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/shioaji_ticks.py` & `mypylib-0.1.75/mypylib/shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/sjtools.py` & `mypylib-0.1.75/mypylib/sjtools.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/tLineNotify.py` & `mypylib-0.1.75/mypylib/tLineNotify.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/ti.py` & `mypylib-0.1.75/mypylib/ti.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,19 +122,24 @@
     def push(self, tick: Union[Tick, Quote]):
 
         if tick.datetime.time() < datetime.time(9, 0, 0):
             return
 
         if tick.simtrade == 1:
             return
-
-        self.price_ask = tick.ask_price[0] if tick.ask_price[0] != 0 else self.price_ask
-        self.price_bid = tick.bid_price[0] if tick.bid_price[0] != 0 else self.price_bid
-        self.volume_ask = tick.ask_volume[0] if tick.ask_volume[0] != 0 else self.volume_ask
-        self.volume_bid = tick.bid_volume[0] if tick.bid_volume[0] != 0 else self.volume_bid
+        if False:
+            self.price_ask = tick.ask_price[0] if tick.ask_price[0] != 0 else self.price_ask
+            self.price_bid = tick.bid_price[0] if tick.bid_price[0] != 0 else self.price_bid
+            self.volume_ask = tick.ask_volume[0] if tick.ask_volume[0] != 0 else self.volume_ask
+            self.volume_bid = tick.bid_volume[0] if tick.bid_volume[0] != 0 else self.volume_bid
+        else:
+            self.price_ask = tick.close if tick.close != 0 else self.price_ask
+            self.price_bid = tick.close if tick.close != 0 else self.price_bid
+            self.volume_ask = tick.ask_side_total_vol if tick.ask_side_total_vol != 0 else self.volume_ask
+            self.volume_bid = tick.bid_side_total_vol if tick.bid_side_total_vol != 0 else self.volume_bid
 
         if tick.close == 0:
             return
 
         # 第一個成交的 tick 到來的時間
         if not self.bool_start_time_determined:
             self.time_start = tick.datetime.replace(hour=9, minute=0, second=0, microsecond=0)
```

### Comparing `mypylib-0.1.74/mypylib/tmpDevelopment/warrant_test.py` & `mypylib-0.1.75/mypylib/tmpDevelopment/warrant_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/tplaysound.py` & `mypylib-0.1.75/mypylib/tplaysound.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/tredis.py` & `mypylib-0.1.75/mypylib/tredis.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib/warrant.py` & `mypylib-0.1.75/mypylib/warrant.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/mypylib.egg-info/SOURCES.txt` & `mypylib-0.1.75/mypylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.74/setup.py` & `mypylib-0.1.75/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/pysailfish-1.2.0.tar.gz` & `tmp/pysailfish-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysailfish-1.2.0.tar", max compression
+gzip compressed data, was "pysailfish-1.3.0.tar", max compression
```

## Comparing `pysailfish-1.2.0.tar` & `pysailfish-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,38 @@
--rw-r--r--   0        0        0     9184 2023-05-02 01:57:06.179743 pysailfish-1.2.0/README.md
--rw-r--r--   0        0        0      290 2023-05-02 01:57:27.595525 pysailfish-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 01:21:34.884388 pysailfish-1.2.0/pysailfish/__init__.py
--rw-r--r--   0        0        0     7671 2023-05-02 01:29:21.852922 pysailfish-1.2.0/pysailfish/app/EAs/MA_EA.py
--rw-r--r--   0        0        0     1213 2023-05-02 01:28:29.628493 pysailfish-1.2.0/pysailfish/app/EAs/MT4ClientEA.py
--rw-r--r--   0        0        0      401 2023-05-02 01:21:34.912388 pysailfish-1.2.0/pysailfish/app/Mainpage.dox
--rw-r--r--   0        0        0        0 2023-05-02 01:23:53.313928 pysailfish-1.2.0/pysailfish/app/__init__.py
--rw-r--r--   0        0        0     3368 2023-05-02 01:28:29.628493 pysailfish-1.2.0/pysailfish/app/main.py
--rw-r--r--   0        0        0     2088 2023-05-02 01:28:29.628493 pysailfish-1.2.0/pysailfish/app/test_tcp_client.py
--rw-r--r--   0        0        0     3450 2023-05-02 01:28:29.628493 pysailfish-1.2.0/pysailfish/app/test_tcp_server_client.py
--rw-r--r--   0        0        0     5805 2023-05-02 01:28:29.628493 pysailfish-1.2.0/pysailfish/internal/DataCtrl/MT4DataCtrl/MT4DataCtrl.py
--rw-r--r--   0        0        0    26775 2023-05-02 01:29:21.852922 pysailfish-1.2.0/pysailfish/internal/MT_EA/MT4_EA.py
--rw-r--r--   0        0        0     1741 2023-05-02 01:29:21.852922 pysailfish-1.2.0/pysailfish/internal/MT_EA/account_information.py
--rw-r--r--   0        0        0     1672 2023-05-02 01:29:21.852922 pysailfish-1.2.0/pysailfish/internal/MT_EA/common_functions.py
--rw-r--r--   0        0        0     4531 2023-05-02 01:29:21.852922 pysailfish-1.2.0/pysailfish/internal/MT_EA/market_info.py
--rw-r--r--   0        0        0     9675 2023-05-02 01:24:33.698340 pysailfish-1.2.0/pysailfish/internal/MT_EA/mt4_const.py
--rw-r--r--   0        0        0    10493 2023-05-02 01:24:33.698340 pysailfish-1.2.0/pysailfish/internal/MT_EA/mt4_fun_num_map.py
--rw-r--r--   0        0        0    18293 2023-05-02 01:33:23.550747 pysailfish-1.2.0/pysailfish/internal/MT_EA/object_functions.py
--rw-r--r--   0        0        0      485 2023-05-02 01:24:33.698340 pysailfish-1.2.0/pysailfish/internal/MT_EA/predefined_variables.py
--rw-r--r--   0        0        0    25760 2023-05-02 01:29:21.852922 pysailfish-1.2.0/pysailfish/internal/MT_EA/technical_indicators.py
--rw-r--r--   0        0        0    19884 2023-05-02 01:29:21.852922 pysailfish-1.2.0/pysailfish/internal/MT_EA/timeseries_and_indicators_access.py
--rw-r--r--   0        0        0     5219 2023-05-02 01:29:21.852922 pysailfish-1.2.0/pysailfish/internal/MT_EA/trade_functions.py
--rw-r--r--   0        0        0     4456 2023-05-02 01:24:33.698340 pysailfish-1.2.0/pysailfish/internal/Network/TCPCast.py
--rw-r--r--   0        0        0        0 2023-05-02 01:21:34.912388 pysailfish-1.2.0/pysailfish/internal/__init__.py
--rw-r--r--   0        0        0    10213 1970-01-01 00:00:00.000000 pysailfish-1.2.0/setup.py
--rw-r--r--   0        0        0     9665 1970-01-01 00:00:00.000000 pysailfish-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     9184 2023-05-02 01:57:06.179743 pysailfish-1.3.0/README.md
+-rw-r--r--   0        0        0      267 2023-06-01 03:58:26.515114 pysailfish-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 01:21:34.884388 pysailfish-1.3.0/pysailfish/__init__.py
+-rw-r--r--   0        0        0     7671 2023-05-02 01:29:21.852922 pysailfish-1.3.0/pysailfish/app/EAs/MA_EA.py
+-rw-r--r--   0        0        0     1213 2023-05-02 01:28:29.628493 pysailfish-1.3.0/pysailfish/app/EAs/MT4ClientEA.py
+-rw-r--r--   0        0        0      401 2023-05-02 01:21:34.912388 pysailfish-1.3.0/pysailfish/app/Mainpage.dox
+-rw-r--r--   0        0        0        0 2023-05-02 01:23:53.313928 pysailfish-1.3.0/pysailfish/app/__init__.py
+-rw-r--r--   0        0        0     3376 2023-06-01 03:56:23.982981 pysailfish-1.3.0/pysailfish/app/main.py
+-rw-r--r--   0        0        0     2097 2023-06-01 03:56:53.079013 pysailfish-1.3.0/pysailfish/app/test_tcp_client.py
+-rw-r--r--   0        0        0     3458 2023-06-01 03:57:52.851079 pysailfish-1.3.0/pysailfish/app/test_tcp_server_client.py
+-rw-r--r--   0        0        0     5822 2023-06-01 03:57:42.707068 pysailfish-1.3.0/pysailfish/internal/DataCtrl/MT4DataCtrl/MT4DataCtrl.py
+-rw-r--r--   0        0        0    26783 2023-06-01 03:57:28.483052 pysailfish-1.3.0/pysailfish/internal/MT_EA/MT4_EA.py
+-rw-r--r--   0        0        0     1741 2023-05-02 01:29:21.852922 pysailfish-1.3.0/pysailfish/internal/MT_EA/account_information.py
+-rw-r--r--   0        0        0     1672 2023-05-02 01:29:21.852922 pysailfish-1.3.0/pysailfish/internal/MT_EA/common_functions.py
+-rw-r--r--   0        0        0     4531 2023-05-02 01:29:21.852922 pysailfish-1.3.0/pysailfish/internal/MT_EA/market_info.py
+-rw-r--r--   0        0        0     9675 2023-05-02 01:24:33.698340 pysailfish-1.3.0/pysailfish/internal/MT_EA/mt4_const.py
+-rw-r--r--   0        0        0    10493 2023-05-02 01:24:33.698340 pysailfish-1.3.0/pysailfish/internal/MT_EA/mt4_fun_num_map.py
+-rw-r--r--   0        0        0    18293 2023-05-02 01:33:23.550747 pysailfish-1.3.0/pysailfish/internal/MT_EA/object_functions.py
+-rw-r--r--   0        0        0      485 2023-05-02 01:24:33.698340 pysailfish-1.3.0/pysailfish/internal/MT_EA/predefined_variables.py
+-rw-r--r--   0        0        0    25760 2023-05-02 01:29:21.852922 pysailfish-1.3.0/pysailfish/internal/MT_EA/technical_indicators.py
+-rw-r--r--   0        0        0    19884 2023-05-02 01:29:21.852922 pysailfish-1.3.0/pysailfish/internal/MT_EA/timeseries_and_indicators_access.py
+-rw-r--r--   0        0        0     5219 2023-05-02 01:29:21.852922 pysailfish-1.3.0/pysailfish/internal/MT_EA/trade_functions.py
+-rw-r--r--   0        0        0     4456 2023-05-02 01:24:33.698340 pysailfish-1.3.0/pysailfish/internal/Network/TCPCast.py
+-rw-r--r--   0        0        0        0 2023-05-02 01:21:34.912388 pysailfish-1.3.0/pysailfish/internal/__init__.py
+-rw-r--r--   0        0        0      566 2023-06-01 03:56:12.466967 pysailfish-1.3.0/pysailfish/internal/devTools/AtomicData.py
+-rw-r--r--   0        0        0     1388 2023-06-01 03:56:12.466967 pysailfish-1.3.0/pysailfish/internal/devTools/ThreadClass.py
+-rw-r--r--   0        0        0        0 2023-06-01 03:56:12.466967 pysailfish-1.3.0/pysailfish/internal/observability/__init__.py
+-rw-r--r--   0        0        0     3930 2023-06-01 03:56:12.466967 pysailfish-1.3.0/pysailfish/internal/observability/log_helper.py
+-rw-r--r--   0        0        0      145 2023-06-01 03:56:12.466967 pysailfish-1.3.0/pysailfish/internal/observability/logging_json/__init__.py
+-rw-r--r--   0        0        0     2814 2023-06-01 03:56:12.466967 pysailfish-1.3.0/pysailfish/internal/observability/logging_json/_formatter.py
+-rw-r--r--   0        0        0      372 2023-06-01 03:56:12.466967 pysailfish-1.3.0/pysailfish/internal/observability/logging_json/version.py
+-rw-r--r--   0        0        0        0 2023-06-01 03:56:12.466967 pysailfish-1.3.0/pysailfish/internal/observability/logstash/__init__.py
+-rw-r--r--   0        0        0     4792 2023-06-01 03:56:12.466967 pysailfish-1.3.0/pysailfish/internal/observability/logstash/formatter.py
+-rw-r--r--   0        0        0     4865 2023-06-01 03:56:12.466967 pysailfish-1.3.0/pysailfish/internal/observability/logstash/handler_amqp.py
+-rw-r--r--   0        0        0     1218 2023-06-01 03:56:12.466967 pysailfish-1.3.0/pysailfish/internal/observability/logstash/handler_tcp.py
+-rw-r--r--   0        0        0      891 2023-06-01 03:56:12.466967 pysailfish-1.3.0/pysailfish/internal/observability/logstash/handler_udp.py
+-rw-r--r--   0        0        0    10288 1970-01-01 00:00:00.000000 pysailfish-1.3.0/setup.py
+-rw-r--r--   0        0        0     9621 1970-01-01 00:00:00.000000 pysailfish-1.3.0/PKG-INFO
```

### Comparing `pysailfish-1.2.0/README.md` & `pysailfish-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pysailfish-1.2.0/pysailfish/app/EAs/MA_EA.py` & `pysailfish-1.3.0/pysailfish/app/EAs/MA_EA.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.2.0/pysailfish/app/EAs/MT4ClientEA.py` & `pysailfish-1.3.0/pysailfish/app/EAs/MT4ClientEA.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.2.0/pysailfish/app/main.py` & `pysailfish-1.3.0/pysailfish/app/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 
 # Imports
 import argparse
 import logging
 import threading
 import time
 
-import sfdevtools.observability.log_helper as lh
-
+import pysailfish.internal.observability.log_helper as lh
 from pysailfish.internal.Network.TCPCast import TCPCast, TCPStatus
 
 # Variables
 server_ip: str = "192.168.1.104" # "0.0.0.0"
 server_port: int = 7788
 tcp_server: TCPCast = TCPCast()
 tcp_client: TCPCast = TCPCast()
```

### Comparing `pysailfish-1.2.0/pysailfish/app/test_tcp_client.py` & `pysailfish-1.3.0/pysailfish/app/test_tcp_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 # Imports
 import argparse
 import logging
 import threading
 import time
 
-import sfdevtools.observability.log_helper as lh
 
+import pysailfish.internal.observability.log_helper as lh
 from pysailfish.internal.Network.TCPCast import TCPCast, TCPStatus
 
 # Variables
 server_ip: str = "127.0.0.1" # "0.0.0.0" --- for linux and docker "127.0.0.1" --- for windows
 server_port: int = 23456
 tcp_client: TCPCast = TCPCast()
```

### Comparing `pysailfish-1.2.0/pysailfish/app/test_tcp_server_client.py` & `pysailfish-1.3.0/pysailfish/app/test_tcp_server_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 
 # Imports
 import argparse
 import logging
 import threading
 import time
 
-import sfdevtools.observability.log_helper as lh
-
+import pysailfish.internal.observability.log_helper as lh
 from pysailfish.internal.Network.TCPCast import TCPCast, TCPStatus
 
 # Variables
 server_ip: str = "0.0.0.0" # "0.0.0.0" --- for linux and docker "127.0.0.1" --- for windows
 server_port: int = 7788
 tcp_server: TCPCast = TCPCast()
 tcp_client: TCPCast = TCPCast()
```

### Comparing `pysailfish-1.2.0/pysailfish/internal/DataCtrl/MT4DataCtrl/MT4DataCtrl.py` & `pysailfish-1.3.0/pysailfish/internal/DataCtrl/MT4DataCtrl/MT4DataCtrl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import logging
 import time
 import traceback
 from typing import List, Dict, Tuple, Union, Set, Any
 from datetime import datetime
 
-import sfdevtools.observability.log_helper as lh
-from sfdevtools.devTools.ThreadClass import ThreadClass
-
+import pysailfish.internal.observability.log_helper as lh
 from pysailfish.internal.Network.TCPCast import TCPCast, TCPStatus
+from pysailfish.internal.devTools.ThreadClass import ThreadClass
 
 class MT4DataCtrl(ThreadClass):
     def __init__(self):
         self.__logger: logging.Logger = None
         self.__tcp_client: TCPCast = None
         self.__mt4_msg_callback: Any = None
         self.__data_pool: str = ""
```

### Comparing `pysailfish-1.2.0/pysailfish/internal/MT_EA/MT4_EA.py` & `pysailfish-1.3.0/pysailfish/internal/MT_EA/MT4_EA.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Dict, List, Set, Tuple, Union, Any
 from datetime import datetime
 import logging
 import time
 import decimal
 
-import sfdevtools.observability.log_helper as lh
-
 from pysailfish.internal.DataCtrl.MT4DataCtrl.MT4DataCtrl import MT4DataCtrl
 from pysailfish.internal.Network.TCPCast import TCPCast, TCPStatus
 from pysailfish.internal.MT_EA.mt4_fun_num_map import mt4_fun_num_map
+import pysailfish.internal.observability.log_helper as lh
 import pysailfish.internal.MT_EA.predefined_variables as pv
 import pysailfish.internal.MT_EA.trade_functions as tf
 import pysailfish.internal.MT_EA.common_functions as cf
 import pysailfish.internal.MT_EA.technical_indicators as ti
 import pysailfish.internal.MT_EA.account_information as ai
 import pysailfish.internal.MT_EA.market_info as mi
 import pysailfish.internal.MT_EA.timeseries_and_indicators_access as taia
```

### Comparing `pysailfish-1.2.0/pysailfish/internal/MT_EA/account_information.py` & `pysailfish-1.3.0/pysailfish/internal/MT_EA/account_information.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.2.0/pysailfish/internal/MT_EA/common_functions.py` & `pysailfish-1.3.0/pysailfish/internal/MT_EA/common_functions.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.2.0/pysailfish/internal/MT_EA/market_info.py` & `pysailfish-1.3.0/pysailfish/internal/MT_EA/market_info.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.2.0/pysailfish/internal/MT_EA/mt4_const.py` & `pysailfish-1.3.0/pysailfish/internal/MT_EA/mt4_const.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.2.0/pysailfish/internal/MT_EA/mt4_fun_num_map.py` & `pysailfish-1.3.0/pysailfish/internal/MT_EA/mt4_fun_num_map.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.2.0/pysailfish/internal/MT_EA/object_functions.py` & `pysailfish-1.3.0/pysailfish/internal/MT_EA/object_functions.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.2.0/pysailfish/internal/MT_EA/technical_indicators.py` & `pysailfish-1.3.0/pysailfish/internal/MT_EA/technical_indicators.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.2.0/pysailfish/internal/MT_EA/timeseries_and_indicators_access.py` & `pysailfish-1.3.0/pysailfish/internal/MT_EA/timeseries_and_indicators_access.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.2.0/pysailfish/internal/MT_EA/trade_functions.py` & `pysailfish-1.3.0/pysailfish/internal/MT_EA/trade_functions.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.2.0/pysailfish/internal/Network/TCPCast.py` & `pysailfish-1.3.0/pysailfish/internal/Network/TCPCast.py`

 * *Files identical despite different names*

### Comparing `pysailfish-1.2.0/setup.py` & `pysailfish-1.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 packages = \
 ['pysailfish',
  'pysailfish.app',
  'pysailfish.app.EAs',
  'pysailfish.internal',
  'pysailfish.internal.DataCtrl.MT4DataCtrl',
  'pysailfish.internal.MT_EA',
- 'pysailfish.internal.Network']
+ 'pysailfish.internal.Network',
+ 'pysailfish.internal.devTools',
+ 'pysailfish.internal.observability',
+ 'pysailfish.internal.observability.logging_json',
+ 'pysailfish.internal.observability.logstash']
 
 package_data = \
 {'': ['*']}
 
-install_requires = \
-['sfdevtools>=1.74.0,<2.0.0']
-
 setup_kwargs = {
     'name': 'pysailfish',
-    'version': '1.2.0',
+    'version': '1.3.0',
     'description': '',
     'long_description': '\n## pysailfish\n\n### Example EA --- simple client\n```python\nfrom pysailfish.internal.MT_EA.MT4_EA import MT4_EA\n\nclass MT4DemoEA(MT4_EA):\n    def __init__(self):\n        super().__init__()\n\n    # override\n    def _OnInit(self) -> int:\n        self._logger.info(self._user_inputs)\n        self._logger.info("Here")\n        return 0\n\n    # override\n    def _OnDeinit(self, reason: int) -> None:\n        self._logger.info(f"Here reason: {reason}")\n        return None\n\n    # override\n    def _OnTick(self) -> None:\n        self._logger.info("Here")\n        return None\n\n    # override\n    def _OnTimer(self) -> None:\n        return None\n\n    # override\n    def _OnTester(self) -> float:\n        self._logger.info("Here")\n        return 0.0\n\n    # override\n    def _OnChartEvent(self\n                      , id: int\n                      , lparam: int\n                      , dparam: float\n                      , sparam: str) -> None:\n        self._logger.info(f"Here id: {id} lparam: {lparam} dparam: {dparam} sparam: {sparam}")\n        return None\n\ndef main() -> None:\n    ea = MT4DemoEA()\n    ea.InitComponent(server_ip="127.0.0.1"\n                     , server_port=23456\n                     , ea_name="MT4DemoEA")\n    ea.StartEA()\n\nif __name__ == "__main__":\n    main()\n```\n\n### Example EA --- Moving Average EA\n```python\nfrom datetime import datetime\n\nimport pysailfish.internal.MT_EA.mt4_const as mc\nfrom pysailfish.internal.MT_EA.MT4_EA import MT4_EA\n\nclass MA_EA(MT4_EA):\n    def __init__(self):\n        super().__init__()\n\n    # override\n    def _OnInit(self) -> int:\n        self._logger.info(self._user_inputs)\n        self._logger.info("Here")\n        return 0\n\n    # override\n    def _OnDeinit(self, reason: int) -> None:\n        self._logger.info(f"Here reason: {reason}")\n        return None\n\n    # override\n    def _OnTick(self) -> None:\n        vv = self.iADX(symbol=self._pv.symbol\n                       , timeframe=mc.PERIOD_CURRENT\n                       , period=self._user_inputs["MovingPeriod"]\n                       , applied_price=mc.PRICE_CLOSE\n                       , mode=mc.MODE_MAIN\n                       , shift=0)\n        # self._logger.info(f"Here {self._pv.symbol} {self._pv.time[0]}")\n        # --- check for history and trading\n        if self._pv.bars < 100 or self._pv.is_trade_allowed == False:\n            return\n\n        # --- calculate open orders by current symbol\n        if self.__calculate_current_orders(self._pv.symbol) == 0:\n            self.__check_for_open()\n        else:\n            self.__check_for_close()\n        return None\n\n    # override\n    def _OnTimer(self) -> None:\n        return None\n\n    # override\n    def _OnTester(self) -> float:\n        self._logger.info("Here")\n        return 0.0\n\n    # override\n    def _OnChartEvent(self\n                      , id: int\n                      , lparam: int\n                      , dparam: float\n                      , sparam: str) -> None:\n        self._logger.info(f"Here id: {id} lparam: {lparam} dparam: {dparam} sparam: {sparam}")\n        return None\n\n    def __check_for_close(self) -> None:\n        ma: float = 0\n        #--- go trading only for first tiks of new bar\n        if self._pv.volume[0] > 1:\n            return None\n        #--- get Moving Average\n        ma = self.iMA(symbol=self._pv.symbol\n                      , timeframe=mc.PERIOD_CURRENT\n                      , ma_period=self._user_inputs["MovingPeriod"]\n                      , ma_shift=self._user_inputs["MovingShift"]\n                      , ma_method=mc.MODE_SMA\n                      , applied_price=mc.PRICE_CLOSE\n                      , shift=0)\n        #---\n        for i in range(self.OrdersTotal()):\n            if self.OrderSelect(index=i, select=mc.SELECT_BY_POS, pool=mc.MODE_TRADES) == False:\n                break\n            if self.OrderMagicNumber() != self._pv.magic_num or self.OrderSymbol() != self._pv.symbol:\n                continue\n            #--- check order type\n            if self.OrderType() == mc.OP_BUY:\n                if self._pv.open[1] > ma and self._pv.close[1] < ma:\n                    if not self.OrderClose(ticket=self.OrderTicket(), lots=self.OrderLots(), price=self._pv.bid, slippage=3, arrow_color=mc.clrWhite):\n                        self._logger.error(f"OrderClose error {self.GetLastError()}")\n                break\n            if self.OrderType() == mc.OP_SELL:\n                if self._pv.open[1] < ma and self._pv.close[1] > ma:\n                    if not self.OrderClose(ticket=self.OrderTicket(), lots=self.OrderLots(), price=self._pv.ask, slippage=3, arrow_color=mc.clrWhite):\n                        self._logger.error(f"OrderClose error {self.GetLastError()}");\n                break\n\n    def __lots_optimized(self) -> float:\n        lot: float = float(self._user_inputs["Lots"])\n        maximum_risk: float = float(self._user_inputs["MaximumRisk"])\n        decrease_factor: float = float(self._user_inputs["DecreaseFactor"])\n        orders: int = self.OrdersHistoryTotal() # history orders total\n        losses: int = 0 # number of losses orders without a break\n        #--- select lot size\n        lot = self.NormalizeDouble(value=(self.AccountFreeMargin() * maximum_risk / 1000.0), digits=1);\n        #--- calcuulate number of losses orders without a break\n        if decrease_factor > 0:\n            for i in reversed(range(orders)):\n                if self.OrderSelect(index=i, select=mc.SELECT_BY_POS, pool=mc.MODE_HISTORY) == False:\n                    self._logger.error("Error in history")\n                    break\n                if self.OrderSymbol() != self._pv.symbol or self.OrderType() > mc.OP_SELL:\n                    continue\n                #---\n                if self.OrderProfit() > 0:\n                    break\n                if self.OrderProfit() < 0:\n                    losses += 1\n            if losses > 1:\n                lot = self.NormalizeDouble(value=(lot - lot * losses / decrease_factor), digits=1)\n        #--- return lot size\n        if lot < 0.1:\n            lot = 0.1\n        return lot\n\n    def __check_for_open(self) -> None:\n        ma: float = 0\n        res: int = 0\n        #--- go trading only for first tiks of new bar\n        if self._pv.volume[0] > 1:\n            return None\n        #--- get Moving Average\n        ma = self.iMA(symbol=self._pv.symbol\n                      , timeframe=mc.PERIOD_CURRENT\n                      , ma_period=self._user_inputs["MovingPeriod"]\n                      , ma_shift=self._user_inputs["MovingShift"]\n                      , ma_method=mc.MODE_SMA\n                      , applied_price=mc.PRICE_CLOSE\n                      , shift=0)\n        #--- sell conditions\n        if self._pv.open[1] > ma and self._pv.close[1] < ma:\n            res = self.OrderSend(symbol=self._pv.symbol\n                                 , cmd=mc.OP_SELL\n                                 , volume=self.__lots_optimized()\n                                 , price=self._pv.bid\n                                 , slippage=3\n                                 , stoploss=0\n                                 , takeprofit=0\n                                 , comment=""\n                                 , magic=self._pv.magic_num\n                                 , expiration=datetime(1970, 1, 1, 0, 0, 0)\n                                 , arrow_color=mc.clrRed)\n            return None\n        #--- buy conditions\n        if self._pv.open[1] < ma and self._pv.close[1] > ma:\n            res = self.OrderSend(symbol=self._pv.symbol\n                                 , cmd=mc.OP_BUY\n                                 , volume=self.__lots_optimized()\n                                 , price=self._pv.ask\n                                 , slippage=3\n                                 , stoploss=0\n                                 , takeprofit=0\n                                 , comment=""\n                                 , magic=self._pv.magic_num\n                                 , expiration=datetime(1970, 1, 1, 0, 0, 0)\n                                 , arrow_color=mc.clrBlue)\n            return None\n\n    def __calculate_current_orders(self, symbol: str) -> int:\n        buys: int = 0\n        sells: int = 0\n        # ---\n        for i in range(self.OrdersTotal()):\n            if self._tf.order_select(index=i, select=mc.SELECT_BY_POS, pool=mc.MODE_TRADES) == False:\n                break\n            if self.OrderSymbol() == self._pv.symbol and self.OrderMagicNumber() == self._pv.magic_num:\n                if self.OrderType() == mc.OP_BUY:\n                    buys += 1\n                if self.OrderType() == mc.OP_SELL:\n                    sells += 1\n        # --- return orders volume\n        if buys > 0:\n            return buys\n        else:\n            return -sells\n\ndef main() -> None:\n    ea = MA_EA()\n    ea.InitComponent(server_ip="127.0.0.1"\n                     , server_port=23456\n                     , ea_name="MA_EA")\n    ea.StartEA()\n\nif __name__ == "__main__":\n    main()\n```\n\n### How to publish to pypi\n```bash\n# set up pypi token\n$ poetry config pypi-token.pypi my-token\n\n# build the project\n$ poetry build\n\n# publish the project\n$ poetry publish\n\n# DONE\n```\n',
     'author': 'SulfredLee',
     'author_email': 'sflee1112@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
-    'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pysailfish-1.2.0/PKG-INFO` & `pysailfish-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: pysailfish
-Version: 1.2.0
+Version: 1.3.0
 Summary: 
 Author: SulfredLee
 Author-email: sflee1112@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: sfdevtools (>=1.74.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 
 ## pysailfish
 
 ### Example EA --- simple client
 ```python
```


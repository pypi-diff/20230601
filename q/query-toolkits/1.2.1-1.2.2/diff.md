# Comparing `tmp/query_toolkits-1.2.1-py3-none-any.whl.zip` & `tmp/query_toolkits-1.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 2514854 bytes, number of entries: 18
+Zip file size: 2515022 bytes, number of entries: 18
 -rw-r--r--  2.0 unx      845 b- defN 23-May-22 02:33 query_toolkits/__init__.py
 -rw-r--r--  2.0 unx    40836 b- defN 23-Mar-29 03:08 query_toolkits/error_correction.py
--rw-r--r--  2.0 unx    26721 b- defN 23-May-22 02:33 query_toolkits/extractor.py
--rw-r--r--  2.0 unx      683 b- defN 23-May-16 14:13 query_toolkits/financial_index.txt
--rw-r--r--  2.0 unx    15889 b- defN 23-May-16 13:44 query_toolkits/financial_index_full.txt
+-rw-r--r--  2.0 unx    26728 b- defN 23-Jun-01 03:20 query_toolkits/extractor.py
+-rw-r--r--  2.0 unx      783 b- defN 23-Jun-01 03:18 query_toolkits/financial_index.txt
+-rw-r--r--  2.0 unx    16386 b- defN 23-Jun-01 04:01 query_toolkits/financial_index_full.txt
 -rw-r--r--  2.0 unx  1056198 b- defN 23-Feb-27 08:08 query_toolkits/fund_product.txt
 -rw-r--r--  2.0 unx    18015 b- defN 23-May-16 12:35 query_toolkits/index.txt
 -rw-------  2.0 unx 44320114 b- defN 23-Mar-29 02:13 query_toolkits/info.json
 -rw-r--r--  2.0 unx      153 b- defN 22-Oct-10 04:02 query_toolkits/keyword.txt
 -rw-r--r--  2.0 unx   634483 b- defN 22-Oct-12 02:15 query_toolkits/organization.txt
 -rw-r--r--  2.0 unx     9995 b- defN 23-May-16 12:30 query_toolkits/product.txt
 -rw-r--r--  2.0 unx     2237 b- defN 22-Aug-15 03:50 query_toolkits/unit_transform
 -rw-r--r--  2.0 unx     5453 b- defN 23-Mar-29 02:52 query_toolkits/utils.py
 -rw-------  2.0 unx   420676 b- defN 22-Oct-20 07:33 query_toolkits/weapon.txt
--rw-r--r--  2.0 unx      230 b- defN 23-May-22 02:34 query_toolkits-1.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 02:34 query_toolkits-1.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-May-22 02:34 query_toolkits-1.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1534 b- defN 23-May-22 02:34 query_toolkits-1.2.1.dist-info/RECORD
-18 files, 46554169 bytes uncompressed, 2512354 bytes compressed:  94.6%
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-01 08:43 query_toolkits-1.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 08:43 query_toolkits-1.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-01 08:43 query_toolkits-1.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1534 b- defN 23-Jun-01 08:43 query_toolkits-1.2.2.dist-info/RECORD
+18 files, 46554773 bytes uncompressed, 2512522 bytes compressed:  94.6%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: query_toolkits/utils.py
 Comment: 
 
 Filename: query_toolkits/weapon.txt
 Comment: 
 
-Filename: query_toolkits-1.2.1.dist-info/METADATA
+Filename: query_toolkits-1.2.2.dist-info/METADATA
 Comment: 
 
-Filename: query_toolkits-1.2.1.dist-info/WHEEL
+Filename: query_toolkits-1.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: query_toolkits-1.2.1.dist-info/top_level.txt
+Filename: query_toolkits-1.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: query_toolkits-1.2.1.dist-info/RECORD
+Filename: query_toolkits-1.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## query_toolkits/extractor.py

```diff
@@ -10,15 +10,15 @@
                                                  os.path.dirname(__file__), path))
 
 class Extractor:
     def __init__(self):
         self.unit_transform = utils._read_table(_get_module_path("unit_transform"))
         self.organization = utils._read_list(_get_module_path("organization.txt"))
         self.keyword = utils._read_list(_get_module_path("keyword.txt"))
-        self.financial_dict = utils.list2dict(utils._read_list(_get_module_path("financial_index.txt")))
+        self.financial_dict = utils.list2dict(utils._read_list(_get_module_path("financial_index_full.txt")))
         self.financial_dict_keys = set(self.financial_dict.keys())
         self.fund_name = utils._read_list(_get_module_path("fund_product.txt"))
         self.stock_dict = utils._stock_dict(_get_module_path("info.json"))
         self.product_dict = utils.list2dict(utils._read_list(_get_module_path("product.txt")))
         self.index_dict = utils.list2dict(utils._read_list(_get_module_path("index.txt")))
 
 
@@ -518,14 +518,16 @@
 
 
 
 
 
 
 
+
+
```

## query_toolkits/financial_index.txt

```diff
@@ -35,8 +35,14 @@
 带息债务占比
 商誉占比
 现金短债比
 固定资产占比
 存货占比
 PEG
 流动比
-速冻比
+速冻比
+每股资本公积金
+每股净资产
+每股未分配利润
+每股经营现金流
+资产负债率
+
```

## query_toolkits/financial_index_full.txt

```diff
@@ -1,34 +1,32 @@
-市盈,pe，市盈率
-市净,pb，市净率
-市销率
+市盈,pe，市盈率,p/e
+市净,pb，市净率,p/b
+市销率,ps,p/s
 市现率
-每股收益
 净利润
 归母净利润
 股息率
 流通股，流通股本
 总市值，总值，市值
 销售毛利率
 营收
 净资产收益率，ROE
 总资产净利率，ROA
 投入资本回报率, ROIC
 营业利润率
-净利率
 资产净利率
 毛利率
 净利润增长率
 存货周转率
 营业收入
 营业收入增长率
 归母净利润增长率
 扣非净利润增长率
 自由现金流
-经营现金流
+经营现金流，经营活动产生现金流量，经营活动现金流
 收现比
 净现比
 分红募资比
 换手率
 大股东质押率
 存货周转天数
 应收帐款周转天数
@@ -197,28 +195,28 @@
 固定资产投资
 固定资产投资额
 固定资产投资率
 固定资产周转率,固定资产利用率
 固定资产周转天数
 管理费用
 管理费用率
-归母净利润,归属母公司净利润,归属母公司股东净利润,归属于母公司所有者的净利润
+归母净利润,归属母公司净利润,归属母公司股东净利润,归属于母公司所有者的净利润，归属母公司股东的净利润，归属上市公司股东的净利润
 归母净利润率
 归母净利润增长
 归母净利润增长率
 归属母公司股东权益,归属于母公司股东权益
 归属于股东的权益
 合同负债
 核心一级资本充足率
 会计年度
 活动现金流
 活期存款余额
 货币资金
 获利能力
-基本每股收益,归属母公司普通股股东净利润
+归属母公司普通股股东净利润
 计息负债
 计息负债成本率
 价格
 价格区间
 价格收益率
 价值
 价值回报率,价值加权回报率
@@ -246,15 +244,15 @@
 经营现金流入净额
 经营性现金流,经营活动现金净流
 经营性资产收益率
 经营资产
 净负债,净负债/股东权益,净负债/净资产
 净负债率,债务股权比率
 净利差
-净利率
+净利率，净利润率
 净利润
 净利润率
 净利润同比增长率
 净利润增长率
 净流动资产
 净收入,手续费净收入,净利息收入
 净收益
@@ -272,15 +270,15 @@
 净值比率
 净资产额,净资产总额
 净资产利润率
 净资产收益,ROE
 净资产收益率,权益净利率,股东权益报酬率,净值报酬率,股本回报率
 净资产增长率
 绝对涨幅
-扣非净利润
+扣非净利润,EVE净利润,扣除非经营损益净利润,扣除非经营性损益净利润,扣除非经营性损益的净利润,扣除非经常损益净利润,扣除非经常性损益净利润,扣除非经常性损益的净利润
 累计营收增速
 利率
 利润,利润表
 利润分配
 利润率,profit rate
 利润同比增速
 利润增长率
@@ -304,25 +302,25 @@
 流动资金增量
 流通股本
 流通股比例,股票流通比例
 流通市值
 买入
 毛利率,毛利润率
 毛利率预测
-毛利润
+毛利润，毛利
 毛收入,总收入
 毛收益率
 每股股利
 每股股息
 每股红利
 每股经营现金净流
 每股经营性现金流净额
 每股净资产
 每股净资产收益
-每股收益,每股盈利,EPS,每股税后利润,每股盈余
+每股收益,每股盈利,EPS,每股税后利润,每股盈余，基本每股收益
 每股有形资产
 每股帐面价值,BVPS
 每股指标
 目标价
 纳税额
 内部收益率
 年度净利润
@@ -366,17 +364,16 @@
 趋势回报率
 权益,权益比率,权益总额,权益报酬率
 权益乘数
 权益性投资收益
 让渡资产使用权收入
 人工成本
 日均成交值
-融资现金流
 融资现金流合计
-融资现金流量,融资活动现金流量,融资活动净现金流量,融资活动产生现金流量,融资性现金流量
+融资现金流，融资现金流量,融资活动现金流量,融资活动净现金流量,融资活动产生现金流量,融资性现金流量，融资活动产生现金流量
 三项费用
 少数股东权益,少数股权
 少数股东损益
 生息率
 生息资产
 生息资产收益率
 市销率,PS
@@ -433,16 +430,15 @@
 投资价值
 投资决策
 投资评级
 投资收益,投资净收益
 投资收益率
 投资损失
 投资现金净流入
-投资现金流
-投资现金流量,投资活动现金流量
+投资现金流，投资现金流量,投资活动现金流量，投资活动产生现金流量
 投资现金流量净额,投资活动现金流量净额,投资活动产生的现金流量净额,投资活动净现金流量
 投资性房地产
 投资性现金流,投资活动现金净流
 投资性现金流量,投资活动产生现金流量
 投资占比
 外汇汇率
 违约金收入
@@ -534,15 +530,15 @@
 营业成本
 营业费用
 营业费用率
 营业利率
 营业利润,销售利润
 营业利润增长率,营业利润增长
 营业利润占营业收入比率,营业利润率
-营业收入,营收
+营业收入,营收，营业额
 营业收入增速
 营业收入增长
 营业收入增长率,营收收入增长率,营收增长率
 营业税金及附加
 营业税金率
 营业外收入
 营业外收支
@@ -799,10 +795,12 @@
 佣金率
 运营效率比率
 主营业务利润
 自由现金流量股息支付率
 综合成本率
 综合赔付率
 总产能
+复合年均增长率，cagr，复合增长率
+
```

## Comparing `query_toolkits-1.2.1.dist-info/RECORD` & `query_toolkits-1.2.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 query_toolkits/__init__.py,sha256=EveacW4_39hG1bXQXu2-_iach21RtE1NVgSjXgmaDyE,845
 query_toolkits/error_correction.py,sha256=auit3b2ihsuWufmNixOrjC5CEjVrD2IiAzj461YrJUg,40836
-query_toolkits/extractor.py,sha256=6QwR2P-SXkf0-HeEtND5n6S-PikZSHQEwUTZSC5JmyM,26721
-query_toolkits/financial_index.txt,sha256=BJDWXmJ0vziCHq6hq8cOEUCdPegzweiugvDObb23lKQ,683
-query_toolkits/financial_index_full.txt,sha256=1ViFxMXJd2BvCxjlOI0vAAKuHFTrx2JAdnjtId9jxqc,15889
+query_toolkits/extractor.py,sha256=SHgNMCmFPvJUiwF2k4IghZ6BUooPNmTxAvUgC6ftxv8,26728
+query_toolkits/financial_index.txt,sha256=Lw12OQ50B8-vFD3W6H7uAFtAWkmHDx1az5PX9I5h98g,783
+query_toolkits/financial_index_full.txt,sha256=IreFvGQWJJtzT67BU8rSJcdonMSkbKPSz-IMzGwL8RY,16386
 query_toolkits/fund_product.txt,sha256=Fn3FPhk10KjtHkyXD0OHK8OttYjVtN4KRiTQ6X4c0uI,1056198
 query_toolkits/index.txt,sha256=W9_pC0bCTEVykwjwSI1Zi7gFFW94BrsvKdkzRBkhWBw,18015
 query_toolkits/info.json,sha256=BC85jy__r1H89WHSJqkmfKK0arna3MlP0V3cDvARo_w,44320114
 query_toolkits/keyword.txt,sha256=iFtkA8SUDbKViFYSg2YPP9RG_btJ35AlGor06ywy0A4,153
 query_toolkits/organization.txt,sha256=hRLDyvQKxw-_XgM2WEQ9MD3DvmanTluYu2Z6Se5JYro,634483
 query_toolkits/product.txt,sha256=PAWJ7YtTOydgsGcZ470hQ-wgXtYHMEDCFa23lKy1Zns,9995
 query_toolkits/unit_transform,sha256=yHFE7ydHauFdJy13GNCyYmNZy0gQWd0lYlvki_6OUD4,2237
 query_toolkits/utils.py,sha256=zPTVyjmxeioiND7PlUfCkUjMi50wKgcRghyzmo_20ig,5453
 query_toolkits/weapon.txt,sha256=rpGr_JynyYjrvnoM-swGLM1DLdxNKITUNJyfb_juw_E,420676
-query_toolkits-1.2.1.dist-info/METADATA,sha256=suJdXJZE39lMZr_yfg7u78ZQSclXepTJNWjf_vVWfQ0,230
-query_toolkits-1.2.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-query_toolkits-1.2.1.dist-info/top_level.txt,sha256=oX-XPh75LlcNrWWX-7EQ7ciThjo7m_iFQkriyWxvwCo,15
-query_toolkits-1.2.1.dist-info/RECORD,,
+query_toolkits-1.2.2.dist-info/METADATA,sha256=7jd7s_unoNo2upJnJ9g7ueSr5-vARsRehm1-_DrMTrY,230
+query_toolkits-1.2.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+query_toolkits-1.2.2.dist-info/top_level.txt,sha256=oX-XPh75LlcNrWWX-7EQ7ciThjo7m_iFQkriyWxvwCo,15
+query_toolkits-1.2.2.dist-info/RECORD,,
```


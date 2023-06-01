# Comparing `tmp/sinergym-2.4.1.tar.gz` & `tmp/sinergym-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinergym-2.4.1.tar", last modified: Tue May 30 13:36:31 2023, max compression
+gzip compressed data, was "sinergym-2.5.0.tar", last modified: Thu Jun  1 14:14:15 2023, max compression
```

## Comparing `sinergym-2.4.1.tar` & `sinergym-2.5.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.872037 sinergym-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-30 13:36:28.000000 sinergym-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-30 13:36:28.000000 sinergym-2.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-05-30 13:36:31.872037 sinergym-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-05-30 13:36:28.000000 sinergym-2.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-30 13:36:30.000000 sinergym-2.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-30 13:36:31.872037 sinergym-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-30 13:36:30.000000 sinergym-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.840037 sinergym-2.4.1/sinergym/
--rw-r--r--   0 runner    (1001) docker     (123)    95172 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.840037 sinergym-2.4.1/sinergym/config/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36306 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/config/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.836037 sinergym-2.4.1/sinergym/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.844037 sinergym-2.4.1/sinergym/data/buildings/
--rw-r--r--   0 runner    (1001) docker     (123)   155871 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON
--rw-r--r--   0 runner    (1001) docker     (123)   147138 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/buildings/5ZoneAutoDXVAV.epJSON
--rw-r--r--   0 runner    (1001) docker     (123)   627443 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.epJSON
--rw-r--r--   0 runner    (1001) docker     (123)   361854 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.epJSON
--rw-r--r--   0 runner    (1001) docker     (123)   521353 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/buildings/OfficeGridStorageSmoothing.epJSON
--rw-r--r--   0 runner    (1001) docker     (123)   251292 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/buildings/ShopWithVandBattery.epJSON
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.844037 sinergym-2.4.1/sinergym/data/variables/
--rw-r--r--   0 runner    (1001) docker     (123)    35474 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    32612 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/variables/5ZoneAutoDXVAV.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    39868 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    36451 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    42336 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/variables/OfficeGridStorageSmoothing.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    42494 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/variables/ShopWithVandBattery.rdd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.868037 sinergym-2.4.1/sinergym/data/weather/
--rw-r--r--   0 runner    (1001) docker     (123)    28629 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1565086 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28503 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1550279 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28704 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1621761 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1553382 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28801 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1558629 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1558423 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28659 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1601571 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29016 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1637298 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29489 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1629153 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28793 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1639985 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29614 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1613784 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29529 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1624547 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1625209 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.868037 sinergym-2.4.1/sinergym/envs/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/envs/eplus_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.872037 sinergym-2.4.1/sinergym/simulators/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/simulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/simulators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25211 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/simulators/eplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/simulators/eplus_alpha.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.872037 sinergym-2.4.1/sinergym/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    39674 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/env_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    12757 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/utils/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 13:36:30.000000 sinergym-2.4.1/sinergym/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:36:31.840037 sinergym-2.4.1/sinergym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-05-30 13:36:31.000000 sinergym-2.4.1/sinergym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-30 13:36:31.000000 sinergym-2.4.1/sinergym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:36:31.000000 sinergym-2.4.1/sinergym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-30 13:36:31.000000 sinergym-2.4.1/sinergym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 13:36:31.000000 sinergym-2.4.1/sinergym.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:15.225474 sinergym-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-01 14:14:12.000000 sinergym-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-01 14:14:12.000000 sinergym-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-06-01 14:14:15.225474 sinergym-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-06-01 14:14:12.000000 sinergym-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-01 14:14:14.000000 sinergym-2.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-01 14:14:15.225474 sinergym-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-01 14:14:14.000000 sinergym-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:15.193473 sinergym-2.5.0/sinergym/
+-rw-r--r--   0 runner    (1001) docker     (123)    95280 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:15.193473 sinergym-2.5.0/sinergym/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36311 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/config/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:15.193473 sinergym-2.5.0/sinergym/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:15.197473 sinergym-2.5.0/sinergym/data/buildings/
+-rw-r--r--   0 runner    (1001) docker     (123)   167116 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON
+-rw-r--r--   0 runner    (1001) docker     (123)   153252 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/buildings/5ZoneAutoDXVAV.epJSON
+-rw-r--r--   0 runner    (1001) docker     (123)   595916 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/buildings/ASHRAE901_OfficeMedium_STD2019_Denver.epJSON
+-rw-r--r--   0 runner    (1001) docker     (123)   273893 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/buildings/ASHRAE901_Warehouse_STD2019_Denver.epJSON
+-rw-r--r--   0 runner    (1001) docker     (123)   522393 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/buildings/LrgOff_GridStorageScheduled.epJSON
+-rw-r--r--   0 runner    (1001) docker     (123)   251679 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/buildings/ShopWithPVandBattery.epJSON
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:15.197473 sinergym-2.5.0/sinergym/data/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)    39571 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    35724 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/variables/5ZoneAutoDXVAV.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    43088 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/variables/ASHRAE901_OfficeMedium_STD2019_Denver.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    40843 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/variables/ASHRAE901_Warehouse_STD2019_Denver.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    45556 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/variables/LrgOff_GridStorageScheduled.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    46370 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/variables/ShopWithPVandBattery.rdd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:15.221474 sinergym-2.5.0/sinergym/data/weather/
+-rw-r--r--   0 runner    (1001) docker     (123)    28629 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1565086 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28503 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1550279 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28704 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1621761 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1553382 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28801 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1558629 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1558423 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28659 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1601571 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29016 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1637298 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29489 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1629153 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28793 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1639985 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29614 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1613784 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29529 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1624547 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1625209 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:15.221474 sinergym-2.5.0/sinergym/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/envs/eplus_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:15.225474 sinergym-2.5.0/sinergym/simulators/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/simulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/simulators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25211 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/simulators/eplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/simulators/eplus_alpha.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:15.225474 sinergym-2.5.0/sinergym/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39016 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/utils/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/utils/env_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/utils/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12757 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/utils/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/utils/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 14:14:14.000000 sinergym-2.5.0/sinergym/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:14:15.193473 sinergym-2.5.0/sinergym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-06-01 14:14:15.000000 sinergym-2.5.0/sinergym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-01 14:14:15.000000 sinergym-2.5.0/sinergym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:14:15.000000 sinergym-2.5.0/sinergym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-01 14:14:15.000000 sinergym-2.5.0/sinergym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 14:14:15.000000 sinergym-2.5.0/sinergym.egg-info/top_level.txt
```

### Comparing `sinergym-2.4.1/LICENSE` & `sinergym-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/PKG-INFO` & `sinergym-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinergym
-Version: 2.4.1
+Version: 2.5.0
 Summary: The goal of sinergym is to create an environment following OpenAI Gym interface for wrapping simulation engines for building control using deep reinforcement learning.
 Home-page: https://github.com/ugr-sail/sinergym
 Author: J. Jiménez, J. Gómez, M. Molina, A. Manjavacas, A. Campoy
 Author-email: alejandroac79@gmail.com
 License: MIT
 Keywords: control reinforcement-learning buildings reinforcement-learning-environments
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sinergym Version: 2.4.1 Summary: The goal of
+Metadata-Version: 2.1 Name: sinergym Version: 2.5.0 Summary: The goal of
 sinergym is to create an environment following OpenAI Gym interface for
 wrapping simulation engines for building control using deep reinforcement
 learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
 J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
 alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
 buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
```

### Comparing `sinergym-2.4.1/README.md` & `sinergym-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/setup.py` & `sinergym-2.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/__init__.py` & `sinergym-2.5.0/sinergym/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -651,15 +651,15 @@
 # ---------------------------------------------------------------------------- #
 
 # 25) WH, hot weather, discrete actions
 register(
     id='Eplus-warehouse-hot-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
+        'building_file': 'ASHRAE901_Warehouse_STD2019_Denver.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -677,15 +677,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 26) WH, hot weather, continuous actions
 register(
     id='Eplus-warehouse-hot-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
+        'building_file': 'ASHRAE901_Warehouse_STD2019_Denver.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -703,15 +703,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 27) WH, hot weather, discrete actions and stochastic
 register(
     id='Eplus-warehouse-hot-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
+        'building_file': 'ASHRAE901_Warehouse_STD2019_Denver.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -730,15 +730,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 28) WH, hot weather, continuous actions and stochastic
 register(
     id='Eplus-warehouse-hot-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
+        'building_file': 'ASHRAE901_Warehouse_STD2019_Denver.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -757,15 +757,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 29) WH, mixed weather, discrete actions
 register(
     id='Eplus-warehouse-mixed-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
+        'building_file': 'ASHRAE901_Warehouse_STD2019_Denver.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -783,15 +783,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 30) WH, mixed weather, continuous actions
 register(
     id='Eplus-warehouse-mixed-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
+        'building_file': 'ASHRAE901_Warehouse_STD2019_Denver.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -809,15 +809,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 31) WH, mixed weather, discrete actions and stochastic
 register(
     id='Eplus-warehouse-mixed-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
+        'building_file': 'ASHRAE901_Warehouse_STD2019_Denver.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -836,15 +836,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 32) WH, mixed weather, continuous actions and stochastic
 register(
     id='Eplus-warehouse-mixed-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
+        'building_file': 'ASHRAE901_Warehouse_STD2019_Denver.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -863,15 +863,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 33) WH, cool weather, discrete actions
 register(
     id='Eplus-warehouse-cool-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
+        'building_file': 'ASHRAE901_Warehouse_STD2019_Denver.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -889,15 +889,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 34) WH, cool weather, continuous actions
 register(
     id='Eplus-warehouse-cool-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
+        'building_file': 'ASHRAE901_Warehouse_STD2019_Denver.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -915,15 +915,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 35) WH, cool weather, discrete actions and stochastic
 register(
     id='Eplus-warehouse-cool-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
+        'building_file': 'ASHRAE901_Warehouse_STD2019_Denver.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -942,15 +942,15 @@
         'action_definition': DEFAULT_WAREHOUSE_ACTION_DEFINITION})
 
 # 36) WH, cool weather, continuous actions and stochastic
 register(
     id='Eplus-warehouse-cool-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_Warehouse_Denver.epJSON',
+        'building_file': 'ASHRAE901_Warehouse_STD2019_Denver.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_WAREHOUSE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_WAREHOUSE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_WAREHOUSE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_WAREHOUSE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_WAREHOUSE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -974,15 +974,15 @@
 # ---------------------------------------------------------------------------- #
 
 # 37) MO, hot weather, discrete actions
 register(
     id='Eplus-office-hot-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
+        'building_file': 'ASHRAE901_OfficeMedium_STD2019_Denver.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1015,15 +1015,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 38) MO, hot weather, continuous actions
 register(
     id='Eplus-office-hot-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
+        'building_file': 'ASHRAE901_OfficeMedium_STD2019_Denver.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1056,15 +1056,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 39) MO, hot weather, discrete actions and stochastic
 register(
     id='Eplus-office-hot-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
+        'building_file': 'ASHRAE901_OfficeMedium_STD2019_Denver.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1098,15 +1098,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 40) MO, hot weather, continuous actions and stochastic
 register(
     id='Eplus-office-hot-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
+        'building_file': 'ASHRAE901_OfficeMedium_STD2019_Denver.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1140,15 +1140,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 41) MO, mixed weather, discrete actions
 register(
     id='Eplus-office-mixed-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
+        'building_file': 'ASHRAE901_OfficeMedium_STD2019_Denver.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1181,15 +1181,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 42) MO, mixed weather, continuous actions
 register(
     id='Eplus-office-mixed-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
+        'building_file': 'ASHRAE901_OfficeMedium_STD2019_Denver.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1222,15 +1222,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 43) MO, mixed weather, discrete actions and stochastic
 register(
     id='Eplus-office-mixed-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
+        'building_file': 'ASHRAE901_OfficeMedium_STD2019_Denver.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1264,15 +1264,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 44) MO, mixed weather, continuous actions and stochastic
 register(
     id='Eplus-office-mixed-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
+        'building_file': 'ASHRAE901_OfficeMedium_STD2019_Denver.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1306,15 +1306,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 45) MO, cool weather, discrete actions
 register(
     id='Eplus-office-cool-discrete-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
+        'building_file': 'ASHRAE901_OfficeMedium_STD2019_Denver.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1347,15 +1347,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 46) MO, cool weather, continuous actions
 register(
     id='Eplus-office-cool-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
+        'building_file': 'ASHRAE901_OfficeMedium_STD2019_Denver.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1388,15 +1388,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 47) MO, cool weather, discrete actions and stochastic
 register(
     id='Eplus-office-cool-discrete-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
+        'building_file': 'ASHRAE901_OfficeMedium_STD2019_Denver.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_DISCRETE,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1430,15 +1430,15 @@
         'action_definition': DEFAULT_OFFICE_ACTION_DEFINITION})
 
 # 48) MO, cool weather, continuous actions and stochastic
 register(
     id='Eplus-office-cool-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ASHRAE9012016_OfficeMedium_Denver.epJSON',
+        'building_file': 'ASHRAE901_OfficeMedium_STD2019_Denver.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_OFFICE_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICE_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICE_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICE_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICE_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1475,15 +1475,15 @@
 #                                  Office Grid                                 #
 # ---------------------------------------------------------------------------- #
 
 register(
     id='Eplus-officegrid-cool-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'OfficeGridStorageSmoothing.epJSON',
+        'building_file': 'LrgOff_GridStorageScheduled.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_OFFICEGRID_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICEGRID_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICEGRID_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICEGRID_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICEGRID_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1517,15 +1517,15 @@
         'env_name': 'officegrid-cool-continuous-v1',
         'action_definition': DEFAULT_OFFICEGRID_ACTION_DEFINITION})
 
 register(
     id='Eplus-officegrid-mixed-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'OfficeGridStorageSmoothing.epJSON',
+        'building_file': 'LrgOff_GridStorageScheduled.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_OFFICEGRID_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICEGRID_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICEGRID_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICEGRID_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICEGRID_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1559,15 +1559,15 @@
         'env_name': 'officegrid-mixed-continuous-v1',
         'action_definition': DEFAULT_OFFICEGRID_ACTION_DEFINITION})
 
 register(
     id='Eplus-officegrid-hot-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'OfficeGridStorageSmoothing.epJSON',
+        'building_file': 'LrgOff_GridStorageScheduled.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_OFFICEGRID_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICEGRID_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICEGRID_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICEGRID_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICEGRID_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1601,15 +1601,15 @@
         'env_name': 'officegrid-hot-continuous-v1',
         'action_definition': DEFAULT_OFFICEGRID_ACTION_DEFINITION})
 
 register(
     id='Eplus-officegrid-cool-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'OfficeGridStorageSmoothing.epJSON',
+        'building_file': 'LrgOff_GridStorageScheduled.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_OFFICEGRID_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICEGRID_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICEGRID_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICEGRID_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICEGRID_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1644,15 +1644,15 @@
         'env_name': 'officegrid-cool-continuous-stochastic-v1',
         'action_definition': DEFAULT_OFFICEGRID_ACTION_DEFINITION})
 
 register(
     id='Eplus-officegrid-mixed-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'OfficeGridStorageSmoothing.epJSON',
+        'building_file': 'LrgOff_GridStorageScheduled.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_OFFICEGRID_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICEGRID_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICEGRID_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICEGRID_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICEGRID_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1687,15 +1687,15 @@
         'env_name': 'officegrid-mixed-continuous-stochastic-v1',
         'action_definition': DEFAULT_OFFICEGRID_ACTION_DEFINITION})
 
 register(
     id='Eplus-officegrid-hot-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'OfficeGridStorageSmoothing.epJSON',
+        'building_file': 'LrgOff_GridStorageScheduled.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_OFFICEGRID_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_OFFICEGRID_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_OFFICEGRID_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_OFFICEGRID_ACTION_VARIABLES,
         'action_mapping': DEFAULT_OFFICEGRID_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1734,15 +1734,15 @@
 #                                 Shop Battery                                 #
 # ---------------------------------------------------------------------------- #
 
 register(
     id='Eplus-shop-cool-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ShopWithVandBattery.epJSON',
+        'building_file': 'ShopWithPVandBattery.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_SHOP_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_SHOP_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_SHOP_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_SHOP_ACTION_VARIABLES,
         'action_mapping': DEFAULT_SHOP_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1762,15 +1762,15 @@
         'env_name': 'shop-cool-continuous-v1',
         'action_definition': DEFAULT_SHOP_ACTION_DEFINITION})
 
 register(
     id='Eplus-shop-mixed-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ShopWithVandBattery.epJSON',
+        'building_file': 'ShopWithPVandBattery.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_SHOP_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_SHOP_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_SHOP_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_SHOP_ACTION_VARIABLES,
         'action_mapping': DEFAULT_SHOP_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1790,15 +1790,15 @@
         'env_name': 'shop-mixed-continuous-v1',
         'action_definition': DEFAULT_SHOP_ACTION_DEFINITION})
 
 register(
     id='Eplus-shop-hot-continuous-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ShopWithVandBattery.epJSON',
+        'building_file': 'ShopWithPVandBattery.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_SHOP_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_SHOP_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_SHOP_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_SHOP_ACTION_VARIABLES,
         'action_mapping': DEFAULT_SHOP_ACTION_MAPPING,
         'reward': LinearReward,
@@ -1818,15 +1818,15 @@
         'env_name': 'shop-hot-continuous-v1',
         'action_definition': DEFAULT_SHOP_ACTION_DEFINITION})
 
 register(
     id='Eplus-shop-cool-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ShopWithVandBattery.epJSON',
+        'building_file': 'ShopWithPVandBattery.epJSON',
         'weather_file': 'USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw',
         'observation_space': DEFAULT_SHOP_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_SHOP_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_SHOP_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_SHOP_ACTION_VARIABLES,
         'action_mapping': DEFAULT_SHOP_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1847,15 +1847,15 @@
         'env_name': 'shop-cool-continuous-stochastic-v1',
         'action_definition': DEFAULT_SHOP_ACTION_DEFINITION})
 
 register(
     id='Eplus-shop-mixed-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ShopWithVandBattery.epJSON',
+        'building_file': 'ShopWithPVandBattery.epJSON',
         'weather_file': 'USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw',
         'observation_space': DEFAULT_SHOP_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_SHOP_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_SHOP_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_SHOP_ACTION_VARIABLES,
         'action_mapping': DEFAULT_SHOP_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
@@ -1876,15 +1876,15 @@
         'env_name': 'shop-mixed-continuous-stochastic-v1',
         'action_definition': DEFAULT_SHOP_ACTION_DEFINITION})
 
 register(
     id='Eplus-shop-hot-continuous-stochastic-v1',
     entry_point='sinergym.envs:EplusEnv',
     kwargs={
-        'building_file': 'ShopWithVandBattery.epJSON',
+        'building_file': 'ShopWithPVandBattery.epJSON',
         'weather_file': 'USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw',
         'observation_space': DEFAULT_SHOP_OBSERVATION_SPACE,
         'observation_variables': DEFAULT_SHOP_OBSERVATION_VARIABLES,
         'action_space': DEFAULT_SHOP_ACTION_SPACE_CONTINUOUS,
         'action_variables': DEFAULT_SHOP_ACTION_VARIABLES,
         'action_mapping': DEFAULT_SHOP_ACTION_MAPPING,
         'weather_variability': (1.0, 0.0, 0.001),
```

### Comparing `sinergym-2.4.1/sinergym/config/modeling.py` & `sinergym-2.5.0/sinergym/config/modeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         :param _json_path: JSON path origin for apply extra configuration.
         :param weather_files: weather available files for each episode
         :param _weather_path: EPW path origin for apply weather to simulation in current episode.
         :param _ddy_path: DDY path origin for get DesignDays and weather Location
         :param experiment_path: Path for Sinergym experiment output
         :param episode_path: Path for Sinergym specific episode (before first simulator reset this param is None)
         :param max_ep_store: Number of episodes directories will be stored in experiment_path
-        :param config: Dict config with extra configuration which is required to modify IDF model (may be None)
+        :param config: Dict config with extra configuration which is required to modify building model (may be None)
         :param _idd: IDD opyplus object to set up Epm
         :param building: Building model (Dictionary extracted from JSON)
         :param ddy_model: opyplus Epm object with DDY model
         :param weather_data: opyplus WeatherData object with EPW data
         :param action_definition: Dict with action definition to automatic building model preparation.
     """
```

### Comparing `sinergym-2.4.1/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON` & `sinergym-2.5.0/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9878962422675873%*

 * *Differences: {"'AirLoopHVAC:OutdoorAirSystem'": "{'East Zone OA System': {delete: "*

 * *                                   "['availability_manager_list_name']}, 'West Zone OA System': "*

 * *                                   "{delete: ['availability_manager_list_name']}}",*

 * * "'Coil:Cooling:DX:SingleSpeed'": "{'East DX Cooling Coil': "*

 * *                                  "{'2023_rated_evaporator_fan_power_per_volume_flow_rate': "*

 * *                                  "934.4}, 'West DX Cooling Coil': "*

 * *                                   […]*

```diff
@@ -37,20 +37,18 @@
         "West Data Center Sys Controllers": {
             "controller_1_name": "West CW Coil Controller",
             "controller_1_object_type": "Controller:WaterCoil"
         }
     },
     "AirLoopHVAC:OutdoorAirSystem": {
         "East Zone OA System": {
-            "availability_manager_list_name": "East Data Center Avail List",
             "controller_list_name": "East Data Center OA Controllers",
             "outdoor_air_equipment_list_name": "East Data Center OA Equipment"
         },
         "West Zone OA System": {
-            "availability_manager_list_name": "West Data Center Avail List",
             "controller_list_name": "West Data Center OA Controllers",
             "outdoor_air_equipment_list_name": "West Data Center OA Equipment"
         }
     },
     "AirLoopHVAC:OutdoorAirSystem:EquipmentList": {
         "East Data Center OA Equipment": {
             "component_1_name": "East Data Center OAM Box",
@@ -1363,14 +1361,15 @@
             "nominal_cop": 5.0,
             "optimum_part_load_ratio": 0.65,
             "temperature_rise_coefficient": 2.682759
         }
     },
     "Coil:Cooling:DX:SingleSpeed": {
         "East DX Cooling Coil": {
+            "2023_rated_evaporator_fan_power_per_volume_flow_rate": 934.4,
             "air_inlet_node_name": "East Zone IEC Outlet Node",
             "air_outlet_node_name": "East Zone CCoil Air Outlet Node",
             "availability_schedule_name": "EastDXCCoilAvailSched",
             "energy_input_ratio_function_of_flow_fraction_curve_name": "DXSysACCoolEIRFFF",
             "energy_input_ratio_function_of_temperature_curve_name": "DXSysACCoolEIRFT",
             "gross_rated_cooling_cop": 3.0,
             "gross_rated_sensible_heat_ratio": "Autosize",
@@ -1378,14 +1377,15 @@
             "part_load_fraction_correlation_curve_name": "DXSysACCoolPLFFPLR",
             "rated_air_flow_rate": "Autosize",
             "report_ashrae_standard_127_performance_ratings": "Yes",
             "total_cooling_capacity_function_of_flow_fraction_curve_name": "DXSysACCoolCapFFF",
             "total_cooling_capacity_function_of_temperature_curve_name": "DXSysACCoolCapFT"
         },
         "West DX Cooling Coil": {
+            "2023_rated_evaporator_fan_power_per_volume_flow_rate": 934.4,
             "air_inlet_node_name": "West Zone IEC Outlet Node",
             "air_outlet_node_name": "West Zone CCoil Air Outlet Node",
             "availability_schedule_name": "WestDXCCoilAvailSched",
             "energy_input_ratio_function_of_flow_fraction_curve_name": "DXSysACCoolEIRFFF",
             "energy_input_ratio_function_of_temperature_curve_name": "DXSysACCoolEIRFT",
             "gross_rated_cooling_cop": 3.0,
             "gross_rated_sensible_heat_ratio": "Autosize",
@@ -1864,30 +1864,30 @@
             "design_level": 0.0,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "MiscPlug",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "East Zone"
+            "zone_or_zonelist_or_space_or_spacelist_name": "East Zone"
         },
         "West Zone_MiscPlug_Equip": {
             "design_level": 0.0,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "MiscPlug",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.25,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "West Zone"
+            "zone_or_zonelist_or_space_or_spacelist_name": "West Zone"
         }
     },
     "ElectricEquipment:ITE:AirCooled": {
         "EastDataCenter_Equip": {
-            "air_flow_calculation_method": "FlowFromSystem",
+            "air_flow_calculation_method": "FlowControlWithApproachTemperatures",
             "air_flow_function_of_loading_and_air_temperature_curve_name": "Data Center Servers Airflow fLoadTemp",
             "air_inlet_connection_type": "AdjustedSupply",
             "cpu_end_use_subcategory": "ITE-CPU",
             "cpu_loading_schedule_name": "Data Center CPU Loading Schedule",
             "cpu_power_input_function_of_loading_and_air_temperature_curve_name": "Data Center Servers Power fLoadTemp",
             "design_electric_power_supply_efficiency": 0.9,
             "design_entering_air_temperature": 15,
@@ -1899,17 +1899,19 @@
             "electric_power_supply_efficiency_function_of_part_load_ratio_curve_name": "UPS Efficiency fPLR",
             "electric_power_supply_end_use_subcategory": "ITE-UPS",
             "environmental_class": "A3",
             "fan_end_use_subcategory": "ITE-Fans",
             "fan_power_input_function_of_flow_curve_name": "ECM FanPower fFlow",
             "fraction_of_electric_power_supply_losses_to_zone": 1,
             "recirculation_function_of_loading_and_supply_temperature_curve_name": "Data Center Recirculation fLoadTemp",
+            "return_temperature_difference": 0,
             "supply_air_node_name": "East Zone Inlet Node",
+            "supply_temperature_difference": 2,
             "watts_per_zone_floor_area": 200,
-            "zone_name": "East Zone"
+            "zone_or_space_name": "East Zone"
         },
         "WestDataCenter_Equip": {
             "air_flow_calculation_method": "FlowFromSystem",
             "air_flow_function_of_loading_and_air_temperature_curve_name": "Data Center Servers Airflow fLoadTemp",
             "air_inlet_connection_type": "AdjustedSupply",
             "cpu_end_use_subcategory": "ITE-CPU",
             "cpu_loading_schedule_name": "Data Center CPU Loading Schedule",
@@ -1926,15 +1928,15 @@
             "environmental_class": "A3",
             "fan_end_use_subcategory": "ITE-Fans",
             "fan_power_input_function_of_flow_curve_name": "ECM FanPower fFlow",
             "fraction_of_electric_power_supply_losses_to_zone": 1,
             "recirculation_function_of_loading_and_supply_temperature_curve_name": "Data Center Recirculation fLoadTemp",
             "supply_air_node_name": "West Zone Inlet Node",
             "watts_per_zone_floor_area": 200,
-            "zone_name": "West Zone"
+            "zone_or_space_name": "West Zone"
         }
     },
     "EnergyManagementSystem:GlobalVariable": {
         "EnergyManagementSystem:GlobalVariable 1": {
             "variables": [
                 {
                     "erl_variable_name": "PUE_Value"
@@ -1949,15 +1951,27 @@
             "update_frequency": "SystemTimestep"
         }
     },
     "EnergyManagementSystem:Program": {
         "CalculatePUE": {
             "lines": [
                 {
-                    "program_line": "set PUE_Value = Whole_Building_Power / IT_Equip_Power"
+                    "program_line": "IF IT_Equip_power > 0.0"
+                },
+                {
+                    "program_line": "set PUE_Value = whole_building_power / IT_Equip_power"
+                },
+                {
+                    "program_line": "ELSE"
+                },
+                {
+                    "program_line": "set PUE_Value = 0.0"
+                },
+                {
+                    "program_line": "ENDIF"
                 }
             ]
         }
     },
     "EnergyManagementSystem:ProgramCallingManager": {
         "Calculate Power Utilization Effectiveness": {
             "energyplus_model_calling_point": "EndOfZoneTimestepBeforeZoneReporting",
@@ -2120,26 +2134,26 @@
             "end_use_subcategory": "GeneralLights",
             "fraction_radiant": 0.59,
             "fraction_replaceable": 0,
             "fraction_visible": 0.2,
             "lighting_level": 284,
             "return_air_fraction": 0.0,
             "schedule_name": "LIGHTS-1",
-            "zone_or_zonelist_name": "East Zone"
+            "zone_or_zonelist_or_space_or_spacelist_name": "East Zone"
         },
         "West Zone Lights": {
             "design_level_calculation_method": "LightingLevel",
             "end_use_subcategory": "GeneralLights",
             "fraction_radiant": 0.59,
             "fraction_replaceable": 0,
             "fraction_visible": 0.2,
             "lighting_level": 284,
             "return_air_fraction": 0.0,
             "schedule_name": "LIGHTS-1",
-            "zone_or_zonelist_name": "West Zone"
+            "zone_or_zonelist_or_space_or_spacelist_name": "West Zone"
         }
     },
     "Material": {
         "1/2IN Gypsum": {
             "conductivity": 0.16,
             "density": 784.9,
             "roughness": "Smooth",
@@ -2360,17 +2374,14 @@
             "ems_runtime_language_debug_output_level": "Verbose",
             "internal_variable_availability_dictionary_reporting": "Verbose"
         }
     },
     "Output:Surfaces:Drawing": {
         "Output:Surfaces:Drawing 1": {
             "report_type": "DXF"
-        },
-        "Output:Surfaces:Drawing 2": {
-            "report_type": "DXF"
         }
     },
     "Output:Table:SummaryReports": {
         "Output:Table:SummaryReports 1": {
             "reports": [
                 {
                     "report_name": "AllSummary"
@@ -2378,140 +2389,415 @@
             ]
         }
     },
     "Output:Variable": {
         "Output:Variable 1": {
             "key_value": "*",
             "reporting_frequency": "Timestep",
-            "variable_name": "Site Outdoor Air Drybulb Temperature"
+            "variable_name": "Power Utilization Effectiveness"
         },
         "Output:Variable 10": {
-            "key_value": "West Zone",
+            "key_value": "East Outside Air Inlet Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermostat Cooling Setpoint Temperature"
+            "variable_name": "System Node Mass Flow Rate"
         },
         "Output:Variable 11": {
-            "key_value": "West Zone PEOPLE",
+            "key_value": "West Outside Air Inlet Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermal Comfort Fanger Model PMV"
+            "variable_name": "System Node Temperature"
         },
         "Output:Variable 12": {
-            "key_value": "West Zone",
+            "key_value": "East Outside Air Inlet Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "Zone People Occupant Count"
+            "variable_name": "System Node Temperature"
         },
         "Output:Variable 13": {
-            "key_value": "West Zone PEOPLE",
+            "key_value": "West IEC Secondary Air Inlet Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermal Comfort Fanger Model PPD"
+            "variable_name": "System Node Mass Flow Rate"
         },
         "Output:Variable 14": {
-            "key_value": "West Zone PEOPLE",
+            "key_value": "West IEC Secondary Air Inlet Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermal Comfort Clothing Value"
+            "variable_name": "System Node Temperature"
         },
         "Output:Variable 15": {
-            "key_value": "West Zone PEOPLE",
+            "key_value": "East IEC Secondary Air Inlet Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermal Comfort Mean Radiant Temperature"
+            "variable_name": "System Node Mass Flow Rate"
         },
         "Output:Variable 16": {
-            "key_value": "East Zone",
+            "key_value": "East IEC Secondary Air Inlet Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "Zone Air Temperature"
+            "variable_name": "System Node Temperature"
         },
         "Output:Variable 17": {
-            "key_value": "East Zone",
+            "key_value": "West IEC Secondary Air Outlet Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "Zone Air Relative Humidity"
+            "variable_name": "System Node Temperature"
         },
         "Output:Variable 18": {
-            "key_value": "East Zone",
+            "key_value": "West IEC Secondary Air Outlet Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermostat Heating Setpoint Temperature"
+            "variable_name": "System Node Mass Flow Rate"
         },
         "Output:Variable 19": {
-            "key_value": "East Zone",
+            "key_value": "West Zone Return Air Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermostat Cooling Setpoint Temperature"
+            "variable_name": "System Node Mass Flow Rate"
         },
         "Output:Variable 2": {
             "key_value": "*",
             "reporting_frequency": "Timestep",
-            "variable_name": "Site Outdoor Air Relative Humidity"
+            "variable_name": "Site Outdoor Air Drybulb Temperature"
         },
         "Output:Variable 20": {
-            "key_value": "East Zone PEOPLE",
+            "key_value": "West Zone Return Air Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermal Comfort Fanger Model PMV"
+            "variable_name": "System Node Temperature"
         },
         "Output:Variable 21": {
-            "key_value": "East Zone",
+            "key_value": "West Zone Mixed Air Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "Zone People Occupant Count"
+            "variable_name": "System Node Mass Flow Rate"
         },
         "Output:Variable 22": {
-            "key_value": "East Zone PEOPLE",
+            "key_value": "West Zone Mixed Air Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermal Comfort Fanger Model PPD"
+            "variable_name": "System Node Temperature"
         },
         "Output:Variable 23": {
-            "key_value": "East Zone PEOPLE",
+            "key_value": "West Zone Supply Fan Outlet Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermal Comfort Clothing Value"
+            "variable_name": "System Node Temperature"
         },
         "Output:Variable 24": {
-            "key_value": "East Zone PEOPLE",
+            "key_value": "East Zone Supply Fan Outlet Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermal Comfort Mean Radiant Temperature"
+            "variable_name": "System Node Temperature"
         },
         "Output:Variable 25": {
-            "key_value": "*",
+            "key_value": "West Zone DEC Outlet Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "People Air Temperature"
+            "variable_name": "System Node Temperature"
         },
         "Output:Variable 26": {
-            "key_value": "*",
+            "key_value": "West Zone IEC Outlet Node",
+            "reporting_frequency": "Timestep",
+            "variable_name": "System Node Temperature"
+        },
+        "Output:Variable 27": {
+            "key_value": "West Zone IEC Outlet Node",
+            "reporting_frequency": "Timestep",
+            "variable_name": "System Node Setpoint Temperature"
+        },
+        "Output:Variable 28": {
+            "key_value": "East Zone DEC Outlet Node",
+            "reporting_frequency": "Timestep",
+            "variable_name": "System Node Temperature"
+        },
+        "Output:Variable 29": {
+            "key_value": "East Zone IEC Outlet Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "Facility Total HVAC Electricity Demand Rate"
+            "variable_name": "System Node Temperature"
         },
         "Output:Variable 3": {
+            "key_value": "West Zone",
+            "reporting_frequency": "Timestep",
+            "variable_name": "Zone Air Temperature"
+        },
+        "Output:Variable 30": {
+            "key_value": "West Zone CCoil Air Outlet Node",
+            "reporting_frequency": "Timestep",
+            "variable_name": "System Node Temperature"
+        },
+        "Output:Variable 31": {
+            "key_value": "East Zone CCoil Air Outlet Node",
+            "reporting_frequency": "Timestep",
+            "variable_name": "System Node Temperature"
+        },
+        "Output:Variable 32": {
+            "key_value": "West Air Loop Outlet Node",
+            "reporting_frequency": "Timestep",
+            "variable_name": "System Node Temperature"
+        },
+        "Output:Variable 33": {
+            "key_value": "East Air Loop Outlet Node",
+            "reporting_frequency": "Timestep",
+            "variable_name": "System Node Temperature"
+        },
+        "Output:Variable 34": {
+            "key_value": "West Zone Inlet Node",
+            "reporting_frequency": "Timestep",
+            "variable_name": "System Node Mass Flow Rate"
+        },
+        "Output:Variable 35": {
+            "key_value": "West Zone Inlet Node",
+            "reporting_frequency": "Timestep",
+            "variable_name": "System Node Temperature"
+        },
+        "Output:Variable 36": {
+            "key_value": "East Zone Inlet Node",
+            "reporting_frequency": "Timestep",
+            "variable_name": "System Node Mass Flow Rate"
+        },
+        "Output:Variable 37": {
+            "key_value": "East Zone Inlet Node",
+            "reporting_frequency": "Timestep",
+            "variable_name": "System Node Temperature"
+        },
+        "Output:Variable 38": {
             "key_value": "*",
             "reporting_frequency": "Timestep",
-            "variable_name": "Site Wind Speed"
+            "variable_name": "Evaporative Cooler Stage Effectiveness"
+        },
+        "Output:Variable 39": {
+            "key_value": "*",
+            "reporting_frequency": "Timestep",
+            "variable_name": "Evaporative Cooler Total Stage Effectiveness"
         },
         "Output:Variable 4": {
+            "key_value": "East Zone",
+            "reporting_frequency": "Timestep",
+            "variable_name": "Zone Air Temperature"
+        },
+        "Output:Variable 40": {
             "key_value": "*",
             "reporting_frequency": "Timestep",
-            "variable_name": "Site Wind Direction"
+            "variable_name": "Evaporative Cooler Operating Mode Status"
         },
-        "Output:Variable 5": {
+        "Output:Variable 41": {
             "key_value": "*",
             "reporting_frequency": "Timestep",
-            "variable_name": "Site Diffuse Solar Radiation Rate per Area"
+            "variable_name": "Evaporative Cooler Electricity Rate"
         },
-        "Output:Variable 6": {
+        "Output:Variable 42": {
             "key_value": "*",
             "reporting_frequency": "Timestep",
-            "variable_name": "Site Direct Solar Radiation Rate per Area"
+            "variable_name": "Evaporative Cooler Water Volume"
         },
-        "Output:Variable 7": {
+        "Output:Variable 43": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE CPU Electricity Rate"
+        },
+        "Output:Variable 44": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Fan Electricity Rate"
+        },
+        "Output:Variable 45": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE UPS Electricity Rate"
+        },
+        "Output:Variable 46": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE CPU Electricity Rate at Design Inlet Conditions"
+        },
+        "Output:Variable 47": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Fan Electricity Rate at Design Inlet Conditions"
+        },
+        "Output:Variable 48": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE UPS Heat Gain to Zone Rate"
+        },
+        "Output:Variable 49": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Total Heat Gain to Zone Rate"
+        },
+        "Output:Variable 5": {
             "key_value": "West Zone",
             "reporting_frequency": "Timestep",
-            "variable_name": "Zone Air Temperature"
+            "variable_name": "Zone Air Relative Humidity"
         },
-        "Output:Variable 8": {
-            "key_value": "West Zone",
+        "Output:Variable 50": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Standard Density Air Volume Flow Rate"
+        },
+        "Output:Variable 51": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Air Inlet Dry-Bulb Temperature"
+        },
+        "Output:Variable 52": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Air Inlet Dewpoint Temperature"
+        },
+        "Output:Variable 53": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Air Inlet Relative Humidity"
+        },
+        "Output:Variable 54": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Air Outlet Dry-Bulb Temperature"
+        },
+        "Output:Variable 55": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Supply Heat Index"
+        },
+        "Output:Variable 56": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Air Inlet Operating Range Exceeded Time"
+        },
+        "Output:Variable 57": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Air Inlet Dry-Bulb Temperature Above Operating Range Time"
+        },
+        "Output:Variable 58": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Air Inlet Dry-Bulb Temperature Below Operating Range Time"
+        },
+        "Output:Variable 59": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Air Inlet Dewpoint Temperature Above Operating Range Time"
+        },
+        "Output:Variable 6": {
+            "key_value": "East Zone",
             "reporting_frequency": "Timestep",
             "variable_name": "Zone Air Relative Humidity"
         },
+        "Output:Variable 60": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Air Inlet Dewpoint Temperature Below Operating Range Time"
+        },
+        "Output:Variable 61": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Air Inlet Relative Humidity Above Operating Range Time"
+        },
+        "Output:Variable 62": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Air Inlet Relative Humidity Below Operating Range Time"
+        },
+        "Output:Variable 63": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Air Inlet Dry-Bulb Temperature Difference Above Operating Range"
+        },
+        "Output:Variable 64": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Air Inlet Dry-Bulb Temperature Difference Below Operating Range"
+        },
+        "Output:Variable 65": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Air Inlet Dewpoint Temperature Difference Above Operating Range"
+        },
+        "Output:Variable 66": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Air Inlet Dewpoint Temperature Difference Below Operating Range"
+        },
+        "Output:Variable 67": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Air Inlet Relative Humidity Difference Above Operating Range"
+        },
+        "Output:Variable 68": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "ITE Air Inlet Relative Humidity Difference Below Operating Range"
+        },
+        "Output:Variable 69": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Zone ITE CPU Electricity Rate"
+        },
+        "Output:Variable 7": {
+            "key_value": "*",
+            "reporting_frequency": "Timestep",
+            "variable_name": "Cooling Coil Total Cooling Rate"
+        },
+        "Output:Variable 70": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Zone ITE Fan Electricity Rate"
+        },
+        "Output:Variable 71": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Zone ITE UPS Electricity Rate"
+        },
+        "Output:Variable 72": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Zone ITE CPU Electricity Rate at Design Inlet Conditions"
+        },
+        "Output:Variable 73": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Zone ITE Fan Electricity Rate at Design Inlet Conditions"
+        },
+        "Output:Variable 74": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Zone ITE UPS Heat Gain to Zone Rate"
+        },
+        "Output:Variable 75": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Zone ITE Total Heat Gain to Zone Rate"
+        },
+        "Output:Variable 76": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Chiller Evaporator Cooling Rate"
+        },
+        "Output:Variable 77": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Chiller Evaporator Inlet Temperature"
+        },
+        "Output:Variable 78": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Chiller Evaporator Outlet Temperature"
+        },
+        "Output:Variable 79": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Chiller Condenser Heat Transfer Rate"
+        },
+        "Output:Variable 8": {
+            "key_value": "*",
+            "reporting_frequency": "Timestep",
+            "variable_name": "Cooling Coil Sensible Cooling Rate"
+        },
+        "Output:Variable 80": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Chiller Condenser Inlet Temperature"
+        },
+        "Output:Variable 81": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Chiller Condenser Outlet Temperature"
+        },
         "Output:Variable 9": {
-            "key_value": "West Zone",
+            "key_value": "West Outside Air Inlet Node",
             "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermostat Heating Setpoint Temperature"
+            "variable_name": "System Node Mass Flow Rate"
         }
     },
     "Output:VariableDictionary": {
         "Output:VariableDictionary 1": {
             "key_field": "regular"
         }
     },
@@ -2523,39 +2809,37 @@
     "People": {
         "East Zone PEOPLE": {
             "activity_level_schedule_name": "Activity Sch",
             "air_velocity_schedule_name": "Air Velo Sch",
             "carbon_dioxide_generation_rate": 3.82e-08,
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "Clothing Sch",
-            "enable_ashrae_55_comfort_warnings": "No",
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
-            "number_of_people": 7,
+            "number_of_people": 0,
             "number_of_people_calculation_method": "People",
             "number_of_people_schedule_name": "OFFICE OCCUPANCY",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "Work Eff Sch",
-            "zone_or_zonelist_name": "East Zone"
+            "zone_or_zonelist_or_space_or_spacelist_name": "East Zone"
         },
         "West Zone PEOPLE": {
             "activity_level_schedule_name": "Activity Sch",
             "air_velocity_schedule_name": "Air Velo Sch",
             "carbon_dioxide_generation_rate": 3.82e-08,
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "Clothing Sch",
-            "enable_ashrae_55_comfort_warnings": "No",
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
-            "number_of_people": 11,
+            "number_of_people": 0,
             "number_of_people_calculation_method": "People",
             "number_of_people_schedule_name": "OFFICE OCCUPANCY",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "Work Eff Sch",
-            "zone_or_zonelist_name": "West Zone"
+            "zone_or_zonelist_or_space_or_spacelist_name": "West Zone"
         }
     },
     "Pipe:Adiabatic": {
         "CW Demand Side Bypass Pipe": {
             "inlet_node_name": "CW Demand Bypass Inlet Node",
             "outlet_node_name": "CW Demand Bypass Outlet Node"
         },
@@ -4102,15 +4386,15 @@
     "Timestep": {
         "Timestep 1": {
             "number_of_timesteps_per_hour": 4
         }
     },
     "Version": {
         "Version 1": {
-            "version_identifier": "9.5"
+            "version_identifier": "23.1"
         }
     },
     "Zone": {
         "East Plenum": {
             "ceiling_height": "Autocalculate",
             "direction_of_relative_north": 0.0,
             "multiplier": 1,
```

### Comparing `sinergym-2.4.1/sinergym/data/buildings/5ZoneAutoDXVAV.epJSON` & `sinergym-2.5.0/sinergym/data/buildings/5ZoneAutoDXVAV.epJSON`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8878833735078052%*

 * *Differences: {"'AirLoopHVAC:OutdoorAirSystem'": "{'OA Sys 1': {delete: ['availability_manager_list_name']}}",*

 * * "'AirTerminal:SingleDuct:VAV:Reheat'": "{'SPACE1-1 VAV Reheat': {'damper_heating_action': "*

 * *                                        "'ReverseWithLimits', 'reheat_coil_object_type': "*

 * *                                        "'Coil:Heating:Fuel', "*

 * *                                        "'maximum_flow_per_zone_floor_area_during_reheat': "*

 * *                                        "0.002032}, 'SPACE2-1 VAV Reheat': […]*

```diff
@@ -14,15 +14,14 @@
         "OA Sys 1 Controllers": {
             "controller_1_name": "OA Controller 1",
             "controller_1_object_type": "Controller:OutdoorAir"
         }
     },
     "AirLoopHVAC:OutdoorAirSystem": {
         "OA Sys 1": {
-            "availability_manager_list_name": "VAV Sys 1 Avail List",
             "controller_list_name": "OA Sys 1 Controllers",
             "outdoor_air_equipment_list_name": "OA Sys 1 Equipment"
         }
     },
     "AirLoopHVAC:OutdoorAirSystem:EquipmentList": {
         "OA Sys 1 Equipment": {
             "component_1_name": "OA Mixing Box 1",
@@ -101,86 +100,91 @@
         "SPACE1-1 VAV Reheat": {
             "air_inlet_node_name": "SPACE1-1 ATU In Node",
             "air_outlet_node_name": "SPACE1-1 In Node",
             "availability_schedule_name": "ReheatCoilAvailSched",
             "constant_minimum_air_flow_fraction": 0.1,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "SPACE1-1 Zone Coil Air In Node",
-            "damper_heating_action": "Reverse",
+            "damper_heating_action": "ReverseWithLimits",
             "design_specification_outdoor_air_object_name": "ZoneMinOARequirements",
             "maximum_air_flow_rate": "Autosize",
             "maximum_flow_fraction_during_reheat": "Autosize",
+            "maximum_flow_per_zone_floor_area_during_reheat": 0.002032,
             "maximum_hot_water_or_steam_flow_rate": 0.0,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "SPACE1-1 Zone Coil",
-            "reheat_coil_object_type": "Coil:Heating:Electric",
+            "reheat_coil_object_type": "Coil:Heating:Fuel",
             "zone_minimum_air_flow_input_method": "Constant"
         },
         "SPACE2-1 VAV Reheat": {
             "air_inlet_node_name": "SPACE2-1 ATU In Node",
             "air_outlet_node_name": "SPACE2-1 In Node",
             "availability_schedule_name": "ReheatCoilAvailSched",
             "constant_minimum_air_flow_fraction": 0.1,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "SPACE2-1 Zone Coil Air In Node",
-            "damper_heating_action": "Reverse",
+            "damper_heating_action": "ReverseWithLimits",
             "design_specification_outdoor_air_object_name": "ZoneMinOARequirements",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_per_zone_floor_area_during_reheat": 0.002032,
             "maximum_hot_water_or_steam_flow_rate": 0.0,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "SPACE2-1 Zone Coil",
-            "reheat_coil_object_type": "Coil:Heating:Electric",
+            "reheat_coil_object_type": "Coil:Heating:Fuel",
             "zone_minimum_air_flow_input_method": "Constant"
         },
         "SPACE3-1 VAV Reheat": {
             "air_inlet_node_name": "SPACE3-1 ATU In Node",
             "air_outlet_node_name": "SPACE3-1 In Node",
             "availability_schedule_name": "ReheatCoilAvailSched",
             "constant_minimum_air_flow_fraction": 0.1,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "SPACE3-1 Zone Coil Air In Node",
-            "damper_heating_action": "Reverse",
+            "damper_heating_action": "ReverseWithLimits",
             "design_specification_outdoor_air_object_name": "ZoneMinOARequirements",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_per_zone_floor_area_during_reheat": 0.002032,
             "maximum_hot_water_or_steam_flow_rate": 0.0,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "SPACE3-1 Zone Coil",
-            "reheat_coil_object_type": "Coil:Heating:Electric",
+            "reheat_coil_object_type": "Coil:Heating:Fuel",
             "zone_minimum_air_flow_input_method": "Constant"
         },
         "SPACE4-1 VAV Reheat": {
             "air_inlet_node_name": "SPACE4-1 ATU In Node",
             "air_outlet_node_name": "SPACE4-1 In Node",
             "availability_schedule_name": "ReheatCoilAvailSched",
             "constant_minimum_air_flow_fraction": 0.1,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "SPACE4-1 Zone Coil Air In Node",
-            "damper_heating_action": "Reverse",
+            "damper_heating_action": "ReverseWithLimits",
             "design_specification_outdoor_air_object_name": "ZoneMinOARequirements",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_per_zone_floor_area_during_reheat": 0.002032,
             "maximum_hot_water_or_steam_flow_rate": 0.0,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "SPACE4-1 Zone Coil",
-            "reheat_coil_object_type": "Coil:Heating:Electric",
+            "reheat_coil_object_type": "Coil:Heating:Fuel",
             "zone_minimum_air_flow_input_method": "Constant"
         },
         "SPACE5-1 VAV Reheat": {
             "air_inlet_node_name": "SPACE5-1 ATU In Node",
             "air_outlet_node_name": "SPACE5-1 In Node",
             "availability_schedule_name": "ReheatCoilAvailSched",
             "constant_minimum_air_flow_fraction": 0.1,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "SPACE5-1 Zone Coil Air In Node",
-            "damper_heating_action": "Reverse",
+            "damper_heating_action": "ReverseWithLimits",
             "design_specification_outdoor_air_object_name": "ZoneMinOARequirements",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_per_zone_floor_area_during_reheat": 0.002032,
             "maximum_hot_water_or_steam_flow_rate": 0.0,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "SPACE5-1 Zone Coil",
-            "reheat_coil_object_type": "Coil:Heating:Electric",
+            "reheat_coil_object_type": "Coil:Heating:Fuel",
             "zone_minimum_air_flow_input_method": "Constant"
         }
     },
     "AvailabilityManager:Scheduled": {
         "VAV Sys 1 Avail": {
             "schedule_name": "FanAvailSched"
         }
@@ -209,15 +213,15 @@
                     "component_name": "DX Cooling Coil System 1",
                     "component_object_type": "CoilSystem:Cooling:DX",
                     "component_outlet_node_name": "Main Cooling Coil 1 Outlet Node"
                 },
                 {
                     "component_inlet_node_name": "Main Cooling Coil 1 Outlet Node",
                     "component_name": "Main Heating Coil 1",
-                    "component_object_type": "Coil:Heating:Electric",
+                    "component_object_type": "Coil:Heating:Fuel",
                     "component_outlet_node_name": "Main Heating Coil 1 Outlet Node"
                 },
                 {
                     "component_inlet_node_name": "Main Heating Coil 1 Outlet Node",
                     "component_name": "Supply Fan 1",
                     "component_object_type": "Fan:VariableVolume",
                     "component_outlet_node_name": "VAV Sys 1 Outlet Node"
@@ -1564,69 +1568,75 @@
             "condenser_air_inlet_node_name": "Main Cooling Coil 1 Condenser Node",
             "condenser_type": "EvaporativelyCooled",
             "energy_input_ratio_function_of_flow_fraction_curve_name": "PackagedRatedCoolEIRFFlow",
             "energy_input_ratio_function_of_temperature_curve_name": "VarSpeedCoolEIRFT",
             "high_speed_gross_rated_cooling_cop": 3.0,
             "high_speed_gross_rated_total_cooling_capacity": "Autosize",
             "high_speed_rated_air_flow_rate": "Autosize",
-            "high_speed_rated_sensible_heat_ratio": "Autosize",
+            "high_speed_rated_sensible_heat_ratio": 0.8,
             "low_speed_energy_input_ratio_function_of_temperature_curve_name": "VarSpeedCoolEIRLSFT",
             "low_speed_gross_rated_cooling_cop": 4.2,
-            "low_speed_gross_rated_sensible_heat_ratio": "Autosize",
+            "low_speed_gross_rated_sensible_heat_ratio": 0.8,
             "low_speed_gross_rated_total_cooling_capacity": "Autosize",
             "low_speed_rated_air_flow_rate": "Autosize",
             "low_speed_total_cooling_capacity_function_of_temperature_curve_name": "VarSpeedCoolCapLSFT",
             "part_load_fraction_correlation_curve_name": "VarSpeedCyclingPLFFPLR",
             "total_cooling_capacity_function_of_flow_fraction_curve_name": "PackagedRatedCoolCapFFlow",
             "total_cooling_capacity_function_of_temperature_curve_name": "VarSpeedCoolCapFT",
             "unit_internal_static_air_pressure": 450
         }
     },
-    "Coil:Heating:Electric": {
+    "Coil:Heating:Fuel": {
         "Main heating Coil 1": {
             "air_inlet_node_name": "Main Cooling Coil 1 Outlet Node",
             "air_outlet_node_name": "Main Heating Coil 1 Outlet Node",
             "availability_schedule_name": "ReheatCoilAvailSched",
-            "efficiency": 0.98,
+            "burner_efficiency": 0.8,
+            "fuel_type": "NaturalGas",
             "nominal_capacity": "Autosize",
             "temperature_setpoint_node_name": "Main Heating Coil 1 Outlet Node"
         },
         "SPACE1-1 Zone Coil": {
             "air_inlet_node_name": "SPACE1-1 Zone Coil Air In Node",
             "air_outlet_node_name": "SPACE1-1 In Node",
             "availability_schedule_name": "ReheatCoilAvailSched",
-            "efficiency": 0.98,
+            "burner_efficiency": 0.8,
+            "fuel_type": "NaturalGas",
             "nominal_capacity": "Autosize"
         },
         "SPACE2-1 Zone Coil": {
             "air_inlet_node_name": "SPACE2-1 Zone Coil Air In Node",
             "air_outlet_node_name": "SPACE2-1 In Node",
             "availability_schedule_name": "ReheatCoilAvailSched",
-            "efficiency": 0.98,
+            "burner_efficiency": 0.8,
+            "fuel_type": "NaturalGas",
             "nominal_capacity": "Autosize"
         },
         "SPACE3-1 Zone Coil": {
             "air_inlet_node_name": "SPACE3-1 Zone Coil Air In Node",
             "air_outlet_node_name": "SPACE3-1 In Node",
             "availability_schedule_name": "ReheatCoilAvailSched",
-            "efficiency": 0.98,
+            "burner_efficiency": 0.8,
+            "fuel_type": "NaturalGas",
             "nominal_capacity": "Autosize"
         },
         "SPACE4-1 Zone Coil": {
             "air_inlet_node_name": "SPACE4-1 Zone Coil Air In Node",
             "air_outlet_node_name": "SPACE4-1 In Node",
             "availability_schedule_name": "ReheatCoilAvailSched",
-            "efficiency": 0.98,
+            "burner_efficiency": 0.8,
+            "fuel_type": "NaturalGas",
             "nominal_capacity": "Autosize"
         },
         "SPACE5-1 Zone Coil": {
             "air_inlet_node_name": "SPACE5-1 Zone Coil Air In Node",
             "air_outlet_node_name": "SPACE5-1 In Node",
             "availability_schedule_name": "ReheatCoilAvailSched",
-            "efficiency": 0.98,
+            "burner_efficiency": 0.8,
+            "fuel_type": "NaturalGas",
             "nominal_capacity": "Autosize"
         }
     },
     "CoilSystem:Cooling:DX": {
         "DX Cooling Coil System 1": {
             "availability_schedule_name": "CoolingCoilAvailSched",
             "cooling_coil_name": "Main Cooling Coil 1",
@@ -1641,32 +1651,14 @@
             "outside_layer": "MAT-CLNG-1"
         },
         "Dbl Clr 3mm/13mm Air": {
             "layer_2": "AIR 13MM",
             "layer_3": "CLEAR 3MM",
             "outside_layer": "CLEAR 3MM"
         },
-        "Dbl Clr 3mm/13mm Arg": {
-            "layer_2": "ARGON 13MM",
-            "layer_3": "CLEAR 3MM",
-            "outside_layer": "CLEAR 3MM"
-        },
-        "Dbl Clr 6mm/6mm Air": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "CLEAR 6MM"
-        },
-        "Dbl LoE (e2=.1) Clr 6mm/6mm Air": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE CLEAR 6MM"
-        },
-        "FLOOR-1": {
-            "outside_layer": "MAT-FLOOR-1"
-        },
         "FLOOR-SLAB-1": {
             "layer_2": "CP01",
             "outside_layer": "CC03"
         },
         "INT-WALL-1": {
             "layer_2": "AL21",
             "layer_3": "GP02",
@@ -1674,17 +1666,14 @@
         },
         "ROOF-1": {
             "layer_2": "BR01",
             "layer_3": "IN46",
             "layer_4": "WD01",
             "outside_layer": "RG01"
         },
-        "SB-U": {
-            "outside_layer": "MAT-SB-U"
-        },
         "Sgl Grey 3mm": {
             "outside_layer": "GREY 3MM"
         },
         "WALL-1": {
             "layer_2": "PW03",
             "layer_3": "IN02",
             "layer_4": "GP01",
@@ -1843,51 +1832,51 @@
         "SPACE1-1 ElecEq 1": {
             "design_level": 1056,
             "design_level_calculation_method": "EquipmentLevel",
             "fraction_latent": 0,
             "fraction_lost": 0,
             "fraction_radiant": 0.3,
             "schedule_name": "EQUIP-1",
-            "zone_or_zonelist_name": "SPACE1-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE1-1"
         },
         "SPACE2-1 ElecEq 1": {
             "design_level": 456,
             "design_level_calculation_method": "EquipmentLevel",
             "fraction_latent": 0,
             "fraction_lost": 0,
             "fraction_radiant": 0.3,
             "schedule_name": "EQUIP-1",
-            "zone_or_zonelist_name": "SPACE2-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE2-1"
         },
         "SPACE3-1 ElecEq 1": {
             "design_level": 1056,
             "design_level_calculation_method": "EquipmentLevel",
             "fraction_latent": 0,
             "fraction_lost": 0,
             "fraction_radiant": 0.3,
             "schedule_name": "EQUIP-1",
-            "zone_or_zonelist_name": "SPACE3-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE3-1"
         },
         "SPACE4-1 ElecEq 1": {
             "design_level": 456,
             "design_level_calculation_method": "EquipmentLevel",
             "fraction_latent": 0,
             "fraction_lost": 0,
             "fraction_radiant": 0.3,
             "schedule_name": "EQUIP-1",
-            "zone_or_zonelist_name": "SPACE4-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE4-1"
         },
         "SPACE5-1 ElecEq 1": {
             "design_level": 1976,
             "design_level_calculation_method": "EquipmentLevel",
             "fraction_latent": 0,
             "fraction_lost": 0,
             "fraction_radiant": 0.3,
             "schedule_name": "EQUIP-1",
-            "zone_or_zonelist_name": "SPACE5-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE5-1"
         }
     },
     "Fan:VariableVolume": {
         "Supply Fan 1": {
             "air_inlet_node_name": "Main Heating Coil 1 Outlet Node",
             "air_outlet_node_name": "VAV Sys 1 Outlet Node",
             "availability_schedule_name": "FanAvailSched",
@@ -2045,59 +2034,59 @@
             "end_use_subcategory": "GeneralLights",
             "fraction_radiant": 0.59,
             "fraction_replaceable": 0,
             "fraction_visible": 0.2,
             "lighting_level": 1584,
             "return_air_fraction": 0.2,
             "schedule_name": "LIGHTS-1",
-            "zone_or_zonelist_name": "SPACE1-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE1-1"
         },
         "SPACE2-1 Lights 1": {
             "design_level_calculation_method": "LightingLevel",
             "end_use_subcategory": "GeneralLights",
             "fraction_radiant": 0.59,
             "fraction_replaceable": 0,
             "fraction_visible": 0.2,
             "lighting_level": 684,
             "return_air_fraction": 0.2,
             "schedule_name": "LIGHTS-1",
-            "zone_or_zonelist_name": "SPACE2-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE2-1"
         },
         "SPACE3-1 Lights 1": {
             "design_level_calculation_method": "LightingLevel",
             "end_use_subcategory": "GeneralLights",
             "fraction_radiant": 0.59,
             "fraction_replaceable": 0,
             "fraction_visible": 0.2,
             "lighting_level": 1584,
             "return_air_fraction": 0.2,
             "schedule_name": "LIGHTS-1",
-            "zone_or_zonelist_name": "SPACE3-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE3-1"
         },
         "SPACE4-1 Lights 1": {
             "design_level_calculation_method": "LightingLevel",
             "end_use_subcategory": "GeneralLights",
             "fraction_radiant": 0.59,
             "fraction_replaceable": 0,
             "fraction_visible": 0.2,
             "lighting_level": 684,
             "return_air_fraction": 0.2,
             "schedule_name": "LIGHTS-1",
-            "zone_or_zonelist_name": "SPACE4-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE4-1"
         },
         "SPACE5-1 Lights 1": {
             "design_level_calculation_method": "LightingLevel",
             "end_use_subcategory": "GeneralLights",
             "fraction_radiant": 0.59,
             "fraction_replaceable": 0,
             "fraction_visible": 0.2,
             "lighting_level": 2964,
             "return_air_fraction": 0.2,
             "schedule_name": "LIGHTS-1",
-            "zone_or_zonelist_name": "SPACE5-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE5-1"
         }
     },
     "Material": {
         "BR01": {
             "conductivity": 0.162,
             "density": 1121.0,
             "roughness": "VeryRough",
@@ -2318,14 +2307,114 @@
             "nodes": [
                 {
                     "node_or_nodelist_name": "OutsideAirInletNodes"
                 }
             ]
         }
     },
+    "Output:Meter": {
+        "Output:Meter 1": {
+            "key_name": "Cooling:Electricity",
+            "reporting_frequency": "Monthly"
+        },
+        "Output:Meter 10": {
+            "key_name": "Fans:Electricity",
+            "reporting_frequency": "RunPeriod"
+        },
+        "Output:Meter 11": {
+            "key_name": "HeatingCoils:EnergyTransfer",
+            "reporting_frequency": "RunPeriod"
+        },
+        "Output:Meter 12": {
+            "key_name": "CoolingCoils:EnergyTransfer",
+            "reporting_frequency": "RunPeriod"
+        },
+        "Output:Meter 13": {
+            "key_name": "InteriorLights:Electricity",
+            "reporting_frequency": "RunPeriod"
+        },
+        "Output:Meter 14": {
+            "key_name": "InteriorEquipment:Electricity",
+            "reporting_frequency": "RunPeriod"
+        },
+        "Output:Meter 2": {
+            "key_name": "Heating:NaturalGas",
+            "reporting_frequency": "Monthly"
+        },
+        "Output:Meter 3": {
+            "key_name": "Fans:Electricity",
+            "reporting_frequency": "Monthly"
+        },
+        "Output:Meter 4": {
+            "key_name": "HeatingCoils:EnergyTransfer",
+            "reporting_frequency": "Monthly"
+        },
+        "Output:Meter 5": {
+            "key_name": "CoolingCoils:EnergyTransfer",
+            "reporting_frequency": "Monthly"
+        },
+        "Output:Meter 6": {
+            "key_name": "InteriorLights:Electricity",
+            "reporting_frequency": "Monthly"
+        },
+        "Output:Meter 7": {
+            "key_name": "InteriorEquipment:Electricity",
+            "reporting_frequency": "Monthly"
+        },
+        "Output:Meter 8": {
+            "key_name": "Cooling:Electricity",
+            "reporting_frequency": "RunPeriod"
+        },
+        "Output:Meter 9": {
+            "key_name": "Heating:NaturalGas",
+            "reporting_frequency": "RunPeriod"
+        }
+    },
+    "Output:Meter:MeterFileOnly": {
+        "Output:Meter:MeterFileOnly 1": {
+            "key_name": "Electricity:Facility",
+            "reporting_frequency": "Monthly"
+        },
+        "Output:Meter:MeterFileOnly 10": {
+            "key_name": "NaturalGas:HVAC",
+            "reporting_frequency": "RunPeriod"
+        },
+        "Output:Meter:MeterFileOnly 2": {
+            "key_name": "Electricity:Building",
+            "reporting_frequency": "Monthly"
+        },
+        "Output:Meter:MeterFileOnly 3": {
+            "key_name": "Electricity:HVAC",
+            "reporting_frequency": "Monthly"
+        },
+        "Output:Meter:MeterFileOnly 4": {
+            "key_name": "NaturalGas:Facility",
+            "reporting_frequency": "Monthly"
+        },
+        "Output:Meter:MeterFileOnly 5": {
+            "key_name": "NaturalGas:HVAC",
+            "reporting_frequency": "Monthly"
+        },
+        "Output:Meter:MeterFileOnly 6": {
+            "key_name": "Electricity:Facility",
+            "reporting_frequency": "RunPeriod"
+        },
+        "Output:Meter:MeterFileOnly 7": {
+            "key_name": "Electricity:Building",
+            "reporting_frequency": "RunPeriod"
+        },
+        "Output:Meter:MeterFileOnly 8": {
+            "key_name": "Electricity:HVAC",
+            "reporting_frequency": "RunPeriod"
+        },
+        "Output:Meter:MeterFileOnly 9": {
+            "key_name": "NaturalGas:Facility",
+            "reporting_frequency": "RunPeriod"
+        }
+    },
     "Output:Surfaces:Drawing": {
         "Output:Surfaces:Drawing 1": {
             "report_type": "DXF"
         }
     },
     "Output:Table:SummaryReports": {
         "Output:Table:SummaryReports 1": {
@@ -2335,208 +2424,234 @@
                 }
             ]
         }
     },
     "Output:Variable": {
         "Output:Variable 1": {
             "key_value": "*",
-            "reporting_frequency": "Timestep",
+            "reporting_frequency": "Hourly",
             "variable_name": "Site Outdoor Air Drybulb Temperature"
         },
         "Output:Variable 10": {
-            "key_value": "SPACE1-1",
-            "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermostat Cooling Setpoint Temperature"
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Fan Electricity Rate"
         },
         "Output:Variable 11": {
-            "key_value": "SPACE1-1 PEOPLE 1",
-            "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermal Comfort Fanger Model PMV"
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Heating Coil NaturalGas Rate"
         },
         "Output:Variable 12": {
-            "key_value": "SPACE1-1",
-            "reporting_frequency": "Timestep",
-            "variable_name": "Zone People Occupant Count"
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "People Occupant Count"
         },
         "Output:Variable 13": {
-            "key_value": "SPACE1-1 PEOPLE 1",
-            "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermal Comfort Fanger Model PPD"
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Zone Air Terminal VAV Damper Position"
         },
         "Output:Variable 14": {
-            "key_value": "SPACE1-1 PEOPLE 1",
-            "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermal Comfort Clothing Value"
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Zone Air Terminal Minimum Air Flow Fraction"
         },
         "Output:Variable 15": {
-            "key_value": "SPACE1-1 PEOPLE 1",
-            "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermal Comfort Mean Radiant Temperature"
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Zone Air Terminal Outdoor Air Volume Flow Rate"
         },
         "Output:Variable 16": {
-            "key_value": "*",
-            "reporting_frequency": "Timestep",
-            "variable_name": "People Air Temperature"
+            "key_value": "SPACE1-1 In Node",
+            "reporting_frequency": "Hourly",
+            "variable_name": "System Node Temperature"
         },
         "Output:Variable 17": {
-            "key_value": "*",
-            "reporting_frequency": "Timestep",
-            "variable_name": "Facility Total HVAC Electricity Demand Rate"
+            "key_value": "SPACE2-1 In Node",
+            "reporting_frequency": "Hourly",
+            "variable_name": "System Node Temperature"
         },
         "Output:Variable 18": {
-            "key_value": "SPACE1-1 IN NODE",
-            "reporting_frequency": "Timestep",
+            "key_value": "SPACE3-1 In Node",
+            "reporting_frequency": "Hourly",
             "variable_name": "System Node Temperature"
         },
         "Output:Variable 19": {
-            "key_value": "VAV SYS 1 OUTLET NODE",
-            "reporting_frequency": "Timestep",
+            "key_value": "SPACE4-1 In Node",
+            "reporting_frequency": "Hourly",
             "variable_name": "System Node Temperature"
         },
         "Output:Variable 2": {
             "key_value": "*",
-            "reporting_frequency": "Timestep",
-            "variable_name": "Site Outdoor Air Relative Humidity"
+            "reporting_frequency": "Hourly",
+            "variable_name": "Zone Air Temperature"
         },
         "Output:Variable 20": {
-            "key_value": "SPACE1-1 IN NODE",
-            "reporting_frequency": "Timestep",
-            "variable_name": "System Node Mass Flow Rate"
+            "key_value": "SPACE5-1 In Node",
+            "reporting_frequency": "Hourly",
+            "variable_name": "System Node Temperature"
         },
         "Output:Variable 21": {
-            "key_value": "VAV SYS 1 OUTLET NODE",
-            "reporting_frequency": "Timestep",
-            "variable_name": "System Node Mass Flow Rate"
+            "key_value": "SPACE1-1 In Node",
+            "reporting_frequency": "Hourly",
+            "variable_name": "System Node Standard Density Volume Flow Rate"
+        },
+        "Output:Variable 22": {
+            "key_value": "SPACE2-1 In Node",
+            "reporting_frequency": "Hourly",
+            "variable_name": "System Node Standard Density Volume Flow Rate"
+        },
+        "Output:Variable 23": {
+            "key_value": "SPACE3-1 In Node",
+            "reporting_frequency": "Hourly",
+            "variable_name": "System Node Standard Density Volume Flow Rate"
+        },
+        "Output:Variable 24": {
+            "key_value": "SPACE4-1 In Node",
+            "reporting_frequency": "Hourly",
+            "variable_name": "System Node Standard Density Volume Flow Rate"
+        },
+        "Output:Variable 25": {
+            "key_value": "SPACE5-1 In Node",
+            "reporting_frequency": "Hourly",
+            "variable_name": "System Node Standard Density Volume Flow Rate"
+        },
+        "Output:Variable 26": {
+            "key_value": "SPACE1-1 In Node",
+            "reporting_frequency": "Hourly",
+            "variable_name": "System Node Current Density Volume Flow Rate"
+        },
+        "Output:Variable 27": {
+            "key_value": "SPACE2-1 In Node",
+            "reporting_frequency": "Hourly",
+            "variable_name": "System Node Current Density Volume Flow Rate"
+        },
+        "Output:Variable 28": {
+            "key_value": "SPACE3-1 In Node",
+            "reporting_frequency": "Hourly",
+            "variable_name": "System Node Current Density Volume Flow Rate"
+        },
+        "Output:Variable 29": {
+            "key_value": "SPACE4-1 In Node",
+            "reporting_frequency": "Hourly",
+            "variable_name": "System Node Current Density Volume Flow Rate"
         },
         "Output:Variable 3": {
             "key_value": "*",
-            "reporting_frequency": "Timestep",
-            "variable_name": "Site Wind Speed"
+            "reporting_frequency": "Hourly",
+            "variable_name": "Zone Air System Sensible Cooling Rate"
+        },
+        "Output:Variable 30": {
+            "key_value": "SPACE5-1 In Node",
+            "reporting_frequency": "Hourly",
+            "variable_name": "System Node Current Density Volume Flow Rate"
+        },
+        "Output:Variable 31": {
+            "key_value": "Outside Air Inlet Node 1",
+            "reporting_frequency": "Hourly",
+            "variable_name": "System Node Standard Density Volume Flow Rate"
+        },
+        "Output:Variable 32": {
+            "key_value": "Outside Air Inlet Node 1",
+            "reporting_frequency": "Hourly",
+            "variable_name": "System Node Current Density Volume Flow Rate"
+        },
+        "Output:Variable 33": {
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Air System Outdoor Air Flow Fraction"
         },
         "Output:Variable 4": {
             "key_value": "*",
-            "reporting_frequency": "Timestep",
-            "variable_name": "Site Wind Direction"
+            "reporting_frequency": "Hourly",
+            "variable_name": "Zone Air System Sensible Heating Rate"
         },
         "Output:Variable 5": {
             "key_value": "*",
-            "reporting_frequency": "Timestep",
-            "variable_name": "Site Diffuse Solar Radiation Rate per Area"
+            "reporting_frequency": "Hourly",
+            "variable_name": "Coil System Compressor Speed Ratio"
         },
         "Output:Variable 6": {
             "key_value": "*",
-            "reporting_frequency": "Timestep",
-            "variable_name": "Site Direct Solar Radiation Rate per Area"
+            "reporting_frequency": "Hourly",
+            "variable_name": "Cooling Coil Electricity Rate"
         },
         "Output:Variable 7": {
-            "key_value": "SPACE1-1",
-            "reporting_frequency": "Timestep",
-            "variable_name": "Zone Air Temperature"
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Cooling Coil Runtime Fraction"
         },
         "Output:Variable 8": {
-            "key_value": "SPACE1-1",
-            "reporting_frequency": "Timestep",
-            "variable_name": "Zone Air Relative Humidity"
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Cooling Coil Basin Heater Electricity Rate"
         },
         "Output:Variable 9": {
-            "key_value": "SPACE1-1",
-            "reporting_frequency": "Timestep",
-            "variable_name": "Zone Thermostat Heating Setpoint Temperature"
+            "key_value": "*",
+            "reporting_frequency": "Hourly",
+            "variable_name": "Cooling Coil Basin Heater Electricity Energy"
         }
     },
     "Output:VariableDictionary": {
         "Output:VariableDictionary 1": {
             "key_field": "regular"
         }
     },
     "OutputControl:Table:Style": {
         "OutputControl:Table:Style 1": {
-            "column_separator": "HTML"
+            "column_separator": "HTML",
+            "unit_conversion": "InchPound"
         }
     },
     "People": {
         "SPACE1-1 People 1": {
             "activity_level_schedule_name": "ActSchd",
-            "air_velocity_schedule_name": "AirVelocitySch",
-            "carbon_dioxide_generation_rate": 3.82e-08,
-            "clothing_insulation_calculation_method": "DynamicClothingModelASHRAE55",
-            "enable_ashrae_55_comfort_warnings": "No",
             "fraction_radiant": 0.3,
-            "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people": 11,
             "number_of_people_calculation_method": "People",
             "number_of_people_schedule_name": "OCCUPY-1",
             "sensible_heat_fraction": "Autocalculate",
-            "thermal_comfort_model_1_type": "Fanger",
-            "work_efficiency_schedule_name": "WorkEffSch",
-            "zone_or_zonelist_name": "SPACE1-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE1-1"
         },
         "SPACE2-1 People 1": {
             "activity_level_schedule_name": "ActSchd",
-            "air_velocity_schedule_name": "AirVelocitySch",
-            "carbon_dioxide_generation_rate": 3.82e-08,
-            "clothing_insulation_calculation_method": "DynamicClothingModelASHRAE55",
-            "enable_ashrae_55_comfort_warnings": "No",
             "fraction_radiant": 0.3,
-            "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people": 5,
             "number_of_people_calculation_method": "People",
             "number_of_people_schedule_name": "OCCUPY-1",
             "sensible_heat_fraction": "Autocalculate",
-            "thermal_comfort_model_1_type": "Fanger",
-            "work_efficiency_schedule_name": "WorkEffSch",
-            "zone_or_zonelist_name": "SPACE2-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE2-1"
         },
         "SPACE3-1 People 1": {
             "activity_level_schedule_name": "ActSchd",
-            "air_velocity_schedule_name": "AirVelocitySch",
-            "carbon_dioxide_generation_rate": 3.82e-08,
-            "clothing_insulation_calculation_method": "DynamicClothingModelASHRAE55",
-            "enable_ashrae_55_comfort_warnings": "No",
             "fraction_radiant": 0.3,
-            "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people": 11,
             "number_of_people_calculation_method": "People",
             "number_of_people_schedule_name": "OCCUPY-1",
             "sensible_heat_fraction": "Autocalculate",
-            "thermal_comfort_model_1_type": "Fanger",
-            "work_efficiency_schedule_name": "WorkEffSch",
-            "zone_or_zonelist_name": "SPACE3-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE3-1"
         },
         "SPACE4-1 People 1": {
             "activity_level_schedule_name": "ActSchd",
-            "air_velocity_schedule_name": "AirVelocitySch",
-            "carbon_dioxide_generation_rate": 3.82e-08,
-            "clothing_insulation_calculation_method": "DynamicClothingModelASHRAE55",
-            "enable_ashrae_55_comfort_warnings": "No",
             "fraction_radiant": 0.3,
-            "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people": 5,
             "number_of_people_calculation_method": "People",
             "number_of_people_schedule_name": "OCCUPY-1",
             "sensible_heat_fraction": "Autocalculate",
-            "thermal_comfort_model_1_type": "Fanger",
-            "work_efficiency_schedule_name": "WorkEffSch",
-            "zone_or_zonelist_name": "SPACE4-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE4-1"
         },
         "SPACE5-1 People 1": {
             "activity_level_schedule_name": "ActSchd",
-            "air_velocity_schedule_name": "AirVelocitySch",
-            "carbon_dioxide_generation_rate": 3.82e-08,
-            "clothing_insulation_calculation_method": "DynamicClothingModelASHRAE55",
-            "enable_ashrae_55_comfort_warnings": "No",
             "fraction_radiant": 0.3,
-            "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people": 20,
             "number_of_people_calculation_method": "People",
             "number_of_people_schedule_name": "OCCUPY-1",
             "sensible_heat_fraction": "Autocalculate",
-            "thermal_comfort_model_1_type": "Fanger",
-            "work_efficiency_schedule_name": "WorkEffSch",
-            "zone_or_zonelist_name": "SPACE5-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE5-1"
         }
     },
     "RunPeriod": {
         "RUNPERIOD 1": {
             "apply_weekend_holiday_rule": "No",
             "begin_day_of_month": 1,
             "begin_month": 1,
@@ -2565,50 +2680,40 @@
                 },
                 {
                     "field": 117.239997864
                 }
             ],
             "schedule_type_limits_name": "Any Number"
         },
-        "ActivitySch": {
+        "BasinHeaterSched": {
             "data": [
                 {
-                    "field": "Through: 12/31"
+                    "field": "Through: 1/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 117
-                }
-            ],
-            "schedule_type_limits_name": "Any Number"
-        },
-        "AirVelocitySch": {
-            "data": [
+                    "field": 1.0
+                },
                 {
-                    "field": "Through: 12/31"
+                    "field": "Through: 2/2"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.137
-                }
-            ],
-            "schedule_type_limits_name": "Any Number"
-        },
-        "BasinHeaterSched": {
-            "data": [
+                    "field": 0.0
+                },
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
@@ -2705,68 +2810,81 @@
                 },
                 {
                     "field": 40.0
                 }
             ],
             "schedule_type_limits_name": "Temperature"
         },
-        "ClothingSch": {
+        "CoolingCoilAvailSched": {
             "data": [
                 {
-                    "field": "Through: 4/1"
+                    "field": "Through: 3/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 1
+                    "field": 0.0
                 },
                 {
                     "field": "Through: 9/30"
                 },
                 {
-                    "field": "For: AllDays"
+                    "field": "For: WeekDays"
+                },
+                {
+                    "field": "Until: 7:00"
+                },
+                {
+                    "field": 0.0
+                },
+                {
+                    "field": "Until: 17:00"
+                },
+                {
+                    "field": 1.0
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.5
+                    "field": 0.0
                 },
                 {
-                    "field": "Through: 12/31"
+                    "field": "For: SummerDesignDay WinterDesignDay"
                 },
                 {
-                    "field": "For: AllDays"
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 1.0
+                },
+                {
+                    "field": "For: AllOtherDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 1
-                }
-            ],
-            "schedule_type_limits_name": "Any Number"
-        },
-        "CoolingCoilAvailSched": {
-            "data": [
+                    "field": 0.0
+                },
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 1.0
+                    "field": 0.0
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
         "EQUIP-1": {
             "data": [
                 {
@@ -2834,14 +2952,68 @@
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
         "FanAvailSched": {
             "data": [
                 {
+                    "field": "Through: 3/31"
+                },
+                {
+                    "field": "For: AllDays"
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 1.0
+                },
+                {
+                    "field": "Through: 9/30"
+                },
+                {
+                    "field": "For: WeekDays"
+                },
+                {
+                    "field": "Until: 7:00"
+                },
+                {
+                    "field": 0.0
+                },
+                {
+                    "field": "Until: 17:00"
+                },
+                {
+                    "field": 1.0
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0.0
+                },
+                {
+                    "field": "For: SummerDesignDay WinterDesignDay"
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 1.0
+                },
+                {
+                    "field": "For: AllOtherDays"
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0.0
+                },
+                {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
@@ -3239,14 +3411,68 @@
                 }
             ],
             "schedule_type_limits_name": "Temperature"
         },
         "ReheatCoilAvailSched": {
             "data": [
                 {
+                    "field": "Through: 3/31"
+                },
+                {
+                    "field": "For: AllDays"
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 1.0
+                },
+                {
+                    "field": "Through: 9/30"
+                },
+                {
+                    "field": "For: WeekDays"
+                },
+                {
+                    "field": "Until: 7:00"
+                },
+                {
+                    "field": 0.0
+                },
+                {
+                    "field": "Until: 17:00"
+                },
+                {
+                    "field": 1.0
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0.0
+                },
+                {
+                    "field": "For: SummerDesignDay WinterDesignDay"
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 1.0
+                },
+                {
+                    "field": "For: AllOtherDays"
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0.0
+                },
+                {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
@@ -3311,31 +3537,14 @@
                 },
                 {
                     "field": 0.0
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "WorkEffSch": {
-            "data": [
-                {
-                    "field": "Through: 12/31"
-                },
-                {
-                    "field": "For: AllDays"
-                },
-                {
-                    "field": "Until: 24:00"
-                },
-                {
-                    "field": 0.0
-                }
-            ],
-            "schedule_type_limits_name": "Fraction"
-        },
         "Zone Control Type Sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: SummerDesignDay"
@@ -3402,22 +3611,19 @@
             "control_variable": "Temperature",
             "fan_inlet_node_name": "Main Heating Coil 1 Outlet Node",
             "fan_outlet_node_name": "VAV Sys 1 Outlet Node",
             "reference_setpoint_node_name": "VAV Sys 1 Outlet Node",
             "setpoint_node_or_nodelist_name": "Supply Fan Upstream Nodes"
         }
     },
-    "SetpointManager:Warmest": {
+    "SetpointManager:Scheduled": {
         "Supply Air Temp Manager 1": {
             "control_variable": "Temperature",
-            "hvac_air_loop_name": "VAV Sys 1",
-            "maximum_setpoint_temperature": 18,
-            "minimum_setpoint_temperature": 12,
-            "setpoint_node_or_nodelist_name": "Supply Air Temp Nodes 1",
-            "strategy": "MaximumTemperature"
+            "schedule_name": "Seasonal Reset Supply Air Temp Sch",
+            "setpoint_node_or_nodelist_name": "Supply Air Temp Nodes 1"
         }
     },
     "Shading:Zone:Detailed": {
         "Main South Overhang": {
             "base_surface_name": "FRONT-1",
             "number_of_vertices": 4,
             "transmittance_schedule_name": "ShadeTransSch",
@@ -3496,51 +3702,51 @@
             "may_ground_temperature": 20.43,
             "november_ground_temperature": 20.44,
             "october_ground_temperature": 20.55,
             "september_ground_temperature": 20.78
         }
     },
     "Site:Location": {
-        "Pittsburgh Allegheny Co Ap_PA_USA Design_Conditions": {
-            "elevation": 380.0,
-            "latitude": 40.35,
-            "longitude": -79.92,
-            "time_zone": -5.0
+        "CHICAGO_IL_USA TMY2-94846": {
+            "elevation": 190.0,
+            "latitude": 41.78,
+            "longitude": -87.75,
+            "time_zone": -6.0
         }
     },
     "Sizing:Parameters": {
         "Sizing:Parameters 1": {
-            "cooling_sizing_factor": 1.3,
-            "heating_sizing_factor": 1.3
+            "cooling_sizing_factor": 1.0,
+            "heating_sizing_factor": 1.0
         }
     },
     "Sizing:System": {
         "Sizing:System 1": {
             "100_outdoor_air_in_cooling": "No",
             "100_outdoor_air_in_heating": "No",
             "airloop_name": "VAV Sys 1",
             "central_cooling_capacity_control_method": "VAV",
             "central_cooling_design_supply_air_humidity_ratio": 0.009,
-            "central_cooling_design_supply_air_temperature": 12.0,
+            "central_cooling_design_supply_air_temperature": 16.0,
             "central_heating_design_supply_air_humidity_ratio": 0.009,
             "central_heating_design_supply_air_temperature": 18.0,
-            "central_heating_maximum_system_air_flow_ratio": 1.0,
+            "central_heating_maximum_system_air_flow_ratio": 0.3,
             "cooling_design_capacity": "Autosize",
             "cooling_design_capacity_method": "CoolingDesignCapacity",
             "cooling_supply_air_flow_rate": 0,
             "cooling_supply_air_flow_rate_method": "DesignDay",
             "design_outdoor_air_flow_rate": "Autosize",
             "heating_design_capacity": "Autosize",
             "heating_design_capacity_method": "HeatingDesignCapacity",
             "heating_supply_air_flow_rate": 0,
             "heating_supply_air_flow_rate_method": "DesignDay",
             "precool_design_humidity_ratio": 0.008,
-            "precool_design_temperature": 30.0,
+            "precool_design_temperature": 11.0,
             "preheat_design_humidity_ratio": 0.008,
-            "preheat_design_temperature": -15.0,
+            "preheat_design_temperature": 7.0,
             "type_of_load_to_size_on": "Sensible",
             "type_of_zone_sum_to_use": "NonCoincident",
             "zone_maximum_outdoor_air_fraction": 1.0
         }
     },
     "Sizing:Zone": {
         "Sizing:Zone 1": {
@@ -3554,15 +3760,15 @@
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.009,
             "zone_cooling_design_supply_air_temperature": 16.0,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
             "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.004,
-            "zone_heating_design_supply_air_temperature": 35.0,
+            "zone_heating_design_supply_air_temperature": 50.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
             "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "SPACE1-1"
         },
         "Sizing:Zone 2": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
@@ -3574,15 +3780,15 @@
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.009,
             "zone_cooling_design_supply_air_temperature": 16.0,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
             "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.004,
-            "zone_heating_design_supply_air_temperature": 35.0,
+            "zone_heating_design_supply_air_temperature": 50.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
             "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "SPACE2-1"
         },
         "Sizing:Zone 3": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
@@ -3594,15 +3800,15 @@
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.009,
             "zone_cooling_design_supply_air_temperature": 16.0,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
             "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.004,
-            "zone_heating_design_supply_air_temperature": 35.0,
+            "zone_heating_design_supply_air_temperature": 50.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
             "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "SPACE3-1"
         },
         "Sizing:Zone 4": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
@@ -3614,15 +3820,15 @@
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.009,
             "zone_cooling_design_supply_air_temperature": 16.0,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
             "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.004,
-            "zone_heating_design_supply_air_temperature": 35.0,
+            "zone_heating_design_supply_air_temperature": 50.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
             "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "SPACE4-1"
         },
         "Sizing:Zone 5": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
@@ -3634,57 +3840,54 @@
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.009,
             "zone_cooling_design_supply_air_temperature": 16.0,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
             "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.004,
-            "zone_heating_design_supply_air_temperature": 35.0,
+            "zone_heating_design_supply_air_temperature": 50.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
             "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "SPACE5-1"
         }
     },
     "SizingPeriod:DesignDay": {
-        "Pittsburgh Allegheny Co Ap Ann Clg .4% Condns DB=>MWB": {
-            "ashrae_clear_sky_optical_depth_for_beam_irradiance_taub_": 0.484,
-            "ashrae_clear_sky_optical_depth_for_diffuse_irradiance_taud_": 1.916,
-            "barometric_pressure": 96842.0,
-            "daily_dry_bulb_temperature_range": 9.9,
-            "day_of_month": 21,
+        "CHICAGO_IL_USA Annual Cooling 1% Design Conditions DB/MCWB": {
+            "barometric_pressure": 99063.0,
+            "daily_dry_bulb_temperature_range": 10.7,
+            "day_of_month": 3,
             "day_type": "SummerDesignDay",
             "daylight_saving_time_indicator": "No",
-            "dry_bulb_temperature_range_modifier_type": "DefaultMultipliers",
             "humidity_condition_type": "WetBulb",
-            "maximum_dry_bulb_temperature": 32.2,
+            "maximum_dry_bulb_temperature": 31.5,
             "month": 7,
             "rain_indicator": "No",
+            "sky_clearness": 1.0,
             "snow_indicator": "No",
-            "solar_model_indicator": "ASHRAETau",
-            "wetbulb_or_dewpoint_at_maximum_dry_bulb": 22.5,
-            "wind_direction": 240,
-            "wind_speed": 4.4
+            "solar_model_indicator": "ASHRAEClearSky",
+            "wetbulb_or_dewpoint_at_maximum_dry_bulb": 23.0,
+            "wind_direction": 230,
+            "wind_speed": 5.3
         },
-        "Pittsburgh Allegheny Co Ap Ann Htg 99.6% Condns DB": {
-            "barometric_pressure": 96842.0,
+        "CHICAGO_IL_USA Annual Heating 99% Design Conditions DB": {
+            "barometric_pressure": 99063.0,
             "daily_dry_bulb_temperature_range": 0.0,
-            "day_of_month": 21,
+            "day_of_month": 8,
             "day_type": "WinterDesignDay",
             "daylight_saving_time_indicator": "No",
-            "dry_bulb_temperature_range_modifier_type": "DefaultMultipliers",
             "humidity_condition_type": "WetBulb",
-            "maximum_dry_bulb_temperature": -15.4,
+            "maximum_dry_bulb_temperature": -17.3,
             "month": 1,
             "rain_indicator": "No",
             "sky_clearness": 0.0,
             "snow_indicator": "No",
             "solar_model_indicator": "ASHRAEClearSky",
-            "wetbulb_or_dewpoint_at_maximum_dry_bulb": -15.4,
-            "wind_direction": 240,
-            "wind_speed": 4.7
+            "wetbulb_or_dewpoint_at_maximum_dry_bulb": -17.3,
+            "wind_direction": 270,
+            "wind_speed": 4.9
         }
     },
     "SurfaceConvectionAlgorithm:Inside": {
         "SurfaceConvectionAlgorithm:Inside 1": {
             "algorithm": "Simple"
         }
     },
@@ -3718,15 +3921,15 @@
     "Timestep": {
         "Timestep 1": {
             "number_of_timesteps_per_hour": 4
         }
     },
     "Version": {
         "Version 1": {
-            "version_identifier": "9.5"
+            "version_identifier": "23.1"
         }
     },
     "WindowMaterial:Gas": {
         "AIR 13MM": {
             "gas_type": "Air",
             "thickness": 0.0127
         },
@@ -4037,51 +4240,51 @@
             "constant_term_coefficient": 0,
             "design_flow_rate": 0.0167,
             "design_flow_rate_calculation_method": "Flow/Zone",
             "schedule_name": "INFIL-SCH",
             "temperature_term_coefficient": 0,
             "velocity_squared_term_coefficient": 0,
             "velocity_term_coefficient": 0.2237,
-            "zone_or_zonelist_name": "SPACE1-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE1-1"
         },
         "SPACE2-1 Infil 1": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0.00717,
             "design_flow_rate_calculation_method": "Flow/Zone",
             "schedule_name": "INFIL-SCH",
             "temperature_term_coefficient": 0,
             "velocity_squared_term_coefficient": 0,
             "velocity_term_coefficient": 0.2237,
-            "zone_or_zonelist_name": "SPACE2-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE2-1"
         },
         "SPACE3-1 Infil 1": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0.0167,
             "design_flow_rate_calculation_method": "Flow/Zone",
             "schedule_name": "INFIL-SCH",
             "temperature_term_coefficient": 0,
             "velocity_squared_term_coefficient": 0,
             "velocity_term_coefficient": 0.2237,
-            "zone_or_zonelist_name": "SPACE3-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE3-1"
         },
         "SPACE4-1 Infil 1": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0.00717,
             "design_flow_rate_calculation_method": "Flow/Zone",
             "schedule_name": "INFIL-SCH",
             "temperature_term_coefficient": 0,
             "velocity_squared_term_coefficient": 0,
             "velocity_term_coefficient": 0.2237,
-            "zone_or_zonelist_name": "SPACE4-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE4-1"
         },
         "SPACE5-1 Infil 1": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0.031089,
             "design_flow_rate_calculation_method": "Flow/Zone",
             "schedule_name": "INFIL-SCH",
             "temperature_term_coefficient": 0,
             "velocity_squared_term_coefficient": 0,
             "velocity_term_coefficient": 0.2237,
-            "zone_or_zonelist_name": "SPACE5-1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "SPACE5-1"
         }
     }
 }
```

### Comparing `sinergym-2.4.1/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.epJSON` & `sinergym-2.5.0/sinergym/data/buildings/ASHRAE901_OfficeMedium_STD2019_Denver.epJSON`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8836514561014804%*

 * *Differences: {"'AirLoopHVAC:OutdoorAirSystem'": "{'PACU_VAV_bot_OA': {delete: "*

 * *                                   "['availability_manager_list_name']}, 'PACU_VAV_mid_OA': "*

 * *                                   "{delete: ['availability_manager_list_name']}, "*

 * *                                   "'PACU_VAV_top_OA': {delete: "*

 * *                                   "['availability_manager_list_name']}}",*

 * * "'AirTerminal:SingleDuct:VAV:Reheat'": "{'Core_bottom VAV Box Component': "*

 * *                                        "{'consta […]*

```diff
@@ -40,25 +40,22 @@
         "PACU_VAV_top_OA_Controllers": {
             "controller_1_name": "PACU_VAV_top_OA_Controller",
             "controller_1_object_type": "Controller:OutdoorAir"
         }
     },
     "AirLoopHVAC:OutdoorAirSystem": {
         "PACU_VAV_bot_OA": {
-            "availability_manager_list_name": "PACU_VAV_bot Availability Manager List",
             "controller_list_name": "PACU_VAV_bot_OA_Controllers",
             "outdoor_air_equipment_list_name": "PACU_VAV_bot_OA_Equipment"
         },
         "PACU_VAV_mid_OA": {
-            "availability_manager_list_name": "PACU_VAV_mid Availability Manager List",
             "controller_list_name": "PACU_VAV_mid_OA_Controllers",
             "outdoor_air_equipment_list_name": "PACU_VAV_mid_OA_Equipment"
         },
         "PACU_VAV_top_OA": {
-            "availability_manager_list_name": "PACU_VAV_top Availability Manager List",
             "controller_list_name": "PACU_VAV_top_OA_Controllers",
             "outdoor_air_equipment_list_name": "PACU_VAV_top_OA_Equipment"
         }
     },
     "AirLoopHVAC:OutdoorAirSystem:EquipmentList": {
         "PACU_VAV_bot_OA_Equipment": {
             "component_1_name": "PACU_VAV_bot_OAMixing Box",
@@ -300,230 +297,260 @@
         }
     },
     "AirTerminal:SingleDuct:VAV:Reheat": {
         "Core_bottom VAV Box Component": {
             "air_inlet_node_name": "Core_bottom VAV Box Inlet Node",
             "air_outlet_node_name": "Core_bottom VAV Box Outlet Node",
             "availability_schedule_name": "ALWAYS_ON",
-            "constant_minimum_air_flow_fraction": 0.3,
+            "constant_minimum_air_flow_fraction": 0.147,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "Core_bottom VAV Box Damper Node",
             "damper_heating_action": "Normal",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_fraction_during_reheat": 0.5,
             "maximum_hot_water_or_steam_flow_rate": "Autosize",
+            "maximum_reheat_air_temperature": 40,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "Core_bottom VAV Box Reheat Coil",
             "reheat_coil_object_type": "Coil:Heating:Electric",
             "zone_minimum_air_flow_input_method": "Constant"
         },
         "Core_mid VAV Box Component": {
             "air_inlet_node_name": "Core_mid VAV Box Inlet Node",
             "air_outlet_node_name": "Core_mid VAV Box Outlet Node",
             "availability_schedule_name": "ALWAYS_ON",
-            "constant_minimum_air_flow_fraction": 0.307432099778152,
+            "constant_minimum_air_flow_fraction": 0.256,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "Core_mid VAV Box Damper Node",
             "damper_heating_action": "Normal",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_fraction_during_reheat": 0.5,
             "maximum_hot_water_or_steam_flow_rate": "Autosize",
+            "maximum_reheat_air_temperature": 40,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "Core_mid VAV Box Reheat Coil",
             "reheat_coil_object_type": "Coil:Heating:Electric",
             "zone_minimum_air_flow_input_method": "Constant"
         },
         "Core_top VAV Box Component": {
             "air_inlet_node_name": "Core_top VAV Box Inlet Node",
             "air_outlet_node_name": "Core_top VAV Box Outlet Node",
             "availability_schedule_name": "ALWAYS_ON",
-            "constant_minimum_air_flow_fraction": 0.3,
+            "constant_minimum_air_flow_fraction": 0.25,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "Core_top VAV Box Damper Node",
             "damper_heating_action": "Normal",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_fraction_during_reheat": 0.5,
             "maximum_hot_water_or_steam_flow_rate": "Autosize",
+            "maximum_reheat_air_temperature": 40,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "Core_top VAV Box Reheat Coil",
             "reheat_coil_object_type": "Coil:Heating:Electric",
             "zone_minimum_air_flow_input_method": "Constant"
         },
         "Perimeter_bot_ZN_1 VAV Box Component": {
             "air_inlet_node_name": "Perimeter_bot_ZN_1 VAV Box Inlet Node",
             "air_outlet_node_name": "Perimeter_bot_ZN_1 VAV Box Outlet Node",
             "availability_schedule_name": "ALWAYS_ON",
-            "constant_minimum_air_flow_fraction": 0.3,
+            "constant_minimum_air_flow_fraction": 0.214,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "Perimeter_bot_ZN_1 VAV Box Damper Node",
             "damper_heating_action": "Normal",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_fraction_during_reheat": 0.5,
             "maximum_hot_water_or_steam_flow_rate": "Autosize",
+            "maximum_reheat_air_temperature": 40,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "Perimeter_bot_ZN_1 VAV Box Reheat Coil",
             "reheat_coil_object_type": "Coil:Heating:Electric",
             "zone_minimum_air_flow_input_method": "Constant"
         },
         "Perimeter_bot_ZN_2 VAV Box Component": {
             "air_inlet_node_name": "Perimeter_bot_ZN_2 VAV Box Inlet Node",
             "air_outlet_node_name": "Perimeter_bot_ZN_2 VAV Box Outlet Node",
             "availability_schedule_name": "ALWAYS_ON",
-            "constant_minimum_air_flow_fraction": 0.3,
+            "constant_minimum_air_flow_fraction": 0.122,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "Perimeter_bot_ZN_2 VAV Box Damper Node",
             "damper_heating_action": "Normal",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_fraction_during_reheat": 0.5,
             "maximum_hot_water_or_steam_flow_rate": "Autosize",
+            "maximum_reheat_air_temperature": 40,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "Perimeter_bot_ZN_2 VAV Box Reheat Coil",
             "reheat_coil_object_type": "Coil:Heating:Electric",
             "zone_minimum_air_flow_input_method": "Constant"
         },
         "Perimeter_bot_ZN_3 VAV Box Component": {
             "air_inlet_node_name": "Perimeter_bot_ZN_3 VAV Box Inlet Node",
             "air_outlet_node_name": "Perimeter_bot_ZN_3 VAV Box Outlet Node",
             "availability_schedule_name": "ALWAYS_ON",
-            "constant_minimum_air_flow_fraction": 0.305230058147285,
+            "constant_minimum_air_flow_fraction": 0.241,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "Perimeter_bot_ZN_3 VAV Box Damper Node",
             "damper_heating_action": "Normal",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_fraction_during_reheat": 0.5,
             "maximum_hot_water_or_steam_flow_rate": "Autosize",
+            "maximum_reheat_air_temperature": 40,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "Perimeter_bot_ZN_3 VAV Box Reheat Coil",
             "reheat_coil_object_type": "Coil:Heating:Electric",
             "zone_minimum_air_flow_input_method": "Constant"
         },
         "Perimeter_bot_ZN_4 VAV Box Component": {
             "air_inlet_node_name": "Perimeter_bot_ZN_4 VAV Box Inlet Node",
             "air_outlet_node_name": "Perimeter_bot_ZN_4 VAV Box Outlet Node",
             "availability_schedule_name": "ALWAYS_ON",
-            "constant_minimum_air_flow_fraction": 0.3,
+            "constant_minimum_air_flow_fraction": 0.111,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "Perimeter_bot_ZN_4 VAV Box Damper Node",
             "damper_heating_action": "Normal",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_fraction_during_reheat": 0.5,
             "maximum_hot_water_or_steam_flow_rate": "Autosize",
+            "maximum_reheat_air_temperature": 40,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "Perimeter_bot_ZN_4 VAV Box Reheat Coil",
             "reheat_coil_object_type": "Coil:Heating:Electric",
             "zone_minimum_air_flow_input_method": "Constant"
         },
         "Perimeter_mid_ZN_1 VAV Box Component": {
             "air_inlet_node_name": "Perimeter_mid_ZN_1 VAV Box Inlet Node",
             "air_outlet_node_name": "Perimeter_mid_ZN_1 VAV Box Outlet Node",
             "availability_schedule_name": "ALWAYS_ON",
-            "constant_minimum_air_flow_fraction": 0.3,
+            "constant_minimum_air_flow_fraction": 0.192,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "Perimeter_mid_ZN_1 VAV Box Damper Node",
             "damper_heating_action": "Normal",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_fraction_during_reheat": 0.5,
             "maximum_hot_water_or_steam_flow_rate": "Autosize",
+            "maximum_reheat_air_temperature": 40,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "Perimeter_mid_ZN_1 VAV Box Reheat Coil",
             "reheat_coil_object_type": "Coil:Heating:Electric",
             "zone_minimum_air_flow_input_method": "Constant"
         },
         "Perimeter_mid_ZN_2 VAV Box Component": {
             "air_inlet_node_name": "Perimeter_mid_ZN_2 VAV Box Inlet Node",
             "air_outlet_node_name": "Perimeter_mid_ZN_2 VAV Box Outlet Node",
             "availability_schedule_name": "ALWAYS_ON",
-            "constant_minimum_air_flow_fraction": 0.3,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "Perimeter_mid_ZN_2 VAV Box Damper Node",
             "damper_heating_action": "Normal",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_fraction_during_reheat": 0.5,
             "maximum_hot_water_or_steam_flow_rate": "Autosize",
+            "maximum_reheat_air_temperature": 40,
+            "minimum_air_flow_fraction_schedule_name": "PERIMETER_MID_ZN_2_MDP_Sch",
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "Perimeter_mid_ZN_2 VAV Box Reheat Coil",
             "reheat_coil_object_type": "Coil:Heating:Electric",
-            "zone_minimum_air_flow_input_method": "Constant"
+            "zone_minimum_air_flow_input_method": "Scheduled"
         },
         "Perimeter_mid_ZN_3 VAV Box Component": {
             "air_inlet_node_name": "Perimeter_mid_ZN_3 VAV Box Inlet Node",
             "air_outlet_node_name": "Perimeter_mid_ZN_3 VAV Box Outlet Node",
             "availability_schedule_name": "ALWAYS_ON",
-            "constant_minimum_air_flow_fraction": 0.3,
+            "constant_minimum_air_flow_fraction": 0.216,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "Perimeter_mid_ZN_3 VAV Box Damper Node",
             "damper_heating_action": "Normal",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_fraction_during_reheat": 0.5,
             "maximum_hot_water_or_steam_flow_rate": "Autosize",
+            "maximum_reheat_air_temperature": 40,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "Perimeter_mid_ZN_3 VAV Box Reheat Coil",
             "reheat_coil_object_type": "Coil:Heating:Electric",
             "zone_minimum_air_flow_input_method": "Constant"
         },
         "Perimeter_mid_ZN_4 VAV Box Component": {
             "air_inlet_node_name": "Perimeter_mid_ZN_4 VAV Box Inlet Node",
             "air_outlet_node_name": "Perimeter_mid_ZN_4 VAV Box Outlet Node",
             "availability_schedule_name": "ALWAYS_ON",
-            "constant_minimum_air_flow_fraction": 0.3,
+            "constant_minimum_air_flow_fraction": 0.094,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "Perimeter_mid_ZN_4 VAV Box Damper Node",
             "damper_heating_action": "Normal",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_fraction_during_reheat": 0.5,
             "maximum_hot_water_or_steam_flow_rate": "Autosize",
+            "maximum_reheat_air_temperature": 40,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "Perimeter_mid_ZN_4 VAV Box Reheat Coil",
             "reheat_coil_object_type": "Coil:Heating:Electric",
             "zone_minimum_air_flow_input_method": "Constant"
         },
         "Perimeter_top_ZN_1 VAV Box Component": {
             "air_inlet_node_name": "Perimeter_top_ZN_1 VAV Box Inlet Node",
             "air_outlet_node_name": "Perimeter_top_ZN_1 VAV Box Outlet Node",
             "availability_schedule_name": "ALWAYS_ON",
-            "constant_minimum_air_flow_fraction": 0.3,
+            "constant_minimum_air_flow_fraction": 0.172,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "Perimeter_top_ZN_1 VAV Box Damper Node",
             "damper_heating_action": "Normal",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_fraction_during_reheat": 0.5,
             "maximum_hot_water_or_steam_flow_rate": "Autosize",
+            "maximum_reheat_air_temperature": 40,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "Perimeter_top_ZN_1 VAV Box Reheat Coil",
             "reheat_coil_object_type": "Coil:Heating:Electric",
             "zone_minimum_air_flow_input_method": "Constant"
         },
         "Perimeter_top_ZN_2 VAV Box Component": {
             "air_inlet_node_name": "Perimeter_top_ZN_2 VAV Box Inlet Node",
             "air_outlet_node_name": "Perimeter_top_ZN_2 VAV Box Outlet Node",
             "availability_schedule_name": "ALWAYS_ON",
-            "constant_minimum_air_flow_fraction": 0.3,
+            "constant_minimum_air_flow_fraction": 0.098,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "Perimeter_top_ZN_2 VAV Box Damper Node",
             "damper_heating_action": "Normal",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_fraction_during_reheat": 0.5,
             "maximum_hot_water_or_steam_flow_rate": "Autosize",
+            "maximum_reheat_air_temperature": 40,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "Perimeter_top_ZN_2 VAV Box Reheat Coil",
             "reheat_coil_object_type": "Coil:Heating:Electric",
             "zone_minimum_air_flow_input_method": "Constant"
         },
         "Perimeter_top_ZN_3 VAV Box Component": {
             "air_inlet_node_name": "Perimeter_top_ZN_3 VAV Box Inlet Node",
             "air_outlet_node_name": "Perimeter_top_ZN_3 VAV Box Outlet Node",
             "availability_schedule_name": "ALWAYS_ON",
-            "constant_minimum_air_flow_fraction": 0.3,
+            "constant_minimum_air_flow_fraction": 0.189,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "Perimeter_top_ZN_3 VAV Box Damper Node",
             "damper_heating_action": "Normal",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_fraction_during_reheat": 0.5,
             "maximum_hot_water_or_steam_flow_rate": "Autosize",
+            "maximum_reheat_air_temperature": 40,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "Perimeter_top_ZN_3 VAV Box Reheat Coil",
             "reheat_coil_object_type": "Coil:Heating:Electric",
             "zone_minimum_air_flow_input_method": "Constant"
         },
         "Perimeter_top_ZN_4 VAV Box Component": {
             "air_inlet_node_name": "Perimeter_top_ZN_4 VAV Box Inlet Node",
             "air_outlet_node_name": "Perimeter_top_ZN_4 VAV Box Outlet Node",
             "availability_schedule_name": "ALWAYS_ON",
-            "constant_minimum_air_flow_fraction": 0.3,
+            "constant_minimum_air_flow_fraction": 0.088,
             "convergence_tolerance": 0.001,
             "damper_air_outlet_node_name": "Perimeter_top_ZN_4 VAV Box Damper Node",
             "damper_heating_action": "Normal",
             "maximum_air_flow_rate": "Autosize",
+            "maximum_flow_fraction_during_reheat": 0.5,
             "maximum_hot_water_or_steam_flow_rate": "Autosize",
+            "maximum_reheat_air_temperature": 40,
             "minimum_hot_water_or_steam_flow_rate": 0.0,
             "reheat_coil_name": "Perimeter_top_ZN_4 VAV Box Reheat Coil",
             "reheat_coil_object_type": "Coil:Heating:Electric",
             "zone_minimum_air_flow_input_method": "Constant"
         }
     },
     "AvailabilityManager:NightCycle": {
@@ -978,20 +1005,20 @@
                 {
                     "branch_name": "SHWSys1 Supply Outlet Branch"
                 }
             ]
         }
     },
     "Building": {
-        "Medium Office": {
+        "OfficeMedium": {
             "loads_convergence_tolerance_value": 0.04,
-            "maximum_number_of_warmup_days": 25,
+            "maximum_number_of_warmup_days": 15,
             "minimum_number_of_warmup_days": 6,
             "north_axis": 0.0,
-            "solar_distribution": "FullInteriorAndExterior",
+            "solar_distribution": "MinimalShadowing",
             "temperature_convergence_tolerance_value": 0.2,
             "terrain": "City"
         }
     },
     "BuildingSurface:Detailed": {
         "Building_Roof": {
             "construction_name": "nonres_roof",
@@ -1055,17 +1082,17 @@
                 }
             ],
             "view_factor_to_ground": "Autocalculate",
             "wind_exposure": "NoWind",
             "zone_name": "Core_bottom"
         },
         "Core_bot_ZN_5_Floor": {
-            "construction_name": "ext_slab_8in_with_carpet",
+            "construction_name": "Core_bot_ZN_5_Floor_Ffactor",
             "number_of_vertices": 4,
-            "outside_boundary_condition": "Ground",
+            "outside_boundary_condition": "Adiabatic",
             "sun_exposure": "NoSun",
             "surface_type": "Floor",
             "vertices": [
                 {
                     "vertex_x_coordinate": 45.3375,
                     "vertex_y_coordinate": 28.7006,
                     "vertex_z_coordinate": 0.0
@@ -1776,17 +1803,17 @@
                 }
             ],
             "view_factor_to_ground": "Autocalculate",
             "wind_exposure": "NoWind",
             "zone_name": "Perimeter_bot_ZN_1"
         },
         "Perimeter_bot_ZN_1_Floor": {
-            "construction_name": "ext_slab_8in_with_carpet",
+            "construction_name": "Perimeter_bot_ZN_1_Floor_Ffactor",
             "number_of_vertices": 4,
-            "outside_boundary_condition": "Ground",
+            "outside_boundary_condition": "GroundFCfactorMethod",
             "sun_exposure": "NoSun",
             "surface_type": "Floor",
             "vertices": [
                 {
                     "vertex_x_coordinate": 0.0,
                     "vertex_y_coordinate": 0.0,
                     "vertex_z_coordinate": 0.0
@@ -1906,17 +1933,17 @@
                 }
             ],
             "view_factor_to_ground": "Autocalculate",
             "wind_exposure": "NoWind",
             "zone_name": "Perimeter_bot_ZN_2"
         },
         "Perimeter_bot_ZN_2_Floor": {
-            "construction_name": "ext_slab_8in_with_carpet",
+            "construction_name": "Perimeter_bot_ZN_2_Floor_Ffactor",
             "number_of_vertices": 4,
-            "outside_boundary_condition": "Ground",
+            "outside_boundary_condition": "GroundFCfactorMethod",
             "sun_exposure": "NoSun",
             "surface_type": "Floor",
             "vertices": [
                 {
                     "vertex_x_coordinate": 49.911,
                     "vertex_y_coordinate": 0.0,
                     "vertex_z_coordinate": 0.0
@@ -2036,17 +2063,17 @@
                 }
             ],
             "view_factor_to_ground": "Autocalculate",
             "wind_exposure": "NoWind",
             "zone_name": "Perimeter_bot_ZN_3"
         },
         "Perimeter_bot_ZN_3_Floor": {
-            "construction_name": "ext_slab_8in_with_carpet",
+            "construction_name": "Perimeter_bot_ZN_3_Floor_Ffactor",
             "number_of_vertices": 4,
-            "outside_boundary_condition": "Ground",
+            "outside_boundary_condition": "GroundFCfactorMethod",
             "sun_exposure": "NoSun",
             "surface_type": "Floor",
             "vertices": [
                 {
                     "vertex_x_coordinate": 49.911,
                     "vertex_y_coordinate": 33.2738,
                     "vertex_z_coordinate": 0.0
@@ -2166,17 +2193,17 @@
                 }
             ],
             "view_factor_to_ground": "Autocalculate",
             "wind_exposure": "NoWind",
             "zone_name": "Perimeter_bot_ZN_4"
         },
         "Perimeter_bot_ZN_4_Floor": {
-            "construction_name": "ext_slab_8in_with_carpet",
+            "construction_name": "Perimeter_bot_ZN_4_Floor_Ffactor",
             "number_of_vertices": 4,
-            "outside_boundary_condition": "Ground",
+            "outside_boundary_condition": "GroundFCfactorMethod",
             "sun_exposure": "NoSun",
             "surface_type": "Floor",
             "vertices": [
                 {
                     "vertex_x_coordinate": 0.0,
                     "vertex_y_coordinate": 33.2738,
                     "vertex_z_coordinate": 0.0
@@ -3580,15 +3607,15 @@
             "energy_input_ratio_function_of_temperature_curve_name": "FURNACE_PACU_VAV_CoolCCarrier48TM014_12tons_EIRFT",
             "high_speed_gross_rated_cooling_cop": 3.39928881549157,
             "high_speed_gross_rated_total_cooling_capacity": "Autosize",
             "high_speed_rated_air_flow_rate": "Autosize",
             "high_speed_rated_sensible_heat_ratio": "Autosize",
             "low_speed_energy_input_ratio_function_of_temperature_curve_name": "FURNACE_PACU_VAV_CoolCCarrier48TM014_12tons_EIRFT",
             "low_speed_gross_rated_cooling_cop": 3.39928881549157,
-            "low_speed_gross_rated_sensible_heat_ratio": 0.69,
+            "low_speed_gross_rated_sensible_heat_ratio": "Autosize",
             "low_speed_gross_rated_total_cooling_capacity": "Autosize",
             "low_speed_rated_air_flow_rate": "Autosize",
             "low_speed_total_cooling_capacity_function_of_temperature_curve_name": "FURNACE_PACU_VAV_CoolCCarrier48TM014_12tons_CapFT",
             "part_load_fraction_correlation_curve_name": "FURNACE_PACU_VAV_CoolCIEA_HVAC_BESTEST_9ton-PLR",
             "total_cooling_capacity_function_of_flow_fraction_curve_name": "FURNACE_PACU_VAV_CoolCCarrier48TM014_12tons_FFF",
             "total_cooling_capacity_function_of_temperature_curve_name": "FURNACE_PACU_VAV_CoolCCarrier48TM014_12tons_CapFT"
         },
@@ -3600,15 +3627,15 @@
             "energy_input_ratio_function_of_temperature_curve_name": "FURNACE_PACU_VAV_CoolCCarrier48TM014_12tons_EIRFT",
             "high_speed_gross_rated_cooling_cop": 3.39928881549157,
             "high_speed_gross_rated_total_cooling_capacity": "Autosize",
             "high_speed_rated_air_flow_rate": "Autosize",
             "high_speed_rated_sensible_heat_ratio": "Autosize",
             "low_speed_energy_input_ratio_function_of_temperature_curve_name": "FURNACE_PACU_VAV_CoolCCarrier48TM014_12tons_EIRFT",
             "low_speed_gross_rated_cooling_cop": 3.39928881549157,
-            "low_speed_gross_rated_sensible_heat_ratio": 0.69,
+            "low_speed_gross_rated_sensible_heat_ratio": "Autosize",
             "low_speed_gross_rated_total_cooling_capacity": "Autosize",
             "low_speed_rated_air_flow_rate": "Autosize",
             "low_speed_total_cooling_capacity_function_of_temperature_curve_name": "FURNACE_PACU_VAV_CoolCCarrier48TM014_12tons_CapFT",
             "part_load_fraction_correlation_curve_name": "FURNACE_PACU_VAV_CoolCIEA_HVAC_BESTEST_9ton-PLR",
             "total_cooling_capacity_function_of_flow_fraction_curve_name": "FURNACE_PACU_VAV_CoolCCarrier48TM014_12tons_FFF",
             "total_cooling_capacity_function_of_temperature_curve_name": "FURNACE_PACU_VAV_CoolCCarrier48TM014_12tons_CapFT"
         },
@@ -3620,15 +3647,15 @@
             "energy_input_ratio_function_of_temperature_curve_name": "FURNACE_PACU_VAV_CoolCCarrier48TM014_12tons_EIRFT",
             "high_speed_gross_rated_cooling_cop": 3.39928881549157,
             "high_speed_gross_rated_total_cooling_capacity": "Autosize",
             "high_speed_rated_air_flow_rate": "Autosize",
             "high_speed_rated_sensible_heat_ratio": "Autosize",
             "low_speed_energy_input_ratio_function_of_temperature_curve_name": "FURNACE_PACU_VAV_CoolCCarrier48TM014_12tons_EIRFT",
             "low_speed_gross_rated_cooling_cop": 3.39928881549157,
-            "low_speed_gross_rated_sensible_heat_ratio": 0.69,
+            "low_speed_gross_rated_sensible_heat_ratio": "Autosize",
             "low_speed_gross_rated_total_cooling_capacity": "Autosize",
             "low_speed_rated_air_flow_rate": "Autosize",
             "low_speed_total_cooling_capacity_function_of_temperature_curve_name": "FURNACE_PACU_VAV_CoolCCarrier48TM014_12tons_CapFT",
             "part_load_fraction_correlation_curve_name": "FURNACE_PACU_VAV_CoolCIEA_HVAC_BESTEST_9ton-PLR",
             "total_cooling_capacity_function_of_flow_fraction_curve_name": "FURNACE_PACU_VAV_CoolCCarrier48TM014_12tons_FFF",
             "total_cooling_capacity_function_of_temperature_curve_name": "FURNACE_PACU_VAV_CoolCCarrier48TM014_12tons_CapFT"
         }
@@ -3741,33 +3768,33 @@
         }
     },
     "Coil:Heating:Fuel": {
         "PACU_VAV_bot_HeatC": {
             "air_inlet_node_name": "PACU_VAV_bot_CoolC-PACU_VAV_bot_HeatCNode",
             "air_outlet_node_name": "PACU_VAV_bot_HeatC-PACU_VAV_bot FanNode",
             "availability_schedule_name": "ALWAYS_ON",
-            "burner_efficiency": 0.8,
+            "burner_efficiency": 0.81,
             "fuel_type": "NaturalGas",
             "nominal_capacity": "Autosize",
             "temperature_setpoint_node_name": "PACU_VAV_bot_HeatC-PACU_VAV_bot FanNode"
         },
         "PACU_VAV_mid_HeatC": {
             "air_inlet_node_name": "PACU_VAV_mid_CoolC-PACU_VAV_mid_HeatCNode",
             "air_outlet_node_name": "PACU_VAV_mid_HeatC-PACU_VAV_mid FanNode",
             "availability_schedule_name": "ALWAYS_ON",
-            "burner_efficiency": 0.8,
+            "burner_efficiency": 0.81,
             "fuel_type": "NaturalGas",
             "nominal_capacity": "Autosize",
             "temperature_setpoint_node_name": "PACU_VAV_mid_HeatC-PACU_VAV_mid FanNode"
         },
         "PACU_VAV_top_HeatC": {
             "air_inlet_node_name": "PACU_VAV_top_CoolC-PACU_VAV_top_HeatCNode",
             "air_outlet_node_name": "PACU_VAV_top_HeatC-PACU_VAV_top FanNode",
             "availability_schedule_name": "ALWAYS_ON",
-            "burner_efficiency": 0.8,
+            "burner_efficiency": 0.81,
             "fuel_type": "NaturalGas",
             "nominal_capacity": "Autosize",
             "temperature_setpoint_node_name": "PACU_VAV_top_HeatC-PACU_VAV_top FanNode"
         }
     },
     "CoilSystem:Cooling:DX": {
         "PACU_VAV_bot_CoolC": {
@@ -3957,471 +3984,16 @@
         },
         "OpaqueDoor": {
             "outside_layer": "Std Opaque Door Panel"
         },
         "Swinging Door_con": {
             "outside_layer": "Opaque Door panel_con"
         },
-        "Window_U_0.19_SHGC_0.20": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "COATED POLY-55",
-            "layer_4": "AIR 13MM",
-            "layer_5": "CLEAR 6MM",
-            "outside_layer": "BRONZE 6MM"
-        },
-        "Window_U_0.24_SHGC_0.11": {
-            "layer_2": "ARGON 13MM",
-            "layer_3": "LoE SPEC SEL CLEAR 6MM Rev",
-            "outside_layer": "ECABS-2 COLORED 6MM"
-        },
-        "Window_U_0.24_SHGC_0.16": {
-            "layer_2": "ARGON 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "ECABS-2 COLORED 6MM"
-        },
-        "Window_U_0.24_SHGC_0.23": {
-            "layer_2": "ARGON 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE SPEC SEL TINT 6MM"
-        },
-        "Window_U_0.25_SHGC_0.40": {
-            "layer_2": "ARGON 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE TINT 6MM"
-        },
-        "Window_U_0.29_SHGC_0.11": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "LoE SPEC SEL CLEAR 6MM Rev",
-            "outside_layer": "ECREF-2 COLORED 6MM"
-        },
-        "Window_U_0.29_SHGC_0.17": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "ECABS-2 COLORED 6MM"
-        },
-        "Window_U_0.29_SHGC_0.22": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "COATED POLY-55",
-            "layer_4": "AIR 6MM",
-            "layer_5": "CLEAR 6MM",
-            "outside_layer": "BRONZE 6MM"
-        },
-        "Window_U_0.29_SHGC_0.45": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "LoE SPEC SEL CLEAR 6MM Rev",
-            "outside_layer": "ECREF-2 BLEACHED 6MM"
-        },
-        "Window_U_0.30_SHGC_0.40": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE TINT 6MM"
-        },
-        "Window_U_0.33_SHGC_0.11": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "LoE SPEC SEL CLEAR 6MM Rev",
-            "outside_layer": "ECREF-2 COLORED 6MM"
-        },
-        "Window_U_0.33_SHGC_0.40": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE TINT 6MM"
-        },
-        "Window_U_0.33_SHGC_0.45": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "COATED POLY-77",
-            "layer_4": "AIR 6MM",
-            "layer_5": "CLEAR 3MM",
-            "outside_layer": "CLEAR 3MM"
-        },
-        "Window_U_0.34_SHGC_0.40": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE TINT 6MM"
-        },
-        "Window_U_0.34_SHGC_0.45": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "PYR B CLEAR 6MM"
-        },
-        "Window_U_0.35_SHGC_0.26": {
-            "layer_2": "ARGON 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF C CLEAR MID 6MM"
-        },
-        "Window_U_0.35_SHGC_0.35": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE TINT 6MM"
-        },
-        "Window_U_0.36_SHGC_0.35": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE SPEC SEL TINT 6MM"
-        },
-        "Window_U_0.37_SHGC_0.45": {
-            "layer_2": "Gap_1_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_4321_LayerAvg"
-        },
-        "Window_U_0.38_SHGC_0.26": {
-            "layer_2": "ARGON 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF B TINT HI 6MM"
-        },
-        "Window_U_0.38_SHGC_0.30": {
-            "layer_2": "ARGON 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_0.38_SHGC_0.36": {
-            "layer_2": "Gap_9_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_2531_LayerAvg"
-        },
-        "Window_U_0.38_SHGC_0.41": {
-            "layer_2": "Gap_1_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_4313_LayerAvg"
-        },
-        "Window_U_0.39_SHGC_0.32": {
-            "outside_layer": "Theoretical Glass 347"
-        },
-        "Window_U_0.39_SHGC_0.36": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE TINT 6MM"
-        },
-        "Window_U_0.39_SHGC_0.38": {
-            "outside_layer": "Theoretical Glass 297"
-        },
-        "Window_U_0.39_SHGC_0.40": {
-            "layer_2": "Gap_1_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_282_LayerAvg"
-        },
-        "Window_U_0.40_SHGC_0.38": {
-            "layer_2": "Gap_1_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_8652_LayerAvg"
-        },
-        "Window_U_0.40_SHGC_0.4": {
-            "layer_2": "Gap_1_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_8652_LayerAvg"
-        },
-        "Window_U_0.40_SHGC_0.43": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE SPEC SEL CLEAR 3MM"
-        },
-        "Window_U_0.40_SHGC_0.45": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "LoE SPEC SEL CLEAR 6MM Rev",
-            "outside_layer": "ECABS-2 BLEACHED 6MM"
-        },
-        "Window_U_0.41_SHGC_0.38": {
-            "layer_2": "Gap_1_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_8652_LayerAvg"
-        },
-        "Window_U_0.42_SHGC_0.35": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE TINT 6MM"
-        },
-        "Window_U_0.42_SHGC_0.40": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE TINT 6MM"
-        },
-        "Window_U_0.42_SHGC_0.45": {
-            "layer_2": "ARGON 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF D CLEAR 6MM"
-        },
-        "Window_U_0.43_SHGC_0.26": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_0.43_SHGC_0.29": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE SPEC SEL TINT 6MM"
-        },
-        "Window_U_0.44_SHGC_0.20": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF B TINT HI 6MM"
-        },
-        "Window_U_0.44_SHGC_0.26": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_0.44_SHGC_0.40": {
-            "layer_2": "Gap_9_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_9731_LayerAvg"
-        },
-        "Window_U_0.45_SHGC_0.27": {
-            "layer_2": "Air 13MM",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_12116_LayerAvg"
-        },
-        "Window_U_0.45_SHGC_0.31": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_0.45_SHGC_0.38": {
-            "layer_2": "Gap_1_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_2532_LayerAvg"
-        },
-        "Window_U_0.46_SHGC_0.45": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "GREY 6MM"
-        },
-        "Window_U_0.47_SHGC_0.40": {
-            "layer_2": "Gap_1_W_0_0043",
-            "layer_3": "Glass_2010F_LayerAvg",
-            "outside_layer": "Glass_2052_LayerAvg"
-        },
-        "Window_U_0.48_SHGC_0.40": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF D CLEAR 6MM"
-        },
-        "Window_U_0.50_SHGC_0.25": {
-            "layer_2": "Gap_1_W_0_0042",
-            "layer_3": "Glass_2022F_LayerAvg",
-            "outside_layer": "Glass_2175_LayerAvg"
-        },
-        "Window_U_0.50_SHGC_0.40": {
-            "layer_2": "Gap_1_W_0_0038",
-            "layer_3": "Glass_2027F_LayerAvg",
-            "outside_layer": "Glass_2052_LayerAvg"
-        },
-        "Window_U_0.51_SHGC_0.25": {
-            "layer_2": "Gap_1_W_0_0090",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_1576_LayerAvg"
-        },
-        "Window_U_0.52_SHGC_0.22": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF B CLEAR LO 6MM"
-        },
-        "Window_U_0.52_SHGC_0.40": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF D CLEAR 6MM"
-        },
-        "Window_U_0.54_SHGC_0.13": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF A CLEAR LO 6MM"
-        },
-        "Window_U_0.54_SHGC_0.18": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF A TINT MID 6MM"
-        },
-        "Window_U_0.54_SHGC_0.25": {
-            "layer_2": "Gap_1_W_0_0070",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_1576_LayerAvg"
-        },
-        "Window_U_0.54_SHGC_0.27": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF C CLEAR HI 6MM"
-        },
-        "Window_U_0.55_SHGC_0.25": {
-            "layer_2": "Gap_1_W_0_0032",
-            "layer_3": "Glass_2022F_LayerAvg",
-            "outside_layer": "Glass_2175_LayerAvg"
-        },
-        "Window_U_0.55_SHGC_0.31": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF D TINT 6MM"
-        },
-        "Window_U_0.55_SHGC_0.35": {
-            "layer_2": "Gap_1_W_0_0038",
-            "layer_3": "Glass_2027F_LayerAvg",
-            "outside_layer": "Glass_2052_LayerAvg"
-        },
-        "Window_U_0.56_SHGC_0.25": {
-            "layer_2": "Gap_1_W_0_0060",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_1576_LayerAvg"
-        },
-        "Window_U_0.56_SHGC_0.35": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF D TINT 6MM"
-        },
-        "Window_U_0.56_SHGC_0.76": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 3MM",
-            "outside_layer": "CLEAR 3MM"
-        },
-        "Window_U_0.57_SHGC_0.25": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF C CLEAR HI 6MM"
-        },
-        "Window_U_0.57_SHGC_0.39": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF D CLEAR 6MM"
-        },
-        "Window_U_0.57_SHGC_0.49": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "BLUE 6MM"
-        },
-        "Window_U_0.58_SHGC_0.25": {
-            "layer_2": "Gap_1_W_0_0052",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_1576_LayerAvg"
-        },
-        "Window_U_0.59_SHGC_0.25": {
-            "layer_2": "Gap_1_W_0_0048",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_1576_LayerAvg"
-        },
-        "Window_U_0.60_SHGC_0.25": {
-            "layer_2": "Gap_1_W_0_0025",
-            "layer_3": "Glass_2022F_LayerAvg",
-            "outside_layer": "Glass_2175_LayerAvg"
-        },
-        "Window_U_0.62_SHGC_0.25": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF C CLEAR HI 6MM"
-        },
-        "Window_U_0.62_SHGC_0.39": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF D CLEAR 6MM"
-        },
-        "Window_U_0.62_SHGC_0.49": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "BLUE 6MM"
-        },
-        "Window_U_0.65_SHGC_0.25": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF C CLEAR HI 6MM"
-        },
-        "Window_U_0.65_SHGC_0.35": {
-            "layer_2": "Gap_1_W_0_0024",
-            "layer_3": "Glass_2027F_LayerAvg",
-            "outside_layer": "Glass_2052_LayerAvg"
-        },
-        "Window_U_0.67_SHGC_0.77": {
-            "outside_layer": "PYR B CLEAR 3MM"
-        },
-        "Window_U_0.71_SHGC_0.25": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF C CLEAR HI 6MM"
-        },
-        "Window_U_0.72_SHGC_0.25": {
-            "outside_layer": "REF B TINT MID 6MM"
-        },
-        "Window_U_0.75_SHGC_0.35": {
-            "layer_2": "Gap_1_W_0_0018",
-            "layer_3": "Glass_2027F_LayerAvg",
-            "outside_layer": "Glass_2052_LayerAvg"
-        },
-        "Window_U_0.75_SHGC_0.6": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 3MM",
-            "outside_layer": "GREY 3MM"
-        },
-        "Window_U_0.75_SHGC_0.72": {
-            "outside_layer": "PYR B CLEAR 6MM"
-        },
-        "Window_U_0.85_SHGC_0.78": {
-            "outside_layer": "PYR A CLEAR 3MM"
-        },
-        "Window_U_0.88_SHGC_0.16": {
-            "outside_layer": "REF A CLEAR LO 6MM"
-        },
-        "Window_U_0.88_SHGC_0.27": {
-            "outside_layer": "ECREF-1 COLORED 6MM"
-        },
-        "Window_U_0.90_SHGC_0.40": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_0.98_SHGC_0.45": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_0.98_SHGC_0.68": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_0.9_SHGC_0.6": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_1.05_SHGC_0.40": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_1.08_SHGC_0.25": {
-            "outside_layer": "ECREF-1 COLORED 6MM"
-        },
-        "Window_U_1.15_SHGC_0.68": {
-            "outside_layer": "GREEN 3MM"
-        },
-        "Window_U_1.16_SHGC_0.25": {
-            "outside_layer": "ECREF-1 COLORED 6MM"
-        },
-        "Window_U_1.17_SHGC_0.39": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_1.17_SHGC_0.49": {
-            "outside_layer": "REF D CLEAR 6MM"
-        },
-        "Window_U_1.17_SHGC_0.68": {
-            "outside_layer": "GREEN 3MM"
-        },
-        "Window_U_1.22_SHGC_0.25": {
-            "outside_layer": "ECREF-1 COLORED 6MM"
-        },
-        "Window_U_1.22_SHGC_0.34": {
-            "outside_layer": "REF C CLEAR HI 6MM"
-        },
-        "Window_U_1.22_SHGC_0.39": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_1.22_SHGC_0.61": {
-            "outside_layer": "GREEN 6MM"
-        },
-        "Window_U_1.30_SHGC_0.68": {
-            "outside_layer": "GREEN 3MM"
-        },
-        "Window_U_1.60_SHGC_0.40": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_1.70_SHGC_0.36": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_1.80_SHGC_0.36": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_1.98_SHGC_0.36": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_1.98_SHGC_0.61": {
-            "outside_layer": "GREEN 6MM"
+        "Window_U_0.36_SHGC_0.38": {
+            "outside_layer": "Glazing Layer"
         },
         "basement_wall": {
             "outside_layer": "M10 200mm concrete block basement wall"
         },
         "ext_slab_6in": {
             "outside_layer": "150mm Normalweight concrete floor"
         },
@@ -4516,19 +4088,46 @@
         },
         "semiheated_roof": {
             "layer_2": "Semiheated_Roof_Insulation",
             "layer_3": "F08 Metal surface",
             "outside_layer": "F13 Built-up roofing"
         }
     },
+    "Construction:FfactorGroundFloor": {
+        "Core_bot_ZN_5_Floor_Ffactor": {
+            "area": 983.5365718200002,
+            "f_factor": 0.90012,
+            "perimeterexposed": 0
+        },
+        "Perimeter_bot_ZN_1_Floor_Ffactor": {
+            "area": 207.33814098,
+            "f_factor": 0.90012,
+            "perimeterexposed": 49.911
+        },
+        "Perimeter_bot_ZN_2_Floor_Ffactor": {
+            "area": 131.26219410000022,
+            "f_factor": 0.90012,
+            "perimeterexposed": 33.2738
+        },
+        "Perimeter_bot_ZN_3_Floor_Ffactor": {
+            "area": 207.33814097999993,
+            "f_factor": 0.90012,
+            "perimeterexposed": 49.911
+        },
+        "Perimeter_bot_ZN_4_Floor_Ffactor": {
+            "area": 131.25358392,
+            "f_factor": 0.90012,
+            "perimeterexposed": 33.2738
+        }
+    },
     "Controller:MechanicalVentilation": {
         "PACU_VAV_BOT_DCV": {
             "availability_schedule_name": "MinOA_MotorizedDamper_Sched",
             "demand_controlled_ventilation": "Yes",
-            "system_outdoor_air_method": "VentilationRateProcedure",
+            "system_outdoor_air_method": "Standard62.1VentilationRateProcedureWithLimit",
             "zone_specifications": [
                 {
                     "design_specification_outdoor_air_object_name": "CM DSOA Core_bottom",
                     "design_specification_zone_air_distribution_object_name": "CM DSZAD Core_bottom",
                     "zone_or_zonelist_name": "Core_bottom"
                 },
                 {
@@ -4552,15 +4151,15 @@
                     "zone_or_zonelist_name": "Perimeter_bot_ZN_4"
                 }
             ]
         },
         "PACU_VAV_MID_DCV": {
             "availability_schedule_name": "MinOA_MotorizedDamper_Sched",
             "demand_controlled_ventilation": "Yes",
-            "system_outdoor_air_method": "VentilationRateProcedure",
+            "system_outdoor_air_method": "Standard62.1VentilationRateProcedureWithLimit",
             "zone_specifications": [
                 {
                     "design_specification_outdoor_air_object_name": "CM DSOA Core_mid",
                     "design_specification_zone_air_distribution_object_name": "CM DSZAD Core_mid",
                     "zone_or_zonelist_name": "Core_mid"
                 },
                 {
@@ -4584,15 +4183,15 @@
                     "zone_or_zonelist_name": "Perimeter_mid_ZN_4"
                 }
             ]
         },
         "PACU_VAV_TOP_DCV": {
             "availability_schedule_name": "MinOA_MotorizedDamper_Sched",
             "demand_controlled_ventilation": "Yes",
-            "system_outdoor_air_method": "VentilationRateProcedure",
+            "system_outdoor_air_method": "Standard62.1VentilationRateProcedureWithLimit",
             "zone_specifications": [
                 {
                     "design_specification_outdoor_air_object_name": "CM DSOA Core_top",
                     "design_specification_zone_air_distribution_object_name": "CM DSZAD Core_top",
                     "zone_or_zonelist_name": "Core_top"
                 },
                 {
@@ -4619,53 +4218,62 @@
         }
     },
     "Controller:OutdoorAir": {
         "PACU_VAV_bot_OA_Controller": {
             "actuator_node_name": "PACU_VAV_bot_OAInlet Node",
             "economizer_control_action_type": "ModulateFlow",
             "economizer_control_type": "DifferentialDryBulb",
-            "lockout_type": "NoLockout",
+            "lockout_type": "LockoutWithHeating",
+            "maximum_fraction_of_outdoor_air_schedule_name": "VAV_BOT Max OA Fraction",
             "maximum_outdoor_air_flow_rate": "Autosize",
             "mechanical_ventilation_controller_name": "PACU_VAV_BOT_DCV",
             "minimum_limit_type": "FixedMinimum",
             "minimum_outdoor_air_flow_rate": 0,
             "minimum_outdoor_air_schedule_name": "MinOA_MotorizedDamper_Sched",
             "mixed_air_node_name": "PACU_VAV_bot_OA-PACU_VAV_bot_CoolCNode",
             "relief_air_outlet_node_name": "PACU_VAV_bot_OARelief Node",
             "return_air_node_name": "PACU_VAV_bot Supply Equipment Inlet Node"
         },
         "PACU_VAV_mid_OA_Controller": {
             "actuator_node_name": "PACU_VAV_mid_OAInlet Node",
             "economizer_control_action_type": "ModulateFlow",
             "economizer_control_type": "DifferentialDryBulb",
-            "lockout_type": "NoLockout",
+            "lockout_type": "LockoutWithHeating",
+            "maximum_fraction_of_outdoor_air_schedule_name": "VAV_MID Max OA Fraction",
             "maximum_outdoor_air_flow_rate": "Autosize",
             "mechanical_ventilation_controller_name": "PACU_VAV_MID_DCV",
             "minimum_limit_type": "FixedMinimum",
             "minimum_outdoor_air_flow_rate": 0,
             "minimum_outdoor_air_schedule_name": "MinOA_MotorizedDamper_Sched",
             "mixed_air_node_name": "PACU_VAV_mid_OA-PACU_VAV_mid_CoolCNode",
             "relief_air_outlet_node_name": "PACU_VAV_mid_OARelief Node",
             "return_air_node_name": "PACU_VAV_mid Supply Equipment Inlet Node"
         },
         "PACU_VAV_top_OA_Controller": {
             "actuator_node_name": "PACU_VAV_top_OAInlet Node",
             "economizer_control_action_type": "ModulateFlow",
             "economizer_control_type": "DifferentialDryBulb",
-            "lockout_type": "NoLockout",
+            "lockout_type": "LockoutWithHeating",
+            "maximum_fraction_of_outdoor_air_schedule_name": "VAV_TOP Max OA Fraction",
             "maximum_outdoor_air_flow_rate": "Autosize",
             "mechanical_ventilation_controller_name": "PACU_VAV_TOP_DCV",
             "minimum_limit_type": "FixedMinimum",
             "minimum_outdoor_air_flow_rate": 0,
             "minimum_outdoor_air_schedule_name": "MinOA_MotorizedDamper_Sched",
             "mixed_air_node_name": "PACU_VAV_top_OA-PACU_VAV_top_CoolCNode",
             "relief_air_outlet_node_name": "PACU_VAV_top_OARelief Node",
             "return_air_node_name": "PACU_VAV_top Supply Equipment Inlet Node"
         }
     },
+    "ConvergenceLimits": {
+        "ConvergenceLimits 1": {
+            "maximum_hvac_iterations": 5,
+            "minimum_system_timestep": 15
+        }
+    },
     "Curve:Biquadratic": {
         "FURNACE_PACU_VAV_CoolCCarrier48TM014_12tons_CapFT": {
             "coefficient1_constant": 1.39072,
             "coefficient2_x": -0.0529058,
             "coefficient3_x_2": 0.0018423,
             "coefficient4_y": 0.00058267,
             "coefficient5_y_2": -0.000186814,
@@ -4712,443 +4320,443 @@
         }
     },
     "Daylighting:Controls": {
         "Perimeter_bot_ZN_1_DaylCtrl": {
             "control_data": [
                 {
                     "daylighting_reference_point_name": "Perimeter_bot_ZN_1_DaylRefPt1",
-                    "fraction_of_zone_controlled_by_reference_point": 0.3835,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.3835,
+                    "illuminance_setpoint_at_reference_point": 377
                 },
                 {
                     "daylighting_reference_point_name": "Perimeter_bot_ZN_1_DaylRefPt2",
-                    "fraction_of_zone_controlled_by_reference_point": 0.1395,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.1395,
+                    "illuminance_setpoint_at_reference_point": 377
                 }
             ],
             "daylighting_method": "SplitFlux",
             "glare_calculation_azimuth_angle_of_view_direction_clockwise_from_zone_y_axis": 180.0,
             "glare_calculation_daylighting_reference_point_name": "Perimeter_bot_ZN_1_DaylRefPt1",
-            "lighting_control_type": "Stepped",
+            "lighting_control_type": "ContinuousOff",
             "maximum_allowable_discomfort_glare_index": 22.0,
-            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.3,
+            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "minimum_light_output_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "number_of_stepped_control_steps": 3,
             "probability_lighting_will_be_reset_when_needed_in_manual_stepped_control": 1.0,
-            "zone_name": "Perimeter_bot_ZN_1"
+            "zone_or_space_name": "Perimeter_bot_ZN_1"
         },
         "Perimeter_bot_ZN_2_DaylCtrl": {
             "control_data": [
                 {
                     "daylighting_reference_point_name": "Perimeter_bot_ZN_2_DaylRefPt1",
-                    "fraction_of_zone_controlled_by_reference_point": 0.3835,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.3835,
+                    "illuminance_setpoint_at_reference_point": 377
                 },
                 {
                     "daylighting_reference_point_name": "Perimeter_bot_ZN_2_DaylRefPt2",
-                    "fraction_of_zone_controlled_by_reference_point": 0.1395,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.1395,
+                    "illuminance_setpoint_at_reference_point": 377
                 }
             ],
             "daylighting_method": "SplitFlux",
             "glare_calculation_azimuth_angle_of_view_direction_clockwise_from_zone_y_axis": 90.0,
             "glare_calculation_daylighting_reference_point_name": "Perimeter_bot_ZN_2_DaylRefPt1",
-            "lighting_control_type": "Stepped",
+            "lighting_control_type": "ContinuousOff",
             "maximum_allowable_discomfort_glare_index": 22.0,
-            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.3,
+            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "minimum_light_output_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "number_of_stepped_control_steps": 3,
             "probability_lighting_will_be_reset_when_needed_in_manual_stepped_control": 1.0,
-            "zone_name": "Perimeter_bot_ZN_2"
+            "zone_or_space_name": "Perimeter_bot_ZN_2"
         },
         "Perimeter_bot_ZN_3_DaylCtrl": {
             "control_data": [
                 {
                     "daylighting_reference_point_name": "Perimeter_bot_ZN_3_DaylRefPt1",
-                    "fraction_of_zone_controlled_by_reference_point": 0.3835,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.3835,
+                    "illuminance_setpoint_at_reference_point": 377
                 },
                 {
                     "daylighting_reference_point_name": "Perimeter_bot_ZN_3_DaylRefPt2",
-                    "fraction_of_zone_controlled_by_reference_point": 0.1395,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.1395,
+                    "illuminance_setpoint_at_reference_point": 377
                 }
             ],
             "daylighting_method": "SplitFlux",
             "glare_calculation_azimuth_angle_of_view_direction_clockwise_from_zone_y_axis": 0.0,
             "glare_calculation_daylighting_reference_point_name": "Perimeter_bot_ZN_3_DaylRefPt1",
-            "lighting_control_type": "Stepped",
+            "lighting_control_type": "ContinuousOff",
             "maximum_allowable_discomfort_glare_index": 22.0,
-            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.3,
+            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "minimum_light_output_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "number_of_stepped_control_steps": 3,
             "probability_lighting_will_be_reset_when_needed_in_manual_stepped_control": 1.0,
-            "zone_name": "Perimeter_bot_ZN_3"
+            "zone_or_space_name": "Perimeter_bot_ZN_3"
         },
         "Perimeter_bot_ZN_4_DaylCtrl": {
             "control_data": [
                 {
                     "daylighting_reference_point_name": "Perimeter_bot_ZN_4_DaylRefPt1",
-                    "fraction_of_zone_controlled_by_reference_point": 0.3835,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.3835,
+                    "illuminance_setpoint_at_reference_point": 377
                 },
                 {
                     "daylighting_reference_point_name": "Perimeter_bot_ZN_4_DaylRefPt2",
-                    "fraction_of_zone_controlled_by_reference_point": 0.1395,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.1395,
+                    "illuminance_setpoint_at_reference_point": 377
                 }
             ],
             "daylighting_method": "SplitFlux",
             "glare_calculation_azimuth_angle_of_view_direction_clockwise_from_zone_y_axis": 270.0,
             "glare_calculation_daylighting_reference_point_name": "Perimeter_bot_ZN_4_DaylRefPt1",
-            "lighting_control_type": "Stepped",
+            "lighting_control_type": "ContinuousOff",
             "maximum_allowable_discomfort_glare_index": 22.0,
-            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.3,
+            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "minimum_light_output_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "number_of_stepped_control_steps": 3,
             "probability_lighting_will_be_reset_when_needed_in_manual_stepped_control": 1.0,
-            "zone_name": "Perimeter_bot_ZN_4"
+            "zone_or_space_name": "Perimeter_bot_ZN_4"
         },
         "Perimeter_mid_ZN_1_DaylCtrl": {
             "control_data": [
                 {
                     "daylighting_reference_point_name": "Perimeter_mid_ZN_1_DaylRefPt1",
-                    "fraction_of_zone_controlled_by_reference_point": 0.3835,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.3835,
+                    "illuminance_setpoint_at_reference_point": 377
                 },
                 {
                     "daylighting_reference_point_name": "Perimeter_mid_ZN_1_DaylRefPt2",
-                    "fraction_of_zone_controlled_by_reference_point": 0.1395,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.1395,
+                    "illuminance_setpoint_at_reference_point": 377
                 }
             ],
             "daylighting_method": "SplitFlux",
             "glare_calculation_azimuth_angle_of_view_direction_clockwise_from_zone_y_axis": 180.0,
             "glare_calculation_daylighting_reference_point_name": "Perimeter_mid_ZN_1_DaylRefPt1",
-            "lighting_control_type": "Stepped",
+            "lighting_control_type": "ContinuousOff",
             "maximum_allowable_discomfort_glare_index": 22.0,
-            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.3,
+            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "minimum_light_output_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "number_of_stepped_control_steps": 3,
             "probability_lighting_will_be_reset_when_needed_in_manual_stepped_control": 1.0,
-            "zone_name": "Perimeter_mid_ZN_1"
+            "zone_or_space_name": "Perimeter_mid_ZN_1"
         },
         "Perimeter_mid_ZN_2_DaylCtrl": {
             "control_data": [
                 {
                     "daylighting_reference_point_name": "Perimeter_mid_ZN_2_DaylRefPt1",
-                    "fraction_of_zone_controlled_by_reference_point": 0.3835,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.3835,
+                    "illuminance_setpoint_at_reference_point": 377
                 },
                 {
                     "daylighting_reference_point_name": "Perimeter_mid_ZN_2_DaylRefPt2",
-                    "fraction_of_zone_controlled_by_reference_point": 0.1395,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.1395,
+                    "illuminance_setpoint_at_reference_point": 377
                 }
             ],
             "daylighting_method": "SplitFlux",
             "glare_calculation_azimuth_angle_of_view_direction_clockwise_from_zone_y_axis": 90.0,
             "glare_calculation_daylighting_reference_point_name": "Perimeter_mid_ZN_2_DaylRefPt1",
-            "lighting_control_type": "Stepped",
+            "lighting_control_type": "ContinuousOff",
             "maximum_allowable_discomfort_glare_index": 22.0,
-            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.3,
+            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "minimum_light_output_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "number_of_stepped_control_steps": 3,
             "probability_lighting_will_be_reset_when_needed_in_manual_stepped_control": 1.0,
-            "zone_name": "Perimeter_mid_ZN_2"
+            "zone_or_space_name": "Perimeter_mid_ZN_2"
         },
         "Perimeter_mid_ZN_3_DaylCtrl": {
             "control_data": [
                 {
                     "daylighting_reference_point_name": "Perimeter_mid_ZN_3_DaylRefPt1",
-                    "fraction_of_zone_controlled_by_reference_point": 0.3835,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.3835,
+                    "illuminance_setpoint_at_reference_point": 377
                 },
                 {
                     "daylighting_reference_point_name": "Perimeter_mid_ZN_3_DaylRefPt2",
-                    "fraction_of_zone_controlled_by_reference_point": 0.1395,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.1395,
+                    "illuminance_setpoint_at_reference_point": 377
                 }
             ],
             "daylighting_method": "SplitFlux",
             "glare_calculation_azimuth_angle_of_view_direction_clockwise_from_zone_y_axis": 0.0,
             "glare_calculation_daylighting_reference_point_name": "Perimeter_mid_ZN_3_DaylRefPt1",
-            "lighting_control_type": "Stepped",
+            "lighting_control_type": "ContinuousOff",
             "maximum_allowable_discomfort_glare_index": 22.0,
-            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.3,
+            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "minimum_light_output_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "number_of_stepped_control_steps": 3,
             "probability_lighting_will_be_reset_when_needed_in_manual_stepped_control": 1.0,
-            "zone_name": "Perimeter_mid_ZN_3"
+            "zone_or_space_name": "Perimeter_mid_ZN_3"
         },
         "Perimeter_mid_ZN_4_DaylCtrl": {
             "control_data": [
                 {
                     "daylighting_reference_point_name": "Perimeter_mid_ZN_4_DaylRefPt1",
-                    "fraction_of_zone_controlled_by_reference_point": 0.3835,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.3835,
+                    "illuminance_setpoint_at_reference_point": 377
                 },
                 {
                     "daylighting_reference_point_name": "Perimeter_mid_ZN_4_DaylRefPt2",
-                    "fraction_of_zone_controlled_by_reference_point": 0.1395,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.1395,
+                    "illuminance_setpoint_at_reference_point": 377
                 }
             ],
             "daylighting_method": "SplitFlux",
             "glare_calculation_azimuth_angle_of_view_direction_clockwise_from_zone_y_axis": 270.0,
             "glare_calculation_daylighting_reference_point_name": "Perimeter_mid_ZN_4_DaylRefPt1",
-            "lighting_control_type": "Stepped",
+            "lighting_control_type": "ContinuousOff",
             "maximum_allowable_discomfort_glare_index": 22.0,
-            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.3,
+            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "minimum_light_output_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "number_of_stepped_control_steps": 3,
             "probability_lighting_will_be_reset_when_needed_in_manual_stepped_control": 1.0,
-            "zone_name": "Perimeter_mid_ZN_4"
+            "zone_or_space_name": "Perimeter_mid_ZN_4"
         },
         "Perimeter_top_ZN_1_DaylCtrl": {
             "control_data": [
                 {
                     "daylighting_reference_point_name": "Perimeter_top_ZN_1_DaylRefPt1",
-                    "fraction_of_zone_controlled_by_reference_point": 0.3835,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.3835,
+                    "illuminance_setpoint_at_reference_point": 377
                 },
                 {
                     "daylighting_reference_point_name": "Perimeter_top_ZN_1_DaylRefPt2",
-                    "fraction_of_zone_controlled_by_reference_point": 0.1395,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.1395,
+                    "illuminance_setpoint_at_reference_point": 377
                 }
             ],
             "daylighting_method": "SplitFlux",
             "glare_calculation_azimuth_angle_of_view_direction_clockwise_from_zone_y_axis": 180.0,
             "glare_calculation_daylighting_reference_point_name": "Perimeter_top_ZN_1_DaylRefPt1",
-            "lighting_control_type": "Stepped",
+            "lighting_control_type": "ContinuousOff",
             "maximum_allowable_discomfort_glare_index": 22.0,
-            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.3,
+            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "minimum_light_output_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "number_of_stepped_control_steps": 3,
             "probability_lighting_will_be_reset_when_needed_in_manual_stepped_control": 1.0,
-            "zone_name": "Perimeter_top_ZN_1"
+            "zone_or_space_name": "Perimeter_top_ZN_1"
         },
         "Perimeter_top_ZN_2_DaylCtrl": {
             "control_data": [
                 {
                     "daylighting_reference_point_name": "Perimeter_top_ZN_2_DaylRefPt1",
-                    "fraction_of_zone_controlled_by_reference_point": 0.3835,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.3835,
+                    "illuminance_setpoint_at_reference_point": 377
                 },
                 {
                     "daylighting_reference_point_name": "Perimeter_top_ZN_2_DaylRefPt2",
-                    "fraction_of_zone_controlled_by_reference_point": 0.1395,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.1395,
+                    "illuminance_setpoint_at_reference_point": 377
                 }
             ],
             "daylighting_method": "SplitFlux",
             "glare_calculation_azimuth_angle_of_view_direction_clockwise_from_zone_y_axis": 90.0,
             "glare_calculation_daylighting_reference_point_name": "Perimeter_top_ZN_2_DaylRefPt1",
-            "lighting_control_type": "Stepped",
+            "lighting_control_type": "ContinuousOff",
             "maximum_allowable_discomfort_glare_index": 22.0,
-            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.3,
+            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "minimum_light_output_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "number_of_stepped_control_steps": 3,
             "probability_lighting_will_be_reset_when_needed_in_manual_stepped_control": 1.0,
-            "zone_name": "Perimeter_top_ZN_2"
+            "zone_or_space_name": "Perimeter_top_ZN_2"
         },
         "Perimeter_top_ZN_3_DaylCtrl": {
             "control_data": [
                 {
                     "daylighting_reference_point_name": "Perimeter_top_ZN_3_DaylRefPt1",
-                    "fraction_of_zone_controlled_by_reference_point": 0.3835,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.3835,
+                    "illuminance_setpoint_at_reference_point": 377
                 },
                 {
                     "daylighting_reference_point_name": "Perimeter_top_ZN_3_DaylRefPt2",
-                    "fraction_of_zone_controlled_by_reference_point": 0.1395,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.1395,
+                    "illuminance_setpoint_at_reference_point": 377
                 }
             ],
             "daylighting_method": "SplitFlux",
             "glare_calculation_azimuth_angle_of_view_direction_clockwise_from_zone_y_axis": 0.0,
             "glare_calculation_daylighting_reference_point_name": "Perimeter_top_ZN_3_DaylRefPt1",
-            "lighting_control_type": "Stepped",
+            "lighting_control_type": "ContinuousOff",
             "maximum_allowable_discomfort_glare_index": 22.0,
-            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.3,
+            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "minimum_light_output_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "number_of_stepped_control_steps": 3,
             "probability_lighting_will_be_reset_when_needed_in_manual_stepped_control": 1.0,
-            "zone_name": "Perimeter_top_ZN_3"
+            "zone_or_space_name": "Perimeter_top_ZN_3"
         },
         "Perimeter_top_ZN_4_DaylCtrl": {
             "control_data": [
                 {
                     "daylighting_reference_point_name": "Perimeter_top_ZN_4_DaylRefPt1",
-                    "fraction_of_zone_controlled_by_reference_point": 0.3835,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.3835,
+                    "illuminance_setpoint_at_reference_point": 377
                 },
                 {
                     "daylighting_reference_point_name": "Perimeter_top_ZN_4_DaylRefPt2",
-                    "fraction_of_zone_controlled_by_reference_point": 0.1395,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.1395,
+                    "illuminance_setpoint_at_reference_point": 377
                 }
             ],
             "daylighting_method": "SplitFlux",
             "glare_calculation_azimuth_angle_of_view_direction_clockwise_from_zone_y_axis": 270.0,
             "glare_calculation_daylighting_reference_point_name": "Perimeter_top_ZN_4_DaylRefPt1",
-            "lighting_control_type": "Stepped",
+            "lighting_control_type": "ContinuousOff",
             "maximum_allowable_discomfort_glare_index": 22.0,
-            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.3,
+            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "minimum_light_output_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "number_of_stepped_control_steps": 3,
             "probability_lighting_will_be_reset_when_needed_in_manual_stepped_control": 1.0,
-            "zone_name": "Perimeter_top_ZN_4"
+            "zone_or_space_name": "Perimeter_top_ZN_4"
         }
     },
     "Daylighting:ReferencePoint": {
         "Perimeter_bot_ZN_1_DaylRefPt1": {
             "x_coordinate_of_reference_point": 24.9555,
             "y_coordinate_of_reference_point": 1.524,
             "z_coordinate_of_reference_point": 0.762,
-            "zone_name": "Perimeter_bot_ZN_1"
+            "zone_or_space_name": "Perimeter_bot_ZN_1"
         },
         "Perimeter_bot_ZN_1_DaylRefPt2": {
             "x_coordinate_of_reference_point": 24.9555,
             "y_coordinate_of_reference_point": 3.048,
             "z_coordinate_of_reference_point": 0.762,
-            "zone_name": "Perimeter_bot_ZN_1"
+            "zone_or_space_name": "Perimeter_bot_ZN_1"
         },
         "Perimeter_bot_ZN_2_DaylRefPt1": {
             "x_coordinate_of_reference_point": 48.387,
             "y_coordinate_of_reference_point": 16.6369,
             "z_coordinate_of_reference_point": 0.762,
-            "zone_name": "Perimeter_bot_ZN_2"
+            "zone_or_space_name": "Perimeter_bot_ZN_2"
         },
         "Perimeter_bot_ZN_2_DaylRefPt2": {
             "x_coordinate_of_reference_point": 46.863,
             "y_coordinate_of_reference_point": 16.6369,
             "z_coordinate_of_reference_point": 0.762,
-            "zone_name": "Perimeter_bot_ZN_2"
+            "zone_or_space_name": "Perimeter_bot_ZN_2"
         },
         "Perimeter_bot_ZN_3_DaylRefPt1": {
             "x_coordinate_of_reference_point": 24.9555,
             "y_coordinate_of_reference_point": 31.7498,
             "z_coordinate_of_reference_point": 0.762,
-            "zone_name": "Perimeter_bot_ZN_3"
+            "zone_or_space_name": "Perimeter_bot_ZN_3"
         },
         "Perimeter_bot_ZN_3_DaylRefPt2": {
             "x_coordinate_of_reference_point": 24.9555,
             "y_coordinate_of_reference_point": 30.2258,
             "z_coordinate_of_reference_point": 0.762,
-            "zone_name": "Perimeter_bot_ZN_3"
+            "zone_or_space_name": "Perimeter_bot_ZN_3"
         },
         "Perimeter_bot_ZN_4_DaylRefPt1": {
             "x_coordinate_of_reference_point": 1.524,
             "y_coordinate_of_reference_point": 16.6369,
             "z_coordinate_of_reference_point": 0.762,
-            "zone_name": "Perimeter_bot_ZN_4"
+            "zone_or_space_name": "Perimeter_bot_ZN_4"
         },
         "Perimeter_bot_ZN_4_DaylRefPt2": {
             "x_coordinate_of_reference_point": 3.048,
             "y_coordinate_of_reference_point": 16.6369,
             "z_coordinate_of_reference_point": 0.762,
-            "zone_name": "Perimeter_bot_ZN_4"
+            "zone_or_space_name": "Perimeter_bot_ZN_4"
         },
         "Perimeter_mid_ZN_1_DaylRefPt1": {
             "x_coordinate_of_reference_point": 24.9555,
             "y_coordinate_of_reference_point": 1.524,
             "z_coordinate_of_reference_point": 4.7244,
-            "zone_name": "Perimeter_mid_ZN_1"
+            "zone_or_space_name": "Perimeter_mid_ZN_1"
         },
         "Perimeter_mid_ZN_1_DaylRefPt2": {
             "x_coordinate_of_reference_point": 24.9555,
             "y_coordinate_of_reference_point": 3.048,
             "z_coordinate_of_reference_point": 4.7244,
-            "zone_name": "Perimeter_mid_ZN_1"
+            "zone_or_space_name": "Perimeter_mid_ZN_1"
         },
         "Perimeter_mid_ZN_2_DaylRefPt1": {
             "x_coordinate_of_reference_point": 48.387,
             "y_coordinate_of_reference_point": 16.6369,
             "z_coordinate_of_reference_point": 4.7244,
-            "zone_name": "Perimeter_mid_ZN_2"
+            "zone_or_space_name": "Perimeter_mid_ZN_2"
         },
         "Perimeter_mid_ZN_2_DaylRefPt2": {
             "x_coordinate_of_reference_point": 46.863,
             "y_coordinate_of_reference_point": 16.6369,
             "z_coordinate_of_reference_point": 4.7244,
-            "zone_name": "Perimeter_mid_ZN_2"
+            "zone_or_space_name": "Perimeter_mid_ZN_2"
         },
         "Perimeter_mid_ZN_3_DaylRefPt1": {
             "x_coordinate_of_reference_point": 24.9555,
             "y_coordinate_of_reference_point": 31.7498,
             "z_coordinate_of_reference_point": 4.7244,
-            "zone_name": "Perimeter_mid_ZN_3"
+            "zone_or_space_name": "Perimeter_mid_ZN_3"
         },
         "Perimeter_mid_ZN_3_DaylRefPt2": {
             "x_coordinate_of_reference_point": 24.9555,
             "y_coordinate_of_reference_point": 30.2258,
             "z_coordinate_of_reference_point": 4.7244,
-            "zone_name": "Perimeter_mid_ZN_3"
+            "zone_or_space_name": "Perimeter_mid_ZN_3"
         },
         "Perimeter_mid_ZN_4_DaylRefPt1": {
             "x_coordinate_of_reference_point": 1.524,
             "y_coordinate_of_reference_point": 16.6369,
             "z_coordinate_of_reference_point": 4.7244,
-            "zone_name": "Perimeter_mid_ZN_4"
+            "zone_or_space_name": "Perimeter_mid_ZN_4"
         },
         "Perimeter_mid_ZN_4_DaylRefPt2": {
             "x_coordinate_of_reference_point": 3.048,
             "y_coordinate_of_reference_point": 16.6369,
             "z_coordinate_of_reference_point": 4.7244,
-            "zone_name": "Perimeter_mid_ZN_4"
+            "zone_or_space_name": "Perimeter_mid_ZN_4"
         },
         "Perimeter_top_ZN_1_DaylRefPt1": {
             "x_coordinate_of_reference_point": 24.9555,
             "y_coordinate_of_reference_point": 1.524,
             "z_coordinate_of_reference_point": 8.687,
-            "zone_name": "Perimeter_top_ZN_1"
+            "zone_or_space_name": "Perimeter_top_ZN_1"
         },
         "Perimeter_top_ZN_1_DaylRefPt2": {
             "x_coordinate_of_reference_point": 24.9555,
             "y_coordinate_of_reference_point": 3.048,
             "z_coordinate_of_reference_point": 8.687,
-            "zone_name": "Perimeter_top_ZN_1"
+            "zone_or_space_name": "Perimeter_top_ZN_1"
         },
         "Perimeter_top_ZN_2_DaylRefPt1": {
             "x_coordinate_of_reference_point": 48.387,
             "y_coordinate_of_reference_point": 16.6369,
             "z_coordinate_of_reference_point": 8.687,
-            "zone_name": "Perimeter_top_ZN_2"
+            "zone_or_space_name": "Perimeter_top_ZN_2"
         },
         "Perimeter_top_ZN_2_DaylRefPt2": {
             "x_coordinate_of_reference_point": 46.863,
             "y_coordinate_of_reference_point": 16.6369,
             "z_coordinate_of_reference_point": 8.687,
-            "zone_name": "Perimeter_top_ZN_2"
+            "zone_or_space_name": "Perimeter_top_ZN_2"
         },
         "Perimeter_top_ZN_3_DaylRefPt1": {
             "x_coordinate_of_reference_point": 24.9555,
             "y_coordinate_of_reference_point": 31.7498,
             "z_coordinate_of_reference_point": 8.687,
-            "zone_name": "Perimeter_top_ZN_3"
+            "zone_or_space_name": "Perimeter_top_ZN_3"
         },
         "Perimeter_top_ZN_3_DaylRefPt2": {
             "x_coordinate_of_reference_point": 24.9555,
             "y_coordinate_of_reference_point": 30.2258,
             "z_coordinate_of_reference_point": 8.687,
-            "zone_name": "Perimeter_top_ZN_3"
+            "zone_or_space_name": "Perimeter_top_ZN_3"
         },
         "Perimeter_top_ZN_4_DaylRefPt1": {
             "x_coordinate_of_reference_point": 1.524,
             "y_coordinate_of_reference_point": 16.6369,
             "z_coordinate_of_reference_point": 8.687,
-            "zone_name": "Perimeter_top_ZN_4"
+            "zone_or_space_name": "Perimeter_top_ZN_4"
         },
         "Perimeter_top_ZN_4_DaylRefPt2": {
             "x_coordinate_of_reference_point": 3.048,
             "y_coordinate_of_reference_point": 16.6369,
             "z_coordinate_of_reference_point": 8.687,
-            "zone_name": "Perimeter_top_ZN_4"
+            "zone_or_space_name": "Perimeter_top_ZN_4"
         }
     },
     "DesignSpecification:OutdoorAir": {
         "CM DSOA Core_bottom": {
             "outdoor_air_flow_per_person": 1e-08,
             "outdoor_air_flow_per_zone_floor_area": 0.000431773,
             "outdoor_air_method": "Sum"
@@ -5186,16 +4794,18 @@
         "CM DSOA Perimeter_mid_ZN_1": {
             "outdoor_air_flow_per_person": 1e-08,
             "outdoor_air_flow_per_zone_floor_area": 0.000431773,
             "outdoor_air_method": "Sum"
         },
         "CM DSOA Perimeter_mid_ZN_2": {
             "outdoor_air_flow_per_person": 1e-08,
+            "outdoor_air_flow_per_zone": 0.0,
             "outdoor_air_flow_per_zone_floor_area": 0.000431773,
-            "outdoor_air_method": "Sum"
+            "outdoor_air_method": "Sum",
+            "outdoor_air_schedule_name": "PERIMETER_MID_ZN_2_OA_Mult"
         },
         "CM DSOA Perimeter_mid_ZN_3": {
             "outdoor_air_flow_per_person": 1e-08,
             "outdoor_air_flow_per_zone_floor_area": 0.000431773,
             "outdoor_air_method": "Sum"
         },
         "CM DSOA Perimeter_mid_ZN_4": {
@@ -5262,15 +4872,16 @@
             "outdoor_air_flow_per_zone": 0.0,
             "outdoor_air_flow_per_zone_floor_area": 0.000431773,
             "outdoor_air_method": "Flow/Area"
         },
         "SZ DSOA Perimeter_mid_ZN_2": {
             "outdoor_air_flow_per_zone": 0.0,
             "outdoor_air_flow_per_zone_floor_area": 0.000431773,
-            "outdoor_air_method": "Flow/Area"
+            "outdoor_air_method": "Flow/Area",
+            "outdoor_air_schedule_name": "PERIMETER_MID_ZN_2_OA_Mult"
         },
         "SZ DSOA Perimeter_mid_ZN_3": {
             "outdoor_air_flow_per_zone": 0.0,
             "outdoor_air_flow_per_zone_floor_area": 0.000431773,
             "outdoor_air_method": "Flow/Area"
         },
         "SZ DSOA Perimeter_mid_ZN_4": {
@@ -5355,186 +4966,191 @@
         "CM DSZAD Perimeter_top_ZN_3": {
             "zone_air_distribution_effectiveness_in_cooling_mode": 1,
             "zone_air_distribution_effectiveness_in_heating_mode": 1
         },
         "CM DSZAD Perimeter_top_ZN_4": {
             "zone_air_distribution_effectiveness_in_cooling_mode": 1,
             "zone_air_distribution_effectiveness_in_heating_mode": 1
+        },
+        "VAV_Zone_AirDistribution": {
+            "minimum_zone_ventilation_efficiency": 0.6,
+            "zone_air_distribution_effectiveness_in_cooling_mode": 1,
+            "zone_air_distribution_effectiveness_in_heating_mode": 1
         }
     },
     "ElectricEquipment": {
         "Core_bottom_Elevators_Equip": {
             "design_level": 32109.8901098901,
             "design_level_calculation_method": "EquipmentLevel",
-            "end_use_subcategory": "MiscPlug",
+            "end_use_subcategory": "ElevatorLift",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_ELEVATORS",
-            "zone_or_zonelist_name": "Core_bottom"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_bottom"
         },
         "Core_bottom_MiscPlug_Equip": {
             "design_level": 7937.1558,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "MiscPlug",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "Core_bottom"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_bottom"
         },
         "Core_mid_MiscPlug_Equip": {
             "design_level": 7937.1558,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "MiscPlug",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "Core_mid"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_mid"
         },
         "Core_top_MiscPlug_Equip": {
             "design_level": 7937.1558,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "MiscPlug",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "Core_top"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_top"
         },
         "Elevators_Lights_Fan": {
             "design_level": 125,
             "design_level_calculation_method": "EquipmentLevel",
-            "end_use_subcategory": "MiscPlug",
+            "end_use_subcategory": "ElevatorLightsFan",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "ELEV_LIGHT_FAN_SCH_ADD_DF",
-            "zone_or_zonelist_name": "Core_bottom"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_bottom"
         },
         "Perimeter_bot_ZN_1_MiscPlug_Equip": {
             "design_level": 1673.2028,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "MiscPlug",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_1"
         },
         "Perimeter_bot_ZN_2_MiscPlug_Equip": {
             "design_level": 1059.217,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "MiscPlug",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_2"
         },
         "Perimeter_bot_ZN_3_MiscPlug_Equip": {
             "design_level": 1673.2138,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "MiscPlug",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_3"
         },
         "Perimeter_bot_ZN_4_MiscPlug_Equip": {
             "design_level": 1059.21,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "MiscPlug",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_4"
         },
         "Perimeter_mid_ZN_1_MiscPlug_Equip": {
             "design_level": 1673.2028,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "MiscPlug",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_1"
         },
         "Perimeter_mid_ZN_2_MiscPlug_Equip": {
             "design_level": 1059.217,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "MiscPlug",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_2"
         },
         "Perimeter_mid_ZN_3_MiscPlug_Equip": {
             "design_level": 1673.2138,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "MiscPlug",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_3"
         },
         "Perimeter_mid_ZN_4_MiscPlug_Equip": {
             "design_level": 1059.21,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "MiscPlug",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_4"
         },
         "Perimeter_top_ZN_1_MiscPlug_Equip": {
             "design_level": 1673.2028,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "MiscPlug",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "Perimeter_top_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_1"
         },
         "Perimeter_top_ZN_2_MiscPlug_Equip": {
             "design_level": 1059.217,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "MiscPlug",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "Perimeter_top_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_2"
         },
         "Perimeter_top_ZN_3_MiscPlug_Equip": {
             "design_level": 1673.2138,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "MiscPlug",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "Perimeter_top_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_3"
         },
         "Perimeter_top_ZN_4_MiscPlug_Equip": {
             "design_level": 1059.21,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "MiscPlug",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "Perimeter_top_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_4"
         }
     },
     "ElectricLoadCenter:Transformer": {
         "Transformer 1": {
             "availability_schedule_name": "Always_On",
             "conductor_material": "Aluminum",
             "consider_transformer_loss_for_utility_cost": "Yes",
@@ -5559,14 +5175,19 @@
     },
     "EnergyManagementSystem:Actuator": {
         "CLGSETP_SCH_Actuator": {
             "actuated_component_control_type": "Schedule Value",
             "actuated_component_type": "Schedule:Compact",
             "actuated_component_unique_name": "CLGSETP_SCH_Yes_Optimum"
         },
+        "CLGSETP_SCH_w_SB_Actuator": {
+            "actuated_component_control_type": "Schedule Value",
+            "actuated_component_type": "Schedule:Compact",
+            "actuated_component_unique_name": "CLGSETP_SCH_Yes_Optimum_w_SB"
+        },
         "Core_bottom_Light_Actuator": {
             "actuated_component_control_type": "Electricity Rate",
             "actuated_component_type": "Lights",
             "actuated_component_unique_name": "Core_bottom_lights"
         },
         "Core_mid_Light_Actuator": {
             "actuated_component_control_type": "Electricity Rate",
@@ -5579,14 +5200,19 @@
             "actuated_component_unique_name": "Core_top_lights"
         },
         "HTGSETP_SCH_Actuator": {
             "actuated_component_control_type": "Schedule Value",
             "actuated_component_type": "Schedule:Compact",
             "actuated_component_unique_name": "HTGSETP_SCH_Yes_Optimum"
         },
+        "HTGSETP_SCH_w_SB_Actuator": {
+            "actuated_component_control_type": "Schedule Value",
+            "actuated_component_type": "Schedule:Compact",
+            "actuated_component_unique_name": "HTGSETP_SCH_Yes_Optimum_w_SB"
+        },
         "Perimeter_bot_ZN_1_Light_Actuator": {
             "actuated_component_control_type": "Electricity Rate",
             "actuated_component_type": "Lights",
             "actuated_component_unique_name": "Perimeter_bot_ZN_1_lights"
         },
         "Perimeter_bot_ZN_2_Light_Actuator": {
             "actuated_component_control_type": "Electricity Rate",
@@ -5732,32 +5358,50 @@
                 {
                     "program_line": "SET CLGSETP_SCH_Actuator = 26.7"
                 },
                 {
                     "program_line": "SET HTGSETP_SCH_Actuator = 15.6"
                 },
                 {
+                    "program_line": "SET CLGSETP_SCH_w_SB_Actuator = 26.7"
+                },
+                {
+                    "program_line": "SET HTGSETP_SCH_w_SB_Actuator = 15.6"
+                },
+                {
                     "program_line": "ELSEIF DaylightSavings==1 && DayOfWeek>1 && Hour==4 && OAT<23.9 && OAT>1.7"
                 },
                 {
                     "program_line": "SET CLGSETP_SCH_Actuator = 26.7"
                 },
                 {
                     "program_line": "SET HTGSETP_SCH_Actuator = 15.6"
                 },
                 {
+                    "program_line": "SET CLGSETP_SCH_w_SB_Actuator = 26.7"
+                },
+                {
+                    "program_line": "SET HTGSETP_SCH_w_SB_Actuator = 15.6"
+                },
+                {
                     "program_line": "ELSE"
                 },
                 {
                     "program_line": "SET CLGSETP_SCH_Actuator = NULL"
                 },
                 {
                     "program_line": "SET HTGSETP_SCH_Actuator = NULL"
                 },
                 {
+                    "program_line": "SET CLGSETP_SCH_w_SB_Actuator = NULL"
+                },
+                {
+                    "program_line": "SET HTGSETP_SCH_w_SB_Actuator = NULL"
+                },
+                {
                     "program_line": "ENDIF"
                 }
             ]
         },
         "SET_Core_bottom_Light_EMS_Program": {
             "lines": [
                 {
@@ -5939,24 +5583,42 @@
                 {
                     "program_line": "SET Perimeter_mid_ZN_2_LSr_IP =0.093*Perimeter_mid_ZN_2_LSr/Perimeter_mid_ZN_2_Area"
                 },
                 {
                     "program_line": "IF (Perimeter_mid_ZN_2_Occ_Sensor <= 0) && (Perimeter_mid_ZN_2_LSr_IP >= 0.02)"
                 },
                 {
+                    "program_line": "IF (DaylightSavings==0) && ((Hour < 7) || (Hour > 16))"
+                },
+                {
+                    "program_line": "SET Perimeter_mid_ZN_2_Light_Actuator = 0.02*Perimeter_mid_ZN_2_Area/0.09290304"
+                },
+                {
+                    "program_line": "ELSEIF (DaylightSavings==1) && ((Hour < 6) || (Hour > 15))"
+                },
+                {
                     "program_line": "SET Perimeter_mid_ZN_2_Light_Actuator = 0.02*Perimeter_mid_ZN_2_Area/0.09290304"
                 },
                 {
                     "program_line": "ELSE"
                 },
                 {
                     "program_line": "SET Perimeter_mid_ZN_2_Light_Actuator = NULL"
                 },
                 {
                     "program_line": "ENDIF"
+                },
+                {
+                    "program_line": "ELSE"
+                },
+                {
+                    "program_line": "SET Perimeter_mid_ZN_2_Light_Actuator = NULL"
+                },
+                {
+                    "program_line": "ENDIF"
                 }
             ]
         },
         "SET_Perimeter_mid_ZN_3_Light_EMS_Program": {
             "lines": [
                 {
                     "program_line": "SET Perimeter_mid_ZN_3_LSr_IP =0.093*Perimeter_mid_ZN_3_LSr/Perimeter_mid_ZN_3_Area"
@@ -6357,14 +6019,50 @@
         "Perimeter_top_ZN_4_LSr": {
             "output_variable_or_output_meter_index_key_name": "Perimeter_top_ZN_4",
             "output_variable_or_output_meter_name": "Zone Lights Electricity Rate"
         },
         "Perimeter_top_ZN_4_Occ_Sensor": {
             "output_variable_or_output_meter_index_key_name": "Perimeter_top_ZN_4",
             "output_variable_or_output_meter_name": "People Occupant Count"
+        },
+        "VAV_bot_OA": {
+            "output_variable_or_output_meter_index_key_name": "PACU_VAV_bot",
+            "output_variable_or_output_meter_name": "Air System Outdoor Air Mass Flow Rate"
+        },
+        "VAV_bot_OA_VRP": {
+            "output_variable_or_output_meter_index_key_name": "PACU_VAV_bot",
+            "output_variable_or_output_meter_name": "Air System Outdoor Air Mechanical Ventilation Requested Mass Flow Rate"
+        },
+        "VAV_bot_SUPPLY_FLOW": {
+            "output_variable_or_output_meter_index_key_name": "PACU_VAV_bot_OA-PACU_VAV_bot_CoolCNode",
+            "output_variable_or_output_meter_name": "System Node Standard Density Volume Flow Rate"
+        },
+        "VAV_mid_OA": {
+            "output_variable_or_output_meter_index_key_name": "PACU_VAV_mid",
+            "output_variable_or_output_meter_name": "Air System Outdoor Air Mass Flow Rate"
+        },
+        "VAV_mid_OA_VRP": {
+            "output_variable_or_output_meter_index_key_name": "PACU_VAV_mid",
+            "output_variable_or_output_meter_name": "Air System Outdoor Air Mechanical Ventilation Requested Mass Flow Rate"
+        },
+        "VAV_mid_SUPPLY_FLOW": {
+            "output_variable_or_output_meter_index_key_name": "PACU_VAV_mid_OA-PACU_VAV_mid_CoolCNode",
+            "output_variable_or_output_meter_name": "System Node Standard Density Volume Flow Rate"
+        },
+        "VAV_top_OA": {
+            "output_variable_or_output_meter_index_key_name": "PACU_VAV_top",
+            "output_variable_or_output_meter_name": "Air System Outdoor Air Mass Flow Rate"
+        },
+        "VAV_top_OA_VRP": {
+            "output_variable_or_output_meter_index_key_name": "PACU_VAV_top",
+            "output_variable_or_output_meter_name": "Air System Outdoor Air Mechanical Ventilation Requested Mass Flow Rate"
+        },
+        "VAV_top_SUPPLY_FLOW": {
+            "output_variable_or_output_meter_index_key_name": "PACU_VAV_top_OA-PACU_VAV_top_CoolCNode",
+            "output_variable_or_output_meter_name": "System Node Standard Density Volume Flow Rate"
         }
     },
     "Exterior:Lights": {
         "Exterior_Lights_a": {
             "control_option": "AstronomicalClock",
             "design_level": 519.2,
             "end_use_subcategory": "General",
@@ -6408,19 +6106,19 @@
             "fan_power_coefficient_1": 0.0408,
             "fan_power_coefficient_2": 0.088,
             "fan_power_coefficient_3": -0.0729,
             "fan_power_coefficient_4": 0.9437,
             "fan_power_coefficient_5": 0,
             "fan_power_minimum_flow_fraction": 0.25,
             "fan_power_minimum_flow_rate_input_method": "Fraction",
-            "fan_total_efficiency": 0.6045,
+            "fan_total_efficiency": 0.6006,
             "maximum_flow_rate": "Autosize",
-            "motor_efficiency": 0.93,
+            "motor_efficiency": 0.924,
             "motor_in_airstream_fraction": 1.0,
-            "pressure_rise": 1389.42
+            "pressure_rise": 1314.72
         },
         "PACU_VAV_top Fan": {
             "air_inlet_node_name": "PACU_VAV_top_HeatC-PACU_VAV_top FanNode",
             "air_outlet_node_name": "PACU_VAV_top Supply Equipment Outlet Node",
             "availability_schedule_name": "HVACOperationSchd",
             "fan_power_coefficient_1": 0.0408,
             "fan_power_coefficient_2": 0.088,
@@ -6471,67 +6169,67 @@
             "vertex_3_z_coordinate": 0.0,
             "vertex_4_x_coordinate": 33.925703488322,
             "vertex_4_y_coordinate": 0.0,
             "vertex_4_z_coordinate": 2.1336
         },
         "Perimeter_bot_ZN_1_Wall_South_Window1": {
             "building_surface_name": "Perimeter_bot_ZN_1_Wall_South",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 0.0,
             "vertex_1_y_coordinate": 0.0,
             "vertex_1_z_coordinate": 2.3293,
             "vertex_2_x_coordinate": 0.0,
             "vertex_2_y_coordinate": 0.0,
-            "vertex_2_z_coordinate": 0.954652,
+            "vertex_2_z_coordinate": 0.95455007488,
             "vertex_3_x_coordinate": 15.8242,
             "vertex_3_y_coordinate": 0.0,
-            "vertex_3_z_coordinate": 0.954652,
+            "vertex_3_z_coordinate": 0.95455007488,
             "vertex_4_x_coordinate": 15.8242,
             "vertex_4_y_coordinate": 0.0,
             "vertex_4_z_coordinate": 2.3293,
             "view_factor_to_ground": "Autocalculate"
         },
         "Perimeter_bot_ZN_1_Wall_South_Window2": {
             "building_surface_name": "Perimeter_bot_ZN_1_Wall_South",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 17.0434,
             "vertex_1_y_coordinate": 0.0,
             "vertex_1_z_coordinate": 2.3293,
             "vertex_2_x_coordinate": 17.0434,
             "vertex_2_y_coordinate": 0.0,
-            "vertex_2_z_coordinate": 0.954652,
+            "vertex_2_z_coordinate": 0.95455007488,
             "vertex_3_x_coordinate": 32.8676,
             "vertex_3_y_coordinate": 0.0,
-            "vertex_3_z_coordinate": 0.954652,
+            "vertex_3_z_coordinate": 0.95455007488,
             "vertex_4_x_coordinate": 32.8676,
             "vertex_4_y_coordinate": 0.0,
             "vertex_4_z_coordinate": 2.3293,
             "view_factor_to_ground": "Autocalculate"
         },
         "Perimeter_bot_ZN_1_Wall_South_Window3": {
             "building_surface_name": "Perimeter_bot_ZN_1_Wall_South",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 34.0868,
             "vertex_1_y_coordinate": 0.0,
             "vertex_1_z_coordinate": 2.3293,
             "vertex_2_x_coordinate": 34.0868,
             "vertex_2_y_coordinate": 0.0,
-            "vertex_2_z_coordinate": 0.954652,
+            "vertex_2_z_coordinate": 0.95455007488,
             "vertex_3_x_coordinate": 49.91,
             "vertex_3_y_coordinate": 0.0,
-            "vertex_3_z_coordinate": 0.954652,
+            "vertex_3_z_coordinate": 0.95455007488,
             "vertex_4_x_coordinate": 49.91,
             "vertex_4_y_coordinate": 0.0,
             "vertex_4_z_coordinate": 2.3293,
             "view_factor_to_ground": "Autocalculate"
         },
         "Perimeter_bot_ZN_2_Wall_East_Door": {
             "building_surface_name": "Perimeter_bot_ZN_2_Wall_East",
@@ -6549,47 +6247,47 @@
             "vertex_3_z_coordinate": 0.0,
             "vertex_4_x_coordinate": 49.911,
             "vertex_4_y_coordinate": 31.899598503573,
             "vertex_4_z_coordinate": 2.1336
         },
         "Perimeter_bot_ZN_2_Wall_East_Window1": {
             "building_surface_name": "Perimeter_bot_ZN_2_Wall_East",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 49.911,
             "vertex_1_y_coordinate": 0.0,
             "vertex_1_z_coordinate": 2.3293,
             "vertex_2_x_coordinate": 49.911,
             "vertex_2_y_coordinate": 0.0,
-            "vertex_2_z_coordinate": 0.971924,
+            "vertex_2_z_coordinate": 0.97196720032,
             "vertex_3_x_coordinate": 49.911,
             "vertex_3_y_coordinate": 30.8353,
-            "vertex_3_z_coordinate": 0.971924,
+            "vertex_3_z_coordinate": 0.97196720032,
             "vertex_4_x_coordinate": 49.911,
             "vertex_4_y_coordinate": 30.8353,
             "vertex_4_z_coordinate": 2.3293,
             "view_factor_to_ground": "Autocalculate"
         },
         "Perimeter_bot_ZN_2_Wall_East_Window2": {
             "building_surface_name": "Perimeter_bot_ZN_2_Wall_East",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 49.911,
             "vertex_1_y_coordinate": 32.0545,
             "vertex_1_z_coordinate": 2.3293,
             "vertex_2_x_coordinate": 49.911,
             "vertex_2_y_coordinate": 32.0545,
-            "vertex_2_z_coordinate": 0.971924,
+            "vertex_2_z_coordinate": 0.97196720032,
             "vertex_3_x_coordinate": 49.911,
             "vertex_3_y_coordinate": 33.2737,
-            "vertex_3_z_coordinate": 0.971924,
+            "vertex_3_z_coordinate": 0.97196720032,
             "vertex_4_x_coordinate": 49.911,
             "vertex_4_y_coordinate": 33.2737,
             "vertex_4_z_coordinate": 2.3293,
             "view_factor_to_ground": "Autocalculate"
         },
         "Perimeter_bot_ZN_3_Wall_North_Door1": {
             "building_surface_name": "Perimeter_bot_ZN_3_Wall_North",
@@ -6625,67 +6323,67 @@
             "vertex_3_z_coordinate": 0.0,
             "vertex_4_x_coordinate": 15.928941472948,
             "vertex_4_y_coordinate": 33.2738,
             "vertex_4_z_coordinate": 2.1336
         },
         "Perimeter_bot_ZN_3_Wall_North_Window1": {
             "building_surface_name": "Perimeter_bot_ZN_3_Wall_North",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 49.91,
             "vertex_1_y_coordinate": 33.2738,
             "vertex_1_z_coordinate": 2.3293,
             "vertex_2_x_coordinate": 49.91,
             "vertex_2_y_coordinate": 33.2738,
-            "vertex_2_z_coordinate": 0.954652,
+            "vertex_2_z_coordinate": 0.95455007488,
             "vertex_3_x_coordinate": 34.0868,
             "vertex_3_y_coordinate": 33.2738,
-            "vertex_3_z_coordinate": 0.954652,
+            "vertex_3_z_coordinate": 0.95455007488,
             "vertex_4_x_coordinate": 34.0868,
             "vertex_4_y_coordinate": 33.2738,
             "vertex_4_z_coordinate": 2.3293,
             "view_factor_to_ground": "Autocalculate"
         },
         "Perimeter_bot_ZN_3_Wall_North_Window2": {
             "building_surface_name": "Perimeter_bot_ZN_3_Wall_North",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 32.8676,
             "vertex_1_y_coordinate": 33.2738,
             "vertex_1_z_coordinate": 2.3293,
             "vertex_2_x_coordinate": 32.8676,
             "vertex_2_y_coordinate": 33.2738,
-            "vertex_2_z_coordinate": 0.954652,
+            "vertex_2_z_coordinate": 0.95455007488,
             "vertex_3_x_coordinate": 17.0434,
             "vertex_3_y_coordinate": 33.2738,
-            "vertex_3_z_coordinate": 0.954652,
+            "vertex_3_z_coordinate": 0.95455007488,
             "vertex_4_x_coordinate": 17.0434,
             "vertex_4_y_coordinate": 33.2738,
             "vertex_4_z_coordinate": 2.3293,
             "view_factor_to_ground": "Autocalculate"
         },
         "Perimeter_bot_ZN_3_Wall_North_Window3": {
             "building_surface_name": "Perimeter_bot_ZN_3_Wall_North",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 15.8242,
             "vertex_1_y_coordinate": 33.2738,
             "vertex_1_z_coordinate": 2.3293,
             "vertex_2_x_coordinate": 15.8242,
             "vertex_2_y_coordinate": 33.2738,
-            "vertex_2_z_coordinate": 0.954652,
+            "vertex_2_z_coordinate": 0.95455007488,
             "vertex_3_x_coordinate": 0.0,
             "vertex_3_y_coordinate": 33.2738,
-            "vertex_3_z_coordinate": 0.954652,
+            "vertex_3_z_coordinate": 0.95455007488,
             "vertex_4_x_coordinate": 0.0,
             "vertex_4_y_coordinate": 33.2738,
             "vertex_4_z_coordinate": 2.3293,
             "view_factor_to_ground": "Autocalculate"
         },
         "Perimeter_bot_ZN_4_Wall_West_Door": {
             "building_surface_name": "Perimeter_bot_ZN_4_Wall_West",
@@ -6703,55 +6401,55 @@
             "vertex_3_z_coordinate": 0.0,
             "vertex_4_x_coordinate": 0.0,
             "vertex_4_y_coordinate": 1.365191323208,
             "vertex_4_z_coordinate": 2.1336
         },
         "Perimeter_bot_ZN_4_Wall_West_Window1": {
             "building_surface_name": "Perimeter_bot_ZN_4_Wall_West",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 0.0,
             "vertex_1_y_coordinate": 33.2737,
             "vertex_1_z_coordinate": 2.3293,
             "vertex_2_x_coordinate": 0.0,
             "vertex_2_y_coordinate": 33.2737,
-            "vertex_2_z_coordinate": 0.971924,
+            "vertex_2_z_coordinate": 0.97196720032,
             "vertex_3_x_coordinate": 0.0,
             "vertex_3_y_coordinate": 2.4384,
-            "vertex_3_z_coordinate": 0.971924,
+            "vertex_3_z_coordinate": 0.97196720032,
             "vertex_4_x_coordinate": 0.0,
             "vertex_4_y_coordinate": 2.4384,
             "vertex_4_z_coordinate": 2.3293,
             "view_factor_to_ground": "Autocalculate"
         },
         "Perimeter_bot_ZN_4_Wall_West_Window2": {
             "building_surface_name": "Perimeter_bot_ZN_4_Wall_West",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 0.0,
             "vertex_1_y_coordinate": 1.2192,
             "vertex_1_z_coordinate": 2.3293,
             "vertex_2_x_coordinate": 0.0,
             "vertex_2_y_coordinate": 1.2192,
-            "vertex_2_z_coordinate": 0.971924,
+            "vertex_2_z_coordinate": 0.97196720032,
             "vertex_3_x_coordinate": 0.0,
             "vertex_3_y_coordinate": 0.0,
-            "vertex_3_z_coordinate": 0.971924,
+            "vertex_3_z_coordinate": 0.97196720032,
             "vertex_4_x_coordinate": 0.0,
             "vertex_4_y_coordinate": 0.0,
             "vertex_4_z_coordinate": 2.3293,
             "view_factor_to_ground": "Autocalculate"
         },
         "Perimeter_mid_ZN_1_Wall_South_Window": {
             "building_surface_name": "Perimeter_mid_ZN_1_Wall_South",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 0.0,
             "vertex_1_y_coordinate": 0.0,
             "vertex_1_z_coordinate": 6.2917,
             "vertex_2_x_coordinate": 0.0,
@@ -6763,15 +6461,15 @@
             "vertex_4_x_coordinate": 49.91,
             "vertex_4_y_coordinate": 0.0,
             "vertex_4_z_coordinate": 6.2917,
             "view_factor_to_ground": "Autocalculate"
         },
         "Perimeter_mid_ZN_2_Wall_East_Window": {
             "building_surface_name": "Perimeter_mid_ZN_2_Wall_East",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 49.911,
             "vertex_1_y_coordinate": 0.0,
             "vertex_1_z_coordinate": 6.2917,
             "vertex_2_x_coordinate": 49.911,
@@ -6783,15 +6481,15 @@
             "vertex_4_x_coordinate": 49.911,
             "vertex_4_y_coordinate": 33.2737,
             "vertex_4_z_coordinate": 6.2917,
             "view_factor_to_ground": "Autocalculate"
         },
         "Perimeter_mid_ZN_3_Wall_North_Window": {
             "building_surface_name": "Perimeter_mid_ZN_3_Wall_North",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 49.91,
             "vertex_1_y_coordinate": 33.2738,
             "vertex_1_z_coordinate": 6.2917,
             "vertex_2_x_coordinate": 49.91,
@@ -6803,15 +6501,15 @@
             "vertex_4_x_coordinate": 0.0,
             "vertex_4_y_coordinate": 33.2738,
             "vertex_4_z_coordinate": 6.2917,
             "view_factor_to_ground": "Autocalculate"
         },
         "Perimeter_mid_ZN_4_Wall_West_Window": {
             "building_surface_name": "Perimeter_mid_ZN_4_Wall_West",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 0.0,
             "vertex_1_y_coordinate": 33.2737,
             "vertex_1_z_coordinate": 6.2917,
             "vertex_2_x_coordinate": 0.0,
@@ -6823,15 +6521,15 @@
             "vertex_4_x_coordinate": 0.0,
             "vertex_4_y_coordinate": 0.0,
             "vertex_4_z_coordinate": 6.2917,
             "view_factor_to_ground": "Autocalculate"
         },
         "Perimeter_top_ZN_1_Wall_South_Window": {
             "building_surface_name": "Perimeter_top_ZN_1_Wall_South",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 0.0,
             "vertex_1_y_coordinate": 0.0,
             "vertex_1_z_coordinate": 10.2541,
             "vertex_2_x_coordinate": 0.0,
@@ -6843,15 +6541,15 @@
             "vertex_4_x_coordinate": 49.91,
             "vertex_4_y_coordinate": 0.0,
             "vertex_4_z_coordinate": 10.2541,
             "view_factor_to_ground": "Autocalculate"
         },
         "Perimeter_top_ZN_2_Wall_East_Window": {
             "building_surface_name": "Perimeter_top_ZN_2_Wall_East",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 49.911,
             "vertex_1_y_coordinate": 0.0,
             "vertex_1_z_coordinate": 10.2541,
             "vertex_2_x_coordinate": 49.911,
@@ -6863,15 +6561,15 @@
             "vertex_4_x_coordinate": 49.911,
             "vertex_4_y_coordinate": 33.2737,
             "vertex_4_z_coordinate": 10.2541,
             "view_factor_to_ground": "Autocalculate"
         },
         "Perimeter_top_ZN_3_Wall_North_Window": {
             "building_surface_name": "Perimeter_top_ZN_3_Wall_North",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 49.91,
             "vertex_1_y_coordinate": 33.2738,
             "vertex_1_z_coordinate": 10.2541,
             "vertex_2_x_coordinate": 49.91,
@@ -6883,15 +6581,15 @@
             "vertex_4_x_coordinate": 0.0,
             "vertex_4_y_coordinate": 33.2738,
             "vertex_4_z_coordinate": 10.2541,
             "view_factor_to_ground": "Autocalculate"
         },
         "Perimeter_top_ZN_4_Wall_West_Window": {
             "building_surface_name": "Perimeter_top_ZN_4_Wall_West",
-            "construction_name": "Window_U_0.41_SHGC_0.38",
+            "construction_name": "Window_U_0.36_SHGC_0.38",
             "multiplier": 1.0,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 0.0,
             "vertex_1_y_coordinate": 33.2737,
             "vertex_1_z_coordinate": 10.2541,
             "vertex_2_x_coordinate": 0.0,
@@ -6994,191 +6692,191 @@
             "surface_area": 262.5056,
             "zone_or_zonelist_name": "Perimeter_top_ZN_4"
         }
     },
     "Lights": {
         "Core_bottom_Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "General Lights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
-            "watts_per_zone_floor_area": 8.503489229,
-            "zone_or_zonelist_name": "Core_bottom"
+            "watts_per_zone_floor_area": 6.888902667,
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_bottom"
         },
         "Core_mid_Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "General Lights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
-            "watts_per_zone_floor_area": 8.503489229,
-            "zone_or_zonelist_name": "Core_mid"
+            "watts_per_zone_floor_area": 6.888902667,
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_mid"
         },
         "Core_top_Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "General Lights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
-            "watts_per_zone_floor_area": 8.503489229,
-            "zone_or_zonelist_name": "Core_top"
+            "watts_per_zone_floor_area": 6.888902667,
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_top"
         },
         "Perimeter_bot_ZN_1_Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "General Lights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
-            "watts_per_zone_floor_area": 8.503489229,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_1"
+            "watts_per_zone_floor_area": 6.888902667,
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_1"
         },
         "Perimeter_bot_ZN_2_Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "General Lights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
-            "watts_per_zone_floor_area": 8.503489229,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_2"
+            "watts_per_zone_floor_area": 6.888902667,
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_2"
         },
         "Perimeter_bot_ZN_3_Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "General Lights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
-            "watts_per_zone_floor_area": 8.503489229,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_3"
+            "watts_per_zone_floor_area": 6.888902667,
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_3"
         },
         "Perimeter_bot_ZN_4_Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "General Lights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
-            "watts_per_zone_floor_area": 8.503489229,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_4"
+            "watts_per_zone_floor_area": 6.888902667,
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_4"
         },
         "Perimeter_mid_ZN_1_Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "General Lights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
-            "watts_per_zone_floor_area": 8.503489229,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_1"
+            "watts_per_zone_floor_area": 6.888902667,
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_1"
         },
         "Perimeter_mid_ZN_2_Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "General Lights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
-            "watts_per_zone_floor_area": 8.503489229,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_2"
+            "watts_per_zone_floor_area": 6.888902667,
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_2"
         },
         "Perimeter_mid_ZN_3_Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "General Lights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
-            "watts_per_zone_floor_area": 8.503489229,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_3"
+            "watts_per_zone_floor_area": 6.888902667,
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_3"
         },
         "Perimeter_mid_ZN_4_Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "General Lights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
-            "watts_per_zone_floor_area": 8.503489229,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_4"
+            "watts_per_zone_floor_area": 6.888902667,
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_4"
         },
         "Perimeter_top_ZN_1_Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "General Lights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
-            "watts_per_zone_floor_area": 8.503489229,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_1"
+            "watts_per_zone_floor_area": 6.888902667,
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_1"
         },
         "Perimeter_top_ZN_2_Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "General Lights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
-            "watts_per_zone_floor_area": 8.503489229,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_2"
+            "watts_per_zone_floor_area": 6.888902667,
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_2"
         },
         "Perimeter_top_ZN_3_Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "General Lights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
-            "watts_per_zone_floor_area": 8.503489229,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_3"
+            "watts_per_zone_floor_area": 6.888902667,
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_3"
         },
         "Perimeter_top_ZN_4_Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "General Lights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
-            "watts_per_zone_floor_area": 8.503489229,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_4"
+            "watts_per_zone_floor_area": 6.888902667,
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_4"
         }
     },
     "Material": {
         "100mm Normalweight concrete floor": {
             "conductivity": 2.31,
             "density": 2322,
             "roughness": "MediumRough",
@@ -7629,978 +7327,413 @@
         "Output:Meter:MeterFileOnly 2": {
             "key_name": "ElectricityNet:Facility",
             "reporting_frequency": "Hourly"
         },
         "Output:Meter:MeterFileOnly 3": {
             "key_name": "NaturalGas:Facility",
             "reporting_frequency": "Hourly"
-        },
-        "Output:Meter:MeterFileOnly 4": {
-            "key_name": "InteriorLights:Electricity",
-            "reporting_frequency": "Hourly"
-        },
-        "Output:Meter:MeterFileOnly 5": {
-            "key_name": "InteriorEquipment:Electricity",
-            "reporting_frequency": "Hourly"
         }
     },
     "Output:Surfaces:Drawing": {
         "Output:Surfaces:Drawing 1": {
             "report_type": "DXF"
         }
     },
     "Output:Surfaces:List": {
         "Output:Surfaces:List 1": {
             "report_type": "Details"
         }
     },
     "Output:Table:Monthly": {
-        "Building Energy Performance - Electricity": {
-            "digits_after_decimal": 2,
-            "variable_details": [
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "InteriorLights:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "TaskLights:InteriorLights:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "ExteriorLights:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "General:InteriorEquipment:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "ExteriorEquipment:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Fans:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Pumps:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Heating:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Cooling:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "HeatRejection:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Humidifier:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "HeatRecovery:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "WaterSystems:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Cogeneration:Electricity"
-                }
-            ]
-        },
-        "Building Energy Performance - Natural Gas": {
-            "digits_after_decimal": 2,
+        "NameHolderMonthlySummary ClimateZone 5B": {
+            "digits_after_decimal": 3,
             "variable_details": [
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "InteriorEquipment:NaturalGas"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "ExteriorEquipment:NaturalGas"
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
                     "variable_or_meter_name": "Heating:NaturalGas"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Cooling:NaturalGas"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "WaterSystems:NaturalGas"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Cogeneration:NaturalGas"
-                }
-            ]
-        },
-        "Building Loads - Cooling": {
-            "digits_after_decimal": 2,
-            "variable_details": [
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Air System Sensible Cooling Energy"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "Zone Air System Sensible Cooling Rate"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Site Outdoor Air Drybulb Temperature"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Site Outdoor Air Wetbulb Temperature"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Total Internal Latent Gain Energy"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "Zone Total Internal Latent Gain Energy"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Site Outdoor Air Drybulb Temperature"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Site Outdoor Air Wetbulb Temperature"
-                }
-            ]
-        },
-        "Building Loads - Electric": {
-            "digits_after_decimal": 2,
-            "variable_details": [
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Lights Electricity Energy"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "Zone Lights Electricity Energy"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Electric Equipment Electricity Energy"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "Zone Electric Equipment Electricity Energy"
                 }
             ]
         },
-        "Building Loads - Heating": {
-            "digits_after_decimal": 2,
-            "variable_details": [
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Air System Sensible Heating Energy"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "Zone Air System Sensible Heating Rate"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Site Outdoor Air Drybulb Temperature"
-                }
-            ]
-        },
-        "Comfort Report - Simple 55": {
-            "digits_after_decimal": 2,
-            "variable_details": [
-                {
-                    "aggregation_type_for_variable_or_meter": "HoursNonZero",
-                    "variable_or_meter_name": "Zone Thermal Comfort ASHRAE 55 Simple Model Summer Clothes Not Comfortable Time"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverageDuringHoursShown",
-                    "variable_or_meter_name": "Zone Mean Air Temperature"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "HoursNonZero",
-                    "variable_or_meter_name": "Zone Thermal Comfort ASHRAE 55 Simple Model Winter Clothes Not Comfortable Time"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverageDuringHoursShown",
-                    "variable_or_meter_name": "Zone Mean Air Temperature"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "HoursNonZero",
-                    "variable_or_meter_name": "Zone Thermal Comfort ASHRAE 55 Simple Model Summer or Winter Clothes Not Comfortable Time"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverageDuringHoursShown",
-                    "variable_or_meter_name": "Zone Mean Air Temperature"
-                }
-            ]
-        },
-        "Components of Peak Electrical Demand": {
+        "NameHolderMonthlySummary CodeAmendment NoneAmend": {
             "digits_after_decimal": 3,
             "variable_details": [
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Electricity:Facility"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "Electricity:Facility"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "InteriorLights:Electricity"
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "InteriorEquipment:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Fans:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Heating:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Cooling:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "ExteriorLights:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Pumps:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "HeatRejection:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "ExteriorEquipment:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Humidification:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "HeatRecovery:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "WaterSystems:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Refrigeration:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Generators:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "ElectricityProduced:Facility"
-                }
-            ]
-        },
-        "Components of Peak Net Electrical Demand": {
-            "digits_after_decimal": 3,
-            "variable_details": [
-                {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "ElectricityNet:Facility"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "ElectricityNet:Facility"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "InteriorLights:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "InteriorEquipment:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Fans:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Heating:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Cooling:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "ExteriorLights:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Pumps:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "HeatRejection:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "ExteriorEquipment:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Humidification:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "HeatRecovery:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "WaterSystems:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Refrigeration:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Generators:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "ElectricityProduced:Facility"
+                    "variable_or_meter_name": "Heating:NaturalGas"
                 }
             ]
         },
-        "Energy Consumption - Electricity & Natural Gas": {
-            "digits_after_decimal": 2,
+        "NameHolderMonthlySummary CodeName ASHRAE901": {
+            "digits_after_decimal": 3,
             "variable_details": [
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Electricity:Building"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "Electricity:Building"
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "NaturalGas:Building"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "NaturalGas:Building"
+                    "variable_or_meter_name": "Heating:NaturalGas"
                 }
             ]
         },
-        "Monthly Indoor Temp": {
-            "digits_after_decimal": 2,
+        "NameHolderMonthlySummary CodeYear 2019": {
+            "digits_after_decimal": 3,
             "variable_details": [
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Mean Air Temperature"
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Site Outdoor Air Drybulb Temperature"
-                }
-            ]
-        },
-        "Outdoor Air Summary": {
-            "digits_after_decimal": 3,
-            "variable_details": [
-                {
-                    "aggregation_type_for_variable_or_meter": "HoursNonZero",
-                    "variable_or_meter_name": "Zone People Occupant Count"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverageDuringHoursShown",
-                    "variable_or_meter_name": "Zone People Occupant Count"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverageDuringHoursShown",
-                    "variable_or_meter_name": "Zone Mechanical Ventilation Air Changes per Hour"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverageDuringHoursShown",
-                    "variable_or_meter_name": "Zone Infiltration Air Change Rate"
+                    "variable_or_meter_name": "Heating:NaturalGas"
                 }
             ]
         },
-        "Overall HVAC Air System Loads": {
+        "NameHolderMonthlySummary PrototypeName OfficeMedium": {
             "digits_after_decimal": 3,
             "variable_details": [
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Air System Total Heating Energy"
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Air System Total Cooling Energy"
+                    "variable_or_meter_name": "Heating:NaturalGas"
                 }
             ]
         },
-        "Overall HVAC System Energy": {
+        "NameHolderMonthlySummary RepresentCity USA_CO_Denver": {
             "digits_after_decimal": 3,
             "variable_details": [
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Electricity:HVAC"
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
                     "variable_or_meter_name": "Heating:NaturalGas"
                 }
             ]
         },
-        "Peak Electrical Demand": {
+        "NameHolderMonthlySummary State National": {
             "digits_after_decimal": 3,
             "variable_details": [
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Electricity:Facility"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "Electricity:Facility"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "InteriorLights:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "InteriorEquipment:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Fans:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Heating:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Cooling:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "ExteriorLights:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Pumps:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "HeatRejection:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "ExteriorEquipment:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Humidification:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "HeatRecovery:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "WaterSystems:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Refrigeration:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Generators:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "ElectricityProduced:Facility"
-                }
-            ]
-        },
-        "Peak Energy End-Use - Electricity Part 1": {
-            "digits_after_decimal": 2,
-            "variable_details": [
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "InteriorLights:Electricity"
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "TaskLights:InteriorLights:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "ExteriorLights:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "General:InteriorEquipment:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "ExteriorEquipment:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "Fans:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "Pumps:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "Heating:Electricity"
-                }
-            ]
-        },
-        "Peak Gas Demand": {
-            "digits_after_decimal": 3,
-            "variable_details": [
-                {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "NaturalGas:Facility"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "NaturalGas:Facility"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "NaturalGas:HVAC"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "InteriorEquipment:NaturalGas"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "MiscPlugGas:InteriorEquipment:NaturalGas"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "NaturalGas:Plant"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "WaterSystems:NaturalGas"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Water Heater:WaterSystems:NaturalGas"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
                     "variable_or_meter_name": "Heating:NaturalGas"
                 }
             ]
         },
-        "Setpoints Not Met With Temperatures": {
-            "digits_after_decimal": 2,
-            "variable_details": [
-                {
-                    "aggregation_type_for_variable_or_meter": "HoursNonZero",
-                    "variable_or_meter_name": "Zone Heating Setpoint Not Met Time"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverageDuringHoursShown",
-                    "variable_or_meter_name": "Zone Mean Air Temperature"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "HoursNonZero",
-                    "variable_or_meter_name": "Zone Heating Setpoint Not Met While Occupied Time"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverageDuringHoursShown",
-                    "variable_or_meter_name": "Zone Mean Air Temperature"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "HoursNonZero",
-                    "variable_or_meter_name": "Zone Cooling Setpoint Not Met Time"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverageDuringHoursShown",
-                    "variable_or_meter_name": "Zone Mean Air Temperature"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "HoursNonZero",
-                    "variable_or_meter_name": "Zone Cooling Setpoint Not Met While Occupied Time"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverageDuringHoursShown",
-                    "variable_or_meter_name": "Zone Mean Air Temperature"
-                }
-            ]
-        },
-        "Space Loads": {
-            "digits_after_decimal": 2,
+        "NameHolderMonthlySummary TaskPurpose ProgressIndicator": {
+            "digits_after_decimal": 3,
             "variable_details": [
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone People Total Heating Energy"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Lights Total Heating Energy"
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Electric Equipment Total Heating Energy"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Infiltration Sensible Heat Gain Energy"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Infiltration Sensible Heat Loss Energy"
+                    "variable_or_meter_name": "Heating:NaturalGas"
                 }
             ]
         },
-        "Ventilation Load Components": {
+        "NameHolderMonthlySummary TaskScope National": {
             "digits_after_decimal": 3,
             "variable_details": [
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Mechanical Ventilation No Load Heat Removal Energy"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Mechanical Ventilation Cooling Load Increase Energy"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Mechanical Ventilation Cooling Load Increase Due to Overheating Energy"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Mechanical Ventilation Cooling Load Decrease Energy"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Mechanical Ventilation No Load Heat Addition Energy"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Mechanical Ventilation Heating Load Increase Energy"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Mechanical Ventilation Heating Load Increase Due to Overcooling Energy"
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Mechanical Ventilation Heating Load Decrease Energy"
+                    "variable_or_meter_name": "Heating:NaturalGas"
                 }
             ]
         }
     },
     "Output:Table:SummaryReports": {
         "Output:Table:SummaryReports 1": {
             "reports": [
                 {
-                    "report_name": "AnnualBuildingUtilityPerformanceSummary"
-                },
-                {
-                    "report_name": "InputVerificationandResultsSummary"
+                    "report_name": "AllSummaryAndMonthly"
                 },
                 {
-                    "report_name": "ClimaticDataSummary"
-                },
-                {
-                    "report_name": "EquipmentSummary"
-                },
-                {
-                    "report_name": "EnvelopeSummary"
+                    "report_name": "Standard62.1Summary"
                 }
             ]
         }
     },
     "Output:VariableDictionary": {
         "Output:VariableDictionary 1": {
             "key_field": "regular"
         }
     },
+    "OutputControl:ReportingTolerances": {
+        "OutputControl:ReportingTolerances 1": {
+            "tolerance_for_time_cooling_setpoint_not_met": 0.556,
+            "tolerance_for_time_heating_setpoint_not_met": 0.556
+        }
+    },
     "OutputControl:Table:Style": {
         "OutputControl:Table:Style 1": {
             "column_separator": "CommaAndHTML"
         }
     },
     "People": {
         "Core_bottom": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.5787942465724,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
-            "number_of_people_schedule_name": "BLDG_OCC_SCH",
+            "number_of_people_schedule_name": "BLDG_OCC_SCH_wo_SB",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.5787942465724,
-            "zone_or_zonelist_name": "Core_bottom"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_bottom"
         },
         "Core_mid": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.5787942465724,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
-            "number_of_people_schedule_name": "BLDG_OCC_SCH",
+            "number_of_people_schedule_name": "BLDG_OCC_SCH_wo_SB",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.5787942465724,
-            "zone_or_zonelist_name": "Core_mid"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_mid"
         },
         "Core_top": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.5787942465724,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
-            "number_of_people_schedule_name": "BLDG_OCC_SCH",
+            "number_of_people_schedule_name": "BLDG_OCC_SCH_wo_SB",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.5787942465724,
-            "zone_or_zonelist_name": "Core_top"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_top"
         },
         "Perimeter_bot_ZN_1": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.5787942465724,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
-            "number_of_people_schedule_name": "BLDG_OCC_SCH",
+            "number_of_people_schedule_name": "BLDG_OCC_SCH_wo_SB",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.5787942465724,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_1"
         },
         "Perimeter_bot_ZN_2": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.5787942465724,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
-            "number_of_people_schedule_name": "BLDG_OCC_SCH",
+            "number_of_people_schedule_name": "BLDG_OCC_SCH_wo_SB",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.5787942465724,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_2"
         },
         "Perimeter_bot_ZN_3": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.5787942465724,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
-            "number_of_people_schedule_name": "BLDG_OCC_SCH",
+            "number_of_people_schedule_name": "BLDG_OCC_SCH_wo_SB",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.5787942465724,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_3"
         },
         "Perimeter_bot_ZN_4": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.5787942465724,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
-            "number_of_people_schedule_name": "BLDG_OCC_SCH",
+            "number_of_people_schedule_name": "BLDG_OCC_SCH_wo_SB",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.5787942465724,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_4"
         },
         "Perimeter_mid_ZN_1": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.5787942465724,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
-            "number_of_people_schedule_name": "BLDG_OCC_SCH",
+            "number_of_people_schedule_name": "BLDG_OCC_SCH_wo_SB",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.5787942465724,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_1"
         },
         "Perimeter_mid_ZN_2": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.5787942465724,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
-            "number_of_people_schedule_name": "BLDG_OCC_SCH",
+            "number_of_people_schedule_name": "BLDG_OCC_SCH_w_SB",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.5787942465724,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_2"
         },
         "Perimeter_mid_ZN_3": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.5787942465724,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
-            "number_of_people_schedule_name": "BLDG_OCC_SCH",
+            "number_of_people_schedule_name": "BLDG_OCC_SCH_wo_SB",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.5787942465724,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_3"
         },
         "Perimeter_mid_ZN_4": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.5787942465724,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
-            "number_of_people_schedule_name": "BLDG_OCC_SCH",
+            "number_of_people_schedule_name": "BLDG_OCC_SCH_wo_SB",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.5787942465724,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_4"
         },
         "Perimeter_top_ZN_1": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.5787942465724,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
-            "number_of_people_schedule_name": "BLDG_OCC_SCH",
+            "number_of_people_schedule_name": "BLDG_OCC_SCH_wo_SB",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.5787942465724,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_1"
         },
         "Perimeter_top_ZN_2": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.5787942465724,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
-            "number_of_people_schedule_name": "BLDG_OCC_SCH",
+            "number_of_people_schedule_name": "BLDG_OCC_SCH_wo_SB",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.5787942465724,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_2"
         },
         "Perimeter_top_ZN_3": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.5787942465724,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
-            "number_of_people_schedule_name": "BLDG_OCC_SCH",
+            "number_of_people_schedule_name": "BLDG_OCC_SCH_wo_SB",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.5787942465724,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_3"
         },
         "Perimeter_top_ZN_4": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.5787942465724,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
-            "number_of_people_schedule_name": "BLDG_OCC_SCH",
+            "number_of_people_schedule_name": "BLDG_OCC_SCH_wo_SB",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.5787942465724,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_4"
         }
     },
     "Pipe:Adiabatic": {
         "SHWSys1 Demand Bypass Pipe": {
             "inlet_node_name": "SHWSys1 Demand Bypass Pipe Inlet Node",
             "outlet_node_name": "SHWSys1 Demand Bypass Pipe Outlet Node"
         },
@@ -8630,15 +7763,15 @@
                 }
             ]
         }
     },
     "PlantEquipmentOperation:HeatingLoad": {
         "SHWSys1 Operation Scheme": {
             "load_range_1_lower_limit": 0.0,
-            "load_range_1_upper_limit": 1000000000000000,
+            "load_range_1_upper_limit": 1000000000000000.0,
             "range_1_equipment_list_name": "SHWSys1 Equipment List"
         }
     },
     "PlantEquipmentOperationSchemes": {
         "SHWSys1 Loop Operation Scheme List": {
             "control_scheme_1_name": "SHWSys1 Operation Scheme",
             "control_scheme_1_object_type": "PlantEquipmentOperation:HeatingLoad",
@@ -8680,15 +7813,15 @@
     },
     "RunPeriod": {
         "Run Period 1": {
             "apply_weekend_holiday_rule": "No",
             "begin_day_of_month": 1,
             "begin_month": 1,
             "begin_year": 1991,
-            "day_of_week_for_start_day": "Tuesday",
+            "day_of_week_for_start_day": "Sunday",
             "end_day_of_month": 31,
             "end_month": 12,
             "end_year": 1991,
             "use_weather_file_daylight_saving_period": "No",
             "use_weather_file_holidays_and_special_days": "No",
             "use_weather_file_rain_indicators": "Yes",
             "use_weather_file_snow_indicators": "Yes"
@@ -9467,14 +8600,720 @@
                 },
                 {
                     "field": 0.0
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
+        "BLDG_OCC_SCH_w_SB": {
+            "data": [
+                {
+                    "field": "Through: 12/31"
+                },
+                {
+                    "field": "For: Weekdays"
+                },
+                {
+                    "field": "Until: 01:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 02:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 03:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 04:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 05:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 06:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 07:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 08:00"
+                },
+                {
+                    "field": 0.2
+                },
+                {
+                    "field": "Until: 09:00"
+                },
+                {
+                    "field": 0.95
+                },
+                {
+                    "field": "Until: 10:00"
+                },
+                {
+                    "field": 0.95
+                },
+                {
+                    "field": "Until: 11:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 12:00"
+                },
+                {
+                    "field": 0.95
+                },
+                {
+                    "field": "Until: 13:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 14:00"
+                },
+                {
+                    "field": 0.95
+                },
+                {
+                    "field": "Until: 15:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 16:00"
+                },
+                {
+                    "field": 0.95
+                },
+                {
+                    "field": "Until: 17:00"
+                },
+                {
+                    "field": 0.95
+                },
+                {
+                    "field": "Until: 18:00"
+                },
+                {
+                    "field": 0.3
+                },
+                {
+                    "field": "Until: 19:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 20:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 21:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 22:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 23:00"
+                },
+                {
+                    "field": 0.05
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0.05
+                },
+                {
+                    "field": "For: Saturday"
+                },
+                {
+                    "field": "Until: 01:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 02:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 03:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 04:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 05:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 06:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 07:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 08:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 09:00"
+                },
+                {
+                    "field": 0.3
+                },
+                {
+                    "field": "Until: 10:00"
+                },
+                {
+                    "field": 0.3
+                },
+                {
+                    "field": "Until: 11:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 12:00"
+                },
+                {
+                    "field": 0.3
+                },
+                {
+                    "field": "Until: 13:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 14:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 15:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 16:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 17:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 18:00"
+                },
+                {
+                    "field": 0.05
+                },
+                {
+                    "field": "Until: 19:00"
+                },
+                {
+                    "field": 0.05
+                },
+                {
+                    "field": "Until: 20:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 21:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 22:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 23:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "For: SummerDesignDay"
+                },
+                {
+                    "field": "Until: 06:00"
+                },
+                {
+                    "field": 1e-09
+                },
+                {
+                    "field": "Until: 22:00"
+                },
+                {
+                    "field": 1.0
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0.05
+                },
+                {
+                    "field": "For: WinterDesignDay"
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0.0
+                },
+                {
+                    "field": "For:Sunday Holidays AllOtherDays"
+                },
+                {
+                    "field": "Until: 06:00"
+                },
+                {
+                    "field": 0.0
+                },
+                {
+                    "field": "Until: 18:00"
+                },
+                {
+                    "field": 0.05
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0.0
+                }
+            ],
+            "schedule_type_limits_name": "Fraction"
+        },
+        "BLDG_OCC_SCH_wo_SB": {
+            "data": [
+                {
+                    "field": "Through: 12/31"
+                },
+                {
+                    "field": "For: Weekdays"
+                },
+                {
+                    "field": "Until: 01:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 02:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 03:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 04:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 05:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 06:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 07:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 08:00"
+                },
+                {
+                    "field": 0.2
+                },
+                {
+                    "field": "Until: 09:00"
+                },
+                {
+                    "field": 0.95
+                },
+                {
+                    "field": "Until: 10:00"
+                },
+                {
+                    "field": 0.95
+                },
+                {
+                    "field": "Until: 11:00"
+                },
+                {
+                    "field": 0.975703226795432
+                },
+                {
+                    "field": "Until: 12:00"
+                },
+                {
+                    "field": 0.95
+                },
+                {
+                    "field": "Until: 13:00"
+                },
+                {
+                    "field": 0.513528014102859
+                },
+                {
+                    "field": "Until: 14:00"
+                },
+                {
+                    "field": 0.95
+                },
+                {
+                    "field": "Until: 15:00"
+                },
+                {
+                    "field": 0.975703226795432
+                },
+                {
+                    "field": "Until: 16:00"
+                },
+                {
+                    "field": 0.95
+                },
+                {
+                    "field": "Until: 17:00"
+                },
+                {
+                    "field": 0.95
+                },
+                {
+                    "field": "Until: 18:00"
+                },
+                {
+                    "field": 0.3
+                },
+                {
+                    "field": "Until: 19:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 20:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 21:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 22:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 23:00"
+                },
+                {
+                    "field": 0.05
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0.05
+                },
+                {
+                    "field": "For: Saturday"
+                },
+                {
+                    "field": "Until: 01:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 02:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 03:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 04:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 05:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 06:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 07:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 08:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 09:00"
+                },
+                {
+                    "field": 0.3
+                },
+                {
+                    "field": "Until: 10:00"
+                },
+                {
+                    "field": 0.3
+                },
+                {
+                    "field": "Until: 11:00"
+                },
+                {
+                    "field": 0.308116808461715
+                },
+                {
+                    "field": "Until: 12:00"
+                },
+                {
+                    "field": 0.3
+                },
+                {
+                    "field": "Until: 13:00"
+                },
+                {
+                    "field": 0.102705602820572
+                },
+                {
+                    "field": "Until: 14:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 15:00"
+                },
+                {
+                    "field": 0.102705602820572
+                },
+                {
+                    "field": "Until: 16:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 17:00"
+                },
+                {
+                    "field": 0.1
+                },
+                {
+                    "field": "Until: 18:00"
+                },
+                {
+                    "field": 0.05
+                },
+                {
+                    "field": "Until: 19:00"
+                },
+                {
+                    "field": 0.05
+                },
+                {
+                    "field": "Until: 20:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 21:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 22:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 23:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "For: SummerDesignDay"
+                },
+                {
+                    "field": "Until: 06:00"
+                },
+                {
+                    "field": 1e-09
+                },
+                {
+                    "field": "Until: 22:00"
+                },
+                {
+                    "field": 1.0
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0.05
+                },
+                {
+                    "field": "For: WinterDesignDay"
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0.0
+                },
+                {
+                    "field": "For:Sunday Holidays AllOtherDays"
+                },
+                {
+                    "field": "Until: 06:00"
+                },
+                {
+                    "field": 0.0
+                },
+                {
+                    "field": "Until: 18:00"
+                },
+                {
+                    "field": 0.05
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0.0
+                }
+            ],
+            "schedule_type_limits_name": "Fraction"
+        },
         "BLDG_SWH_SCH": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: Weekdays SummerDesignDay"
@@ -10623,224 +10462,526 @@
                 },
                 {
                     "field": 26.7
                 }
             ],
             "schedule_type_limits_name": "Temperature"
         },
-        "CLOTHING_SCH": {
+        "CLGSETP_SCH_YES_OPTIMUM_w_SB": {
             "data": [
                 {
-                    "field": "Through: 04/30"
+                    "field": "Through: 12/31"
                 },
                 {
-                    "field": "For: AllDays"
+                    "field": "For: Weekdays"
+                },
+                {
+                    "field": "Until: 01:00"
+                },
+                {
+                    "field": 26.7
+                },
+                {
+                    "field": "Until: 02:00"
+                },
+                {
+                    "field": 26.7
+                },
+                {
+                    "field": "Until: 03:00"
+                },
+                {
+                    "field": 26.7
+                },
+                {
+                    "field": "Until: 04:00"
+                },
+                {
+                    "field": 26.7
+                },
+                {
+                    "field": "Until: 05:00"
+                },
+                {
+                    "field": 26.7
+                },
+                {
+                    "field": "Until: 06:00"
+                },
+                {
+                    "field": 25.6
+                },
+                {
+                    "field": "Until: 07:00"
+                },
+                {
+                    "field": 25
+                },
+                {
+                    "field": "Until: 08:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 09:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 10:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 11:00"
+                },
+                {
+                    "field": 24.5555555555556
+                },
+                {
+                    "field": "Until: 12:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 13:00"
+                },
+                {
+                    "field": 24.5555555555556
+                },
+                {
+                    "field": "Until: 14:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 15:00"
+                },
+                {
+                    "field": 24.5555555555556
+                },
+                {
+                    "field": "Until: 16:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 17:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 18:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 19:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 20:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 21:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 22:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 23:00"
+                },
+                {
+                    "field": 26.7
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 1.0
+                    "field": 26.7
                 },
                 {
-                    "field": "Through: 09/30"
+                    "field": "For: Saturday"
                 },
                 {
-                    "field": "For: AllDays"
+                    "field": "Until: 01:00"
+                },
+                {
+                    "field": 26.7
+                },
+                {
+                    "field": "Until: 02:00"
+                },
+                {
+                    "field": 26.7
+                },
+                {
+                    "field": "Until: 03:00"
+                },
+                {
+                    "field": 26.7
+                },
+                {
+                    "field": "Until: 04:00"
+                },
+                {
+                    "field": 26.7
+                },
+                {
+                    "field": "Until: 05:00"
+                },
+                {
+                    "field": 26.7
+                },
+                {
+                    "field": "Until: 06:00"
+                },
+                {
+                    "field": 25.7
+                },
+                {
+                    "field": "Until: 07:00"
+                },
+                {
+                    "field": 25
+                },
+                {
+                    "field": "Until: 08:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 09:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 10:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 11:00"
+                },
+                {
+                    "field": 24.5555555555556
+                },
+                {
+                    "field": "Until: 12:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 13:00"
+                },
+                {
+                    "field": 24.5555555555556
+                },
+                {
+                    "field": "Until: 14:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 15:00"
+                },
+                {
+                    "field": 24.5555555555556
+                },
+                {
+                    "field": "Until: 16:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 17:00"
+                },
+                {
+                    "field": 24
+                },
+                {
+                    "field": "Until: 18:00"
+                },
+                {
+                    "field": 26.7
+                },
+                {
+                    "field": "Until: 19:00"
+                },
+                {
+                    "field": 26.7
+                },
+                {
+                    "field": "Until: 20:00"
+                },
+                {
+                    "field": 26.7
+                },
+                {
+                    "field": "Until: 21:00"
+                },
+                {
+                    "field": 26.7
+                },
+                {
+                    "field": "Until: 22:00"
+                },
+                {
+                    "field": 26.7
+                },
+                {
+                    "field": "Until: 23:00"
+                },
+                {
+                    "field": 26.7
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.5
+                    "field": 26.7
                 },
                 {
-                    "field": "Through: 12/31"
+                    "field": "For: SummerDesignDay"
                 },
                 {
-                    "field": "For: AllDays"
+                    "field": "Until: 05:00"
+                },
+                {
+                    "field": 26.7
+                },
+                {
+                    "field": "Until: 06:00"
+                },
+                {
+                    "field": 25.7
+                },
+                {
+                    "field": "Until: 07:00"
+                },
+                {
+                    "field": 25.0
+                },
+                {
+                    "field": "Until: 22:00"
+                },
+                {
+                    "field": 24.0
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 1.0
-                }
-            ],
-            "schedule_type_limits_name": "Any Number"
-        },
-        "CW-Loop-Temp-Schedule": {
-            "data": [
+                    "field": 26.7
+                },
                 {
-                    "field": "Through: 12/31"
+                    "field": "For WinterDesignDay"
                 },
                 {
-                    "field": "For: AllDays"
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 26.7
+                },
+                {
+                    "field": "For:Sunday Holidays AllOtherDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 6.7
+                    "field": 26.7
                 }
             ],
             "schedule_type_limits_name": "Temperature"
         },
-        "Cool-Supply-Air-Temp-Sch": {
+        "CLOTHING_SCH": {
             "data": [
                 {
-                    "field": "Through: 12/31"
+                    "field": "Through: 04/30"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 12.8
-                }
-            ],
-            "schedule_type_limits_name": "Temperature"
-        },
-        "CoolingCoilAvailSched": {
-            "data": [
+                    "field": 1.0
+                },
+                {
+                    "field": "Through: 09/30"
+                },
+                {
+                    "field": "For: AllDays"
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0.5
+                },
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
                     "field": 1.0
                 }
             ],
-            "schedule_type_limits_name": "Fraction"
+            "schedule_type_limits_name": "Any Number"
         },
-        "Core_bottom sub cat Latent fract sched": {
+        "CW-Loop-Temp-Schedule": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.05
+                    "field": 6.7
                 }
             ],
-            "schedule_type_limits_name": "Fraction"
+            "schedule_type_limits_name": "Temperature"
         },
-        "Core_bottom sub cat Sensible fract sched": {
+        "CoolingCoilAvailSched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.2
+                    "field": 1.0
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "Core_bottom sub cat Temp Sched": {
+        "Core_bottom sub cat Latent fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 60.0
+                    "field": 0.05
                 }
             ],
-            "schedule_type_limits_name": "Temperature"
+            "schedule_type_limits_name": "Fraction"
         },
-        "Core_bottom sub catHot Supply Temp Sched": {
+        "Core_bottom sub cat Sensible fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 55
+                    "field": 0.2
                 }
             ],
-            "schedule_type_limits_name": "Temperature"
+            "schedule_type_limits_name": "Fraction"
         },
-        "Core_mid sub cat Latent fract sched": {
+        "Core_bottom sub catHot Supply Temp Sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.05
+                    "field": 55
                 }
             ],
-            "schedule_type_limits_name": "Fraction"
+            "schedule_type_limits_name": "Temperature"
         },
-        "Core_mid sub cat Sensible fract sched": {
+        "Core_mid sub cat Latent fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.2
+                    "field": 0.05
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "Core_mid sub cat Temp Sched": {
+        "Core_mid sub cat Sensible fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 60.0
+                    "field": 0.2
                 }
             ],
-            "schedule_type_limits_name": "Temperature"
+            "schedule_type_limits_name": "Fraction"
         },
         "Core_mid sub catHot Supply Temp Sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
@@ -10885,31 +11026,14 @@
                 },
                 {
                     "field": 0.2
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "Core_top sub cat Temp Sched": {
-            "data": [
-                {
-                    "field": "Through: 12/31"
-                },
-                {
-                    "field": "For: AllDays"
-                },
-                {
-                    "field": "Until: 24:00"
-                },
-                {
-                    "field": 60.0
-                }
-            ],
-            "schedule_type_limits_name": "Temperature"
-        },
         "Core_top sub catHot Supply Temp Sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
@@ -12174,103 +12298,439 @@
                 },
                 {
                     "field": 15.6
                 }
             ],
             "schedule_type_limits_name": "Temperature"
         },
-        "HVACOperationSchd": {
+        "HTGSETP_SCH_YES_OPTIMUM_w_SB": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
-                    "field": "For: Weekdays SummerDesignDay"
+                    "field": "For: Weekdays"
+                },
+                {
+                    "field": "Until: 01:00"
+                },
+                {
+                    "field": 15.6
+                },
+                {
+                    "field": "Until: 02:00"
+                },
+                {
+                    "field": 15.6
+                },
+                {
+                    "field": "Until: 03:00"
+                },
+                {
+                    "field": 15.6
+                },
+                {
+                    "field": "Until: 04:00"
+                },
+                {
+                    "field": 15.6
+                },
+                {
+                    "field": "Until: 05:00"
+                },
+                {
+                    "field": 15.6
                 },
                 {
                     "field": "Until: 06:00"
                 },
                 {
-                    "field": 0.0
+                    "field": 17.8
+                },
+                {
+                    "field": "Until: 07:00"
+                },
+                {
+                    "field": 20
+                },
+                {
+                    "field": "Until: 08:00"
+                },
+                {
+                    "field": 21
+                },
+                {
+                    "field": "Until: 09:00"
+                },
+                {
+                    "field": 21
+                },
+                {
+                    "field": "Until: 10:00"
+                },
+                {
+                    "field": 21
+                },
+                {
+                    "field": "Until: 11:00"
+                },
+                {
+                    "field": 20.4444444444444
+                },
+                {
+                    "field": "Until: 12:00"
+                },
+                {
+                    "field": 21
+                },
+                {
+                    "field": "Until: 13:00"
+                },
+                {
+                    "field": 20.4444444444444
+                },
+                {
+                    "field": "Until: 14:00"
+                },
+                {
+                    "field": 21
+                },
+                {
+                    "field": "Until: 15:00"
+                },
+                {
+                    "field": 20.4444444444444
+                },
+                {
+                    "field": "Until: 16:00"
+                },
+                {
+                    "field": 21
+                },
+                {
+                    "field": "Until: 17:00"
+                },
+                {
+                    "field": 21
+                },
+                {
+                    "field": "Until: 18:00"
+                },
+                {
+                    "field": 21
+                },
+                {
+                    "field": "Until: 19:00"
+                },
+                {
+                    "field": 21
+                },
+                {
+                    "field": "Until: 20:00"
+                },
+                {
+                    "field": 21
+                },
+                {
+                    "field": "Until: 21:00"
+                },
+                {
+                    "field": 21
                 },
                 {
                     "field": "Until: 22:00"
                 },
                 {
-                    "field": 1.0
+                    "field": 21
+                },
+                {
+                    "field": "Until: 23:00"
+                },
+                {
+                    "field": 15.6
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.0
+                    "field": 15.6
                 },
                 {
-                    "field": "For: Saturday WinterDesignDay"
+                    "field": "For: Saturday"
+                },
+                {
+                    "field": "Until: 01:00"
+                },
+                {
+                    "field": 15.6
+                },
+                {
+                    "field": "Until: 02:00"
+                },
+                {
+                    "field": 15.6
+                },
+                {
+                    "field": "Until: 03:00"
+                },
+                {
+                    "field": 15.6
+                },
+                {
+                    "field": "Until: 04:00"
+                },
+                {
+                    "field": 15.6
+                },
+                {
+                    "field": "Until: 05:00"
+                },
+                {
+                    "field": 15.6
                 },
                 {
                     "field": "Until: 06:00"
                 },
                 {
-                    "field": 0.0
+                    "field": 17.6
+                },
+                {
+                    "field": "Until: 07:00"
+                },
+                {
+                    "field": 20
+                },
+                {
+                    "field": "Until: 08:00"
+                },
+                {
+                    "field": 21
+                },
+                {
+                    "field": "Until: 09:00"
+                },
+                {
+                    "field": 21
+                },
+                {
+                    "field": "Until: 10:00"
+                },
+                {
+                    "field": 21
+                },
+                {
+                    "field": "Until: 11:00"
+                },
+                {
+                    "field": 20.4444444444444
+                },
+                {
+                    "field": "Until: 12:00"
+                },
+                {
+                    "field": 21
+                },
+                {
+                    "field": "Until: 13:00"
+                },
+                {
+                    "field": 20.4444444444444
+                },
+                {
+                    "field": "Until: 14:00"
+                },
+                {
+                    "field": 21
+                },
+                {
+                    "field": "Until: 15:00"
+                },
+                {
+                    "field": 20.4444444444444
+                },
+                {
+                    "field": "Until: 16:00"
+                },
+                {
+                    "field": 21
+                },
+                {
+                    "field": "Until: 17:00"
+                },
+                {
+                    "field": 21
                 },
                 {
                     "field": "Until: 18:00"
                 },
                 {
-                    "field": 1.0
+                    "field": 15.6
+                },
+                {
+                    "field": "Until: 19:00"
+                },
+                {
+                    "field": 15.6
+                },
+                {
+                    "field": "Until: 20:00"
+                },
+                {
+                    "field": 15.6
+                },
+                {
+                    "field": "Until: 21:00"
+                },
+                {
+                    "field": 15.6
+                },
+                {
+                    "field": "Until: 22:00"
+                },
+                {
+                    "field": 15.6
+                },
+                {
+                    "field": "Until: 23:00"
+                },
+                {
+                    "field": 15.6
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.0
+                    "field": 15.6
+                },
+                {
+                    "field": "For: WinterDesignDay"
+                },
+                {
+                    "field": "Until: 05:00"
+                },
+                {
+                    "field": 15.6
+                },
+                {
+                    "field": "Until: 06:00"
+                },
+                {
+                    "field": 17.6
+                },
+                {
+                    "field": "Until: 07:00"
+                },
+                {
+                    "field": 19.6
+                },
+                {
+                    "field": "Until: 22:00"
+                },
+                {
+                    "field": 21.0
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 15.6
+                },
+                {
+                    "field": "For SummerDesignDay"
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 15.6
                 },
                 {
                     "field": "For:Sunday Holidays AllOtherDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.0
+                    "field": 15.6
                 }
             ],
-            "schedule_type_limits_name": "on/off"
+            "schedule_type_limits_name": "Temperature"
         },
-        "HW-Loop-Temp-Schedule": {
+        "HVACOperationSchd": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
-                    "field": "For: AllDays"
+                    "field": "For: Weekdays SummerDesignDay"
+                },
+                {
+                    "field": "Until: 06:00"
+                },
+                {
+                    "field": 0.0
+                },
+                {
+                    "field": "Until: 22:00"
+                },
+                {
+                    "field": 1.0
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 60.0
+                    "field": 0.0
+                },
+                {
+                    "field": "For: Saturday WinterDesignDay"
+                },
+                {
+                    "field": "Until: 06:00"
+                },
+                {
+                    "field": 0.0
+                },
+                {
+                    "field": "Until: 18:00"
+                },
+                {
+                    "field": 1.0
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0.0
+                },
+                {
+                    "field": "For:Sunday Holidays AllOtherDays"
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0.0
                 }
             ],
-            "schedule_type_limits_name": "Temperature"
+            "schedule_type_limits_name": "on/off"
         },
-        "Heat-Supply-Air-Temp-Sch": {
+        "HW-Loop-Temp-Schedule": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 12.8
+                    "field": 60.0
                 }
             ],
             "schedule_type_limits_name": "Temperature"
         },
         "Hours_of_operation": {
             "data": [
                 {
@@ -12570,202 +13030,671 @@
                 },
                 {
                     "field": 1.0
                 }
             ],
             "schedule_type_limits_name": "fraction"
         },
-        "Perimeter_bot_ZN_1 sub cat Latent fract sched": {
+        "PERIMETER_MID_ZN_2_MDP_Sch": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
-                    "field": "For: AllDays"
+                    "field": "For: Weekdays"
                 },
                 {
-                    "field": "Until: 24:00"
+                    "field": "Until: 01:00"
                 },
                 {
-                    "field": 0.05
-                }
-            ],
-            "schedule_type_limits_name": "Fraction"
-        },
-        "Perimeter_bot_ZN_1 sub cat Sensible fract sched": {
-            "data": [
+                    "field": 0.097
+                },
                 {
-                    "field": "Through: 12/31"
+                    "field": "Until: 02:00"
                 },
                 {
-                    "field": "For: AllDays"
+                    "field": 0.097
                 },
                 {
-                    "field": "Until: 24:00"
+                    "field": "Until: 03:00"
                 },
                 {
-                    "field": 0.2
-                }
-            ],
-            "schedule_type_limits_name": "Fraction"
-        },
-        "Perimeter_bot_ZN_1 sub cat Temp Sched": {
-            "data": [
+                    "field": 0.097
+                },
                 {
-                    "field": "Through: 12/31"
+                    "field": "Until: 04:00"
                 },
                 {
-                    "field": "For: AllDays"
+                    "field": 0.097
                 },
                 {
-                    "field": "Until: 24:00"
+                    "field": "Until: 05:00"
                 },
                 {
-                    "field": 60.0
-                }
-            ],
-            "schedule_type_limits_name": "Temperature"
-        },
-        "Perimeter_bot_ZN_1 sub catHot Supply Temp Sched": {
-            "data": [
+                    "field": 0.097
+                },
                 {
-                    "field": "Through: 12/31"
+                    "field": "Until: 06:00"
                 },
                 {
-                    "field": "For: AllDays"
+                    "field": 0.097
                 },
                 {
-                    "field": "Until: 24:00"
+                    "field": "Until: 07:00"
                 },
                 {
-                    "field": 55
-                }
-            ],
-            "schedule_type_limits_name": "Temperature"
-        },
-        "Perimeter_bot_ZN_2 sub cat Latent fract sched": {
-            "data": [
+                    "field": 0.097
+                },
                 {
-                    "field": "Through: 12/31"
+                    "field": "Until: 08:00"
                 },
                 {
-                    "field": "For: AllDays"
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 09:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 10:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 11:00"
+                },
+                {
+                    "field": 0.01
+                },
+                {
+                    "field": "Until: 12:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 13:00"
+                },
+                {
+                    "field": 0.01
+                },
+                {
+                    "field": "Until: 14:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 15:00"
+                },
+                {
+                    "field": 0.01
+                },
+                {
+                    "field": "Until: 16:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 17:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 18:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 19:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 20:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 21:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 22:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 23:00"
+                },
+                {
+                    "field": 0.097
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.05
-                }
-            ],
-            "schedule_type_limits_name": "Fraction"
-        },
-        "Perimeter_bot_ZN_2 sub cat Sensible fract sched": {
-            "data": [
+                    "field": 0.097
+                },
                 {
-                    "field": "Through: 12/31"
+                    "field": "For: Saturday"
                 },
                 {
-                    "field": "For: AllDays"
+                    "field": "Until: 01:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 02:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 03:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 04:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 05:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 06:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 07:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 08:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 09:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 10:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 11:00"
+                },
+                {
+                    "field": 0.01
+                },
+                {
+                    "field": "Until: 12:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 13:00"
+                },
+                {
+                    "field": 0.01
+                },
+                {
+                    "field": "Until: 14:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 15:00"
+                },
+                {
+                    "field": 0.01
+                },
+                {
+                    "field": "Until: 16:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 17:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 18:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 19:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 20:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 21:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 22:00"
+                },
+                {
+                    "field": 0.097
+                },
+                {
+                    "field": "Until: 23:00"
+                },
+                {
+                    "field": 0.097
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.2
+                    "field": 0.097
+                },
+                {
+                    "field": "For: AllOtherDays"
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 0.097
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_bot_ZN_2 sub cat Temp Sched": {
+        "PERIMETER_MID_ZN_2_OA_Mult": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
-                    "field": "For: AllDays"
+                    "field": "For: Weekdays"
                 },
                 {
-                    "field": "Until: 24:00"
+                    "field": "Until: 01:00"
                 },
                 {
-                    "field": 60.0
-                }
-            ],
-            "schedule_type_limits_name": "Temperature"
-        },
-        "Perimeter_bot_ZN_2 sub catHot Supply Temp Sched": {
-            "data": [
+                    "field": 1
+                },
                 {
-                    "field": "Through: 12/31"
+                    "field": "Until: 02:00"
                 },
                 {
-                    "field": "For: AllDays"
+                    "field": 1
+                },
+                {
+                    "field": "Until: 03:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 04:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 05:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 06:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 07:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 08:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 09:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 10:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 11:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 12:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 13:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 14:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 15:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 16:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 17:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 18:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 19:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 20:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 21:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 22:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 23:00"
+                },
+                {
+                    "field": 1
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 55
-                }
-            ],
-            "schedule_type_limits_name": "Temperature"
-        },
-        "Perimeter_bot_ZN_3 sub cat Latent fract sched": {
-            "data": [
+                    "field": 1
+                },
                 {
-                    "field": "Through: 12/31"
+                    "field": "For: Saturday"
                 },
                 {
-                    "field": "For: AllDays"
+                    "field": "Until: 01:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 02:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 03:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 04:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 05:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 06:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 07:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 08:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 09:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 10:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 11:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 12:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 13:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 14:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 15:00"
+                },
+                {
+                    "field": 0
+                },
+                {
+                    "field": "Until: 16:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 17:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 18:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 19:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 20:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 21:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 22:00"
+                },
+                {
+                    "field": 1
+                },
+                {
+                    "field": "Until: 23:00"
+                },
+                {
+                    "field": 1
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.05
+                    "field": 1
+                },
+                {
+                    "field": "For: AllOtherDays"
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 1
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_bot_ZN_3 sub cat Sensible fract sched": {
+        "Perimeter_bot_ZN_1 sub cat Latent fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.2
+                    "field": 0.05
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_bot_ZN_3 sub cat Temp Sched": {
+        "Perimeter_bot_ZN_1 sub cat Sensible fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 60.0
+                    "field": 0.2
                 }
             ],
-            "schedule_type_limits_name": "Temperature"
+            "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_bot_ZN_3 sub catHot Supply Temp Sched": {
+        "Perimeter_bot_ZN_1 sub catHot Supply Temp Sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
@@ -12774,15 +13703,15 @@
                 },
                 {
                     "field": 55
                 }
             ],
             "schedule_type_limits_name": "Temperature"
         },
-        "Perimeter_bot_ZN_4 sub cat Latent fract sched": {
+        "Perimeter_bot_ZN_2 sub cat Latent fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
@@ -12791,15 +13720,15 @@
                 },
                 {
                     "field": 0.05
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_bot_ZN_4 sub cat Sensible fract sched": {
+        "Perimeter_bot_ZN_2 sub cat Sensible fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
@@ -12808,168 +13737,168 @@
                 },
                 {
                     "field": 0.2
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_bot_ZN_4 sub cat Temp Sched": {
+        "Perimeter_bot_ZN_2 sub catHot Supply Temp Sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 60.0
+                    "field": 55
                 }
             ],
             "schedule_type_limits_name": "Temperature"
         },
-        "Perimeter_bot_ZN_4 sub catHot Supply Temp Sched": {
+        "Perimeter_bot_ZN_3 sub cat Latent fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 55
+                    "field": 0.05
                 }
             ],
-            "schedule_type_limits_name": "Temperature"
+            "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_mid_ZN_1 sub cat Latent fract sched": {
+        "Perimeter_bot_ZN_3 sub cat Sensible fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.05
+                    "field": 0.2
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_mid_ZN_1 sub cat Sensible fract sched": {
+        "Perimeter_bot_ZN_3 sub catHot Supply Temp Sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.2
+                    "field": 55
                 }
             ],
-            "schedule_type_limits_name": "Fraction"
+            "schedule_type_limits_name": "Temperature"
         },
-        "Perimeter_mid_ZN_1 sub cat Temp Sched": {
+        "Perimeter_bot_ZN_4 sub cat Latent fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 60.0
+                    "field": 0.05
                 }
             ],
-            "schedule_type_limits_name": "Temperature"
+            "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_mid_ZN_1 sub catHot Supply Temp Sched": {
+        "Perimeter_bot_ZN_4 sub cat Sensible fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 55
+                    "field": 0.2
                 }
             ],
-            "schedule_type_limits_name": "Temperature"
+            "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_mid_ZN_2 sub cat Latent fract sched": {
+        "Perimeter_bot_ZN_4 sub catHot Supply Temp Sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.05
+                    "field": 55
                 }
             ],
-            "schedule_type_limits_name": "Fraction"
+            "schedule_type_limits_name": "Temperature"
         },
-        "Perimeter_mid_ZN_2 sub cat Sensible fract sched": {
+        "Perimeter_mid_ZN_1 sub cat Latent fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.2
+                    "field": 0.05
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_mid_ZN_2 sub cat Temp Sched": {
+        "Perimeter_mid_ZN_1 sub cat Sensible fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 60.0
+                    "field": 0.2
                 }
             ],
-            "schedule_type_limits_name": "Temperature"
+            "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_mid_ZN_2 sub catHot Supply Temp Sched": {
+        "Perimeter_mid_ZN_1 sub catHot Supply Temp Sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
@@ -12978,15 +13907,15 @@
                 },
                 {
                     "field": 55
                 }
             ],
             "schedule_type_limits_name": "Temperature"
         },
-        "Perimeter_mid_ZN_3 sub cat Latent fract sched": {
+        "Perimeter_mid_ZN_2 sub cat Latent fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
@@ -12995,15 +13924,15 @@
                 },
                 {
                     "field": 0.05
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_mid_ZN_3 sub cat Sensible fract sched": {
+        "Perimeter_mid_ZN_2 sub cat Sensible fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
@@ -13012,166 +13941,166 @@
                 },
                 {
                     "field": 0.2
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_mid_ZN_3 sub cat Temp Sched": {
+        "Perimeter_mid_ZN_2 sub catHot Supply Temp Sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 60.0
+                    "field": 55
                 }
             ],
             "schedule_type_limits_name": "Temperature"
         },
-        "Perimeter_mid_ZN_3 sub catHot Supply Temp Sched": {
+        "Perimeter_mid_ZN_3 sub cat Latent fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 55
+                    "field": 0.05
                 }
             ],
-            "schedule_type_limits_name": "Temperature"
+            "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_mid_ZN_4 sub cat Latent fract sched": {
+        "Perimeter_mid_ZN_3 sub cat Sensible fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.05
+                    "field": 0.2
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_mid_ZN_4 sub cat Sensible fract sched": {
+        "Perimeter_mid_ZN_3 sub catHot Supply Temp Sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.2
+                    "field": 55
                 }
             ],
-            "schedule_type_limits_name": "Fraction"
+            "schedule_type_limits_name": "Temperature"
         },
-        "Perimeter_mid_ZN_4 sub cat Temp Sched": {
+        "Perimeter_mid_ZN_4 sub cat Latent fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 60.0
+                    "field": 0.05
                 }
             ],
-            "schedule_type_limits_name": "Temperature"
+            "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_mid_ZN_4 sub catHot Supply Temp Sched": {
+        "Perimeter_mid_ZN_4 sub cat Sensible fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 55
+                    "field": 0.2
                 }
             ],
-            "schedule_type_limits_name": "Temperature"
+            "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_top_ZN_1 sub cat Latent fract sched": {
+        "Perimeter_mid_ZN_4 sub catHot Supply Temp Sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.05
+                    "field": 55
                 }
             ],
-            "schedule_type_limits_name": "Fraction"
+            "schedule_type_limits_name": "Temperature"
         },
-        "Perimeter_top_ZN_1 sub cat Sensible fract sched": {
+        "Perimeter_top_ZN_1 sub cat Latent fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 0.2
+                    "field": 0.05
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_top_ZN_1 sub cat Temp Sched": {
+        "Perimeter_top_ZN_1 sub cat Sensible fract sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
                 },
                 {
                     "field": "Until: 24:00"
                 },
                 {
-                    "field": 60.0
+                    "field": 0.2
                 }
             ],
-            "schedule_type_limits_name": "Temperature"
+            "schedule_type_limits_name": "Fraction"
         },
         "Perimeter_top_ZN_1 sub catHot Supply Temp Sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
@@ -13216,31 +14145,14 @@
                 },
                 {
                     "field": 0.2
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_top_ZN_2 sub cat Temp Sched": {
-            "data": [
-                {
-                    "field": "Through: 12/31"
-                },
-                {
-                    "field": "For: AllDays"
-                },
-                {
-                    "field": "Until: 24:00"
-                },
-                {
-                    "field": 60.0
-                }
-            ],
-            "schedule_type_limits_name": "Temperature"
-        },
         "Perimeter_top_ZN_2 sub catHot Supply Temp Sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
@@ -13284,31 +14196,14 @@
                 },
                 {
                     "field": 0.2
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_top_ZN_3 sub cat Temp Sched": {
-            "data": [
-                {
-                    "field": "Through: 12/31"
-                },
-                {
-                    "field": "For: AllDays"
-                },
-                {
-                    "field": "Until: 24:00"
-                },
-                {
-                    "field": 60.0
-                }
-            ],
-            "schedule_type_limits_name": "Temperature"
-        },
         "Perimeter_top_ZN_3 sub catHot Supply Temp Sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
@@ -13352,31 +14247,14 @@
                 },
                 {
                     "field": 0.2
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         },
-        "Perimeter_top_ZN_4 sub cat Temp Sched": {
-            "data": [
-                {
-                    "field": "Through: 12/31"
-                },
-                {
-                    "field": "For: AllDays"
-                },
-                {
-                    "field": "Until: 24:00"
-                },
-                {
-                    "field": 60.0
-                }
-            ],
-            "schedule_type_limits_name": "Temperature"
-        },
         "Perimeter_top_ZN_4 sub catHot Supply Temp Sched": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
@@ -13488,14 +14366,31 @@
                 },
                 {
                     "field": 60.0
                 }
             ],
             "schedule_type_limits_name": "Temperature"
         },
+        "Supply-Air-Temp-Sch": {
+            "data": [
+                {
+                    "field": "Through: 12/31"
+                },
+                {
+                    "field": "For: AllDays"
+                },
+                {
+                    "field": "Until: 24:00"
+                },
+                {
+                    "field": 12.8
+                }
+            ],
+            "schedule_type_limits_name": "Temperature"
+        },
         "WORK_EFF_SCH": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
                     "field": "For: AllDays"
@@ -13506,14 +14401,25 @@
                 {
                     "field": 0.0
                 }
             ],
             "schedule_type_limits_name": "Fraction"
         }
     },
+    "Schedule:Constant": {
+        "VAV_BOT Max OA Fraction": {
+            "hourly_value": 1.0
+        },
+        "VAV_MID Max OA Fraction": {
+            "hourly_value": 1.0
+        },
+        "VAV_TOP Max OA Fraction": {
+            "hourly_value": 1.0
+        }
+    },
     "ScheduleTypeLimits": {
         "Any Number": {},
         "Control Type": {
             "lower_limit_value": 0,
             "numeric_type": "Discrete",
             "upper_limit_value": 4
         },
@@ -13651,28 +14557,28 @@
             "do_system_sizing_calculation": "Yes",
             "do_zone_sizing_calculation": "Yes",
             "maximum_number_of_hvac_sizing_simulation_passes": 1,
             "run_simulation_for_sizing_periods": "Yes",
             "run_simulation_for_weather_file_run_periods": "Yes"
         }
     },
-    "Site:GroundTemperature:BuildingSurface": {
-        "Site:GroundTemperature:BuildingSurface 1": {
-            "april_ground_temperature": 20.53,
-            "august_ground_temperature": 23.35,
-            "december_ground_temperature": 20.61,
-            "february_ground_temperature": 20.49,
-            "january_ground_temperature": 20.53,
-            "july_ground_temperature": 23.26,
-            "june_ground_temperature": 22.84,
-            "march_ground_temperature": 20.52,
-            "may_ground_temperature": 20.6,
-            "november_ground_temperature": 20.76,
-            "october_ground_temperature": 21.14,
-            "september_ground_temperature": 23.38
+    "Site:GroundTemperature:FCfactorMethod": {
+        "Site:GroundTemperature:FCfactorMethod 1": {
+            "april_ground_temperature": 0.8,
+            "august_ground_temperature": 13.7,
+            "december_ground_temperature": 18.5,
+            "february_ground_temperature": 3.0,
+            "january_ground_temperature": 7.1,
+            "july_ground_temperature": 6.1,
+            "june_ground_temperature": 4.8,
+            "march_ground_temperature": -1.0,
+            "may_ground_temperature": -0.2,
+            "november_ground_temperature": 21.7,
+            "october_ground_temperature": 22.7,
+            "september_ground_temperature": 22.2
         }
     },
     "Site:Location": {
         "Denver-Aurora-Buckley.AFB_CO_USA WMO=724695": {
             "elevation": 1726.0,
             "latitude": 39.72,
             "longitude": -104.75,
@@ -13686,15 +14592,15 @@
             "maximum_difference_in_monthly_average_outdoor_air_temperatures": 23.7
         }
     },
     "Sizing:Parameters": {
         "Sizing:Parameters 1": {
             "cooling_sizing_factor": 1.0,
             "heating_sizing_factor": 1.0,
-            "timesteps_in_averaging_window": 8
+            "timesteps_in_averaging_window": 6
         }
     },
     "Sizing:Plant": {
         "Sizing:Plant 1": {
             "design_loop_exit_temperature": 60,
             "loop_design_temperature_difference": 5.0,
             "loop_type": "Heating",
@@ -13702,424 +14608,391 @@
         }
     },
     "Sizing:System": {
         "Sizing:System 1": {
             "100_outdoor_air_in_cooling": "No",
             "100_outdoor_air_in_heating": "No",
             "airloop_name": "PACU_VAV_bot",
-            "central_cooling_capacity_control_method": "OnOff",
             "central_cooling_design_supply_air_humidity_ratio": 0.0085,
             "central_cooling_design_supply_air_temperature": 12.8,
             "central_heating_design_supply_air_humidity_ratio": 0.008,
             "central_heating_design_supply_air_temperature": 12.8,
             "central_heating_maximum_system_air_flow_ratio": 0.3,
-            "cooling_design_capacity": "Autosize",
-            "cooling_design_capacity_method": "CoolingDesignCapacity",
             "cooling_supply_air_flow_rate": 0.0,
             "cooling_supply_air_flow_rate_method": "DesignDay",
-            "design_outdoor_air_flow_rate": 1.19508883333333,
-            "heating_design_capacity": "Autosize",
-            "heating_design_capacity_method": "HeatingDesignCapacity",
+            "design_outdoor_air_flow_rate": 0.9561,
             "heating_supply_air_flow_rate": 0.0,
             "heating_supply_air_flow_rate_method": "DesignDay",
             "precool_design_humidity_ratio": 0.008,
             "precool_design_temperature": 12.8,
             "preheat_design_humidity_ratio": 0.008,
             "preheat_design_temperature": 7.0,
             "system_outdoor_air_method": "ZoneSum",
             "type_of_load_to_size_on": "Sensible",
-            "type_of_zone_sum_to_use": "Coincident",
-            "zone_maximum_outdoor_air_fraction": 1.0
+            "type_of_zone_sum_to_use": "Coincident"
         },
         "Sizing:System 2": {
             "100_outdoor_air_in_cooling": "No",
             "100_outdoor_air_in_heating": "No",
             "airloop_name": "PACU_VAV_mid",
-            "central_cooling_capacity_control_method": "OnOff",
             "central_cooling_design_supply_air_humidity_ratio": 0.0085,
             "central_cooling_design_supply_air_temperature": 12.8,
             "central_heating_design_supply_air_humidity_ratio": 0.008,
             "central_heating_design_supply_air_temperature": 12.8,
             "central_heating_maximum_system_air_flow_ratio": 0.3,
-            "cooling_design_capacity": "Autosize",
-            "cooling_design_capacity_method": "CoolingDesignCapacity",
             "cooling_supply_air_flow_rate": 0.0,
             "cooling_supply_air_flow_rate_method": "DesignDay",
-            "design_outdoor_air_flow_rate": 1.19508883333333,
-            "heating_design_capacity": "Autosize",
-            "heating_design_capacity_method": "HeatingDesignCapacity",
+            "design_outdoor_air_flow_rate": 0.9561,
             "heating_supply_air_flow_rate": 0.0,
             "heating_supply_air_flow_rate_method": "DesignDay",
             "precool_design_humidity_ratio": 0.008,
             "precool_design_temperature": 12.8,
             "preheat_design_humidity_ratio": 0.008,
             "preheat_design_temperature": 7.0,
             "system_outdoor_air_method": "ZoneSum",
             "type_of_load_to_size_on": "Sensible",
-            "type_of_zone_sum_to_use": "Coincident",
-            "zone_maximum_outdoor_air_fraction": 1.0
+            "type_of_zone_sum_to_use": "Coincident"
         },
         "Sizing:System 3": {
             "100_outdoor_air_in_cooling": "No",
             "100_outdoor_air_in_heating": "No",
             "airloop_name": "PACU_VAV_top",
-            "central_cooling_capacity_control_method": "OnOff",
             "central_cooling_design_supply_air_humidity_ratio": 0.0085,
             "central_cooling_design_supply_air_temperature": 12.8,
             "central_heating_design_supply_air_humidity_ratio": 0.008,
             "central_heating_design_supply_air_temperature": 12.8,
             "central_heating_maximum_system_air_flow_ratio": 0.3,
-            "cooling_design_capacity": "Autosize",
-            "cooling_design_capacity_method": "CoolingDesignCapacity",
             "cooling_supply_air_flow_rate": 0.0,
             "cooling_supply_air_flow_rate_method": "DesignDay",
-            "design_outdoor_air_flow_rate": 1.1865461959444,
-            "heating_design_capacity": "Autosize",
-            "heating_design_capacity_method": "HeatingDesignCapacity",
+            "design_outdoor_air_flow_rate": 0.9561,
             "heating_supply_air_flow_rate": 0.0,
             "heating_supply_air_flow_rate_method": "DesignDay",
             "precool_design_humidity_ratio": 0.008,
             "precool_design_temperature": 12.8,
             "preheat_design_humidity_ratio": 0.008,
             "preheat_design_temperature": 7.0,
             "system_outdoor_air_method": "ZoneSum",
             "type_of_load_to_size_on": "Sensible",
-            "type_of_zone_sum_to_use": "Coincident",
-            "zone_maximum_outdoor_air_fraction": 1.0
+            "type_of_zone_sum_to_use": "Coincident"
         }
     },
     "Sizing:Zone": {
         "Sizing:Zone 1": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
             "cooling_design_air_flow_rate": 0.0,
             "cooling_minimum_air_flow": 0.0,
             "cooling_minimum_air_flow_fraction": 0.0,
             "dedicated_outdoor_air_high_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_low_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_system_control_strategy": "NeutralSupplyAir",
             "design_specification_outdoor_air_object_name": "SZ DSOA Core_bottom",
+            "design_specification_zone_air_distribution_object_name": "VAV_Zone_AirDistribution",
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0.0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.0085,
             "zone_cooling_design_supply_air_temperature": 12.8,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.008,
             "zone_heating_design_supply_air_temperature": 40.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "Core_bottom"
         },
         "Sizing:Zone 10": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
             "cooling_design_air_flow_rate": 0.0,
             "cooling_minimum_air_flow": 0.0,
             "cooling_minimum_air_flow_fraction": 0.0,
             "dedicated_outdoor_air_high_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_low_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_system_control_strategy": "NeutralSupplyAir",
             "design_specification_outdoor_air_object_name": "SZ DSOA Perimeter_bot_ZN_1",
+            "design_specification_zone_air_distribution_object_name": "VAV_Zone_AirDistribution",
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0.0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.0085,
             "zone_cooling_design_supply_air_temperature": 12.8,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.008,
             "zone_heating_design_supply_air_temperature": 40.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "Perimeter_bot_ZN_1"
         },
         "Sizing:Zone 11": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
             "cooling_design_air_flow_rate": 0.0,
             "cooling_minimum_air_flow": 0.0,
             "cooling_minimum_air_flow_fraction": 0.0,
             "dedicated_outdoor_air_high_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_low_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_system_control_strategy": "NeutralSupplyAir",
             "design_specification_outdoor_air_object_name": "SZ DSOA Perimeter_bot_ZN_4",
+            "design_specification_zone_air_distribution_object_name": "VAV_Zone_AirDistribution",
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0.0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.0085,
             "zone_cooling_design_supply_air_temperature": 12.8,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.008,
             "zone_heating_design_supply_air_temperature": 40.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "Perimeter_bot_ZN_4"
         },
         "Sizing:Zone 12": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
             "cooling_design_air_flow_rate": 0.0,
             "cooling_minimum_air_flow": 0.0,
             "cooling_minimum_air_flow_fraction": 0.0,
             "dedicated_outdoor_air_high_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_low_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_system_control_strategy": "NeutralSupplyAir",
             "design_specification_outdoor_air_object_name": "SZ DSOA Perimeter_mid_ZN_3",
+            "design_specification_zone_air_distribution_object_name": "VAV_Zone_AirDistribution",
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0.0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.0085,
             "zone_cooling_design_supply_air_temperature": 12.8,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.008,
             "zone_heating_design_supply_air_temperature": 40.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "Perimeter_mid_ZN_3"
         },
         "Sizing:Zone 13": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
             "cooling_design_air_flow_rate": 0.0,
             "cooling_minimum_air_flow": 0.0,
             "cooling_minimum_air_flow_fraction": 0.0,
             "dedicated_outdoor_air_high_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_low_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_system_control_strategy": "NeutralSupplyAir",
             "design_specification_outdoor_air_object_name": "SZ DSOA Perimeter_mid_ZN_2",
+            "design_specification_zone_air_distribution_object_name": "VAV_Zone_AirDistribution",
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0.0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.0085,
             "zone_cooling_design_supply_air_temperature": 12.8,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.008,
             "zone_heating_design_supply_air_temperature": 40.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "Perimeter_mid_ZN_2"
         },
         "Sizing:Zone 14": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
             "cooling_design_air_flow_rate": 0.0,
             "cooling_minimum_air_flow": 0.0,
             "cooling_minimum_air_flow_fraction": 0.0,
             "dedicated_outdoor_air_high_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_low_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_system_control_strategy": "NeutralSupplyAir",
             "design_specification_outdoor_air_object_name": "SZ DSOA Perimeter_mid_ZN_1",
+            "design_specification_zone_air_distribution_object_name": "VAV_Zone_AirDistribution",
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0.0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.0085,
             "zone_cooling_design_supply_air_temperature": 12.8,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.008,
             "zone_heating_design_supply_air_temperature": 40.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "Perimeter_mid_ZN_1"
         },
         "Sizing:Zone 15": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
             "cooling_design_air_flow_rate": 0.0,
             "cooling_minimum_air_flow": 0.0,
             "cooling_minimum_air_flow_fraction": 0.0,
             "dedicated_outdoor_air_high_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_low_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_system_control_strategy": "NeutralSupplyAir",
             "design_specification_outdoor_air_object_name": "SZ DSOA Perimeter_mid_ZN_4",
+            "design_specification_zone_air_distribution_object_name": "VAV_Zone_AirDistribution",
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0.0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.0085,
             "zone_cooling_design_supply_air_temperature": 12.8,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.008,
             "zone_heating_design_supply_air_temperature": 40.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "Perimeter_mid_ZN_4"
         },
         "Sizing:Zone 2": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
             "cooling_design_air_flow_rate": 0.0,
             "cooling_minimum_air_flow": 0.0,
             "cooling_minimum_air_flow_fraction": 0.0,
             "dedicated_outdoor_air_high_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_low_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_system_control_strategy": "NeutralSupplyAir",
             "design_specification_outdoor_air_object_name": "SZ DSOA Core_mid",
+            "design_specification_zone_air_distribution_object_name": "VAV_Zone_AirDistribution",
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0.0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.0085,
             "zone_cooling_design_supply_air_temperature": 12.8,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.008,
             "zone_heating_design_supply_air_temperature": 40.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "Core_mid"
         },
         "Sizing:Zone 3": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
             "cooling_design_air_flow_rate": 0.0,
             "cooling_minimum_air_flow": 0.0,
             "cooling_minimum_air_flow_fraction": 0.0,
             "dedicated_outdoor_air_high_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_low_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_system_control_strategy": "NeutralSupplyAir",
             "design_specification_outdoor_air_object_name": "SZ DSOA Core_top",
+            "design_specification_zone_air_distribution_object_name": "VAV_Zone_AirDistribution",
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0.0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.0085,
             "zone_cooling_design_supply_air_temperature": 12.8,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.008,
             "zone_heating_design_supply_air_temperature": 40.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "Core_top"
         },
         "Sizing:Zone 4": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
             "cooling_design_air_flow_rate": 0.0,
             "cooling_minimum_air_flow": 0.0,
             "cooling_minimum_air_flow_fraction": 0.0,
             "dedicated_outdoor_air_high_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_low_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_system_control_strategy": "NeutralSupplyAir",
             "design_specification_outdoor_air_object_name": "SZ DSOA Perimeter_top_ZN_3",
+            "design_specification_zone_air_distribution_object_name": "VAV_Zone_AirDistribution",
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0.0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.0085,
             "zone_cooling_design_supply_air_temperature": 12.8,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.008,
             "zone_heating_design_supply_air_temperature": 40.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "Perimeter_top_ZN_3"
         },
         "Sizing:Zone 5": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
             "cooling_design_air_flow_rate": 0.0,
             "cooling_minimum_air_flow": 0.0,
             "cooling_minimum_air_flow_fraction": 0.0,
             "dedicated_outdoor_air_high_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_low_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_system_control_strategy": "NeutralSupplyAir",
             "design_specification_outdoor_air_object_name": "SZ DSOA Perimeter_top_ZN_2",
+            "design_specification_zone_air_distribution_object_name": "VAV_Zone_AirDistribution",
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0.0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.0085,
             "zone_cooling_design_supply_air_temperature": 12.8,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.008,
             "zone_heating_design_supply_air_temperature": 40.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "Perimeter_top_ZN_2"
         },
         "Sizing:Zone 6": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
             "cooling_design_air_flow_rate": 0.0,
             "cooling_minimum_air_flow": 0.0,
             "cooling_minimum_air_flow_fraction": 0.0,
             "dedicated_outdoor_air_high_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_low_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_system_control_strategy": "NeutralSupplyAir",
             "design_specification_outdoor_air_object_name": "SZ DSOA Perimeter_top_ZN_1",
+            "design_specification_zone_air_distribution_object_name": "VAV_Zone_AirDistribution",
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0.0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.0085,
             "zone_cooling_design_supply_air_temperature": 12.8,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.008,
             "zone_heating_design_supply_air_temperature": 40.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "Perimeter_top_ZN_1"
         },
         "Sizing:Zone 7": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
             "cooling_design_air_flow_rate": 0.0,
             "cooling_minimum_air_flow": 0.0,
             "cooling_minimum_air_flow_fraction": 0.0,
             "dedicated_outdoor_air_high_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_low_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_system_control_strategy": "NeutralSupplyAir",
             "design_specification_outdoor_air_object_name": "SZ DSOA Perimeter_top_ZN_4",
+            "design_specification_zone_air_distribution_object_name": "VAV_Zone_AirDistribution",
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0.0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.0085,
             "zone_cooling_design_supply_air_temperature": 12.8,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.008,
             "zone_heating_design_supply_air_temperature": 40.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "Perimeter_top_ZN_4"
         },
         "Sizing:Zone 8": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
             "cooling_design_air_flow_rate": 0.0,
             "cooling_minimum_air_flow": 0.0,
             "cooling_minimum_air_flow_fraction": 0.0,
             "dedicated_outdoor_air_high_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_low_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_system_control_strategy": "NeutralSupplyAir",
             "design_specification_outdoor_air_object_name": "SZ DSOA Perimeter_bot_ZN_3",
+            "design_specification_zone_air_distribution_object_name": "VAV_Zone_AirDistribution",
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0.0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.0085,
             "zone_cooling_design_supply_air_temperature": 12.8,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.008,
             "zone_heating_design_supply_air_temperature": 40.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "Perimeter_bot_ZN_3"
         },
         "Sizing:Zone 9": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
             "cooling_design_air_flow_rate": 0.0,
             "cooling_minimum_air_flow": 0.0,
             "cooling_minimum_air_flow_fraction": 0.0,
             "dedicated_outdoor_air_high_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_low_setpoint_temperature_for_design": "Autosize",
             "dedicated_outdoor_air_system_control_strategy": "NeutralSupplyAir",
             "design_specification_outdoor_air_object_name": "SZ DSOA Perimeter_bot_ZN_2",
+            "design_specification_zone_air_distribution_object_name": "VAV_Zone_AirDistribution",
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0.0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.0085,
             "zone_cooling_design_supply_air_temperature": 12.8,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_cooling_sizing_factor": 0.0,
             "zone_heating_design_supply_air_humidity_ratio": 0.008,
             "zone_heating_design_supply_air_temperature": 40.0,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_heating_sizing_factor": 0.0,
             "zone_or_zonelist_name": "Perimeter_bot_ZN_2"
         }
     },
     "SizingPeriod:DesignDay": {
         "Denver-Aurora-Buckley.AFB_CO_USA Ann Clg .4% Condns DB=>MWB": {
             "ashrae_clear_sky_optical_depth_for_beam_irradiance_taub_": 0.423,
             "ashrae_clear_sky_optical_depth_for_diffuse_irradiance_taud_": 2.02,
@@ -14198,16 +15071,16 @@
             "heating_setpoint_temperature_schedule_name": "HTGSETP_SCH_YES_OPTIMUM"
         },
         "Perimeter_mid_ZN_1 DualSPSched": {
             "cooling_setpoint_temperature_schedule_name": "CLGSETP_SCH_YES_OPTIMUM",
             "heating_setpoint_temperature_schedule_name": "HTGSETP_SCH_YES_OPTIMUM"
         },
         "Perimeter_mid_ZN_2 DualSPSched": {
-            "cooling_setpoint_temperature_schedule_name": "CLGSETP_SCH_YES_OPTIMUM",
-            "heating_setpoint_temperature_schedule_name": "HTGSETP_SCH_YES_OPTIMUM"
+            "cooling_setpoint_temperature_schedule_name": "CLGSETP_SCH_YES_OPTIMUM_w_SB",
+            "heating_setpoint_temperature_schedule_name": "HTGSETP_SCH_YES_OPTIMUM_w_SB"
         },
         "Perimeter_mid_ZN_3 DualSPSched": {
             "cooling_setpoint_temperature_schedule_name": "CLGSETP_SCH_YES_OPTIMUM",
             "heating_setpoint_temperature_schedule_name": "HTGSETP_SCH_YES_OPTIMUM"
         },
         "Perimeter_mid_ZN_4 DualSPSched": {
             "cooling_setpoint_temperature_schedule_name": "CLGSETP_SCH_YES_OPTIMUM",
@@ -14233,15 +15106,15 @@
     "Timestep": {
         "Timestep 1": {
             "number_of_timesteps_per_hour": 4
         }
     },
     "Version": {
         "Version 1": {
-            "version_identifier": "9.5"
+            "version_identifier": "23.1"
         }
     },
     "WaterHeater:Mixed": {
         "SHWSys1 Water Heater": {
             "ambient_temperature_indicator": "Zone",
             "ambient_temperature_zone_name": "CORE_BOTTOM",
             "deadband_temperature_difference": 2.0,
@@ -14403,1156 +15276,366 @@
             ],
             "inlet_node_name": "Perimeter_top_ZN_4 sub cat Water Inlet Node",
             "outlet_node_name": "Perimeter_top_ZN_4 sub cat Water Outlet Node"
         }
     },
     "WaterUse:Equipment": {
         "Core_bottom sub cat": {
-            "end_use_subcategory": "sub cat",
+            "end_use_subcategory": "WaterUse",
             "flow_rate_fraction_schedule_name": "BLDG_SWH_SCH",
             "hot_water_supply_temperature_schedule_name": "Core_bottom sub catHot Supply Temp Sched",
             "latent_fraction_schedule_name": "Core_bottom sub cat Latent fract sched",
-            "peak_flow_rate": 3.575111e-06,
+            "peak_flow_rate": 3.57511e-06,
             "sensible_fraction_schedule_name": "Core_bottom sub cat Sensible fract sched",
-            "target_temperature_schedule_name": "Core_bottom sub cat Temp Sched",
             "zone_name": "Core_bottom"
         },
         "Core_mid sub cat": {
-            "end_use_subcategory": "sub cat",
+            "end_use_subcategory": "WaterUse",
             "flow_rate_fraction_schedule_name": "BLDG_SWH_SCH",
             "hot_water_supply_temperature_schedule_name": "Core_mid sub catHot Supply Temp Sched",
             "latent_fraction_schedule_name": "Core_mid sub cat Latent fract sched",
-            "peak_flow_rate": 3.575111e-06,
+            "peak_flow_rate": 3.57511e-06,
             "sensible_fraction_schedule_name": "Core_mid sub cat Sensible fract sched",
-            "target_temperature_schedule_name": "Core_mid sub cat Temp Sched",
             "zone_name": "Core_mid"
         },
         "Core_top sub cat": {
-            "end_use_subcategory": "sub cat",
+            "end_use_subcategory": "WaterUse",
             "flow_rate_fraction_schedule_name": "BLDG_SWH_SCH",
             "hot_water_supply_temperature_schedule_name": "Core_top sub catHot Supply Temp Sched",
             "latent_fraction_schedule_name": "Core_top sub cat Latent fract sched",
-            "peak_flow_rate": 3.575111e-06,
+            "peak_flow_rate": 3.57511e-06,
             "sensible_fraction_schedule_name": "Core_top sub cat Sensible fract sched",
-            "target_temperature_schedule_name": "Core_top sub cat Temp Sched",
             "zone_name": "Core_top"
         },
         "Perimeter_bot_ZN_1 sub cat": {
-            "end_use_subcategory": "sub cat",
+            "end_use_subcategory": "WaterUse",
             "flow_rate_fraction_schedule_name": "BLDG_SWH_SCH",
             "hot_water_supply_temperature_schedule_name": "Perimeter_bot_ZN_1 sub catHot Supply Temp Sched",
             "latent_fraction_schedule_name": "Perimeter_bot_ZN_1 sub cat Latent fract sched",
-            "peak_flow_rate": 3.575111e-06,
+            "peak_flow_rate": 3.57511e-06,
             "sensible_fraction_schedule_name": "Perimeter_bot_ZN_1 sub cat Sensible fract sched",
-            "target_temperature_schedule_name": "Perimeter_bot_ZN_1 sub cat Temp Sched",
             "zone_name": "Perimeter_bot_ZN_1"
         },
         "Perimeter_bot_ZN_2 sub cat": {
-            "end_use_subcategory": "sub cat",
+            "end_use_subcategory": "WaterUse",
             "flow_rate_fraction_schedule_name": "BLDG_SWH_SCH",
             "hot_water_supply_temperature_schedule_name": "Perimeter_bot_ZN_2 sub catHot Supply Temp Sched",
             "latent_fraction_schedule_name": "Perimeter_bot_ZN_2 sub cat Latent fract sched",
-            "peak_flow_rate": 3.575111e-06,
+            "peak_flow_rate": 3.57511e-06,
             "sensible_fraction_schedule_name": "Perimeter_bot_ZN_2 sub cat Sensible fract sched",
-            "target_temperature_schedule_name": "Perimeter_bot_ZN_2 sub cat Temp Sched",
             "zone_name": "Perimeter_bot_ZN_2"
         },
         "Perimeter_bot_ZN_3 sub cat": {
-            "end_use_subcategory": "sub cat",
+            "end_use_subcategory": "WaterUse",
             "flow_rate_fraction_schedule_name": "BLDG_SWH_SCH",
             "hot_water_supply_temperature_schedule_name": "Perimeter_bot_ZN_3 sub catHot Supply Temp Sched",
             "latent_fraction_schedule_name": "Perimeter_bot_ZN_3 sub cat Latent fract sched",
-            "peak_flow_rate": 3.575111e-06,
+            "peak_flow_rate": 3.57511e-06,
             "sensible_fraction_schedule_name": "Perimeter_bot_ZN_3 sub cat Sensible fract sched",
-            "target_temperature_schedule_name": "Perimeter_bot_ZN_3 sub cat Temp Sched",
             "zone_name": "Perimeter_bot_ZN_3"
         },
         "Perimeter_bot_ZN_4 sub cat": {
-            "end_use_subcategory": "sub cat",
+            "end_use_subcategory": "WaterUse",
             "flow_rate_fraction_schedule_name": "BLDG_SWH_SCH",
             "hot_water_supply_temperature_schedule_name": "Perimeter_bot_ZN_4 sub catHot Supply Temp Sched",
             "latent_fraction_schedule_name": "Perimeter_bot_ZN_4 sub cat Latent fract sched",
-            "peak_flow_rate": 3.575111e-06,
+            "peak_flow_rate": 3.57511e-06,
             "sensible_fraction_schedule_name": "Perimeter_bot_ZN_4 sub cat Sensible fract sched",
-            "target_temperature_schedule_name": "Perimeter_bot_ZN_4 sub cat Temp Sched",
             "zone_name": "Perimeter_bot_ZN_4"
         },
         "Perimeter_mid_ZN_1 sub cat": {
-            "end_use_subcategory": "sub cat",
+            "end_use_subcategory": "WaterUse",
             "flow_rate_fraction_schedule_name": "BLDG_SWH_SCH",
             "hot_water_supply_temperature_schedule_name": "Perimeter_mid_ZN_1 sub catHot Supply Temp Sched",
             "latent_fraction_schedule_name": "Perimeter_mid_ZN_1 sub cat Latent fract sched",
-            "peak_flow_rate": 3.575111e-06,
+            "peak_flow_rate": 3.57511e-06,
             "sensible_fraction_schedule_name": "Perimeter_mid_ZN_1 sub cat Sensible fract sched",
-            "target_temperature_schedule_name": "Perimeter_mid_ZN_1 sub cat Temp Sched",
             "zone_name": "Perimeter_mid_ZN_1"
         },
         "Perimeter_mid_ZN_2 sub cat": {
-            "end_use_subcategory": "sub cat",
+            "end_use_subcategory": "WaterUse",
             "flow_rate_fraction_schedule_name": "BLDG_SWH_SCH",
             "hot_water_supply_temperature_schedule_name": "Perimeter_mid_ZN_2 sub catHot Supply Temp Sched",
             "latent_fraction_schedule_name": "Perimeter_mid_ZN_2 sub cat Latent fract sched",
-            "peak_flow_rate": 3.575111e-06,
+            "peak_flow_rate": 3.57511e-06,
             "sensible_fraction_schedule_name": "Perimeter_mid_ZN_2 sub cat Sensible fract sched",
-            "target_temperature_schedule_name": "Perimeter_mid_ZN_2 sub cat Temp Sched",
             "zone_name": "Perimeter_mid_ZN_2"
         },
         "Perimeter_mid_ZN_3 sub cat": {
-            "end_use_subcategory": "sub cat",
+            "end_use_subcategory": "WaterUse",
             "flow_rate_fraction_schedule_name": "BLDG_SWH_SCH",
             "hot_water_supply_temperature_schedule_name": "Perimeter_mid_ZN_3 sub catHot Supply Temp Sched",
             "latent_fraction_schedule_name": "Perimeter_mid_ZN_3 sub cat Latent fract sched",
-            "peak_flow_rate": 3.575111e-06,
+            "peak_flow_rate": 3.57511e-06,
             "sensible_fraction_schedule_name": "Perimeter_mid_ZN_3 sub cat Sensible fract sched",
-            "target_temperature_schedule_name": "Perimeter_mid_ZN_3 sub cat Temp Sched",
             "zone_name": "Perimeter_mid_ZN_3"
         },
         "Perimeter_mid_ZN_4 sub cat": {
-            "end_use_subcategory": "sub cat",
+            "end_use_subcategory": "WaterUse",
             "flow_rate_fraction_schedule_name": "BLDG_SWH_SCH",
             "hot_water_supply_temperature_schedule_name": "Perimeter_mid_ZN_4 sub catHot Supply Temp Sched",
             "latent_fraction_schedule_name": "Perimeter_mid_ZN_4 sub cat Latent fract sched",
-            "peak_flow_rate": 3.575111e-06,
+            "peak_flow_rate": 3.57511e-06,
             "sensible_fraction_schedule_name": "Perimeter_mid_ZN_4 sub cat Sensible fract sched",
-            "target_temperature_schedule_name": "Perimeter_mid_ZN_4 sub cat Temp Sched",
             "zone_name": "Perimeter_mid_ZN_4"
         },
         "Perimeter_top_ZN_1 sub cat": {
-            "end_use_subcategory": "sub cat",
+            "end_use_subcategory": "WaterUse",
             "flow_rate_fraction_schedule_name": "BLDG_SWH_SCH",
             "hot_water_supply_temperature_schedule_name": "Perimeter_top_ZN_1 sub catHot Supply Temp Sched",
             "latent_fraction_schedule_name": "Perimeter_top_ZN_1 sub cat Latent fract sched",
-            "peak_flow_rate": 3.575111e-06,
+            "peak_flow_rate": 3.57511e-06,
             "sensible_fraction_schedule_name": "Perimeter_top_ZN_1 sub cat Sensible fract sched",
-            "target_temperature_schedule_name": "Perimeter_top_ZN_1 sub cat Temp Sched",
             "zone_name": "Perimeter_top_ZN_1"
         },
         "Perimeter_top_ZN_2 sub cat": {
-            "end_use_subcategory": "sub cat",
+            "end_use_subcategory": "WaterUse",
             "flow_rate_fraction_schedule_name": "BLDG_SWH_SCH",
             "hot_water_supply_temperature_schedule_name": "Perimeter_top_ZN_2 sub catHot Supply Temp Sched",
             "latent_fraction_schedule_name": "Perimeter_top_ZN_2 sub cat Latent fract sched",
-            "peak_flow_rate": 3.575111e-06,
+            "peak_flow_rate": 3.57511e-06,
             "sensible_fraction_schedule_name": "Perimeter_top_ZN_2 sub cat Sensible fract sched",
-            "target_temperature_schedule_name": "Perimeter_top_ZN_2 sub cat Temp Sched",
             "zone_name": "Perimeter_top_ZN_2"
         },
         "Perimeter_top_ZN_3 sub cat": {
-            "end_use_subcategory": "sub cat",
+            "end_use_subcategory": "WaterUse",
             "flow_rate_fraction_schedule_name": "BLDG_SWH_SCH",
             "hot_water_supply_temperature_schedule_name": "Perimeter_top_ZN_3 sub catHot Supply Temp Sched",
             "latent_fraction_schedule_name": "Perimeter_top_ZN_3 sub cat Latent fract sched",
-            "peak_flow_rate": 3.575111e-06,
+            "peak_flow_rate": 3.57511e-06,
             "sensible_fraction_schedule_name": "Perimeter_top_ZN_3 sub cat Sensible fract sched",
-            "target_temperature_schedule_name": "Perimeter_top_ZN_3 sub cat Temp Sched",
             "zone_name": "Perimeter_top_ZN_3"
         },
         "Perimeter_top_ZN_4 sub cat": {
-            "end_use_subcategory": "sub cat",
+            "end_use_subcategory": "WaterUse",
             "flow_rate_fraction_schedule_name": "BLDG_SWH_SCH",
             "hot_water_supply_temperature_schedule_name": "Perimeter_top_ZN_4 sub catHot Supply Temp Sched",
             "latent_fraction_schedule_name": "Perimeter_top_ZN_4 sub cat Latent fract sched",
-            "peak_flow_rate": 3.575111e-06,
+            "peak_flow_rate": 3.57511e-06,
             "sensible_fraction_schedule_name": "Perimeter_top_ZN_4 sub cat Sensible fract sched",
-            "target_temperature_schedule_name": "Perimeter_top_ZN_4 sub cat Temp Sched",
             "zone_name": "Perimeter_top_ZN_4"
         }
     },
-    "WindowMaterial:Gas": {
-        "AIR 13MM": {
-            "gas_type": "Air",
-            "thickness": 0.0127
-        },
-        "AIR 6MM": {
-            "gas_type": "Air",
-            "thickness": 0.0063
-        },
-        "ARGON 13MM": {
-            "gas_type": "Argon",
-            "thickness": 0.0127
-        },
-        "Gap_1_W_0_0018": {
-            "gas_type": "Air",
-            "thickness": 0.0018
-        },
-        "Gap_1_W_0_0024": {
-            "gas_type": "Air",
-            "thickness": 0.0024
-        },
-        "Gap_1_W_0_0025": {
-            "gas_type": "Air",
-            "thickness": 0.0025
-        },
-        "Gap_1_W_0_0032": {
-            "gas_type": "Air",
-            "thickness": 0.0032
-        },
-        "Gap_1_W_0_0038": {
-            "gas_type": "Air",
-            "thickness": 0.0038
-        },
-        "Gap_1_W_0_0042": {
-            "gas_type": "Air",
-            "thickness": 0.0042
-        },
-        "Gap_1_W_0_0043": {
-            "gas_type": "Air",
-            "thickness": 0.0043
-        },
-        "Gap_1_W_0_0046": {
-            "gas_type": "Air",
-            "thickness": 0.0046
-        },
-        "Gap_1_W_0_0048": {
-            "gas_type": "Air",
-            "thickness": 0.0048
-        },
-        "Gap_1_W_0_0052": {
-            "gas_type": "Air",
-            "thickness": 0.0052
-        },
-        "Gap_1_W_0_0060": {
-            "gas_type": "Air",
-            "thickness": 0.006
-        },
-        "Gap_1_W_0_0070": {
-            "gas_type": "Air",
-            "thickness": 0.007
-        },
-        "Gap_1_W_0_0090": {
-            "gas_type": "Air",
-            "thickness": 0.009
-        },
-        "Gap_1_W_0_0127": {
-            "gas_type": "Air",
-            "thickness": 0.0127
-        }
-    },
-    "WindowMaterial:GasMixture": {
-        "Gap_9_W_0_0127": {
-            "gas_1_fraction": 0.1,
-            "gas_1_type": "Air",
-            "gas_2_fraction": 0.9,
-            "gas_2_type": "Argon",
-            "number_of_gases_in_mixture": 2,
-            "thickness": 0.0127
-        }
-    },
-    "WindowMaterial:Glazing": {
-        "BLUE 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.05,
-            "back_side_visible_reflectance_at_normal_incidence": 0.06,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.05,
-            "front_side_visible_reflectance_at_normal_incidence": 0.06,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.48,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.57
-        },
-        "BRONZE 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.054,
-            "back_side_visible_reflectance_at_normal_incidence": 0.057,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.054,
-            "front_side_visible_reflectance_at_normal_incidence": 0.057,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.482,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.534
-        },
-        "CLEAR 3MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.075,
-            "back_side_visible_reflectance_at_normal_incidence": 0.081,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.075,
-            "front_side_visible_reflectance_at_normal_incidence": 0.081,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.837,
-            "thickness": 0.003,
-            "visible_transmittance_at_normal_incidence": 0.898
-        },
-        "CLEAR 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.071,
-            "back_side_visible_reflectance_at_normal_incidence": 0.08,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.071,
-            "front_side_visible_reflectance_at_normal_incidence": 0.08,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.775,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.881
-        },
-        "COATED POLY-55": {
-            "back_side_infrared_hemispherical_emissivity": 0.72,
-            "back_side_solar_reflectance_at_normal_incidence": 0.593,
-            "back_side_visible_reflectance_at_normal_incidence": 0.375,
-            "conductivity": 0.14,
-            "front_side_infrared_hemispherical_emissivity": 0.046,
-            "front_side_solar_reflectance_at_normal_incidence": 0.582,
-            "front_side_visible_reflectance_at_normal_incidence": 0.336,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.32,
-            "thickness": 0.00051,
-            "visible_transmittance_at_normal_incidence": 0.551
-        },
-        "COATED POLY-77": {
-            "back_side_infrared_hemispherical_emissivity": 0.72,
-            "back_side_solar_reflectance_at_normal_incidence": 0.398,
-            "back_side_visible_reflectance_at_normal_incidence": 0.167,
-            "conductivity": 0.14,
-            "front_side_infrared_hemispherical_emissivity": 0.075,
-            "front_side_solar_reflectance_at_normal_incidence": 0.402,
-            "front_side_visible_reflectance_at_normal_incidence": 0.147,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.504,
-            "thickness": 0.00051,
-            "visible_transmittance_at_normal_incidence": 0.766
-        },
-        "ECABS-2 BLEACHED 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.1,
-            "back_side_solar_reflectance_at_normal_incidence": 0.086,
-            "back_side_visible_reflectance_at_normal_incidence": 0.099,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.086,
-            "front_side_visible_reflectance_at_normal_incidence": 0.099,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.814,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.847
-        },
-        "ECABS-2 COLORED 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.1,
-            "back_side_solar_reflectance_at_normal_incidence": 0.179,
-            "back_side_visible_reflectance_at_normal_incidence": 0.081,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.179,
-            "front_side_visible_reflectance_at_normal_incidence": 0.081,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.111,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.128
-        },
-        "ECREF-1 COLORED 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.219,
-            "back_side_visible_reflectance_at_normal_incidence": 0.073,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.219,
-            "front_side_visible_reflectance_at_normal_incidence": 0.073,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.099,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.155
-        },
-        "ECREF-2 BLEACHED 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.1,
-            "back_side_solar_reflectance_at_normal_incidence": 0.168,
-            "back_side_visible_reflectance_at_normal_incidence": 0.11,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.168,
-            "front_side_visible_reflectance_at_normal_incidence": 0.11,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.694,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.818
-        },
-        "ECREF-2 COLORED 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.1,
-            "back_side_solar_reflectance_at_normal_incidence": 0.219,
-            "back_side_visible_reflectance_at_normal_incidence": 0.073,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.219,
-            "front_side_visible_reflectance_at_normal_incidence": 0.073,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.099,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.155
-        },
-        "GREEN 3MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.063,
-            "back_side_visible_reflectance_at_normal_incidence": 0.075,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.063,
-            "front_side_visible_reflectance_at_normal_incidence": 0.075,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.635,
-            "thickness": 0.003,
-            "visible_transmittance_at_normal_incidence": 0.822
-        },
-        "GREEN 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.056,
-            "back_side_visible_reflectance_at_normal_incidence": 0.07,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.056,
-            "front_side_visible_reflectance_at_normal_incidence": 0.07,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.487,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.749
-        },
-        "GREY 3MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.061,
-            "back_side_visible_reflectance_at_normal_incidence": 0.061,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.061,
-            "front_side_visible_reflectance_at_normal_incidence": 0.061,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.626,
-            "thickness": 0.003,
-            "visible_transmittance_at_normal_incidence": 0.611
-        },
-        "GREY 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.053,
-            "back_side_visible_reflectance_at_normal_incidence": 0.052,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.053,
-            "front_side_visible_reflectance_at_normal_incidence": 0.052,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.455,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.431
-        },
-        "Glass_102_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.07485449,
-            "back_side_visible_reflectance_at_normal_incidence": 0.082564,
-            "conductivity": 1.0,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.07476376,
-            "front_side_visible_reflectance_at_normal_incidence": 0.082563,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.833848,
-            "thickness": 0.003048,
-            "visible_transmittance_at_normal_incidence": 0.89926
-        },
-        "Glass_12116_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.538265,
-            "back_side_solar_reflectance_at_normal_incidence": 0.2199938,
-            "back_side_visible_reflectance_at_normal_incidence": 0.081654,
-            "conductivity": 1.000345,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.1094601,
-            "front_side_visible_reflectance_at_normal_incidence": 0.182598,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.171874,
-            "thickness": 0.00475,
-            "visible_transmittance_at_normal_incidence": 0.322771
-        },
-        "Glass_1576_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.868,
-            "back_side_solar_reflectance_at_normal_incidence": 0.1825558,
-            "back_side_visible_reflectance_at_normal_incidence": 0.128077,
-            "conductivity": 0.846,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.3034693,
-            "front_side_visible_reflectance_at_normal_incidence": 0.128888,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.167637,
-            "thickness": 0.003058,
-            "visible_transmittance_at_normal_incidence": 0.341994
-        },
-        "Glass_2010F_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.3410654,
-            "back_side_visible_reflectance_at_normal_incidence": 0.056031,
-            "conductivity": 1,
-            "front_side_infrared_hemispherical_emissivity": 0.042274,
-            "front_side_solar_reflectance_at_normal_incidence": 0.4183747,
-            "front_side_visible_reflectance_at_normal_incidence": 0.043577,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.434294,
-            "thickness": 0.00221,
-            "visible_transmittance_at_normal_incidence": 0.797579
-        },
-        "Glass_2022F_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.2656452,
-            "back_side_visible_reflectance_at_normal_incidence": 0.05547,
-            "conductivity": 1,
-            "front_side_infrared_hemispherical_emissivity": 0.046,
-            "front_side_solar_reflectance_at_normal_incidence": 0.3940945,
-            "front_side_visible_reflectance_at_normal_incidence": 0.042734,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.355897,
-            "thickness": 0.0039,
-            "visible_transmittance_at_normal_incidence": 0.677694
-        },
-        "Glass_2027F_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.340935,
-            "back_side_visible_reflectance_at_normal_incidence": 0.073741,
-            "conductivity": 1,
-            "front_side_infrared_hemispherical_emissivity": 0.03675,
-            "front_side_solar_reflectance_at_normal_incidence": 0.4700695,
-            "front_side_visible_reflectance_at_normal_incidence": 0.0546,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.369744,
-            "thickness": 0.004,
-            "visible_transmittance_at_normal_incidence": 0.765222
-        },
-        "Glass_2052_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.05449309,
-            "back_side_visible_reflectance_at_normal_incidence": 0.058397,
-            "conductivity": 1,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.05422805,
-            "front_side_visible_reflectance_at_normal_incidence": 0.05805,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.507767,
-            "thickness": 0.00837,
-            "visible_transmittance_at_normal_incidence": 0.586833
-        },
-        "Glass_2175_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.4379779,
-            "back_side_visible_reflectance_at_normal_incidence": 0.10654,
-            "conductivity": 1,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.2176064,
-            "front_side_visible_reflectance_at_normal_incidence": 0.078729,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.167758,
-            "thickness": 0.0086,
-            "visible_transmittance_at_normal_incidence": 0.416044
-        },
-        "Glass_2531_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.454,
-            "back_side_solar_reflectance_at_normal_incidence": 0.3617666,
-            "back_side_visible_reflectance_at_normal_incidence": 0.232929,
-            "conductivity": 0.934,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.3198325,
-            "front_side_visible_reflectance_at_normal_incidence": 0.25084,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.350556,
-            "thickness": 0.00306,
-            "visible_transmittance_at_normal_incidence": 0.490923
-        },
-        "Glass_2532_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.676,
-            "back_side_solar_reflectance_at_normal_incidence": 0.2732317,
-            "back_side_visible_reflectance_at_normal_incidence": 0.079448,
-            "conductivity": 0.933,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.2268281,
-            "front_side_visible_reflectance_at_normal_incidence": 0.0766,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.340824,
-            "thickness": 0.00306,
-            "visible_transmittance_at_normal_incidence": 0.543814
-        },
-        "Glass_282_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.37,
-            "back_side_solar_reflectance_at_normal_incidence": 0.4058073,
-            "back_side_visible_reflectance_at_normal_incidence": 0.270435,
-            "conductivity": 0.94,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.2956174,
-            "front_side_visible_reflectance_at_normal_incidence": 0.237458,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.352565,
-            "thickness": 0.003251,
-            "visible_transmittance_at_normal_incidence": 0.510046
-        },
-        "Glass_4313_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.298,
-            "back_side_solar_reflectance_at_normal_incidence": 0.09944001,
-            "back_side_visible_reflectance_at_normal_incidence": 0.096992,
-            "conductivity": 1.0,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.07114256,
-            "front_side_visible_reflectance_at_normal_incidence": 0.077225,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.373486,
-            "thickness": 0.00385,
-            "visible_transmittance_at_normal_incidence": 0.6013
-        },
-        "Glass_4321_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.279,
-            "back_side_solar_reflectance_at_normal_incidence": 0.09994167,
-            "back_side_visible_reflectance_at_normal_incidence": 0.094819,
-            "conductivity": 0.814,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.0742419,
-            "front_side_visible_reflectance_at_normal_incidence": 0.072726,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.425947,
-            "thickness": 0.00618,
-            "visible_transmittance_at_normal_incidence": 0.559652
-        },
-        "Glass_8652_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.39,
-            "back_side_solar_reflectance_at_normal_incidence": 0.4621051,
-            "back_side_visible_reflectance_at_normal_incidence": 0.306829,
-            "conductivity": 0.962,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.2989869,
-            "front_side_visible_reflectance_at_normal_incidence": 0.209449,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.343691,
-            "thickness": 0.003059,
-            "visible_transmittance_at_normal_incidence": 0.487937
-        },
-        "Glass_9731_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.203399,
-            "back_side_visible_reflectance_at_normal_incidence": 0.070696,
-            "conductivity": 0.815,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.2079376,
-            "front_side_visible_reflectance_at_normal_incidence": 0.071115,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.369424,
-            "thickness": 0.01248,
-            "visible_transmittance_at_normal_incidence": 0.710088
-        },
-        "LoE CLEAR 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.1,
-            "back_side_solar_reflectance_at_normal_incidence": 0.22,
-            "back_side_visible_reflectance_at_normal_incidence": 0.078,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.17,
-            "front_side_visible_reflectance_at_normal_incidence": 0.055,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.6,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.84
-        },
-        "LoE SPEC SEL CLEAR 3MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.03,
-            "back_side_solar_reflectance_at_normal_incidence": 0.37,
-            "back_side_visible_reflectance_at_normal_incidence": 0.06,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.34,
-            "front_side_visible_reflectance_at_normal_incidence": 0.07,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.45,
-            "thickness": 0.003,
-            "visible_transmittance_at_normal_incidence": 0.78
-        },
-        "LoE SPEC SEL CLEAR 6MM Rev": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.3,
-            "back_side_visible_reflectance_at_normal_incidence": 0.07,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.03,
-            "front_side_solar_reflectance_at_normal_incidence": 0.42,
-            "front_side_visible_reflectance_at_normal_incidence": 0.06,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.43,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.77
-        },
-        "LoE SPEC SEL TINT 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.03,
-            "back_side_solar_reflectance_at_normal_incidence": 0.41,
-            "back_side_visible_reflectance_at_normal_incidence": 0.04,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.14,
-            "front_side_visible_reflectance_at_normal_incidence": 0.06,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.26,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.46
-        },
-        "LoE TINT 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.1,
-            "back_side_solar_reflectance_at_normal_incidence": 0.2,
-            "back_side_visible_reflectance_at_normal_incidence": 0.054,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.093,
-            "front_side_visible_reflectance_at_normal_incidence": 0.035,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.36,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.5
-        },
-        "PYR A CLEAR 3MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.4,
-            "back_side_solar_reflectance_at_normal_incidence": 0.1,
-            "back_side_visible_reflectance_at_normal_incidence": 0.12,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.1,
-            "front_side_visible_reflectance_at_normal_incidence": 0.12,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.75,
-            "thickness": 0.003,
-            "visible_transmittance_at_normal_incidence": 0.85
-        },
-        "PYR B CLEAR 3MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.2,
-            "back_side_solar_reflectance_at_normal_incidence": 0.1,
-            "back_side_visible_reflectance_at_normal_incidence": 0.12,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.09,
-            "front_side_visible_reflectance_at_normal_incidence": 0.11,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.74,
-            "thickness": 0.003,
-            "visible_transmittance_at_normal_incidence": 0.82
-        },
-        "PYR B CLEAR 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.2,
-            "back_side_solar_reflectance_at_normal_incidence": 0.1,
-            "back_side_visible_reflectance_at_normal_incidence": 0.12,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.09,
-            "front_side_visible_reflectance_at_normal_incidence": 0.11,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.68,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.81
-        },
-        "REF A CLEAR LO 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.4,
-            "back_side_solar_reflectance_at_normal_incidence": 0.493,
-            "back_side_visible_reflectance_at_normal_incidence": 0.37,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.341,
-            "front_side_visible_reflectance_at_normal_incidence": 0.41,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.066,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.08
-        },
-        "REF A TINT MID 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.47,
-            "back_side_solar_reflectance_at_normal_incidence": 0.42,
-            "back_side_visible_reflectance_at_normal_incidence": 0.35,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.13,
-            "front_side_visible_reflectance_at_normal_incidence": 0.14,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.06,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.09
-        },
-        "REF B CLEAR HI 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.6,
-            "back_side_solar_reflectance_at_normal_incidence": 0.32,
-            "back_side_visible_reflectance_at_normal_incidence": 0.29,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.16,
-            "front_side_visible_reflectance_at_normal_incidence": 0.16,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.24,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.3
-        },
-        "REF B CLEAR LO 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.58,
-            "back_side_solar_reflectance_at_normal_incidence": 0.38,
-            "back_side_visible_reflectance_at_normal_incidence": 0.33,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.22,
-            "front_side_visible_reflectance_at_normal_incidence": 0.23,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.15,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.2
-        },
-        "REF B TINT HI 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.6,
-            "back_side_solar_reflectance_at_normal_incidence": 0.33,
-            "back_side_visible_reflectance_at_normal_incidence": 0.28,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.09,
-            "front_side_visible_reflectance_at_normal_incidence": 0.08,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.15,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.18
-        },
-        "REF B TINT MID 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.45,
-            "back_side_solar_reflectance_at_normal_incidence": 0.41,
-            "back_side_visible_reflectance_at_normal_incidence": 0.32,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.11,
-            "front_side_visible_reflectance_at_normal_incidence": 0.1,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.1,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.13
-        },
-        "REF C CLEAR HI 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.55,
-            "back_side_solar_reflectance_at_normal_incidence": 0.39,
-            "back_side_visible_reflectance_at_normal_incidence": 0.35,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.16,
-            "front_side_visible_reflectance_at_normal_incidence": 0.17,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.2,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.22
-        },
-        "REF C CLEAR MID 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.51,
-            "back_side_solar_reflectance_at_normal_incidence": 0.42,
-            "back_side_visible_reflectance_at_normal_incidence": 0.38,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.2,
-            "front_side_visible_reflectance_at_normal_incidence": 0.21,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.17,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.19
-        },
-        "REF D CLEAR 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.82,
-            "back_side_solar_reflectance_at_normal_incidence": 0.379,
-            "back_side_visible_reflectance_at_normal_incidence": 0.505,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.308,
-            "front_side_visible_reflectance_at_normal_incidence": 0.453,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.429,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.334
-        },
-        "REF D TINT 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.82,
-            "back_side_solar_reflectance_at_normal_incidence": 0.36,
-            "back_side_visible_reflectance_at_normal_incidence": 0.45,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.14,
-            "front_side_visible_reflectance_at_normal_incidence": 0.18,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.3,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.25
-        },
-        "Theoretical Glass 297": {
-            "back_side_infrared_hemispherical_emissivity": 0.9,
-            "back_side_solar_reflectance_at_normal_incidence": 0.574961,
-            "back_side_visible_reflectance_at_normal_incidence": 0.420302,
-            "conductivity": 0.0103561,
-            "front_side_infrared_hemispherical_emissivity": 0.9,
-            "front_side_solar_reflectance_at_normal_incidence": 0.574961,
-            "front_side_visible_reflectance_at_normal_incidence": 0.420302,
-            "infrared_transmittance_at_normal_incidence": 0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.375039,
-            "thickness": 0.003,
-            "visible_transmittance_at_normal_incidence": 0.529698
-        },
-        "Theoretical Glass 347": {
-            "back_side_infrared_hemispherical_emissivity": 0.9,
-            "back_side_solar_reflectance_at_normal_incidence": 0.634139,
-            "back_side_visible_reflectance_at_normal_incidence": 0.470089,
-            "conductivity": 0.010358,
-            "front_side_infrared_hemispherical_emissivity": 0.9,
-            "front_side_solar_reflectance_at_normal_incidence": 0.634139,
-            "front_side_visible_reflectance_at_normal_incidence": 0.470089,
-            "infrared_transmittance_at_normal_incidence": 0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.315861,
-            "thickness": 0.003,
-            "visible_transmittance_at_normal_incidence": 0.479911
+    "WindowMaterial:SimpleGlazingSystem": {
+        "Glazing Layer": {
+            "solar_heat_gain_coefficient": 0.38,
+            "u_factor": 2.0441736,
+            "visible_transmittance": 0.418
         }
     },
     "Zone": {
         "Core_bottom": {
             "ceiling_height": 2.7432,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "Core_mid": {
             "ceiling_height": 2.7432,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "Core_top": {
             "ceiling_height": 2.7432,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "FirstFloor_Plenum": {
             "ceiling_height": 1.2192,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "No",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "MidFloor_Plenum": {
             "ceiling_height": 1.2192,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "No",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "Perimeter_bot_ZN_1": {
             "ceiling_height": 2.7432,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "Perimeter_bot_ZN_2": {
             "ceiling_height": 2.7432,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "Perimeter_bot_ZN_3": {
             "ceiling_height": 2.7432,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "Perimeter_bot_ZN_4": {
             "ceiling_height": 2.7432,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "Perimeter_mid_ZN_1": {
             "ceiling_height": 2.7432,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "Perimeter_mid_ZN_2": {
             "ceiling_height": 2.7432,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "Perimeter_mid_ZN_3": {
             "ceiling_height": 2.7432,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "Perimeter_mid_ZN_4": {
             "ceiling_height": 2.7432,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "Perimeter_top_ZN_1": {
             "ceiling_height": 2.7432,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "Perimeter_top_ZN_2": {
             "ceiling_height": 2.7432,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "Perimeter_top_ZN_3": {
             "ceiling_height": 2.7432,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "Perimeter_top_ZN_4": {
             "ceiling_height": 2.7432,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "TopFloor_Plenum": {
             "ceiling_height": 1.2192,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "No",
             "type": 1,
             "volume": "Autocalculate",
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         }
@@ -16001,180 +16084,180 @@
         }
     },
     "ZoneInfiltration:DesignFlowRate": {
         "FirstFloor_Plenum_Infiltration": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.00056896,
+            "flow_rate_per_exterior_surface_area": 0.00056896,
             "schedule_name": "INFIL_SCH_PNNL",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "FirstFloor_Plenum"
+            "zone_or_zonelist_or_space_or_spacelist_name": "FirstFloor_Plenum"
         },
         "MidFloor_Plenum_Infiltration": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.00056896,
+            "flow_rate_per_exterior_surface_area": 0.00056896,
             "schedule_name": "INFIL_SCH_PNNL",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "MidFloor_Plenum"
+            "zone_or_zonelist_or_space_or_spacelist_name": "MidFloor_Plenum"
         },
         "Perimeter_bot_ZN_1_Door_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate": 0.678659786,
             "design_flow_rate_calculation_method": "Flow/Zone",
             "schedule_name": "INFIL_Door_Opening_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_1"
         },
         "Perimeter_bot_ZN_1_Infiltration": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.00056896,
+            "flow_rate_per_exterior_surface_area": 0.00056896,
             "schedule_name": "INFIL_SCH_PNNL",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_1"
         },
         "Perimeter_bot_ZN_2_Infiltration": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.00056896,
+            "flow_rate_per_exterior_surface_area": 0.00056896,
             "schedule_name": "INFIL_SCH_PNNL",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_2"
         },
         "Perimeter_bot_ZN_3_Infiltration": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.00056896,
+            "flow_rate_per_exterior_surface_area": 0.00056896,
             "schedule_name": "INFIL_SCH_PNNL",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_3"
         },
         "Perimeter_bot_ZN_4_Infiltration": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.00056896,
+            "flow_rate_per_exterior_surface_area": 0.00056896,
             "schedule_name": "INFIL_SCH_PNNL",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_4"
         },
         "Perimeter_mid_ZN_1_Infiltration": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.00056896,
+            "flow_rate_per_exterior_surface_area": 0.00056896,
             "schedule_name": "INFIL_SCH_PNNL",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_1"
         },
         "Perimeter_mid_ZN_2_Infiltration": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.00056896,
+            "flow_rate_per_exterior_surface_area": 0.00056896,
             "schedule_name": "INFIL_SCH_PNNL",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_2"
         },
         "Perimeter_mid_ZN_3_Infiltration": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.00056896,
+            "flow_rate_per_exterior_surface_area": 0.00056896,
             "schedule_name": "INFIL_SCH_PNNL",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_3"
         },
         "Perimeter_mid_ZN_4_Infiltration": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.00056896,
+            "flow_rate_per_exterior_surface_area": 0.00056896,
             "schedule_name": "INFIL_SCH_PNNL",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_4"
         },
         "Perimeter_top_ZN_1_Infiltration": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.00056896,
+            "flow_rate_per_exterior_surface_area": 0.00056896,
             "schedule_name": "INFIL_SCH_PNNL",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_1"
         },
         "Perimeter_top_ZN_2_Infiltration": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.00056896,
+            "flow_rate_per_exterior_surface_area": 0.00056896,
             "schedule_name": "INFIL_SCH_PNNL",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_2"
         },
         "Perimeter_top_ZN_3_Infiltration": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.00056896,
+            "flow_rate_per_exterior_surface_area": 0.00056896,
             "schedule_name": "INFIL_SCH_PNNL",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_3"
         },
         "Perimeter_top_ZN_4_Infiltration": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.00056896,
+            "flow_rate_per_exterior_surface_area": 0.00056896,
             "schedule_name": "INFIL_SCH_PNNL",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_4"
         },
         "TopFloor_Plenum_Infiltration": {
             "constant_term_coefficient": 0,
             "design_flow_rate": 0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 6.19256064e-05,
+            "flow_rate_per_exterior_surface_area": 6.19256064e-05,
             "schedule_name": "INFIL_SCH_PNNL",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "TopFloor_Plenum"
+            "zone_or_zonelist_or_space_or_spacelist_name": "TopFloor_Plenum"
         }
     }
 }
```

### Comparing `sinergym-2.4.1/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.epJSON` & `sinergym-2.5.0/sinergym/data/buildings/ASHRAE901_Warehouse_STD2019_Denver.epJSON`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7594648185338838%*

 * *Differences: {"'AirLoopHVAC:OutdoorAirSystem'": "{'PSZ-Fine Storage OA System': {delete: "*

 * *                                   "['availability_manager_list_name']}, 'PSZ-Office OA System': "*

 * *                                   "{delete: ['availability_manager_list_name']}}",*

 * * "'AirLoopHVAC:UnitarySystem'": "OrderedDict([('PSZ-Fine_Unitary_Package_DX', "*

 * *                                "OrderedDict([('air_inlet_node_name', 'PSZ-Fine Storage Mixed Air "*

 * *                                "Outlet'), ('air_outlet_node_name', 'PS […]*

```diff
@@ -27,20 +27,18 @@
         "PSZ-Office OA System Controllers": {
             "controller_1_name": "PSZ-Office OA Controller",
             "controller_1_object_type": "Controller:OutdoorAir"
         }
     },
     "AirLoopHVAC:OutdoorAirSystem": {
         "PSZ-Fine Storage OA System": {
-            "availability_manager_list_name": "PSZ-Fine Storage Availability Managers",
             "controller_list_name": "PSZ-Fine Storage OA System Controllers",
             "outdoor_air_equipment_list_name": "PSZ-Fine Storage OA System Equipment"
         },
         "PSZ-Office OA System": {
-            "availability_manager_list_name": "PSZ-Office Availability Managers",
             "controller_list_name": "PSZ-Office OA System Controllers",
             "outdoor_air_equipment_list_name": "PSZ-Office OA System Equipment"
         }
     },
     "AirLoopHVAC:OutdoorAirSystem:EquipmentList": {
         "PSZ-Fine Storage OA System Equipment": {
             "component_1_name": "PSZ-Fine Storage OA Mixing Box",
@@ -87,14 +85,74 @@
                     "component_name": "PSZ-Office Zone Splitter",
                     "component_object_type": "AirLoopHVAC:ZoneSplitter"
                 }
             ],
             "supply_air_path_inlet_node_name": "PSZ-Office Supply Path Inlet"
         }
     },
+    "AirLoopHVAC:UnitarySystem": {
+        "PSZ-Fine_Unitary_Package_DX": {
+            "air_inlet_node_name": "PSZ-Fine Storage Mixed Air Outlet",
+            "air_outlet_node_name": "PSZ-Fine Storage Air Loop Outlet",
+            "availability_schedule_name": "COMPACT HVAC-ALWAYS 1",
+            "control_type": "Load",
+            "controlling_zone_or_thermostat_location": "Zone2 Fine Storage",
+            "cooling_coil_name": "PSZ-Fine Storage Cooling Coil",
+            "cooling_coil_object_type": "Coil:Cooling:DX:MultiSpeed",
+            "cooling_supply_air_flow_rate": "Autosize",
+            "cooling_supply_air_flow_rate_method": "SupplyAirFlowRate",
+            "dehumidification_control_type": "None",
+            "design_specification_multispeed_object_name": "PSZ-Fine_Unitary_Package_DX_Perf",
+            "design_specification_multispeed_object_type": "UnitarySystemPerformance:Multispeed",
+            "dx_heating_coil_sizing_ratio": 1,
+            "fan_placement": "BlowThrough",
+            "heating_coil_name": "PSZ-Fine Storage Heating Coil",
+            "heating_coil_object_type": "Coil:Heating:Fuel",
+            "heating_supply_air_flow_rate": "Autosize",
+            "heating_supply_air_flow_rate_method": "SupplyAirFlowRate",
+            "latent_load_control": "SensibleOnlyLoadControl",
+            "maximum_supply_air_temperature": "Autosize",
+            "minimum_supply_air_temperature": 2,
+            "no_load_supply_air_flow_rate": "Autosize",
+            "no_load_supply_air_flow_rate_method": "SupplyAirFlowRate",
+            "supply_air_fan_operating_mode_schedule_name": "FanSched",
+            "supply_fan_name": "PSZ-Fine Storage_addAQ Supply Fan",
+            "supply_fan_object_type": "Fan:SystemModel",
+            "use_doas_dx_cooling_coil": "No"
+        },
+        "PSZ-Office_Unitary_Package_DX": {
+            "air_inlet_node_name": "PSZ-Office Mixed Air Outlet",
+            "air_outlet_node_name": "PSZ-Office Air Loop Outlet",
+            "availability_schedule_name": "COMPACT HVAC-ALWAYS 1",
+            "control_type": "Load",
+            "controlling_zone_or_thermostat_location": "Zone1 Office",
+            "cooling_coil_name": "PSZ-Office Cooling Coil",
+            "cooling_coil_object_type": "Coil:Cooling:DX:MultiSpeed",
+            "cooling_supply_air_flow_rate": "Autosize",
+            "cooling_supply_air_flow_rate_method": "SupplyAirFlowRate",
+            "dehumidification_control_type": "None",
+            "design_specification_multispeed_object_name": "PSZ-Office_Unitary_Package_DX_Perf",
+            "design_specification_multispeed_object_type": "UnitarySystemPerformance:Multispeed",
+            "dx_heating_coil_sizing_ratio": 1,
+            "fan_placement": "BlowThrough",
+            "heating_coil_name": "PSZ-Office Heating Coil",
+            "heating_coil_object_type": "Coil:Heating:Fuel",
+            "heating_supply_air_flow_rate": "Autosize",
+            "heating_supply_air_flow_rate_method": "SupplyAirFlowRate",
+            "latent_load_control": "SensibleOnlyLoadControl",
+            "maximum_supply_air_temperature": "Autosize",
+            "minimum_supply_air_temperature": 2,
+            "no_load_supply_air_flow_rate": "Autosize",
+            "no_load_supply_air_flow_rate_method": "SupplyAirFlowRate",
+            "supply_air_fan_operating_mode_schedule_name": "FanSched",
+            "supply_fan_name": "PSZ-Office_addAQ Supply Fan",
+            "supply_fan_object_type": "Fan:SystemModel",
+            "use_doas_dx_cooling_coil": "No"
+        }
+    },
     "AirLoopHVAC:ZoneMixer": {
         "PSZ-Fine Storage Zone Mixer": {
             "nodes": [
                 {
                     "inlet_node_name": "Zone2 Fine Storage Return Outlet"
                 }
             ],
@@ -184,56 +242,32 @@
                     "component_inlet_node_name": "PSZ-Fine Storage Air Loop Inlet",
                     "component_name": "PSZ-Fine Storage OA System",
                     "component_object_type": "AirLoopHVAC:OutdoorAirSystem",
                     "component_outlet_node_name": "PSZ-Fine Storage Mixed Air Outlet"
                 },
                 {
                     "component_inlet_node_name": "PSZ-Fine Storage Mixed Air Outlet",
-                    "component_name": "PSZ-Fine Storage Supply Fan",
-                    "component_object_type": "Fan:ConstantVolume",
-                    "component_outlet_node_name": "PSZ-Fine Storage Supply Fan Outlet"
-                },
-                {
-                    "component_inlet_node_name": "PSZ-Fine Storage Supply Fan Outlet",
-                    "component_name": "PSZ-Fine Storage Heating Coil",
-                    "component_object_type": "Coil:Heating:Fuel",
-                    "component_outlet_node_name": "PSZ-Fine Storage Heating Coil Outlet"
-                },
-                {
-                    "component_inlet_node_name": "PSZ-Fine Storage Heating Coil Outlet",
-                    "component_name": "PSZ-Fine Storage_Unitary_Package_DX",
-                    "component_object_type": "CoilSystem:Cooling:DX",
+                    "component_name": "PSZ-Fine_Unitary_Package_DX",
+                    "component_object_type": "AirLoopHVAC:UnitarySystem",
                     "component_outlet_node_name": "PSZ-Fine Storage Air Loop Outlet"
                 }
             ]
         },
         "PSZ-Office Main Branch": {
             "components": [
                 {
                     "component_inlet_node_name": "PSZ-Office Air Loop Inlet",
                     "component_name": "PSZ-Office OA System",
                     "component_object_type": "AirLoopHVAC:OutdoorAirSystem",
                     "component_outlet_node_name": "PSZ-Office Mixed Air Outlet"
                 },
                 {
                     "component_inlet_node_name": "PSZ-Office Mixed Air Outlet",
-                    "component_name": "PSZ-Office Supply Fan",
-                    "component_object_type": "Fan:ConstantVolume",
-                    "component_outlet_node_name": "PSZ-Office Supply Fan Outlet"
-                },
-                {
-                    "component_inlet_node_name": "PSZ-Office Supply Fan Outlet",
-                    "component_name": "PSZ-Office Heating Coil",
-                    "component_object_type": "Coil:Heating:Fuel",
-                    "component_outlet_node_name": "PSZ-Office Heating Coil Outlet"
-                },
-                {
-                    "component_inlet_node_name": "PSZ-Office Heating Coil Outlet",
                     "component_name": "PSZ-Office_Unitary_Package_DX",
-                    "component_object_type": "CoilSystem:Cooling:DX",
+                    "component_object_type": "AirLoopHVAC:UnitarySystem",
                     "component_outlet_node_name": "PSZ-Office Air Loop Outlet"
                 }
             ]
         }
     },
     "BranchList": {
         "PSZ-Fine Storage Branches": {
@@ -250,27 +284,27 @@
                 }
             ]
         }
     },
     "Building": {
         "Warehouse": {
             "loads_convergence_tolerance_value": 0.04,
-            "maximum_number_of_warmup_days": 25,
+            "maximum_number_of_warmup_days": 15,
             "minimum_number_of_warmup_days": 6,
             "north_axis": 90,
             "solar_distribution": "FullExterior",
             "temperature_convergence_tolerance_value": 0.4,
             "terrain": "Urban"
         }
     },
     "BuildingSurface:Detailed": {
         "Bulk Storage Floor": {
-            "construction_name": "ext_slab_6in",
+            "construction_name": "BulkStorageFloor_Ffactor",
             "number_of_vertices": "Autocalculate",
-            "outside_boundary_condition": "Ground",
+            "outside_boundary_condition": "GroundFCfactorMethod",
             "sun_exposure": "NoSun",
             "surface_type": "Floor",
             "vertices": [
                 {
                     "vertex_x_coordinate": 45.7177703814647,
                     "vertex_y_coordinate": 100.579094839222,
                     "vertex_z_coordinate": 0
@@ -453,17 +487,17 @@
                 }
             ],
             "view_factor_to_ground": "Autocalculate",
             "wind_exposure": "WindExposed",
             "zone_name": "Zone3 Bulk Storage"
         },
         "Fine Storage Floor": {
-            "construction_name": "ext_slab_6in",
+            "construction_name": "FineStorageFloor_Ffactor",
             "number_of_vertices": "Autocalculate",
-            "outside_boundary_condition": "Ground",
+            "outside_boundary_condition": "GroundFCfactorMethod",
             "sun_exposure": "NoSun",
             "surface_type": "Floor",
             "vertices": [
                 {
                     "vertex_x_coordinate": 45.7177703814647,
                     "vertex_y_coordinate": 30.4785135876431,
                     "vertex_z_coordinate": 0
@@ -687,17 +721,17 @@
                 }
             ],
             "view_factor_to_ground": "Autocalculate",
             "wind_exposure": "WindExposed",
             "zone_name": "Zone2 Fine Storage"
         },
         "Office Floor": {
-            "construction_name": "ext_slab_6in",
+            "construction_name": "OfficeFloor_Ffactor",
             "number_of_vertices": "Autocalculate",
-            "outside_boundary_condition": "Ground",
+            "outside_boundary_condition": "GroundFCfactorMethod",
             "sun_exposure": "NoSun",
             "surface_type": "Floor",
             "vertices": [
                 {
                     "vertex_x_coordinate": 25.9067365494966,
                     "vertex_y_coordinate": 9.14355407629293,
                     "vertex_z_coordinate": 0
@@ -882,110 +916,126 @@
                 }
             ],
             "view_factor_to_ground": "Autocalculate",
             "wind_exposure": "NoWind",
             "zone_name": "Zone1 Office"
         }
     },
-    "Coil:Cooling:DX:TwoSpeed": {
+    "Coil:Cooling:DX:MultiSpeed": {
         "PSZ-Fine Storage Cooling Coil": {
+            "2017_speed_1_rated_evaporator_fan_power_per_volume_flow_rate": 0,
+            "2017_speed_2_rated_evaporator_fan_power_per_volume_flow_rate": 0,
+            "2023_speed_1_rated_evaporator_fan_power_per_volume_flow_rate": 934.4,
+            "2023_speed_2_rated_evaporator_fan_power_per_volume_flow_rate": 934.4,
             "air_inlet_node_name": "PSZ-Fine Storage Heating Coil Outlet",
             "air_outlet_node_name": "PSZ-Fine Storage Air Loop Outlet",
+            "apply_latent_degradation_to_speeds_greater_than_1": "No",
+            "apply_part_load_fraction_to_speeds_greater_than_1": "No",
             "availability_schedule_name": "COMPACT HVAC-ALWAYS 1",
-            "energy_input_ratio_function_of_flow_fraction_curve_name": "PSZ-Fine Storage DX Coil EIR-FF",
-            "energy_input_ratio_function_of_temperature_curve_name": "PSZ-Fine Storage DX Coil EIR-FT",
-            "high_speed_gross_rated_cooling_cop": 4.11713235489972,
-            "high_speed_gross_rated_total_cooling_capacity": 17790.44,
-            "high_speed_rated_air_flow_rate": 1.05822,
-            "high_speed_rated_sensible_heat_ratio": 0.79301,
-            "low_speed_energy_input_ratio_function_of_temperature_curve_name": "PSZ-Fine Storage DX Coil EIR-FT",
-            "low_speed_gross_rated_cooling_cop": 4.11713235489972,
-            "low_speed_gross_rated_sensible_heat_ratio": 0.79301,
-            "low_speed_gross_rated_total_cooling_capacity": 8895.22,
-            "low_speed_rated_air_flow_rate": 0.70548,
-            "low_speed_total_cooling_capacity_function_of_temperature_curve_name": "PSZ-Fine Storage DX Coil Cap-FT",
-            "part_load_fraction_correlation_curve_name": "PSZ-Fine Storage DX Coil PLF",
-            "total_cooling_capacity_function_of_flow_fraction_curve_name": "PSZ-Fine Storage DX Coil Cap-FF",
-            "total_cooling_capacity_function_of_temperature_curve_name": "PSZ-Fine Storage DX Coil Cap-FT"
+            "basin_heater_setpoint_temperature": 2,
+            "condenser_type": "AirCooled",
+            "fuel_type": "Electricity",
+            "maximum_outdoor_dry_bulb_temperature_for_crankcase_heater_operation": 10,
+            "number_of_speeds": 2,
+            "speed_1_energy_input_ratio_function_of_flow_fraction_curve_name": "PSZ-AC_Unitary_PackagecoolEIRFFF",
+            "speed_1_energy_input_ratio_function_of_temperature_curve_name": "PSZ-AC_Unitary_PackagecoolEIRFT",
+            "speed_1_evaporative_condenser_effectiveness": 0.9,
+            "speed_1_gross_rated_cooling_cop": 3.7988306741603,
+            "speed_1_gross_rated_sensible_heat_ratio": 0.7457,
+            "speed_1_gross_rated_total_cooling_capacity": 19319.855,
+            "speed_1_part_load_fraction_correlation_curve_name": "PSZ-AC_Unitary_PackagecoolPLR",
+            "speed_1_rated_air_flow_rate": 1.33200666666667,
+            "speed_1_rated_waste_heat_fraction_of_power_input": 0.2,
+            "speed_1_total_cooling_capacity_function_of_flow_fraction_curve_name": "PSZ-AC_Unitary_PackagecoolFFF",
+            "speed_1_total_cooling_capacity_function_of_temperature_curve_name": "PSZ-AC_Unitary_PackagecoolCapFT",
+            "speed_2_energy_input_ratio_function_of_flow_fraction_curve_name": "PSZ-AC_Unitary_PackagecoolEIRFFF",
+            "speed_2_energy_input_ratio_function_of_temperature_curve_name": "PSZ-AC_Unitary_PackagecoolEIRFT",
+            "speed_2_evaporative_condenser_effectiveness": 0.9,
+            "speed_2_gross_rated_cooling_cop": 3.7988306741603,
+            "speed_2_gross_rated_sensible_heat_ratio": 0.7457,
+            "speed_2_gross_rated_total_cooling_capacity": 38639.71,
+            "speed_2_part_load_fraction_correlation_curve_name": "PSZ-AC_Unitary_PackagecoolPLR",
+            "speed_2_rated_air_flow_rate": 1.99801,
+            "speed_2_rated_waste_heat_fraction_of_power_input": 0.2,
+            "speed_2_total_cooling_capacity_function_of_flow_fraction_curve_name": "PSZ-AC_Unitary_PackagecoolFFF",
+            "speed_2_total_cooling_capacity_function_of_temperature_curve_name": "PSZ-AC_Unitary_PackagecoolCapFT"
         },
         "PSZ-Office Cooling Coil": {
+            "2017_speed_1_rated_evaporator_fan_power_per_volume_flow_rate": 0,
+            "2017_speed_2_rated_evaporator_fan_power_per_volume_flow_rate": 0,
+            "2023_speed_1_rated_evaporator_fan_power_per_volume_flow_rate": 934.4,
+            "2023_speed_2_rated_evaporator_fan_power_per_volume_flow_rate": 934.4,
             "air_inlet_node_name": "PSZ-Office Heating Coil Outlet",
             "air_outlet_node_name": "PSZ-Office Air Loop Outlet",
+            "apply_latent_degradation_to_speeds_greater_than_1": "No",
+            "apply_part_load_fraction_to_speeds_greater_than_1": "No",
             "availability_schedule_name": "COMPACT HVAC-ALWAYS 1",
-            "energy_input_ratio_function_of_flow_fraction_curve_name": "PSZ-Office DX Coil EIR-FF",
-            "energy_input_ratio_function_of_temperature_curve_name": "PSZ-Office DX Coil EIR-FT",
-            "high_speed_gross_rated_cooling_cop": 4.11713235489972,
-            "high_speed_gross_rated_total_cooling_capacity": 9041.45,
-            "high_speed_rated_air_flow_rate": 0.54619,
-            "high_speed_rated_sensible_heat_ratio": 0.79866,
-            "low_speed_energy_input_ratio_function_of_temperature_curve_name": "PSZ-Office DX Coil EIR-FT",
-            "low_speed_gross_rated_cooling_cop": 4.11713235489972,
-            "low_speed_gross_rated_sensible_heat_ratio": 0.79866,
-            "low_speed_gross_rated_total_cooling_capacity": 4520.725,
-            "low_speed_rated_air_flow_rate": 0.364126666666667,
-            "low_speed_total_cooling_capacity_function_of_temperature_curve_name": "PSZ-Office DX Coil Cap-FT",
-            "part_load_fraction_correlation_curve_name": "PSZ-Office DX Coil PLF",
-            "total_cooling_capacity_function_of_flow_fraction_curve_name": "PSZ-Office DX Coil Cap-FF",
-            "total_cooling_capacity_function_of_temperature_curve_name": "PSZ-Office DX Coil Cap-FT"
+            "basin_heater_setpoint_temperature": 2,
+            "condenser_type": "AirCooled",
+            "fuel_type": "Electricity",
+            "maximum_outdoor_dry_bulb_temperature_for_crankcase_heater_operation": 10,
+            "number_of_speeds": 2,
+            "speed_1_energy_input_ratio_function_of_flow_fraction_curve_name": "PSZ-AC_Unitary_PackagecoolEIRFFF",
+            "speed_1_energy_input_ratio_function_of_temperature_curve_name": "PSZ-AC_Unitary_PackagecoolEIRFT",
+            "speed_1_evaporative_condenser_effectiveness": 0.9,
+            "speed_1_gross_rated_cooling_cop": 4.11713235489972,
+            "speed_1_gross_rated_sensible_heat_ratio": 0.79866,
+            "speed_1_gross_rated_total_cooling_capacity": 8107.42,
+            "speed_1_part_load_fraction_correlation_curve_name": "PSZ-AC_Unitary_PackagecoolPLR",
+            "speed_1_rated_air_flow_rate": 0.653026666666667,
+            "speed_1_rated_waste_heat_fraction_of_power_input": 0.2,
+            "speed_1_total_cooling_capacity_function_of_flow_fraction_curve_name": "PSZ-AC_Unitary_PackagecoolFFF",
+            "speed_1_total_cooling_capacity_function_of_temperature_curve_name": "PSZ-AC_Unitary_PackagecoolCapFT",
+            "speed_2_energy_input_ratio_function_of_flow_fraction_curve_name": "PSZ-AC_Unitary_PackagecoolEIRFFF",
+            "speed_2_energy_input_ratio_function_of_temperature_curve_name": "PSZ-AC_Unitary_PackagecoolEIRFT",
+            "speed_2_evaporative_condenser_effectiveness": 0.9,
+            "speed_2_gross_rated_cooling_cop": 4.11713235489972,
+            "speed_2_gross_rated_sensible_heat_ratio": 0.79866,
+            "speed_2_gross_rated_total_cooling_capacity": 16214.84,
+            "speed_2_part_load_fraction_correlation_curve_name": "PSZ-AC_Unitary_PackagecoolPLR",
+            "speed_2_rated_air_flow_rate": 0.97954,
+            "speed_2_rated_waste_heat_fraction_of_power_input": 0.2,
+            "speed_2_total_cooling_capacity_function_of_flow_fraction_curve_name": "PSZ-AC_Unitary_PackagecoolFFF",
+            "speed_2_total_cooling_capacity_function_of_temperature_curve_name": "PSZ-AC_Unitary_PackagecoolCapFT"
         }
     },
     "Coil:Heating:Fuel": {
         "PSZ-Fine Storage Heating Coil": {
             "air_inlet_node_name": "PSZ-Fine Storage Supply Fan Outlet",
             "air_outlet_node_name": "PSZ-Fine Storage Heating Coil Outlet",
             "availability_schedule_name": "COMPACT HVAC-ALWAYS 1",
-            "burner_efficiency": 0.8,
+            "burner_efficiency": 0.81,
             "fuel_type": "NaturalGas",
             "nominal_capacity": "Autosize",
             "parasitic_electric_load": 0.0,
             "parasitic_fuel_load": 0.0,
-            "part_load_fraction_correlation_curve_name": "PSZ-Fine Storage Heating Coil PLF-FPLR",
-            "temperature_setpoint_node_name": "PSZ-Fine Storage Heating Coil Outlet"
+            "part_load_fraction_correlation_curve_name": "PSZ-Fine Storage Heating Coil PLF-FPLR"
         },
         "PSZ-Office Heating Coil": {
             "air_inlet_node_name": "PSZ-Office Supply Fan Outlet",
             "air_outlet_node_name": "PSZ-Office Heating Coil Outlet",
             "availability_schedule_name": "COMPACT HVAC-ALWAYS 1",
-            "burner_efficiency": 0.8,
+            "burner_efficiency": 0.81,
             "fuel_type": "NaturalGas",
             "nominal_capacity": "Autosize",
             "parasitic_electric_load": 0.0,
             "parasitic_fuel_load": 0.0,
-            "part_load_fraction_correlation_curve_name": "PSZ-Office Heating Coil PLF-FPLR",
-            "temperature_setpoint_node_name": "PSZ-Office Heating Coil Outlet"
+            "part_load_fraction_correlation_curve_name": "PSZ-Office Heating Coil PLF-FPLR"
         },
         "Zone3UnitHeaterHeatingCoil": {
             "air_inlet_node_name": "Zone3UnitHeaterFanOutletNode",
             "air_outlet_node_name": "Zone3UnitHeaterAirOutletNode",
             "availability_schedule_name": "Zone3HeatingCoilAvailability",
             "burner_efficiency": 0.8,
             "fuel_type": "NaturalGas",
             "nominal_capacity": "Autosize",
             "parasitic_electric_load": 0.0,
             "parasitic_fuel_load": 0
         }
     },
-    "CoilSystem:Cooling:DX": {
-        "PSZ-Fine Storage_Unitary_Package_DX": {
-            "availability_schedule_name": "COMPACT HVAC-ALWAYS 1",
-            "cooling_coil_name": "PSZ-Fine Storage Cooling Coil",
-            "cooling_coil_object_type": "Coil:Cooling:DX:TwoSpeed",
-            "dx_cooling_coil_system_inlet_node_name": "PSZ-Fine Storage Heating Coil Outlet",
-            "dx_cooling_coil_system_outlet_node_name": "PSZ-Fine Storage Air Loop Outlet",
-            "dx_cooling_coil_system_sensor_node_name": "PSZ-Fine Storage Air Loop Outlet"
-        },
-        "PSZ-Office_Unitary_Package_DX": {
-            "availability_schedule_name": "COMPACT HVAC-ALWAYS 1",
-            "cooling_coil_name": "PSZ-Office Cooling Coil",
-            "cooling_coil_object_type": "Coil:Cooling:DX:TwoSpeed",
-            "dx_cooling_coil_system_inlet_node_name": "PSZ-Office Heating Coil Outlet",
-            "dx_cooling_coil_system_outlet_node_name": "PSZ-Office Air Loop Outlet",
-            "dx_cooling_coil_system_sensor_node_name": "PSZ-Office Air Loop Outlet"
-        }
-    },
     "Construction": {
         "Air_Wall": {
             "outside_layer": "Air_Wall_Material"
         },
         "AtticRoofDeck": {
             "layer_2": "G02 16mm plywood",
             "outside_layer": "F12 Asphalt shingles"
@@ -1011,492 +1061,43 @@
             "layer_2": "R13_Insulation",
             "layer_3": "Gypsum or plaster board - 9.5mm",
             "outside_layer": "Gypsum or plaster board - 9.5mm"
         },
         "InteriorFurnishings": {
             "outside_layer": "Std Wood 6inch"
         },
+        "NonresWindow_U_0.36_SHGC_0.38": {
+            "outside_layer": "Nonres Window Glazing Layer"
+        },
         "OpaqueDoor": {
             "outside_layer": "Std Opaque Door Panel"
         },
         "Overhead Door_con": {
             "outside_layer": "Overhead Door_con Panel"
         },
         "Overhead Door_semi": {
             "outside_layer": "Overhead Door_semi Panel"
         },
+        "SemiHtdSkylight_U_0.75_SHGC_0.55": {
+            "outside_layer": "Semiheated Skylight Glazing Layer"
+        },
         "Skylight Double Clear": {
             "layer_2": "AIR 3MM",
             "layer_3": "CLEAR 2.5MM",
             "outside_layer": "CLEAR 2.5MM"
         },
+        "Skylight_U_0.5_SHGC_0.4": {
+            "outside_layer": "Nonres Skylight Glazing Layer"
+        },
         "Swinging Door_con": {
             "outside_layer": "Opaque Door panel_con"
         },
         "Swinging Door_semi": {
             "outside_layer": "Opaque Door panel_semi"
         },
-        "Window_U_0.19_SHGC_0.20": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "COATED POLY-55",
-            "layer_4": "AIR 13MM",
-            "layer_5": "CLEAR 6MM",
-            "outside_layer": "BRONZE 6MM"
-        },
-        "Window_U_0.24_SHGC_0.11": {
-            "layer_2": "ARGON 13MM",
-            "layer_3": "LoE SPEC SEL CLEAR 6MM Rev",
-            "outside_layer": "ECABS-2 COLORED 6MM"
-        },
-        "Window_U_0.24_SHGC_0.16": {
-            "layer_2": "ARGON 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "ECABS-2 COLORED 6MM"
-        },
-        "Window_U_0.24_SHGC_0.23": {
-            "layer_2": "ARGON 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE SPEC SEL TINT 6MM"
-        },
-        "Window_U_0.25_SHGC_0.40": {
-            "layer_2": "ARGON 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE TINT 6MM"
-        },
-        "Window_U_0.29_SHGC_0.11": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "LoE SPEC SEL CLEAR 6MM Rev",
-            "outside_layer": "ECREF-2 COLORED 6MM"
-        },
-        "Window_U_0.29_SHGC_0.17": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "ECABS-2 COLORED 6MM"
-        },
-        "Window_U_0.29_SHGC_0.22": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "COATED POLY-55",
-            "layer_4": "AIR 6MM",
-            "layer_5": "CLEAR 6MM",
-            "outside_layer": "BRONZE 6MM"
-        },
-        "Window_U_0.29_SHGC_0.45": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "LoE SPEC SEL CLEAR 6MM Rev",
-            "outside_layer": "ECREF-2 BLEACHED 6MM"
-        },
-        "Window_U_0.30_SHGC_0.40": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE TINT 6MM"
-        },
-        "Window_U_0.33_SHGC_0.11": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "LoE SPEC SEL CLEAR 6MM Rev",
-            "outside_layer": "ECREF-2 COLORED 6MM"
-        },
-        "Window_U_0.33_SHGC_0.40": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE TINT 6MM"
-        },
-        "Window_U_0.33_SHGC_0.45": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "COATED POLY-77",
-            "layer_4": "AIR 6MM",
-            "layer_5": "CLEAR 3MM",
-            "outside_layer": "CLEAR 3MM"
-        },
-        "Window_U_0.34_SHGC_0.40": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE TINT 6MM"
-        },
-        "Window_U_0.34_SHGC_0.45": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "PYR B CLEAR 6MM"
-        },
-        "Window_U_0.35_SHGC_0.26": {
-            "layer_2": "ARGON 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF C CLEAR MID 6MM"
-        },
-        "Window_U_0.35_SHGC_0.35": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE TINT 6MM"
-        },
-        "Window_U_0.36_SHGC_0.35": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE SPEC SEL TINT 6MM"
-        },
-        "Window_U_0.37_SHGC_0.45": {
-            "layer_2": "Gap_1_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_4321_LayerAvg"
-        },
-        "Window_U_0.38_SHGC_0.26": {
-            "layer_2": "ARGON 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF B TINT HI 6MM"
-        },
-        "Window_U_0.38_SHGC_0.30": {
-            "layer_2": "ARGON 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_0.38_SHGC_0.36": {
-            "layer_2": "Gap_9_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_2531_LayerAvg"
-        },
-        "Window_U_0.38_SHGC_0.41": {
-            "layer_2": "Gap_1_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_4313_LayerAvg"
-        },
-        "Window_U_0.39_SHGC_0.32": {
-            "outside_layer": "Theoretical Glass 347"
-        },
-        "Window_U_0.39_SHGC_0.36": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE TINT 6MM"
-        },
-        "Window_U_0.39_SHGC_0.38": {
-            "outside_layer": "Theoretical Glass 297"
-        },
-        "Window_U_0.39_SHGC_0.40": {
-            "layer_2": "Gap_1_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_282_LayerAvg"
-        },
-        "Window_U_0.40_SHGC_0.38": {
-            "layer_2": "Gap_1_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_8652_LayerAvg"
-        },
-        "Window_U_0.40_SHGC_0.4": {
-            "layer_2": "Gap_1_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_8652_LayerAvg"
-        },
-        "Window_U_0.40_SHGC_0.43": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE SPEC SEL CLEAR 3MM"
-        },
-        "Window_U_0.40_SHGC_0.45": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "LoE SPEC SEL CLEAR 6MM Rev",
-            "outside_layer": "ECABS-2 BLEACHED 6MM"
-        },
-        "Window_U_0.41_SHGC_0.38": {
-            "layer_2": "Gap_1_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_8652_LayerAvg"
-        },
-        "Window_U_0.42_SHGC_0.35": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE TINT 6MM"
-        },
-        "Window_U_0.42_SHGC_0.40": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE TINT 6MM"
-        },
-        "Window_U_0.42_SHGC_0.45": {
-            "layer_2": "ARGON 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF D CLEAR 6MM"
-        },
-        "Window_U_0.43_SHGC_0.26": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_0.43_SHGC_0.29": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "LoE SPEC SEL TINT 6MM"
-        },
-        "Window_U_0.44_SHGC_0.20": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF B TINT HI 6MM"
-        },
-        "Window_U_0.44_SHGC_0.26": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_0.44_SHGC_0.40": {
-            "layer_2": "Gap_9_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_9731_LayerAvg"
-        },
-        "Window_U_0.45_SHGC_0.27": {
-            "layer_2": "Air 13MM",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_12116_LayerAvg"
-        },
-        "Window_U_0.45_SHGC_0.31": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_0.45_SHGC_0.38": {
-            "layer_2": "Gap_1_W_0_0127",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_2532_LayerAvg"
-        },
-        "Window_U_0.46_SHGC_0.45": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "GREY 6MM"
-        },
-        "Window_U_0.47_SHGC_0.40": {
-            "layer_2": "Gap_1_W_0_0043",
-            "layer_3": "Glass_2010F_LayerAvg",
-            "outside_layer": "Glass_2052_LayerAvg"
-        },
-        "Window_U_0.48_SHGC_0.40": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF D CLEAR 6MM"
-        },
-        "Window_U_0.50_SHGC_0.25": {
-            "layer_2": "Gap_1_W_0_0042",
-            "layer_3": "Glass_2022F_LayerAvg",
-            "outside_layer": "Glass_2175_LayerAvg"
-        },
-        "Window_U_0.50_SHGC_0.40": {
-            "layer_2": "Gap_1_W_0_0038",
-            "layer_3": "Glass_2027F_LayerAvg",
-            "outside_layer": "Glass_2052_LayerAvg"
-        },
-        "Window_U_0.51_SHGC_0.25": {
-            "layer_2": "Gap_1_W_0_0090",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_1576_LayerAvg"
-        },
-        "Window_U_0.52_SHGC_0.22": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF B CLEAR LO 6MM"
-        },
-        "Window_U_0.52_SHGC_0.40": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF D CLEAR 6MM"
-        },
-        "Window_U_0.54_SHGC_0.13": {
-            "layer_2": "AIR 13MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF A CLEAR LO 6MM"
-        },
-        "Window_U_0.54_SHGC_0.18": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF A TINT MID 6MM"
-        },
-        "Window_U_0.54_SHGC_0.25": {
-            "layer_2": "Gap_1_W_0_0070",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_1576_LayerAvg"
-        },
-        "Window_U_0.54_SHGC_0.27": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF C CLEAR HI 6MM"
-        },
-        "Window_U_0.55_SHGC_0.25": {
-            "layer_2": "Gap_1_W_0_0032",
-            "layer_3": "Glass_2022F_LayerAvg",
-            "outside_layer": "Glass_2175_LayerAvg"
-        },
-        "Window_U_0.55_SHGC_0.31": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF D TINT 6MM"
-        },
-        "Window_U_0.55_SHGC_0.35": {
-            "layer_2": "Gap_1_W_0_0038",
-            "layer_3": "Glass_2027F_LayerAvg",
-            "outside_layer": "Glass_2052_LayerAvg"
-        },
-        "Window_U_0.56_SHGC_0.25": {
-            "layer_2": "Gap_1_W_0_0060",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_1576_LayerAvg"
-        },
-        "Window_U_0.56_SHGC_0.35": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF D TINT 6MM"
-        },
-        "Window_U_0.56_SHGC_0.76": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 3MM",
-            "outside_layer": "CLEAR 3MM"
-        },
-        "Window_U_0.57_SHGC_0.25": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF C CLEAR HI 6MM"
-        },
-        "Window_U_0.57_SHGC_0.39": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF D CLEAR 6MM"
-        },
-        "Window_U_0.57_SHGC_0.49": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "BLUE 6MM"
-        },
-        "Window_U_0.58_SHGC_0.25": {
-            "layer_2": "Gap_1_W_0_0052",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_1576_LayerAvg"
-        },
-        "Window_U_0.59_SHGC_0.25": {
-            "layer_2": "Gap_1_W_0_0048",
-            "layer_3": "Glass_102_LayerAvg",
-            "outside_layer": "Glass_1576_LayerAvg"
-        },
-        "Window_U_0.60_SHGC_0.25": {
-            "layer_2": "Gap_1_W_0_0025",
-            "layer_3": "Glass_2022F_LayerAvg",
-            "outside_layer": "Glass_2175_LayerAvg"
-        },
-        "Window_U_0.62_SHGC_0.25": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF C CLEAR HI 6MM"
-        },
-        "Window_U_0.62_SHGC_0.39": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF D CLEAR 6MM"
-        },
-        "Window_U_0.62_SHGC_0.49": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "BLUE 6MM"
-        },
-        "Window_U_0.65_SHGC_0.25": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF C CLEAR HI 6MM"
-        },
-        "Window_U_0.65_SHGC_0.35": {
-            "layer_2": "Gap_1_W_0_0024",
-            "layer_3": "Glass_2027F_LayerAvg",
-            "outside_layer": "Glass_2052_LayerAvg"
-        },
-        "Window_U_0.67_SHGC_0.77": {
-            "outside_layer": "PYR B CLEAR 3MM"
-        },
-        "Window_U_0.71_SHGC_0.25": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 6MM",
-            "outside_layer": "REF C CLEAR HI 6MM"
-        },
-        "Window_U_0.72_SHGC_0.25": {
-            "outside_layer": "REF B TINT MID 6MM"
-        },
-        "Window_U_0.75_SHGC_0.35": {
-            "layer_2": "Gap_1_W_0_0018",
-            "layer_3": "Glass_2027F_LayerAvg",
-            "outside_layer": "Glass_2052_LayerAvg"
-        },
-        "Window_U_0.75_SHGC_0.6": {
-            "layer_2": "AIR 6MM",
-            "layer_3": "CLEAR 3MM",
-            "outside_layer": "GREY 3MM"
-        },
-        "Window_U_0.75_SHGC_0.72": {
-            "outside_layer": "PYR B CLEAR 6MM"
-        },
-        "Window_U_0.85_SHGC_0.78": {
-            "outside_layer": "PYR A CLEAR 3MM"
-        },
-        "Window_U_0.88_SHGC_0.16": {
-            "outside_layer": "REF A CLEAR LO 6MM"
-        },
-        "Window_U_0.88_SHGC_0.27": {
-            "outside_layer": "ECREF-1 COLORED 6MM"
-        },
-        "Window_U_0.90_SHGC_0.40": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_0.98_SHGC_0.45": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_0.98_SHGC_0.68": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_0.9_SHGC_0.6": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_1.05_SHGC_0.40": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_1.08_SHGC_0.25": {
-            "outside_layer": "ECREF-1 COLORED 6MM"
-        },
-        "Window_U_1.15_SHGC_0.68": {
-            "outside_layer": "GREEN 3MM"
-        },
-        "Window_U_1.16_SHGC_0.25": {
-            "outside_layer": "ECREF-1 COLORED 6MM"
-        },
-        "Window_U_1.17_SHGC_0.39": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_1.17_SHGC_0.49": {
-            "outside_layer": "REF D CLEAR 6MM"
-        },
-        "Window_U_1.17_SHGC_0.68": {
-            "outside_layer": "GREEN 3MM"
-        },
-        "Window_U_1.22_SHGC_0.25": {
-            "outside_layer": "ECREF-1 COLORED 6MM"
-        },
-        "Window_U_1.22_SHGC_0.34": {
-            "outside_layer": "REF C CLEAR HI 6MM"
-        },
-        "Window_U_1.22_SHGC_0.39": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_1.22_SHGC_0.61": {
-            "outside_layer": "GREEN 6MM"
-        },
-        "Window_U_1.30_SHGC_0.68": {
-            "outside_layer": "GREEN 3MM"
-        },
-        "Window_U_1.60_SHGC_0.40": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_1.70_SHGC_0.36": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_1.80_SHGC_0.36": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_1.98_SHGC_0.36": {
-            "outside_layer": "REF B CLEAR HI 6MM"
-        },
-        "Window_U_1.98_SHGC_0.61": {
-            "outside_layer": "GREEN 6MM"
-        },
         "basement_wall": {
             "outside_layer": "M10 200mm concrete block basement wall"
         },
         "ext_slab_6in": {
             "outside_layer": "150mm Normalweight concrete floor"
         },
         "ext_slab_6in_with_carpet": {
@@ -1584,82 +1185,81 @@
             "outside_layer": "CP02 CARPET PAD"
         },
         "semiheated_roof": {
             "layer_2": "Semiheated_Roof_Insulation",
             "outside_layer": "F08 Metal roof surface"
         }
     },
+    "Construction:FfactorGroundFloor": {
+        "BulkStorageFloor_Ffactor": {
+            "area": 3204.8422772668932,
+            "f_factor": 1.26363,
+            "perimeterexposed": 185.91893288462248
+        },
+        "FineStorageFloor_Ffactor": {
+            "area": 1156.5300391876226,
+            "f_factor": 1.26363,
+            "perimeterexposed": 71.62450693096137
+        },
+        "OfficeFloor_Ffactor": {
+            "area": 236.87964658059664,
+            "f_factor": 1.26363,
+            "perimeterexposed": 35.05029062578953
+        }
+    },
     "Controller:OutdoorAir": {
         "PSZ-Fine Storage OA Controller": {
             "actuator_node_name": "PSZ-Fine Storage Outside Air Inlet",
             "economizer_control_action_type": "ModulateFlow",
             "economizer_control_type": "DifferentialDryBulb",
-            "lockout_type": "NoLockout",
-            "maximum_fraction_of_outdoor_air_schedule_name": "PSZ_Fine_Timestep_Econ_Eff_SCH",
+            "lockout_type": "LockoutWithHeating",
+            "maximum_fraction_of_outdoor_air_schedule_name": "SZ_system_OA_Max_Frac_SCH",
             "maximum_outdoor_air_flow_rate": "Autosize",
             "minimum_limit_type": "FixedMinimum",
             "minimum_outdoor_air_flow_rate": "Autosize",
             "minimum_outdoor_air_schedule_name": "MinOA_MotorizedDamper_Sched",
             "mixed_air_node_name": "PSZ-Fine Storage Mixed Air Outlet",
             "relief_air_outlet_node_name": "PSZ-Fine Storage Relief Air Outlet",
             "return_air_node_name": "PSZ-Fine Storage Air Loop Inlet"
         },
         "PSZ-Office OA Controller": {
             "actuator_node_name": "PSZ-Office Outside Air Inlet",
             "economizer_control_action_type": "ModulateFlow",
-            "economizer_control_type": "NoEconomizer",
-            "lockout_type": "NoLockout",
-            "maximum_fraction_of_outdoor_air_schedule_name": "PSZ_Office_Timestep_Econ_Eff_SCH",
+            "economizer_control_type": "DifferentialDryBulb",
+            "lockout_type": "LockoutWithHeating",
+            "maximum_fraction_of_outdoor_air_schedule_name": "SZ_system_OA_Max_Frac_SCH",
             "maximum_outdoor_air_flow_rate": "Autosize",
             "minimum_limit_type": "FixedMinimum",
             "minimum_outdoor_air_flow_rate": "Autosize",
             "minimum_outdoor_air_schedule_name": "MinOA_MotorizedDamper_Sched",
             "mixed_air_node_name": "PSZ-Office Mixed Air Outlet",
             "relief_air_outlet_node_name": "PSZ-Office Relief Air Outlet",
             "return_air_node_name": "PSZ-Office Air Loop Inlet"
         }
     },
+    "ConvergenceLimits": {
+        "ConvergenceLimits 1": {
+            "maximum_hvac_iterations": 5,
+            "minimum_system_timestep": 15
+        }
+    },
     "Curve:Biquadratic": {
-        "PSZ-Fine Storage DX Coil Cap-FT": {
-            "coefficient1_constant": 0.942587793,
-            "coefficient2_x": 0.009543347,
-            "coefficient3_x_2": 0.00068377,
-            "coefficient4_y": -0.011042676,
-            "coefficient5_y_2": 5.249e-06,
-            "coefficient6_x_y": -9.72e-06,
-            "maximum_value_of_x": 23.88889,
-            "maximum_value_of_y": 46.11111,
-            "minimum_value_of_x": 12.77778,
-            "minimum_value_of_y": 23.88889
-        },
-        "PSZ-Fine Storage DX Coil EIR-FT": {
-            "coefficient1_constant": 0.342414409,
-            "coefficient2_x": 0.034885008,
-            "coefficient3_x_2": -0.0006237,
-            "coefficient4_y": 0.004977216,
-            "coefficient5_y_2": 0.000437951,
-            "coefficient6_x_y": -0.000728028,
-            "maximum_value_of_x": 23.88889,
-            "maximum_value_of_y": 46.11111,
-            "minimum_value_of_x": 12.77778,
-            "minimum_value_of_y": 23.88889
-        },
-        "PSZ-Office DX Coil Cap-FT": {
+        "PSZ-AC_Unitary_PackagecoolCapFT": {
             "coefficient1_constant": 0.942587793,
             "coefficient2_x": 0.009543347,
             "coefficient3_x_2": 0.00068377,
             "coefficient4_y": -0.011042676,
             "coefficient5_y_2": 5.249e-06,
             "coefficient6_x_y": -9.72e-06,
             "maximum_value_of_x": 23.88889,
             "maximum_value_of_y": 46.11111,
             "minimum_value_of_x": 12.77778,
             "minimum_value_of_y": 23.88889
         },
-        "PSZ-Office DX Coil EIR-FT": {
+        "PSZ-AC_Unitary_PackagecoolEIRFT": {
             "coefficient1_constant": 0.342414409,
             "coefficient2_x": 0.034885008,
             "coefficient3_x_2": -0.0006237,
             "coefficient4_y": 0.004977216,
             "coefficient5_y_2": 0.000437951,
             "coefficient6_x_y": -0.000728028,
             "maximum_value_of_x": 23.88889,
@@ -1683,167 +1283,146 @@
             "coefficient3_x_2": 0,
             "coefficient4_x_3": 0,
             "maximum_value_of_x": 1,
             "minimum_value_of_x": 0
         }
     },
     "Curve:Quadratic": {
-        "PSZ-Fine Storage DX Coil Cap-FF": {
-            "coefficient1_constant": 0.8,
-            "coefficient2_x": 0.2,
-            "coefficient3_x_2": 0,
-            "maximum_value_of_x": 1.5,
-            "minimum_value_of_x": 0.5
-        },
-        "PSZ-Fine Storage DX Coil EIR-FF": {
+        "PSZ-AC_Unitary_PackagecoolEIRFFF": {
             "coefficient1_constant": 1.1552,
             "coefficient2_x": -0.1808,
             "coefficient3_x_2": 0.0256,
             "maximum_value_of_x": 1.5,
             "minimum_value_of_x": 0.5
         },
-        "PSZ-Fine Storage DX Coil PLF": {
-            "coefficient1_constant": 0.85,
-            "coefficient2_x": 0.15,
-            "coefficient3_x_2": 0,
-            "maximum_value_of_x": 1,
-            "minimum_value_of_x": 0
-        },
-        "PSZ-Office DX Coil Cap-FF": {
+        "PSZ-AC_Unitary_PackagecoolFFF": {
             "coefficient1_constant": 0.8,
             "coefficient2_x": 0.2,
             "coefficient3_x_2": 0,
             "maximum_value_of_x": 1.5,
             "minimum_value_of_x": 0.5
         },
-        "PSZ-Office DX Coil EIR-FF": {
-            "coefficient1_constant": 1.1552,
-            "coefficient2_x": -0.1808,
-            "coefficient3_x_2": 0.0256,
-            "maximum_value_of_x": 1.5,
-            "minimum_value_of_x": 0.5
-        },
-        "PSZ-Office DX Coil PLF": {
+        "PSZ-AC_Unitary_PackagecoolPLR": {
             "coefficient1_constant": 0.85,
             "coefficient2_x": 0.15,
             "coefficient3_x_2": 0,
             "maximum_value_of_x": 1,
             "minimum_value_of_x": 0
         }
     },
     "Daylighting:Controls": {
         "Zone1 Office_DaylCtrl": {
             "control_data": [
                 {
                     "daylighting_reference_point_name": "Zone1 Office_DaylRefPt1",
-                    "fraction_of_zone_controlled_by_reference_point": 0.29,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.29,
+                    "illuminance_setpoint_at_reference_point": 377.0
                 },
                 {
                     "daylighting_reference_point_name": "Zone1 Office_DaylRefPt2",
-                    "fraction_of_zone_controlled_by_reference_point": 0.1,
-                    "illuminance_setpoint_at_reference_point": 375.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.1,
+                    "illuminance_setpoint_at_reference_point": 377.0
                 }
             ],
             "daylighting_method": "SplitFlux",
             "glare_calculation_azimuth_angle_of_view_direction_clockwise_from_zone_y_axis": 180.0,
             "glare_calculation_daylighting_reference_point_name": "Zone1 Office_DaylRefPt1",
-            "lighting_control_type": "Stepped",
+            "lighting_control_type": "ContinuousOff",
             "maximum_allowable_discomfort_glare_index": 22.0,
-            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.3,
+            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "minimum_light_output_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "number_of_stepped_control_steps": 3,
             "probability_lighting_will_be_reset_when_needed_in_manual_stepped_control": 1.0,
-            "zone_name": "Zone1 Office"
+            "zone_or_space_name": "Zone1 Office"
         },
         "Zone2 Fine Storage_DaylCtrl": {
             "control_data": [
                 {
                     "daylighting_reference_point_name": "Zone2 Fine Storage_DaylRefPt1",
-                    "fraction_of_zone_controlled_by_reference_point": 0.25,
-                    "illuminance_setpoint_at_reference_point": 300.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.25,
+                    "illuminance_setpoint_at_reference_point": 323.0
                 },
                 {
                     "daylighting_reference_point_name": "Zone2 Fine Storage_DaylRefPt2",
-                    "fraction_of_zone_controlled_by_reference_point": 0.25,
-                    "illuminance_setpoint_at_reference_point": 300.0
+                    "fraction_of_lights_controlled_by_reference_point": 0.25,
+                    "illuminance_setpoint_at_reference_point": 323.0
                 }
             ],
             "daylighting_method": "SplitFlux",
             "glare_calculation_azimuth_angle_of_view_direction_clockwise_from_zone_y_axis": 0.0,
             "glare_calculation_daylighting_reference_point_name": "Zone2 Fine Storage_DaylRefPt1",
-            "lighting_control_type": "Stepped",
+            "lighting_control_type": "ContinuousOff",
             "maximum_allowable_discomfort_glare_index": 22.0,
-            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.3,
+            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "minimum_light_output_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "number_of_stepped_control_steps": 3,
             "probability_lighting_will_be_reset_when_needed_in_manual_stepped_control": 1.0,
-            "zone_name": "Zone2 Fine Storage"
+            "zone_or_space_name": "Zone2 Fine Storage"
         },
         "Zone3 Bulk Storage_DaylCtrl": {
             "control_data": [
                 {
                     "daylighting_reference_point_name": "Zone3 Bulk Storage_DaylRefPt1",
-                    "fraction_of_zone_controlled_by_reference_point": 0.25,
-                    "illuminance_setpoint_at_reference_point": 200
+                    "fraction_of_lights_controlled_by_reference_point": 0.25,
+                    "illuminance_setpoint_at_reference_point": 215
                 },
                 {
                     "daylighting_reference_point_name": "Zone3 Bulk Storage_DaylRefPt2",
-                    "fraction_of_zone_controlled_by_reference_point": 0.25,
-                    "illuminance_setpoint_at_reference_point": 200
+                    "fraction_of_lights_controlled_by_reference_point": 0.25,
+                    "illuminance_setpoint_at_reference_point": 215
                 }
             ],
             "daylighting_method": "SplitFlux",
             "glare_calculation_azimuth_angle_of_view_direction_clockwise_from_zone_y_axis": 0,
             "glare_calculation_daylighting_reference_point_name": "Zone3 Bulk Storage_DaylRefPt1",
-            "lighting_control_type": "Stepped",
+            "lighting_control_type": "ContinuousOff",
             "maximum_allowable_discomfort_glare_index": 22,
-            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.3,
+            "minimum_input_power_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "minimum_light_output_fraction_for_continuous_or_continuousoff_dimming_control": 0.2,
             "number_of_stepped_control_steps": 3,
             "probability_lighting_will_be_reset_when_needed_in_manual_stepped_control": 1,
-            "zone_name": "Zone3 Bulk Storage"
+            "zone_or_space_name": "Zone3 Bulk Storage"
         }
     },
     "Daylighting:ReferencePoint": {
         "Zone1 Office_DaylRefPt1": {
             "x_coordinate_of_reference_point": 3.2675,
             "y_coordinate_of_reference_point": 4.5718,
             "z_coordinate_of_reference_point": 0.762,
-            "zone_name": "Zone1 Office"
+            "zone_or_space_name": "Zone1 Office"
         },
         "Zone1 Office_DaylRefPt2": {
             "x_coordinate_of_reference_point": 20.4216,
             "y_coordinate_of_reference_point": 4.5718,
             "z_coordinate_of_reference_point": 0.762,
-            "zone_name": "Zone1 Office"
+            "zone_or_space_name": "Zone1 Office"
         },
         "Zone2 Fine Storage_DaylRefPt1": {
             "x_coordinate_of_reference_point": 27.8892,
             "y_coordinate_of_reference_point": 24.9936,
             "z_coordinate_of_reference_point": 0.762,
-            "zone_name": "Zone2 Fine Storage"
+            "zone_or_space_name": "Zone2 Fine Storage"
         },
         "Zone2 Fine Storage_DaylRefPt2": {
             "x_coordinate_of_reference_point": 3.81,
             "y_coordinate_of_reference_point": 24.9936,
             "z_coordinate_of_reference_point": 0.762,
-            "zone_name": "Zone2 Fine Storage"
+            "zone_or_space_name": "Zone2 Fine Storage"
         },
         "Zone3 Bulk Storage_DaylRefPt1": {
             "x_coordinate_of_reference_point": 22.9,
             "y_coordinate_of_reference_point": 48,
             "z_coordinate_of_reference_point": 0,
-            "zone_name": "Zone3 Bulk Storage"
+            "zone_or_space_name": "Zone3 Bulk Storage"
         },
         "Zone3 Bulk Storage_DaylRefPt2": {
             "x_coordinate_of_reference_point": 22.9,
             "y_coordinate_of_reference_point": 34.7,
             "z_coordinate_of_reference_point": 0,
-            "zone_name": "Zone3 Bulk Storage"
+            "zone_or_space_name": "Zone3 Bulk Storage"
         }
     },
     "DesignSpecification:OutdoorAir": {
         "SZ DSOA Zone1 Office": {
             "outdoor_air_flow_per_person": 0.0,
             "outdoor_air_flow_per_zone": 0,
             "outdoor_air_flow_per_zone_floor_area": 0.000431801,
@@ -1862,47 +1441,27 @@
             "outdoor_air_method": "Flow/Area"
         }
     },
     "ElectricEquipment": {
         "Bulk Storage  Plug Load": {
             "design_level": 8200.12,
             "design_level_calculation_method": "EquipmentLevel",
-            "end_use_subcategory": "General",
+            "end_use_subcategory": "MiscPlug",
             "schedule_name": "Bulk Storage Plug Schedule",
-            "zone_or_zonelist_name": "Zone3 Bulk Storage"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Zone3 Bulk Storage"
         },
         "Office Plug Load": {
             "design_level": 1912.5,
             "design_level_calculation_method": "EquipmentLevel",
-            "end_use_subcategory": "General",
+            "end_use_subcategory": "MiscPlug",
             "schedule_name": "Office_Plug_SCH",
-            "zone_or_zonelist_name": "Zone1 Office"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Zone1 Office"
         }
     },
     "EnergyManagementSystem:Actuator": {
-        "PSZ_Fine_Fan_Pressure": {
-            "actuated_component_control_type": "Fan Pressure Rise",
-            "actuated_component_type": "Fan",
-            "actuated_component_unique_name": "PSZ-Fine Storage Supply Fan"
-        },
-        "PSZ_Fine_Timestep_Econ_Eff": {
-            "actuated_component_control_type": "Schedule Value",
-            "actuated_component_type": "Schedule:Constant",
-            "actuated_component_unique_name": "PSZ_Fine_Timestep_Econ_Eff_SCH"
-        },
-        "PSZ_Office_Fan_Pressure": {
-            "actuated_component_control_type": "Fan Pressure Rise",
-            "actuated_component_type": "Fan",
-            "actuated_component_unique_name": "PSZ-Office Supply Fan"
-        },
-        "PSZ_Office_Timestep_Econ_Eff": {
-            "actuated_component_control_type": "Schedule Value",
-            "actuated_component_type": "Schedule:Constant",
-            "actuated_component_unique_name": "PSZ_Office_Timestep_Econ_Eff_SCH"
-        },
         "Zone1_Office_Light_Actuator": {
             "actuated_component_control_type": "Electricity Rate",
             "actuated_component_type": "Lights",
             "actuated_component_unique_name": "Office Lights"
         },
         "Zone2_Fine_Storage_Light_Actuator": {
             "actuated_component_control_type": "Electricity Rate",
@@ -1911,848 +1470,29 @@
         },
         "Zone3_Bulk_Storage_Light_Actuator": {
             "actuated_component_control_type": "Electricity Rate",
             "actuated_component_type": "Lights",
             "actuated_component_unique_name": "Bulk Storage Area Lights"
         }
     },
-    "EnergyManagementSystem:GlobalVariable": {
-        "EnergyManagementSystem:GlobalVariable 1": {
-            "variables": [
-                {
-                    "erl_variable_name": "PSZ_Office_FanPwrExponent"
-                },
-                {
-                    "erl_variable_name": "PSZ_Office_Stage1Speed"
-                },
-                {
-                    "erl_variable_name": "PSZ_Office_Stage2Speed"
-                },
-                {
-                    "erl_variable_name": "PSZ_Office_HeatSpeed"
-                },
-                {
-                    "erl_variable_name": "PSZ_Office_VenSpeed"
-                },
-                {
-                    "erl_variable_name": "PSZ_Office_Number_of_Stages"
-                }
-            ]
-        },
-        "EnergyManagementSystem:GlobalVariable 2": {
-            "variables": [
-                {
-                    "erl_variable_name": "PSZ_Fine_FanPwrExponent"
-                },
-                {
-                    "erl_variable_name": "PSZ_Fine_Stage1Speed"
-                },
-                {
-                    "erl_variable_name": "PSZ_Fine_Stage2Speed"
-                },
-                {
-                    "erl_variable_name": "PSZ_Fine_HeatSpeed"
-                },
-                {
-                    "erl_variable_name": "PSZ_Fine_VenSpeed"
-                },
-                {
-                    "erl_variable_name": "PSZ_Fine_Number_of_Stages"
-                }
-            ]
-        }
-    },
     "EnergyManagementSystem:InternalVariable": {
-        "PSZ_Fine_DesignFlowMass": {
-            "internal_data_index_key_name": "PSZ-Fine Storage OA Controller",
-            "internal_data_type": "Outdoor Air Controller Maximum Mass Flow Rate"
-        },
-        "PSZ_Fine_Fan_DesignPressure": {
-            "internal_data_index_key_name": "PSZ-Fine Storage Supply Fan",
-            "internal_data_type": "Fan Nominal Pressure Rise"
-        },
-        "PSZ_Fine_OADesignMass": {
-            "internal_data_index_key_name": "PSZ-Fine Storage OA Controller",
-            "internal_data_type": "Outdoor Air Controller Minimum Mass Flow Rate"
-        },
-        "PSZ_Office_DesignFlowMass": {
-            "internal_data_index_key_name": "PSZ-Office OA Controller",
-            "internal_data_type": "Outdoor Air Controller Maximum Mass Flow Rate"
-        },
-        "PSZ_Office_Fan_DesignPressure": {
-            "internal_data_index_key_name": "PSZ-Office Supply Fan",
-            "internal_data_type": "Fan Nominal Pressure Rise"
-        },
-        "PSZ_Office_OADesignMass": {
-            "internal_data_index_key_name": "PSZ-Office OA Controller",
-            "internal_data_type": "Outdoor Air Controller Minimum Mass Flow Rate"
-        },
         "Zone1_Office_Area": {
             "internal_data_index_key_name": "Zone1 Office",
             "internal_data_type": "Zone Floor Area"
         },
         "Zone2_Fine_Storage_Area": {
             "internal_data_index_key_name": "Zone2 Fine Storage",
             "internal_data_type": "Zone Floor Area"
         },
         "Zone3_Bulk_Storage_Area": {
             "internal_data_index_key_name": "Zone3 Bulk Storage",
             "internal_data_type": "Zone Floor Area"
         }
     },
     "EnergyManagementSystem:Program": {
-        "PSZ_Fine_Economizer_CTRL_Prog": {
-            "lines": [
-                {
-                    "program_line": "SET PSZ_Fine_Timestep_Econ_Eff = 0.7"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_MaxE = 0.7"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_DAT_Rqd = (PSZ_Fine_DAT_Rqd*1.8) +32"
-                },
-                {
-                    "program_line": "SET OAT_F = (OAT_F*1.8) +32"
-                },
-                {
-                    "program_line": "SET OAwb_F = (OAwb_F*1.8) +32"
-                },
-                {
-                    "program_line": "IF PSZ_Fine_OAFlowMass > (PSZ_Fine_OADesignMass * PSZ_Fine_OASch)"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Econo_Active = 1"
-                },
-                {
-                    "program_line": "ELSE"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Econo_Active = 0"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_dT_Needed = 75 - PSZ_Fine_DAT_Rqd"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Cool_Des_dT = ((98*0.15) + (75*(1-0.15))) - 55"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Cool_Load = PSZ_Fine_dT_Needed/ PSZ_Fine_Cool_Des_dT"
-                },
-                {
-                    "program_line": "IF PSZ_Fine_Cool_Load > 1"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Cool_Load = 1"
-                },
-                {
-                    "program_line": "ELSEIF PSZ_Fine_Cool_Load < 0"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Cool_Load = 0"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "IF PSZ_Fine_Econo_Active == 1"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Stage = PSZ_Fine_Number_of_Stages"
-                },
-                {
-                    "program_line": "IF PSZ_Fine_Stage == 2"
-                },
-                {
-                    "program_line": "IF PSZ_Fine_Cool_Load < 0.6"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Timestep_Econ_Eff = PSZ_Fine_MaxE"
-                },
-                {
-                    "program_line": "ELSE"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_ECO_Eff = 0-2.18919863612305"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_ECO_Eff = PSZ_Fine_ECO_Eff + (0-0.674461284910428 * PSZ_Fine_Cool_Load)"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_ECO_Eff = PSZ_Fine_ECO_Eff + (0.000459106275872404 * (OAT_F^2))"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_ECO_Eff = PSZ_Fine_ECO_Eff + (0-0.00000484778537945252 * (OAT_F^3))"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_ECO_Eff = PSZ_Fine_ECO_Eff + (0.182915713033586 * OAwb_F)"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_ECO_Eff = PSZ_Fine_ECO_Eff + (0-0.00382838660261133 * (OAwb_F^2))"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_ECO_Eff = PSZ_Fine_ECO_Eff + (0.0000255567460240583 * (OAwb_F^3))"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Timestep_Econ_Eff = PSZ_Fine_ECO_Eff"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "ELSE"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_ECO_Eff = 2.36337942464462"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_ECO_Eff = PSZ_Fine_ECO_Eff + (0-0.409939515512619 * PSZ_Fine_Cool_Load)"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_ECO_Eff = PSZ_Fine_ECO_Eff + (0-0.0565205596792225 * OAwb_F)"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_ECO_Eff = PSZ_Fine_ECO_Eff + (0-0.0000632612294169389 * (OAT_F^2))"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Timestep_Econ_Eff = PSZ_Fine_ECO_Eff + (0.000571724868775081 * (OAwb_F^2))"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "IF PSZ_Fine_Timestep_Econ_Eff > PSZ_Fine_MaxE"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Timestep_Econ_Eff = PSZ_Fine_MaxE"
-                },
-                {
-                    "program_line": "ELSEIF PSZ_Fine_Timestep_Econ_Eff < (PSZ_Fine_OADesignMass * PSZ_Fine_OASch)"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Timestep_Econ_Eff = (PSZ_Fine_OADesignMass * PSZ_Fine_OASch)"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "ENDIF"
-                }
-            ]
-        },
-        "PSZ_Fine_Fan_Control": {
-            "lines": [
-                {
-                    "program_line": "SET PSZ_FINE_Number_of_Stages = 1"
-                },
-                {
-                    "program_line": "IF PSZ_Fine_Number_of_Stages == 1"
-                },
-                {
-                    "program_line": "Return"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "IF PSZ_Fine_HeatingRTF > 0"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Heating = PSZ_Fine_HeatingRTF"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Ven = 1 - PSZ_Fine_HeatingRTF"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Eco = 0"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Stage1 = 0"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Stage2 = 0"
-                },
-                {
-                    "program_line": "ELSE"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Heating = 0"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_EcoSpeed = PSZ_Fine_VenSpeed"
-                },
-                {
-                    "program_line": "IF PSZ_Fine_SpeedRatio == 0"
-                },
-                {
-                    "program_line": "IF PSZ_Fine_RTF > 0"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Stage1 = PSZ_Fine_RTF"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Stage2 = 0"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Ven = 1-PSZ_Fine_RTF"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Eco = 0"
-                },
-                {
-                    "program_line": "IF PSZ_Fine_OAFlowMass > (PSZ_Fine_OADesignMass * PSZ_Fine_OASch)"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Stage1Speed = 1.0"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "ELSE"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Stage1 = 0"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Stage2 = 0"
-                },
-                {
-                    "program_line": "IF PSZ_Fine_OAFlowMass > (PSZ_Fine_OADesignMass * PSZ_Fine_OASch)"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Eco = 1.0"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Ven = 0"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Exp_DAT = PSZ_Fine_DAT_Rqd - (1-PSZ_Fine_VenSpeed) * ZONE2 FINE STORAGE_Temp"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Exp_DAT = PSZ_Fine_Exp_DAT/PSZ_Fine_VenSpeed"
-                },
-                {
-                    "program_line": "IF OAT_F > PSZ_Fine_Exp_DAT"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_EcoSpeed = PSZ_Fine_Stage2Speed"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "ELSE"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Eco = 0"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Ven = 1.0"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "ELSE"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Stage1 = 1- PSZ_Fine_SpeedRatio"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Stage2 = PSZ_Fine_SpeedRatio"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Ven = 0"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Eco = 0"
-                },
-                {
-                    "program_line": "IF PSZ_Fine_OAFlowMass > (PSZ_Fine_OADesignMass * PSZ_Fine_OASch)"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Stage1Speed = 1.0"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_FPR = PSZ_Fine_Ven * (PSZ_Fine_VenSpeed ^ PSZ_Fine_FanPwrExponent)"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_FPR = PSZ_Fine_FPR + PSZ_Fine_Eco * (PSZ_Fine_EcoSpeed ^ PSZ_Fine_FanPwrExponent)"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_FPR_1 = PSZ_Fine_Stage1 * (PSZ_Fine_Stage1Speed ^ PSZ_Fine_FanPwrExponent)"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_FPR = PSZ_Fine_FPR + PSZ_Fine_FPR_1"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_FPR_2 = PSZ_Fine_Stage2 * (PSZ_Fine_Stage2Speed ^ PSZ_Fine_FanPwrExponent)"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_FPR = PSZ_Fine_FPR + PSZ_Fine_FPR_2"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_FPR_3 = PSZ_Fine_Heating * (PSZ_Fine_HeatSpeed ^ PSZ_Fine_FanPwrExponent)"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_FanPwrRatio = PSZ_Fine_FPR +  PSZ_Fine_FPR_3"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Fan_Pressure = PSZ_Fine_Fan_DesignPressure * PSZ_Fine_FanPwrRatio"
-                }
-            ]
-        },
-        "PSZ_Fine_Set_Fan_Par": {
-            "lines": [
-                {
-                    "program_line": "SET PSZ_FINE_Number_of_Stages = 1"
-                },
-                {
-                    "program_line": "IF PSZ_Fine_Number_of_Stages == 1"
-                },
-                {
-                    "program_line": "Return"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_FanPwrExponent = 2.2"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_OAFrac = PSZ_Fine_OAFlowMass/PSZ_Fine_DesignFlowMass"
-                },
-                {
-                    "program_line": "IF  PSZ_Fine_OAFrac < 0.66"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_VenSpeed = 0.66"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Stage1Speed = 0.66"
-                },
-                {
-                    "program_line": "ELSE"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_VenSpeed = PSZ_Fine_OAFrac"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Stage1Speed = PSZ_Fine_OAFrac"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_Stage2Speed = 1.0"
-                },
-                {
-                    "program_line": "SET PSZ_Fine_HeatSpeed = 1.0"
-                }
-            ]
-        },
-        "PSZ_Fine_Set_Number_of_Stages": {
-            "lines": [
-                {
-                    "program_line": "SET PSZ_FINE_Number_of_Stages = 1"
-                }
-            ]
-        },
-        "PSZ_Office_Economizer_CTRL_Prog": {
-            "lines": [
-                {
-                    "program_line": "SET PSZ_Office_Timestep_Econ_Eff = 0.7"
-                },
-                {
-                    "program_line": "SET PSZ_Office_MaxE = 0.7"
-                },
-                {
-                    "program_line": "SET PSZ_Office_DAT_Rqd = (PSZ_Office_DAT_Rqd*1.8) +32"
-                },
-                {
-                    "program_line": "SET OAT_F = (OAT_F*1.8) +32"
-                },
-                {
-                    "program_line": "SET OAwb_F = (OAwb_F*1.8) +32"
-                },
-                {
-                    "program_line": "IF PSZ_Office_OAFlowMass > (PSZ_Office_OADesignMass * PSZ_Office_OASch)"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Econo_Active = 1"
-                },
-                {
-                    "program_line": "ELSE"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Econo_Active = 0"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "SET PSZ_Office_dT_Needed = 75 - PSZ_Office_DAT_Rqd"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Cool_Des_dT = ((98*0.15) + (75*(1-0.15))) - 55"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Cool_Load = PSZ_Office_dT_Needed/ PSZ_Office_Cool_Des_dT"
-                },
-                {
-                    "program_line": "IF PSZ_Office_Cool_Load > 1"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Cool_Load = 1"
-                },
-                {
-                    "program_line": "ELSEIF PSZ_Office_Cool_Load < 0"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Cool_Load = 0"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "IF PSZ_Office_Econo_Active == 1"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Stage = PSZ_Office_Number_of_Stages"
-                },
-                {
-                    "program_line": "IF PSZ_Office_Stage == 2"
-                },
-                {
-                    "program_line": "IF PSZ_Office_Cool_Load < 0.6"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Timestep_Econ_Eff = PSZ_Office_MaxE"
-                },
-                {
-                    "program_line": "ELSE"
-                },
-                {
-                    "program_line": "SET PSZ_Office_ECO_Eff = 0-2.18919863612305"
-                },
-                {
-                    "program_line": "SET PSZ_Office_ECO_Eff = PSZ_Office_ECO_Eff + (0-0.674461284910428 * PSZ_Office_Cool_Load)"
-                },
-                {
-                    "program_line": "SET PSZ_Office_ECO_Eff = PSZ_Office_ECO_Eff + (0.000459106275872404 * (OAT_F^2))"
-                },
-                {
-                    "program_line": "SET PSZ_Office_ECO_Eff = PSZ_Office_ECO_Eff + (0-0.00000484778537945252 * (OAT_F^3))"
-                },
-                {
-                    "program_line": "SET PSZ_Office_ECO_Eff = PSZ_Office_ECO_Eff + (0.182915713033586 * OAwb_F)"
-                },
-                {
-                    "program_line": "SET PSZ_Office_ECO_Eff = PSZ_Office_ECO_Eff + (0-0.00382838660261133 * (OAwb_F^2))"
-                },
-                {
-                    "program_line": "SET PSZ_Office_ECO_Eff = PSZ_Office_ECO_Eff + (0.0000255567460240583 * (OAwb_F^3))"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Timestep_Econ_Eff = PSZ_Office_ECO_Eff"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "ELSE"
-                },
-                {
-                    "program_line": "SET PSZ_Office_ECO_Eff = 2.36337942464462"
-                },
-                {
-                    "program_line": "SET PSZ_Office_ECO_Eff = PSZ_Office_ECO_Eff + (0-0.409939515512619 * PSZ_Office_Cool_Load)"
-                },
-                {
-                    "program_line": "SET PSZ_Office_ECO_Eff = PSZ_Office_ECO_Eff + (0-0.0565205596792225 * OAwb_F)"
-                },
-                {
-                    "program_line": "SET PSZ_Office_ECO_Eff = PSZ_Office_ECO_Eff + (0-0.0000632612294169389 * (OAT_F^2))"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Timestep_Econ_Eff = PSZ_Office_ECO_Eff + (0.000571724868775081 * (OAwb_F^2))"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "IF PSZ_Office_Timestep_Econ_Eff > PSZ_Office_MaxE"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Timestep_Econ_Eff = PSZ_Office_MaxE"
-                },
-                {
-                    "program_line": "ELSEIF PSZ_Office_Timestep_Econ_Eff < (PSZ_Office_OADesignMass * PSZ_Office_OASch)"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Timestep_Econ_Eff = (PSZ_Office_OADesignMass * PSZ_Office_OASch)"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "ENDIF"
-                }
-            ]
-        },
-        "PSZ_Office_Fan_Control": {
-            "lines": [
-                {
-                    "program_line": "SET PSZ_OFFICE_Number_of_Stages =  1"
-                },
-                {
-                    "program_line": "IF PSZ_Office_Number_of_Stages == 1"
-                },
-                {
-                    "program_line": "Return"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "IF PSZ_Office_HeatingRTF > 0"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Heating = PSZ_Office_HeatingRTF"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Ven = 1 - PSZ_Office_HeatingRTF"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Eco = 0"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Stage1 = 0"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Stage2 = 0"
-                },
-                {
-                    "program_line": "ELSE"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Heating = 0"
-                },
-                {
-                    "program_line": "SET PSZ_Office_EcoSpeed = PSZ_Office_VenSpeed"
-                },
-                {
-                    "program_line": "IF PSZ_Office_SpeedRatio == 0"
-                },
-                {
-                    "program_line": "IF PSZ_Office_RTF > 0"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Stage1 = PSZ_Office_RTF"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Stage2 = 0"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Ven = 1-PSZ_Office_RTF"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Eco = 0"
-                },
-                {
-                    "program_line": "IF PSZ_Office_OAFlowMass > (PSZ_Office_OADesignMass * PSZ_Office_OASch)"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Stage1Speed = 1.0"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "ELSE"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Stage1 = 0"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Stage2 = 0"
-                },
-                {
-                    "program_line": "IF PSZ_Office_OAFlowMass > (PSZ_Office_OADesignMass * PSZ_Office_OASch)"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Eco = 1.0"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Ven = 0"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Exp_DAT = PSZ_Office_DAT_Rqd - (1-PSZ_Office_VenSpeed) * ZONE1 OFFICE_Temp"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Exp_DAT = PSZ_Office_Exp_DAT/PSZ_Office_VenSpeed"
-                },
-                {
-                    "program_line": "IF OAT_F > PSZ_Office_Exp_DAT"
-                },
-                {
-                    "program_line": "SET PSZ_Office_EcoSpeed = PSZ_Office_Stage2Speed"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "ELSE"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Eco = 0"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Ven = 1.0"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "ELSE"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Stage1 = 1- PSZ_Office_SpeedRatio"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Stage2 = PSZ_Office_SpeedRatio"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Ven = 0"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Eco = 0"
-                },
-                {
-                    "program_line": "IF PSZ_Office_OAFlowMass > (PSZ_Office_OADesignMass * PSZ_Office_OASch)"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Stage1Speed = 1.0"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "SET PSZ_Office_FPR = PSZ_Office_Ven * (PSZ_Office_VenSpeed ^ PSZ_Office_FanPwrExponent)"
-                },
-                {
-                    "program_line": "SET PSZ_Office_FPR_0 = PSZ_Office_Eco * (PSZ_Office_EcoSpeed ^ PSZ_Office_FanPwrExponent)"
-                },
-                {
-                    "program_line": "SET PSZ_Office_FPR = PSZ_Office_FPR_0 + PSZ_Office_FPR"
-                },
-                {
-                    "program_line": "SET PSZ_Office_FPR_1 = PSZ_Office_Stage1 * (PSZ_Office_Stage1Speed ^ PSZ_Office_FanPwrExponent)"
-                },
-                {
-                    "program_line": "SET PSZ_Office_FPR = PSZ_Office_FPR + PSZ_Office_FPR_1"
-                },
-                {
-                    "program_line": "SET PSZ_Office_FPR_2 = PSZ_Office_Stage2 * (PSZ_Office_Stage2Speed ^ PSZ_Office_FanPwrExponent)"
-                },
-                {
-                    "program_line": "SET PSZ_Office_FPR = PSZ_Office_FPR + PSZ_Office_FPR_2"
-                },
-                {
-                    "program_line": "SET PSZ_Office_FPR_3 = PSZ_Office_Heating * (PSZ_Office_HeatSpeed ^ PSZ_Office_FanPwrExponent)"
-                },
-                {
-                    "program_line": "SET PSZ_Office_FanPwrRatio = PSZ_Office_FPR +  PSZ_Office_FPR_3"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Fan_Pressure = PSZ_Office_Fan_DesignPressure * PSZ_Office_FanPwrRatio"
-                }
-            ]
-        },
-        "PSZ_Office_Set_Fan_Par": {
-            "lines": [
-                {
-                    "program_line": "SET PSZ_OFFICE_Number_of_Stages =  1"
-                },
-                {
-                    "program_line": "IF PSZ_Office_Number_of_Stages == 1"
-                },
-                {
-                    "program_line": "Return"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "SET PSZ_Office_FanPwrExponent = 2.2"
-                },
-                {
-                    "program_line": "SET PSZ_Office_OAFrac = PSZ_Office_OAFlowMass/PSZ_Office_DesignFlowMass"
-                },
-                {
-                    "program_line": "IF  PSZ_Office_OAFrac < 0.66"
-                },
-                {
-                    "program_line": "SET PSZ_Office_VenSpeed = 0.66"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Stage1Speed = 0.66"
-                },
-                {
-                    "program_line": "ELSE"
-                },
-                {
-                    "program_line": "SET PSZ_Office_VenSpeed = PSZ_Office_OAFrac"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Stage1Speed = PSZ_Office_OAFrac"
-                },
-                {
-                    "program_line": "ENDIF"
-                },
-                {
-                    "program_line": "SET PSZ_Office_Stage2Speed = 1.0"
-                },
-                {
-                    "program_line": "SET PSZ_Office_HeatSpeed = 1.0"
-                }
-            ]
-        },
-        "PSZ_Office_Set_Number_of_Stages": {
-            "lines": [
-                {
-                    "program_line": "SET PSZ_OFFICE_Number_of_Stages =  1"
-                }
-            ]
-        },
         "SET_Zone1_Office_Light_EMS_Program": {
             "lines": [
                 {
                     "program_line": "SET Zone1_Office_LSr_IP=0.093*Zone1_Office_LSr/Zone1_Office_Area"
                 },
                 {
                     "program_line": "IF (Zone1_Office_Occ_Sensor <= 0) && (Zone1_Office_LSr_IP >= 0.02)"
@@ -2813,78 +1553,14 @@
                 {
                     "program_line": "ENDIF"
                 }
             ]
         }
     },
     "EnergyManagementSystem:ProgramCallingManager": {
-        "PSZ_Fine_ECO_Manager": {
-            "energyplus_model_calling_point": "InsideHVACSystemIterationLoop",
-            "programs": [
-                {
-                    "program_name": "PSZ_Fine_Economizer_CTRL_Prog"
-                }
-            ]
-        },
-        "PSZ_Fine_Fan_Main_Manager": {
-            "energyplus_model_calling_point": "BeginTimestepBeforePredictor",
-            "programs": [
-                {
-                    "program_name": "PSZ_Fine_Fan_Control"
-                }
-            ]
-        },
-        "PSZ_Fine_Fan_Parameter_manager": {
-            "energyplus_model_calling_point": "BeginNewEnvironment",
-            "programs": [
-                {
-                    "program_name": "PSZ_Fine_Set_Fan_Par"
-                }
-            ]
-        },
-        "PSZ_Fine_Set_Number_of_Stages_CallingManager": {
-            "energyplus_model_calling_point": "BeginNewEnvironment",
-            "programs": [
-                {
-                    "program_name": "PSZ_Fine_Set_Number_of_Stages"
-                }
-            ]
-        },
-        "PSZ_Office_ECO_Manager": {
-            "energyplus_model_calling_point": "InsideHVACSystemIterationLoop",
-            "programs": [
-                {
-                    "program_name": "PSZ_Office_Economizer_CTRL_Prog"
-                }
-            ]
-        },
-        "PSZ_Office_Fan_Main_Manager": {
-            "energyplus_model_calling_point": "BeginTimestepBeforePredictor",
-            "programs": [
-                {
-                    "program_name": "PSZ_Office_Fan_Control"
-                }
-            ]
-        },
-        "PSZ_Office_Fan_Parameter_manager": {
-            "energyplus_model_calling_point": "BeginNewEnvironment",
-            "programs": [
-                {
-                    "program_name": "PSZ_Office_Set_Fan_Par"
-                }
-            ]
-        },
-        "PSZ_Office_Set_Number_of_Stages_CallingManager": {
-            "energyplus_model_calling_point": "BeginNewEnvironment",
-            "programs": [
-                {
-                    "program_name": "PSZ_Office_Set_Number_of_Stages"
-                }
-            ]
-        },
         "SET_Zone1_Office_Light_EMS_Program_Prog_Manager": {
             "energyplus_model_calling_point": "BeginTimestepBeforePredictor",
             "programs": [
                 {
                     "program_name": "SET_Zone1_Office_Light_EMS_Program"
                 }
             ]
@@ -2906,82 +1582,14 @@
             ]
         }
     },
     "EnergyManagementSystem:Sensor": {
         "OAT_F": {
             "output_variable_or_output_meter_name": "Site Outdoor Air Drybulb Temperature"
         },
-        "OAwb_F": {
-            "output_variable_or_output_meter_index_key_name": "*",
-            "output_variable_or_output_meter_name": "Site Outdoor Air Wetbulb Temperature"
-        },
-        "PSZ_Fine_DAT_Rqd": {
-            "output_variable_or_output_meter_index_key_name": "PSZ-Fine Storage Air Loop Outlet",
-            "output_variable_or_output_meter_name": "System Node Setpoint Temperature"
-        },
-        "PSZ_Fine_Econo_Status": {
-            "output_variable_or_output_meter_index_key_name": "PSZ-Fine Storage",
-            "output_variable_or_output_meter_name": "Air System Outdoor Air Economizer Status"
-        },
-        "PSZ_Fine_HeatingRTF": {
-            "output_variable_or_output_meter_index_key_name": "PSZ-Fine Storage Heating Coil",
-            "output_variable_or_output_meter_name": "Heating Coil Runtime Fraction"
-        },
-        "PSZ_Fine_OAFlowMass": {
-            "output_variable_or_output_meter_index_key_name": "PSZ-Fine Storage Outside Air Inlet",
-            "output_variable_or_output_meter_name": "System Node Mass Flow Rate"
-        },
-        "PSZ_Fine_OASch": {
-            "output_variable_or_output_meter_index_key_name": "MinOA_MotorizedDamper_Sched",
-            "output_variable_or_output_meter_name": "Schedule Value"
-        },
-        "PSZ_Fine_RTF": {
-            "output_variable_or_output_meter_index_key_name": "PSZ-Fine Storage Cooling Coil",
-            "output_variable_or_output_meter_name": "Cooling Coil Runtime Fraction"
-        },
-        "PSZ_Fine_SpeedRatio": {
-            "output_variable_or_output_meter_index_key_name": "PSZ-Fine Storage_Unitary_Package_DX",
-            "output_variable_or_output_meter_name": "Coil System Compressor Speed Ratio"
-        },
-        "PSZ_Office_DAT_Rqd": {
-            "output_variable_or_output_meter_index_key_name": "PSZ-Office Air Loop Outlet",
-            "output_variable_or_output_meter_name": "System Node Setpoint Temperature"
-        },
-        "PSZ_Office_Econo_Status": {
-            "output_variable_or_output_meter_index_key_name": "PSZ-Office",
-            "output_variable_or_output_meter_name": "Air System Outdoor Air Economizer Status"
-        },
-        "PSZ_Office_HeatingRTF": {
-            "output_variable_or_output_meter_index_key_name": "PSZ-Office Heating Coil",
-            "output_variable_or_output_meter_name": "Heating Coil Runtime Fraction"
-        },
-        "PSZ_Office_OAFlowMass": {
-            "output_variable_or_output_meter_index_key_name": "PSZ-Office Outside Air Inlet",
-            "output_variable_or_output_meter_name": "System Node Mass Flow Rate"
-        },
-        "PSZ_Office_OASch": {
-            "output_variable_or_output_meter_index_key_name": "MinOA_MotorizedDamper_Sched",
-            "output_variable_or_output_meter_name": "Schedule Value"
-        },
-        "PSZ_Office_RTF": {
-            "output_variable_or_output_meter_index_key_name": "PSZ-Office Cooling Coil",
-            "output_variable_or_output_meter_name": "Cooling Coil Runtime Fraction"
-        },
-        "PSZ_Office_SpeedRatio": {
-            "output_variable_or_output_meter_index_key_name": "PSZ-Office_Unitary_Package_DX",
-            "output_variable_or_output_meter_name": "Coil System Compressor Speed Ratio"
-        },
-        "ZONE1_OFFICE_Temp": {
-            "output_variable_or_output_meter_index_key_name": "Zone1 Office Zone Air Node",
-            "output_variable_or_output_meter_name": "System Node Temperature"
-        },
-        "ZONE2_FINE_STORAGE_Temp": {
-            "output_variable_or_output_meter_index_key_name": "ZONE2 FINE STORAGE Zone Air Node",
-            "output_variable_or_output_meter_name": "System Node Temperature"
-        },
         "Zone1_Office_LSr": {
             "output_variable_or_output_meter_index_key_name": "Zone1 Office",
             "output_variable_or_output_meter_name": "Zone Lights Electricity Rate"
         },
         "Zone1_Office_Occ_Sensor": {
             "output_variable_or_output_meter_index_key_name": "Office People",
             "output_variable_or_output_meter_name": "People Occupant Count"
@@ -3012,48 +1620,74 @@
             "control_option": "AstronomicalClock",
             "design_level": 1004.9,
             "end_use_subcategory": "General",
             "schedule_name": "Exterior_lighting_schedule_c_2016"
         }
     },
     "Fan:ConstantVolume": {
-        "PSZ-Fine Storage Supply Fan": {
-            "air_inlet_node_name": "PSZ-Fine Storage Mixed Air Outlet",
-            "air_outlet_node_name": "PSZ-Fine Storage Supply Fan Outlet",
-            "availability_schedule_name": "FanSched",
-            "end_use_subcategory": "General",
-            "fan_total_efficiency": 0.56225,
-            "maximum_flow_rate": "Autosize",
-            "motor_efficiency": 0.865,
-            "motor_in_airstream_fraction": 1,
-            "pressure_rise": 622.5
-        },
-        "PSZ-Office Supply Fan": {
-            "air_inlet_node_name": "PSZ-Office Mixed Air Outlet",
-            "air_outlet_node_name": "PSZ-Office Supply Fan Outlet",
-            "availability_schedule_name": "FanSched",
-            "end_use_subcategory": "General",
-            "fan_total_efficiency": 0.55575,
-            "maximum_flow_rate": "Autosize",
-            "motor_efficiency": 0.855,
-            "motor_in_airstream_fraction": 1,
-            "pressure_rise": 622.5
-        },
         "Zone3UnitHeaterFan": {
             "air_inlet_node_name": "Zone3UnitHeaterAirInletNode",
             "air_outlet_node_name": "Zone3UnitHeaterFanOutletNode",
             "availability_schedule_name": "COMPACT HVAC-ALWAYS 1",
-            "end_use_subcategory": "Bulk Storage Fan",
+            "end_use_subcategory": "General",
             "fan_total_efficiency": 0.536,
             "maximum_flow_rate": "Autosize",
             "motor_efficiency": 0.825,
             "motor_in_airstream_fraction": 1.0,
             "pressure_rise": 49.8
         }
     },
+    "Fan:SystemModel": {
+        "PSZ-Fine Storage_addAQ Supply Fan": {
+            "air_inlet_node_name": "PSZ-Fine Storage Mixed Air Outlet",
+            "air_outlet_node_name": "PSZ-Fine Storage Supply Fan Outlet",
+            "availability_schedule_name": "FanSched",
+            "design_electric_power_consumption": "Autosize",
+            "design_maximum_air_flow_rate": "Autosize",
+            "design_power_sizing_method": "TotalEfficiencyAndPressure",
+            "design_pressure_rise": 622.5,
+            "electric_power_minimum_flow_rate_fraction": 1,
+            "end_use_subcategory": "General",
+            "fan_total_efficiency": 0.58175,
+            "motor_efficiency": 0.895,
+            "motor_in_air_stream_fraction": 1.0,
+            "night_ventilation_mode_pressure_rise": 622.5,
+            "number_of_speeds": 1,
+            "speed_control_method": "Discrete",
+            "speed_fractions": [
+                {
+                    "speed_electric_power_fraction": 1,
+                    "speed_flow_fraction": 1
+                }
+            ]
+        },
+        "PSZ-Office_addAQ Supply Fan": {
+            "air_inlet_node_name": "PSZ-Office Mixed Air Outlet",
+            "air_outlet_node_name": "PSZ-Office Supply Fan Outlet",
+            "availability_schedule_name": "FanSched",
+            "design_electric_power_consumption": "Autosize",
+            "design_maximum_air_flow_rate": "Autosize",
+            "design_power_sizing_method": "TotalEfficiencyAndPressure",
+            "design_pressure_rise": 622.5,
+            "electric_power_minimum_flow_rate_fraction": 1,
+            "end_use_subcategory": "General",
+            "fan_total_efficiency": 0.56225,
+            "motor_efficiency": 0.865,
+            "motor_in_air_stream_fraction": 1.0,
+            "night_ventilation_mode_pressure_rise": 622.5,
+            "number_of_speeds": 1,
+            "speed_control_method": "Discrete",
+            "speed_fractions": [
+                {
+                    "speed_electric_power_fraction": 1,
+                    "speed_flow_fraction": 1
+                }
+            ]
+        }
+    },
     "FenestrationSurface:Detailed": {
         "Bulk Storage Door1": {
             "building_surface_name": "Bulk Storage Right Wall",
             "construction_name": "Swinging Door_semi",
             "multiplier": 1,
             "number_of_vertices": 4,
             "surface_type": "Door",
@@ -3545,15 +2179,15 @@
             "vertex_4_x_coordinate": 45.7177703814647,
             "vertex_4_y_coordinate": 15.6964344976362,
             "vertex_4_z_coordinate": 2.13349595113502,
             "view_factor_to_ground": "Autocalculate"
         },
         "FineStorage_skylight_1": {
             "building_surface_name": "Fine Storage Roof",
-            "construction_name": "Window_U_0.50_SHGC_0.40",
+            "construction_name": "Skylight_U_0.5_SHGC_0.4",
             "frame_and_divider_name": "Skylight_Frame_Nonres",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 10.8204,
             "vertex_1_y_coordinate": 18.438914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 12.0396,
@@ -3564,15 +2198,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 10.8204,
             "vertex_4_y_coordinate": 19.658114,
             "vertex_4_z_coordinate": 8.533984
         },
         "FineStorage_skylight_10": {
             "building_surface_name": "Fine Storage Roof",
-            "construction_name": "Window_U_0.50_SHGC_0.40",
+            "construction_name": "Skylight_U_0.5_SHGC_0.4",
             "frame_and_divider_name": "Skylight_Frame_Nonres",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 39.3954,
             "vertex_1_y_coordinate": 18.438914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 40.6146,
@@ -3583,15 +2217,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 39.3954,
             "vertex_4_y_coordinate": 19.658114,
             "vertex_4_z_coordinate": 8.533984
         },
         "FineStorage_skylight_11": {
             "building_surface_name": "Fine Storage Roof",
-            "construction_name": "Window_U_0.50_SHGC_0.40",
+            "construction_name": "Skylight_U_0.5_SHGC_0.4",
             "frame_and_divider_name": "Skylight_Frame_Nonres",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 5.1054,
             "vertex_1_y_coordinate": 18.438914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 6.3246,
@@ -3602,15 +2236,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 5.1054,
             "vertex_4_y_coordinate": 19.658114,
             "vertex_4_z_coordinate": 8.533984
         },
         "FineStorage_skylight_12": {
             "building_surface_name": "Fine Storage Roof",
-            "construction_name": "Window_U_0.50_SHGC_0.40",
+            "construction_name": "Skylight_U_0.5_SHGC_0.4",
             "frame_and_divider_name": "Skylight_Frame_Nonres",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 5.1054,
             "vertex_1_y_coordinate": 26.058914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 6.3246,
@@ -3621,15 +2255,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 5.1054,
             "vertex_4_y_coordinate": 27.278114,
             "vertex_4_z_coordinate": 8.533984
         },
         "FineStorage_skylight_13": {
             "building_surface_name": "Fine Storage Roof",
-            "construction_name": "Window_U_0.50_SHGC_0.40",
+            "construction_name": "Skylight_U_0.5_SHGC_0.4",
             "frame_and_divider_name": "Skylight_Frame_Nonres",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 10.8204,
             "vertex_1_y_coordinate": 26.058914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 12.0396,
@@ -3640,15 +2274,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 10.8204,
             "vertex_4_y_coordinate": 27.278114,
             "vertex_4_z_coordinate": 8.533984
         },
         "FineStorage_skylight_14": {
             "building_surface_name": "Fine Storage Roof",
-            "construction_name": "Window_U_0.50_SHGC_0.40",
+            "construction_name": "Skylight_U_0.5_SHGC_0.4",
             "frame_and_divider_name": "Skylight_Frame_Nonres",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 16.5354,
             "vertex_1_y_coordinate": 26.058914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 17.7546,
@@ -3659,15 +2293,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 16.5354,
             "vertex_4_y_coordinate": 27.278114,
             "vertex_4_z_coordinate": 8.533984
         },
         "FineStorage_skylight_2": {
             "building_surface_name": "Fine Storage Roof",
-            "construction_name": "Window_U_0.50_SHGC_0.40",
+            "construction_name": "Skylight_U_0.5_SHGC_0.4",
             "frame_and_divider_name": "Skylight_Frame_Nonres",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 22.2504,
             "vertex_1_y_coordinate": 26.058914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 23.4696,
@@ -3678,15 +2312,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 22.2504,
             "vertex_4_y_coordinate": 27.278114,
             "vertex_4_z_coordinate": 8.533984
         },
         "FineStorage_skylight_3": {
             "building_surface_name": "Fine Storage Roof",
-            "construction_name": "Window_U_0.50_SHGC_0.40",
+            "construction_name": "Skylight_U_0.5_SHGC_0.4",
             "frame_and_divider_name": "Skylight_Frame_Nonres",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 27.9654,
             "vertex_1_y_coordinate": 26.058914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 29.1846,
@@ -3697,15 +2331,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 27.9654,
             "vertex_4_y_coordinate": 27.278114,
             "vertex_4_z_coordinate": 8.533984
         },
         "FineStorage_skylight_4": {
             "building_surface_name": "Fine Storage Roof",
-            "construction_name": "Window_U_0.50_SHGC_0.40",
+            "construction_name": "Skylight_U_0.5_SHGC_0.4",
             "frame_and_divider_name": "Skylight_Frame_Nonres",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 33.6804,
             "vertex_1_y_coordinate": 26.058914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 34.8996,
@@ -3716,15 +2350,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 33.6804,
             "vertex_4_y_coordinate": 27.278114,
             "vertex_4_z_coordinate": 8.533984
         },
         "FineStorage_skylight_5": {
             "building_surface_name": "Fine Storage Roof",
-            "construction_name": "Window_U_0.50_SHGC_0.40",
+            "construction_name": "Skylight_U_0.5_SHGC_0.4",
             "frame_and_divider_name": "Skylight_Frame_Nonres",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 39.3954,
             "vertex_1_y_coordinate": 26.058914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 40.6146,
@@ -3735,15 +2369,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 39.3954,
             "vertex_4_y_coordinate": 27.278114,
             "vertex_4_z_coordinate": 8.533984
         },
         "FineStorage_skylight_6": {
             "building_surface_name": "Fine Storage Roof",
-            "construction_name": "Window_U_0.50_SHGC_0.40",
+            "construction_name": "Skylight_U_0.5_SHGC_0.4",
             "frame_and_divider_name": "Skylight_Frame_Nonres",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 16.5354,
             "vertex_1_y_coordinate": 18.438914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 17.7546,
@@ -3754,15 +2388,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 16.5354,
             "vertex_4_y_coordinate": 19.658114,
             "vertex_4_z_coordinate": 8.533984
         },
         "FineStorage_skylight_7": {
             "building_surface_name": "Fine Storage Roof",
-            "construction_name": "Window_U_0.50_SHGC_0.40",
+            "construction_name": "Skylight_U_0.5_SHGC_0.4",
             "frame_and_divider_name": "Skylight_Frame_Nonres",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 22.2504,
             "vertex_1_y_coordinate": 18.438914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 23.4696,
@@ -3773,15 +2407,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 22.2504,
             "vertex_4_y_coordinate": 19.658114,
             "vertex_4_z_coordinate": 8.533984
         },
         "FineStorage_skylight_8": {
             "building_surface_name": "Fine Storage Roof",
-            "construction_name": "Window_U_0.50_SHGC_0.40",
+            "construction_name": "Skylight_U_0.5_SHGC_0.4",
             "frame_and_divider_name": "Skylight_Frame_Nonres",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 27.9654,
             "vertex_1_y_coordinate": 18.438914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 29.1846,
@@ -3792,15 +2426,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 27.9654,
             "vertex_4_y_coordinate": 19.658114,
             "vertex_4_z_coordinate": 8.533984
         },
         "FineStorage_skylight_9": {
             "building_surface_name": "Fine Storage Roof",
-            "construction_name": "Window_U_0.50_SHGC_0.40",
+            "construction_name": "Skylight_U_0.5_SHGC_0.4",
             "frame_and_divider_name": "Skylight_Frame_Nonres",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 33.6804,
             "vertex_1_y_coordinate": 18.438914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 34.8996,
@@ -3831,15 +2465,15 @@
             "vertex_4_x_coordinate": 12.953323682378,
             "vertex_4_y_coordinate": 0.0,
             "vertex_4_z_coordinate": 2.133495951135,
             "view_factor_to_ground": "Autocalculate"
         },
         "Office Front Wall Window 1": {
             "building_surface_name": "Office Front Wall",
-            "construction_name": "Window_U_0.45_SHGC_0.38",
+            "construction_name": "NonresWindow_U_0.36_SHGC_0.38",
             "multiplier": 1,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 3.65742163051717,
             "vertex_1_y_coordinate": 0,
             "vertex_1_z_coordinate": 2.43929602151392,
             "vertex_2_x_coordinate": 3.65742163051717,
@@ -3851,15 +2485,15 @@
             "vertex_4_x_coordinate": 7.31484326103434,
             "vertex_4_y_coordinate": 0,
             "vertex_4_z_coordinate": 2.43929602151392,
             "view_factor_to_ground": "Autocalculate"
         },
         "Office Front Wall Window2": {
             "building_surface_name": "Office Front Wall",
-            "construction_name": "Window_U_0.45_SHGC_0.38",
+            "construction_name": "NonresWindow_U_0.36_SHGC_0.38",
             "multiplier": 1,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 18.5918932884623,
             "vertex_1_y_coordinate": 0,
             "vertex_1_z_coordinate": 2.43929602151392,
             "vertex_2_x_coordinate": 18.5918932884623,
@@ -3891,15 +2525,15 @@
             "vertex_4_x_coordinate": 0,
             "vertex_4_y_coordinate": 4.11459933433182,
             "vertex_4_z_coordinate": 2.13349595113502,
             "view_factor_to_ground": "Autocalculate"
         },
         "Office Left Wall Window1": {
             "building_surface_name": "Office Left Wall",
-            "construction_name": "Window_U_0.45_SHGC_0.38",
+            "construction_name": "NonresWindow_U_0.36_SHGC_0.38",
             "multiplier": 1,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 0,
             "vertex_1_y_coordinate": 7.51904930207155,
             "vertex_1_z_coordinate": 2.43929602151392,
             "vertex_2_x_coordinate": 0,
@@ -3911,15 +2545,15 @@
             "vertex_4_x_coordinate": 0,
             "vertex_4_y_coordinate": 5.38555335093654,
             "vertex_4_z_coordinate": 2.43929602151392,
             "view_factor_to_ground": "Autocalculate"
         },
         "Office Left Wall Window2": {
             "building_surface_name": "Office Left Wall",
-            "construction_name": "Window_U_0.45_SHGC_0.38",
+            "construction_name": "NonresWindow_U_0.36_SHGC_0.38",
             "multiplier": 1,
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 0,
             "vertex_1_y_coordinate": 3.75800072535639,
             "vertex_1_z_coordinate": 2.43929602151392,
             "vertex_2_x_coordinate": 0,
@@ -3931,15 +2565,15 @@
             "vertex_4_x_coordinate": 0,
             "vertex_4_y_coordinate": 1.62450477422138,
             "vertex_4_z_coordinate": 2.43929602151392,
             "view_factor_to_ground": "Autocalculate"
         },
         "Skylight_r1c1": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 41.75537,
             "vertex_1_y_coordinate": 34.440914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 42.97457,
@@ -3950,15 +2584,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 41.75537,
             "vertex_4_y_coordinate": 35.660114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r1c2": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 41.75537,
             "vertex_1_y_coordinate": 43.076914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 42.97457,
@@ -3969,15 +2603,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 41.75537,
             "vertex_4_y_coordinate": 44.296114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r1c3": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 41.75537,
             "vertex_1_y_coordinate": 51.712914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 42.97457,
@@ -3988,15 +2622,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 41.75537,
             "vertex_4_y_coordinate": 52.932114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r1c4": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 41.75537,
             "vertex_1_y_coordinate": 60.348914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 42.97457,
@@ -4007,15 +2641,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 41.75537,
             "vertex_4_y_coordinate": 61.568114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r2c1": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 36.17753,
             "vertex_1_y_coordinate": 34.440914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 37.39673,
@@ -4026,15 +2660,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 36.17753,
             "vertex_4_y_coordinate": 35.660114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r2c2": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 36.17753,
             "vertex_1_y_coordinate": 43.076914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 37.39673,
@@ -4045,15 +2679,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 36.17753,
             "vertex_4_y_coordinate": 44.296114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r2c3": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 36.17753,
             "vertex_1_y_coordinate": 51.712914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 37.39673,
@@ -4064,15 +2698,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 36.17753,
             "vertex_4_y_coordinate": 52.932114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r2c4": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 36.17753,
             "vertex_1_y_coordinate": 60.348914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 37.39673,
@@ -4083,15 +2717,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 36.17753,
             "vertex_4_y_coordinate": 61.568114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r3c1": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 30.59969,
             "vertex_1_y_coordinate": 34.440914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 31.81889,
@@ -4102,15 +2736,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 30.59969,
             "vertex_4_y_coordinate": 35.660114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r3c2": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 30.59969,
             "vertex_1_y_coordinate": 43.076914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 31.81889,
@@ -4121,15 +2755,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 30.59969,
             "vertex_4_y_coordinate": 44.296114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r3c3": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 30.59969,
             "vertex_1_y_coordinate": 60.348914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 31.81889,
@@ -4140,15 +2774,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 30.59969,
             "vertex_4_y_coordinate": 61.568114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r3c4": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 30.59969,
             "vertex_1_y_coordinate": 51.712914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 31.81889,
@@ -4159,15 +2793,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 30.59969,
             "vertex_4_y_coordinate": 52.932114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r4c1": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 25.02185,
             "vertex_1_y_coordinate": 34.440914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 26.24105,
@@ -4178,15 +2812,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 25.02185,
             "vertex_4_y_coordinate": 35.660114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r4c2": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 25.02185,
             "vertex_1_y_coordinate": 43.076914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 26.24105,
@@ -4197,15 +2831,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 25.02185,
             "vertex_4_y_coordinate": 44.296114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r4c3": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 25.02185,
             "vertex_1_y_coordinate": 51.712914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 26.24105,
@@ -4216,15 +2850,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 25.02185,
             "vertex_4_y_coordinate": 52.932114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r4c4": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 25.02185,
             "vertex_1_y_coordinate": 60.348914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 26.24105,
@@ -4235,15 +2869,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 25.02185,
             "vertex_4_y_coordinate": 61.568114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r5c1": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 19.44401,
             "vertex_1_y_coordinate": 34.440914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 20.66321,
@@ -4254,15 +2888,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 19.44401,
             "vertex_4_y_coordinate": 35.660114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r5c2": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 19.44401,
             "vertex_1_y_coordinate": 43.076914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 20.66321,
@@ -4273,15 +2907,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 19.44401,
             "vertex_4_y_coordinate": 44.296114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r5c3": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 19.44401,
             "vertex_1_y_coordinate": 51.712914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 20.66321,
@@ -4292,15 +2926,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 19.44401,
             "vertex_4_y_coordinate": 52.932114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r5c4": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 19.44401,
             "vertex_1_y_coordinate": 60.348914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 20.66321,
@@ -4311,15 +2945,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 19.44401,
             "vertex_4_y_coordinate": 61.568114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r6c1": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 13.86617,
             "vertex_1_y_coordinate": 34.440914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 15.08537,
@@ -4330,15 +2964,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 13.86617,
             "vertex_4_y_coordinate": 35.660114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r6c2": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 13.86617,
             "vertex_1_y_coordinate": 43.076914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 15.08537,
@@ -4349,15 +2983,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 13.86617,
             "vertex_4_y_coordinate": 44.296114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r6c3": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 13.86617,
             "vertex_1_y_coordinate": 51.712914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 15.08537,
@@ -4368,15 +3002,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 13.86617,
             "vertex_4_y_coordinate": 52.932114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r6c4": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 13.86617,
             "vertex_1_y_coordinate": 60.348914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 15.08537,
@@ -4387,15 +3021,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 13.86617,
             "vertex_4_y_coordinate": 61.568114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r7c1": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 8.28833,
             "vertex_1_y_coordinate": 34.440914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 9.50753,
@@ -4406,15 +3040,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 8.28833,
             "vertex_4_y_coordinate": 35.660114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r7c2": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 8.28833,
             "vertex_1_y_coordinate": 43.076914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 9.50753,
@@ -4425,15 +3059,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 8.28833,
             "vertex_4_y_coordinate": 44.296114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r7c3": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 8.28833,
             "vertex_1_y_coordinate": 51.712914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 9.50753,
@@ -4444,15 +3078,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 8.28833,
             "vertex_4_y_coordinate": 52.932114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r7c4": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 8.28833,
             "vertex_1_y_coordinate": 60.348914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 9.50753,
@@ -4463,15 +3097,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 8.28833,
             "vertex_4_y_coordinate": 61.568114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r8c1": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 2.71049,
             "vertex_1_y_coordinate": 34.440914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 3.92969,
@@ -4482,15 +3116,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 2.71049,
             "vertex_4_y_coordinate": 35.660114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r8c2": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 2.71049,
             "vertex_1_y_coordinate": 43.076914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 3.92969,
@@ -4501,15 +3135,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 2.71049,
             "vertex_4_y_coordinate": 44.296114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r8c3": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 2.71049,
             "vertex_1_y_coordinate": 51.712914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 3.92969,
@@ -4520,15 +3154,15 @@
             "vertex_3_z_coordinate": 8.533984,
             "vertex_4_x_coordinate": 2.71049,
             "vertex_4_y_coordinate": 52.932114,
             "vertex_4_z_coordinate": 8.533984
         },
         "Skylight_r8c4": {
             "building_surface_name": "Bulk Storage Roof",
-            "construction_name": "Window_U_0.98_SHGC_0.68",
+            "construction_name": "SemiHtdSkylight_U_0.75_SHGC_0.55",
             "frame_and_divider_name": "Skylight_Frame_Semiheated",
             "number_of_vertices": 4,
             "surface_type": "Window",
             "vertex_1_x_coordinate": 2.71049,
             "vertex_1_y_coordinate": 60.348914,
             "vertex_1_z_coordinate": 8.533984,
             "vertex_2_x_coordinate": 3.92969,
@@ -4560,47 +3194,47 @@
             "surface_area": 6028.44715712782,
             "zone_or_zonelist_name": "Zone3 Bulk Storage"
         }
     },
     "Lights": {
         "Bulk Storage Area Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "GeneralLights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.42,
             "fraction_replaceable": 1,
             "fraction_visible": 0.18,
             "return_air_fraction": 0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_STORAGE_SCH",
-            "watts_per_zone_floor_area": 3.767368646,
-            "zone_or_zonelist_name": "Zone3 Bulk Storage"
+            "watts_per_zone_floor_area": 3.552090438,
+            "zone_or_zonelist_or_space_or_spacelist_name": "Zone3 Bulk Storage"
         },
         "Fine Storage Area Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "GeneralLights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.42,
             "fraction_replaceable": 1,
             "fraction_visible": 0.18,
             "return_air_fraction": 0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_STORAGE_SCH",
             "watts_per_zone_floor_area": 7.427098188,
-            "zone_or_zonelist_name": "Zone2 Fine Storage"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Zone2 Fine Storage"
         },
         "Office Lights": {
             "design_level_calculation_method": "Watts/Area",
-            "end_use_subcategory": "GeneralLights",
+            "end_use_subcategory": "LightsWired",
             "fraction_radiant": 0.37,
             "fraction_replaceable": 1,
             "fraction_visible": 0.18,
             "return_air_fraction": 0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_OFFICE_SCH",
-            "watts_per_zone_floor_area": 8.503489229,
-            "zone_or_zonelist_name": "Zone1 Office"
+            "watts_per_zone_floor_area": 6.888902667,
+            "zone_or_zonelist_or_space_or_spacelist_name": "Zone1 Office"
         }
     },
     "Material": {
         "100mm Normalweight concrete floor": {
             "conductivity": 2.31,
             "density": 2322,
             "roughness": "MediumRough",
@@ -4876,29 +3510,29 @@
             "thermal_resistance": 0.0299387330245182,
             "visible_absorptance": 0.7
         },
         "Semiheated_Exterior_Wall_Insulation": {
             "roughness": "MediumSmooth",
             "solar_absorptance": 0.7,
             "thermal_absorptance": 0.9,
-            "thermal_resistance": 1.32942862923026,
+            "thermal_resistance": 1.64444403979094,
             "visible_absorptance": 0.7
         },
         "Semiheated_Floor_Insulation": {
             "roughness": "MediumSmooth",
             "solar_absorptance": 0.7,
             "thermal_absorptance": 0.9,
             "thermal_resistance": 0.0299387330245182,
             "visible_absorptance": 0.7
         },
         "Semiheated_Roof_Insulation": {
             "roughness": "MediumSmooth",
             "solar_absorptance": 0.7,
             "thermal_absorptance": 0.9,
-            "thermal_resistance": 1.98442595005136,
+            "thermal_resistance": 2.0103016765077,
             "visible_absorptance": 0.7
         },
         "Std Opaque Door Panel": {
             "roughness": "MediumRough",
             "solar_absorptance": 0.7,
             "thermal_absorptance": 0.9,
             "thermal_resistance": 0.123456790123457,
@@ -4965,219 +3599,207 @@
     "Output:Constructions": {
         "Output:Constructions 1": {
             "details_type_1": "Constructions"
         }
     },
     "Output:Meter:MeterFileOnly": {
         "Output:Meter:MeterFileOnly 1": {
-            "key_name": "InteriorLights:Electricity",
+            "key_name": "Electricity:Facility",
             "reporting_frequency": "Hourly"
         },
         "Output:Meter:MeterFileOnly 2": {
-            "key_name": "InteriorEquipment:Electricity",
+            "key_name": "ElectricityNet:Facility",
+            "reporting_frequency": "Hourly"
+        },
+        "Output:Meter:MeterFileOnly 3": {
+            "key_name": "NaturalGas:Facility",
+            "reporting_frequency": "Hourly"
+        },
+        "Output:Meter:MeterFileOnly 4": {
+            "key_name": "Electricity:Facility",
+            "reporting_frequency": "Hourly"
+        },
+        "Output:Meter:MeterFileOnly 5": {
+            "key_name": "ElectricityNet:Facility",
+            "reporting_frequency": "Hourly"
+        },
+        "Output:Meter:MeterFileOnly 6": {
+            "key_name": "NaturalGas:Facility",
             "reporting_frequency": "Hourly"
         }
     },
     "Output:Surfaces:Drawing": {
         "Output:Surfaces:Drawing 1": {
             "report_specifications_1": "Triangulate3DFace",
             "report_type": "DXF"
         }
     },
     "Output:Table:Monthly": {
-        "Monthly Indoor Temp": {
-            "digits_after_decimal": 2,
+        "NameHolderMonthlySummary ClimateZone 5B": {
+            "digits_after_decimal": 3,
             "variable_details": [
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Zone Mean Air Temperature"
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Site Outdoor Air Drybulb Temperature"
+                    "variable_or_meter_name": "Heating:NaturalGas"
                 }
             ]
         },
-        "Peak Electrical Demand": {
+        "NameHolderMonthlySummary CodeAmendment NoneAmend": {
             "digits_after_decimal": 3,
             "variable_details": [
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "Electricity:Facility"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "Electricity:Facility"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "InteriorLights:Electricity"
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "InteriorEquipment:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Fans:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Heating:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Cooling:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "ExteriorLights:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Pumps:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "HeatRejection:Electricity"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "ExteriorEquipment:Electricity"
-                },
+                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
+                    "variable_or_meter_name": "Heating:NaturalGas"
+                }
+            ]
+        },
+        "NameHolderMonthlySummary CodeName ASHRAE901": {
+            "digits_after_decimal": 3,
+            "variable_details": [
                 {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Humidification:Electricity"
+                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "HeatRecovery:Electricity"
-                },
+                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
+                    "variable_or_meter_name": "Heating:NaturalGas"
+                }
+            ]
+        },
+        "NameHolderMonthlySummary CodeYear 2019": {
+            "digits_after_decimal": 3,
+            "variable_details": [
                 {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "WaterSystems:Electricity"
+                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Refrigeration:Electricity"
-                },
+                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
+                    "variable_or_meter_name": "Heating:NaturalGas"
+                }
+            ]
+        },
+        "NameHolderMonthlySummary PrototypeName Warehouse": {
+            "digits_after_decimal": 3,
+            "variable_details": [
                 {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Generators:Electricity"
+                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "ElectricityProduced:Facility"
+                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
+                    "variable_or_meter_name": "Heating:NaturalGas"
                 }
             ]
         },
-        "Peak Gas Demand": {
+        "NameHolderMonthlySummary RepresentCity USA_CO_Denver": {
             "digits_after_decimal": 3,
             "variable_details": [
                 {
                     "aggregation_type_for_variable_or_meter": "SumOrAverage",
-                    "variable_or_meter_name": "NaturalGas:Facility"
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
-                    "aggregation_type_for_variable_or_meter": "Maximum",
-                    "variable_or_meter_name": "NaturalGas:Facility"
-                },
-                {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "NaturalGas:HVAC"
-                },
+                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
+                    "variable_or_meter_name": "Heating:NaturalGas"
+                }
+            ]
+        },
+        "NameHolderMonthlySummary State National": {
+            "digits_after_decimal": 3,
+            "variable_details": [
                 {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "InteriorEquipment:NaturalGas"
+                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "MiscPlugGas:InteriorEquipment:NaturalGas"
-                },
+                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
+                    "variable_or_meter_name": "Heating:NaturalGas"
+                }
+            ]
+        },
+        "NameHolderMonthlySummary TaskPurpose ProgressIndicator": {
+            "digits_after_decimal": 3,
+            "variable_details": [
                 {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "NaturalGas:Plant"
+                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "WaterSystems:NaturalGas"
-                },
+                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
+                    "variable_or_meter_name": "Heating:NaturalGas"
+                }
+            ]
+        },
+        "NameHolderMonthlySummary TaskScope National": {
+            "digits_after_decimal": 3,
+            "variable_details": [
                 {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
-                    "variable_or_meter_name": "Water Heater:WaterSystems:NaturalGas"
+                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
+                    "variable_or_meter_name": "Site Outdoor Air Drybulb"
                 },
                 {
-                    "aggregation_type_for_variable_or_meter": "ValueWhenMaximumOrMinimum",
+                    "aggregation_type_for_variable_or_meter": "SumOrAverage",
                     "variable_or_meter_name": "Heating:NaturalGas"
                 }
             ]
         }
     },
     "Output:Table:SummaryReports": {
         "Output:Table:SummaryReports 1": {
             "reports": [
                 {
-                    "report_name": "EnvelopeSummary"
-                },
-                {
-                    "report_name": "InputVerificationandResultsSummary"
-                },
-                {
-                    "report_name": "AnnualBuildingUtilityPerformanceSummary"
-                },
-                {
-                    "report_name": "EquipmentSummary"
-                },
-                {
-                    "report_name": "AnnualBuildingUtilityPerformanceSummary"
-                },
-                {
-                    "report_name": "InputVerificationandResultsSummary"
-                },
-                {
-                    "report_name": "AllMonthly"
+                    "report_name": "AllSummaryAndMonthly"
                 }
             ]
         }
     },
     "Output:VariableDictionary": {
         "Output:VariableDictionary 1": {
             "key_field": "regular"
         }
     },
-    "OutputControl:Sizing:Style": {
-        "OutputControl:Sizing:Style 1": {
-            "column_separator": "Comma"
+    "OutputControl:ReportingTolerances": {
+        "OutputControl:ReportingTolerances 1": {
+            "tolerance_for_time_cooling_setpoint_not_met": 0.556,
+            "tolerance_for_time_heating_setpoint_not_met": 0.556
         }
     },
     "OutputControl:Table:Style": {
         "OutputControl:Table:Style 1": {
-            "column_separator": "CommaAndHTML",
-            "unit_conversion": "JtoMJ"
+            "column_separator": "CommaAndHTML"
         }
     },
     "People": {
         "Office People": {
             "activity_level_schedule_name": "Office Activity Schedule",
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people": 5,
             "number_of_people_calculation_method": "People",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "sensible_heat_fraction": "Autocalculate",
-            "zone_or_zonelist_name": "Zone1 Office"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Zone1 Office"
         }
     },
     "RunPeriod": {
         "Run Period 1": {
             "apply_weekend_holiday_rule": "Yes",
             "begin_day_of_month": 1,
             "begin_month": 1,
             "begin_year": 1991,
-            "day_of_week_for_start_day": "Tuesday",
+            "day_of_week_for_start_day": "Monday",
             "end_day_of_month": 31,
             "end_month": 12,
             "end_year": 1991,
             "use_weather_file_daylight_saving_period": "No",
             "use_weather_file_holidays_and_special_days": "No",
             "use_weather_file_rain_indicators": "Yes",
             "use_weather_file_snow_indicators": "Yes"
@@ -5253,15 +3875,15 @@
                 {
                     "field": "Until: 24:00"
                 },
                 {
                     "field": 0
                 }
             ],
-            "schedule_type_limits_name": "Any Number"
+            "schedule_type_limits_name": "On/Off"
         },
         "ALWAYS_ON": {
             "data": [
                 {
                     "field": "Through: 12/31"
                 },
                 {
@@ -5270,15 +3892,15 @@
                 {
                     "field": "Until: 24:00"
                 },
                 {
                     "field": 1
                 }
             ],
-            "schedule_type_limits_name": "Any Number"
+            "schedule_type_limits_name": "On/Off"
         },
         "Always Off Schedule": {
             "data": [
                 {
                     "field": "THROUGH: 12/31"
                 },
                 {
@@ -6329,20 +4951,16 @@
                     "field": 1
                 }
             ],
             "schedule_type_limits_name": "Control Type"
         }
     },
     "Schedule:Constant": {
-        "PSZ_Fine_Timestep_Econ_Eff_SCH": {
-            "hourly_value": 0.7,
-            "schedule_type_limits_name": "Fraction"
-        },
-        "PSZ_Office_Timestep_Econ_Eff_SCH": {
-            "hourly_value": 0.7,
+        "SZ_system_OA_Max_Frac_SCH": {
+            "hourly_value": 0.75,
             "schedule_type_limits_name": "Fraction"
         }
     },
     "Schedule:Day:Hourly": {
         "Bulk Storage INFIL_Adva WD": {
             "hour_1": 0.75,
             "hour_10": 1,
@@ -7696,95 +6314,106 @@
             "upper_limit_value": 1.0
         },
         "On-Off Schedule": {
             "lower_limit_value": 0,
             "numeric_type": "Discrete",
             "upper_limit_value": 1
         },
+        "On/Off": {
+            "lower_limit_value": 0,
+            "numeric_type": "Discrete",
+            "upper_limit_value": 1
+        },
         "Temperature": {
             "lower_limit_value": -60.0,
             "numeric_type": "Continuous",
             "upper_limit_value": 200
         }
     },
     "SetpointManager:MixedAir": {
-        "PSZ-Fine Storage HeatC Temp Manager": {
-            "control_variable": "Temperature",
-            "fan_inlet_node_name": "PSZ-Fine Storage Mixed Air Outlet",
-            "fan_outlet_node_name": "PSZ-Fine Storage Mixed Air Outlet",
-            "reference_setpoint_node_name": "PSZ-Fine Storage Air Loop Outlet",
-            "setpoint_node_or_nodelist_name": "PSZ-Fine Storage Heating Coil Outlet"
-        },
         "PSZ-Fine Storage OAMixed Air Temp Manager": {
             "control_variable": "Temperature",
             "fan_inlet_node_name": "PSZ-Fine Storage Mixed Air Outlet",
             "fan_outlet_node_name": "PSZ-Fine Storage Supply Fan Outlet",
             "reference_setpoint_node_name": "PSZ-Fine Storage Air Loop Outlet",
             "setpoint_node_or_nodelist_name": "PSZ-Fine Storage Mixed Air Outlet"
         },
-        "PSZ-Office HeatC Temp Manager": {
-            "control_variable": "Temperature",
-            "fan_inlet_node_name": "PSZ-Office Mixed Air Outlet",
-            "fan_outlet_node_name": "PSZ-Office Mixed Air Outlet",
-            "reference_setpoint_node_name": "PSZ-Office Air Loop Outlet",
-            "setpoint_node_or_nodelist_name": "PSZ-Office Heating Coil Outlet"
-        },
         "PSZ-Office OAMixed Air Temp Manager": {
             "control_variable": "Temperature",
             "fan_inlet_node_name": "PSZ-Office Mixed Air Outlet",
             "fan_outlet_node_name": "PSZ-Office Supply Fan Outlet",
             "reference_setpoint_node_name": "PSZ-Office Air Loop Outlet",
             "setpoint_node_or_nodelist_name": "PSZ-Office Mixed Air Outlet"
         }
     },
-    "SetpointManager:SingleZone:Reheat": {
-        "PSZ-Fine Storage Supply Air Temp Manager": {
+    "SetpointManager:SingleZone:Cooling": {
+        "PSZ-Fine Storage Supply Air Temp Manager - Clg": {
             "control_variable": "Temperature",
             "control_zone_name": "Zone2 Fine Storage",
             "maximum_supply_air_temperature": 43.3333344812747,
             "minimum_supply_air_temperature": 12.7777781162733,
             "setpoint_node_or_nodelist_name": "PSZ-Fine Storage Air Loop Outlet",
             "zone_inlet_node_name": "Zone2 Fine Storage Zone Equip Inlet",
             "zone_node_name": "Zone2 Fine Storage Zone Air Node"
         },
-        "PSZ-Office Supply Air Temp Manager": {
+        "PSZ-Office Supply Air Temp Manager - Clg": {
             "control_variable": "Temperature",
             "control_zone_name": "Zone1 Office",
             "maximum_supply_air_temperature": 43.3333344812747,
             "minimum_supply_air_temperature": 12.7777781162733,
             "setpoint_node_or_nodelist_name": "PSZ-Office Air Loop Outlet",
             "zone_inlet_node_name": "Zone1 Office Zone Equip Inlet",
             "zone_node_name": "Zone1 Office Zone Air Node"
         }
     },
+    "SetpointManager:SingleZone:Heating": {
+        "PSZ-Fine Storage Supply Air Temp Manager - Htg": {
+            "control_variable": "Temperature",
+            "control_zone_name": "Zone2 Fine Storage",
+            "maximum_supply_air_temperature": 43.3333344812747,
+            "minimum_supply_air_temperature": 12.7777781162733,
+            "setpoint_node_or_nodelist_name": "PSZ-Fine Storage Heating Coil Outlet",
+            "zone_inlet_node_name": "Zone2 Fine Storage Zone Equip Inlet",
+            "zone_node_name": "Zone2 Fine Storage Zone Air Node"
+        },
+        "PSZ-Office Supply Air Temp Manager - Htg": {
+            "control_variable": "Temperature",
+            "control_zone_name": "Zone1 Office",
+            "maximum_supply_air_temperature": 43.3333344812747,
+            "minimum_supply_air_temperature": 12.7777781162733,
+            "setpoint_node_or_nodelist_name": "PSZ-Office Heating Coil Outlet",
+            "zone_inlet_node_name": "Zone1 Office Zone Equip Inlet",
+            "zone_node_name": "Zone1 Office Zone Air Node"
+        }
+    },
     "SimulationControl": {
         "SimulationControl 1": {
             "do_hvac_sizing_simulation_for_sizing_periods": "No",
             "do_plant_sizing_calculation": "No",
             "do_system_sizing_calculation": "Yes",
             "do_zone_sizing_calculation": "Yes",
             "maximum_number_of_hvac_sizing_simulation_passes": 1,
             "run_simulation_for_sizing_periods": "Yes",
             "run_simulation_for_weather_file_run_periods": "Yes"
         }
     },
-    "Site:GroundTemperature:BuildingSurface": {
-        "Site:GroundTemperature:BuildingSurface 1": {
-            "april_ground_temperature": 12.65,
-            "august_ground_temperature": 21.22,
-            "december_ground_temperature": 12.75,
-            "february_ground_temperature": 12.62,
-            "january_ground_temperature": 12.68,
-            "july_ground_temperature": 21.76,
-            "june_ground_temperature": 20.37,
-            "march_ground_temperature": 12.65,
-            "may_ground_temperature": 13.46,
-            "november_ground_temperature": 12.94,
-            "october_ground_temperature": 13.56,
-            "september_ground_temperature": 18.64
+    "Site:GroundTemperature:FCfactorMethod": {
+        "Site:GroundTemperature:FCfactorMethod 1": {
+            "april_ground_temperature": 0.8,
+            "august_ground_temperature": 13.7,
+            "december_ground_temperature": 18.5,
+            "february_ground_temperature": 3.0,
+            "january_ground_temperature": 7.1,
+            "july_ground_temperature": 6.1,
+            "june_ground_temperature": 4.8,
+            "march_ground_temperature": -1.0,
+            "may_ground_temperature": -0.2,
+            "november_ground_temperature": 21.7,
+            "october_ground_temperature": 22.7,
+            "september_ground_temperature": 22.2
         }
     },
     "Site:Location": {
         "Denver-Aurora-Buckley.AFB_CO_USA WMO=724695": {
             "elevation": 1726.0,
             "latitude": 39.72,
             "longitude": -104.75,
@@ -7798,27 +6427,27 @@
             "maximum_difference_in_monthly_average_outdoor_air_temperatures": 23.7
         }
     },
     "Sizing:Parameters": {
         "Sizing:Parameters 1": {
             "cooling_sizing_factor": 1.2,
             "heating_sizing_factor": 1.2,
-            "timesteps_in_averaging_window": 4
+            "timesteps_in_averaging_window": 6
         }
     },
     "Sizing:System": {
         "Sizing:System 1": {
             "100_outdoor_air_in_cooling": "No",
             "100_outdoor_air_in_heating": "No",
             "airloop_name": "PSZ-Office",
             "central_cooling_capacity_control_method": "OnOff",
             "central_cooling_design_supply_air_humidity_ratio": 0.008,
             "central_cooling_design_supply_air_temperature": 12,
             "central_heating_design_supply_air_humidity_ratio": 0.008,
-            "central_heating_design_supply_air_temperature": 50,
+            "central_heating_design_supply_air_temperature": 40,
             "central_heating_maximum_system_air_flow_ratio": 1,
             "cooling_design_capacity": "Autosize",
             "cooling_design_capacity_method": "CoolingDesignCapacity",
             "cooling_supply_air_flow_rate": 0,
             "cooling_supply_air_flow_rate_method": "DesignDay",
             "design_outdoor_air_flow_rate": "Autosize",
             "heating_design_capacity": "Autosize",
@@ -7827,26 +6456,26 @@
             "heating_supply_air_flow_rate_method": "DesignDay",
             "precool_design_humidity_ratio": 0.008,
             "precool_design_temperature": 11.0,
             "preheat_design_humidity_ratio": 0.008,
             "preheat_design_temperature": 7,
             "system_outdoor_air_method": "ZoneSum",
             "type_of_load_to_size_on": "Sensible",
-            "type_of_zone_sum_to_use": "NonCoincident",
+            "type_of_zone_sum_to_use": "Coincident",
             "zone_maximum_outdoor_air_fraction": 1.0
         },
         "Sizing:System 2": {
             "100_outdoor_air_in_cooling": "No",
             "100_outdoor_air_in_heating": "No",
             "airloop_name": "PSZ-Fine Storage",
             "central_cooling_capacity_control_method": "OnOff",
             "central_cooling_design_supply_air_humidity_ratio": 0.008,
             "central_cooling_design_supply_air_temperature": 12,
             "central_heating_design_supply_air_humidity_ratio": 0.008,
-            "central_heating_design_supply_air_temperature": 50,
+            "central_heating_design_supply_air_temperature": 40,
             "central_heating_maximum_system_air_flow_ratio": 1,
             "cooling_design_capacity": "Autosize",
             "cooling_design_capacity_method": "CoolingDesignCapacity",
             "cooling_supply_air_flow_rate": 0,
             "cooling_supply_air_flow_rate_method": "DesignDay",
             "design_outdoor_air_flow_rate": "Autosize",
             "heating_design_capacity": "Autosize",
@@ -7855,15 +6484,15 @@
             "heating_supply_air_flow_rate_method": "DesignDay",
             "precool_design_humidity_ratio": 0.008,
             "precool_design_temperature": 11.0,
             "preheat_design_humidity_ratio": 0.008,
             "preheat_design_temperature": 7,
             "system_outdoor_air_method": "ZoneSum",
             "type_of_load_to_size_on": "Sensible",
-            "type_of_zone_sum_to_use": "NonCoincident",
+            "type_of_zone_sum_to_use": "Coincident",
             "zone_maximum_outdoor_air_fraction": 1.0
         }
     },
     "Sizing:Zone": {
         "Sizing:Zone 1": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
@@ -7875,19 +6504,17 @@
             "design_specification_outdoor_air_object_name": "SZ DSOA Zone1 Office",
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0,
             "heating_maximum_air_flow_fraction": 0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.008,
             "zone_cooling_design_supply_air_temperature": 14,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_cooling_sizing_factor": 0,
             "zone_heating_design_supply_air_humidity_ratio": 0.008,
             "zone_heating_design_supply_air_temperature": 50,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_heating_sizing_factor": 0,
             "zone_or_zonelist_name": "Zone1 Office"
         },
         "Sizing:Zone 2": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
             "cooling_design_air_flow_rate": 0,
             "cooling_minimum_air_flow_fraction": 0,
@@ -7897,19 +6524,17 @@
             "design_specification_outdoor_air_object_name": "SZ DSOA Zone2 Fine Storage",
             "heating_design_air_flow_method": "DesignDay",
             "heating_design_air_flow_rate": 0,
             "heating_maximum_air_flow_fraction": 0,
             "zone_cooling_design_supply_air_humidity_ratio": 0.008,
             "zone_cooling_design_supply_air_temperature": 14,
             "zone_cooling_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_cooling_sizing_factor": 0,
             "zone_heating_design_supply_air_humidity_ratio": 0.008,
             "zone_heating_design_supply_air_temperature": 50,
             "zone_heating_design_supply_air_temperature_input_method": "SupplyAirTemperature",
-            "zone_heating_sizing_factor": 0,
             "zone_or_zonelist_name": "Zone2 Fine Storage"
         },
         "Sizing:Zone 3": {
             "account_for_dedicated_outdoor_air_system": "No",
             "cooling_design_air_flow_method": "DesignDay",
             "cooling_minimum_air_flow_per_zone_floor_area": 0,
             "dedicated_outdoor_air_high_setpoint_temperature_for_design": "Autosize",
@@ -7993,17 +6618,51 @@
         }
     },
     "Timestep": {
         "Timestep 1": {
             "number_of_timesteps_per_hour": 4
         }
     },
+    "UnitarySystemPerformance:Multispeed": {
+        "PSZ-Fine_Unitary_Package_DX_Perf": {
+            "flow_ratios": [
+                {
+                    "cooling_speed_supply_air_flow_ratio": 1.0,
+                    "heating_speed_supply_air_flow_ratio": 1
+                },
+                {
+                    "cooling_speed_supply_air_flow_ratio": 1,
+                    "heating_speed_supply_air_flow_ratio": 1
+                }
+            ],
+            "no_load_supply_air_flow_rate_ratio": 1.0,
+            "number_of_speeds_for_cooling": 2,
+            "number_of_speeds_for_heating": 2,
+            "single_mode_operation": "No"
+        },
+        "PSZ-Office_Unitary_Package_DX_Perf": {
+            "flow_ratios": [
+                {
+                    "cooling_speed_supply_air_flow_ratio": 1.0,
+                    "heating_speed_supply_air_flow_ratio": 1
+                },
+                {
+                    "cooling_speed_supply_air_flow_ratio": 1,
+                    "heating_speed_supply_air_flow_ratio": 1
+                }
+            ],
+            "no_load_supply_air_flow_rate_ratio": 1.0,
+            "number_of_speeds_for_cooling": 2,
+            "number_of_speeds_for_heating": 2,
+            "single_mode_operation": "No"
+        }
+    },
     "Version": {
         "Version 1": {
-            "version_identifier": "9.5"
+            "version_identifier": "23.1"
         }
     },
     "WaterHeater:Mixed": {
         "Electric Tank": {
             "ambient_temperature_indicator": "Zone",
             "ambient_temperature_zone_name": "Zone1 Office",
             "deadband_temperature_difference": 2.00000005298191,
@@ -8022,825 +6681,64 @@
             "peak_use_flow_rate": 8.07469089073934e-06,
             "setpoint_temperature_schedule_name": "Hot Water Setpoint Temp Schedule",
             "tank_volume": 0.0757082515247699,
             "use_flow_rate_fraction_schedule_name": "Office DHW Schedule"
         }
     },
     "WindowMaterial:Gas": {
-        "AIR 13MM": {
-            "gas_type": "Air",
-            "thickness": 0.0127
-        },
         "AIR 3MM": {
             "gas_type": "Air",
             "thickness": 0.0032
-        },
-        "AIR 6MM": {
-            "gas_type": "Air",
-            "thickness": 0.0063
-        },
-        "ARGON 13MM": {
-            "gas_type": "Argon",
-            "thickness": 0.0127
-        },
-        "Gap_1_W_0_0018": {
-            "gas_type": "Air",
-            "thickness": 0.0018
-        },
-        "Gap_1_W_0_0024": {
-            "gas_type": "Air",
-            "thickness": 0.0024
-        },
-        "Gap_1_W_0_0025": {
-            "gas_type": "Air",
-            "thickness": 0.0025
-        },
-        "Gap_1_W_0_0032": {
-            "gas_type": "Air",
-            "thickness": 0.0032
-        },
-        "Gap_1_W_0_0038": {
-            "gas_type": "Air",
-            "thickness": 0.0038
-        },
-        "Gap_1_W_0_0042": {
-            "gas_type": "Air",
-            "thickness": 0.0042
-        },
-        "Gap_1_W_0_0043": {
-            "gas_type": "Air",
-            "thickness": 0.0043
-        },
-        "Gap_1_W_0_0046": {
-            "gas_type": "Air",
-            "thickness": 0.0046
-        },
-        "Gap_1_W_0_0048": {
-            "gas_type": "Air",
-            "thickness": 0.0048
-        },
-        "Gap_1_W_0_0052": {
-            "gas_type": "Air",
-            "thickness": 0.0052
-        },
-        "Gap_1_W_0_0060": {
-            "gas_type": "Air",
-            "thickness": 0.006
-        },
-        "Gap_1_W_0_0070": {
-            "gas_type": "Air",
-            "thickness": 0.007
-        },
-        "Gap_1_W_0_0090": {
-            "gas_type": "Air",
-            "thickness": 0.009
-        },
-        "Gap_1_W_0_0127": {
-            "gas_type": "Air",
-            "thickness": 0.0127
-        }
-    },
-    "WindowMaterial:GasMixture": {
-        "Gap_9_W_0_0127": {
-            "gas_1_fraction": 0.1,
-            "gas_1_type": "Air",
-            "gas_2_fraction": 0.9,
-            "gas_2_type": "Argon",
-            "number_of_gases_in_mixture": 2,
-            "thickness": 0.0127
         }
     },
     "WindowMaterial:Glazing": {
-        "BLUE 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.05,
-            "back_side_visible_reflectance_at_normal_incidence": 0.06,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.05,
-            "front_side_visible_reflectance_at_normal_incidence": 0.06,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.48,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.57
-        },
-        "BRONZE 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.054,
-            "back_side_visible_reflectance_at_normal_incidence": 0.057,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.054,
-            "front_side_visible_reflectance_at_normal_incidence": 0.057,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.482,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.534
-        },
         "CLEAR 2.5MM": {
             "back_side_infrared_hemispherical_emissivity": 0.84,
             "back_side_solar_reflectance_at_normal_incidence": 0.075,
             "back_side_visible_reflectance_at_normal_incidence": 0.081,
             "conductivity": 0.9,
             "front_side_infrared_hemispherical_emissivity": 0.84,
             "front_side_solar_reflectance_at_normal_incidence": 0.075,
             "front_side_visible_reflectance_at_normal_incidence": 0.081,
             "infrared_transmittance_at_normal_incidence": 0.0,
             "optical_data_type": "SpectralAverage",
             "solar_transmittance_at_normal_incidence": 0.8,
             "thickness": 0.0025,
             "visible_transmittance_at_normal_incidence": 0.901
         },
-        "CLEAR 3MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.075,
-            "back_side_visible_reflectance_at_normal_incidence": 0.081,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.075,
-            "front_side_visible_reflectance_at_normal_incidence": 0.081,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.837,
-            "thickness": 0.003,
-            "visible_transmittance_at_normal_incidence": 0.898
-        },
-        "CLEAR 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.071,
-            "back_side_visible_reflectance_at_normal_incidence": 0.08,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.071,
-            "front_side_visible_reflectance_at_normal_incidence": 0.08,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.775,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.881
-        },
-        "COATED POLY-55": {
-            "back_side_infrared_hemispherical_emissivity": 0.72,
-            "back_side_solar_reflectance_at_normal_incidence": 0.593,
-            "back_side_visible_reflectance_at_normal_incidence": 0.375,
-            "conductivity": 0.14,
-            "front_side_infrared_hemispherical_emissivity": 0.046,
-            "front_side_solar_reflectance_at_normal_incidence": 0.582,
-            "front_side_visible_reflectance_at_normal_incidence": 0.336,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.32,
-            "thickness": 0.00051,
-            "visible_transmittance_at_normal_incidence": 0.551
-        },
-        "COATED POLY-77": {
-            "back_side_infrared_hemispherical_emissivity": 0.72,
-            "back_side_solar_reflectance_at_normal_incidence": 0.398,
-            "back_side_visible_reflectance_at_normal_incidence": 0.167,
-            "conductivity": 0.14,
-            "front_side_infrared_hemispherical_emissivity": 0.075,
-            "front_side_solar_reflectance_at_normal_incidence": 0.402,
-            "front_side_visible_reflectance_at_normal_incidence": 0.147,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.504,
-            "thickness": 0.00051,
-            "visible_transmittance_at_normal_incidence": 0.766
-        },
-        "ECABS-2 BLEACHED 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.1,
-            "back_side_solar_reflectance_at_normal_incidence": 0.086,
-            "back_side_visible_reflectance_at_normal_incidence": 0.099,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.086,
-            "front_side_visible_reflectance_at_normal_incidence": 0.099,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.814,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.847
-        },
-        "ECABS-2 COLORED 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.1,
-            "back_side_solar_reflectance_at_normal_incidence": 0.179,
-            "back_side_visible_reflectance_at_normal_incidence": 0.081,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.179,
-            "front_side_visible_reflectance_at_normal_incidence": 0.081,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.111,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.128
-        },
-        "ECREF-1 COLORED 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.219,
-            "back_side_visible_reflectance_at_normal_incidence": 0.073,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.219,
-            "front_side_visible_reflectance_at_normal_incidence": 0.073,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.099,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.155
-        },
-        "ECREF-2 BLEACHED 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.1,
-            "back_side_solar_reflectance_at_normal_incidence": 0.168,
-            "back_side_visible_reflectance_at_normal_incidence": 0.11,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.168,
-            "front_side_visible_reflectance_at_normal_incidence": 0.11,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.694,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.818
-        },
-        "ECREF-2 COLORED 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.1,
-            "back_side_solar_reflectance_at_normal_incidence": 0.219,
-            "back_side_visible_reflectance_at_normal_incidence": 0.073,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.219,
-            "front_side_visible_reflectance_at_normal_incidence": 0.073,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.099,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.155
-        },
-        "GREEN 3MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.063,
-            "back_side_visible_reflectance_at_normal_incidence": 0.075,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.063,
-            "front_side_visible_reflectance_at_normal_incidence": 0.075,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.635,
-            "thickness": 0.003,
-            "visible_transmittance_at_normal_incidence": 0.822
-        },
-        "GREEN 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.056,
-            "back_side_visible_reflectance_at_normal_incidence": 0.07,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.056,
-            "front_side_visible_reflectance_at_normal_incidence": 0.07,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.487,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.749
-        },
-        "GREY 3MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.061,
-            "back_side_visible_reflectance_at_normal_incidence": 0.061,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.061,
-            "front_side_visible_reflectance_at_normal_incidence": 0.061,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.626,
-            "thickness": 0.003,
-            "visible_transmittance_at_normal_incidence": 0.611
-        },
-        "GREY 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.053,
-            "back_side_visible_reflectance_at_normal_incidence": 0.052,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.053,
-            "front_side_visible_reflectance_at_normal_incidence": 0.052,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.455,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.431
-        },
-        "Glass_102_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.07485449,
-            "back_side_visible_reflectance_at_normal_incidence": 0.082564,
-            "conductivity": 1.0,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.07476376,
-            "front_side_visible_reflectance_at_normal_incidence": 0.082563,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.833848,
-            "thickness": 0.003048,
-            "visible_transmittance_at_normal_incidence": 0.89926
-        },
-        "Glass_12116_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.538265,
-            "back_side_solar_reflectance_at_normal_incidence": 0.2199938,
-            "back_side_visible_reflectance_at_normal_incidence": 0.081654,
-            "conductivity": 1.000345,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.1094601,
-            "front_side_visible_reflectance_at_normal_incidence": 0.182598,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.171874,
-            "thickness": 0.00475,
-            "visible_transmittance_at_normal_incidence": 0.322771
-        },
-        "Glass_1576_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.868,
-            "back_side_solar_reflectance_at_normal_incidence": 0.1825558,
-            "back_side_visible_reflectance_at_normal_incidence": 0.128077,
-            "conductivity": 0.846,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.3034693,
-            "front_side_visible_reflectance_at_normal_incidence": 0.128888,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.167637,
-            "thickness": 0.003058,
-            "visible_transmittance_at_normal_incidence": 0.341994
-        },
-        "Glass_2010F_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.3410654,
-            "back_side_visible_reflectance_at_normal_incidence": 0.056031,
-            "conductivity": 1,
-            "front_side_infrared_hemispherical_emissivity": 0.042274,
-            "front_side_solar_reflectance_at_normal_incidence": 0.4183747,
-            "front_side_visible_reflectance_at_normal_incidence": 0.043577,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.434294,
-            "thickness": 0.00221,
-            "visible_transmittance_at_normal_incidence": 0.797579
-        },
-        "Glass_2022F_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.2656452,
-            "back_side_visible_reflectance_at_normal_incidence": 0.05547,
-            "conductivity": 1,
-            "front_side_infrared_hemispherical_emissivity": 0.046,
-            "front_side_solar_reflectance_at_normal_incidence": 0.3940945,
-            "front_side_visible_reflectance_at_normal_incidence": 0.042734,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.355897,
-            "thickness": 0.0039,
-            "visible_transmittance_at_normal_incidence": 0.677694
-        },
-        "Glass_2027F_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.340935,
-            "back_side_visible_reflectance_at_normal_incidence": 0.073741,
-            "conductivity": 1,
-            "front_side_infrared_hemispherical_emissivity": 0.03675,
-            "front_side_solar_reflectance_at_normal_incidence": 0.4700695,
-            "front_side_visible_reflectance_at_normal_incidence": 0.0546,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.369744,
-            "thickness": 0.004,
-            "visible_transmittance_at_normal_incidence": 0.765222
-        },
-        "Glass_2052_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.05449309,
-            "back_side_visible_reflectance_at_normal_incidence": 0.058397,
-            "conductivity": 1,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.05422805,
-            "front_side_visible_reflectance_at_normal_incidence": 0.05805,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.507767,
-            "thickness": 0.00837,
-            "visible_transmittance_at_normal_incidence": 0.586833
-        },
-        "Glass_2175_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.4379779,
-            "back_side_visible_reflectance_at_normal_incidence": 0.10654,
-            "conductivity": 1,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.2176064,
-            "front_side_visible_reflectance_at_normal_incidence": 0.078729,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.167758,
-            "thickness": 0.0086,
-            "visible_transmittance_at_normal_incidence": 0.416044
-        },
-        "Glass_2531_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.454,
-            "back_side_solar_reflectance_at_normal_incidence": 0.3617666,
-            "back_side_visible_reflectance_at_normal_incidence": 0.232929,
-            "conductivity": 0.934,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.3198325,
-            "front_side_visible_reflectance_at_normal_incidence": 0.25084,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.350556,
-            "thickness": 0.00306,
-            "visible_transmittance_at_normal_incidence": 0.490923
-        },
-        "Glass_2532_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.676,
-            "back_side_solar_reflectance_at_normal_incidence": 0.2732317,
-            "back_side_visible_reflectance_at_normal_incidence": 0.079448,
-            "conductivity": 0.933,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.2268281,
-            "front_side_visible_reflectance_at_normal_incidence": 0.0766,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.340824,
-            "thickness": 0.00306,
-            "visible_transmittance_at_normal_incidence": 0.543814
-        },
-        "Glass_282_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.37,
-            "back_side_solar_reflectance_at_normal_incidence": 0.4058073,
-            "back_side_visible_reflectance_at_normal_incidence": 0.270435,
-            "conductivity": 0.94,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.2956174,
-            "front_side_visible_reflectance_at_normal_incidence": 0.237458,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.352565,
-            "thickness": 0.003251,
-            "visible_transmittance_at_normal_incidence": 0.510046
-        },
-        "Glass_4313_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.298,
-            "back_side_solar_reflectance_at_normal_incidence": 0.09944001,
-            "back_side_visible_reflectance_at_normal_incidence": 0.096992,
-            "conductivity": 1.0,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.07114256,
-            "front_side_visible_reflectance_at_normal_incidence": 0.077225,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.373486,
-            "thickness": 0.00385,
-            "visible_transmittance_at_normal_incidence": 0.6013
-        },
-        "Glass_4321_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.279,
-            "back_side_solar_reflectance_at_normal_incidence": 0.09994167,
-            "back_side_visible_reflectance_at_normal_incidence": 0.094819,
-            "conductivity": 0.814,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.0742419,
-            "front_side_visible_reflectance_at_normal_incidence": 0.072726,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.425947,
-            "thickness": 0.00618,
-            "visible_transmittance_at_normal_incidence": 0.559652
-        },
-        "Glass_8652_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.39,
-            "back_side_solar_reflectance_at_normal_incidence": 0.4621051,
-            "back_side_visible_reflectance_at_normal_incidence": 0.306829,
-            "conductivity": 0.962,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.2989869,
-            "front_side_visible_reflectance_at_normal_incidence": 0.209449,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.343691,
-            "thickness": 0.003059,
-            "visible_transmittance_at_normal_incidence": 0.487937
-        },
-        "Glass_9731_LayerAvg": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.203399,
-            "back_side_visible_reflectance_at_normal_incidence": 0.070696,
-            "conductivity": 0.815,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.2079376,
-            "front_side_visible_reflectance_at_normal_incidence": 0.071115,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.369424,
-            "thickness": 0.01248,
-            "visible_transmittance_at_normal_incidence": 0.710088
-        },
-        "LoE CLEAR 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.1,
-            "back_side_solar_reflectance_at_normal_incidence": 0.22,
-            "back_side_visible_reflectance_at_normal_incidence": 0.078,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.17,
-            "front_side_visible_reflectance_at_normal_incidence": 0.055,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.6,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.84
-        },
-        "LoE SPEC SEL CLEAR 3MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.03,
-            "back_side_solar_reflectance_at_normal_incidence": 0.37,
-            "back_side_visible_reflectance_at_normal_incidence": 0.06,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.34,
-            "front_side_visible_reflectance_at_normal_incidence": 0.07,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.45,
-            "thickness": 0.003,
-            "visible_transmittance_at_normal_incidence": 0.78
-        },
-        "LoE SPEC SEL CLEAR 6MM Rev": {
-            "back_side_infrared_hemispherical_emissivity": 0.84,
-            "back_side_solar_reflectance_at_normal_incidence": 0.3,
-            "back_side_visible_reflectance_at_normal_incidence": 0.07,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.03,
-            "front_side_solar_reflectance_at_normal_incidence": 0.42,
-            "front_side_visible_reflectance_at_normal_incidence": 0.06,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.43,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.77
-        },
-        "LoE SPEC SEL TINT 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.03,
-            "back_side_solar_reflectance_at_normal_incidence": 0.41,
-            "back_side_visible_reflectance_at_normal_incidence": 0.04,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.14,
-            "front_side_visible_reflectance_at_normal_incidence": 0.06,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.26,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.46
-        },
-        "LoE TINT 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.1,
-            "back_side_solar_reflectance_at_normal_incidence": 0.2,
-            "back_side_visible_reflectance_at_normal_incidence": 0.054,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.093,
-            "front_side_visible_reflectance_at_normal_incidence": 0.035,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.36,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.5
-        },
-        "PYR A CLEAR 3MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.4,
-            "back_side_solar_reflectance_at_normal_incidence": 0.1,
-            "back_side_visible_reflectance_at_normal_incidence": 0.12,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.1,
-            "front_side_visible_reflectance_at_normal_incidence": 0.12,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.75,
-            "thickness": 0.003,
-            "visible_transmittance_at_normal_incidence": 0.85
-        },
-        "PYR B CLEAR 3MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.2,
-            "back_side_solar_reflectance_at_normal_incidence": 0.1,
-            "back_side_visible_reflectance_at_normal_incidence": 0.12,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.09,
-            "front_side_visible_reflectance_at_normal_incidence": 0.11,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.74,
-            "thickness": 0.003,
-            "visible_transmittance_at_normal_incidence": 0.82
-        },
-        "PYR B CLEAR 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.2,
-            "back_side_solar_reflectance_at_normal_incidence": 0.1,
-            "back_side_visible_reflectance_at_normal_incidence": 0.12,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.09,
-            "front_side_visible_reflectance_at_normal_incidence": 0.11,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.68,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.81
-        },
-        "REF A CLEAR LO 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.4,
-            "back_side_solar_reflectance_at_normal_incidence": 0.493,
-            "back_side_visible_reflectance_at_normal_incidence": 0.37,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.341,
-            "front_side_visible_reflectance_at_normal_incidence": 0.41,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.066,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.08
-        },
         "REF A CLEAR MID 6MM": {
             "back_side_infrared_hemispherical_emissivity": 0.47,
             "back_side_solar_reflectance_at_normal_incidence": 0.43,
             "back_side_visible_reflectance_at_normal_incidence": 0.35,
             "conductivity": 0.9,
             "front_side_infrared_hemispherical_emissivity": 0.84,
             "front_side_solar_reflectance_at_normal_incidence": 0.27,
             "front_side_visible_reflectance_at_normal_incidence": 0.31,
             "infrared_transmittance_at_normal_incidence": 0.0,
             "optical_data_type": "SpectralAverage",
             "solar_transmittance_at_normal_incidence": 0.11,
             "thickness": 0.006,
             "visible_transmittance_at_normal_incidence": 0.14
-        },
-        "REF A TINT MID 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.47,
-            "back_side_solar_reflectance_at_normal_incidence": 0.42,
-            "back_side_visible_reflectance_at_normal_incidence": 0.35,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.13,
-            "front_side_visible_reflectance_at_normal_incidence": 0.14,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.06,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.09
-        },
-        "REF B CLEAR HI 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.6,
-            "back_side_solar_reflectance_at_normal_incidence": 0.32,
-            "back_side_visible_reflectance_at_normal_incidence": 0.29,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.16,
-            "front_side_visible_reflectance_at_normal_incidence": 0.16,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.24,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.3
-        },
-        "REF B CLEAR LO 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.58,
-            "back_side_solar_reflectance_at_normal_incidence": 0.38,
-            "back_side_visible_reflectance_at_normal_incidence": 0.33,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.22,
-            "front_side_visible_reflectance_at_normal_incidence": 0.23,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.15,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.2
-        },
-        "REF B TINT HI 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.6,
-            "back_side_solar_reflectance_at_normal_incidence": 0.33,
-            "back_side_visible_reflectance_at_normal_incidence": 0.28,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.09,
-            "front_side_visible_reflectance_at_normal_incidence": 0.08,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.15,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.18
-        },
-        "REF B TINT MID 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.45,
-            "back_side_solar_reflectance_at_normal_incidence": 0.41,
-            "back_side_visible_reflectance_at_normal_incidence": 0.32,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.11,
-            "front_side_visible_reflectance_at_normal_incidence": 0.1,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.1,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.13
-        },
-        "REF C CLEAR HI 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.55,
-            "back_side_solar_reflectance_at_normal_incidence": 0.39,
-            "back_side_visible_reflectance_at_normal_incidence": 0.35,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.16,
-            "front_side_visible_reflectance_at_normal_incidence": 0.17,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.2,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.22
-        },
-        "REF C CLEAR MID 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.51,
-            "back_side_solar_reflectance_at_normal_incidence": 0.42,
-            "back_side_visible_reflectance_at_normal_incidence": 0.38,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.2,
-            "front_side_visible_reflectance_at_normal_incidence": 0.21,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.17,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.19
-        },
-        "REF D CLEAR 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.82,
-            "back_side_solar_reflectance_at_normal_incidence": 0.379,
-            "back_side_visible_reflectance_at_normal_incidence": 0.505,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.308,
-            "front_side_visible_reflectance_at_normal_incidence": 0.453,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.429,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.334
-        },
-        "REF D TINT 6MM": {
-            "back_side_infrared_hemispherical_emissivity": 0.82,
-            "back_side_solar_reflectance_at_normal_incidence": 0.36,
-            "back_side_visible_reflectance_at_normal_incidence": 0.45,
-            "conductivity": 0.9,
-            "front_side_infrared_hemispherical_emissivity": 0.84,
-            "front_side_solar_reflectance_at_normal_incidence": 0.14,
-            "front_side_visible_reflectance_at_normal_incidence": 0.18,
-            "infrared_transmittance_at_normal_incidence": 0.0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.3,
-            "thickness": 0.006,
-            "visible_transmittance_at_normal_incidence": 0.25
-        },
-        "Theoretical Glass 297": {
-            "back_side_infrared_hemispherical_emissivity": 0.9,
-            "back_side_solar_reflectance_at_normal_incidence": 0.574961,
-            "back_side_visible_reflectance_at_normal_incidence": 0.420302,
-            "conductivity": 0.0103561,
-            "front_side_infrared_hemispherical_emissivity": 0.9,
-            "front_side_solar_reflectance_at_normal_incidence": 0.574961,
-            "front_side_visible_reflectance_at_normal_incidence": 0.420302,
-            "infrared_transmittance_at_normal_incidence": 0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.375039,
-            "thickness": 0.003,
-            "visible_transmittance_at_normal_incidence": 0.529698
-        },
-        "Theoretical Glass 347": {
-            "back_side_infrared_hemispherical_emissivity": 0.9,
-            "back_side_solar_reflectance_at_normal_incidence": 0.634139,
-            "back_side_visible_reflectance_at_normal_incidence": 0.470089,
-            "conductivity": 0.010358,
-            "front_side_infrared_hemispherical_emissivity": 0.9,
-            "front_side_solar_reflectance_at_normal_incidence": 0.634139,
-            "front_side_visible_reflectance_at_normal_incidence": 0.470089,
-            "infrared_transmittance_at_normal_incidence": 0,
-            "optical_data_type": "SpectralAverage",
-            "solar_transmittance_at_normal_incidence": 0.315861,
-            "thickness": 0.003,
-            "visible_transmittance_at_normal_incidence": 0.479911
+        }
+    },
+    "WindowMaterial:SimpleGlazingSystem": {
+        "Nonres Skylight Glazing Layer": {
+            "solar_heat_gain_coefficient": 0.4,
+            "u_factor": 2.83913,
+            "visible_transmittance": 0.4
+        },
+        "Nonres Window Glazing Layer": {
+            "solar_heat_gain_coefficient": 0.38,
+            "u_factor": 2.0441736,
+            "visible_transmittance": 0.38
+        },
+        "Semiheated Skylight Glazing Layer": {
+            "solar_heat_gain_coefficient": 0.55,
+            "u_factor": 4.258695,
+            "visible_transmittance": 0.55
         }
     },
     "WindowProperty:FrameAndDivider": {
         "Skylight_Frame_Nonres": {
             "divider_thermal_hemispherical_emissivity": 0.9,
             "frame_conductance": 0,
             "frame_solar_absorptance": 0.7,
@@ -9050,45 +6948,45 @@
             "constant_term_coefficient": 0,
             "design_flow_rate": 2.330231241,
             "design_flow_rate_calculation_method": "Flow/Zone",
             "schedule_name": "Bulk Storage Infil_Base Schedule",
             "temperature_term_coefficient": 0,
             "velocity_squared_term_coefficient": 0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "Zone3 Bulk Storage"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Zone3 Bulk Storage"
         },
         "Fine Storage Infiltration": {
             "constant_term_coefficient": 0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.000225765,
+            "flow_rate_per_exterior_surface_area": 0.000225765,
             "schedule_name": "Fine Sorage Infil Schedule",
             "temperature_term_coefficient": 0,
             "velocity_squared_term_coefficient": 0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "Zone2 Fine Storage"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Zone2 Fine Storage"
         },
         "Office Door Infiltration": {
             "constant_term_coefficient": 1,
             "design_flow_rate": 0.176508178,
             "design_flow_rate_calculation_method": "Flow/Zone",
             "schedule_name": "INFIL_Door_Opening_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "Zone1 Office"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Zone1 Office"
         },
         "Office Infiltration": {
             "constant_term_coefficient": 0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.000220198,
+            "flow_rate_per_exterior_surface_area": 0.000220198,
             "schedule_name": "Office Infil Schedule",
             "temperature_term_coefficient": 0,
             "velocity_squared_term_coefficient": 0,
             "velocity_term_coefficient": 0.224,
-            "zone_or_zonelist_name": "Zone1 Office"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Zone1 Office"
         }
     },
     "ZoneVentilation:DesignFlowRate": {
         "Bulk Storage Ventilation-1": {
             "constant_term_coefficient": 1,
             "delta_temperature": -100,
             "design_flow_rate": 37.7600047937506,
@@ -9101,15 +6999,15 @@
             "minimum_indoor_temperature": 29.4444452244559,
             "minimum_outdoor_temperature": -100,
             "schedule_name": "Always On Schedule",
             "temperature_term_coefficient": 0,
             "velocity_squared_term_coefficient": 0,
             "velocity_term_coefficient": 0,
             "ventilation_type": "Exhaust",
-            "zone_or_zonelist_name": "Zone3 Bulk Storage"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Zone3 Bulk Storage"
         },
         "Bulk Storage Ventilation-2": {
             "constant_term_coefficient": 0,
             "delta_temperature": -100,
             "design_flow_rate": 0.943841435,
             "design_flow_rate_calculation_method": "Flow/Zone",
             "fan_total_efficiency": 1,
@@ -9119,11 +7017,11 @@
             "minimum_indoor_temperature": -73.3333352760033,
             "minimum_outdoor_temperature": -100,
             "schedule_name": "Always On Schedule",
             "temperature_term_coefficient": 0,
             "velocity_squared_term_coefficient": 0,
             "velocity_term_coefficient": 0.224,
             "ventilation_type": "Natural",
-            "zone_or_zonelist_name": "Zone3 Bulk Storage"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Zone3 Bulk Storage"
         }
     }
 }
```

### Comparing `sinergym-2.4.1/sinergym/data/buildings/OfficeGridStorageSmoothing.epJSON` & `sinergym-2.5.0/sinergym/data/buildings/LrgOff_GridStorageScheduled.epJSON`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958243943863412%*

 * *Differences: {"'AirLoopHVAC:OutdoorAirSystem'": "{'VAV_1_OA': {delete: ['availability_manager_list_name']}, "*

 * *                                   "'VAV_2_OA': {delete: ['availability_manager_list_name']}, "*

 * *                                   "'VAV_3_OA': {delete: ['availability_manager_list_name']}, "*

 * *                                   "'VAV_5_OA': {delete: ['availability_manager_list_name']}}",*

 * * "'ElectricEquipment'": "{'Basement_PlugMisc_Equip': "*

 * *                        "{'zone_or_zonelist_or_space_or_spacelist_name': […]*

```diff
@@ -81,30 +81,26 @@
         "VAV_5_OA_Controllers": {
             "controller_1_name": "VAV_5_OA_Controller",
             "controller_1_object_type": "Controller:OutdoorAir"
         }
     },
     "AirLoopHVAC:OutdoorAirSystem": {
         "VAV_1_OA": {
-            "availability_manager_list_name": "VAV_1 Availability Manager List",
             "controller_list_name": "VAV_1_OA_Controllers",
             "outdoor_air_equipment_list_name": "VAV_1_OA_Equipment"
         },
         "VAV_2_OA": {
-            "availability_manager_list_name": "VAV_2 Availability Manager List",
             "controller_list_name": "VAV_2_OA_Controllers",
             "outdoor_air_equipment_list_name": "VAV_2_OA_Equipment"
         },
         "VAV_3_OA": {
-            "availability_manager_list_name": "VAV_3 Availability Manager List",
             "controller_list_name": "VAV_3_OA_Controllers",
             "outdoor_air_equipment_list_name": "VAV_3_OA_Equipment"
         },
         "VAV_5_OA": {
-            "availability_manager_list_name": "VAV_5 Availability Manager List",
             "controller_list_name": "VAV_5_OA_Controllers",
             "outdoor_air_equipment_list_name": "VAV_5_OA_Equipment"
         }
     },
     "AirLoopHVAC:OutdoorAirSystem:EquipmentList": {
         "VAV_1_OA_Equipment": {
             "component_1_name": "VAV_1_OAMixing Box",
@@ -7116,165 +7112,165 @@
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Basement"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Basement"
         },
         "Core_bottom_PlugMisc_Equip": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Core_bottom"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_bottom"
         },
         "Core_mid_PlugMisc_Equip": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Core_mid"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_mid"
         },
         "Core_top_PlugMisc_Equip": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Core_top"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_top"
         },
         "Perimeter_bot_ZN_1_PlugMisc_Equip": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_1"
         },
         "Perimeter_bot_ZN_2_PlugMisc_Equip": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_2"
         },
         "Perimeter_bot_ZN_3_PlugMisc_Equip": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_3"
         },
         "Perimeter_bot_ZN_4_PlugMisc_Equip": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_4"
         },
         "Perimeter_mid_ZN_1_PlugMisc_Equip": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_1"
         },
         "Perimeter_mid_ZN_2_PlugMisc_Equip": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_2"
         },
         "Perimeter_mid_ZN_3_PlugMisc_Equip": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_3"
         },
         "Perimeter_mid_ZN_4_PlugMisc_Equip": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_4"
         },
         "Perimeter_top_ZN_1_PlugMisc_Equip": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_1"
         },
         "Perimeter_top_ZN_2_PlugMisc_Equip": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_2"
         },
         "Perimeter_top_ZN_3_PlugMisc_Equip": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_3"
         },
         "Perimeter_top_ZN_4_PlugMisc_Equip": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_4"
         }
     },
     "ElectricLoadCenter:Distribution": {
         "Grid Battery Load Center": {
             "design_storage_control_charge_power": 500000,
             "design_storage_control_discharge_power": 500000,
             "electrical_buss_type": "DirectCurrentWithInverterDCStorage",
@@ -7760,195 +7756,195 @@
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Basement"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Basement"
         },
         "Core_bottom_Lights": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Core_bottom"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_bottom"
         },
         "Core_mid_Lights": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Core_mid"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_mid"
         },
         "Core_top_Lights": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Core_top"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_top"
         },
         "Perimeter_bot_ZN_1_Lights": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_1"
         },
         "Perimeter_bot_ZN_2_Lights": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_2"
         },
         "Perimeter_bot_ZN_3_Lights": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_3"
         },
         "Perimeter_bot_ZN_4_Lights": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_4"
         },
         "Perimeter_mid_ZN_1_Lights": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_1"
         },
         "Perimeter_mid_ZN_2_Lights": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_2"
         },
         "Perimeter_mid_ZN_3_Lights": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_3"
         },
         "Perimeter_mid_ZN_4_Lights": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_4"
         },
         "Perimeter_top_ZN_1_Lights": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_1"
         },
         "Perimeter_top_ZN_2_Lights": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_2"
         },
         "Perimeter_top_ZN_3_Lights": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_3"
         },
         "Perimeter_top_ZN_4_Lights": {
             "design_level_calculation_method": "Watts/Area",
             "end_use_subcategory": "General",
             "fraction_radiant": 0.7,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "return_air_fraction": 0.0,
             "return_air_fraction_calculated_from_plenum_temperature": "No",
             "schedule_name": "BLDG_LIGHT_SCH",
             "watts_per_zone_floor_area": 10.76,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_4"
         }
     },
     "Material": {
         "1/2IN Gypsum": {
             "conductivity": 0.16,
             "density": 784.9,
             "roughness": "Smooth",
@@ -8827,263 +8823,263 @@
     "People": {
         "Basement People": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 37.16,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 37.16,
-            "zone_or_zonelist_name": "Basement"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Basement"
         },
         "Core_bottom People": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.58,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.58,
-            "zone_or_zonelist_name": "Core_bottom"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_bottom"
         },
         "Core_mid People": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.58,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.58,
-            "zone_or_zonelist_name": "Core_mid"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_mid"
         },
         "Core_top People": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.58,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.58,
-            "zone_or_zonelist_name": "Core_top"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Core_top"
         },
         "Perimeter_bot_ZN_1 People": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.58,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.58,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_1"
         },
         "Perimeter_bot_ZN_2 People": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.58,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.58,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_2"
         },
         "Perimeter_bot_ZN_3 People": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.58,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.58,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_3"
         },
         "Perimeter_bot_ZN_4 People": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.58,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.58,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_4"
         },
         "Perimeter_mid_ZN_1 People": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.58,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.58,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_1"
         },
         "Perimeter_mid_ZN_2 People": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.58,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.58,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_2"
         },
         "Perimeter_mid_ZN_3 People": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.58,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.58,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_3"
         },
         "Perimeter_mid_ZN_4 People": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.58,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.58,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_4"
         },
         "Perimeter_top_ZN_1 People": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.58,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.58,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_1"
         },
         "Perimeter_top_ZN_2 People": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.58,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.58,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_2"
         },
         "Perimeter_top_ZN_3 People": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.58,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.58,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_3"
         },
         "Perimeter_top_ZN_4 People": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "enable_ashrae_55_comfort_warnings": "No",
+            "floor_area_per_person": 18.58,
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people_calculation_method": "Area/Person",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "sensible_heat_fraction": "Autocalculate",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_floor_area_per_person": 18.58,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_4"
         }
     },
     "Pipe:Adiabatic": {
         "CoolSys1 Demand Bypass Pipe": {
             "inlet_node_name": "CoolSys1 Demand Bypass Pipe Inlet Node",
             "outlet_node_name": "CoolSys1 Demand Bypass Pipe Outlet Node"
         },
@@ -9193,32 +9189,32 @@
                 }
             ]
         }
     },
     "PlantEquipmentOperation:CoolingLoad": {
         "CoolSys1 Operation Scheme": {
             "load_range_1_lower_limit": 0.0,
-            "load_range_1_upper_limit": 100000000000000,
+            "load_range_1_upper_limit": 100000000000000.0,
             "range_1_equipment_list_name": "CoolSys1 Equipment List"
         },
         "TowerWaterSys Operation Scheme": {
             "load_range_1_lower_limit": 0.0,
-            "load_range_1_upper_limit": 1000000000000,
+            "load_range_1_upper_limit": 1000000000000.0,
             "range_1_equipment_list_name": "TowerWaterSys Equipment List"
         }
     },
     "PlantEquipmentOperation:HeatingLoad": {
         "HeatSys1 Operation Scheme": {
             "load_range_1_lower_limit": 0.0,
-            "load_range_1_upper_limit": 1000000000000000,
+            "load_range_1_upper_limit": 1000000000000000.0,
             "range_1_equipment_list_name": "HeatSys1 Equipment List"
         },
         "SWHSys1 Operation Scheme": {
             "load_range_1_lower_limit": 0.0,
-            "load_range_1_upper_limit": 1000000000000000,
+            "load_range_1_upper_limit": 1000000000000000.0,
             "range_1_equipment_list_name": "SWHSys1 Equipment List"
         }
     },
     "PlantEquipmentOperationSchemes": {
         "CoolSys1 Loop Operation Scheme List": {
             "control_scheme_1_name": "CoolSys1 Operation Scheme",
             "control_scheme_1_object_type": "PlantEquipmentOperation:CoolingLoad",
@@ -11913,15 +11909,15 @@
             "september_value": 9.2,
             "tariff_name": "IN_EIAMonthlyRateGas",
             "variable_type": "Currency"
         }
     },
     "Version": {
         "Version 1": {
-            "version_identifier": "9.5"
+            "version_identifier": "23.1"
         }
     },
     "WaterHeater:Mixed": {
         "SWHSys1 Water Heater": {
             "ambient_temperature_indicator": "Schedule",
             "ambient_temperature_schedule_name": "SWHSys1 Water Heater Ambient Temperature Schedule Name",
             "deadband_temperature_difference": 2.0,
@@ -12680,156 +12676,156 @@
             "load_distribution_scheme": "SequentialLoad"
         }
     },
     "ZoneInfiltration:DesignFlowRate": {
         "GroundFloor_Plenum_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.000302,
+            "flow_rate_per_exterior_surface_area": 0.000302,
             "schedule_name": "INFIL_QUARTER_ON_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "GroundFloor_Plenum"
+            "zone_or_zonelist_or_space_or_spacelist_name": "GroundFloor_Plenum"
         },
         "MidFloor_Plenum_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.000302,
+            "flow_rate_per_exterior_surface_area": 0.000302,
             "schedule_name": "INFIL_QUARTER_ON_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "MidFloor_Plenum"
+            "zone_or_zonelist_or_space_or_spacelist_name": "MidFloor_Plenum"
         },
         "Perimeter_bot_ZN_1_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.000302,
+            "flow_rate_per_exterior_surface_area": 0.000302,
             "schedule_name": "INFIL_QUARTER_ON_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_1"
         },
         "Perimeter_bot_ZN_2_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.000302,
+            "flow_rate_per_exterior_surface_area": 0.000302,
             "schedule_name": "INFIL_QUARTER_ON_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_2"
         },
         "Perimeter_bot_ZN_3_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.000302,
+            "flow_rate_per_exterior_surface_area": 0.000302,
             "schedule_name": "INFIL_QUARTER_ON_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_3"
         },
         "Perimeter_bot_ZN_4_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.000302,
+            "flow_rate_per_exterior_surface_area": 0.000302,
             "schedule_name": "INFIL_QUARTER_ON_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "Perimeter_bot_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_bot_ZN_4"
         },
         "Perimeter_mid_ZN_1_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.000302,
+            "flow_rate_per_exterior_surface_area": 0.000302,
             "schedule_name": "INFIL_QUARTER_ON_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_1"
         },
         "Perimeter_mid_ZN_2_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.000302,
+            "flow_rate_per_exterior_surface_area": 0.000302,
             "schedule_name": "INFIL_QUARTER_ON_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_2"
         },
         "Perimeter_mid_ZN_3_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.000302,
+            "flow_rate_per_exterior_surface_area": 0.000302,
             "schedule_name": "INFIL_QUARTER_ON_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_3"
         },
         "Perimeter_mid_ZN_4_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.000302,
+            "flow_rate_per_exterior_surface_area": 0.000302,
             "schedule_name": "INFIL_QUARTER_ON_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "Perimeter_mid_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_mid_ZN_4"
         },
         "Perimeter_top_ZN_1_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.000302,
+            "flow_rate_per_exterior_surface_area": 0.000302,
             "schedule_name": "INFIL_QUARTER_ON_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_1"
         },
         "Perimeter_top_ZN_2_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.000302,
+            "flow_rate_per_exterior_surface_area": 0.000302,
             "schedule_name": "INFIL_QUARTER_ON_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_2"
         },
         "Perimeter_top_ZN_3_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.000302,
+            "flow_rate_per_exterior_surface_area": 0.000302,
             "schedule_name": "INFIL_QUARTER_ON_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_3"
         },
         "Perimeter_top_ZN_4_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.000302,
+            "flow_rate_per_exterior_surface_area": 0.000302,
             "schedule_name": "INFIL_QUARTER_ON_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "Perimeter_top_ZN_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "Perimeter_top_ZN_4"
         },
         "TopFloor_Plenum_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate_calculation_method": "Flow/ExteriorArea",
-            "flow_per_exterior_surface_area": 0.000302,
+            "flow_rate_per_exterior_surface_area": 0.000302,
             "schedule_name": "INFIL_QUARTER_ON_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "TopFloor_Plenum"
+            "zone_or_zonelist_or_space_or_spacelist_name": "TopFloor_Plenum"
         }
     }
 }
```

### Comparing `sinergym-2.4.1/sinergym/data/buildings/ShopWithVandBattery.epJSON` & `sinergym-2.5.0/sinergym/data/buildings/ShopWithPVandBattery.epJSON`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954434822978847%*

 * *Differences: {"'AirLoopHVAC:OutdoorAirSystem'": "{'ZN_1_FLR_1_SEC_1:Sys_OA': {delete: "*

 * *                                   "['availability_manager_list_name']}, "*

 * *                                   "'ZN_1_FLR_1_SEC_2:Sys_OA': {delete: "*

 * *                                   "['availability_manager_list_name']}, "*

 * *                                   "'ZN_1_FLR_1_SEC_3:Sys_OA': {delete: "*

 * *                                   "['availability_manager_list_name']}, "*

 * *                                   "'ZN_1_FLR_1_SEC_4:Sys_OA': { […]*

```diff
@@ -66,35 +66,30 @@
         "ZN_1_FLR_1_SEC_5:Sys_OAControllers": {
             "controller_1_name": "ControllerZN_1_FLR_1_SEC_5:Sys_OA",
             "controller_1_object_type": "Controller:OutdoorAir"
         }
     },
     "AirLoopHVAC:OutdoorAirSystem": {
         "ZN_1_FLR_1_SEC_1:Sys_OA": {
-            "availability_manager_list_name": "ZN_1_FLR_1_SEC_1:Sys Availability Manager List",
             "controller_list_name": "ZN_1_FLR_1_SEC_1:Sys_OAControllers",
             "outdoor_air_equipment_list_name": "ZN_1_FLR_1_SEC_1:Sys_OAEquipment"
         },
         "ZN_1_FLR_1_SEC_2:Sys_OA": {
-            "availability_manager_list_name": "ZN_1_FLR_1_SEC_2:Sys Availability Manager List",
             "controller_list_name": "ZN_1_FLR_1_SEC_2:Sys_OAControllers",
             "outdoor_air_equipment_list_name": "ZN_1_FLR_1_SEC_2:Sys_OAEquipment"
         },
         "ZN_1_FLR_1_SEC_3:Sys_OA": {
-            "availability_manager_list_name": "ZN_1_FLR_1_SEC_3:Sys Availability Manager List",
             "controller_list_name": "ZN_1_FLR_1_SEC_3:Sys_OAControllers",
             "outdoor_air_equipment_list_name": "ZN_1_FLR_1_SEC_3:Sys_OAEquipment"
         },
         "ZN_1_FLR_1_SEC_4:Sys_OA": {
-            "availability_manager_list_name": "ZN_1_FLR_1_SEC_4:Sys Availability Manager List",
             "controller_list_name": "ZN_1_FLR_1_SEC_4:Sys_OAControllers",
             "outdoor_air_equipment_list_name": "ZN_1_FLR_1_SEC_4:Sys_OAEquipment"
         },
         "ZN_1_FLR_1_SEC_5:Sys_OA": {
-            "availability_manager_list_name": "ZN_1_FLR_1_SEC_5:Sys Availability Manager List",
             "controller_list_name": "ZN_1_FLR_1_SEC_5:Sys_OAControllers",
             "outdoor_air_equipment_list_name": "ZN_1_FLR_1_SEC_5:Sys_OAEquipment"
         }
     },
     "AirLoopHVAC:OutdoorAirSystem:EquipmentList": {
         "ZN_1_FLR_1_SEC_1:Sys_OAEquipment": {
             "component_1_name": "ZN_1_FLR_1_SEC_1:Sys_OAMixing Box",
@@ -1741,70 +1736,75 @@
             "view_factor_to_ground": 0.0,
             "wind_exposure": "NoWind",
             "zone_name": "ZN_1_FLR_1_SEC_5"
         }
     },
     "Coil:Cooling:DX:SingleSpeed": {
         "ZN_1_FLR_1_SEC_1:SysCoolC DXCoil": {
+            "2023_rated_evaporator_fan_power_per_volume_flow_rate": 934.4,
             "air_inlet_node_name": "ZN_1_FLR_1_SEC_1:Sys_OA-ZN_1_FLR_1_SEC_1:SysCoolCNode",
             "air_outlet_node_name": "ZN_1_FLR_1_SEC_1:SysCoolC-ZN_1_FLR_1_SEC_1:SysHeatCNode",
             "availability_schedule_name": "ALWAYS_ON",
             "energy_input_ratio_function_of_flow_fraction_curve_name": "ZN_1_FLR_1_SEC_1:SysCoolCCarrier48TM014_12tons_EIRFFF",
             "energy_input_ratio_function_of_temperature_curve_name": "ZN_1_FLR_1_SEC_1:SysCoolCCarrier48TM014_12tons_EIRFT",
             "gross_rated_cooling_cop": 2.7835,
             "gross_rated_sensible_heat_ratio": "Autosize",
             "gross_rated_total_cooling_capacity": "Autosize",
             "part_load_fraction_correlation_curve_name": "ZN_1_FLR_1_SEC_1:SysCoolCIEA_HVAC_BESTEST_9ton-PLR",
             "rated_air_flow_rate": "Autosize",
             "total_cooling_capacity_function_of_flow_fraction_curve_name": "ZN_1_FLR_1_SEC_1:SysCoolCCarrier48TM014_12tons_FFF",
             "total_cooling_capacity_function_of_temperature_curve_name": "ZN_1_FLR_1_SEC_1:SysCoolCCarrier48TM014_12tons_CapFT"
         },
         "ZN_1_FLR_1_SEC_2:SysCoolC DXCoil": {
+            "2023_rated_evaporator_fan_power_per_volume_flow_rate": 934.4,
             "air_inlet_node_name": "ZN_1_FLR_1_SEC_2:Sys_OA-ZN_1_FLR_1_SEC_2:SysCoolCNode",
             "air_outlet_node_name": "ZN_1_FLR_1_SEC_2:SysCoolC-ZN_1_FLR_1_SEC_2:SysHeatCNode",
             "availability_schedule_name": "ALWAYS_ON",
             "energy_input_ratio_function_of_flow_fraction_curve_name": "ZN_1_FLR_1_SEC_2:SysCoolCCarrier48TM014_12tons_EIRFFF",
             "energy_input_ratio_function_of_temperature_curve_name": "ZN_1_FLR_1_SEC_2:SysCoolCCarrier48TM014_12tons_EIRFT",
             "gross_rated_cooling_cop": 2.7835,
             "gross_rated_sensible_heat_ratio": "Autosize",
             "gross_rated_total_cooling_capacity": "Autosize",
             "part_load_fraction_correlation_curve_name": "ZN_1_FLR_1_SEC_2:SysCoolCIEA_HVAC_BESTEST_9ton-PLR",
             "rated_air_flow_rate": "Autosize",
             "total_cooling_capacity_function_of_flow_fraction_curve_name": "ZN_1_FLR_1_SEC_2:SysCoolCCarrier48TM014_12tons_FFF",
             "total_cooling_capacity_function_of_temperature_curve_name": "ZN_1_FLR_1_SEC_2:SysCoolCCarrier48TM014_12tons_CapFT"
         },
         "ZN_1_FLR_1_SEC_3:SysCoolC DXCoil": {
+            "2023_rated_evaporator_fan_power_per_volume_flow_rate": 934.4,
             "air_inlet_node_name": "ZN_1_FLR_1_SEC_3:Sys_OA-ZN_1_FLR_1_SEC_3:SysCoolCNode",
             "air_outlet_node_name": "ZN_1_FLR_1_SEC_3:SysCoolC-ZN_1_FLR_1_SEC_3:SysHeatCNode",
             "availability_schedule_name": "ALWAYS_ON",
             "energy_input_ratio_function_of_flow_fraction_curve_name": "ZN_1_FLR_1_SEC_3:SysCoolCCarrier48TM014_12tons_EIRFFF",
             "energy_input_ratio_function_of_temperature_curve_name": "ZN_1_FLR_1_SEC_3:SysCoolCCarrier48TM014_12tons_EIRFT",
             "gross_rated_cooling_cop": 2.7835,
             "gross_rated_sensible_heat_ratio": "Autosize",
             "gross_rated_total_cooling_capacity": "Autosize",
             "part_load_fraction_correlation_curve_name": "ZN_1_FLR_1_SEC_3:SysCoolCIEA_HVAC_BESTEST_9ton-PLR",
             "rated_air_flow_rate": "Autosize",
             "total_cooling_capacity_function_of_flow_fraction_curve_name": "ZN_1_FLR_1_SEC_3:SysCoolCCarrier48TM014_12tons_FFF",
             "total_cooling_capacity_function_of_temperature_curve_name": "ZN_1_FLR_1_SEC_3:SysCoolCCarrier48TM014_12tons_CapFT"
         },
         "ZN_1_FLR_1_SEC_4:SysCoolC DXCoil": {
+            "2023_rated_evaporator_fan_power_per_volume_flow_rate": 934.4,
             "air_inlet_node_name": "ZN_1_FLR_1_SEC_4:Sys_OA-ZN_1_FLR_1_SEC_4:SysCoolCNode",
             "air_outlet_node_name": "ZN_1_FLR_1_SEC_4:SysCoolC-ZN_1_FLR_1_SEC_4:SysHeatCNode",
             "availability_schedule_name": "ALWAYS_ON",
             "energy_input_ratio_function_of_flow_fraction_curve_name": "ZN_1_FLR_1_SEC_4:SysCoolCCarrier48TM014_12tons_EIRFFF",
             "energy_input_ratio_function_of_temperature_curve_name": "ZN_1_FLR_1_SEC_4:SysCoolCCarrier48TM014_12tons_EIRFT",
             "gross_rated_cooling_cop": 2.7835,
             "gross_rated_sensible_heat_ratio": "Autosize",
             "gross_rated_total_cooling_capacity": "Autosize",
             "part_load_fraction_correlation_curve_name": "ZN_1_FLR_1_SEC_4:SysCoolCIEA_HVAC_BESTEST_9ton-PLR",
             "rated_air_flow_rate": "Autosize",
             "total_cooling_capacity_function_of_flow_fraction_curve_name": "ZN_1_FLR_1_SEC_4:SysCoolCCarrier48TM014_12tons_FFF",
             "total_cooling_capacity_function_of_temperature_curve_name": "ZN_1_FLR_1_SEC_4:SysCoolCCarrier48TM014_12tons_CapFT"
         },
         "ZN_1_FLR_1_SEC_5:SysCoolC DXCoil": {
+            "2023_rated_evaporator_fan_power_per_volume_flow_rate": 934.4,
             "air_inlet_node_name": "ZN_1_FLR_1_SEC_5:Sys_OA-ZN_1_FLR_1_SEC_5:SysCoolCNode",
             "air_outlet_node_name": "ZN_1_FLR_1_SEC_5:SysCoolC-ZN_1_FLR_1_SEC_5:SysHeatCNode",
             "availability_schedule_name": "ALWAYS_ON",
             "energy_input_ratio_function_of_flow_fraction_curve_name": "ZN_1_FLR_1_SEC_5:SysCoolCCarrier48TM014_12tons_EIRFFF",
             "energy_input_ratio_function_of_temperature_curve_name": "ZN_1_FLR_1_SEC_5:SysCoolCCarrier48TM014_12tons_EIRFT",
             "gross_rated_cooling_cop": 2.7835,
             "gross_rated_sensible_heat_ratio": "Autosize",
@@ -2536,55 +2536,55 @@
             "design_level": 465.9534,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "GeneralEquipment",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_1"
         },
         "ZN_1_FLR_1_SEC_2_MiscPlug_Equip": {
             "design_level": 362.3476,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "GeneralEquipment",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_2"
         },
         "ZN_1_FLR_1_SEC_3_MiscPlug_Equip": {
             "design_level": 465.9534,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "GeneralEquipment",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_3"
         },
         "ZN_1_FLR_1_SEC_4_MiscPlug_Equip": {
             "design_level": 362.3476,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "GeneralEquipment",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_4"
         },
         "ZN_1_FLR_1_SEC_5_MiscPlug_Equip": {
             "design_level": 658.2385,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "GeneralEquipment",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.5,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_5"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_5"
         }
     },
     "ElectricLoadCenter:Distribution": {
         "PV Array Load Center": {
             "electrical_buss_type": "DirectCurrentWithInverterDCStorage",
             "electrical_storage_object_name": "Kibam",
             "generator_demand_limit_scheme_purchased_electric_demand_limit": 0,
@@ -2830,73 +2830,72 @@
             "nuclear_low_level_emission_factor": 0,
             "pb_emission_factor": 0,
             "pm10_emission_factor": 0.0171765,
             "pm2_5_emission_factor": 0.000138283,
             "pm_emission_factor": 0.0173147,
             "so2_emission_factor": 0.490888,
             "source_energy_factor": 3.712,
-            "units_of_measure": "kg",
             "water_emission_factor": 0.45499
         }
     },
     "GasEquipment": {
         "ZN_1_FLR_1_SEC_1_MiscGas_Equip": {
             "carbon_dioxide_generation_rate": 0,
             "design_level": 184.1006,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "GeneralEquipment",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.2,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_1"
         },
         "ZN_1_FLR_1_SEC_2_MiscGas_Equip": {
             "carbon_dioxide_generation_rate": 0,
             "design_level": 143.1654,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "GeneralEquipment",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.2,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_2"
         },
         "ZN_1_FLR_1_SEC_3_MiscGas_Equip": {
             "carbon_dioxide_generation_rate": 0,
             "design_level": 184.1006,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "GeneralEquipment",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.2,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_3"
         },
         "ZN_1_FLR_1_SEC_4_MiscGas_Equip": {
             "carbon_dioxide_generation_rate": 0,
             "design_level": 143.1654,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "GeneralEquipment",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.2,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_4"
         },
         "ZN_1_FLR_1_SEC_5_MiscGas_Equip": {
             "carbon_dioxide_generation_rate": 0,
             "design_level": 260.0734,
             "design_level_calculation_method": "EquipmentLevel",
             "end_use_subcategory": "GeneralEquipment",
             "fraction_latent": 0.0,
             "fraction_lost": 0.0,
             "fraction_radiant": 0.2,
             "schedule_name": "BLDG_EQUIP_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_5"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_5"
         }
     },
     "Generator:Photovoltaic": {
         "PV:ZN_1_FLR_1_SEC_1_Ceiling": {
             "heat_transfer_integration_mode": "Decoupled",
             "module_performance_name": "20percentEffPVhalfArea",
             "number_of_modules_in_series": 1.0,
@@ -2982,59 +2981,59 @@
             "end_use_subcategory": "General Lights",
             "fraction_radiant": 0.2,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "lighting_level": 1178.0879,
             "return_air_fraction": 0.0,
             "schedule_name": "BLDG_LIGHT_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_1"
         },
         "ZN_1_FLR_1_SEC_2_Lights": {
             "design_level_calculation_method": "LightingLevel",
             "end_use_subcategory": "General Lights",
             "fraction_radiant": 0.2,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "lighting_level": 916.1373,
             "return_air_fraction": 0.0,
             "schedule_name": "BLDG_LIGHT_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_2"
         },
         "ZN_1_FLR_1_SEC_3_Lights": {
             "design_level_calculation_method": "LightingLevel",
             "end_use_subcategory": "General Lights",
             "fraction_radiant": 0.2,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "lighting_level": 1178.0879,
             "return_air_fraction": 0.0,
             "schedule_name": "BLDG_LIGHT_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_3"
         },
         "ZN_1_FLR_1_SEC_4_Lights": {
             "design_level_calculation_method": "LightingLevel",
             "end_use_subcategory": "General Lights",
             "fraction_radiant": 0.2,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "lighting_level": 916.1373,
             "return_air_fraction": 0.0,
             "schedule_name": "BLDG_LIGHT_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_4"
         },
         "ZN_1_FLR_1_SEC_5_Lights": {
             "design_level_calculation_method": "LightingLevel",
             "end_use_subcategory": "General Lights",
             "fraction_radiant": 0.2,
             "fraction_replaceable": 1.0,
             "fraction_visible": 0.2,
             "lighting_level": 1664.2496,
             "return_air_fraction": 0.0,
             "schedule_name": "BLDG_LIGHT_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_5"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_5"
         }
     },
     "Material": {
         "1/2IN Gypsum": {
             "conductivity": 0.16,
             "density": 784.9,
             "roughness": "Smooth",
@@ -3744,75 +3743,75 @@
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people": 0.6039,
             "number_of_people_calculation_method": "People",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_1"
         },
         "ZN_1_FLR_1_SEC_2": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "carbon_dioxide_generation_rate": 3.82e-08,
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people": 0.4696,
             "number_of_people_calculation_method": "People",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_2"
         },
         "ZN_1_FLR_1_SEC_3": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "carbon_dioxide_generation_rate": 3.82e-08,
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people": 0.6039,
             "number_of_people_calculation_method": "People",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_3"
         },
         "ZN_1_FLR_1_SEC_4": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "carbon_dioxide_generation_rate": 3.82e-08,
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people": 0.4696,
             "number_of_people_calculation_method": "People",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_4"
         },
         "ZN_1_FLR_1_SEC_5": {
             "activity_level_schedule_name": "ACTIVITY_SCH",
             "air_velocity_schedule_name": "AIR_VELO_SCH",
             "carbon_dioxide_generation_rate": 3.82e-08,
             "clothing_insulation_calculation_method": "ClothingInsulationSchedule",
             "clothing_insulation_schedule_name": "CLOTHING_SCH",
             "fraction_radiant": 0.3,
             "mean_radiant_temperature_calculation_type": "ZoneAveraged",
             "number_of_people": 0.8531,
             "number_of_people_calculation_method": "People",
             "number_of_people_schedule_name": "BLDG_OCC_SCH",
             "thermal_comfort_model_1_type": "Fanger",
             "work_efficiency_schedule_name": "WORK_EFF_SCH",
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_5"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_5"
         }
     },
     "PhotovoltaicPerformance:Simple": {
         "20percentEffPVhalfArea": {
             "conversion_efficiency_input_mode": "Fixed",
             "fraction_of_surface_area_with_active_solar_cells": 0.5,
             "value_for_cell_efficiency_if_fixed": 0.2
@@ -3849,15 +3848,15 @@
                 }
             ]
         }
     },
     "PlantEquipmentOperation:HeatingLoad": {
         "SHWSys1 Operation Scheme": {
             "load_range_1_lower_limit": 0.0,
-            "load_range_1_upper_limit": 1000000000000000,
+            "load_range_1_upper_limit": 1000000000000000.0,
             "range_1_equipment_list_name": "SHWSys1 Equipment List"
         }
     },
     "PlantEquipmentOperationSchemes": {
         "SHWSys1 Loop Operation Scheme List": {
             "control_scheme_1_name": "SHWSys1 Operation Scheme",
             "control_scheme_1_object_type": "PlantEquipmentOperation:HeatingLoad",
@@ -5600,15 +5599,15 @@
             "september_value": 8.04,
             "tariff_name": "TX_EIAMonthlyRateGas",
             "variable_type": "Currency"
         }
     },
     "Version": {
         "Version 1": {
-            "version_identifier": "9.5"
+            "version_identifier": "23.1"
         }
     },
     "WaterHeater:Mixed": {
         "SHWSys1 Water Heater": {
             "ambient_temperature_indicator": "Schedule",
             "ambient_temperature_schedule_name": "SHWSys1 Water Heater Ambient Temperature Schedule",
             "deadband_temperature_difference": 2.0,
@@ -5810,63 +5809,63 @@
         }
     },
     "Zone": {
         "ZN_1_FLR_1_SEC_1": {
             "ceiling_height": 5.0088,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": 393.3855,
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "ZN_1_FLR_1_SEC_2": {
             "ceiling_height": 5.0088,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": 305.9154,
             "x_origin": 21.7558,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "ZN_1_FLR_1_SEC_3": {
             "ceiling_height": 5.0088,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": 393.3855,
             "x_origin": 4.57,
             "y_origin": 13.3645,
             "z_origin": 0.0
         },
         "ZN_1_FLR_1_SEC_4": {
             "ceiling_height": 5.0088,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": 305.9154,
             "x_origin": 0.0,
             "y_origin": 0.0,
             "z_origin": 0.0
         },
         "ZN_1_FLR_1_SEC_5": {
             "ceiling_height": 5.0088,
             "direction_of_relative_north": 0.0,
             "floor_area": "Autocalculate",
-            "multiplier": 1.0,
+            "multiplier": 1,
             "part_of_total_floor_area": "Yes",
             "type": 1,
             "volume": 555.724,
             "x_origin": 4.57,
             "y_origin": 4.57,
             "z_origin": 0.0
         }
@@ -6029,51 +6028,51 @@
             "constant_term_coefficient": 1.0,
             "design_flow_rate": 0.0542,
             "design_flow_rate_calculation_method": "Flow/Zone",
             "schedule_name": "INFIL_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_1"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_1"
         },
         "ZN_1_FLR_1_SEC_2_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate": 0.0435,
             "design_flow_rate_calculation_method": "Flow/Zone",
             "schedule_name": "INFIL_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_2"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_2"
         },
         "ZN_1_FLR_1_SEC_3_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate": 0.0542,
             "design_flow_rate_calculation_method": "Flow/Zone",
             "schedule_name": "INFIL_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_3"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_3"
         },
         "ZN_1_FLR_1_SEC_4_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate": 0.0435,
             "design_flow_rate_calculation_method": "Flow/Zone",
             "schedule_name": "INFIL_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_4"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_4"
         },
         "ZN_1_FLR_1_SEC_5_Infiltration": {
             "constant_term_coefficient": 1.0,
             "design_flow_rate": 0.0354,
             "design_flow_rate_calculation_method": "Flow/Zone",
             "schedule_name": "INFIL_SCH",
             "temperature_term_coefficient": 0.0,
             "velocity_squared_term_coefficient": 0.0,
             "velocity_term_coefficient": 0.0,
-            "zone_or_zonelist_name": "ZN_1_FLR_1_SEC_5"
+            "zone_or_zonelist_or_space_or_spacelist_name": "ZN_1_FLR_1_SEC_5"
         }
     }
 }
```

### Comparing `sinergym-2.4.1/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd` & `sinergym-2.5.0/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-Program Version,EnergyPlus, Version 9.5.0-de239b2e5f, YMD=2022.05.10 11:29,
+Program Version,EnergyPlus, Version 23.1.0-87ed9199d4, YMD=2023.05.31 13:47,
 Var Type (reported time step),Var Report Type,Variable Name [Units]
 Zone,Average,Site Outdoor Air Drybulb Temperature [C]
 Zone,Average,Site Outdoor Air Dewpoint Temperature [C]
 Zone,Average,Site Outdoor Air Wetbulb Temperature [C]
 Zone,Average,Site Outdoor Air Humidity Ratio [kgWater/kgDryAir]
 Zone,Average,Site Outdoor Air Relative Humidity [%]
 Zone,Average,Site Outdoor Air Barometric Pressure [Pa]
 Zone,Average,Site Wind Speed [m/s]
 Zone,Average,Site Wind Direction [deg]
 Zone,Average,Site Sky Temperature [C]
 Zone,Average,Site Horizontal Infrared Radiation Rate per Area [W/m2]
 Zone,Average,Site Diffuse Solar Radiation Rate per Area [W/m2]
 Zone,Average,Site Direct Solar Radiation Rate per Area [W/m2]
+Zone,Sum,Liquid Precipitation Depth [m]
+Zone,Average,Site Precipitation Rate [m/s]
 Zone,Sum,Site Precipitation Depth [m]
 Zone,Average,Site Ground Reflected Solar Radiation Rate per Area [W/m2]
 Zone,Average,Site Ground Temperature [C]
 Zone,Average,Site Surface Ground Temperature [C]
 Zone,Average,Site Deep Ground Temperature [C]
 Zone,Average,Site Simple Factor Model Ground Temperature [C]
 Zone,Average,Site Total Sky Cover []
@@ -47,14 +49,24 @@
 Zone,Average,Zone Total Internal Visible Radiation Heating Rate [W]
 Zone,Sum,Zone Total Internal Convective Heating Energy [J]
 Zone,Average,Zone Total Internal Convective Heating Rate [W]
 Zone,Sum,Zone Total Internal Latent Gain Energy [J]
 Zone,Average,Zone Total Internal Latent Gain Rate [W]
 Zone,Sum,Zone Total Internal Total Heating Energy [J]
 Zone,Average,Zone Total Internal Total Heating Rate [W]
+Zone,Sum,Space Total Internal Radiant Heating Energy [J]
+Zone,Average,Space Total Internal Radiant Heating Rate [W]
+Zone,Sum,Space Total Internal Visible Radiation Heating Energy [J]
+Zone,Average,Space Total Internal Visible Radiation Heating Rate [W]
+Zone,Sum,Space Total Internal Convective Heating Energy [J]
+Zone,Average,Space Total Internal Convective Heating Rate [W]
+Zone,Sum,Space Total Internal Latent Gain Energy [J]
+Zone,Average,Space Total Internal Latent Gain Rate [W]
+Zone,Sum,Space Total Internal Total Heating Energy [J]
+Zone,Average,Space Total Internal Total Heating Rate [W]
 Zone,Average,People Occupant Count []
 Zone,Sum,People Radiant Heating Energy [J]
 Zone,Average,People Radiant Heating Rate [W]
 Zone,Sum,People Convective Heating Energy [J]
 Zone,Average,People Convective Heating Rate [W]
 Zone,Sum,People Sensible Heating Energy [J]
 Zone,Average,People Sensible Heating Rate [W]
@@ -71,14 +83,25 @@
 Zone,Average,Zone People Convective Heating Rate [W]
 Zone,Sum,Zone People Sensible Heating Energy [J]
 Zone,Average,Zone People Sensible Heating Rate [W]
 Zone,Sum,Zone People Latent Gain Energy [J]
 Zone,Average,Zone People Latent Gain Rate [W]
 Zone,Sum,Zone People Total Heating Energy [J]
 Zone,Average,Zone People Total Heating Rate [W]
+Zone,Average,Space People Occupant Count []
+Zone,Sum,Space People Radiant Heating Energy [J]
+Zone,Average,Space People Radiant Heating Rate [W]
+Zone,Sum,Space People Convective Heating Energy [J]
+Zone,Average,Space People Convective Heating Rate [W]
+Zone,Sum,Space People Sensible Heating Energy [J]
+Zone,Average,Space People Sensible Heating Rate [W]
+Zone,Sum,Space People Latent Gain Energy [J]
+Zone,Average,Space People Latent Gain Rate [W]
+Zone,Sum,Space People Total Heating Energy [J]
+Zone,Average,Space People Total Heating Rate [W]
 Zone,Average,Lights Electricity Rate [W]
 Zone,Sum,Lights Radiant Heating Energy [J]
 Zone,Average,Lights Radiant Heating Rate [W]
 Zone,Sum,Lights Visible Radiation Heating Energy [J]
 Zone,Average,Lights Visible Radiation Heating Rate [W]
 Zone,Sum,Lights Convective Heating Energy [J]
 Zone,Average,Lights Convective Heating Rate [W]
@@ -95,14 +118,26 @@
 Zone,Average,Zone Lights Visible Radiation Heating Rate [W]
 Zone,Sum,Zone Lights Convective Heating Energy [J]
 Zone,Average,Zone Lights Convective Heating Rate [W]
 Zone,Sum,Zone Lights Return Air Heating Energy [J]
 Zone,Average,Zone Lights Return Air Heating Rate [W]
 Zone,Sum,Zone Lights Total Heating Energy [J]
 Zone,Average,Zone Lights Total Heating Rate [W]
+Zone,Average,Space Lights Electricity Rate [W]
+Zone,Sum,Space Lights Electricity Energy [J]
+Zone,Sum,Space Lights Radiant Heating Energy [J]
+Zone,Average,Space Lights Radiant Heating Rate [W]
+Zone,Sum,Space Lights Visible Radiation Heating Energy [J]
+Zone,Average,Space Lights Visible Radiation Heating Rate [W]
+Zone,Sum,Space Lights Convective Heating Energy [J]
+Zone,Average,Space Lights Convective Heating Rate [W]
+Zone,Sum,Space Lights Return Air Heating Energy [J]
+Zone,Average,Space Lights Return Air Heating Rate [W]
+Zone,Sum,Space Lights Total Heating Energy [J]
+Zone,Average,Space Lights Total Heating Rate [W]
 Zone,Average,Electric Equipment Electricity Rate [W]
 Zone,Sum,Electric Equipment Electricity Energy [J]
 Zone,Sum,Electric Equipment Radiant Heating Energy [J]
 Zone,Average,Electric Equipment Radiant Heating Rate [W]
 Zone,Sum,Electric Equipment Convective Heating Energy [J]
 Zone,Average,Electric Equipment Convective Heating Rate [W]
 Zone,Sum,Electric Equipment Latent Gain Energy [J]
@@ -119,14 +154,26 @@
 Zone,Average,Zone Electric Equipment Convective Heating Rate [W]
 Zone,Sum,Zone Electric Equipment Latent Gain Energy [J]
 Zone,Average,Zone Electric Equipment Latent Gain Rate [W]
 Zone,Sum,Zone Electric Equipment Lost Heat Energy [J]
 Zone,Average,Zone Electric Equipment Lost Heat Rate [W]
 Zone,Sum,Zone Electric Equipment Total Heating Energy [J]
 Zone,Average,Zone Electric Equipment Total Heating Rate [W]
+Zone,Average,Space Electric Equipment Electricity Rate [W]
+Zone,Sum,Space Electric Equipment Electricity Energy [J]
+Zone,Sum,Space Electric Equipment Radiant Heating Energy [J]
+Zone,Average,Space Electric Equipment Radiant Heating Rate [W]
+Zone,Sum,Space Electric Equipment Convective Heating Energy [J]
+Zone,Average,Space Electric Equipment Convective Heating Rate [W]
+Zone,Sum,Space Electric Equipment Latent Gain Energy [J]
+Zone,Average,Space Electric Equipment Latent Gain Rate [W]
+Zone,Sum,Space Electric Equipment Lost Heat Energy [J]
+Zone,Average,Space Electric Equipment Lost Heat Rate [W]
+Zone,Sum,Space Electric Equipment Total Heating Energy [J]
+Zone,Average,Space Electric Equipment Total Heating Rate [W]
 Zone,Average,ITE CPU Electricity Rate [W]
 Zone,Average,ITE Fan Electricity Rate [W]
 Zone,Average,ITE UPS Electricity Rate [W]
 Zone,Average,ITE CPU Electricity Rate at Design Inlet Conditions [W]
 Zone,Average,ITE Fan Electricity Rate at Design Inlet Conditions [W]
 Zone,Average,ITE UPS Heat Gain to Zone Rate [W]
 Zone,Average,ITE Total Heat Gain to Zone Rate [W]
@@ -179,27 +226,52 @@
 Zone,Sum,Zone ITE Any Air Inlet Operating Range Exceeded Time [hr]
 Zone,Sum,Zone ITE Any Air Inlet Dry-Bulb Temperature Above Operating Range Time [hr]
 Zone,Sum,Zone ITE Any Air Inlet Dry-Bulb Temperature Below Operating Range Time [hr]
 Zone,Sum,Zone ITE Any Air Inlet Dewpoint Temperature Above Operating Range Time [hr]
 Zone,Sum,Zone ITE Any Air Inlet Dewpoint Temperature Below Operating Range Time [hr]
 Zone,Sum,Zone ITE Any Air Inlet Relative Humidity Above Operating Range Time [hr]
 Zone,Sum,Zone ITE Any Air Inlet Relative Humidity Below Operating Range Time [hr]
+Zone,Average,Space ITE CPU Electricity Rate [W]
+Zone,Average,Space ITE Fan Electricity Rate [W]
+Zone,Average,Space ITE UPS Electricity Rate [W]
+Zone,Average,Space ITE CPU Electricity Rate at Design Inlet Conditions [W]
+Zone,Average,Space ITE Fan Electricity Rate at Design Inlet Conditions [W]
+Zone,Average,Space ITE UPS Heat Gain to Zone Rate [W]
+Zone,Average,Space ITE Total Heat Gain to Zone Rate [W]
+Zone,Sum,Space ITE CPU Electricity Energy [J]
+Zone,Sum,Space ITE Fan Electricity Energy [J]
+Zone,Sum,Space ITE UPS Electricity Energy [J]
+Zone,Sum,Space ITE CPU Electricity Energy at Design Inlet Conditions [J]
+Zone,Sum,Space ITE Fan Electricity Energy at Design Inlet Conditions [J]
+Zone,Sum,Space ITE UPS Heat Gain to Zone Energy [J]
+Zone,Sum,Space ITE Total Heat Gain to Zone Energy [J]
+Zone,Average,Space ITE Standard Density Air Volume Flow Rate [m3/s]
+Zone,Average,Space ITE Air Mass Flow Rate [kg/s]
+Zone,Average,Space ITE Average Supply Heat Index []
+Zone,Sum,Space ITE Any Air Inlet Operating Range Exceeded Time [hr]
+Zone,Sum,Space ITE Any Air Inlet Dry-Bulb Temperature Above Operating Range Time [hr]
+Zone,Sum,Space ITE Any Air Inlet Dry-Bulb Temperature Below Operating Range Time [hr]
+Zone,Sum,Space ITE Any Air Inlet Dewpoint Temperature Above Operating Range Time [hr]
+Zone,Sum,Space ITE Any Air Inlet Dewpoint Temperature Below Operating Range Time [hr]
+Zone,Sum,Space ITE Any Air Inlet Relative Humidity Above Operating Range Time [hr]
+Zone,Sum,Space ITE Any Air Inlet Relative Humidity Below Operating Range Time [hr]
 HVAC,Average,Power Utilization Effectiveness []
+Zone,Average,Zone Mean Radiant Temperature [C]
 Zone,Average,Zone Windows Total Transmitted Solar Radiation Rate [W]
 Zone,Average,Zone Exterior Windows Total Transmitted Beam Solar Radiation Rate [W]
 Zone,Average,Zone Interior Windows Total Transmitted Beam Solar Radiation Rate [W]
 Zone,Average,Zone Exterior Windows Total Transmitted Diffuse Solar Radiation Rate [W]
 Zone,Average,Zone Interior Windows Total Transmitted Diffuse Solar Radiation Rate [W]
-Zone,Average,Zone Windows Total Heat Gain Rate [W]
-Zone,Average,Zone Windows Total Heat Loss Rate [W]
 Zone,Sum,Zone Windows Total Transmitted Solar Radiation Energy [J]
 Zone,Sum,Zone Exterior Windows Total Transmitted Beam Solar Radiation Energy [J]
 Zone,Sum,Zone Interior Windows Total Transmitted Beam Solar Radiation Energy [J]
 Zone,Sum,Zone Exterior Windows Total Transmitted Diffuse Solar Radiation Energy [J]
 Zone,Sum,Zone Interior Windows Total Transmitted Diffuse Solar Radiation Energy [J]
+Zone,Average,Zone Windows Total Heat Gain Rate [W]
+Zone,Average,Zone Windows Total Heat Loss Rate [W]
 Zone,Sum,Zone Windows Total Heat Gain Energy [J]
 Zone,Sum,Zone Windows Total Heat Loss Energy [J]
 Zone,Average,Surface Outside Normal Azimuth Angle [deg]
 Zone,Average,Surface Outside Face Sunlit Area [m2]
 Zone,Average,Surface Outside Face Sunlit Fraction []
 Zone,Average,Surface Outside Face Incident Solar Radiation Rate per Area [W/m2]
 Zone,Average,Surface Outside Face Incident Beam Solar Radiation Rate per Area [W/m2]
@@ -295,15 +367,14 @@
 Zone,Average,Surface Inside Face Convection Model Equation Index []
 Zone,Average,Surface Inside Face Convection Reference Air Index []
 Zone,Average,Surface Outside Face Convection Classification Index []
 Zone,Average,Surface Outside Face Forced Convection Model Equation Index []
 Zone,Average,Surface Outside Face Natural Convection Model Equation Index []
 Zone,Average,Surface Inside Face Heat Source Gain Rate per Area [W/m2]
 Zone,Average,Surface Outside Face Heat Source Gain Rate per Area [W/m2]
-Zone,Average,Zone Mean Radiant Temperature [C]
 Zone,Sum,Site Total Surface Heat Emission to Air [J]
 Zone,Average,Zone Mean Air Temperature [C]
 Zone,Average,Zone Operative Temperature [C]
 Zone,Average,Zone Mean Air Dewpoint Temperature [C]
 Zone,Average,Zone Mean Air Humidity Ratio [kgWater/kgDryAir]
 HVAC,Average,Zone Air Heat Balance Internal Convective Heat Gain Rate [W]
 HVAC,Average,Zone Air Heat Balance Surface Convection Rate [W]
@@ -316,34 +387,34 @@
 HVAC,Average,Zone Exfiltration Sensible Heat Transfer Rate [W]
 HVAC,Average,Zone Exfiltration Latent Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Sensible Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Latent Heat Transfer Rate [W]
 HVAC,Sum,Site Total Zone Exfiltration Heat Loss [J]
 HVAC,Sum,Site Total Zone Exhaust Air Heat Loss [J]
+HVAC,Average,Zone Air Temperature [C]
+HVAC,Average,Zone Air Humidity Ratio []
+HVAC,Average,Zone Air Relative Humidity [%]
 HVAC,Sum,Zone Air System Sensible Heating Energy [J]
 HVAC,Sum,Zone Air System Sensible Cooling Energy [J]
 HVAC,Average,Zone Air System Sensible Heating Rate [W]
 HVAC,Average,Zone Air System Sensible Cooling Rate [W]
-HVAC,Average,Zone Air Temperature [C]
-HVAC,Average,Zone Thermostat Air Temperature [C]
-HVAC,Average,Zone Air Humidity Ratio []
-HVAC,Average,Zone Air Relative Humidity [%]
 HVAC,Average,Zone Predicted Sensible Load to Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Sensible Load to Heating Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Sensible Load to Cooling Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Heating Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Cooling Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Moisture Load Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone Predicted Moisture Load to Humidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone Predicted Moisture Load to Dehumidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load to Humidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load to Dehumidifying Setpoint Moisture Transfer Rate [kgWater/s]
+HVAC,Average,Zone Thermostat Air Temperature [C]
 Zone,Average,Zone Thermostat Control Type []
 HVAC,Average,Zone Thermostat Heating Setpoint Temperature [C]
 HVAC,Average,Zone Thermostat Cooling Setpoint Temperature [C]
 Zone,Average,Zone Adaptive Comfort Operative Temperature Set Point [C]
 HVAC,Average,Zone Predicted Sensible Load Room Air Correction Factor []
 HVAC,Sum,HVAC System Solver Iteration Count []
 HVAC,Sum,Air System Solver Iteration Count []
@@ -442,21 +513,21 @@
 HVAC,Average,Evaporative Cooler Dewpoint Bound Status []
 HVAC,Average,Evaporative Cooler Operating Mode Status []
 HVAC,Average,Evaporative Cooler Stage Effectiveness []
 HVAC,Sum,Evaporative Cooler Electricity Energy [J]
 HVAC,Average,Evaporative Cooler Electricity Rate [W]
 HVAC,Sum,Evaporative Cooler Water Volume [m3]
 HVAC,Sum,Evaporative Cooler Mains Water Volume [m3]
+HVAC,Average,Coil System Part Load Ratio []
+HVAC,Average,Coil System Frost Control Status []
 HVAC,Average,Cooling Coil Latent Cooling Rate [W]
 HVAC,Sum,Cooling Coil Latent Cooling Energy [J]
 HVAC,Average,Cooling Coil Electricity Rate [W]
 HVAC,Sum,Cooling Coil Electricity Energy [J]
 HVAC,Average,Cooling Coil Runtime Fraction []
-HVAC,Average,Coil System Part Load Ratio []
-HVAC,Average,Coil System Frost Control Status []
 HVAC,Average,Chiller Electricity Rate [W]
 HVAC,Sum,Chiller Electricity Energy [J]
 HVAC,Average,Chiller Evaporator Cooling Rate [W]
 HVAC,Sum,Chiller Evaporator Cooling Energy [J]
 HVAC,Average,Chiller Evaporator Inlet Temperature [C]
 HVAC,Average,Chiller Evaporator Outlet Temperature [C]
 HVAC,Average,Chiller Evaporator Mass Flow Rate [kg/s]
```

### Comparing `sinergym-2.4.1/sinergym/data/variables/5ZoneAutoDXVAV.rdd` & `sinergym-2.5.0/sinergym/data/variables/5ZoneAutoDXVAV.rdd`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-Program Version,EnergyPlus, Version 9.5.0-de239b2e5f, YMD=2022.05.06 17:40,
+Program Version,EnergyPlus, Version 23.1.0-87ed9199d4, YMD=2023.05.31 13:48,
 Var Type (reported time step),Var Report Type,Variable Name [Units]
 Zone,Average,Site Outdoor Air Drybulb Temperature [C]
 Zone,Average,Site Outdoor Air Dewpoint Temperature [C]
 Zone,Average,Site Outdoor Air Wetbulb Temperature [C]
 Zone,Average,Site Outdoor Air Humidity Ratio [kgWater/kgDryAir]
 Zone,Average,Site Outdoor Air Relative Humidity [%]
 Zone,Average,Site Outdoor Air Barometric Pressure [Pa]
 Zone,Average,Site Wind Speed [m/s]
 Zone,Average,Site Wind Direction [deg]
 Zone,Average,Site Sky Temperature [C]
 Zone,Average,Site Horizontal Infrared Radiation Rate per Area [W/m2]
 Zone,Average,Site Diffuse Solar Radiation Rate per Area [W/m2]
 Zone,Average,Site Direct Solar Radiation Rate per Area [W/m2]
+Zone,Sum,Liquid Precipitation Depth [m]
+Zone,Average,Site Precipitation Rate [m/s]
 Zone,Sum,Site Precipitation Depth [m]
 Zone,Average,Site Ground Reflected Solar Radiation Rate per Area [W/m2]
 Zone,Average,Site Ground Temperature [C]
 Zone,Average,Site Surface Ground Temperature [C]
 Zone,Average,Site Deep Ground Temperature [C]
 Zone,Average,Site Simple Factor Model Ground Temperature [C]
 Zone,Average,Site Total Sky Cover []
@@ -47,14 +49,24 @@
 Zone,Average,Zone Total Internal Visible Radiation Heating Rate [W]
 Zone,Sum,Zone Total Internal Convective Heating Energy [J]
 Zone,Average,Zone Total Internal Convective Heating Rate [W]
 Zone,Sum,Zone Total Internal Latent Gain Energy [J]
 Zone,Average,Zone Total Internal Latent Gain Rate [W]
 Zone,Sum,Zone Total Internal Total Heating Energy [J]
 Zone,Average,Zone Total Internal Total Heating Rate [W]
+Zone,Sum,Space Total Internal Radiant Heating Energy [J]
+Zone,Average,Space Total Internal Radiant Heating Rate [W]
+Zone,Sum,Space Total Internal Visible Radiation Heating Energy [J]
+Zone,Average,Space Total Internal Visible Radiation Heating Rate [W]
+Zone,Sum,Space Total Internal Convective Heating Energy [J]
+Zone,Average,Space Total Internal Convective Heating Rate [W]
+Zone,Sum,Space Total Internal Latent Gain Energy [J]
+Zone,Average,Space Total Internal Latent Gain Rate [W]
+Zone,Sum,Space Total Internal Total Heating Energy [J]
+Zone,Average,Space Total Internal Total Heating Rate [W]
 Zone,Average,People Occupant Count []
 Zone,Sum,People Radiant Heating Energy [J]
 Zone,Average,People Radiant Heating Rate [W]
 Zone,Sum,People Convective Heating Energy [J]
 Zone,Average,People Convective Heating Rate [W]
 Zone,Sum,People Sensible Heating Energy [J]
 Zone,Average,People Sensible Heating Rate [W]
@@ -71,14 +83,25 @@
 Zone,Average,Zone People Convective Heating Rate [W]
 Zone,Sum,Zone People Sensible Heating Energy [J]
 Zone,Average,Zone People Sensible Heating Rate [W]
 Zone,Sum,Zone People Latent Gain Energy [J]
 Zone,Average,Zone People Latent Gain Rate [W]
 Zone,Sum,Zone People Total Heating Energy [J]
 Zone,Average,Zone People Total Heating Rate [W]
+Zone,Average,Space People Occupant Count []
+Zone,Sum,Space People Radiant Heating Energy [J]
+Zone,Average,Space People Radiant Heating Rate [W]
+Zone,Sum,Space People Convective Heating Energy [J]
+Zone,Average,Space People Convective Heating Rate [W]
+Zone,Sum,Space People Sensible Heating Energy [J]
+Zone,Average,Space People Sensible Heating Rate [W]
+Zone,Sum,Space People Latent Gain Energy [J]
+Zone,Average,Space People Latent Gain Rate [W]
+Zone,Sum,Space People Total Heating Energy [J]
+Zone,Average,Space People Total Heating Rate [W]
 Zone,Average,Lights Electricity Rate [W]
 Zone,Sum,Lights Radiant Heating Energy [J]
 Zone,Average,Lights Radiant Heating Rate [W]
 Zone,Sum,Lights Visible Radiation Heating Energy [J]
 Zone,Average,Lights Visible Radiation Heating Rate [W]
 Zone,Sum,Lights Convective Heating Energy [J]
 Zone,Average,Lights Convective Heating Rate [W]
@@ -95,14 +118,26 @@
 Zone,Average,Zone Lights Visible Radiation Heating Rate [W]
 Zone,Sum,Zone Lights Convective Heating Energy [J]
 Zone,Average,Zone Lights Convective Heating Rate [W]
 Zone,Sum,Zone Lights Return Air Heating Energy [J]
 Zone,Average,Zone Lights Return Air Heating Rate [W]
 Zone,Sum,Zone Lights Total Heating Energy [J]
 Zone,Average,Zone Lights Total Heating Rate [W]
+Zone,Average,Space Lights Electricity Rate [W]
+Zone,Sum,Space Lights Electricity Energy [J]
+Zone,Sum,Space Lights Radiant Heating Energy [J]
+Zone,Average,Space Lights Radiant Heating Rate [W]
+Zone,Sum,Space Lights Visible Radiation Heating Energy [J]
+Zone,Average,Space Lights Visible Radiation Heating Rate [W]
+Zone,Sum,Space Lights Convective Heating Energy [J]
+Zone,Average,Space Lights Convective Heating Rate [W]
+Zone,Sum,Space Lights Return Air Heating Energy [J]
+Zone,Average,Space Lights Return Air Heating Rate [W]
+Zone,Sum,Space Lights Total Heating Energy [J]
+Zone,Average,Space Lights Total Heating Rate [W]
 Zone,Average,Electric Equipment Electricity Rate [W]
 Zone,Sum,Electric Equipment Electricity Energy [J]
 Zone,Sum,Electric Equipment Radiant Heating Energy [J]
 Zone,Average,Electric Equipment Radiant Heating Rate [W]
 Zone,Sum,Electric Equipment Convective Heating Energy [J]
 Zone,Average,Electric Equipment Convective Heating Rate [W]
 Zone,Sum,Electric Equipment Latent Gain Energy [J]
@@ -119,26 +154,39 @@
 Zone,Average,Zone Electric Equipment Convective Heating Rate [W]
 Zone,Sum,Zone Electric Equipment Latent Gain Energy [J]
 Zone,Average,Zone Electric Equipment Latent Gain Rate [W]
 Zone,Sum,Zone Electric Equipment Lost Heat Energy [J]
 Zone,Average,Zone Electric Equipment Lost Heat Rate [W]
 Zone,Sum,Zone Electric Equipment Total Heating Energy [J]
 Zone,Average,Zone Electric Equipment Total Heating Rate [W]
+Zone,Average,Space Electric Equipment Electricity Rate [W]
+Zone,Sum,Space Electric Equipment Electricity Energy [J]
+Zone,Sum,Space Electric Equipment Radiant Heating Energy [J]
+Zone,Average,Space Electric Equipment Radiant Heating Rate [W]
+Zone,Sum,Space Electric Equipment Convective Heating Energy [J]
+Zone,Average,Space Electric Equipment Convective Heating Rate [W]
+Zone,Sum,Space Electric Equipment Latent Gain Energy [J]
+Zone,Average,Space Electric Equipment Latent Gain Rate [W]
+Zone,Sum,Space Electric Equipment Lost Heat Energy [J]
+Zone,Average,Space Electric Equipment Lost Heat Rate [W]
+Zone,Sum,Space Electric Equipment Total Heating Energy [J]
+Zone,Average,Space Electric Equipment Total Heating Rate [W]
+Zone,Average,Zone Mean Radiant Temperature [C]
 Zone,Average,Zone Windows Total Transmitted Solar Radiation Rate [W]
 Zone,Average,Zone Exterior Windows Total Transmitted Beam Solar Radiation Rate [W]
 Zone,Average,Zone Interior Windows Total Transmitted Beam Solar Radiation Rate [W]
 Zone,Average,Zone Exterior Windows Total Transmitted Diffuse Solar Radiation Rate [W]
 Zone,Average,Zone Interior Windows Total Transmitted Diffuse Solar Radiation Rate [W]
-Zone,Average,Zone Windows Total Heat Gain Rate [W]
-Zone,Average,Zone Windows Total Heat Loss Rate [W]
 Zone,Sum,Zone Windows Total Transmitted Solar Radiation Energy [J]
 Zone,Sum,Zone Exterior Windows Total Transmitted Beam Solar Radiation Energy [J]
 Zone,Sum,Zone Interior Windows Total Transmitted Beam Solar Radiation Energy [J]
 Zone,Sum,Zone Exterior Windows Total Transmitted Diffuse Solar Radiation Energy [J]
 Zone,Sum,Zone Interior Windows Total Transmitted Diffuse Solar Radiation Energy [J]
+Zone,Average,Zone Windows Total Heat Gain Rate [W]
+Zone,Average,Zone Windows Total Heat Loss Rate [W]
 Zone,Sum,Zone Windows Total Heat Gain Energy [J]
 Zone,Sum,Zone Windows Total Heat Loss Energy [J]
 Zone,Average,Surface Outside Normal Azimuth Angle [deg]
 Zone,Average,Surface Outside Face Sunlit Area [m2]
 Zone,Average,Surface Outside Face Sunlit Fraction []
 Zone,Average,Surface Outside Face Incident Solar Radiation Rate per Area [W/m2]
 Zone,Average,Surface Outside Face Incident Beam Solar Radiation Rate per Area [W/m2]
@@ -277,15 +325,14 @@
 Zone,Average,Surface Outside Face Forced Convection Model Equation Index []
 Zone,Average,Surface Outside Face Natural Convection Model Equation Index []
 Zone,Average,Surface Inside Face Heat Source Gain Rate per Area [W/m2]
 Zone,Average,Surface Outside Face Heat Source Gain Rate per Area [W/m2]
 Zone,Average,Surface Shading Device Is On Time Fraction []
 Zone,Average,Surface Storm Window On Off Status []
 Zone,Average,Surface Window Blind Slat Angle [deg]
-Zone,Average,Zone Mean Radiant Temperature [C]
 Zone,Sum,Site Total Surface Heat Emission to Air [J]
 Zone,Average,Zone Mean Air Temperature [C]
 Zone,Average,Zone Operative Temperature [C]
 Zone,Average,Zone Mean Air Dewpoint Temperature [C]
 Zone,Average,Zone Mean Air Humidity Ratio [kgWater/kgDryAir]
 HVAC,Average,Zone Air Heat Balance Internal Convective Heat Gain Rate [W]
 HVAC,Average,Zone Air Heat Balance Surface Convection Rate [W]
@@ -298,47 +345,60 @@
 HVAC,Average,Zone Exfiltration Sensible Heat Transfer Rate [W]
 HVAC,Average,Zone Exfiltration Latent Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Sensible Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Latent Heat Transfer Rate [W]
 HVAC,Sum,Site Total Zone Exfiltration Heat Loss [J]
 HVAC,Sum,Site Total Zone Exhaust Air Heat Loss [J]
+HVAC,Sum,Infiltration Sensible Heat Loss Energy [J]
+HVAC,Sum,Infiltration Sensible Heat Gain Energy [J]
+HVAC,Sum,Infiltration Latent Heat Loss Energy [J]
+HVAC,Sum,Infiltration Latent Heat Gain Energy [J]
+HVAC,Sum,Infiltration Total Heat Loss Energy [J]
+HVAC,Sum,Infiltration Total Heat Gain Energy [J]
+HVAC,Average,Infiltration Current Density Volume Flow Rate [m3/s]
+HVAC,Average,Infiltration Standard Density Volume Flow Rate [m3/s]
+HVAC,Sum,Infiltration Current Density Volume [m3]
+HVAC,Sum,Infiltration Standard Density Volume [m3]
+HVAC,Sum,Infiltration Mass [kg]
+HVAC,Average,Infiltration Mass Flow Rate [kg/s]
+HVAC,Average,Infiltration Air Change Rate [ach]
 HVAC,Sum,Zone Infiltration Sensible Heat Loss Energy [J]
 HVAC,Sum,Zone Infiltration Sensible Heat Gain Energy [J]
 HVAC,Sum,Zone Infiltration Latent Heat Loss Energy [J]
 HVAC,Sum,Zone Infiltration Latent Heat Gain Energy [J]
 HVAC,Sum,Zone Infiltration Total Heat Loss Energy [J]
 HVAC,Sum,Zone Infiltration Total Heat Gain Energy [J]
 HVAC,Average,Zone Infiltration Current Density Volume Flow Rate [m3/s]
 HVAC,Average,Zone Infiltration Standard Density Volume Flow Rate [m3/s]
 HVAC,Sum,Zone Infiltration Current Density Volume [m3]
 HVAC,Sum,Zone Infiltration Standard Density Volume [m3]
 HVAC,Sum,Zone Infiltration Mass [kg]
 HVAC,Average,Zone Infiltration Mass Flow Rate [kg/s]
 HVAC,Average,Zone Infiltration Air Change Rate [ach]
+HVAC,Average,Zone Air Temperature [C]
+HVAC,Average,Zone Air Humidity Ratio []
+HVAC,Average,Zone Air Relative Humidity [%]
 HVAC,Sum,Zone Air System Sensible Heating Energy [J]
 HVAC,Sum,Zone Air System Sensible Cooling Energy [J]
 HVAC,Average,Zone Air System Sensible Heating Rate [W]
 HVAC,Average,Zone Air System Sensible Cooling Rate [W]
-HVAC,Average,Zone Air Temperature [C]
-HVAC,Average,Zone Thermostat Air Temperature [C]
-HVAC,Average,Zone Air Humidity Ratio []
-HVAC,Average,Zone Air Relative Humidity [%]
 HVAC,Average,Zone Predicted Sensible Load to Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Sensible Load to Heating Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Sensible Load to Cooling Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Heating Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Cooling Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Moisture Load Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone Predicted Moisture Load to Humidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone Predicted Moisture Load to Dehumidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load to Humidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load to Dehumidifying Setpoint Moisture Transfer Rate [kgWater/s]
+HVAC,Average,Zone Thermostat Air Temperature [C]
 Zone,Average,Zone Thermostat Control Type []
 HVAC,Average,Zone Thermostat Heating Setpoint Temperature [C]
 HVAC,Average,Zone Thermostat Cooling Setpoint Temperature [C]
 Zone,Average,Zone Adaptive Comfort Operative Temperature Set Point [C]
 HVAC,Average,Zone Predicted Sensible Load Room Air Correction Factor []
 HVAC,Sum,HVAC System Solver Iteration Count []
 HVAC,Sum,Air System Solver Iteration Count []
@@ -357,20 +417,14 @@
 HVAC,Sum,Facility Total Produced Electricity Energy [J]
 HVAC,Sum,Zone Oscillating Temperatures Time [hr]
 HVAC,Sum,Zone Oscillating Temperatures During Occupancy Time [hr]
 HVAC,Sum,Zone Oscillating Temperatures in Deadband Time [hr]
 HVAC,Sum,Facility Any Zone Oscillating Temperatures Time [hr]
 HVAC,Sum,Facility Any Zone Oscillating Temperatures During Occupancy Time [hr]
 HVAC,Sum,Facility Any Zone Oscillating Temperatures in Deadband Time [hr]
-Zone,Average,Zone Thermal Comfort Fanger Model PMV []
-Zone,Average,Zone Thermal Comfort Fanger Model PPD [%]
-Zone,Average,Zone Thermal Comfort Clothing Surface Temperature [C]
-Zone,Average,Zone Thermal Comfort Mean Radiant Temperature [C]
-Zone,Average,Zone Thermal Comfort Operative Temperature [C]
-Zone,Average,Zone Thermal Comfort Clothing Value [clo]
 Zone,Sum,Zone Thermal Comfort ASHRAE 55 Simple Model Summer Clothes Not Comfortable Time [hr]
 Zone,Sum,Zone Thermal Comfort ASHRAE 55 Simple Model Winter Clothes Not Comfortable Time [hr]
 Zone,Sum,Zone Thermal Comfort ASHRAE 55 Simple Model Summer or Winter Clothes Not Comfortable Time [hr]
 Zone,Sum,Facility Thermal Comfort ASHRAE 55 Simple Model Summer Clothes Not Comfortable Time [hr]
 Zone,Sum,Facility Thermal Comfort ASHRAE 55 Simple Model Winter Clothes Not Comfortable Time [hr]
 Zone,Sum,Facility Thermal Comfort ASHRAE 55 Simple Model Summer or Winter Clothes Not Comfortable Time [hr]
 Zone,Sum,Zone Heating Setpoint Not Met Time [hr]
@@ -389,16 +443,21 @@
 HVAC,Average,Zone Air Terminal Sensible Heating Rate [W]
 HVAC,Average,Zone Air Terminal Sensible Cooling Rate [W]
 HVAC,Average,Zone Air Terminal VAV Damper Position []
 HVAC,Average,Zone Air Terminal Minimum Air Flow Fraction []
 HVAC,Average,Zone Air Terminal Outdoor Air Volume Flow Rate [m3/s]
 HVAC,Sum,Heating Coil Heating Energy [J]
 HVAC,Average,Heating Coil Heating Rate [W]
+HVAC,Sum,Heating Coil NaturalGas Energy [J]
+HVAC,Average,Heating Coil NaturalGas Rate [W]
 HVAC,Sum,Heating Coil Electricity Energy [J]
 HVAC,Average,Heating Coil Electricity Rate [W]
+HVAC,Average,Heating Coil Runtime Fraction []
+HVAC,Average,Heating Coil Ancillary NaturalGas Rate [W]
+HVAC,Sum,Heating Coil Ancillary NaturalGas Energy [J]
 HVAC,Average,Availability Manager Scheduled Control Status []
 HVAC,Average,Air System Simulation Cycle On Off Status []
 HVAC,Average,Fan Electricity Rate [W]
 HVAC,Average,Fan Rise in Air Temperature [deltaC]
 HVAC,Average,Fan Heat Gain to Air [W]
 HVAC,Sum,Fan Electricity Energy [J]
 HVAC,Average,Fan Air Mass Flow Rate [kg/s]
@@ -414,14 +473,17 @@
 HVAC,Average,Air System Outdoor Air Flow Fraction []
 HVAC,Average,Air System Outdoor Air Minimum Flow Fraction []
 HVAC,Average,Air System Outdoor Air Mass Flow Rate [kg/s]
 HVAC,Average,Air System Mixed Air Mass Flow Rate [kg/s]
 HVAC,Average,Air System Relief Air Heat Transfer Rate [W]
 HVAC,Average,Air System Relief Air Sensible Heat Transfer Rate [W]
 HVAC,Average,Air System Relief Air Latent Heat Transfer Rate [W]
+HVAC,Average,Coil System Cycling Ratio []
+HVAC,Average,Coil System Compressor Speed Ratio []
+HVAC,Average,Coil System Frost Control Status []
 HVAC,Average,Cooling Coil Total Cooling Rate [W]
 HVAC,Sum,Cooling Coil Total Cooling Energy [J]
 HVAC,Average,Cooling Coil Sensible Cooling Rate [W]
 HVAC,Sum,Cooling Coil Sensible Cooling Energy [J]
 HVAC,Average,Cooling Coil Latent Cooling Rate [W]
 HVAC,Sum,Cooling Coil Latent Cooling Energy [J]
 HVAC,Average,Cooling Coil Electricity Rate [W]
@@ -430,17 +492,14 @@
 HVAC,Average,Cooling Coil Condenser Inlet Temperature [C]
 HVAC,Sum,Cooling Coil Evaporative Condenser Water Volume [m3]
 HVAC,Sum,Cooling Coil Evaporative Condenser Mains Supply Water Volume [m3]
 HVAC,Average,Cooling Coil Evaporative Condenser Pump Electricity Rate [W]
 HVAC,Sum,Cooling Coil Evaporative Condenser Pump Electricity Energy [J]
 HVAC,Average,Cooling Coil Basin Heater Electricity Rate [W]
 HVAC,Sum,Cooling Coil Basin Heater Electricity Energy [J]
-HVAC,Average,Coil System Cycling Ratio []
-HVAC,Average,Coil System Compressor Speed Ratio []
-HVAC,Average,Coil System Frost Control Status []
 HVAC,Average,Performance Curve Input Variable 1 Value []
 HVAC,Average,Performance Curve Input Variable 2 Value []
 HVAC,Average,Performance Curve Output Value []
 HVAC,Average,System Node Temperature [C]
 HVAC,Average,System Node Mass Flow Rate [kg/s]
 HVAC,Average,System Node Humidity Ratio [kgWater/kgDryAir]
 HVAC,Average,System Node Setpoint Temperature [C]
```

### Comparing `sinergym-2.4.1/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd` & `sinergym-2.5.0/sinergym/data/variables/ASHRAE901_Warehouse_STD2019_Denver.rdd`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-Program Version,EnergyPlus, Version 9.5.0-de239b2e5f, YMD=2022.06.06 12:00,
+Program Version,EnergyPlus, Version 23.1.0-87ed9199d4, YMD=2023.06.01 09:05,
 Var Type (reported time step),Var Report Type,Variable Name [Units]
 Zone,Average,Site Outdoor Air Drybulb Temperature [C]
 Zone,Average,Site Outdoor Air Dewpoint Temperature [C]
 Zone,Average,Site Outdoor Air Wetbulb Temperature [C]
 Zone,Average,Site Outdoor Air Humidity Ratio [kgWater/kgDryAir]
 Zone,Average,Site Outdoor Air Relative Humidity [%]
 Zone,Average,Site Outdoor Air Barometric Pressure [Pa]
 Zone,Average,Site Wind Speed [m/s]
 Zone,Average,Site Wind Direction [deg]
 Zone,Average,Site Sky Temperature [C]
 Zone,Average,Site Horizontal Infrared Radiation Rate per Area [W/m2]
 Zone,Average,Site Diffuse Solar Radiation Rate per Area [W/m2]
 Zone,Average,Site Direct Solar Radiation Rate per Area [W/m2]
+Zone,Sum,Liquid Precipitation Depth [m]
+Zone,Average,Site Precipitation Rate [m/s]
 Zone,Sum,Site Precipitation Depth [m]
 Zone,Average,Site Ground Reflected Solar Radiation Rate per Area [W/m2]
 Zone,Average,Site Ground Temperature [C]
 Zone,Average,Site Surface Ground Temperature [C]
 Zone,Average,Site Deep Ground Temperature [C]
 Zone,Average,Site Simple Factor Model Ground Temperature [C]
 Zone,Average,Site Total Sky Cover []
@@ -47,14 +49,24 @@
 Zone,Average,Zone Total Internal Visible Radiation Heating Rate [W]
 Zone,Sum,Zone Total Internal Convective Heating Energy [J]
 Zone,Average,Zone Total Internal Convective Heating Rate [W]
 Zone,Sum,Zone Total Internal Latent Gain Energy [J]
 Zone,Average,Zone Total Internal Latent Gain Rate [W]
 Zone,Sum,Zone Total Internal Total Heating Energy [J]
 Zone,Average,Zone Total Internal Total Heating Rate [W]
+Zone,Sum,Space Total Internal Radiant Heating Energy [J]
+Zone,Average,Space Total Internal Radiant Heating Rate [W]
+Zone,Sum,Space Total Internal Visible Radiation Heating Energy [J]
+Zone,Average,Space Total Internal Visible Radiation Heating Rate [W]
+Zone,Sum,Space Total Internal Convective Heating Energy [J]
+Zone,Average,Space Total Internal Convective Heating Rate [W]
+Zone,Sum,Space Total Internal Latent Gain Energy [J]
+Zone,Average,Space Total Internal Latent Gain Rate [W]
+Zone,Sum,Space Total Internal Total Heating Energy [J]
+Zone,Average,Space Total Internal Total Heating Rate [W]
 Zone,Average,People Occupant Count []
 Zone,Sum,People Radiant Heating Energy [J]
 Zone,Average,People Radiant Heating Rate [W]
 Zone,Sum,People Convective Heating Energy [J]
 Zone,Average,People Convective Heating Rate [W]
 Zone,Sum,People Sensible Heating Energy [J]
 Zone,Average,People Sensible Heating Rate [W]
@@ -71,14 +83,25 @@
 Zone,Average,Zone People Convective Heating Rate [W]
 Zone,Sum,Zone People Sensible Heating Energy [J]
 Zone,Average,Zone People Sensible Heating Rate [W]
 Zone,Sum,Zone People Latent Gain Energy [J]
 Zone,Average,Zone People Latent Gain Rate [W]
 Zone,Sum,Zone People Total Heating Energy [J]
 Zone,Average,Zone People Total Heating Rate [W]
+Zone,Average,Space People Occupant Count []
+Zone,Sum,Space People Radiant Heating Energy [J]
+Zone,Average,Space People Radiant Heating Rate [W]
+Zone,Sum,Space People Convective Heating Energy [J]
+Zone,Average,Space People Convective Heating Rate [W]
+Zone,Sum,Space People Sensible Heating Energy [J]
+Zone,Average,Space People Sensible Heating Rate [W]
+Zone,Sum,Space People Latent Gain Energy [J]
+Zone,Average,Space People Latent Gain Rate [W]
+Zone,Sum,Space People Total Heating Energy [J]
+Zone,Average,Space People Total Heating Rate [W]
 Zone,Average,Lights Electricity Rate [W]
 Zone,Sum,Lights Radiant Heating Energy [J]
 Zone,Average,Lights Radiant Heating Rate [W]
 Zone,Sum,Lights Visible Radiation Heating Energy [J]
 Zone,Average,Lights Visible Radiation Heating Rate [W]
 Zone,Sum,Lights Convective Heating Energy [J]
 Zone,Average,Lights Convective Heating Rate [W]
@@ -95,14 +118,26 @@
 Zone,Average,Zone Lights Visible Radiation Heating Rate [W]
 Zone,Sum,Zone Lights Convective Heating Energy [J]
 Zone,Average,Zone Lights Convective Heating Rate [W]
 Zone,Sum,Zone Lights Return Air Heating Energy [J]
 Zone,Average,Zone Lights Return Air Heating Rate [W]
 Zone,Sum,Zone Lights Total Heating Energy [J]
 Zone,Average,Zone Lights Total Heating Rate [W]
+Zone,Average,Space Lights Electricity Rate [W]
+Zone,Sum,Space Lights Electricity Energy [J]
+Zone,Sum,Space Lights Radiant Heating Energy [J]
+Zone,Average,Space Lights Radiant Heating Rate [W]
+Zone,Sum,Space Lights Visible Radiation Heating Energy [J]
+Zone,Average,Space Lights Visible Radiation Heating Rate [W]
+Zone,Sum,Space Lights Convective Heating Energy [J]
+Zone,Average,Space Lights Convective Heating Rate [W]
+Zone,Sum,Space Lights Return Air Heating Energy [J]
+Zone,Average,Space Lights Return Air Heating Rate [W]
+Zone,Sum,Space Lights Total Heating Energy [J]
+Zone,Average,Space Lights Total Heating Rate [W]
 Zone,Average,Electric Equipment Electricity Rate [W]
 Zone,Sum,Electric Equipment Electricity Energy [J]
 Zone,Sum,Electric Equipment Radiant Heating Energy [J]
 Zone,Average,Electric Equipment Radiant Heating Rate [W]
 Zone,Sum,Electric Equipment Convective Heating Energy [J]
 Zone,Average,Electric Equipment Convective Heating Rate [W]
 Zone,Sum,Electric Equipment Latent Gain Energy [J]
@@ -119,27 +154,39 @@
 Zone,Average,Zone Electric Equipment Convective Heating Rate [W]
 Zone,Sum,Zone Electric Equipment Latent Gain Energy [J]
 Zone,Average,Zone Electric Equipment Latent Gain Rate [W]
 Zone,Sum,Zone Electric Equipment Lost Heat Energy [J]
 Zone,Average,Zone Electric Equipment Lost Heat Rate [W]
 Zone,Sum,Zone Electric Equipment Total Heating Energy [J]
 Zone,Average,Zone Electric Equipment Total Heating Rate [W]
-Zone,Sum,Wired_LTG [J]
+Zone,Average,Space Electric Equipment Electricity Rate [W]
+Zone,Sum,Space Electric Equipment Electricity Energy [J]
+Zone,Sum,Space Electric Equipment Radiant Heating Energy [J]
+Zone,Average,Space Electric Equipment Radiant Heating Rate [W]
+Zone,Sum,Space Electric Equipment Convective Heating Energy [J]
+Zone,Average,Space Electric Equipment Convective Heating Rate [W]
+Zone,Sum,Space Electric Equipment Latent Gain Energy [J]
+Zone,Average,Space Electric Equipment Latent Gain Rate [W]
+Zone,Sum,Space Electric Equipment Lost Heat Energy [J]
+Zone,Average,Space Electric Equipment Lost Heat Rate [W]
+Zone,Sum,Space Electric Equipment Total Heating Energy [J]
+Zone,Average,Space Electric Equipment Total Heating Rate [W]
+Zone,Average,Zone Mean Radiant Temperature [C]
 Zone,Average,Zone Windows Total Transmitted Solar Radiation Rate [W]
 Zone,Average,Zone Exterior Windows Total Transmitted Beam Solar Radiation Rate [W]
 Zone,Average,Zone Interior Windows Total Transmitted Beam Solar Radiation Rate [W]
 Zone,Average,Zone Exterior Windows Total Transmitted Diffuse Solar Radiation Rate [W]
 Zone,Average,Zone Interior Windows Total Transmitted Diffuse Solar Radiation Rate [W]
-Zone,Average,Zone Windows Total Heat Gain Rate [W]
-Zone,Average,Zone Windows Total Heat Loss Rate [W]
 Zone,Sum,Zone Windows Total Transmitted Solar Radiation Energy [J]
 Zone,Sum,Zone Exterior Windows Total Transmitted Beam Solar Radiation Energy [J]
 Zone,Sum,Zone Interior Windows Total Transmitted Beam Solar Radiation Energy [J]
 Zone,Sum,Zone Exterior Windows Total Transmitted Diffuse Solar Radiation Energy [J]
 Zone,Sum,Zone Interior Windows Total Transmitted Diffuse Solar Radiation Energy [J]
+Zone,Average,Zone Windows Total Heat Gain Rate [W]
+Zone,Average,Zone Windows Total Heat Loss Rate [W]
 Zone,Sum,Zone Windows Total Heat Gain Energy [J]
 Zone,Sum,Zone Windows Total Heat Loss Energy [J]
 Zone,Average,Surface Outside Normal Azimuth Angle [deg]
 Zone,Average,Surface Outside Face Sunlit Area [m2]
 Zone,Average,Surface Outside Face Sunlit Fraction []
 Zone,Average,Surface Outside Face Incident Solar Radiation Rate per Area [W/m2]
 Zone,Average,Surface Outside Face Incident Beam Solar Radiation Rate per Area [W/m2]
@@ -154,15 +201,15 @@
 Zone,Average,Surface Anisotropic Sky Multiplier []
 Zone,Average,Surface Window BSDF Beam Direction Number []
 Zone,Average,Surface Window BSDF Beam Theta Angle [rad]
 Zone,Average,Surface Window BSDF Beam Phi Angle [rad]
 Zone,Average,Surface Window Total Glazing Layers Absorbed Solar Radiation Rate [W]
 Zone,Average,Surface Window Total Glazing Layers Absorbed Shortwave Radiation Rate [W]
 Zone,Average,Surface Window Front Face Temperature Layer 1 [C]
-Zone,Average,Surface Window Back Face Temperature Layer 3 [C]
+Zone,Average,Surface Window Back Face Temperature Layer 1 [C]
 Zone,Average,Surface Window Transmitted Solar Radiation Rate [W]
 Zone,Average,Surface Window Transmitted Beam Solar Radiation Rate [W]
 Zone,Average,Surface Window Transmitted Beam To Beam Solar Radiation Rate [W]
 Zone,Average,Surface Window Transmitted Beam To Diffuse Solar Radiation Rate [W]
 Zone,Average,Surface Window Transmitted Diffuse Solar Radiation Rate [W]
 Zone,Average,Surface Window Heat Gain Rate [W]
 Zone,Average,Surface Window Heat Loss Rate [W]
@@ -239,14 +286,33 @@
 Zone,Sum,Surface Inside Face Lights Radiation Heat Gain Energy [J]
 Zone,Average,Surface Inside Face Internal Gains Radiation Heat Gain Rate [W]
 Zone,Average,Surface Inside Face Internal Gains Radiation Heat Gain Rate per Area [W/m2]
 Zone,Sum,Surface Inside Face Internal Gains Radiation Heat Gain Energy [J]
 Zone,Average,Surface Inside Face System Radiation Heat Gain Rate [W]
 Zone,Average,Surface Inside Face System Radiation Heat Gain Rate per Area [W/m2]
 Zone,Sum,Surface Inside Face System Radiation Heat Gain Energy [J]
+Zone,Average,Surface Outside Face Outdoor Air Drybulb Temperature [C]
+Zone,Average,Surface Outside Face Outdoor Air Wetbulb Temperature [C]
+Zone,Average,Surface Outside Face Outdoor Air Wind Speed [m/s]
+Zone,Average,Surface Outside Face Outdoor Air Wind Direction [deg]
+Zone,Average,Surface Outside Face Convection Heat Gain Rate [W]
+Zone,Average,Surface Outside Face Convection Heat Gain Rate per Area [W/m2]
+Zone,Sum,Surface Outside Face Convection Heat Gain Energy [J]
+Zone,Average,Surface Outside Face Convection Heat Transfer Coefficient [W/m2-K]
+Zone,Average,Surface Outside Face Net Thermal Radiation Heat Gain Rate [W]
+Zone,Average,Surface Outside Face Net Thermal Radiation Heat Gain Rate per Area [W/m2]
+Zone,Sum,Surface Outside Face Net Thermal Radiation Heat Gain Energy [J]
+Zone,Average,Surface Outside Face Thermal Radiation to Air Heat Transfer Coefficient [W/m2-K]
+Zone,Average,Surface Outside Face Thermal Radiation to Sky Heat Transfer Coefficient [W/m2-K]
+Zone,Average,Surface Outside Face Thermal Radiation to Ground Heat Transfer Coefficient [W/m2-K]
+Zone,Average,Surface Outside Face Thermal Radiation to Air Heat Transfer Rate [W]
+Zone,Average,Surface Outside Face Heat Emission to Air Rate [W]
+Zone,Average,Surface Outside Face Solar Radiation Heat Gain Rate [W]
+Zone,Average,Surface Outside Face Solar Radiation Heat Gain Rate per Area [W/m2]
+Zone,Sum,Surface Outside Face Solar Radiation Heat Gain Energy [J]
 Zone,Average,Surface Inside Face Conduction Heat Transfer Rate [W]
 Zone,Average,Surface Inside Face Conduction Heat Gain Rate [W]
 Zone,Average,Surface Inside Face Conduction Heat Loss Rate [W]
 Zone,Average,Surface Inside Face Conduction Heat Transfer Rate per Area [W/m2]
 Zone,Sum,Surface Inside Face Conduction Heat Transfer Energy [J]
 Zone,Average,Surface Outside Face Conduction Heat Transfer Rate [W]
 Zone,Average,Surface Outside Face Conduction Heat Gain Rate [W]
@@ -263,42 +329,22 @@
 Zone,Average,Surface Heat Storage Loss Rate [W]
 Zone,Average,Surface Heat Storage Rate per Area [W/m2]
 Zone,Sum,Surface Heat Storage Energy [J]
 Zone,Average,Surface Inside Face Beam Solar Radiation Heat Gain Rate [W]
 Zone,Average,Surface Inside Face Convection Classification Index []
 Zone,Average,Surface Inside Face Convection Model Equation Index []
 Zone,Average,Surface Inside Face Convection Reference Air Index []
-Zone,Average,Surface Inside Face Heat Source Gain Rate per Area [W/m2]
-Zone,Average,Surface Outside Face Heat Source Gain Rate per Area [W/m2]
-Zone,Average,Surface Outside Face Outdoor Air Drybulb Temperature [C]
-Zone,Average,Surface Outside Face Outdoor Air Wetbulb Temperature [C]
-Zone,Average,Surface Outside Face Outdoor Air Wind Speed [m/s]
-Zone,Average,Surface Outside Face Outdoor Air Wind Direction [deg]
-Zone,Average,Surface Outside Face Convection Heat Gain Rate [W]
-Zone,Average,Surface Outside Face Convection Heat Gain Rate per Area [W/m2]
-Zone,Sum,Surface Outside Face Convection Heat Gain Energy [J]
-Zone,Average,Surface Outside Face Convection Heat Transfer Coefficient [W/m2-K]
-Zone,Average,Surface Outside Face Net Thermal Radiation Heat Gain Rate [W]
-Zone,Average,Surface Outside Face Net Thermal Radiation Heat Gain Rate per Area [W/m2]
-Zone,Sum,Surface Outside Face Net Thermal Radiation Heat Gain Energy [J]
-Zone,Average,Surface Outside Face Thermal Radiation to Air Heat Transfer Coefficient [W/m2-K]
-Zone,Average,Surface Outside Face Thermal Radiation to Sky Heat Transfer Coefficient [W/m2-K]
-Zone,Average,Surface Outside Face Thermal Radiation to Ground Heat Transfer Coefficient [W/m2-K]
-Zone,Average,Surface Outside Face Thermal Radiation to Air Heat Transfer Rate [W]
-Zone,Average,Surface Outside Face Heat Emission to Air Rate [W]
-Zone,Average,Surface Outside Face Solar Radiation Heat Gain Rate [W]
-Zone,Average,Surface Outside Face Solar Radiation Heat Gain Rate per Area [W/m2]
-Zone,Sum,Surface Outside Face Solar Radiation Heat Gain Energy [J]
 Zone,Average,Surface Outside Face Convection Classification Index []
 Zone,Average,Surface Outside Face Forced Convection Model Equation Index []
 Zone,Average,Surface Outside Face Natural Convection Model Equation Index []
+Zone,Average,Surface Inside Face Heat Source Gain Rate per Area [W/m2]
+Zone,Average,Surface Outside Face Heat Source Gain Rate per Area [W/m2]
 Zone,Average,Surface Shading Device Is On Time Fraction []
 Zone,Average,Surface Storm Window On Off Status []
 Zone,Average,Surface Window Blind Slat Angle [deg]
-Zone,Average,Zone Mean Radiant Temperature [C]
 Zone,Sum,Site Total Surface Heat Emission to Air [J]
 Zone,Average,Zone Mean Air Temperature [C]
 Zone,Average,Zone Operative Temperature [C]
 Zone,Average,Zone Mean Air Dewpoint Temperature [C]
 Zone,Average,Zone Mean Air Humidity Ratio [kgWater/kgDryAir]
 HVAC,Average,Zone Air Heat Balance Internal Convective Heat Gain Rate [W]
 HVAC,Average,Zone Air Heat Balance Surface Convection Rate [W]
@@ -311,81 +357,84 @@
 HVAC,Average,Zone Exfiltration Sensible Heat Transfer Rate [W]
 HVAC,Average,Zone Exfiltration Latent Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Sensible Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Latent Heat Transfer Rate [W]
 HVAC,Sum,Site Total Zone Exfiltration Heat Loss [J]
 HVAC,Sum,Site Total Zone Exhaust Air Heat Loss [J]
+HVAC,Sum,Infiltration Sensible Heat Loss Energy [J]
+HVAC,Sum,Infiltration Sensible Heat Gain Energy [J]
+HVAC,Sum,Infiltration Latent Heat Loss Energy [J]
+HVAC,Sum,Infiltration Latent Heat Gain Energy [J]
+HVAC,Sum,Infiltration Total Heat Loss Energy [J]
+HVAC,Sum,Infiltration Total Heat Gain Energy [J]
+HVAC,Average,Infiltration Current Density Volume Flow Rate [m3/s]
+HVAC,Average,Infiltration Standard Density Volume Flow Rate [m3/s]
+HVAC,Sum,Infiltration Current Density Volume [m3]
+HVAC,Sum,Infiltration Standard Density Volume [m3]
+HVAC,Sum,Infiltration Mass [kg]
+HVAC,Average,Infiltration Mass Flow Rate [kg/s]
+HVAC,Average,Infiltration Air Change Rate [ach]
 HVAC,Sum,Zone Infiltration Sensible Heat Loss Energy [J]
 HVAC,Sum,Zone Infiltration Sensible Heat Gain Energy [J]
 HVAC,Sum,Zone Infiltration Latent Heat Loss Energy [J]
 HVAC,Sum,Zone Infiltration Latent Heat Gain Energy [J]
 HVAC,Sum,Zone Infiltration Total Heat Loss Energy [J]
 HVAC,Sum,Zone Infiltration Total Heat Gain Energy [J]
 HVAC,Average,Zone Infiltration Current Density Volume Flow Rate [m3/s]
 HVAC,Average,Zone Infiltration Standard Density Volume Flow Rate [m3/s]
 HVAC,Sum,Zone Infiltration Current Density Volume [m3]
 HVAC,Sum,Zone Infiltration Standard Density Volume [m3]
 HVAC,Sum,Zone Infiltration Mass [kg]
 HVAC,Average,Zone Infiltration Mass Flow Rate [kg/s]
 HVAC,Average,Zone Infiltration Air Change Rate [ach]
+HVAC,Sum,Zone Ventilation Sensible Heat Loss Energy [J]
+HVAC,Sum,Zone Ventilation Sensible Heat Gain Energy [J]
+HVAC,Sum,Zone Ventilation Latent Heat Loss Energy [J]
+HVAC,Sum,Zone Ventilation Latent Heat Gain Energy [J]
+HVAC,Sum,Zone Ventilation Total Heat Loss Energy [J]
+HVAC,Sum,Zone Ventilation Total Heat Gain Energy [J]
+HVAC,Average,Zone Ventilation Current Density Volume Flow Rate [m3/s]
+HVAC,Average,Zone Ventilation Standard Density Volume Flow Rate [m3/s]
+HVAC,Sum,Zone Ventilation Current Density Volume [m3]
+HVAC,Sum,Zone Ventilation Standard Density Volume [m3]
+HVAC,Sum,Zone Ventilation Mass [kg]
+HVAC,Average,Zone Ventilation Mass Flow Rate [kg/s]
+HVAC,Average,Zone Ventilation Air Change Rate [ach]
+HVAC,Sum,Zone Ventilation Fan Electricity Energy [J]
+HVAC,Average,Zone Ventilation Air Inlet Temperature [C]
+HVAC,Average,Zone Air Temperature [C]
+HVAC,Average,Zone Air Humidity Ratio []
+HVAC,Average,Zone Air Relative Humidity [%]
 HVAC,Sum,Zone Air System Sensible Heating Energy [J]
 HVAC,Sum,Zone Air System Sensible Cooling Energy [J]
 HVAC,Average,Zone Air System Sensible Heating Rate [W]
 HVAC,Average,Zone Air System Sensible Cooling Rate [W]
-HVAC,Average,Zone Air Temperature [C]
-HVAC,Average,Zone Thermostat Air Temperature [C]
-HVAC,Average,Zone Air Humidity Ratio []
-HVAC,Average,Zone Air Relative Humidity [%]
 HVAC,Average,Zone Predicted Sensible Load to Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Sensible Load to Heating Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Sensible Load to Cooling Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Heating Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Cooling Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Moisture Load Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone Predicted Moisture Load to Humidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone Predicted Moisture Load to Dehumidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load to Humidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load to Dehumidifying Setpoint Moisture Transfer Rate [kgWater/s]
+HVAC,Average,Zone Thermostat Air Temperature [C]
 Zone,Average,Zone Thermostat Control Type []
 HVAC,Average,Zone Thermostat Heating Setpoint Temperature [C]
 HVAC,Average,Zone Thermostat Cooling Setpoint Temperature [C]
 Zone,Average,Zone Adaptive Comfort Operative Temperature Set Point [C]
 HVAC,Average,Zone Predicted Sensible Load Room Air Correction Factor []
 HVAC,Sum,HVAC System Solver Iteration Count []
 HVAC,Sum,Air System Solver Iteration Count []
 HVAC,Sum,Air System Relief Air Total Heat Loss Energy [J]
 HVAC,Sum,HVAC System Total Heat Rejection Energy [J]
-HVAC,Average,Availability Manager Night Cycle Control Status []
-HVAC,Average,Plant System Cycle On Off Status []
-HVAC,Average,Plant Supply Side Cooling Demand Rate [W]
-HVAC,Average,Plant Supply Side Heating Demand Rate [W]
-HVAC,Average,Plant Supply Side Inlet Mass Flow Rate [kg/s]
-HVAC,Average,Plant Supply Side Inlet Temperature [C]
-HVAC,Average,Plant Supply Side Outlet Temperature [C]
-HVAC,Average,Plant Supply Side Not Distributed Demand Rate [W]
-HVAC,Average,Plant Supply Side Unmet Demand Rate [W]
-HVAC,Average,Debug Plant Loop Bypass Fraction []
-HVAC,Average,Debug Plant Last Simulated Loop Side []
-HVAC,Sum,Plant Solver Sub Iteration Count []
-HVAC,Sum,Plant Solver Half Loop Calls Count []
-HVAC,Average,Transformer Efficiency []
-HVAC,Average,Transformer Input Electricity Rate [W]
-HVAC,Sum,Transformer Input Electricity Energy [J]
-HVAC,Average,Transformer Output Electricity Rate [W]
-HVAC,Sum,Transformer Output Electricity Energy [J]
-HVAC,Average,Transformer No Load Loss Rate [W]
-HVAC,Sum,Transformer No Load Loss Energy [J]
-HVAC,Average,Transformer Load Loss Rate [W]
-HVAC,Sum,Transformer Load Loss Energy [J]
-HVAC,Average,Transformer Thermal Loss Rate [W]
-HVAC,Sum,Transformer Thermal Loss Energy [J]
-HVAC,Sum,Transformer Distribution Electricity Loss Energy [J]
 HVAC,Average,Facility Total Purchased Electricity Rate [W]
 HVAC,Sum,Facility Total Purchased Electricity Energy [J]
 HVAC,Average,Facility Total Surplus Electricity Rate [W]
 HVAC,Sum,Facility Total Surplus Electricity Energy [J]
 HVAC,Average,Facility Net Purchased Electricity Rate [W]
 HVAC,Sum,Facility Net Purchased Electricity Energy [J]
 HVAC,Average,Facility Total Building Electricity Demand Rate [W]
@@ -395,20 +444,14 @@
 HVAC,Sum,Facility Total Produced Electricity Energy [J]
 HVAC,Sum,Zone Oscillating Temperatures Time [hr]
 HVAC,Sum,Zone Oscillating Temperatures During Occupancy Time [hr]
 HVAC,Sum,Zone Oscillating Temperatures in Deadband Time [hr]
 HVAC,Sum,Facility Any Zone Oscillating Temperatures Time [hr]
 HVAC,Sum,Facility Any Zone Oscillating Temperatures During Occupancy Time [hr]
 HVAC,Sum,Facility Any Zone Oscillating Temperatures in Deadband Time [hr]
-Zone,Average,Zone Thermal Comfort Fanger Model PMV []
-Zone,Average,Zone Thermal Comfort Fanger Model PPD [%]
-Zone,Average,Zone Thermal Comfort Clothing Surface Temperature [C]
-Zone,Average,Zone Thermal Comfort Mean Radiant Temperature [C]
-Zone,Average,Zone Thermal Comfort Operative Temperature [C]
-Zone,Average,Zone Thermal Comfort Clothing Value [clo]
 Zone,Sum,Zone Thermal Comfort ASHRAE 55 Simple Model Summer Clothes Not Comfortable Time [hr]
 Zone,Sum,Zone Thermal Comfort ASHRAE 55 Simple Model Winter Clothes Not Comfortable Time [hr]
 Zone,Sum,Zone Thermal Comfort ASHRAE 55 Simple Model Summer or Winter Clothes Not Comfortable Time [hr]
 Zone,Sum,Facility Thermal Comfort ASHRAE 55 Simple Model Summer Clothes Not Comfortable Time [hr]
 Zone,Sum,Facility Thermal Comfort ASHRAE 55 Simple Model Winter Clothes Not Comfortable Time [hr]
 Zone,Sum,Facility Thermal Comfort ASHRAE 55 Simple Model Summer or Winter Clothes Not Comfortable Time [hr]
 Zone,Sum,Zone Heating Setpoint Not Met Time [hr]
@@ -422,32 +465,71 @@
 Zone,Average,Zone Heat Index [C]
 Zone,Average,Zone Humidity Index []
 Zone,Average,Schedule Value []
 HVAC,Sum,Zone Air Terminal Sensible Heating Energy [J]
 HVAC,Sum,Zone Air Terminal Sensible Cooling Energy [J]
 HVAC,Average,Zone Air Terminal Sensible Heating Rate [W]
 HVAC,Average,Zone Air Terminal Sensible Cooling Rate [W]
-HVAC,Average,Zone Air Terminal VAV Damper Position []
-HVAC,Average,Zone Air Terminal Minimum Air Flow Fraction []
 HVAC,Average,Zone Air Terminal Outdoor Air Volume Flow Rate [m3/s]
+HVAC,Average,Fan Electricity Rate [W]
+HVAC,Average,Fan Rise in Air Temperature [deltaC]
+HVAC,Average,Fan Heat Gain to Air [W]
+HVAC,Sum,Fan Electricity Energy [J]
+HVAC,Average,Fan Air Mass Flow Rate [kg/s]
+HVAC,Average,Zone Unit Heater Heating Rate [W]
+HVAC,Sum,Zone Unit Heater Heating Energy [J]
+HVAC,Average,Zone Unit Heater Fan Electricity Rate [W]
+HVAC,Sum,Zone Unit Heater Fan Electricity Energy [J]
+HVAC,Average,Zone Unit Heater Fan Availability Status []
 HVAC,Sum,Heating Coil Heating Energy [J]
 HVAC,Average,Heating Coil Heating Rate [W]
-HVAC,Sum,Heating Coil Electricity Energy [J]
-HVAC,Average,Heating Coil Electricity Rate [W]
 HVAC,Sum,Heating Coil NaturalGas Energy [J]
 HVAC,Average,Heating Coil NaturalGas Rate [W]
+HVAC,Sum,Heating Coil Electricity Energy [J]
+HVAC,Average,Heating Coil Electricity Rate [W]
 HVAC,Average,Heating Coil Runtime Fraction []
 HVAC,Average,Heating Coil Ancillary NaturalGas Rate [W]
 HVAC,Sum,Heating Coil Ancillary NaturalGas Energy [J]
+HVAC,Average,Zone Radiant HVAC Heating Rate [W]
+HVAC,Sum,Zone Radiant HVAC Heating Energy [J]
+HVAC,Average,Zone Radiant HVAC NaturalGas Rate [W]
+HVAC,Sum,Zone Radiant HVAC NaturalGas Energy [J]
+HVAC,Average,Availability Manager Night Cycle Control Status []
+HVAC,Average,Unitary System Part Load Ratio []
+HVAC,Average,Unitary System Total Cooling Rate [W]
+HVAC,Average,Unitary System Sensible Cooling Rate [W]
+HVAC,Average,Unitary System Latent Cooling Rate [W]
+HVAC,Average,Unitary System Total Heating Rate [W]
+HVAC,Average,Unitary System Sensible Heating Rate [W]
+HVAC,Average,Unitary System Latent Heating Rate [W]
+HVAC,Average,Unitary System Ancillary Electricity Rate [W]
+HVAC,Sum,Unitary System Cooling Ancillary Electricity Energy [J]
+HVAC,Sum,Unitary System Heating Ancillary Electricity Energy [J]
+HVAC,Average,Unitary System Electricity Rate [W]
+HVAC,Sum,Unitary System Electricity Energy [J]
+HVAC,Average,Unitary System Predicted Sensible Load to Setpoint Heat Transfer Rate [W]
+HVAC,Average,Unitary System Predicted Moisture Load to Setpoint Heat Transfer Rate [W]
+HVAC,Average,Unitary System Dehumidification Induced Heating Demand Rate [W]
+HVAC,Average,Unitary System Fan Part Load Ratio []
+HVAC,Average,Unitary System Compressor Part Load Ratio []
+HVAC,Average,Unitary System Frost Control Status []
+HVAC,Average,Unitary System DX Coil Cycling Ratio []
+HVAC,Average,Unitary System DX Coil Speed Ratio []
+HVAC,Average,Unitary System DX Coil Speed Level []
 HVAC,Average,Air System Simulation Cycle On Off Status []
-HVAC,Average,Fan Electricity Rate [W]
-HVAC,Average,Fan Rise in Air Temperature [deltaC]
-HVAC,Average,Fan Heat Gain to Air [W]
-HVAC,Sum,Fan Electricity Energy [J]
-HVAC,Average,Fan Air Mass Flow Rate [kg/s]
+HVAC,Average,Fan Runtime Fraction []
+HVAC,Average,Cooling Coil Total Cooling Rate [W]
+HVAC,Sum,Cooling Coil Total Cooling Energy [J]
+HVAC,Average,Cooling Coil Sensible Cooling Rate [W]
+HVAC,Sum,Cooling Coil Sensible Cooling Energy [J]
+HVAC,Average,Cooling Coil Latent Cooling Rate [W]
+HVAC,Sum,Cooling Coil Latent Cooling Energy [J]
+HVAC,Average,Cooling Coil Electricity Rate [W]
+HVAC,Sum,Cooling Coil Electricity Energy [J]
+HVAC,Average,Cooling Coil Runtime Fraction []
 Zone,Average,Exterior Lights Electricity Rate [W]
 Zone,Sum,Exterior Lights Electricity Energy [J]
 HVAC,Sum,Air System Simulation Maximum Iteration Count []
 HVAC,Sum,Air System Simulation Iteration Count []
 HVAC,Sum,Air System Component Model Simulation Calls []
 HVAC,Average,Air System Outdoor Air Economizer Status []
 HVAC,Average,Air System Outdoor Air Heat Recovery Bypass Status []
@@ -458,78 +540,14 @@
 HVAC,Average,Air System Outdoor Air Flow Fraction []
 HVAC,Average,Air System Outdoor Air Minimum Flow Fraction []
 HVAC,Average,Air System Outdoor Air Mass Flow Rate [kg/s]
 HVAC,Average,Air System Mixed Air Mass Flow Rate [kg/s]
 HVAC,Average,Air System Relief Air Heat Transfer Rate [W]
 HVAC,Average,Air System Relief Air Sensible Heat Transfer Rate [W]
 HVAC,Average,Air System Relief Air Latent Heat Transfer Rate [W]
-HVAC,Average,Air System Outdoor Air Mechanical Ventilation Requested Mass Flow Rate [kg/s]
-HVAC,Average,Cooling Coil Total Cooling Rate [W]
-HVAC,Sum,Cooling Coil Total Cooling Energy [J]
-HVAC,Average,Cooling Coil Sensible Cooling Rate [W]
-HVAC,Sum,Cooling Coil Sensible Cooling Energy [J]
-HVAC,Average,Cooling Coil Latent Cooling Rate [W]
-HVAC,Sum,Cooling Coil Latent Cooling Energy [J]
-HVAC,Average,Cooling Coil Electricity Rate [W]
-HVAC,Sum,Cooling Coil Electricity Energy [J]
-HVAC,Average,Cooling Coil Runtime Fraction []
-HVAC,Average,Coil System Cycling Ratio []
-HVAC,Average,Coil System Compressor Speed Ratio []
-HVAC,Average,Coil System Frost Control Status []
-HVAC,Sum,Pump Electricity Energy [J]
-HVAC,Average,Pump Electricity Rate [W]
-HVAC,Average,Pump Shaft Power [W]
-HVAC,Average,Pump Fluid Heat Gain Rate [W]
-HVAC,Sum,Pump Fluid Heat Gain Energy [J]
-HVAC,Average,Pump Outlet Temperature [C]
-HVAC,Average,Pump Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Equipment Hot Water Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Equipment Cold Water Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Equipment Total Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Equipment Hot Water Volume Flow Rate [m3/s]
-HVAC,Average,Water Use Equipment Cold Water Volume Flow Rate [m3/s]
-HVAC,Average,Water Use Equipment Total Volume Flow Rate [m3/s]
-HVAC,Sum,Water Use Equipment Hot Water Volume [m3]
-HVAC,Sum,Water Use Equipment Cold Water Volume [m3]
-HVAC,Sum,Water Use Equipment Total Volume [m3]
-HVAC,Sum,Water Use Equipment Mains Water Volume [m3]
-HVAC,Average,Water Use Equipment Hot Water Temperature [C]
-HVAC,Average,Water Use Equipment Cold Water Temperature [C]
-HVAC,Average,Water Use Equipment Target Water Temperature [C]
-HVAC,Average,Water Use Equipment Mixed Water Temperature [C]
-HVAC,Average,Water Use Equipment Drain Water Temperature [C]
-HVAC,Average,Water Use Equipment Heating Rate [W]
-HVAC,Sum,Water Use Equipment Heating Energy [J]
-HVAC,Average,Water Use Equipment Zone Sensible Heat Gain Rate [W]
-HVAC,Sum,Water Use Equipment Zone Sensible Heat Gain Energy [J]
-HVAC,Average,Water Use Equipment Zone Latent Gain Rate [W]
-HVAC,Sum,Water Use Equipment Zone Latent Gain Energy [J]
-HVAC,Average,Water Use Equipment Zone Moisture Gain Mass Flow Rate [kg/s]
-HVAC,Sum,Water Use Equipment Zone Moisture Gain Mass [kg]
-HVAC,Average,Water Use Connections Hot Water Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Connections Cold Water Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Connections Total Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Connections Drain Water Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Connections Heat Recovery Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Connections Hot Water Volume Flow Rate [m3/s]
-HVAC,Average,Water Use Connections Cold Water Volume Flow Rate [m3/s]
-HVAC,Average,Water Use Connections Total Volume Flow Rate [m3/s]
-HVAC,Sum,Water Use Connections Hot Water Volume [m3]
-HVAC,Sum,Water Use Connections Cold Water Volume [m3]
-HVAC,Sum,Water Use Connections Total Volume [m3]
-HVAC,Average,Water Use Connections Hot Water Temperature [C]
-HVAC,Average,Water Use Connections Cold Water Temperature [C]
-HVAC,Average,Water Use Connections Drain Water Temperature [C]
-HVAC,Average,Water Use Connections Return Water Temperature [C]
-HVAC,Average,Water Use Connections Waste Water Temperature [C]
-HVAC,Average,Water Use Connections Heat Recovery Water Temperature [C]
-HVAC,Average,Water Use Connections Heat Recovery Effectiveness []
-HVAC,Average,Water Use Connections Heat Recovery Rate [W]
-HVAC,Sum,Water Use Connections Heat Recovery Energy [J]
-HVAC,Sum,Water Use Connections Plant Hot Water Energy [J]
 HVAC,Average,Water Heater Tank Temperature [C]
 HVAC,Average,Water Heater Final Tank Temperature [C]
 HVAC,Average,Water Heater Heat Loss Rate [W]
 HVAC,Sum,Water Heater Heat Loss Energy [J]
 HVAC,Average,Water Heater Use Side Mass Flow Rate [kg/s]
 HVAC,Average,Water Heater Use Side Inlet Temperature [C]
 HVAC,Average,Water Heater Use Side Outlet Temperature [C]
@@ -553,23 +571,25 @@
 HVAC,Average,Water Heater Venting Heat Transfer Rate [W]
 HVAC,Sum,Water Heater Venting Heat Transfer Energy [J]
 HVAC,Average,Water Heater Net Heat Transfer Rate [W]
 HVAC,Sum,Water Heater Net Heat Transfer Energy [J]
 HVAC,Sum,Water Heater Cycle On Count []
 HVAC,Average,Water Heater Runtime Fraction []
 HVAC,Average,Water Heater Part Load Ratio []
-HVAC,Average,Water Heater NaturalGas Rate [W]
-HVAC,Sum,Water Heater NaturalGas Energy [J]
-HVAC,Average,Water Heater Off Cycle Parasitic NaturalGas Rate [W]
-HVAC,Sum,Water Heater Off Cycle Parasitic NaturalGas Energy [J]
-HVAC,Average,Water Heater On Cycle Parasitic NaturalGas Rate [W]
-HVAC,Sum,Water Heater On Cycle Parasitic NaturalGas Energy [J]
+HVAC,Average,Water Heater Electricity Rate [W]
+HVAC,Sum,Water Heater Electricity Energy [J]
+HVAC,Average,Water Heater Off Cycle Parasitic Electricity Rate [W]
+HVAC,Sum,Water Heater Off Cycle Parasitic Electricity Energy [J]
+HVAC,Average,Water Heater On Cycle Parasitic Electricity Rate [W]
+HVAC,Sum,Water Heater On Cycle Parasitic Electricity Energy [J]
 HVAC,Average,Water Heater Water Volume Flow Rate [m3/s]
 HVAC,Sum,Water Heater Water Volume [m3]
 HVAC,Sum,Water Heater Mains Water Volume [m3]
+HVAC,Average,Cooling Coil Crankcase Heater Electricity Rate [W]
+HVAC,Sum,Cooling Coil Crankcase Heater Electricity Energy [J]
 HVAC,Average,Performance Curve Input Variable 1 Value []
 HVAC,Average,Performance Curve Input Variable 2 Value []
 HVAC,Average,Performance Curve Output Value []
 HVAC,Average,System Node Temperature [C]
 HVAC,Average,System Node Mass Flow Rate [kg/s]
 HVAC,Average,System Node Humidity Ratio [kgWater/kgDryAir]
 HVAC,Average,System Node Setpoint Temperature [C]
```

### Comparing `sinergym-2.4.1/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd` & `sinergym-2.5.0/sinergym/data/variables/ASHRAE901_OfficeMedium_STD2019_Denver.rdd`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-Program Version,EnergyPlus, Version 9.5.0-de239b2e5f, YMD=2022.05.31 14:33,
+Program Version,EnergyPlus, Version 23.1.0-87ed9199d4, YMD=2023.06.01 09:09,
 Var Type (reported time step),Var Report Type,Variable Name [Units]
 Zone,Average,Site Outdoor Air Drybulb Temperature [C]
 Zone,Average,Site Outdoor Air Dewpoint Temperature [C]
 Zone,Average,Site Outdoor Air Wetbulb Temperature [C]
 Zone,Average,Site Outdoor Air Humidity Ratio [kgWater/kgDryAir]
 Zone,Average,Site Outdoor Air Relative Humidity [%]
 Zone,Average,Site Outdoor Air Barometric Pressure [Pa]
 Zone,Average,Site Wind Speed [m/s]
 Zone,Average,Site Wind Direction [deg]
 Zone,Average,Site Sky Temperature [C]
 Zone,Average,Site Horizontal Infrared Radiation Rate per Area [W/m2]
 Zone,Average,Site Diffuse Solar Radiation Rate per Area [W/m2]
 Zone,Average,Site Direct Solar Radiation Rate per Area [W/m2]
+Zone,Sum,Liquid Precipitation Depth [m]
+Zone,Average,Site Precipitation Rate [m/s]
 Zone,Sum,Site Precipitation Depth [m]
 Zone,Average,Site Ground Reflected Solar Radiation Rate per Area [W/m2]
 Zone,Average,Site Ground Temperature [C]
 Zone,Average,Site Surface Ground Temperature [C]
 Zone,Average,Site Deep Ground Temperature [C]
 Zone,Average,Site Simple Factor Model Ground Temperature [C]
 Zone,Average,Site Total Sky Cover []
@@ -47,14 +49,24 @@
 Zone,Average,Zone Total Internal Visible Radiation Heating Rate [W]
 Zone,Sum,Zone Total Internal Convective Heating Energy [J]
 Zone,Average,Zone Total Internal Convective Heating Rate [W]
 Zone,Sum,Zone Total Internal Latent Gain Energy [J]
 Zone,Average,Zone Total Internal Latent Gain Rate [W]
 Zone,Sum,Zone Total Internal Total Heating Energy [J]
 Zone,Average,Zone Total Internal Total Heating Rate [W]
+Zone,Sum,Space Total Internal Radiant Heating Energy [J]
+Zone,Average,Space Total Internal Radiant Heating Rate [W]
+Zone,Sum,Space Total Internal Visible Radiation Heating Energy [J]
+Zone,Average,Space Total Internal Visible Radiation Heating Rate [W]
+Zone,Sum,Space Total Internal Convective Heating Energy [J]
+Zone,Average,Space Total Internal Convective Heating Rate [W]
+Zone,Sum,Space Total Internal Latent Gain Energy [J]
+Zone,Average,Space Total Internal Latent Gain Rate [W]
+Zone,Sum,Space Total Internal Total Heating Energy [J]
+Zone,Average,Space Total Internal Total Heating Rate [W]
 Zone,Average,People Occupant Count []
 Zone,Sum,People Radiant Heating Energy [J]
 Zone,Average,People Radiant Heating Rate [W]
 Zone,Sum,People Convective Heating Energy [J]
 Zone,Average,People Convective Heating Rate [W]
 Zone,Sum,People Sensible Heating Energy [J]
 Zone,Average,People Sensible Heating Rate [W]
@@ -71,14 +83,25 @@
 Zone,Average,Zone People Convective Heating Rate [W]
 Zone,Sum,Zone People Sensible Heating Energy [J]
 Zone,Average,Zone People Sensible Heating Rate [W]
 Zone,Sum,Zone People Latent Gain Energy [J]
 Zone,Average,Zone People Latent Gain Rate [W]
 Zone,Sum,Zone People Total Heating Energy [J]
 Zone,Average,Zone People Total Heating Rate [W]
+Zone,Average,Space People Occupant Count []
+Zone,Sum,Space People Radiant Heating Energy [J]
+Zone,Average,Space People Radiant Heating Rate [W]
+Zone,Sum,Space People Convective Heating Energy [J]
+Zone,Average,Space People Convective Heating Rate [W]
+Zone,Sum,Space People Sensible Heating Energy [J]
+Zone,Average,Space People Sensible Heating Rate [W]
+Zone,Sum,Space People Latent Gain Energy [J]
+Zone,Average,Space People Latent Gain Rate [W]
+Zone,Sum,Space People Total Heating Energy [J]
+Zone,Average,Space People Total Heating Rate [W]
 Zone,Average,Lights Electricity Rate [W]
 Zone,Sum,Lights Radiant Heating Energy [J]
 Zone,Average,Lights Radiant Heating Rate [W]
 Zone,Sum,Lights Visible Radiation Heating Energy [J]
 Zone,Average,Lights Visible Radiation Heating Rate [W]
 Zone,Sum,Lights Convective Heating Energy [J]
 Zone,Average,Lights Convective Heating Rate [W]
@@ -95,14 +118,26 @@
 Zone,Average,Zone Lights Visible Radiation Heating Rate [W]
 Zone,Sum,Zone Lights Convective Heating Energy [J]
 Zone,Average,Zone Lights Convective Heating Rate [W]
 Zone,Sum,Zone Lights Return Air Heating Energy [J]
 Zone,Average,Zone Lights Return Air Heating Rate [W]
 Zone,Sum,Zone Lights Total Heating Energy [J]
 Zone,Average,Zone Lights Total Heating Rate [W]
+Zone,Average,Space Lights Electricity Rate [W]
+Zone,Sum,Space Lights Electricity Energy [J]
+Zone,Sum,Space Lights Radiant Heating Energy [J]
+Zone,Average,Space Lights Radiant Heating Rate [W]
+Zone,Sum,Space Lights Visible Radiation Heating Energy [J]
+Zone,Average,Space Lights Visible Radiation Heating Rate [W]
+Zone,Sum,Space Lights Convective Heating Energy [J]
+Zone,Average,Space Lights Convective Heating Rate [W]
+Zone,Sum,Space Lights Return Air Heating Energy [J]
+Zone,Average,Space Lights Return Air Heating Rate [W]
+Zone,Sum,Space Lights Total Heating Energy [J]
+Zone,Average,Space Lights Total Heating Rate [W]
 Zone,Average,Electric Equipment Electricity Rate [W]
 Zone,Sum,Electric Equipment Electricity Energy [J]
 Zone,Sum,Electric Equipment Radiant Heating Energy [J]
 Zone,Average,Electric Equipment Radiant Heating Rate [W]
 Zone,Sum,Electric Equipment Convective Heating Energy [J]
 Zone,Average,Electric Equipment Convective Heating Rate [W]
 Zone,Sum,Electric Equipment Latent Gain Energy [J]
@@ -119,26 +154,40 @@
 Zone,Average,Zone Electric Equipment Convective Heating Rate [W]
 Zone,Sum,Zone Electric Equipment Latent Gain Energy [J]
 Zone,Average,Zone Electric Equipment Latent Gain Rate [W]
 Zone,Sum,Zone Electric Equipment Lost Heat Energy [J]
 Zone,Average,Zone Electric Equipment Lost Heat Rate [W]
 Zone,Sum,Zone Electric Equipment Total Heating Energy [J]
 Zone,Average,Zone Electric Equipment Total Heating Rate [W]
+Zone,Average,Space Electric Equipment Electricity Rate [W]
+Zone,Sum,Space Electric Equipment Electricity Energy [J]
+Zone,Sum,Space Electric Equipment Radiant Heating Energy [J]
+Zone,Average,Space Electric Equipment Radiant Heating Rate [W]
+Zone,Sum,Space Electric Equipment Convective Heating Energy [J]
+Zone,Average,Space Electric Equipment Convective Heating Rate [W]
+Zone,Sum,Space Electric Equipment Latent Gain Energy [J]
+Zone,Average,Space Electric Equipment Latent Gain Rate [W]
+Zone,Sum,Space Electric Equipment Lost Heat Energy [J]
+Zone,Average,Space Electric Equipment Lost Heat Rate [W]
+Zone,Sum,Space Electric Equipment Total Heating Energy [J]
+Zone,Average,Space Electric Equipment Total Heating Rate [W]
+Zone,Sum,Wired_LTG [J]
+Zone,Average,Zone Mean Radiant Temperature [C]
 Zone,Average,Zone Windows Total Transmitted Solar Radiation Rate [W]
 Zone,Average,Zone Exterior Windows Total Transmitted Beam Solar Radiation Rate [W]
 Zone,Average,Zone Interior Windows Total Transmitted Beam Solar Radiation Rate [W]
 Zone,Average,Zone Exterior Windows Total Transmitted Diffuse Solar Radiation Rate [W]
 Zone,Average,Zone Interior Windows Total Transmitted Diffuse Solar Radiation Rate [W]
-Zone,Average,Zone Windows Total Heat Gain Rate [W]
-Zone,Average,Zone Windows Total Heat Loss Rate [W]
 Zone,Sum,Zone Windows Total Transmitted Solar Radiation Energy [J]
 Zone,Sum,Zone Exterior Windows Total Transmitted Beam Solar Radiation Energy [J]
 Zone,Sum,Zone Interior Windows Total Transmitted Beam Solar Radiation Energy [J]
 Zone,Sum,Zone Exterior Windows Total Transmitted Diffuse Solar Radiation Energy [J]
 Zone,Sum,Zone Interior Windows Total Transmitted Diffuse Solar Radiation Energy [J]
+Zone,Average,Zone Windows Total Heat Gain Rate [W]
+Zone,Average,Zone Windows Total Heat Loss Rate [W]
 Zone,Sum,Zone Windows Total Heat Gain Energy [J]
 Zone,Sum,Zone Windows Total Heat Loss Energy [J]
 Zone,Average,Surface Outside Normal Azimuth Angle [deg]
 Zone,Average,Surface Outside Face Sunlit Area [m2]
 Zone,Average,Surface Outside Face Sunlit Fraction []
 Zone,Average,Surface Outside Face Incident Solar Radiation Rate per Area [W/m2]
 Zone,Average,Surface Outside Face Incident Beam Solar Radiation Rate per Area [W/m2]
@@ -153,15 +202,15 @@
 Zone,Average,Surface Anisotropic Sky Multiplier []
 Zone,Average,Surface Window BSDF Beam Direction Number []
 Zone,Average,Surface Window BSDF Beam Theta Angle [rad]
 Zone,Average,Surface Window BSDF Beam Phi Angle [rad]
 Zone,Average,Surface Window Total Glazing Layers Absorbed Solar Radiation Rate [W]
 Zone,Average,Surface Window Total Glazing Layers Absorbed Shortwave Radiation Rate [W]
 Zone,Average,Surface Window Front Face Temperature Layer 1 [C]
-Zone,Average,Surface Window Back Face Temperature Layer 3 [C]
+Zone,Average,Surface Window Back Face Temperature Layer 1 [C]
 Zone,Average,Surface Window Transmitted Solar Radiation Rate [W]
 Zone,Average,Surface Window Transmitted Beam Solar Radiation Rate [W]
 Zone,Average,Surface Window Transmitted Beam To Beam Solar Radiation Rate [W]
 Zone,Average,Surface Window Transmitted Beam To Diffuse Solar Radiation Rate [W]
 Zone,Average,Surface Window Transmitted Diffuse Solar Radiation Rate [W]
 Zone,Average,Surface Window Heat Gain Rate [W]
 Zone,Average,Surface Window Heat Loss Rate [W]
@@ -189,15 +238,14 @@
 Zone,Sum,Surface Window Outside Reveal Reflected Beam Solar Radiation Energy [J]
 Zone,Average,Surface Window Solar Horizontal Profile Angle [deg]
 Zone,Average,Surface Window Solar Vertical Profile Angle [deg]
 Zone,Average,Surface Window Glazing Beam to Beam Solar Transmittance []
 Zone,Average,Surface Window Glazing Beam to Diffuse Solar Transmittance []
 Zone,Average,Surface Window Glazing Diffuse to Diffuse Solar Transmittance []
 Zone,Average,Surface Window Model Solver Iteration Count []
-Zone,Average,Surface Window Back Face Temperature Layer 1 [C]
 Zone,Average,Surface Inside Face Exterior Windows Incident Beam Solar Radiation Rate per Area [W/m2]
 Zone,Average,Surface Inside Face Exterior Windows Incident Beam Solar Radiation Rate [W]
 Zone,Average,Surface Inside Face Interior Windows Incident Beam Solar Radiation Rate per Area [W/m2]
 Zone,Average,Surface Inside Face Interior Windows Incident Beam Solar Radiation Rate [W]
 Zone,Average,Surface Inside Face Initial Transmitted Diffuse Absorbed Solar Radiation Rate [W]
 Zone,Average,Surface Inside Face Initial Transmitted Diffuse Transmitted Out Window Solar Radiation Rate [W]
 Zone,Average,Surface Inside Face Absorbed Shortwave Radiation Rate [W]
@@ -239,33 +287,14 @@
 Zone,Sum,Surface Inside Face Lights Radiation Heat Gain Energy [J]
 Zone,Average,Surface Inside Face Internal Gains Radiation Heat Gain Rate [W]
 Zone,Average,Surface Inside Face Internal Gains Radiation Heat Gain Rate per Area [W/m2]
 Zone,Sum,Surface Inside Face Internal Gains Radiation Heat Gain Energy [J]
 Zone,Average,Surface Inside Face System Radiation Heat Gain Rate [W]
 Zone,Average,Surface Inside Face System Radiation Heat Gain Rate per Area [W/m2]
 Zone,Sum,Surface Inside Face System Radiation Heat Gain Energy [J]
-Zone,Average,Surface Outside Face Outdoor Air Drybulb Temperature [C]
-Zone,Average,Surface Outside Face Outdoor Air Wetbulb Temperature [C]
-Zone,Average,Surface Outside Face Outdoor Air Wind Speed [m/s]
-Zone,Average,Surface Outside Face Outdoor Air Wind Direction [deg]
-Zone,Average,Surface Outside Face Convection Heat Gain Rate [W]
-Zone,Average,Surface Outside Face Convection Heat Gain Rate per Area [W/m2]
-Zone,Sum,Surface Outside Face Convection Heat Gain Energy [J]
-Zone,Average,Surface Outside Face Convection Heat Transfer Coefficient [W/m2-K]
-Zone,Average,Surface Outside Face Net Thermal Radiation Heat Gain Rate [W]
-Zone,Average,Surface Outside Face Net Thermal Radiation Heat Gain Rate per Area [W/m2]
-Zone,Sum,Surface Outside Face Net Thermal Radiation Heat Gain Energy [J]
-Zone,Average,Surface Outside Face Thermal Radiation to Air Heat Transfer Coefficient [W/m2-K]
-Zone,Average,Surface Outside Face Thermal Radiation to Sky Heat Transfer Coefficient [W/m2-K]
-Zone,Average,Surface Outside Face Thermal Radiation to Ground Heat Transfer Coefficient [W/m2-K]
-Zone,Average,Surface Outside Face Thermal Radiation to Air Heat Transfer Rate [W]
-Zone,Average,Surface Outside Face Heat Emission to Air Rate [W]
-Zone,Average,Surface Outside Face Solar Radiation Heat Gain Rate [W]
-Zone,Average,Surface Outside Face Solar Radiation Heat Gain Rate per Area [W/m2]
-Zone,Sum,Surface Outside Face Solar Radiation Heat Gain Energy [J]
 Zone,Average,Surface Inside Face Conduction Heat Transfer Rate [W]
 Zone,Average,Surface Inside Face Conduction Heat Gain Rate [W]
 Zone,Average,Surface Inside Face Conduction Heat Loss Rate [W]
 Zone,Average,Surface Inside Face Conduction Heat Transfer Rate per Area [W/m2]
 Zone,Sum,Surface Inside Face Conduction Heat Transfer Energy [J]
 Zone,Average,Surface Outside Face Conduction Heat Transfer Rate [W]
 Zone,Average,Surface Outside Face Conduction Heat Gain Rate [W]
@@ -282,23 +311,41 @@
 Zone,Average,Surface Heat Storage Loss Rate [W]
 Zone,Average,Surface Heat Storage Rate per Area [W/m2]
 Zone,Sum,Surface Heat Storage Energy [J]
 Zone,Average,Surface Inside Face Beam Solar Radiation Heat Gain Rate [W]
 Zone,Average,Surface Inside Face Convection Classification Index []
 Zone,Average,Surface Inside Face Convection Model Equation Index []
 Zone,Average,Surface Inside Face Convection Reference Air Index []
+Zone,Average,Surface Inside Face Heat Source Gain Rate per Area [W/m2]
+Zone,Average,Surface Outside Face Heat Source Gain Rate per Area [W/m2]
+Zone,Average,Surface Outside Face Outdoor Air Drybulb Temperature [C]
+Zone,Average,Surface Outside Face Outdoor Air Wetbulb Temperature [C]
+Zone,Average,Surface Outside Face Outdoor Air Wind Speed [m/s]
+Zone,Average,Surface Outside Face Outdoor Air Wind Direction [deg]
+Zone,Average,Surface Outside Face Convection Heat Gain Rate [W]
+Zone,Average,Surface Outside Face Convection Heat Gain Rate per Area [W/m2]
+Zone,Sum,Surface Outside Face Convection Heat Gain Energy [J]
+Zone,Average,Surface Outside Face Convection Heat Transfer Coefficient [W/m2-K]
+Zone,Average,Surface Outside Face Net Thermal Radiation Heat Gain Rate [W]
+Zone,Average,Surface Outside Face Net Thermal Radiation Heat Gain Rate per Area [W/m2]
+Zone,Sum,Surface Outside Face Net Thermal Radiation Heat Gain Energy [J]
+Zone,Average,Surface Outside Face Thermal Radiation to Air Heat Transfer Coefficient [W/m2-K]
+Zone,Average,Surface Outside Face Thermal Radiation to Sky Heat Transfer Coefficient [W/m2-K]
+Zone,Average,Surface Outside Face Thermal Radiation to Ground Heat Transfer Coefficient [W/m2-K]
+Zone,Average,Surface Outside Face Thermal Radiation to Air Heat Transfer Rate [W]
+Zone,Average,Surface Outside Face Heat Emission to Air Rate [W]
+Zone,Average,Surface Outside Face Solar Radiation Heat Gain Rate [W]
+Zone,Average,Surface Outside Face Solar Radiation Heat Gain Rate per Area [W/m2]
+Zone,Sum,Surface Outside Face Solar Radiation Heat Gain Energy [J]
 Zone,Average,Surface Outside Face Convection Classification Index []
 Zone,Average,Surface Outside Face Forced Convection Model Equation Index []
 Zone,Average,Surface Outside Face Natural Convection Model Equation Index []
-Zone,Average,Surface Inside Face Heat Source Gain Rate per Area [W/m2]
-Zone,Average,Surface Outside Face Heat Source Gain Rate per Area [W/m2]
 Zone,Average,Surface Shading Device Is On Time Fraction []
 Zone,Average,Surface Storm Window On Off Status []
 Zone,Average,Surface Window Blind Slat Angle [deg]
-Zone,Average,Zone Mean Radiant Temperature [C]
 Zone,Sum,Site Total Surface Heat Emission to Air [J]
 Zone,Average,Zone Mean Air Temperature [C]
 Zone,Average,Zone Operative Temperature [C]
 Zone,Average,Zone Mean Air Dewpoint Temperature [C]
 Zone,Average,Zone Mean Air Humidity Ratio [kgWater/kgDryAir]
 HVAC,Average,Zone Air Heat Balance Internal Convective Heat Gain Rate [W]
 HVAC,Average,Zone Air Heat Balance Surface Convection Rate [W]
@@ -311,71 +358,115 @@
 HVAC,Average,Zone Exfiltration Sensible Heat Transfer Rate [W]
 HVAC,Average,Zone Exfiltration Latent Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Sensible Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Latent Heat Transfer Rate [W]
 HVAC,Sum,Site Total Zone Exfiltration Heat Loss [J]
 HVAC,Sum,Site Total Zone Exhaust Air Heat Loss [J]
+HVAC,Sum,Infiltration Sensible Heat Loss Energy [J]
+HVAC,Sum,Infiltration Sensible Heat Gain Energy [J]
+HVAC,Sum,Infiltration Latent Heat Loss Energy [J]
+HVAC,Sum,Infiltration Latent Heat Gain Energy [J]
+HVAC,Sum,Infiltration Total Heat Loss Energy [J]
+HVAC,Sum,Infiltration Total Heat Gain Energy [J]
+HVAC,Average,Infiltration Current Density Volume Flow Rate [m3/s]
+HVAC,Average,Infiltration Standard Density Volume Flow Rate [m3/s]
+HVAC,Sum,Infiltration Current Density Volume [m3]
+HVAC,Sum,Infiltration Standard Density Volume [m3]
+HVAC,Sum,Infiltration Mass [kg]
+HVAC,Average,Infiltration Mass Flow Rate [kg/s]
+HVAC,Average,Infiltration Air Change Rate [ach]
 HVAC,Sum,Zone Infiltration Sensible Heat Loss Energy [J]
 HVAC,Sum,Zone Infiltration Sensible Heat Gain Energy [J]
 HVAC,Sum,Zone Infiltration Latent Heat Loss Energy [J]
 HVAC,Sum,Zone Infiltration Latent Heat Gain Energy [J]
 HVAC,Sum,Zone Infiltration Total Heat Loss Energy [J]
 HVAC,Sum,Zone Infiltration Total Heat Gain Energy [J]
 HVAC,Average,Zone Infiltration Current Density Volume Flow Rate [m3/s]
 HVAC,Average,Zone Infiltration Standard Density Volume Flow Rate [m3/s]
 HVAC,Sum,Zone Infiltration Current Density Volume [m3]
 HVAC,Sum,Zone Infiltration Standard Density Volume [m3]
 HVAC,Sum,Zone Infiltration Mass [kg]
 HVAC,Average,Zone Infiltration Mass Flow Rate [kg/s]
 HVAC,Average,Zone Infiltration Air Change Rate [ach]
-HVAC,Sum,Zone Ventilation Sensible Heat Loss Energy [J]
-HVAC,Sum,Zone Ventilation Sensible Heat Gain Energy [J]
-HVAC,Sum,Zone Ventilation Latent Heat Loss Energy [J]
-HVAC,Sum,Zone Ventilation Latent Heat Gain Energy [J]
-HVAC,Sum,Zone Ventilation Total Heat Loss Energy [J]
-HVAC,Sum,Zone Ventilation Total Heat Gain Energy [J]
-HVAC,Average,Zone Ventilation Current Density Volume Flow Rate [m3/s]
-HVAC,Average,Zone Ventilation Standard Density Volume Flow Rate [m3/s]
-HVAC,Sum,Zone Ventilation Current Density Volume [m3]
-HVAC,Sum,Zone Ventilation Standard Density Volume [m3]
-HVAC,Sum,Zone Ventilation Mass [kg]
-HVAC,Average,Zone Ventilation Mass Flow Rate [kg/s]
-HVAC,Average,Zone Ventilation Air Change Rate [ach]
-HVAC,Sum,Zone Ventilation Fan Electricity Energy [J]
-HVAC,Average,Zone Ventilation Air Inlet Temperature [C]
+HVAC,Average,Zone Air Temperature [C]
+HVAC,Average,Zone Air Humidity Ratio []
+HVAC,Average,Zone Air Relative Humidity [%]
 HVAC,Sum,Zone Air System Sensible Heating Energy [J]
 HVAC,Sum,Zone Air System Sensible Cooling Energy [J]
 HVAC,Average,Zone Air System Sensible Heating Rate [W]
 HVAC,Average,Zone Air System Sensible Cooling Rate [W]
-HVAC,Average,Zone Air Temperature [C]
-HVAC,Average,Zone Thermostat Air Temperature [C]
-HVAC,Average,Zone Air Humidity Ratio []
-HVAC,Average,Zone Air Relative Humidity [%]
 HVAC,Average,Zone Predicted Sensible Load to Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Sensible Load to Heating Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Sensible Load to Cooling Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Heating Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Cooling Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Moisture Load Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone Predicted Moisture Load to Humidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone Predicted Moisture Load to Dehumidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load to Humidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load to Dehumidifying Setpoint Moisture Transfer Rate [kgWater/s]
+HVAC,Average,Zone Thermostat Air Temperature [C]
 Zone,Average,Zone Thermostat Control Type []
 HVAC,Average,Zone Thermostat Heating Setpoint Temperature [C]
 HVAC,Average,Zone Thermostat Cooling Setpoint Temperature [C]
 Zone,Average,Zone Adaptive Comfort Operative Temperature Set Point [C]
 HVAC,Average,Zone Predicted Sensible Load Room Air Correction Factor []
 HVAC,Sum,HVAC System Solver Iteration Count []
 HVAC,Sum,Air System Solver Iteration Count []
 HVAC,Sum,Air System Relief Air Total Heat Loss Energy [J]
 HVAC,Sum,HVAC System Total Heat Rejection Energy [J]
+HVAC,Average,Availability Manager Night Cycle Control Status []
+HVAC,Average,Plant System Cycle On Off Status []
+HVAC,Average,Water Use Connections Hot Water Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Connections Cold Water Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Connections Total Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Connections Drain Water Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Connections Heat Recovery Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Connections Hot Water Volume Flow Rate [m3/s]
+HVAC,Average,Water Use Connections Cold Water Volume Flow Rate [m3/s]
+HVAC,Average,Water Use Connections Total Volume Flow Rate [m3/s]
+HVAC,Sum,Water Use Connections Hot Water Volume [m3]
+HVAC,Sum,Water Use Connections Cold Water Volume [m3]
+HVAC,Sum,Water Use Connections Total Volume [m3]
+HVAC,Average,Water Use Connections Hot Water Temperature [C]
+HVAC,Average,Water Use Connections Cold Water Temperature [C]
+HVAC,Average,Water Use Connections Drain Water Temperature [C]
+HVAC,Average,Water Use Connections Return Water Temperature [C]
+HVAC,Average,Water Use Connections Waste Water Temperature [C]
+HVAC,Average,Water Use Connections Heat Recovery Water Temperature [C]
+HVAC,Average,Water Use Connections Heat Recovery Effectiveness []
+HVAC,Average,Water Use Connections Heat Recovery Rate [W]
+HVAC,Sum,Water Use Connections Heat Recovery Energy [J]
+HVAC,Sum,Water Use Connections Plant Hot Water Energy [J]
+HVAC,Average,Plant Supply Side Cooling Demand Rate [W]
+HVAC,Average,Plant Supply Side Heating Demand Rate [W]
+HVAC,Average,Plant Supply Side Inlet Mass Flow Rate [kg/s]
+HVAC,Average,Plant Supply Side Inlet Temperature [C]
+HVAC,Average,Plant Supply Side Outlet Temperature [C]
+HVAC,Average,Plant Supply Side Not Distributed Demand Rate [W]
+HVAC,Average,Plant Supply Side Unmet Demand Rate [W]
+HVAC,Average,Debug Plant Loop Bypass Fraction []
+HVAC,Average,Debug Plant Last Simulated Loop Side []
+HVAC,Sum,Plant Solver Sub Iteration Count []
+HVAC,Sum,Plant Solver Half Loop Calls Count []
+HVAC,Average,Transformer Efficiency []
+HVAC,Average,Transformer Input Electricity Rate [W]
+HVAC,Sum,Transformer Input Electricity Energy [J]
+HVAC,Average,Transformer Output Electricity Rate [W]
+HVAC,Sum,Transformer Output Electricity Energy [J]
+HVAC,Average,Transformer No Load Loss Rate [W]
+HVAC,Sum,Transformer No Load Loss Energy [J]
+HVAC,Average,Transformer Load Loss Rate [W]
+HVAC,Sum,Transformer Load Loss Energy [J]
+HVAC,Average,Transformer Thermal Loss Rate [W]
+HVAC,Sum,Transformer Thermal Loss Energy [J]
+HVAC,Sum,Transformer Distribution Electricity Loss Energy [J]
 HVAC,Average,Facility Total Purchased Electricity Rate [W]
 HVAC,Sum,Facility Total Purchased Electricity Energy [J]
 HVAC,Average,Facility Total Surplus Electricity Rate [W]
 HVAC,Sum,Facility Total Surplus Electricity Energy [J]
 HVAC,Average,Facility Net Purchased Electricity Rate [W]
 HVAC,Sum,Facility Net Purchased Electricity Energy [J]
 HVAC,Average,Facility Total Building Electricity Demand Rate [W]
@@ -385,14 +476,20 @@
 HVAC,Sum,Facility Total Produced Electricity Energy [J]
 HVAC,Sum,Zone Oscillating Temperatures Time [hr]
 HVAC,Sum,Zone Oscillating Temperatures During Occupancy Time [hr]
 HVAC,Sum,Zone Oscillating Temperatures in Deadband Time [hr]
 HVAC,Sum,Facility Any Zone Oscillating Temperatures Time [hr]
 HVAC,Sum,Facility Any Zone Oscillating Temperatures During Occupancy Time [hr]
 HVAC,Sum,Facility Any Zone Oscillating Temperatures in Deadband Time [hr]
+Zone,Average,Zone Thermal Comfort Fanger Model PMV []
+Zone,Average,Zone Thermal Comfort Fanger Model PPD [%]
+Zone,Average,Zone Thermal Comfort Clothing Surface Temperature [C]
+Zone,Average,Zone Thermal Comfort Mean Radiant Temperature [C]
+Zone,Average,Zone Thermal Comfort Operative Temperature [C]
+Zone,Average,Zone Thermal Comfort Clothing Value [clo]
 Zone,Sum,Zone Thermal Comfort ASHRAE 55 Simple Model Summer Clothes Not Comfortable Time [hr]
 Zone,Sum,Zone Thermal Comfort ASHRAE 55 Simple Model Winter Clothes Not Comfortable Time [hr]
 Zone,Sum,Zone Thermal Comfort ASHRAE 55 Simple Model Summer or Winter Clothes Not Comfortable Time [hr]
 Zone,Sum,Facility Thermal Comfort ASHRAE 55 Simple Model Summer Clothes Not Comfortable Time [hr]
 Zone,Sum,Facility Thermal Comfort ASHRAE 55 Simple Model Winter Clothes Not Comfortable Time [hr]
 Zone,Sum,Facility Thermal Comfort ASHRAE 55 Simple Model Summer or Winter Clothes Not Comfortable Time [hr]
 Zone,Sum,Zone Heating Setpoint Not Met Time [hr]
@@ -406,40 +503,32 @@
 Zone,Average,Zone Heat Index [C]
 Zone,Average,Zone Humidity Index []
 Zone,Average,Schedule Value []
 HVAC,Sum,Zone Air Terminal Sensible Heating Energy [J]
 HVAC,Sum,Zone Air Terminal Sensible Cooling Energy [J]
 HVAC,Average,Zone Air Terminal Sensible Heating Rate [W]
 HVAC,Average,Zone Air Terminal Sensible Cooling Rate [W]
+HVAC,Average,Zone Air Terminal VAV Damper Position []
+HVAC,Average,Zone Air Terminal Minimum Air Flow Fraction []
 HVAC,Average,Zone Air Terminal Outdoor Air Volume Flow Rate [m3/s]
-HVAC,Average,Fan Electricity Rate [W]
-HVAC,Average,Fan Rise in Air Temperature [deltaC]
-HVAC,Average,Fan Heat Gain to Air [W]
-HVAC,Sum,Fan Electricity Energy [J]
-HVAC,Average,Fan Air Mass Flow Rate [kg/s]
-HVAC,Average,Zone Unit Heater Heating Rate [W]
-HVAC,Sum,Zone Unit Heater Heating Energy [J]
-HVAC,Average,Zone Unit Heater Fan Electricity Rate [W]
-HVAC,Sum,Zone Unit Heater Fan Electricity Energy [J]
-HVAC,Average,Zone Unit Heater Fan Availability Status []
 HVAC,Sum,Heating Coil Heating Energy [J]
 HVAC,Average,Heating Coil Heating Rate [W]
-HVAC,Sum,Heating Coil NaturalGas Energy [J]
-HVAC,Average,Heating Coil NaturalGas Rate [W]
 HVAC,Sum,Heating Coil Electricity Energy [J]
 HVAC,Average,Heating Coil Electricity Rate [W]
+HVAC,Sum,Heating Coil NaturalGas Energy [J]
+HVAC,Average,Heating Coil NaturalGas Rate [W]
 HVAC,Average,Heating Coil Runtime Fraction []
 HVAC,Average,Heating Coil Ancillary NaturalGas Rate [W]
 HVAC,Sum,Heating Coil Ancillary NaturalGas Energy [J]
-HVAC,Average,Zone Radiant HVAC Heating Rate [W]
-HVAC,Sum,Zone Radiant HVAC Heating Energy [J]
-HVAC,Average,Zone Radiant HVAC NaturalGas Rate [W]
-HVAC,Sum,Zone Radiant HVAC NaturalGas Energy [J]
-HVAC,Average,Availability Manager Night Cycle Control Status []
 HVAC,Average,Air System Simulation Cycle On Off Status []
+HVAC,Average,Fan Electricity Rate [W]
+HVAC,Average,Fan Rise in Air Temperature [deltaC]
+HVAC,Average,Fan Heat Gain to Air [W]
+HVAC,Sum,Fan Electricity Energy [J]
+HVAC,Average,Fan Air Mass Flow Rate [kg/s]
 Zone,Average,Exterior Lights Electricity Rate [W]
 Zone,Sum,Exterior Lights Electricity Energy [J]
 HVAC,Sum,Air System Simulation Maximum Iteration Count []
 HVAC,Sum,Air System Simulation Iteration Count []
 HVAC,Sum,Air System Component Model Simulation Calls []
 HVAC,Average,Air System Outdoor Air Economizer Status []
 HVAC,Average,Air System Outdoor Air Heat Recovery Bypass Status []
@@ -450,26 +539,50 @@
 HVAC,Average,Air System Outdoor Air Flow Fraction []
 HVAC,Average,Air System Outdoor Air Minimum Flow Fraction []
 HVAC,Average,Air System Outdoor Air Mass Flow Rate [kg/s]
 HVAC,Average,Air System Mixed Air Mass Flow Rate [kg/s]
 HVAC,Average,Air System Relief Air Heat Transfer Rate [W]
 HVAC,Average,Air System Relief Air Sensible Heat Transfer Rate [W]
 HVAC,Average,Air System Relief Air Latent Heat Transfer Rate [W]
+HVAC,Average,Air System Outdoor Air Mechanical Ventilation Requested Mass Flow Rate [kg/s]
+HVAC,Average,Coil System Cycling Ratio []
+HVAC,Average,Coil System Compressor Speed Ratio []
+HVAC,Average,Coil System Frost Control Status []
 HVAC,Average,Cooling Coil Total Cooling Rate [W]
 HVAC,Sum,Cooling Coil Total Cooling Energy [J]
 HVAC,Average,Cooling Coil Sensible Cooling Rate [W]
 HVAC,Sum,Cooling Coil Sensible Cooling Energy [J]
 HVAC,Average,Cooling Coil Latent Cooling Rate [W]
 HVAC,Sum,Cooling Coil Latent Cooling Energy [J]
 HVAC,Average,Cooling Coil Electricity Rate [W]
 HVAC,Sum,Cooling Coil Electricity Energy [J]
 HVAC,Average,Cooling Coil Runtime Fraction []
-HVAC,Average,Coil System Cycling Ratio []
-HVAC,Average,Coil System Compressor Speed Ratio []
-HVAC,Average,Coil System Frost Control Status []
+HVAC,Average,Water Use Equipment Hot Water Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Equipment Cold Water Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Equipment Total Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Equipment Hot Water Volume Flow Rate [m3/s]
+HVAC,Average,Water Use Equipment Cold Water Volume Flow Rate [m3/s]
+HVAC,Average,Water Use Equipment Total Volume Flow Rate [m3/s]
+HVAC,Sum,Water Use Equipment Hot Water Volume [m3]
+HVAC,Sum,Water Use Equipment Cold Water Volume [m3]
+HVAC,Sum,Water Use Equipment Total Volume [m3]
+HVAC,Sum,Water Use Equipment Mains Water Volume [m3]
+HVAC,Average,Water Use Equipment Hot Water Temperature [C]
+HVAC,Average,Water Use Equipment Cold Water Temperature [C]
+HVAC,Average,Water Use Equipment Target Water Temperature [C]
+HVAC,Average,Water Use Equipment Mixed Water Temperature [C]
+HVAC,Average,Water Use Equipment Drain Water Temperature [C]
+HVAC,Average,Water Use Equipment Heating Rate [W]
+HVAC,Sum,Water Use Equipment Heating Energy [J]
+HVAC,Average,Water Use Equipment Zone Sensible Heat Gain Rate [W]
+HVAC,Sum,Water Use Equipment Zone Sensible Heat Gain Energy [J]
+HVAC,Average,Water Use Equipment Zone Latent Gain Rate [W]
+HVAC,Sum,Water Use Equipment Zone Latent Gain Energy [J]
+HVAC,Average,Water Use Equipment Zone Moisture Gain Mass Flow Rate [kg/s]
+HVAC,Sum,Water Use Equipment Zone Moisture Gain Mass [kg]
 HVAC,Average,Water Heater Tank Temperature [C]
 HVAC,Average,Water Heater Final Tank Temperature [C]
 HVAC,Average,Water Heater Heat Loss Rate [W]
 HVAC,Sum,Water Heater Heat Loss Energy [J]
 HVAC,Average,Water Heater Use Side Mass Flow Rate [kg/s]
 HVAC,Average,Water Heater Use Side Inlet Temperature [C]
 HVAC,Average,Water Heater Use Side Outlet Temperature [C]
@@ -493,23 +606,30 @@
 HVAC,Average,Water Heater Venting Heat Transfer Rate [W]
 HVAC,Sum,Water Heater Venting Heat Transfer Energy [J]
 HVAC,Average,Water Heater Net Heat Transfer Rate [W]
 HVAC,Sum,Water Heater Net Heat Transfer Energy [J]
 HVAC,Sum,Water Heater Cycle On Count []
 HVAC,Average,Water Heater Runtime Fraction []
 HVAC,Average,Water Heater Part Load Ratio []
-HVAC,Average,Water Heater Electricity Rate [W]
-HVAC,Sum,Water Heater Electricity Energy [J]
-HVAC,Average,Water Heater Off Cycle Parasitic Electricity Rate [W]
-HVAC,Sum,Water Heater Off Cycle Parasitic Electricity Energy [J]
-HVAC,Average,Water Heater On Cycle Parasitic Electricity Rate [W]
-HVAC,Sum,Water Heater On Cycle Parasitic Electricity Energy [J]
+HVAC,Average,Water Heater NaturalGas Rate [W]
+HVAC,Sum,Water Heater NaturalGas Energy [J]
+HVAC,Average,Water Heater Off Cycle Parasitic NaturalGas Rate [W]
+HVAC,Sum,Water Heater Off Cycle Parasitic NaturalGas Energy [J]
+HVAC,Average,Water Heater On Cycle Parasitic NaturalGas Rate [W]
+HVAC,Sum,Water Heater On Cycle Parasitic NaturalGas Energy [J]
 HVAC,Average,Water Heater Water Volume Flow Rate [m3/s]
 HVAC,Sum,Water Heater Water Volume [m3]
 HVAC,Sum,Water Heater Mains Water Volume [m3]
+HVAC,Sum,Pump Electricity Energy [J]
+HVAC,Average,Pump Electricity Rate [W]
+HVAC,Average,Pump Shaft Power [W]
+HVAC,Average,Pump Fluid Heat Gain Rate [W]
+HVAC,Sum,Pump Fluid Heat Gain Energy [J]
+HVAC,Average,Pump Outlet Temperature [C]
+HVAC,Average,Pump Mass Flow Rate [kg/s]
 HVAC,Average,Performance Curve Input Variable 1 Value []
 HVAC,Average,Performance Curve Input Variable 2 Value []
 HVAC,Average,Performance Curve Output Value []
 HVAC,Average,System Node Temperature [C]
 HVAC,Average,System Node Mass Flow Rate [kg/s]
 HVAC,Average,System Node Humidity Ratio [kgWater/kgDryAir]
 HVAC,Average,System Node Setpoint Temperature [C]
```

### Comparing `sinergym-2.4.1/sinergym/data/variables/OfficeGridStorageSmoothing.rdd` & `sinergym-2.5.0/sinergym/data/variables/LrgOff_GridStorageScheduled.rdd`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-Program Version,EnergyPlus, Version 9.5.0-de239b2e5f, YMD=2022.12.21 12:59,
+Program Version,EnergyPlus, Version 23.1.0-87ed9199d4, YMD=2023.06.01 08:13,
 Var Type (reported time step),Var Report Type,Variable Name [Units]
 Zone,Average,Site Outdoor Air Drybulb Temperature [C]
 Zone,Average,Site Outdoor Air Dewpoint Temperature [C]
 Zone,Average,Site Outdoor Air Wetbulb Temperature [C]
 Zone,Average,Site Outdoor Air Humidity Ratio [kgWater/kgDryAir]
 Zone,Average,Site Outdoor Air Relative Humidity [%]
 Zone,Average,Site Outdoor Air Barometric Pressure [Pa]
 Zone,Average,Site Wind Speed [m/s]
 Zone,Average,Site Wind Direction [deg]
 Zone,Average,Site Sky Temperature [C]
 Zone,Average,Site Horizontal Infrared Radiation Rate per Area [W/m2]
 Zone,Average,Site Diffuse Solar Radiation Rate per Area [W/m2]
 Zone,Average,Site Direct Solar Radiation Rate per Area [W/m2]
+Zone,Sum,Liquid Precipitation Depth [m]
+Zone,Average,Site Precipitation Rate [m/s]
 Zone,Sum,Site Precipitation Depth [m]
 Zone,Average,Site Ground Reflected Solar Radiation Rate per Area [W/m2]
 Zone,Average,Site Ground Temperature [C]
 Zone,Average,Site Surface Ground Temperature [C]
 Zone,Average,Site Deep Ground Temperature [C]
 Zone,Average,Site Simple Factor Model Ground Temperature [C]
 Zone,Average,Site Total Sky Cover []
@@ -47,14 +49,24 @@
 Zone,Average,Zone Total Internal Visible Radiation Heating Rate [W]
 Zone,Sum,Zone Total Internal Convective Heating Energy [J]
 Zone,Average,Zone Total Internal Convective Heating Rate [W]
 Zone,Sum,Zone Total Internal Latent Gain Energy [J]
 Zone,Average,Zone Total Internal Latent Gain Rate [W]
 Zone,Sum,Zone Total Internal Total Heating Energy [J]
 Zone,Average,Zone Total Internal Total Heating Rate [W]
+Zone,Sum,Space Total Internal Radiant Heating Energy [J]
+Zone,Average,Space Total Internal Radiant Heating Rate [W]
+Zone,Sum,Space Total Internal Visible Radiation Heating Energy [J]
+Zone,Average,Space Total Internal Visible Radiation Heating Rate [W]
+Zone,Sum,Space Total Internal Convective Heating Energy [J]
+Zone,Average,Space Total Internal Convective Heating Rate [W]
+Zone,Sum,Space Total Internal Latent Gain Energy [J]
+Zone,Average,Space Total Internal Latent Gain Rate [W]
+Zone,Sum,Space Total Internal Total Heating Energy [J]
+Zone,Average,Space Total Internal Total Heating Rate [W]
 Zone,Average,People Occupant Count []
 Zone,Sum,People Radiant Heating Energy [J]
 Zone,Average,People Radiant Heating Rate [W]
 Zone,Sum,People Convective Heating Energy [J]
 Zone,Average,People Convective Heating Rate [W]
 Zone,Sum,People Sensible Heating Energy [J]
 Zone,Average,People Sensible Heating Rate [W]
@@ -71,14 +83,25 @@
 Zone,Average,Zone People Convective Heating Rate [W]
 Zone,Sum,Zone People Sensible Heating Energy [J]
 Zone,Average,Zone People Sensible Heating Rate [W]
 Zone,Sum,Zone People Latent Gain Energy [J]
 Zone,Average,Zone People Latent Gain Rate [W]
 Zone,Sum,Zone People Total Heating Energy [J]
 Zone,Average,Zone People Total Heating Rate [W]
+Zone,Average,Space People Occupant Count []
+Zone,Sum,Space People Radiant Heating Energy [J]
+Zone,Average,Space People Radiant Heating Rate [W]
+Zone,Sum,Space People Convective Heating Energy [J]
+Zone,Average,Space People Convective Heating Rate [W]
+Zone,Sum,Space People Sensible Heating Energy [J]
+Zone,Average,Space People Sensible Heating Rate [W]
+Zone,Sum,Space People Latent Gain Energy [J]
+Zone,Average,Space People Latent Gain Rate [W]
+Zone,Sum,Space People Total Heating Energy [J]
+Zone,Average,Space People Total Heating Rate [W]
 Zone,Average,Lights Electricity Rate [W]
 Zone,Sum,Lights Radiant Heating Energy [J]
 Zone,Average,Lights Radiant Heating Rate [W]
 Zone,Sum,Lights Visible Radiation Heating Energy [J]
 Zone,Average,Lights Visible Radiation Heating Rate [W]
 Zone,Sum,Lights Convective Heating Energy [J]
 Zone,Average,Lights Convective Heating Rate [W]
@@ -95,14 +118,26 @@
 Zone,Average,Zone Lights Visible Radiation Heating Rate [W]
 Zone,Sum,Zone Lights Convective Heating Energy [J]
 Zone,Average,Zone Lights Convective Heating Rate [W]
 Zone,Sum,Zone Lights Return Air Heating Energy [J]
 Zone,Average,Zone Lights Return Air Heating Rate [W]
 Zone,Sum,Zone Lights Total Heating Energy [J]
 Zone,Average,Zone Lights Total Heating Rate [W]
+Zone,Average,Space Lights Electricity Rate [W]
+Zone,Sum,Space Lights Electricity Energy [J]
+Zone,Sum,Space Lights Radiant Heating Energy [J]
+Zone,Average,Space Lights Radiant Heating Rate [W]
+Zone,Sum,Space Lights Visible Radiation Heating Energy [J]
+Zone,Average,Space Lights Visible Radiation Heating Rate [W]
+Zone,Sum,Space Lights Convective Heating Energy [J]
+Zone,Average,Space Lights Convective Heating Rate [W]
+Zone,Sum,Space Lights Return Air Heating Energy [J]
+Zone,Average,Space Lights Return Air Heating Rate [W]
+Zone,Sum,Space Lights Total Heating Energy [J]
+Zone,Average,Space Lights Total Heating Rate [W]
 Zone,Average,Electric Equipment Electricity Rate [W]
 Zone,Sum,Electric Equipment Electricity Energy [J]
 Zone,Sum,Electric Equipment Radiant Heating Energy [J]
 Zone,Average,Electric Equipment Radiant Heating Rate [W]
 Zone,Sum,Electric Equipment Convective Heating Energy [J]
 Zone,Average,Electric Equipment Convective Heating Rate [W]
 Zone,Sum,Electric Equipment Latent Gain Energy [J]
@@ -119,26 +154,39 @@
 Zone,Average,Zone Electric Equipment Convective Heating Rate [W]
 Zone,Sum,Zone Electric Equipment Latent Gain Energy [J]
 Zone,Average,Zone Electric Equipment Latent Gain Rate [W]
 Zone,Sum,Zone Electric Equipment Lost Heat Energy [J]
 Zone,Average,Zone Electric Equipment Lost Heat Rate [W]
 Zone,Sum,Zone Electric Equipment Total Heating Energy [J]
 Zone,Average,Zone Electric Equipment Total Heating Rate [W]
+Zone,Average,Space Electric Equipment Electricity Rate [W]
+Zone,Sum,Space Electric Equipment Electricity Energy [J]
+Zone,Sum,Space Electric Equipment Radiant Heating Energy [J]
+Zone,Average,Space Electric Equipment Radiant Heating Rate [W]
+Zone,Sum,Space Electric Equipment Convective Heating Energy [J]
+Zone,Average,Space Electric Equipment Convective Heating Rate [W]
+Zone,Sum,Space Electric Equipment Latent Gain Energy [J]
+Zone,Average,Space Electric Equipment Latent Gain Rate [W]
+Zone,Sum,Space Electric Equipment Lost Heat Energy [J]
+Zone,Average,Space Electric Equipment Lost Heat Rate [W]
+Zone,Sum,Space Electric Equipment Total Heating Energy [J]
+Zone,Average,Space Electric Equipment Total Heating Rate [W]
+Zone,Average,Zone Mean Radiant Temperature [C]
 Zone,Average,Zone Windows Total Transmitted Solar Radiation Rate [W]
 Zone,Average,Zone Exterior Windows Total Transmitted Beam Solar Radiation Rate [W]
 Zone,Average,Zone Interior Windows Total Transmitted Beam Solar Radiation Rate [W]
 Zone,Average,Zone Exterior Windows Total Transmitted Diffuse Solar Radiation Rate [W]
 Zone,Average,Zone Interior Windows Total Transmitted Diffuse Solar Radiation Rate [W]
-Zone,Average,Zone Windows Total Heat Gain Rate [W]
-Zone,Average,Zone Windows Total Heat Loss Rate [W]
 Zone,Sum,Zone Windows Total Transmitted Solar Radiation Energy [J]
 Zone,Sum,Zone Exterior Windows Total Transmitted Beam Solar Radiation Energy [J]
 Zone,Sum,Zone Interior Windows Total Transmitted Beam Solar Radiation Energy [J]
 Zone,Sum,Zone Exterior Windows Total Transmitted Diffuse Solar Radiation Energy [J]
 Zone,Sum,Zone Interior Windows Total Transmitted Diffuse Solar Radiation Energy [J]
+Zone,Average,Zone Windows Total Heat Gain Rate [W]
+Zone,Average,Zone Windows Total Heat Loss Rate [W]
 Zone,Sum,Zone Windows Total Heat Gain Energy [J]
 Zone,Sum,Zone Windows Total Heat Loss Energy [J]
 Zone,Average,Surface Outside Normal Azimuth Angle [deg]
 Zone,Average,Surface Outside Face Sunlit Area [m2]
 Zone,Average,Surface Outside Face Sunlit Fraction []
 Zone,Average,Surface Outside Face Incident Solar Radiation Rate per Area [W/m2]
 Zone,Average,Surface Outside Face Incident Beam Solar Radiation Rate per Area [W/m2]
@@ -276,15 +324,14 @@
 Zone,Sum,Surface Outside Face Solar Radiation Heat Gain Energy [J]
 Zone,Average,Surface Outside Face Convection Classification Index []
 Zone,Average,Surface Outside Face Forced Convection Model Equation Index []
 Zone,Average,Surface Outside Face Natural Convection Model Equation Index []
 Zone,Average,Surface Shading Device Is On Time Fraction []
 Zone,Average,Surface Storm Window On Off Status []
 Zone,Average,Surface Window Blind Slat Angle [deg]
-Zone,Average,Zone Mean Radiant Temperature [C]
 Zone,Sum,Site Total Surface Heat Emission to Air [J]
 Zone,Average,Zone Mean Air Temperature [C]
 Zone,Average,Zone Operative Temperature [C]
 Zone,Average,Zone Mean Air Dewpoint Temperature [C]
 Zone,Average,Zone Mean Air Humidity Ratio [kgWater/kgDryAir]
 HVAC,Average,Zone Air Heat Balance Internal Convective Heat Gain Rate [W]
 HVAC,Average,Zone Air Heat Balance Surface Convection Rate [W]
@@ -297,58 +344,92 @@
 HVAC,Average,Zone Exfiltration Sensible Heat Transfer Rate [W]
 HVAC,Average,Zone Exfiltration Latent Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Sensible Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Latent Heat Transfer Rate [W]
 HVAC,Sum,Site Total Zone Exfiltration Heat Loss [J]
 HVAC,Sum,Site Total Zone Exhaust Air Heat Loss [J]
+HVAC,Sum,Infiltration Sensible Heat Loss Energy [J]
+HVAC,Sum,Infiltration Sensible Heat Gain Energy [J]
+HVAC,Sum,Infiltration Latent Heat Loss Energy [J]
+HVAC,Sum,Infiltration Latent Heat Gain Energy [J]
+HVAC,Sum,Infiltration Total Heat Loss Energy [J]
+HVAC,Sum,Infiltration Total Heat Gain Energy [J]
+HVAC,Average,Infiltration Current Density Volume Flow Rate [m3/s]
+HVAC,Average,Infiltration Standard Density Volume Flow Rate [m3/s]
+HVAC,Sum,Infiltration Current Density Volume [m3]
+HVAC,Sum,Infiltration Standard Density Volume [m3]
+HVAC,Sum,Infiltration Mass [kg]
+HVAC,Average,Infiltration Mass Flow Rate [kg/s]
+HVAC,Average,Infiltration Air Change Rate [ach]
 HVAC,Sum,Zone Infiltration Sensible Heat Loss Energy [J]
 HVAC,Sum,Zone Infiltration Sensible Heat Gain Energy [J]
 HVAC,Sum,Zone Infiltration Latent Heat Loss Energy [J]
 HVAC,Sum,Zone Infiltration Latent Heat Gain Energy [J]
 HVAC,Sum,Zone Infiltration Total Heat Loss Energy [J]
 HVAC,Sum,Zone Infiltration Total Heat Gain Energy [J]
 HVAC,Average,Zone Infiltration Current Density Volume Flow Rate [m3/s]
 HVAC,Average,Zone Infiltration Standard Density Volume Flow Rate [m3/s]
 HVAC,Sum,Zone Infiltration Current Density Volume [m3]
 HVAC,Sum,Zone Infiltration Standard Density Volume [m3]
 HVAC,Sum,Zone Infiltration Mass [kg]
 HVAC,Average,Zone Infiltration Mass Flow Rate [kg/s]
 HVAC,Average,Zone Infiltration Air Change Rate [ach]
+HVAC,Average,Zone Air Temperature [C]
+HVAC,Average,Zone Air Humidity Ratio []
+HVAC,Average,Zone Air Relative Humidity [%]
 HVAC,Sum,Zone Air System Sensible Heating Energy [J]
 HVAC,Sum,Zone Air System Sensible Cooling Energy [J]
 HVAC,Average,Zone Air System Sensible Heating Rate [W]
 HVAC,Average,Zone Air System Sensible Cooling Rate [W]
-HVAC,Average,Zone Air Temperature [C]
-HVAC,Average,Zone Thermostat Air Temperature [C]
-HVAC,Average,Zone Air Humidity Ratio []
-HVAC,Average,Zone Air Relative Humidity [%]
 HVAC,Average,Zone Predicted Sensible Load to Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Sensible Load to Heating Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Sensible Load to Cooling Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Heating Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Cooling Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Moisture Load Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone Predicted Moisture Load to Humidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone Predicted Moisture Load to Dehumidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load to Humidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load to Dehumidifying Setpoint Moisture Transfer Rate [kgWater/s]
+HVAC,Average,Zone Thermostat Air Temperature [C]
 Zone,Average,Zone Thermostat Control Type []
 HVAC,Average,Zone Thermostat Heating Setpoint Temperature [C]
 HVAC,Average,Zone Thermostat Cooling Setpoint Temperature [C]
 Zone,Average,Zone Adaptive Comfort Operative Temperature Set Point [C]
 HVAC,Average,Zone Predicted Sensible Load Room Air Correction Factor []
 HVAC,Sum,HVAC System Solver Iteration Count []
 HVAC,Sum,Air System Solver Iteration Count []
 HVAC,Sum,Air System Relief Air Total Heat Loss Energy [J]
 HVAC,Sum,HVAC System Total Heat Rejection Energy [J]
 HVAC,Average,Availability Manager Night Cycle Control Status []
 HVAC,Average,Plant System Cycle On Off Status []
+HVAC,Average,Water Use Connections Hot Water Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Connections Cold Water Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Connections Total Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Connections Drain Water Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Connections Heat Recovery Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Connections Hot Water Volume Flow Rate [m3/s]
+HVAC,Average,Water Use Connections Cold Water Volume Flow Rate [m3/s]
+HVAC,Average,Water Use Connections Total Volume Flow Rate [m3/s]
+HVAC,Sum,Water Use Connections Hot Water Volume [m3]
+HVAC,Sum,Water Use Connections Cold Water Volume [m3]
+HVAC,Sum,Water Use Connections Total Volume [m3]
+HVAC,Average,Water Use Connections Hot Water Temperature [C]
+HVAC,Average,Water Use Connections Cold Water Temperature [C]
+HVAC,Average,Water Use Connections Drain Water Temperature [C]
+HVAC,Average,Water Use Connections Return Water Temperature [C]
+HVAC,Average,Water Use Connections Waste Water Temperature [C]
+HVAC,Average,Water Use Connections Heat Recovery Water Temperature [C]
+HVAC,Average,Water Use Connections Heat Recovery Effectiveness []
+HVAC,Average,Water Use Connections Heat Recovery Rate [W]
+HVAC,Sum,Water Use Connections Heat Recovery Energy [J]
+HVAC,Sum,Water Use Connections Plant Hot Water Energy [J]
 HVAC,Average,Plant Supply Side Cooling Demand Rate [W]
 HVAC,Average,Plant Supply Side Heating Demand Rate [W]
 HVAC,Average,Plant Supply Side Inlet Mass Flow Rate [kg/s]
 HVAC,Average,Plant Supply Side Inlet Temperature [C]
 HVAC,Average,Plant Supply Side Outlet Temperature [C]
 HVAC,Average,Plant Supply Side Not Distributed Demand Rate [W]
 HVAC,Average,Plant Supply Side Unmet Demand Rate [W]
@@ -474,14 +555,37 @@
 HVAC,Average,Air System Outdoor Air Flow Fraction []
 HVAC,Average,Air System Outdoor Air Minimum Flow Fraction []
 HVAC,Average,Air System Outdoor Air Mass Flow Rate [kg/s]
 HVAC,Average,Air System Mixed Air Mass Flow Rate [kg/s]
 HVAC,Average,Air System Relief Air Heat Transfer Rate [W]
 HVAC,Average,Air System Relief Air Sensible Heat Transfer Rate [W]
 HVAC,Average,Air System Relief Air Latent Heat Transfer Rate [W]
+HVAC,Average,Water Use Equipment Hot Water Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Equipment Cold Water Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Equipment Total Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Equipment Hot Water Volume Flow Rate [m3/s]
+HVAC,Average,Water Use Equipment Cold Water Volume Flow Rate [m3/s]
+HVAC,Average,Water Use Equipment Total Volume Flow Rate [m3/s]
+HVAC,Sum,Water Use Equipment Hot Water Volume [m3]
+HVAC,Sum,Water Use Equipment Cold Water Volume [m3]
+HVAC,Sum,Water Use Equipment Total Volume [m3]
+HVAC,Sum,Water Use Equipment Mains Water Volume [m3]
+HVAC,Average,Water Use Equipment Hot Water Temperature [C]
+HVAC,Average,Water Use Equipment Cold Water Temperature [C]
+HVAC,Average,Water Use Equipment Target Water Temperature [C]
+HVAC,Average,Water Use Equipment Mixed Water Temperature [C]
+HVAC,Average,Water Use Equipment Drain Water Temperature [C]
+HVAC,Average,Water Use Equipment Heating Rate [W]
+HVAC,Sum,Water Use Equipment Heating Energy [J]
+HVAC,Average,Water Use Equipment Zone Sensible Heat Gain Rate [W]
+HVAC,Sum,Water Use Equipment Zone Sensible Heat Gain Energy [J]
+HVAC,Average,Water Use Equipment Zone Latent Gain Rate [W]
+HVAC,Sum,Water Use Equipment Zone Latent Gain Energy [J]
+HVAC,Average,Water Use Equipment Zone Moisture Gain Mass Flow Rate [kg/s]
+HVAC,Sum,Water Use Equipment Zone Moisture Gain Mass [kg]
 HVAC,Average,Chiller Part Load Ratio []
 HVAC,Average,Chiller Cycling Ratio []
 HVAC,Average,Chiller Electricity Rate [W]
 HVAC,Sum,Chiller Electricity Energy [J]
 HVAC,Average,Chiller Evaporator Cooling Rate [W]
 HVAC,Sum,Chiller Evaporator Cooling Energy [J]
 HVAC,Average,Chiller False Load Heat Transfer Rate [W]
@@ -505,83 +609,14 @@
 HVAC,Average,Boiler Inlet Temperature [C]
 HVAC,Average,Boiler Outlet Temperature [C]
 HVAC,Average,Boiler Mass Flow Rate [kg/s]
 HVAC,Average,Boiler Ancillary Electricity Rate [W]
 HVAC,Sum,Boiler Ancillary Electricity Energy [J]
 HVAC,Average,Boiler Part Load Ratio []
 HVAC,Average,Boiler Efficiency []
-HVAC,Average,Cooling Tower Inlet Temperature [C]
-HVAC,Average,Cooling Tower Outlet Temperature [C]
-HVAC,Average,Cooling Tower Mass Flow Rate [kg/s]
-HVAC,Average,Cooling Tower Heat Transfer Rate [W]
-HVAC,Average,Cooling Tower Fan Electricity Rate [W]
-HVAC,Sum,Cooling Tower Fan Electricity Energy [J]
-HVAC,Average,Cooling Tower Bypass Fraction []
-HVAC,Average,Cooling Tower Operating Cells Count []
-HVAC,Average,Cooling Tower Fan Cycling Ratio []
-HVAC,Average,Cooling Tower Make Up Water Volume Flow Rate [m3/s]
-HVAC,Sum,Cooling Tower Make Up Water Volume [m3]
-HVAC,Sum,Cooling Tower Make Up Mains Water Volume [m3]
-HVAC,Average,Cooling Tower Water Evaporation Volume Flow Rate [m3/s]
-HVAC,Sum,Cooling Tower Water Evaporation Volume [m3]
-HVAC,Average,Cooling Tower Water Drift Volume Flow Rate [m3/s]
-HVAC,Sum,Cooling Tower Water Drift Volume [m3]
-HVAC,Average,Cooling Tower Water Blowdown Volume Flow Rate [m3/s]
-HVAC,Sum,Cooling Tower Water Blowdown Volume [m3]
-HVAC,Sum,Pump Electricity Energy [J]
-HVAC,Average,Pump Electricity Rate [W]
-HVAC,Average,Pump Shaft Power [W]
-HVAC,Average,Pump Fluid Heat Gain Rate [W]
-HVAC,Sum,Pump Fluid Heat Gain Energy [J]
-HVAC,Average,Pump Outlet Temperature [C]
-HVAC,Average,Pump Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Equipment Hot Water Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Equipment Cold Water Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Equipment Total Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Equipment Hot Water Volume Flow Rate [m3/s]
-HVAC,Average,Water Use Equipment Cold Water Volume Flow Rate [m3/s]
-HVAC,Average,Water Use Equipment Total Volume Flow Rate [m3/s]
-HVAC,Sum,Water Use Equipment Hot Water Volume [m3]
-HVAC,Sum,Water Use Equipment Cold Water Volume [m3]
-HVAC,Sum,Water Use Equipment Total Volume [m3]
-HVAC,Sum,Water Use Equipment Mains Water Volume [m3]
-HVAC,Average,Water Use Equipment Hot Water Temperature [C]
-HVAC,Average,Water Use Equipment Cold Water Temperature [C]
-HVAC,Average,Water Use Equipment Target Water Temperature [C]
-HVAC,Average,Water Use Equipment Mixed Water Temperature [C]
-HVAC,Average,Water Use Equipment Drain Water Temperature [C]
-HVAC,Average,Water Use Equipment Heating Rate [W]
-HVAC,Sum,Water Use Equipment Heating Energy [J]
-HVAC,Average,Water Use Equipment Zone Sensible Heat Gain Rate [W]
-HVAC,Sum,Water Use Equipment Zone Sensible Heat Gain Energy [J]
-HVAC,Average,Water Use Equipment Zone Latent Gain Rate [W]
-HVAC,Sum,Water Use Equipment Zone Latent Gain Energy [J]
-HVAC,Average,Water Use Equipment Zone Moisture Gain Mass Flow Rate [kg/s]
-HVAC,Sum,Water Use Equipment Zone Moisture Gain Mass [kg]
-HVAC,Average,Water Use Connections Hot Water Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Connections Cold Water Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Connections Total Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Connections Drain Water Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Connections Heat Recovery Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Connections Hot Water Volume Flow Rate [m3/s]
-HVAC,Average,Water Use Connections Cold Water Volume Flow Rate [m3/s]
-HVAC,Average,Water Use Connections Total Volume Flow Rate [m3/s]
-HVAC,Sum,Water Use Connections Hot Water Volume [m3]
-HVAC,Sum,Water Use Connections Cold Water Volume [m3]
-HVAC,Sum,Water Use Connections Total Volume [m3]
-HVAC,Average,Water Use Connections Hot Water Temperature [C]
-HVAC,Average,Water Use Connections Cold Water Temperature [C]
-HVAC,Average,Water Use Connections Drain Water Temperature [C]
-HVAC,Average,Water Use Connections Return Water Temperature [C]
-HVAC,Average,Water Use Connections Waste Water Temperature [C]
-HVAC,Average,Water Use Connections Heat Recovery Water Temperature [C]
-HVAC,Average,Water Use Connections Heat Recovery Effectiveness []
-HVAC,Average,Water Use Connections Heat Recovery Rate [W]
-HVAC,Sum,Water Use Connections Heat Recovery Energy [J]
-HVAC,Sum,Water Use Connections Plant Hot Water Energy [J]
 HVAC,Average,Water Heater Tank Temperature [C]
 HVAC,Average,Water Heater Final Tank Temperature [C]
 HVAC,Average,Water Heater Heat Loss Rate [W]
 HVAC,Sum,Water Heater Heat Loss Energy [J]
 HVAC,Average,Water Heater Use Side Mass Flow Rate [kg/s]
 HVAC,Average,Water Heater Use Side Inlet Temperature [C]
 HVAC,Average,Water Heater Use Side Outlet Temperature [C]
@@ -614,14 +649,39 @@
 HVAC,Average,Water Heater Off Cycle Parasitic NaturalGas Rate [W]
 HVAC,Sum,Water Heater Off Cycle Parasitic NaturalGas Energy [J]
 HVAC,Average,Water Heater On Cycle Parasitic NaturalGas Rate [W]
 HVAC,Sum,Water Heater On Cycle Parasitic NaturalGas Energy [J]
 HVAC,Average,Water Heater Water Volume Flow Rate [m3/s]
 HVAC,Sum,Water Heater Water Volume [m3]
 HVAC,Sum,Water Heater Mains Water Volume [m3]
+HVAC,Average,Cooling Tower Inlet Temperature [C]
+HVAC,Average,Cooling Tower Outlet Temperature [C]
+HVAC,Average,Cooling Tower Mass Flow Rate [kg/s]
+HVAC,Average,Cooling Tower Heat Transfer Rate [W]
+HVAC,Average,Cooling Tower Fan Electricity Rate [W]
+HVAC,Sum,Cooling Tower Fan Electricity Energy [J]
+HVAC,Average,Cooling Tower Bypass Fraction []
+HVAC,Average,Cooling Tower Operating Cells Count []
+HVAC,Average,Cooling Tower Fan Cycling Ratio []
+HVAC,Average,Cooling Tower Make Up Water Volume Flow Rate [m3/s]
+HVAC,Sum,Cooling Tower Make Up Water Volume [m3]
+HVAC,Sum,Cooling Tower Make Up Mains Water Volume [m3]
+HVAC,Average,Cooling Tower Water Evaporation Volume Flow Rate [m3/s]
+HVAC,Sum,Cooling Tower Water Evaporation Volume [m3]
+HVAC,Average,Cooling Tower Water Drift Volume Flow Rate [m3/s]
+HVAC,Sum,Cooling Tower Water Drift Volume [m3]
+HVAC,Average,Cooling Tower Water Blowdown Volume Flow Rate [m3/s]
+HVAC,Sum,Cooling Tower Water Blowdown Volume [m3]
+HVAC,Sum,Pump Electricity Energy [J]
+HVAC,Average,Pump Electricity Rate [W]
+HVAC,Average,Pump Shaft Power [W]
+HVAC,Average,Pump Fluid Heat Gain Rate [W]
+HVAC,Sum,Pump Fluid Heat Gain Energy [J]
+HVAC,Average,Pump Outlet Temperature [C]
+HVAC,Average,Pump Mass Flow Rate [kg/s]
 HVAC,Average,Performance Curve Input Variable 1 Value []
 HVAC,Average,Performance Curve Input Variable 2 Value []
 HVAC,Average,Performance Curve Output Value []
 HVAC,Average,System Node Temperature [C]
 HVAC,Average,System Node Mass Flow Rate [kg/s]
 HVAC,Average,System Node Humidity Ratio [kgWater/kgDryAir]
 HVAC,Average,System Node Setpoint Temperature [C]
```

### Comparing `sinergym-2.4.1/sinergym/data/variables/ShopWithVandBattery.rdd` & `sinergym-2.5.0/sinergym/data/variables/ShopWithPVandBattery.rdd`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-Program Version,EnergyPlus, Version 9.5.0-de239b2e5f, YMD=2022.12.21 11:48,
+Program Version,EnergyPlus, Version 23.1.0-87ed9199d4, YMD=2023.06.01 08:15,
 Var Type (reported time step),Var Report Type,Variable Name [Units]
 Zone,Average,Site Outdoor Air Drybulb Temperature [C]
 Zone,Average,Site Outdoor Air Dewpoint Temperature [C]
 Zone,Average,Site Outdoor Air Wetbulb Temperature [C]
 Zone,Average,Site Outdoor Air Humidity Ratio [kgWater/kgDryAir]
 Zone,Average,Site Outdoor Air Relative Humidity [%]
 Zone,Average,Site Outdoor Air Barometric Pressure [Pa]
 Zone,Average,Site Wind Speed [m/s]
 Zone,Average,Site Wind Direction [deg]
 Zone,Average,Site Sky Temperature [C]
 Zone,Average,Site Horizontal Infrared Radiation Rate per Area [W/m2]
 Zone,Average,Site Diffuse Solar Radiation Rate per Area [W/m2]
 Zone,Average,Site Direct Solar Radiation Rate per Area [W/m2]
+Zone,Sum,Liquid Precipitation Depth [m]
+Zone,Average,Site Precipitation Rate [m/s]
 Zone,Sum,Site Precipitation Depth [m]
 Zone,Average,Site Ground Reflected Solar Radiation Rate per Area [W/m2]
 Zone,Average,Site Ground Temperature [C]
 Zone,Average,Site Surface Ground Temperature [C]
 Zone,Average,Site Deep Ground Temperature [C]
 Zone,Average,Site Simple Factor Model Ground Temperature [C]
 Zone,Average,Site Total Sky Cover []
@@ -47,14 +49,24 @@
 Zone,Average,Zone Total Internal Visible Radiation Heating Rate [W]
 Zone,Sum,Zone Total Internal Convective Heating Energy [J]
 Zone,Average,Zone Total Internal Convective Heating Rate [W]
 Zone,Sum,Zone Total Internal Latent Gain Energy [J]
 Zone,Average,Zone Total Internal Latent Gain Rate [W]
 Zone,Sum,Zone Total Internal Total Heating Energy [J]
 Zone,Average,Zone Total Internal Total Heating Rate [W]
+Zone,Sum,Space Total Internal Radiant Heating Energy [J]
+Zone,Average,Space Total Internal Radiant Heating Rate [W]
+Zone,Sum,Space Total Internal Visible Radiation Heating Energy [J]
+Zone,Average,Space Total Internal Visible Radiation Heating Rate [W]
+Zone,Sum,Space Total Internal Convective Heating Energy [J]
+Zone,Average,Space Total Internal Convective Heating Rate [W]
+Zone,Sum,Space Total Internal Latent Gain Energy [J]
+Zone,Average,Space Total Internal Latent Gain Rate [W]
+Zone,Sum,Space Total Internal Total Heating Energy [J]
+Zone,Average,Space Total Internal Total Heating Rate [W]
 Zone,Average,People Occupant Count []
 Zone,Sum,People Radiant Heating Energy [J]
 Zone,Average,People Radiant Heating Rate [W]
 Zone,Sum,People Convective Heating Energy [J]
 Zone,Average,People Convective Heating Rate [W]
 Zone,Sum,People Sensible Heating Energy [J]
 Zone,Average,People Sensible Heating Rate [W]
@@ -71,14 +83,25 @@
 Zone,Average,Zone People Convective Heating Rate [W]
 Zone,Sum,Zone People Sensible Heating Energy [J]
 Zone,Average,Zone People Sensible Heating Rate [W]
 Zone,Sum,Zone People Latent Gain Energy [J]
 Zone,Average,Zone People Latent Gain Rate [W]
 Zone,Sum,Zone People Total Heating Energy [J]
 Zone,Average,Zone People Total Heating Rate [W]
+Zone,Average,Space People Occupant Count []
+Zone,Sum,Space People Radiant Heating Energy [J]
+Zone,Average,Space People Radiant Heating Rate [W]
+Zone,Sum,Space People Convective Heating Energy [J]
+Zone,Average,Space People Convective Heating Rate [W]
+Zone,Sum,Space People Sensible Heating Energy [J]
+Zone,Average,Space People Sensible Heating Rate [W]
+Zone,Sum,Space People Latent Gain Energy [J]
+Zone,Average,Space People Latent Gain Rate [W]
+Zone,Sum,Space People Total Heating Energy [J]
+Zone,Average,Space People Total Heating Rate [W]
 Zone,Average,Lights Electricity Rate [W]
 Zone,Sum,Lights Radiant Heating Energy [J]
 Zone,Average,Lights Radiant Heating Rate [W]
 Zone,Sum,Lights Visible Radiation Heating Energy [J]
 Zone,Average,Lights Visible Radiation Heating Rate [W]
 Zone,Sum,Lights Convective Heating Energy [J]
 Zone,Average,Lights Convective Heating Rate [W]
@@ -95,14 +118,26 @@
 Zone,Average,Zone Lights Visible Radiation Heating Rate [W]
 Zone,Sum,Zone Lights Convective Heating Energy [J]
 Zone,Average,Zone Lights Convective Heating Rate [W]
 Zone,Sum,Zone Lights Return Air Heating Energy [J]
 Zone,Average,Zone Lights Return Air Heating Rate [W]
 Zone,Sum,Zone Lights Total Heating Energy [J]
 Zone,Average,Zone Lights Total Heating Rate [W]
+Zone,Average,Space Lights Electricity Rate [W]
+Zone,Sum,Space Lights Electricity Energy [J]
+Zone,Sum,Space Lights Radiant Heating Energy [J]
+Zone,Average,Space Lights Radiant Heating Rate [W]
+Zone,Sum,Space Lights Visible Radiation Heating Energy [J]
+Zone,Average,Space Lights Visible Radiation Heating Rate [W]
+Zone,Sum,Space Lights Convective Heating Energy [J]
+Zone,Average,Space Lights Convective Heating Rate [W]
+Zone,Sum,Space Lights Return Air Heating Energy [J]
+Zone,Average,Space Lights Return Air Heating Rate [W]
+Zone,Sum,Space Lights Total Heating Energy [J]
+Zone,Average,Space Lights Total Heating Rate [W]
 Zone,Average,Electric Equipment Electricity Rate [W]
 Zone,Sum,Electric Equipment Electricity Energy [J]
 Zone,Sum,Electric Equipment Radiant Heating Energy [J]
 Zone,Average,Electric Equipment Radiant Heating Rate [W]
 Zone,Sum,Electric Equipment Convective Heating Energy [J]
 Zone,Average,Electric Equipment Convective Heating Rate [W]
 Zone,Sum,Electric Equipment Latent Gain Energy [J]
@@ -119,14 +154,26 @@
 Zone,Average,Zone Electric Equipment Convective Heating Rate [W]
 Zone,Sum,Zone Electric Equipment Latent Gain Energy [J]
 Zone,Average,Zone Electric Equipment Latent Gain Rate [W]
 Zone,Sum,Zone Electric Equipment Lost Heat Energy [J]
 Zone,Average,Zone Electric Equipment Lost Heat Rate [W]
 Zone,Sum,Zone Electric Equipment Total Heating Energy [J]
 Zone,Average,Zone Electric Equipment Total Heating Rate [W]
+Zone,Average,Space Electric Equipment Electricity Rate [W]
+Zone,Sum,Space Electric Equipment Electricity Energy [J]
+Zone,Sum,Space Electric Equipment Radiant Heating Energy [J]
+Zone,Average,Space Electric Equipment Radiant Heating Rate [W]
+Zone,Sum,Space Electric Equipment Convective Heating Energy [J]
+Zone,Average,Space Electric Equipment Convective Heating Rate [W]
+Zone,Sum,Space Electric Equipment Latent Gain Energy [J]
+Zone,Average,Space Electric Equipment Latent Gain Rate [W]
+Zone,Sum,Space Electric Equipment Lost Heat Energy [J]
+Zone,Average,Space Electric Equipment Lost Heat Rate [W]
+Zone,Sum,Space Electric Equipment Total Heating Energy [J]
+Zone,Average,Space Electric Equipment Total Heating Rate [W]
 Zone,Average,Gas Equipment NaturalGas Rate [W]
 Zone,Sum,Gas Equipment NaturalGas Energy [J]
 Zone,Sum,Gas Equipment Radiant Heating Energy [J]
 Zone,Sum,Gas Equipment Convective Heating Energy [J]
 Zone,Sum,Gas Equipment Latent Gain Energy [J]
 Zone,Sum,Gas Equipment Lost Heat Energy [J]
 Zone,Sum,Gas Equipment Total Heating Energy [J]
@@ -143,26 +190,39 @@
 Zone,Average,Zone Gas Equipment Convective Heating Rate [W]
 Zone,Sum,Zone Gas Equipment Latent Gain Energy [J]
 Zone,Average,Zone Gas Equipment Latent Gain Rate [W]
 Zone,Sum,Zone Gas Equipment Lost Heat Energy [J]
 Zone,Average,Zone Gas Equipment Lost Heat Rate [W]
 Zone,Sum,Zone Gas Equipment Total Heating Energy [J]
 Zone,Average,Zone Gas Equipment Total Heating Rate [W]
+Zone,Average,Space Gas Equipment NaturalGas Rate [W]
+Zone,Sum,Space Gas Equipment NaturalGas Energy [J]
+Zone,Sum,Space Gas Equipment Radiant Heating Energy [J]
+Zone,Average,Space Gas Equipment Radiant Heating Rate [W]
+Zone,Sum,Space Gas Equipment Convective Heating Energy [J]
+Zone,Average,Space Gas Equipment Convective Heating Rate [W]
+Zone,Sum,Space Gas Equipment Latent Gain Energy [J]
+Zone,Average,Space Gas Equipment Latent Gain Rate [W]
+Zone,Sum,Space Gas Equipment Lost Heat Energy [J]
+Zone,Average,Space Gas Equipment Lost Heat Rate [W]
+Zone,Sum,Space Gas Equipment Total Heating Energy [J]
+Zone,Average,Space Gas Equipment Total Heating Rate [W]
+Zone,Average,Zone Mean Radiant Temperature [C]
 Zone,Average,Zone Windows Total Transmitted Solar Radiation Rate [W]
 Zone,Average,Zone Exterior Windows Total Transmitted Beam Solar Radiation Rate [W]
 Zone,Average,Zone Interior Windows Total Transmitted Beam Solar Radiation Rate [W]
 Zone,Average,Zone Exterior Windows Total Transmitted Diffuse Solar Radiation Rate [W]
 Zone,Average,Zone Interior Windows Total Transmitted Diffuse Solar Radiation Rate [W]
-Zone,Average,Zone Windows Total Heat Gain Rate [W]
-Zone,Average,Zone Windows Total Heat Loss Rate [W]
 Zone,Sum,Zone Windows Total Transmitted Solar Radiation Energy [J]
 Zone,Sum,Zone Exterior Windows Total Transmitted Beam Solar Radiation Energy [J]
 Zone,Sum,Zone Interior Windows Total Transmitted Beam Solar Radiation Energy [J]
 Zone,Sum,Zone Exterior Windows Total Transmitted Diffuse Solar Radiation Energy [J]
 Zone,Sum,Zone Interior Windows Total Transmitted Diffuse Solar Radiation Energy [J]
+Zone,Average,Zone Windows Total Heat Gain Rate [W]
+Zone,Average,Zone Windows Total Heat Loss Rate [W]
 Zone,Sum,Zone Windows Total Heat Gain Energy [J]
 Zone,Sum,Zone Windows Total Heat Loss Energy [J]
 Zone,Average,Surface Outside Normal Azimuth Angle [deg]
 Zone,Average,Surface Outside Face Sunlit Area [m2]
 Zone,Average,Surface Outside Face Sunlit Fraction []
 Zone,Average,Surface Outside Face Incident Solar Radiation Rate per Area [W/m2]
 Zone,Average,Surface Outside Face Incident Beam Solar Radiation Rate per Area [W/m2]
@@ -300,15 +360,14 @@
 Zone,Average,Surface Outside Face Forced Convection Model Equation Index []
 Zone,Average,Surface Outside Face Natural Convection Model Equation Index []
 Zone,Average,Surface Inside Face Heat Source Gain Rate per Area [W/m2]
 Zone,Average,Surface Outside Face Heat Source Gain Rate per Area [W/m2]
 Zone,Average,Surface Shading Device Is On Time Fraction []
 Zone,Average,Surface Storm Window On Off Status []
 Zone,Average,Surface Window Blind Slat Angle [deg]
-Zone,Average,Zone Mean Radiant Temperature [C]
 Zone,Sum,Site Total Surface Heat Emission to Air [J]
 Zone,Average,Zone Mean Air Temperature [C]
 Zone,Average,Zone Operative Temperature [C]
 Zone,Average,Zone Mean Air Dewpoint Temperature [C]
 Zone,Average,Zone Mean Air Humidity Ratio [kgWater/kgDryAir]
 HVAC,Average,Zone Air Heat Balance Internal Convective Heat Gain Rate [W]
 HVAC,Average,Zone Air Heat Balance Surface Convection Rate [W]
@@ -321,58 +380,92 @@
 HVAC,Average,Zone Exfiltration Sensible Heat Transfer Rate [W]
 HVAC,Average,Zone Exfiltration Latent Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Sensible Heat Transfer Rate [W]
 HVAC,Average,Zone Exhaust Air Latent Heat Transfer Rate [W]
 HVAC,Sum,Site Total Zone Exfiltration Heat Loss [J]
 HVAC,Sum,Site Total Zone Exhaust Air Heat Loss [J]
+HVAC,Sum,Infiltration Sensible Heat Loss Energy [J]
+HVAC,Sum,Infiltration Sensible Heat Gain Energy [J]
+HVAC,Sum,Infiltration Latent Heat Loss Energy [J]
+HVAC,Sum,Infiltration Latent Heat Gain Energy [J]
+HVAC,Sum,Infiltration Total Heat Loss Energy [J]
+HVAC,Sum,Infiltration Total Heat Gain Energy [J]
+HVAC,Average,Infiltration Current Density Volume Flow Rate [m3/s]
+HVAC,Average,Infiltration Standard Density Volume Flow Rate [m3/s]
+HVAC,Sum,Infiltration Current Density Volume [m3]
+HVAC,Sum,Infiltration Standard Density Volume [m3]
+HVAC,Sum,Infiltration Mass [kg]
+HVAC,Average,Infiltration Mass Flow Rate [kg/s]
+HVAC,Average,Infiltration Air Change Rate [ach]
 HVAC,Sum,Zone Infiltration Sensible Heat Loss Energy [J]
 HVAC,Sum,Zone Infiltration Sensible Heat Gain Energy [J]
 HVAC,Sum,Zone Infiltration Latent Heat Loss Energy [J]
 HVAC,Sum,Zone Infiltration Latent Heat Gain Energy [J]
 HVAC,Sum,Zone Infiltration Total Heat Loss Energy [J]
 HVAC,Sum,Zone Infiltration Total Heat Gain Energy [J]
 HVAC,Average,Zone Infiltration Current Density Volume Flow Rate [m3/s]
 HVAC,Average,Zone Infiltration Standard Density Volume Flow Rate [m3/s]
 HVAC,Sum,Zone Infiltration Current Density Volume [m3]
 HVAC,Sum,Zone Infiltration Standard Density Volume [m3]
 HVAC,Sum,Zone Infiltration Mass [kg]
 HVAC,Average,Zone Infiltration Mass Flow Rate [kg/s]
 HVAC,Average,Zone Infiltration Air Change Rate [ach]
+HVAC,Average,Zone Air Temperature [C]
+HVAC,Average,Zone Air Humidity Ratio []
+HVAC,Average,Zone Air Relative Humidity [%]
 HVAC,Sum,Zone Air System Sensible Heating Energy [J]
 HVAC,Sum,Zone Air System Sensible Cooling Energy [J]
 HVAC,Average,Zone Air System Sensible Heating Rate [W]
 HVAC,Average,Zone Air System Sensible Cooling Rate [W]
-HVAC,Average,Zone Air Temperature [C]
-HVAC,Average,Zone Thermostat Air Temperature [C]
-HVAC,Average,Zone Air Humidity Ratio []
-HVAC,Average,Zone Air Relative Humidity [%]
 HVAC,Average,Zone Predicted Sensible Load to Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Sensible Load to Heating Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Sensible Load to Cooling Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Heating Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone System Predicted Sensible Load to Cooling Setpoint Heat Transfer Rate [W]
 HVAC,Average,Zone Predicted Moisture Load Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone Predicted Moisture Load to Humidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone Predicted Moisture Load to Dehumidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load to Humidifying Setpoint Moisture Transfer Rate [kgWater/s]
 HVAC,Average,Zone System Predicted Moisture Load to Dehumidifying Setpoint Moisture Transfer Rate [kgWater/s]
+HVAC,Average,Zone Thermostat Air Temperature [C]
 Zone,Average,Zone Thermostat Control Type []
 HVAC,Average,Zone Thermostat Heating Setpoint Temperature [C]
 HVAC,Average,Zone Thermostat Cooling Setpoint Temperature [C]
 Zone,Average,Zone Adaptive Comfort Operative Temperature Set Point [C]
 HVAC,Average,Zone Predicted Sensible Load Room Air Correction Factor []
 HVAC,Sum,HVAC System Solver Iteration Count []
 HVAC,Sum,Air System Solver Iteration Count []
 HVAC,Sum,Air System Relief Air Total Heat Loss Energy [J]
 HVAC,Sum,HVAC System Total Heat Rejection Energy [J]
 HVAC,Average,Availability Manager Night Cycle Control Status []
 HVAC,Average,Plant System Cycle On Off Status []
+HVAC,Average,Water Use Connections Hot Water Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Connections Cold Water Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Connections Total Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Connections Drain Water Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Connections Heat Recovery Mass Flow Rate [kg/s]
+HVAC,Average,Water Use Connections Hot Water Volume Flow Rate [m3/s]
+HVAC,Average,Water Use Connections Cold Water Volume Flow Rate [m3/s]
+HVAC,Average,Water Use Connections Total Volume Flow Rate [m3/s]
+HVAC,Sum,Water Use Connections Hot Water Volume [m3]
+HVAC,Sum,Water Use Connections Cold Water Volume [m3]
+HVAC,Sum,Water Use Connections Total Volume [m3]
+HVAC,Average,Water Use Connections Hot Water Temperature [C]
+HVAC,Average,Water Use Connections Cold Water Temperature [C]
+HVAC,Average,Water Use Connections Drain Water Temperature [C]
+HVAC,Average,Water Use Connections Return Water Temperature [C]
+HVAC,Average,Water Use Connections Waste Water Temperature [C]
+HVAC,Average,Water Use Connections Heat Recovery Water Temperature [C]
+HVAC,Average,Water Use Connections Heat Recovery Effectiveness []
+HVAC,Average,Water Use Connections Heat Recovery Rate [W]
+HVAC,Sum,Water Use Connections Heat Recovery Energy [J]
+HVAC,Sum,Water Use Connections Plant Hot Water Energy [J]
 HVAC,Average,Plant Supply Side Cooling Demand Rate [W]
 HVAC,Average,Plant Supply Side Heating Demand Rate [W]
 HVAC,Average,Plant Supply Side Inlet Mass Flow Rate [kg/s]
 HVAC,Average,Plant Supply Side Inlet Temperature [C]
 HVAC,Average,Plant Supply Side Outlet Temperature [C]
 HVAC,Average,Plant Supply Side Not Distributed Demand Rate [W]
 HVAC,Average,Plant Supply Side Unmet Demand Rate [W]
@@ -483,36 +576,29 @@
 HVAC,Average,Air System Outdoor Air Flow Fraction []
 HVAC,Average,Air System Outdoor Air Minimum Flow Fraction []
 HVAC,Average,Air System Outdoor Air Mass Flow Rate [kg/s]
 HVAC,Average,Air System Mixed Air Mass Flow Rate [kg/s]
 HVAC,Average,Air System Relief Air Heat Transfer Rate [W]
 HVAC,Average,Air System Relief Air Sensible Heat Transfer Rate [W]
 HVAC,Average,Air System Relief Air Latent Heat Transfer Rate [W]
+HVAC,Average,Coil System Part Load Ratio []
+HVAC,Average,Coil System Frost Control Status []
 HVAC,Average,Cooling Coil Total Cooling Rate [W]
 HVAC,Sum,Cooling Coil Total Cooling Energy [J]
 HVAC,Average,Cooling Coil Sensible Cooling Rate [W]
 HVAC,Sum,Cooling Coil Sensible Cooling Energy [J]
 HVAC,Average,Cooling Coil Latent Cooling Rate [W]
 HVAC,Sum,Cooling Coil Latent Cooling Energy [J]
 HVAC,Average,Cooling Coil Electricity Rate [W]
 HVAC,Sum,Cooling Coil Electricity Energy [J]
 HVAC,Average,Cooling Coil Runtime Fraction []
-HVAC,Average,Coil System Part Load Ratio []
-HVAC,Average,Coil System Frost Control Status []
 HVAC,Sum,Heating Coil Heating Energy [J]
 HVAC,Average,Heating Coil Heating Rate [W]
 HVAC,Sum,Heating Coil Electricity Energy [J]
 HVAC,Average,Heating Coil Electricity Rate [W]
-HVAC,Sum,Pump Electricity Energy [J]
-HVAC,Average,Pump Electricity Rate [W]
-HVAC,Average,Pump Shaft Power [W]
-HVAC,Average,Pump Fluid Heat Gain Rate [W]
-HVAC,Sum,Pump Fluid Heat Gain Energy [J]
-HVAC,Average,Pump Outlet Temperature [C]
-HVAC,Average,Pump Mass Flow Rate [kg/s]
 HVAC,Average,Water Use Equipment Hot Water Mass Flow Rate [kg/s]
 HVAC,Average,Water Use Equipment Cold Water Mass Flow Rate [kg/s]
 HVAC,Average,Water Use Equipment Total Mass Flow Rate [kg/s]
 HVAC,Average,Water Use Equipment Hot Water Volume Flow Rate [m3/s]
 HVAC,Average,Water Use Equipment Cold Water Volume Flow Rate [m3/s]
 HVAC,Average,Water Use Equipment Total Volume Flow Rate [m3/s]
 HVAC,Sum,Water Use Equipment Hot Water Volume [m3]
@@ -528,35 +614,14 @@
 HVAC,Sum,Water Use Equipment Heating Energy [J]
 HVAC,Average,Water Use Equipment Zone Sensible Heat Gain Rate [W]
 HVAC,Sum,Water Use Equipment Zone Sensible Heat Gain Energy [J]
 HVAC,Average,Water Use Equipment Zone Latent Gain Rate [W]
 HVAC,Sum,Water Use Equipment Zone Latent Gain Energy [J]
 HVAC,Average,Water Use Equipment Zone Moisture Gain Mass Flow Rate [kg/s]
 HVAC,Sum,Water Use Equipment Zone Moisture Gain Mass [kg]
-HVAC,Average,Water Use Connections Hot Water Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Connections Cold Water Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Connections Total Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Connections Drain Water Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Connections Heat Recovery Mass Flow Rate [kg/s]
-HVAC,Average,Water Use Connections Hot Water Volume Flow Rate [m3/s]
-HVAC,Average,Water Use Connections Cold Water Volume Flow Rate [m3/s]
-HVAC,Average,Water Use Connections Total Volume Flow Rate [m3/s]
-HVAC,Sum,Water Use Connections Hot Water Volume [m3]
-HVAC,Sum,Water Use Connections Cold Water Volume [m3]
-HVAC,Sum,Water Use Connections Total Volume [m3]
-HVAC,Average,Water Use Connections Hot Water Temperature [C]
-HVAC,Average,Water Use Connections Cold Water Temperature [C]
-HVAC,Average,Water Use Connections Drain Water Temperature [C]
-HVAC,Average,Water Use Connections Return Water Temperature [C]
-HVAC,Average,Water Use Connections Waste Water Temperature [C]
-HVAC,Average,Water Use Connections Heat Recovery Water Temperature [C]
-HVAC,Average,Water Use Connections Heat Recovery Effectiveness []
-HVAC,Average,Water Use Connections Heat Recovery Rate [W]
-HVAC,Sum,Water Use Connections Heat Recovery Energy [J]
-HVAC,Sum,Water Use Connections Plant Hot Water Energy [J]
 HVAC,Average,Water Heater Tank Temperature [C]
 HVAC,Average,Water Heater Final Tank Temperature [C]
 HVAC,Average,Water Heater Heat Loss Rate [W]
 HVAC,Sum,Water Heater Heat Loss Energy [J]
 HVAC,Average,Water Heater Use Side Mass Flow Rate [kg/s]
 HVAC,Average,Water Heater Use Side Inlet Temperature [C]
 HVAC,Average,Water Heater Use Side Outlet Temperature [C]
@@ -589,14 +654,21 @@
 HVAC,Average,Water Heater Off Cycle Parasitic Electricity Rate [W]
 HVAC,Sum,Water Heater Off Cycle Parasitic Electricity Energy [J]
 HVAC,Average,Water Heater On Cycle Parasitic Electricity Rate [W]
 HVAC,Sum,Water Heater On Cycle Parasitic Electricity Energy [J]
 HVAC,Average,Water Heater Water Volume Flow Rate [m3/s]
 HVAC,Sum,Water Heater Water Volume [m3]
 HVAC,Sum,Water Heater Mains Water Volume [m3]
+HVAC,Sum,Pump Electricity Energy [J]
+HVAC,Average,Pump Electricity Rate [W]
+HVAC,Average,Pump Shaft Power [W]
+HVAC,Average,Pump Fluid Heat Gain Rate [W]
+HVAC,Sum,Pump Fluid Heat Gain Energy [J]
+HVAC,Average,Pump Outlet Temperature [C]
+HVAC,Average,Pump Mass Flow Rate [kg/s]
 HVAC,Average,Cooling Coil Crankcase Heater Electricity Rate [W]
 HVAC,Sum,Cooling Coil Crankcase Heater Electricity Energy [J]
 HVAC,Average,Performance Curve Input Variable 1 Value []
 HVAC,Average,Performance Curve Input Variable 2 Value []
 HVAC,Average,Performance Curve Output Value []
 HVAC,Average,System Node Temperature [C]
 HVAC,Average,System Node Mass Flow Rate [kg/s]
```

### Comparing `sinergym-2.4.1/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy` & `sinergym-2.5.0/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw` & `sinergym-2.5.0/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy` & `sinergym-2.5.0/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/COL_Bogota.802220_IWEC.epw` & `sinergym-2.5.0/sinergym/data/weather/COL_Bogota.802220_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy` & `sinergym-2.5.0/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/ESP_Granada.084190_SWEC.epw` & `sinergym-2.5.0/sinergym/data/weather/ESP_Granada.084190_SWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy` & `sinergym-2.5.0/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw` & `sinergym-2.5.0/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy` & `sinergym-2.5.0/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw` & `sinergym-2.5.0/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy` & `sinergym-2.5.0/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw` & `sinergym-2.5.0/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy` & `sinergym-2.5.0/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw` & `sinergym-2.5.0/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy` & `sinergym-2.5.0/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw` & `sinergym-2.5.0/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy` & `sinergym-2.5.0/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw` & `sinergym-2.5.0/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy` & `sinergym-2.5.0/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw` & `sinergym-2.5.0/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy` & `sinergym-2.5.0/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw` & `sinergym-2.5.0/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy` & `sinergym-2.5.0/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw` & `sinergym-2.5.0/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy` & `sinergym-2.5.0/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw` & `sinergym-2.5.0/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/envs/eplus_env.py` & `sinergym-2.5.0/sinergym/envs/eplus_env.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/simulators/base.py` & `sinergym-2.5.0/sinergym/simulators/base.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/simulators/eplus.py` & `sinergym-2.5.0/sinergym/simulators/eplus.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/simulators/eplus_alpha.py` & `sinergym-2.5.0/sinergym/simulators/eplus_alpha.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/utils/callbacks.py` & `sinergym-2.5.0/sinergym/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/utils/common.py` & `sinergym-2.5.0/sinergym/utils/common.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/utils/constants.py` & `sinergym-2.5.0/sinergym/utils/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,14 @@
                 'Site Wind Speed(Environment)': [0.0, 23.1],
                 'Space1-ClgSetP-RL': [21.0, 30.0],
                 'Space1-HtgSetP-RL': [15.0, 22.49999],
                 'Zone Air Relative Humidity(SPACE1-1)': [3.287277410867238,
                                                          87.60662171287048],
                 'Zone Air Temperature(SPACE1-1)': [15.22565264653451, 30.00826655379267],
                 'Zone People Occupant Count(SPACE1-1)': [0.0, 11.0],
-                'Zone Thermal Comfort Clothing Value(SPACE1-1 PEOPLE 1)': [0.0, 1.0],
-                'Zone Thermal Comfort Fanger Model PPD(SPACE1-1 PEOPLE 1)': [0.0,
-                                                                             98.37141259444684],
-                'Zone Thermal Comfort Mean Radiant Temperature(SPACE1-1 PEOPLE 1)': [0.0,
-                                                                                     35.98853496778508],
                 'Zone Thermostat Cooling Setpoint Temperature(SPACE1-1)': [21.0, 30.0],
                 'Zone Thermostat Heating Setpoint Temperature(SPACE1-1)': [15.0,
                                                                            22.49999046325684],
                 'comfort_penalty': [-6.508266553792669, -0.0],
                 'day': [1, 31],
                 'done': [False, True],
                 'hour': [0, 23],
@@ -338,18 +333,15 @@
     'Site Wind Speed(Environment)',
     'Site Wind Direction(Environment)',
     'Site Diffuse Solar Radiation Rate per Area(Environment)',
     'Site Direct Solar Radiation Rate per Area(Environment)',
     'Zone Thermostat Heating Setpoint Temperature(SPACE1-1)',
     'Zone Thermostat Cooling Setpoint Temperature(SPACE1-1)',
     'Zone Air Temperature(SPACE1-1)',
-    'Zone Thermal Comfort Mean Radiant Temperature(SPACE1-1 PEOPLE 1)',
     'Zone Air Relative Humidity(SPACE1-1)',
-    'Zone Thermal Comfort Clothing Value(SPACE1-1 PEOPLE 1)',
-    'Zone Thermal Comfort Fanger Model PPD(SPACE1-1 PEOPLE 1)',
     'Zone People Occupant Count(SPACE1-1)',
     'People Air Temperature(SPACE1-1 PEOPLE 1)',
     'Facility Total HVAC Electricity Demand Rate(Whole Building)'
 ]
 
 DEFAULT_5ZONE_ACTION_VARIABLES = [
     'Heating_Setpoint_RL',
```

### Comparing `sinergym-2.4.1/sinergym/utils/controllers.py` & `sinergym-2.5.0/sinergym/utils/controllers.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/utils/env_checker.py` & `sinergym-2.5.0/sinergym/utils/env_checker.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/utils/evaluation.py` & `sinergym-2.5.0/sinergym/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/utils/gcloud.py` & `sinergym-2.5.0/sinergym/utils/gcloud.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/utils/logger.py` & `sinergym-2.5.0/sinergym/utils/logger.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/utils/rewards.py` & `sinergym-2.5.0/sinergym/utils/rewards.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym/utils/wrappers.py` & `sinergym-2.5.0/sinergym/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.4.1/sinergym.egg-info/PKG-INFO` & `sinergym-2.5.0/sinergym.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinergym
-Version: 2.4.1
+Version: 2.5.0
 Summary: The goal of sinergym is to create an environment following OpenAI Gym interface for wrapping simulation engines for building control using deep reinforcement learning.
 Home-page: https://github.com/ugr-sail/sinergym
 Author: J. Jiménez, J. Gómez, M. Molina, A. Manjavacas, A. Campoy
 Author-email: alejandroac79@gmail.com
 License: MIT
 Keywords: control reinforcement-learning buildings reinforcement-learning-environments
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sinergym Version: 2.4.1 Summary: The goal of
+Metadata-Version: 2.1 Name: sinergym Version: 2.5.0 Summary: The goal of
 sinergym is to create an environment following OpenAI Gym interface for
 wrapping simulation engines for building control using deep reinforcement
 learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
 J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
 alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
 buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
```

### Comparing `sinergym-2.4.1/sinergym.egg-info/SOURCES.txt` & `sinergym-2.5.0/sinergym.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 sinergym.egg-info/dependency_links.txt
 sinergym.egg-info/requires.txt
 sinergym.egg-info/top_level.txt
 sinergym/config/__init__.py
 sinergym/config/modeling.py
 sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON
 sinergym/data/buildings/5ZoneAutoDXVAV.epJSON
-sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.epJSON
-sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.epJSON
-sinergym/data/buildings/OfficeGridStorageSmoothing.epJSON
-sinergym/data/buildings/ShopWithVandBattery.epJSON
+sinergym/data/buildings/ASHRAE901_OfficeMedium_STD2019_Denver.epJSON
+sinergym/data/buildings/ASHRAE901_Warehouse_STD2019_Denver.epJSON
+sinergym/data/buildings/LrgOff_GridStorageScheduled.epJSON
+sinergym/data/buildings/ShopWithPVandBattery.epJSON
 sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd
 sinergym/data/variables/5ZoneAutoDXVAV.rdd
-sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd
-sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd
-sinergym/data/variables/OfficeGridStorageSmoothing.rdd
-sinergym/data/variables/ShopWithVandBattery.rdd
+sinergym/data/variables/ASHRAE901_OfficeMedium_STD2019_Denver.rdd
+sinergym/data/variables/ASHRAE901_Warehouse_STD2019_Denver.rdd
+sinergym/data/variables/LrgOff_GridStorageScheduled.rdd
+sinergym/data/variables/ShopWithPVandBattery.rdd
 sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
 sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
 sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
 sinergym/data/weather/COL_Bogota.802220_IWEC.epw
 sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
 sinergym/data/weather/ESP_Granada.084190_SWEC.epw
 sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
```

### Comparing `sinergym-2.4.1/sinergym.egg-info/requires.txt` & `sinergym-2.5.0/sinergym.egg-info/requires.txt`

 * *Files identical despite different names*


# Comparing `tmp/act4e_mcdp-0.6.7-py3-none-any.whl.zip` & `tmp/act4e_mcdp-0.6.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 296336 bytes, number of entries: 17
+Zip file size: 296415 bytes, number of entries: 17
 -rw-r--r--  2.0 unx      454 b- defN 80-Jan-01 00:00 act4e_mcdp/__init__.py
 -rw-r--r--  2.0 unx  1280702 b- defN 80-Jan-01 00:00 act4e_mcdp/autogen_packed_test_data.py
 -rw-r--r--  2.0 unx      578 b- defN 80-Jan-01 00:00 act4e_mcdp/download.py
--rw-r--r--  2.0 unx    11637 b- defN 80-Jan-01 00:00 act4e_mcdp/loading.py
+-rw-r--r--  2.0 unx    11879 b- defN 80-Jan-01 00:00 act4e_mcdp/loading.py
 -rw-r--r--  2.0 unx     3129 b- defN 80-Jan-01 00:00 act4e_mcdp/main_solve_dp.py
 -rw-r--r--  2.0 unx     5076 b- defN 80-Jan-01 00:00 act4e_mcdp/main_solve_dp_queries.py
 -rw-r--r--  2.0 unx     3885 b- defN 80-Jan-01 00:00 act4e_mcdp/main_solve_mcdp.py
 -rw-r--r--  2.0 unx     4656 b- defN 80-Jan-01 00:00 act4e_mcdp/nameddps.py
 -rw-r--r--  2.0 unx     1790 b- defN 80-Jan-01 00:00 act4e_mcdp/posets.py
 -rw-r--r--  2.0 unx    11916 b- defN 80-Jan-01 00:00 act4e_mcdp/primitivedps.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 act4e_mcdp/py.typed
 -rw-r--r--  2.0 unx     7955 b- defN 80-Jan-01 00:00 act4e_mcdp/solution_interface.py
 -rw-r--r--  2.0 unx      253 b- defN 80-Jan-01 00:00 act4e_mcdp/utils.py
--rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 act4e_mcdp-0.6.7.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.6.7.dist-info/WHEEL
--rw-r--r--  2.0 unx      225 b- defN 80-Jan-01 00:00 act4e_mcdp-0.6.7.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1385 b- defN 16-Jan-01 00:00 act4e_mcdp-0.6.7.dist-info/RECORD
-17 files, 1334090 bytes uncompressed, 294072 bytes compressed:  78.0%
+-rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 act4e_mcdp-0.6.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.6.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx      225 b- defN 80-Jan-01 00:00 act4e_mcdp-0.6.8.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1385 b- defN 16-Jan-01 00:00 act4e_mcdp-0.6.8.dist-info/RECORD
+17 files, 1334332 bytes uncompressed, 294151 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: act4e_mcdp/solution_interface.py
 Comment: 
 
 Filename: act4e_mcdp/utils.py
 Comment: 
 
-Filename: act4e_mcdp-0.6.7.dist-info/METADATA
+Filename: act4e_mcdp-0.6.8.dist-info/METADATA
 Comment: 
 
-Filename: act4e_mcdp-0.6.7.dist-info/WHEEL
+Filename: act4e_mcdp-0.6.8.dist-info/WHEEL
 Comment: 
 
-Filename: act4e_mcdp-0.6.7.dist-info/entry_points.txt
+Filename: act4e_mcdp-0.6.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: act4e_mcdp-0.6.7.dist-info/RECORD
+Filename: act4e_mcdp-0.6.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## act4e_mcdp/__init__.py

```diff
@@ -3,15 +3,15 @@
 coloredlogs.install(level="DEBUG")  # type: ignore
 
 from logging import getLogger, DEBUG
 
 logger = getLogger(__name__)
 logger.setLevel(DEBUG)
 
-__version__ = "0.6.7"
+__version__ = "0.6.8"
 
 from .loading import *
 from .main_solve_mcdp import *
 from .main_solve_dp import *
 from .solution_interface import *
 from .nameddps import *
 from .primitivedps import *
```

## act4e_mcdp/loading.py

```diff
@@ -110,15 +110,21 @@
 
 
 @loader_for("CatalogueDP")
 def load_CatalogueDP(ob: dict[str, Any]):
     fields = _load_DP_fields(ob)
     entries = fields["entries"] = {}
     for k, v in ob["entries"].items():
-        entries[k] = EntryInfo(**v)
+        f_max_raw = v["f_max"]
+        r_min_raw = v["r_min"]
+        F = fields["F"]
+        R = fields["R"]
+        f_max = parse_yaml_value(F, f_max_raw)
+        r_min = parse_yaml_value(R, r_min_raw)
+        entries[k] = EntryInfo(f_max=f_max, r_min=r_min)
     return CatalogueDP(**fields)
 
 
 @loader_for("M_Res_MultiplyConstant_DP")
 def load_M_Res_MultiplyConstant_DP(ob: dict[str, Any]):
     fields = _load_DP_fields(ob)
     return M_Res_MultiplyConstant_DP(**fields)
@@ -416,15 +422,15 @@
         raise ValueError(msg) from e
 
 
 def parse_yaml_value(poset: Poset, ob: object) -> object:
     match poset:
         case Numbers():
             if not isinstance(ob, (int, str, float, bool)):
-                msg = "For Poset of numbers, expected string or int, got %s" % type(ob)
+                msg = "For Poset of numbers, expected string or int, got %s.\b%s" % (type(ob), repr(ob))
                 raise ValueError(msg)
             return Decimal(ob)
         case FinitePoset():
             return ob
         case PosetProduct(subs):
             if not isinstance(ob, list):
                 msg = "Expected list, got %s" % type(ob)
```

## Comparing `act4e_mcdp-0.6.7.dist-info/RECORD` & `act4e_mcdp-0.6.8.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-act4e_mcdp/__init__.py,sha256=-mtPKcwrD2doLXopgrXB3IEDCbXAe898WHTy7Zzhm2M,454
+act4e_mcdp/__init__.py,sha256=SUYb5IN5w6iA3wdV241VnD2IMuh3p0TYJQiIHjNYTK8,454
 act4e_mcdp/autogen_packed_test_data.py,sha256=i-setQV1m4kOo8OMbDjtc8IA_RgBVWMs3Ljj-c-LRgw,1280702
 act4e_mcdp/download.py,sha256=meWvp_y9zihZX3B9kTVMOKgVH_1iOZt2Qjhp5tHoH_Q,578
-act4e_mcdp/loading.py,sha256=aIBDMeeVOGKmqSmRcMyEXfAlZqMhuMFU6w5utDafhZc,11637
+act4e_mcdp/loading.py,sha256=nInT1N-Sw8ZfqNTUDhHBNbP-VyK0ThlGMdQbh1ewuG0,11879
 act4e_mcdp/main_solve_dp.py,sha256=3hPh6WdkK9xVzFm4QZPVLw72AaIi3FS0WBxsvcBLM1Y,3129
 act4e_mcdp/main_solve_dp_queries.py,sha256=3zYyan5I3oUqAd8zg-84TCqY8YHft75suultv52jyeg,5076
 act4e_mcdp/main_solve_mcdp.py,sha256=VSgOfgD5Uq0DMMyicY7cLVjCpagkfjLBRn8fV8V2wko,3885
 act4e_mcdp/nameddps.py,sha256=knysGfVrbeilCg9gX4B7S-b8JcuwbfFJN-WMxgCBrXo,4656
 act4e_mcdp/posets.py,sha256=7iijB7waZd3nTyK-_eNBR6YZOWhcTUYtKqCm7irpFKE,1790
 act4e_mcdp/primitivedps.py,sha256=dfA15BwI43XJQMx6OLf2rTu31TWnHcnpIKUaDPxc3r0,11916
 act4e_mcdp/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 act4e_mcdp/solution_interface.py,sha256=ZXjfYHep9JNFukgCJfgs5smqrwazsXmkJU9Da4LIQsg,7955
 act4e_mcdp/utils.py,sha256=l0snq4CINEo4nFEitvqxYDlZGNyu9hC0xW94f4PaxEo,253
-act4e_mcdp-0.6.7.dist-info/METADATA,sha256=78aCMa7gITNqGCqCUKf2XKzytK5IdyOweWlKTMuoY7o,361
-act4e_mcdp-0.6.7.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-act4e_mcdp-0.6.7.dist-info/entry_points.txt,sha256=cFH3w3DzczOms0kJedGgJfIn3m4Ip6dqqlcFy5dRWWI,225
-act4e_mcdp-0.6.7.dist-info/RECORD,,
+act4e_mcdp-0.6.8.dist-info/METADATA,sha256=s8xbDm3r3CZ4NWNGFOSmJ6OqRBj_E3UIoRQ2ZxH-Yws,361
+act4e_mcdp-0.6.8.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+act4e_mcdp-0.6.8.dist-info/entry_points.txt,sha256=cFH3w3DzczOms0kJedGgJfIn3m4Ip6dqqlcFy5dRWWI,225
+act4e_mcdp-0.6.8.dist-info/RECORD,,
```


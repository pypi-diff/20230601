# Comparing `tmp/lung_analysis_pipeline-0.0.2-py3-none-any.whl.zip` & `tmp/lung_analysis_pipeline-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,17 @@
-Zip file size: 224237 bytes, number of entries: 125
+Zip file size: 245051 bytes, number of entries: 136
 -rw-r--r--  2.0 unx     1708 b- defN 23-May-30 04:43 lung_analysis_pipeline/__init__.py
 -rw-r--r--  2.0 unx     6053 b- defN 23-Jun-01 04:17 lung_analysis_pipeline/model_pipeline.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 16:32 lung_analysis_pipeline/Feature_Extractor/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 16:33 lung_analysis_pipeline/Feature_Extractor/HSCNN/__init__.py
+-rw-r--r--  2.0 unx     4877 b- defN 23-Apr-25 19:19 lung_analysis_pipeline/Feature_Extractor/HSCNN/dataloader.py
+-rw-r--r--  2.0 unx    13292 b- defN 23-Jun-01 16:38 lung_analysis_pipeline/Feature_Extractor/HSCNN/model.py
+-rw-r--r--  2.0 unx    23021 b- defN 23-Apr-25 19:23 lung_analysis_pipeline/Feature_Extractor/HSCNN/train.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-30 23:16 lung_analysis_pipeline/Feature_Extractor/radiomics/__init__.py
+-rw-r--r--  2.0 unx     5745 b- defN 23-Jun-01 05:24 lung_analysis_pipeline/Feature_Extractor/radiomics/feature_extractor.py
 -rw-r--r--  2.0 unx      597 b- defN 23-May-30 03:29 lung_analysis_pipeline/NoduleDetect_SANet/__init__.py
 -rw-r--r--  2.0 unx     3891 b- defN 23-May-30 20:36 lung_analysis_pipeline/NoduleDetect_SANet/config.py
 -rw-r--r--  2.0 unx      510 b- defN 23-May-30 00:37 lung_analysis_pipeline/NoduleDetect_SANet/evaluation_updt.py
 -rw-r--r--  2.0 unx     5536 b- defN 23-May-30 04:31 lung_analysis_pipeline/NoduleDetect_SANet/test.py
 -rw-r--r--  2.0 unx     8924 b- defN 23-May-30 00:37 lung_analysis_pipeline/NoduleDetect_SANet/test_normCnd.py
 -rw-r--r--  2.0 unx    15175 b- defN 23-May-30 00:37 lung_analysis_pipeline/NoduleDetect_SANet/train.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-30 00:37 lung_analysis_pipeline/NoduleDetect_SANet/dataset/__init__.py
@@ -36,16 +43,20 @@
 -rw-r--r--  2.0 unx     1530 b- defN 23-May-30 00:37 lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/__init__.py
 -rw-r--r--  2.0 unx      799 b- defN 23-May-30 00:37 lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/build.py
 -rw-r--r--  2.0 unx      383 b- defN 23-May-30 00:37 lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/extension/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-30 00:37 lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/__init__.py
 -rw-r--r--  2.0 unx     1186 b- defN 23-May-30 00:37 lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/__init__.py
 -rw-r--r--  2.0 unx      819 b- defN 23-May-30 00:37 lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/build.py
 -rw-r--r--  2.0 unx      383 b- defN 23-May-30 00:37 lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/extension/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 16:34 lung_analysis_pipeline/NoduleDetect_SANet/utils/__init__.py
+-rw-r--r--  2.0 unx     3777 b- defN 23-May-30 00:37 lung_analysis_pipeline/NoduleDetect_SANet/utils/prepare_dataset_UCLA.py
+-rw-r--r--  2.0 unx     1474 b- defN 23-May-30 00:37 lung_analysis_pipeline/NoduleDetect_SANet/utils/pybox.py
+-rw-r--r--  2.0 unx    17889 b- defN 23-May-30 03:19 lung_analysis_pipeline/NoduleDetect_SANet/utils/util.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-30 01:25 lung_analysis_pipeline/NoduleSeg_MedicalNet/__init__.py
--rw-r--r--  2.0 unx     6850 b- defN 23-May-23 04:02 lung_analysis_pipeline/NoduleSeg_MedicalNet/build_unet_model.py
+-rw-r--r--  2.0 unx     6848 b- defN 23-Jun-01 16:38 lung_analysis_pipeline/NoduleSeg_MedicalNet/build_unet_model.py
 -rw-r--r--  2.0 unx     4368 b- defN 23-Apr-11 19:09 lung_analysis_pipeline/NoduleSeg_MedicalNet/model.py
 -rw-r--r--  2.0 unx     3612 b- defN 23-Apr-28 20:34 lung_analysis_pipeline/NoduleSeg_MedicalNet/setting.py
 -rw-r--r--  2.0 unx     3346 b- defN 23-Apr-11 19:09 lung_analysis_pipeline/NoduleSeg_MedicalNet/test.py
 -rw-r--r--  2.0 unx     5448 b- defN 23-Apr-11 19:09 lung_analysis_pipeline/NoduleSeg_MedicalNet/test_resnet34_lidc.py
 -rw-r--r--  2.0 unx     2301 b- defN 23-Apr-25 21:29 lung_analysis_pipeline/NoduleSeg_MedicalNet/test_unet_lidc.py
 -rw-r--r--  2.0 unx     3482 b- defN 23-Apr-11 19:09 lung_analysis_pipeline/NoduleSeg_MedicalNet/test_unet_norm.py
 -rw-r--r--  2.0 unx     5823 b- defN 23-Apr-11 19:09 lung_analysis_pipeline/NoduleSeg_MedicalNet/train.py
@@ -116,12 +127,12 @@
 -rw-r--r--  2.0 unx     8194 b- defN 23-Apr-07 20:47 lung_analysis_pipeline/dataset/tmp_with_label.py
 -rw-r--r--  2.0 unx    12951 b- defN 23-May-30 03:19 lung_analysis_pipeline/dataset/util.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-13 03:10 lung_analysis_pipeline/options/__init__.py
 -rw-r--r--  2.0 unx     2829 b- defN 23-May-31 17:45 lung_analysis_pipeline/options/opt.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-21 21:06 lung_analysis_pipeline/utils/__init__.py
 -rw-r--r--  2.0 unx    25935 b- defN 23-May-31 04:26 lung_analysis_pipeline/utils/patch.py
 -rw-r--r--  2.0 unx    28571 b- defN 23-Jun-01 04:23 lung_analysis_pipeline/utils/util.py
--rw-r--r--  2.0 unx      390 b- defN 23-Jun-01 16:30 lung_analysis_pipeline-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 16:30 lung_analysis_pipeline-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-01 16:30 lung_analysis_pipeline-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    15348 b- defN 23-Jun-01 16:30 lung_analysis_pipeline-0.0.2.dist-info/RECORD
-125 files, 735123 bytes uncompressed, 198049 bytes compressed:  73.1%
+-rw-r--r--  2.0 unx      390 b- defN 23-Jun-01 16:55 lung_analysis_pipeline-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 16:55 lung_analysis_pipeline-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-01 16:55 lung_analysis_pipeline-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    16620 b- defN 23-Jun-01 16:55 lung_analysis_pipeline-0.0.3.dist-info/RECORD
+136 files, 806468 bytes uncompressed, 216719 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -1,13 +1,34 @@
 Filename: lung_analysis_pipeline/__init__.py
 Comment: 
 
 Filename: lung_analysis_pipeline/model_pipeline.py
 Comment: 
 
+Filename: lung_analysis_pipeline/Feature_Extractor/__init__.py
+Comment: 
+
+Filename: lung_analysis_pipeline/Feature_Extractor/HSCNN/__init__.py
+Comment: 
+
+Filename: lung_analysis_pipeline/Feature_Extractor/HSCNN/dataloader.py
+Comment: 
+
+Filename: lung_analysis_pipeline/Feature_Extractor/HSCNN/model.py
+Comment: 
+
+Filename: lung_analysis_pipeline/Feature_Extractor/HSCNN/train.py
+Comment: 
+
+Filename: lung_analysis_pipeline/Feature_Extractor/radiomics/__init__.py
+Comment: 
+
+Filename: lung_analysis_pipeline/Feature_Extractor/radiomics/feature_extractor.py
+Comment: 
+
 Filename: lung_analysis_pipeline/NoduleDetect_SANet/__init__.py
 Comment: 
 
 Filename: lung_analysis_pipeline/NoduleDetect_SANet/config.py
 Comment: 
 
 Filename: lung_analysis_pipeline/NoduleDetect_SANet/evaluation_updt.py
@@ -117,14 +138,26 @@
 
 Filename: lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/build.py
 Comment: 
 
 Filename: lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/extension/__init__.py
 Comment: 
 
+Filename: lung_analysis_pipeline/NoduleDetect_SANet/utils/__init__.py
+Comment: 
+
+Filename: lung_analysis_pipeline/NoduleDetect_SANet/utils/prepare_dataset_UCLA.py
+Comment: 
+
+Filename: lung_analysis_pipeline/NoduleDetect_SANet/utils/pybox.py
+Comment: 
+
+Filename: lung_analysis_pipeline/NoduleDetect_SANet/utils/util.py
+Comment: 
+
 Filename: lung_analysis_pipeline/NoduleSeg_MedicalNet/__init__.py
 Comment: 
 
 Filename: lung_analysis_pipeline/NoduleSeg_MedicalNet/build_unet_model.py
 Comment: 
 
 Filename: lung_analysis_pipeline/NoduleSeg_MedicalNet/model.py
@@ -357,20 +390,20 @@
 
 Filename: lung_analysis_pipeline/utils/patch.py
 Comment: 
 
 Filename: lung_analysis_pipeline/utils/util.py
 Comment: 
 
-Filename: lung_analysis_pipeline-0.0.2.dist-info/METADATA
+Filename: lung_analysis_pipeline-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: lung_analysis_pipeline-0.0.2.dist-info/WHEEL
+Filename: lung_analysis_pipeline-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: lung_analysis_pipeline-0.0.2.dist-info/top_level.txt
+Filename: lung_analysis_pipeline-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: lung_analysis_pipeline-0.0.2.dist-info/RECORD
+Filename: lung_analysis_pipeline-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lung_analysis_pipeline/NoduleSeg_MedicalNet/build_unet_model.py

```diff
@@ -165,15 +165,15 @@
 
 def create_seg_model(opt, in_nc=1, out_nc=1, nf=64): 
     ## from opt to create segmentation options  
 
     ## create segmentation model    
     model = UNet(in_nc=in_nc, out_nc=out_nc, nf=nf).cuda()
     model = nn.DataParallel(model)
-    path_to_weight = './trails_UNet/models/UNet_epoch_106_best_weight_0.646983.pth.tar'
+    path_to_weight = 'trails_UNet/models/UNet_epoch_106_best_weight_0.646983.pth.tar'
     # path_to_weight = os.path.abspath(os.path.join(os.path.dirname(__file__), path_to_weight))
     # path_to_weight = os.path.join(module_path, path_to_weight)
     path_to_weight = pkg_resources.resource_filename(__name__, path_to_weight)
     checkpoint = torch.load(path_to_weight)
     model.load_state_dict(checkpoint['state_dict'])
 
     # Extract the original model from the DataParallel wrapper
```

## Comparing `lung_analysis_pipeline-0.0.2.dist-info/RECORD` & `lung_analysis_pipeline-0.0.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 lung_analysis_pipeline/__init__.py,sha256=A7r6C5jnS2bR_6diTuty17H3lsDWBdAiaQKZ07fiUJs,1708
 lung_analysis_pipeline/model_pipeline.py,sha256=jcw23YZ0gPA-bQZ2HwbUpyqult_jscUxAvmpqay1poA,6053
+lung_analysis_pipeline/Feature_Extractor/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lung_analysis_pipeline/Feature_Extractor/HSCNN/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lung_analysis_pipeline/Feature_Extractor/HSCNN/dataloader.py,sha256=AuPHx7RpdComXdB9iaZZet6Z3DbJMcfDUWci3T9K7ac,4877
+lung_analysis_pipeline/Feature_Extractor/HSCNN/model.py,sha256=2LjtKvwHWARd22dmIMsKxdVBH3P4vqT3iE9cFe8n0Ro,13292
+lung_analysis_pipeline/Feature_Extractor/HSCNN/train.py,sha256=Qe313RS3lka8LdNbZNEfpORs5Jes-AqblZ5HDVtcwlo,23021
+lung_analysis_pipeline/Feature_Extractor/radiomics/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lung_analysis_pipeline/Feature_Extractor/radiomics/feature_extractor.py,sha256=1b_T3ON78gVUBQKZ2jOdok1QpJ3XTshW6KgS04CwOZs,5745
 lung_analysis_pipeline/NoduleDetect_SANet/__init__.py,sha256=GqNz0ivm6zHskNFoGTn5BXgqGlcEddZ7BZB0wy8Pzss,597
 lung_analysis_pipeline/NoduleDetect_SANet/config.py,sha256=0sxU5Yq9rzrQ7Y9z6047tGFMbC9_c9pugV-VGYfwiLk,3891
 lung_analysis_pipeline/NoduleDetect_SANet/evaluation_updt.py,sha256=DCYXjlAOwAarecIUbLW4W3R5FlH98LEuy6X-EDMbtKE,510
 lung_analysis_pipeline/NoduleDetect_SANet/test.py,sha256=FasEaBWhgbRv_tQ-Xp5z4_X_5KpmUWOzD00J5MR0epY,5536
 lung_analysis_pipeline/NoduleDetect_SANet/test_normCnd.py,sha256=tF3t_lmnJQHla3YmPZ5O-iW62_nlwS_KPN_pPcGJA2M,8924
 lung_analysis_pipeline/NoduleDetect_SANet/train.py,sha256=TOzCDoYDCXBr1CA5u6u36d4TgbyOQTyFUG0pgyWc6ok,15175
 lung_analysis_pipeline/NoduleDetect_SANet/dataset/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -35,16 +42,20 @@
 lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/__init__.py,sha256=e69wiMhnQhlCvxvvvx5zyUsRdk5UoIrm-ISbD2uDBe8,1530
 lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/build.py,sha256=-8sl6-IVSKrcHqPlyi4xo-_8IkPGIXbQStl7B8YLy04,799
 lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/extension/__init__.py,sha256=6v7SBf2RMS53oJIqtCr0KBgJaW3FAwI51Dv-i4Vum2I,383
 lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/__init__.py,sha256=gv0L-zSm6DcQifGkxJwViF4QtoHSpYxEZqIF0DH8-PQ,1186
 lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/build.py,sha256=6GthJ4tlqP9gLm4ejmbwetbWy4GLX0vKvndAyerlx6U,819
 lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/extension/__init__.py,sha256=6v7SBf2RMS53oJIqtCr0KBgJaW3FAwI51Dv-i4Vum2I,383
+lung_analysis_pipeline/NoduleDetect_SANet/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lung_analysis_pipeline/NoduleDetect_SANet/utils/prepare_dataset_UCLA.py,sha256=Kaho2gUraNkCetXSPVM0o56I1Pblbinjms4L5Gvt17s,3777
+lung_analysis_pipeline/NoduleDetect_SANet/utils/pybox.py,sha256=uLRvX38BQ22BDFLREeN61Kc6jaaDuUDHtj2ihJKvXiA,1474
+lung_analysis_pipeline/NoduleDetect_SANet/utils/util.py,sha256=guSKeZ8FjkvqpRiDwU4pcDlefhCScNrxULpCUshQGBs,17889
 lung_analysis_pipeline/NoduleSeg_MedicalNet/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-lung_analysis_pipeline/NoduleSeg_MedicalNet/build_unet_model.py,sha256=ULp-6y4I9UjiOoZVg6EH0B5XMduwq2UwPYBgm080Isw,6850
+lung_analysis_pipeline/NoduleSeg_MedicalNet/build_unet_model.py,sha256=sYT1ORbCZyV7PayrtxdveBstmWc92PFCvBOku4t_vqU,6848
 lung_analysis_pipeline/NoduleSeg_MedicalNet/model.py,sha256=XFkEggOgVfwmQd80qIXUsprSoLRNTgdIOd4j9bNxszo,4368
 lung_analysis_pipeline/NoduleSeg_MedicalNet/setting.py,sha256=0YQgZgcz1v5a4B3-QgqoMR59iyCw-p-McFoK5dPHOkc,3612
 lung_analysis_pipeline/NoduleSeg_MedicalNet/test.py,sha256=cby-hZ6Rw3ikPxO-D7VyhbaNWQWEw8WkU_xvQUUffEU,3346
 lung_analysis_pipeline/NoduleSeg_MedicalNet/test_resnet34_lidc.py,sha256=pxldCo6L7GXobIoN2aPt1gN1E6fFsrmo8Pl6wE1BedY,5448
 lung_analysis_pipeline/NoduleSeg_MedicalNet/test_unet_lidc.py,sha256=OYYh71iMJVQE9YaynvsIySUHj5z4tvvUfxHFbB0DG_E,2301
 lung_analysis_pipeline/NoduleSeg_MedicalNet/test_unet_norm.py,sha256=OoQm5M6TY8Ewm6GrguDueqNeWnT5OsK4cL1fx0EnsDM,3482
 lung_analysis_pipeline/NoduleSeg_MedicalNet/train.py,sha256=Qg2drCa4YjK4-bJtXLtgN60ek4yPCV453hiQrHjVjV0,5823
@@ -115,11 +126,11 @@
 lung_analysis_pipeline/dataset/tmp_with_label.py,sha256=eIn8KE_OwL3hWG_TVchjWFMBEts8TLg1CCoLtKCGRVM,8194
 lung_analysis_pipeline/dataset/util.py,sha256=hpdIuXysXODdEbI0_k8Aes06D6aZSz6v4cSbjLxnFcY,12951
 lung_analysis_pipeline/options/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lung_analysis_pipeline/options/opt.py,sha256=RNLPpyp-an9NJGcjsgbaozkhbe6HU_OkdlslaXipio8,2829
 lung_analysis_pipeline/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lung_analysis_pipeline/utils/patch.py,sha256=lMq6CbDtC7fQ9EN1-SpygZjowJ6PlrloME17Fde-euA,25935
 lung_analysis_pipeline/utils/util.py,sha256=Zo1e0XvSkqDAcZBfyg_4CUFnl18PUgeaZwEwS0bXkMo,28571
-lung_analysis_pipeline-0.0.2.dist-info/METADATA,sha256=1CDcRVOkXFvSKdpxDt8a9aBdGNHpbhdKh6aItU7HHlI,390
-lung_analysis_pipeline-0.0.2.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-lung_analysis_pipeline-0.0.2.dist-info/top_level.txt,sha256=Dg-m-Z14rvvro7_E-pGkMufOWYuYi85T9LTnMxoE7Ig,23
-lung_analysis_pipeline-0.0.2.dist-info/RECORD,,
+lung_analysis_pipeline-0.0.3.dist-info/METADATA,sha256=F5hbk-LN5TyZmB0UuzQOzx02xB9h5XeqgwMNtvW6E_M,390
+lung_analysis_pipeline-0.0.3.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+lung_analysis_pipeline-0.0.3.dist-info/top_level.txt,sha256=Dg-m-Z14rvvro7_E-pGkMufOWYuYi85T9LTnMxoE7Ig,23
+lung_analysis_pipeline-0.0.3.dist-info/RECORD,,
```


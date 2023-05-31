# Comparing `tmp/tpds_core-2.3.4-py3-none-any.whl.zip` & `tmp/tpds_core-2.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,83 +1,88 @@
-Zip file size: 228441 bytes, number of entries: 81
--rw-r--r--  2.0 unx       65 b- defN 23-Mar-14 22:03 tpds/__init__.py
--rw-r--r--  2.0 unx       32 b- defN 23-Mar-14 22:03 tpds/api/__init__.py
--rw-r--r--  2.0 unx     6250 b- defN 23-Mar-14 22:03 tpds/api/core.py
--rw-r--r--  2.0 unx     4301 b- defN 23-Mar-14 22:03 tpds/api/loader.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-14 22:03 tpds/api/api/__init__.py
--rw-r--r--  2.0 unx      528 b- defN 23-Mar-14 22:03 tpds/api/api/router.py
--rw-r--r--  2.0 unx     4745 b- defN 23-Mar-14 22:03 tpds/api/api/usecases.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-14 22:03 tpds/api/api/hw/__init__.py
--rw-r--r--  2.0 unx     3904 b- defN 23-Mar-14 22:03 tpds/api/api/hw/api_board.py
--rw-r--r--  2.0 unx     6741 b- defN 23-Mar-14 22:03 tpds/api/api/hw/api_device.py
--rw-r--r--  2.0 unx     3718 b- defN 23-Mar-14 22:03 tpds/api/api/manifest_file/api_manifest.py
--rw-r--r--  2.0 unx      675 b- defN 23-Mar-14 22:03 tpds/api/api/manifest_file/MCHP_manifest_signer/MCHP_manifest_signer_1_Jan2019_July2019.crt
--rw-r--r--  2.0 unx      676 b- defN 23-Mar-14 22:03 tpds/api/api/manifest_file/MCHP_manifest_signer/MCHP_manifest_signer_2_Aug2019_Aug2020.crt
--rw-r--r--  2.0 unx      676 b- defN 23-Mar-14 22:03 tpds/api/api/manifest_file/MCHP_manifest_signer/MCHP_manifest_signer_3_Aug-13-2020-Aug-13-2023.crt
--rw-r--r--  2.0 unx     3134 b- defN 23-Mar-14 22:03 tpds/api/api/package_manager/api_package_manager.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-14 22:03 tpds/api/api/schemas/__init__.py
--rw-r--r--  2.0 unx     1672 b- defN 23-Mar-14 22:03 tpds/api/api/schemas/hw.py
--rw-r--r--  2.0 unx   221974 b- defN 23-Mar-14 22:03 tpds/api/assets/favicon.ico
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-14 22:03 tpds/api/tests/__init__.py
--rw-r--r--  2.0 unx      212 b- defN 23-Mar-14 22:03 tpds/api/tests/conftest.py
--rw-r--r--  2.0 unx      196 b- defN 23-Mar-14 22:03 tpds/api/tests/pytest.ini
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-14 22:03 tpds/api/tests/api/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-14 22:03 tpds/api/tests/api/hw/__init__.py
--rw-r--r--  2.0 unx     1284 b- defN 23-Mar-14 22:03 tpds/api/tests/api/hw/test_api_board.py
--rw-r--r--  2.0 unx     2272 b- defN 23-Mar-14 22:03 tpds/api/tests/api/hw/test_api_device.py
--rw-r--r--  2.0 unx      289 b- defN 23-Mar-14 22:03 tpds/devices/__init__.py
--rw-r--r--  2.0 unx      773 b- defN 23-Mar-14 22:03 tpds/devices/boards_schema.yaml
--rw-r--r--  2.0 unx     2246 b- defN 23-Mar-14 22:03 tpds/devices/devices_schema.yaml
--rw-r--r--  2.0 unx     3371 b- defN 23-Mar-14 22:03 tpds/devices/tpds_boards.py
--rw-r--r--  2.0 unx     3906 b- defN 23-Mar-14 22:03 tpds/devices/tpds_devices.py
--rw-r--r--  2.0 unx     5121 b- defN 23-Mar-14 22:03 tpds/devices/tpds_models.py
--rw-r--r--  2.0 unx     1106 b- defN 23-Mar-14 22:03 tpds/devices/data/ecc608-tcsm.yaml
--rw-r--r--  2.0 unx     1926 b- defN 23-Mar-14 22:03 tpds/devices/data/ecc608-tflx.yaml
--rw-r--r--  2.0 unx     3962 b- defN 23-Mar-14 22:03 tpds/devices/data/ecc608-tng.yaml
--rw-r--r--  2.0 unx     1312 b- defN 23-Mar-14 22:03 tpds/devices/data/modules.yaml
--rw-r--r--  2.0 unx     1019 b- defN 23-Mar-14 22:03 tpds/devices/data/sha204.yaml
--rw-r--r--  2.0 unx      881 b- defN 23-Mar-14 22:03 tpds/devices/data/ta100.yaml
--rw-r--r--  2.0 unx      124 b- defN 23-Mar-14 22:03 tpds/helper/__init__.py
--rw-r--r--  2.0 unx     2544 b- defN 23-Mar-14 22:03 tpds/helper/logger.py
--rw-r--r--  2.0 unx     4113 b- defN 23-Mar-14 22:03 tpds/helper/processing.py
--rw-r--r--  2.0 unx     2498 b- defN 23-Mar-14 22:03 tpds/helper/utils.py
--rw-r--r--  2.0 unx       21 b- defN 23-Mar-14 22:03 tpds/launcher/__init__.py
--rw-r--r--  2.0 unx     3819 b- defN 23-Mar-14 22:03 tpds/launcher/start.py
--rw-r--r--  2.0 unx      119 b- defN 23-Mar-14 22:03 tpds/package_manager/__init__.py
--rw-r--r--  2.0 unx     2567 b- defN 23-Mar-14 22:03 tpds/package_manager/client_model.py
--rw-r--r--  2.0 unx    13594 b- defN 23-Mar-14 22:03 tpds/package_manager/conda_client.py
--rw-r--r--  2.0 unx     3888 b- defN 23-Mar-14 22:03 tpds/package_manager/data_models.py
--rw-r--r--  2.0 unx    11844 b- defN 23-Mar-14 22:03 tpds/package_manager/manager.py
--rw-r--r--  2.0 unx     1299 b- defN 23-Mar-14 22:03 tpds/package_manager/packages_schema.yaml
--rw-r--r--  2.0 unx     6995 b- defN 23-Mar-14 22:03 tpds/package_manager/pip_client.py
--rw-r--r--  2.0 unx     1239 b- defN 23-Mar-14 22:03 tpds/package_manager/licenses/mchp.txt
--rw-r--r--  2.0 unx    21064 b- defN 23-Mar-14 22:03 tpds/servers/TPDS_notebook_config.py
--rw-r--r--  2.0 unx      202 b- defN 23-Mar-14 22:03 tpds/servers/__init__.py
--rw-r--r--  2.0 unx     4410 b- defN 23-Mar-14 22:03 tpds/servers/jupyter_server.py
--rw-r--r--  2.0 unx    11491 b- defN 23-Mar-14 22:03 tpds/servers/msg_handler.py
--rw-r--r--  2.0 unx    13114 b- defN 23-Mar-14 22:03 tpds/servers/msg_handler_ta.py
--rw-r--r--  2.0 unx     2565 b- defN 23-Mar-14 22:03 tpds/servers/msg_handler_tcustom.py
--rw-r--r--  2.0 unx     4540 b- defN 23-Mar-14 22:03 tpds/servers/msg_handler_tflx.py
--rw-r--r--  2.0 unx     9708 b- defN 23-Mar-14 22:03 tpds/servers/msg_handler_tflx_ecc204.py
--rw-r--r--  2.0 unx     7306 b- defN 23-Mar-14 22:03 tpds/servers/provision_user_inputs.py
--rw-r--r--  2.0 unx     5761 b- defN 23-Mar-14 22:03 tpds/servers/symm_auth_user_inputs.py
--rw-r--r--  2.0 unx    16910 b- defN 23-Mar-14 22:03 tpds/servers/tflx_provisioning_xml_ui.py
--rw-r--r--  2.0 unx     1093 b- defN 23-Mar-14 22:03 tpds/servers/uno_server.py
--rw-r--r--  2.0 unx     3813 b- defN 23-Mar-14 22:03 tpds/servers/websocket_server.py
--rw-r--r--  2.0 unx     9210 b- defN 23-Mar-14 22:03 tpds/servers/wpc_user_inputs.py
--rw-r--r--  2.0 unx       74 b- defN 23-Mar-14 22:03 tpds/settings/__init__.py
--rw-r--r--  2.0 unx     2583 b- defN 23-Mar-14 22:03 tpds/settings/tpds_config.yaml
--rw-r--r--  2.0 unx     1048 b- defN 23-Mar-14 22:03 tpds/settings/tpds_default.yaml
--rw-r--r--  2.0 unx    11471 b- defN 23-Mar-14 22:03 tpds/settings/tpds_settings.py
--rw-r--r--  2.0 unx     3444 b- defN 23-Mar-14 22:03 tpds/settings/validator.py
--rw-r--r--  2.0 unx       48 b- defN 23-Mar-14 22:03 tpds/usecase_collector/__init__.py
--rw-r--r--  2.0 unx     7085 b- defN 23-Mar-14 22:03 tpds/usecase_collector/collector.py
--rw-r--r--  2.0 unx     8889 b- defN 23-Mar-14 22:03 tpds/usecase_collector/usecase.py
--rw-r--r--  2.0 unx     2126 b- defN 23-Mar-14 22:03 tpds/usecase_collector/usecase.yaml
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-14 22:03 tpds/version/__init__.py
--rw-r--r--  2.0 unx     1322 b- defN 23-Mar-14 22:04 tpds_core-2.3.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     2846 b- defN 23-Mar-14 22:04 tpds_core-2.3.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-14 22:04 tpds_core-2.3.4.dist-info/WHEEL
--rw-r--r--  2.0 unx      102 b- defN 23-Mar-14 22:04 tpds_core-2.3.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Mar-14 22:04 tpds_core-2.3.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     7169 b- defN 23-Mar-14 22:04 tpds_core-2.3.4.dist-info/RECORD
-81 files, 503122 bytes uncompressed, 216971 bytes compressed:  56.9%
+Zip file size: 234019 bytes, number of entries: 86
+-rw-r--r--  2.0 unx       65 b- defN 23-May-31 23:10 tpds/__init__.py
+-rw-r--r--  2.0 unx       61 b- defN 23-May-31 23:10 tpds/api/__init__.py
+-rw-r--r--  2.0 unx     6434 b- defN 23-May-31 23:10 tpds/api/core.py
+-rw-r--r--  2.0 unx     4303 b- defN 23-May-31 23:10 tpds/api/loader.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 23:10 tpds/api/api/__init__.py
+-rw-r--r--  2.0 unx      528 b- defN 23-May-31 23:10 tpds/api/api/router.py
+-rw-r--r--  2.0 unx     4745 b- defN 23-May-31 23:10 tpds/api/api/usecases.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 23:10 tpds/api/api/hw/__init__.py
+-rw-r--r--  2.0 unx     3803 b- defN 23-May-31 23:10 tpds/api/api/hw/api_board.py
+-rw-r--r--  2.0 unx     6741 b- defN 23-May-31 23:10 tpds/api/api/hw/api_device.py
+-rw-r--r--  2.0 unx     3711 b- defN 23-May-31 23:10 tpds/api/api/manifest_file/api_manifest.py
+-rw-r--r--  2.0 unx      675 b- defN 23-May-31 23:10 tpds/api/api/manifest_file/MCHP_manifest_signer/MCHP_manifest_signer_1_Jan2019_July2019.crt
+-rw-r--r--  2.0 unx      676 b- defN 23-May-31 23:10 tpds/api/api/manifest_file/MCHP_manifest_signer/MCHP_manifest_signer_2_Aug2019_Aug2020.crt
+-rw-r--r--  2.0 unx      676 b- defN 23-May-31 23:10 tpds/api/api/manifest_file/MCHP_manifest_signer/MCHP_manifest_signer_3_Aug-13-2020-Aug-13-2023.crt
+-rw-r--r--  2.0 unx     3127 b- defN 23-May-31 23:10 tpds/api/api/package_manager/api_package_manager.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 23:10 tpds/api/api/schemas/__init__.py
+-rw-r--r--  2.0 unx     1672 b- defN 23-May-31 23:10 tpds/api/api/schemas/hw.py
+-rw-r--r--  2.0 unx   221974 b- defN 23-May-31 23:10 tpds/api/assets/favicon.ico
+-rw-r--r--  2.0 unx      114 b- defN 23-May-31 23:10 tpds/configurator/__init__.py
+-rw-r--r--  2.0 unx      354 b- defN 23-May-31 23:10 tpds/configurator/algorithms.py
+-rw-r--r--  2.0 unx     2100 b- defN 23-May-31 23:10 tpds/configurator/api.py
+-rw-r--r--  2.0 unx     1245 b- defN 23-May-31 23:10 tpds/configurator/configurator.py
+-rw-r--r--  2.0 unx     5395 b- defN 23-May-31 23:10 tpds/configurator/models.py
+-rw-r--r--  2.0 unx     2377 b- defN 23-May-31 23:10 tpds/configurator/store.py
+-rw-r--r--  2.0 unx      116 b- defN 23-May-31 23:10 tpds/configurator/engine/__init__.py
+-rw-r--r--  2.0 unx     6074 b- defN 23-May-31 23:10 tpds/configurator/engine/engine.py
+-rw-r--r--  2.0 unx      708 b- defN 23-May-31 23:10 tpds/configurator/engine/exceptions.py
+-rw-r--r--  2.0 unx     1332 b- defN 23-May-31 23:10 tpds/configurator/engine/rule.py
+-rw-r--r--  2.0 unx     6867 b- defN 23-May-31 23:10 tpds/configurator/engine/state.py
+-rw-r--r--  2.0 unx      187 b- defN 23-May-31 23:10 tpds/configurator/engine/types.py
+-rw-r--r--  2.0 unx      289 b- defN 23-May-31 23:10 tpds/devices/__init__.py
+-rw-r--r--  2.0 unx      773 b- defN 23-May-31 23:10 tpds/devices/boards_schema.yaml
+-rw-r--r--  2.0 unx     2300 b- defN 23-May-31 23:10 tpds/devices/devices_schema.yaml
+-rw-r--r--  2.0 unx     3292 b- defN 23-May-31 23:10 tpds/devices/tpds_boards.py
+-rw-r--r--  2.0 unx     3849 b- defN 23-May-31 23:10 tpds/devices/tpds_devices.py
+-rw-r--r--  2.0 unx     5099 b- defN 23-May-31 23:10 tpds/devices/tpds_models.py
+-rw-r--r--  2.0 unx     1106 b- defN 23-May-31 23:10 tpds/devices/data/ecc608-tcsm.yaml
+-rw-r--r--  2.0 unx      998 b- defN 23-May-31 23:10 tpds/devices/data/ecc608-tflx.yaml
+-rw-r--r--  2.0 unx     3962 b- defN 23-May-31 23:10 tpds/devices/data/ecc608-tng.yaml
+-rw-r--r--  2.0 unx     1312 b- defN 23-May-31 23:10 tpds/devices/data/modules.yaml
+-rw-r--r--  2.0 unx     1056 b- defN 23-May-31 23:10 tpds/devices/data/sha204.yaml
+-rw-r--r--  2.0 unx      880 b- defN 23-May-31 23:10 tpds/devices/data/ta100.yaml
+-rw-r--r--  2.0 unx      460 b- defN 23-May-31 23:10 tpds/helper/__init__.py
+-rw-r--r--  2.0 unx     2543 b- defN 23-May-31 23:10 tpds/helper/logger.py
+-rw-r--r--  2.0 unx     4113 b- defN 23-May-31 23:10 tpds/helper/processing.py
+-rw-r--r--  2.0 unx      956 b- defN 23-May-31 23:10 tpds/helper/singleton.py
+-rw-r--r--  2.0 unx     2519 b- defN 23-May-31 23:10 tpds/helper/utils.py
+-rw-r--r--  2.0 unx       96 b- defN 23-May-31 23:10 tpds/launcher/__init__.py
+-rw-r--r--  2.0 unx     3819 b- defN 23-May-31 23:10 tpds/launcher/start.py
+-rw-r--r--  2.0 unx      187 b- defN 23-May-31 23:10 tpds/package_manager/__init__.py
+-rw-r--r--  2.0 unx     2567 b- defN 23-May-31 23:10 tpds/package_manager/client_model.py
+-rw-r--r--  2.0 unx     2144 b- defN 23-May-31 23:10 tpds/package_manager/data_models.py
+-rw-r--r--  2.0 unx    11961 b- defN 23-May-31 23:10 tpds/package_manager/manager.py
+-rw-r--r--  2.0 unx     1299 b- defN 23-May-31 23:10 tpds/package_manager/packages_schema.yaml
+-rw-r--r--  2.0 unx     7144 b- defN 23-May-31 23:10 tpds/package_manager/pip_client.py
+-rw-r--r--  2.0 unx     1239 b- defN 23-May-31 23:10 tpds/package_manager/licenses/mchp.txt
+-rw-r--r--  2.0 unx    21064 b- defN 23-May-31 23:10 tpds/servers/TPDS_notebook_config.py
+-rw-r--r--  2.0 unx      332 b- defN 23-May-31 23:10 tpds/servers/__init__.py
+-rw-r--r--  2.0 unx     4410 b- defN 23-May-31 23:10 tpds/servers/jupyter_server.py
+-rw-r--r--  2.0 unx    11754 b- defN 23-May-31 23:10 tpds/servers/msg_handler.py
+-rw-r--r--  2.0 unx    13130 b- defN 23-May-31 23:10 tpds/servers/msg_handler_ta.py
+-rw-r--r--  2.0 unx     2565 b- defN 23-May-31 23:10 tpds/servers/msg_handler_tcustom.py
+-rw-r--r--  2.0 unx     4494 b- defN 23-May-31 23:10 tpds/servers/msg_handler_tflx.py
+-rw-r--r--  2.0 unx     9582 b- defN 23-May-31 23:10 tpds/servers/msg_handler_tflx_ecc204.py
+-rw-r--r--  2.0 unx     7250 b- defN 23-May-31 23:10 tpds/servers/provision_user_inputs.py
+-rw-r--r--  2.0 unx     6091 b- defN 23-May-31 23:10 tpds/servers/symm_auth_user_inputs.py
+-rw-r--r--  2.0 unx    16534 b- defN 23-May-31 23:10 tpds/servers/tflx_provisioning_xml_ui.py
+-rw-r--r--  2.0 unx     1093 b- defN 23-May-31 23:10 tpds/servers/uno_server.py
+-rw-r--r--  2.0 unx     3826 b- defN 23-May-31 23:10 tpds/servers/websocket_server.py
+-rw-r--r--  2.0 unx     9087 b- defN 23-May-31 23:10 tpds/servers/wpc_user_inputs.py
+-rw-r--r--  2.0 unx      111 b- defN 23-May-31 23:10 tpds/settings/__init__.py
+-rw-r--r--  2.0 unx     2583 b- defN 23-May-31 23:10 tpds/settings/tpds_config.yaml
+-rw-r--r--  2.0 unx     1048 b- defN 23-May-31 23:10 tpds/settings/tpds_default.yaml
+-rw-r--r--  2.0 unx    11556 b- defN 23-May-31 23:10 tpds/settings/tpds_settings.py
+-rw-r--r--  2.0 unx     3444 b- defN 23-May-31 23:10 tpds/settings/validator.py
+-rw-r--r--  2.0 unx      138 b- defN 23-May-31 23:10 tpds/usecase_collector/__init__.py
+-rw-r--r--  2.0 unx     7103 b- defN 23-May-31 23:10 tpds/usecase_collector/collector.py
+-rw-r--r--  2.0 unx     9007 b- defN 23-May-31 23:10 tpds/usecase_collector/usecase.py
+-rw-r--r--  2.0 unx     2126 b- defN 23-May-31 23:10 tpds/usecase_collector/usecase.yaml
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 23:10 tpds/version/__init__.py
+-rw-r--r--  2.0 unx     1322 b- defN 23-May-31 23:10 tpds_core-2.3.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3256 b- defN 23-May-31 23:10 tpds_core-2.3.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 23:10 tpds_core-2.3.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx      102 b- defN 23-May-31 23:10 tpds_core-2.3.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-May-31 23:10 tpds_core-2.3.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7604 b- defN 23-May-31 23:10 tpds_core-2.3.5.dist-info/RECORD
+86 files, 512732 bytes uncompressed, 221879 bytes compressed:  56.7%
```

## zipnote {}

```diff
@@ -48,33 +48,48 @@
 
 Filename: tpds/api/api/schemas/hw.py
 Comment: 
 
 Filename: tpds/api/assets/favicon.ico
 Comment: 
 
-Filename: tpds/api/tests/__init__.py
+Filename: tpds/configurator/__init__.py
 Comment: 
 
-Filename: tpds/api/tests/conftest.py
+Filename: tpds/configurator/algorithms.py
 Comment: 
 
-Filename: tpds/api/tests/pytest.ini
+Filename: tpds/configurator/api.py
 Comment: 
 
-Filename: tpds/api/tests/api/__init__.py
+Filename: tpds/configurator/configurator.py
 Comment: 
 
-Filename: tpds/api/tests/api/hw/__init__.py
+Filename: tpds/configurator/models.py
 Comment: 
 
-Filename: tpds/api/tests/api/hw/test_api_board.py
+Filename: tpds/configurator/store.py
 Comment: 
 
-Filename: tpds/api/tests/api/hw/test_api_device.py
+Filename: tpds/configurator/engine/__init__.py
+Comment: 
+
+Filename: tpds/configurator/engine/engine.py
+Comment: 
+
+Filename: tpds/configurator/engine/exceptions.py
+Comment: 
+
+Filename: tpds/configurator/engine/rule.py
+Comment: 
+
+Filename: tpds/configurator/engine/state.py
+Comment: 
+
+Filename: tpds/configurator/engine/types.py
 Comment: 
 
 Filename: tpds/devices/__init__.py
 Comment: 
 
 Filename: tpds/devices/boards_schema.yaml
 Comment: 
@@ -114,14 +129,17 @@
 
 Filename: tpds/helper/logger.py
 Comment: 
 
 Filename: tpds/helper/processing.py
 Comment: 
 
+Filename: tpds/helper/singleton.py
+Comment: 
+
 Filename: tpds/helper/utils.py
 Comment: 
 
 Filename: tpds/launcher/__init__.py
 Comment: 
 
 Filename: tpds/launcher/start.py
@@ -129,17 +147,14 @@
 
 Filename: tpds/package_manager/__init__.py
 Comment: 
 
 Filename: tpds/package_manager/client_model.py
 Comment: 
 
-Filename: tpds/package_manager/conda_client.py
-Comment: 
-
 Filename: tpds/package_manager/data_models.py
 Comment: 
 
 Filename: tpds/package_manager/manager.py
 Comment: 
 
 Filename: tpds/package_manager/packages_schema.yaml
@@ -219,26 +234,26 @@
 
 Filename: tpds/usecase_collector/usecase.yaml
 Comment: 
 
 Filename: tpds/version/__init__.py
 Comment: 
 
-Filename: tpds_core-2.3.4.dist-info/LICENSE
+Filename: tpds_core-2.3.5.dist-info/LICENSE
 Comment: 
 
-Filename: tpds_core-2.3.4.dist-info/METADATA
+Filename: tpds_core-2.3.5.dist-info/METADATA
 Comment: 
 
-Filename: tpds_core-2.3.4.dist-info/WHEEL
+Filename: tpds_core-2.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: tpds_core-2.3.4.dist-info/entry_points.txt
+Filename: tpds_core-2.3.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: tpds_core-2.3.4.dist-info/top_level.txt
+Filename: tpds_core-2.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: tpds_core-2.3.4.dist-info/RECORD
+Filename: tpds_core-2.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tpds/api/__init__.py

```diff
@@ -1 +1,3 @@
 from .core import TpdsApiServer
+
+__all__ = ["TpdsApiServer"]
```

## tpds/api/core.py

```diff
@@ -18,18 +18,20 @@
 # THAT YOU HAVE PAID DIRECTLY TO MICROCHIP FOR THIS SOFTWARE.
 
 import threading
 import time
 
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
-from uvicorn import Config, Server
-
 from fastapi.responses import RedirectResponse
 from starlette.exceptions import HTTPException as StarletteHTTPException
+from uvicorn import Config, Server
+
+from tpds.configurator.api import configurator_api_router
+
 from .api.router import api_router
 from .api.usecases import usecase_router
 from .loader import load_app_root, load_usecases
 
 try:
     from tpds.version.core import __version__
 except ImportError:
@@ -69,14 +71,17 @@
 
     # Extend the app by loading usecases and plugins
     load_usecases(api_inst)
 
     # Attach the usecases
     api_inst.include_router(usecase_router, prefix="/usecases", tags=["Usecases"])
 
+    # Attach the configurator
+    api_inst.include_router(configurator_api_router, prefix="/config", tags=["Configurator"])
+
     # Attach the root application
     load_app_root(api_inst)
 
     # Exception handler for 404 Page
     @api_inst.exception_handler(StarletteHTTPException)
     async def custom_http_exception_handler(request, exc):
         return RedirectResponse("/")
```

## tpds/api/loader.py

```diff
@@ -16,36 +16,37 @@
 # FULLEST EXTENT ALLOWED BY LAW, MICROCHIP'S TOTAL LIABILITY ON ALL CLAIMS IN
 # ANY WAY RELATED TO THIS SOFTWARE WILL NOT EXCEED THE AMOUNT OF FEES, IF ANY,
 # THAT YOU HAVE PAID DIRECTLY TO MICROCHIP FOR THIS SOFTWARE.
 
 import importlib
 import os
 import sys
-
 from typing import Union
 
 from fastapi import FastAPI
 from fastapi.staticfiles import StaticFiles
 
 from tpds.helper import log
 from tpds.usecase_collector.collector import Collector
 from tpds.usecase_collector.usecase import Usecase, UsecaseEntrypoint
 
+
 def load_app_root(api_inst: FastAPI) -> None:
     try:
         import tpds.app_root
 
         app_root_path = tpds.app_root.__path__[0]
         # Mount the base web app - Must be the last operation
         api_inst.mount("", StaticFiles(directory=app_root_path, html=True), name="approot")
     except ImportError:
         log(
             "Unable to find the application root resources - dependency tpds-application-root is missing"
         )
 
+
 def _load_usecase(api_inst: FastAPI, usecase: Union[Usecase, UsecaseEntrypoint]) -> bool:
     backend = getattr(usecase, "backend", None)
     frontend = getattr(usecase, "frontend", None)
 
     if backend:
         if not all(item in sys.modules.keys() for item in backend.requires):
             return False
@@ -60,15 +61,15 @@
 
             # Import the backend as module
             module_inst = importlib.util.module_from_spec(spec)
 
             # Add the module to our global namespace so it's available for use
             sys.modules[spec.name] = module_inst
 
-            print(f'LOADING EXTENSION: {spec.name}')
+            print(f"LOADING EXTENSION: {spec.name}")
 
             # Excute the module (i.e. load and bring in all the imports)
             spec.loader.exec_module(module_inst)
 
             if routers := getattr(backend, "routers", None):
                 for router_name in routers:
                     router = getattr(module_inst, router_name, None)
@@ -93,14 +94,15 @@
             # The usecase should also have a frontend component - this will be attached as a static file
             api_inst.mount(
                 f"/{usecase.name}", StaticFiles(directory=fpath, html=True), name=usecase.name
             )
 
     return True
 
+
 def load_usecases(api_inst: FastAPI) -> None:
     remaining = list(Collector())
 
     while len(remaining):
         for usecase in remaining:
             if _load_usecase(api_inst, usecase):
                 remaining.remove(usecase)
```

## tpds/api/api/hw/api_board.py

```diff
@@ -15,26 +15,28 @@
 # HAS BEEN ADVISED OF THE POSSIBILITY OR THE DAMAGES ARE FORESEEABLE. TO THE
 # FULLEST EXTENT ALLOWED BY LAW, MICROCHIP'S TOTAL LIABILITY ON ALL CLAIMS IN
 # ANY WAY RELATED TO THIS SOFTWARE WILL NOT EXCEED THE AMOUNT OF FEES, IF ANY,
 # THAT YOU HAVE PAID DIRECTLY TO MICROCHIP FOR THIS SOFTWARE.
 
 import os
 from typing import List, Optional
+
 from fastapi import File, UploadFile
 from fastapi.routing import APIRouter
 from pykitinfo import pykitinfo
+from tpds.flash_program import FlashProgram
+
 from tpds.devices import TpdsBoards
 from tpds.devices.tpds_models import BoardDetails
-from tpds.flash_program import FlashProgram
 from tpds.helper import log
 
 router = APIRouter()
 
 
-@router.get('/get_details/{board_name}', response_model=Optional[BoardDetails])
+@router.get("/get_details/{board_name}", response_model=Optional[BoardDetails])
 def get_details(board_name: str):
     """
     Fetches the board details
 
     Parameters
     ----------
         board_name (str):       Name of the board as string
@@ -79,40 +81,32 @@
     -------
         Empty/board names based on what board are connected/recogonized
     """
     resp_boards = []
     all_kits = pykitinfo.detect_all_kits()
     for board, details in TpdsBoards().boards.items():
         if details.mcu_part_number and any(
-            details.mcu_part_number in
-                kit.get("debugger").get("device") for kit in all_kits
+            details.mcu_part_number in kit.get("debugger").get("device") for kit in all_kits
         ):
             resp_boards.append(board)
 
     return resp_boards
 
 
 @router.post("/program/{board_name}")
-async def program_hex_file(
-    board_name: str, factory_hex_path: Optional[UploadFile] = File(None)
-):
+async def program_hex_file(board_name: str, factory_hex_path: Optional[UploadFile] = File(None)):
     try:
         board_info = get_details(board_name)
         flash_program = FlashProgram(board_name, board_info)
-        assert flash_program.is_board_connected(), \
-            'Check the Kit parser board connections'
+        assert flash_program.is_board_connected(), "Check the Kit parser board connections"
         board_status = flash_program.check_board_status()
         log(f"Board Status: {board_status}")
-        if board_status != 'factory_programmed':
-            factory_hex_path = os.path.join(
-                board_info.board_path,
-                board_name,
-                f'{board_name}.hex')
-            assert factory_hex_path, \
-                'Factory hex is unavailable to program'
+        if board_status != "factory_programmed":
+            factory_hex_path = os.path.join(board_info.board_path, board_name, f"{board_name}.hex")
+            assert factory_hex_path, "Factory hex is unavailable to program"
             log(f"Factory hex path: {factory_hex_path}")
             status = flash_program.load_hex_image_with_ipe(factory_hex_path)
         else:
-            status = 'success'
+            status = "success"
     except BaseException as e:
         status = f"{e}"
     return status
```

## tpds/api/api/manifest_file/api_manifest.py

```diff
@@ -71,15 +71,15 @@
                 certificate_list.append(os.path.join(path, cert_file))
 
         result = None
         for certificate in certificate_list:
             try:
                 result = decoder(manifest, certificate)
                 break  # Since the verification is complete, breaking the loop
-            except VerificationError as exp:
+            except VerificationError:
                 continue
             except Exception as exp:
                 return {"message": "Error", "data": f"Manifest decoding is failed with: {exp}"}
 
         if result is None:
             return {
                 "message": "Verification is failed",
```

## tpds/api/api/package_manager/api_package_manager.py

```diff
@@ -14,40 +14,41 @@
 # OF ANY KIND WHATSOEVER RELATED TO THE SOFTWARE, HOWEVER CAUSED, EVEN IF
 # MICROCHIP HAS BEEN ADVISED OF THE POSSIBILITY OR THE DAMAGES ARE
 # FORESEEABLE. TO THE FULLEST EXTENT ALLOWED BY LAW, MICROCHIP'S TOTAL
 # LIABILITY ON ALL CLAIMS IN ANY WAY RELATED TO THIS SOFTWARE WILL NOT EXCEED
 # THE AMOUNT OF FEES, IF ANY, THAT YOU HAVE PAID DIRECTLY TO MICROCHIP FOR
 # THIS SOFTWARE.
 import os
-from fastapi.routing import APIRouter
-from tpds.package_manager.manager import PackageManager
-from fastapi import UploadFile
 from pathlib import Path
 from tempfile import NamedTemporaryFile
-from tpds.helper import log
-from tpds.app.vars import get_app_ref
-from tpds.settings.tpds_settings import reset_runtime_settings
 from typing import Union
 
+from fastapi import UploadFile
+from fastapi.routing import APIRouter
+from tpds.app.vars import get_app_ref
+
+from tpds.helper import log
+from tpds.package_manager.manager import PackageManager
+from tpds.settings.tpds_settings import reset_runtime_settings
 
 router = APIRouter()
 
 
 @router.get("/get_packages/{refresh}")
 def get_packages(refresh: bool = False):
     manager = PackageManager()
-    if (refresh):
+    if refresh:
         manager.refresh_package_list(True, True)
     packages = manager.get_packages()
     for pack in packages:
-        if (pack.installed and pack.latest):
+        if pack.installed and pack.latest:
             pack.isUpdated = pack.installed >= pack.latest
-        if (pack.installed):
+        if pack.installed:
             pack.installed = str(pack.installed)
-        if (pack.latest):
+        if pack.latest:
             pack.latest = str(pack.latest)
     return packages
 
 
 @router.post("/install/{packages}", response_model=int)
 def install_packages(packages: str):
     packages = packages.split(",")
@@ -66,18 +67,18 @@
     return PackageManager().getWheelDetails(wheelPath)
 
 
 @router.post("/shutdown/", response_model=bool)
 def shutdown():
     app_ref = get_app_ref()
     if app_ref._view:
-        log('shutdown')
+        log("shutdown")
         reset_runtime_settings()
         app_ref.stop_backend()
-        log('quitting')
+        log("quitting")
         app_ref.quit()
     else:
         return False
 
 
 async def getFilePath(tempFile: UploadFile) -> Union[str, os.PathLike]:
     contents = await tempFile.read()
```

## tpds/devices/devices_schema.yaml

```diff
@@ -1,13 +1,12 @@
 %YAML 1.1
 ---
 $schema: http://json-schema.org/draft-06/schema#
 $ref: "#/definitions/device_config"
-title:
-  Device Info YAML Schema
+title: Device Info YAML Schema
 definitions:
   device_config:
     title: device_config
     type: object
     additionalProperties: true
     properties:
       title:
@@ -26,19 +25,19 @@
     additionalProperties: True
     properties:
       basePart:
         type: string
       partLink:
         type:
           - string
-          - 'null'
+          - "null"
       toolLink:
         type:
           - string
-          - 'null'
+          - "null"
       provisioningFlow:
         anyOf:
           - $ref: "#/definitions/provisioningFlow"
           - type: object
             additionalProperties:
               type: array
               items:
@@ -49,15 +48,15 @@
           - Silicon
           - System-in-Package
       partInterface:
         $ref: "#/definitions/partInterface"
       productCategory:
         type:
           - string
-          - 'null'
+          - "null"
       tpdsRelease:
         type: boolean
       ndaRequired:
         type: boolean
     required:
       - basePart
       - provisioningFlow
@@ -73,40 +72,43 @@
       packagePin:
         type: string
       partInterface:
         $ref: "#/definitions/partInterface"
       memory:
         type:
           - string
-          - 'null'
+          - "null"
       media:
         type:
           - string
-          - 'null'
+          - "null"
       moq:
-        type: integer
+        anyOf:
+          - type: integer
+          - type: string
+          - type: "null"
         default: 0
       status:
         type:
           - string
-          - 'null'
+          - "null"
     required:
       - partNumber
       - deviceName
       - packagePin
   partInterface:
     type:
       - array
-      - 'null'
+      - "null"
     items:
       type: string
       enum:
         - i2c
         - spi
         - swi
   provisioningFlow:
-      title: ProvisioningFlow
-      enum: 
-        - TrustCUSTOM
-        - Trust&Go
-        - TrustFLEX
-      type: string
+    title: ProvisioningFlow
+    enum:
+      - TrustCUSTOM
+      - Trust&Go
+      - TrustFLEX
+    type: string
```

## tpds/devices/tpds_boards.py

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 import os
 from typing import Any, Mapping, Optional, Union
+
 from tpds.settings.validator import SettingsValidator
+
 from .tpds_models import BoardDetails
 
 try:
     from tpds.proto_boards import get_proto_board_data
 except ImportError:
     get_proto_board_data = None
 
@@ -24,16 +26,15 @@
         instance = super().__new__(cls)
         instance.__dict__ = cls.__shared_state
         return instance
 
     def __init__(self, schema: Optional[str] = None) -> None:
         if not self.__shared_state:
             if schema is None:
-                schema = str(os.path.join(
-                    os.path.dirname(__file__), "boards_schema.yaml"))
+                schema = str(os.path.join(os.path.dirname(__file__), "boards_schema.yaml"))
             super().__init__(schema)
 
 
 class TpdsBoards:
     """
     Global TPDS Device Information Store - acts as a singleton
     """
@@ -68,39 +69,35 @@
     @boards.setter
     def boards(self, values) -> None:
         _v, path = values
         for k, v in _v.items():
             v.update({"board_path": path})
             self._boards.update({k: BoardDetails(**v)})
 
-    def __add_board_info(
-            self, data: Union[Mapping, str, "os.PathLike[str]"]) -> None:
+    def __add_board_info(self, data: Union[Mapping, str, "os.PathLike[str]"]) -> None:
         if v_config := self.__validator.validated(data, True):
             if boards := v_config.get("boards", None):
                 self.boards = (boards, os.path.dirname(data))
 
     def __add_board_info_from_dir(self, dir: "os.PathLike[str]") -> None:
         for name in os.listdir(dir):
             _, ext = os.path.splitext(name)
-            if ext.lower() in [".yaml", ".yml"] and os.path.isfile(
-                    path := os.path.join(dir, name)):
+            if ext.lower() in [".yaml", ".yml"] and os.path.isfile(path := os.path.join(dir, name)):
                 self.__add_board_info(path)
 
-    def add_board_info(
-            self, data: Union[Mapping, str, "os.PathLike[str]"]) -> None:
+    def add_board_info(self, data: Union[Mapping, str, "os.PathLike[str]"]) -> None:
         if isinstance(data, Mapping):
             self.__add_board_info(data)
         elif os.path.exists(data):
             if os.path.isfile(data):
                 self.__add_board_info(data)
             else:
                 self.__add_board_info_from_dir(data)
 
-    def get_board_info(
-            self, board_name: str) -> Optional[BoardDetails]:
+    def get_board_info(self, board_name: str) -> Optional[BoardDetails]:
         for board, details in self.boards.items():
             if board == board_name:
                 return details
         return None
 
 
 __all__ = ["TpdsBoards", "TpdsBoardValidator"]
```

## tpds/devices/tpds_devices.py

```diff
@@ -109,8 +109,8 @@
         elif os.path.exists(data):
             if os.path.isfile(data):
                 self.__add_device_info(data)
             else:
                 self.__add_device_info_from_dir(data)
 
 
-__all__ = ["TpdsDevices", "DeviceDetails", "DevicePartDetails", "DeviceInterface"]
+__all__ = ["TpdsDevices"]
```

## tpds/devices/tpds_models.py

```diff
@@ -53,16 +53,15 @@
     # Trust&Go Project Categories
     tng: Optional[Sequence[str]]
     # Trust Flex Project Categories
     tflex: Optional[Sequence[str]]
 
     class Config:
         allow_population_by_field_name = True
-        fields = {
-            "tcsm": "TrustCUSTOM", "tng": "Trust&Go", "tflex": "TrustFLEX"}
+        fields = {"tcsm": "TrustCUSTOM", "tng": "Trust&Go", "tflex": "TrustFLEX"}
 
 
 class DeviceDetails(BaseModel):
     """
     TPDS Device Details
     """
 
@@ -193,21 +192,20 @@
     # Target MCU device
     mcu_part_number: Optional[str]
     # Name of the programming tool to use
     program_tool: Optional[str]
     # Kit Protocol parser application HID-USB PID
     kit_parser_pid: Optional[int] = 8978
     # Kit Protocol parser application version
-    kit_parser_version: Optional[str] = '0.0.0'
+    kit_parser_version: Optional[str] = "0.0.0"
     # kit_name
     kit_name: Optional[str] = ""
     # product string
     product_string: Optional[str] = ""
     # board path
     board_path: Union[str, None]
     # Connection Details
     # Should use a discriminator field here but
     # it won't get fixed until pydantic 1.9.1
-    connection: Union[
-        BoardConnectionHid, BoardConnectionUart, BoardConnectionBridge, None]
+    connection: Union[BoardConnectionHid, BoardConnectionUart, BoardConnectionBridge, None]
     # Connected Devices
     devices: Optional[Sequence[BoardDeviceDetails]]
```

## tpds/devices/data/ecc608-tflx.yaml

```diff
@@ -8,25 +8,14 @@
     partType: Silicon
     productCategory: Secure Element
     partInterface:
       - i2c
       - swi
     tpdsRelease: Yes
     ndaRequired: No
-  ATECC608B-TFLXLORA:
-    basePart: ATECC608B
-    partLink:
-    provisioningFlow: TrustFLEX
-    partType: Silicon
-    productCategory: Secure Element
-    partInterface:
-      - i2c
-      - swi
-    tpdsRelease: Yes
-    ndaRequired: No
 parts:
   - partNumber: ATECC608B-TFLXTLSU-Proto
     deviceName: ATECC608B-TFLXTLS
     packagePin: UDFN-8
     memory: N/A
     media: Bag
     moq: 10
@@ -48,35 +37,7 @@
   - partNumber: ATECC608B-TFLXTLSS
     deviceName: ATECC608B-TFLXTLS
     packagePin: SOIC-8
     memory: N/A
     media: Reel
     moq: 2000
     status: Production
-  - partNumber: ATECC608B-TFLXLORAU-Proto
-    deviceName: ATECC608B-TFLXLORA
-    packagePin: UDFN-8
-    memory: N/A
-    media: Bag
-    moq: 10
-    status: Contact local Sales
-  - partNumber: ATECC608B-TFLXLORAS-Proto
-    deviceName: ATECC608B-TFLXLORA
-    packagePin: SOIC-8
-    memory: N/A
-    media: Bag
-    moq: 10
-    status: Contact local Sales
-  - partNumber: ATECC608B-TFLXLORAU
-    deviceName: ATECC608B-TFLXLORA
-    packagePin: UDFN-8
-    memory: N/A
-    media: Reel
-    moq: 2000
-    status: Contact local Sales
-  - partNumber: ATECC608B-TFLXLORAS
-    deviceName: ATECC608B-TFLXLORA
-    packagePin: SOIC-8
-    memory: N/A
-    media: Reel
-    moq: 2000
-    status: Contact local Sales
```

## tpds/devices/data/sha204.yaml

```diff
@@ -1,29 +1,29 @@
 ---
 title: SHA204 Device Information
 devices:
   ATSHA204A-TCSM:
     basePart: ATSHA204A
-    partLink: https://www.microchip.com/wwwproducts/eN/ATSHA204A-TCSM
+    partLink: https://www.microchip.com/en-us/product/ATSHA204A-TCSM
     provisioningFlow: TrustCUSTOM
     partType: Silicon
     partInterface:
       - i2c
       - swi
     productCategory: Secure Element
-    tpdsRelease: No
-    ndaRequired: No
+    tpdsRelease: Yes
+    ndaRequired: Yes
   ATSHA204A-RBHCZ:
     basePart: ATSHA204A
-    partLink: null
+    partLink: https://www.microchip.com/en-us/product/ATSHA204A-TCSM
     provisioningFlow: TrustCUSTOM
     partType: Silicon
     productCategory: Secure Element
-    tpdsRelease: No
-    ndaRequired: No
+    tpdsRelease: Yes
+    ndaRequired: Yes
 parts:
   - partNumber: ATSHA204A-TCSMS
     deviceName: ATSHA204A-TCSM
     packagePin: SOIC-8
     memory: N/A
     media: Reel
     moq: 4000
@@ -31,14 +31,14 @@
   - partNumber: ATSHA204A-TCMSU
     deviceName: ATSHA204A-TCSM
     packagePin: UDFN-8
     memory: N/A
     media: Reel
     moq: 4000
     status: Under NDA
-  - partNumber: ATSHA204A-RBHCZ-T
-    deviceName: ATSHA204A-RBHCZ       
+  - partNumber: ATSHA204A-RBHCZ
+    deviceName: ATSHA204A-RBHCZ
     packagePin: RBH 3-pin contact
     memory: N/A
     media: Reel
-    moq: 45000
-    status: Production
+    moq:
+    status: Under NDA
```

## tpds/devices/data/ta100.yaml

```diff
@@ -1,13 +1,13 @@
 ---
 title: TA100 Device Information
 devices:
   TA100:
     basePart: TA100
-    partLink: https://www.microchip.com/wwwproducts/en/ta100
+    partLink: https://www.microchip.com/en-us/product/ta100
     toolLink: https://www.microchip.com/en-us/product/SW-TA100
     provisioningFlow: TrustCUSTOM
     partType: Silicon
     productCategory: Secure Element
     partInterface:
       - i2c
       - spi
@@ -17,25 +17,25 @@
   - partNumber: TA100T-Y240C2X01
     deviceName: TA100
     packagePin: SOIC-8
     partInterface:
       - i2c
     memory: N/A
     media: Reel
-    moq: 4000
+    moq: 3300
     status: Under NDA
   - partNumber: TA100-Y240C2X01
     deviceName: TA100
     packagePin: SOIC-8
     partInterface:
       - spi
     memory: N/A
     media: Reel
-    moq: 4000
+    moq: 3300
     status: Under NDA
   - partNumber: TA100-Y240UFB01
     deviceName: TA100
     packagePin: VQFN-24
     memory: N/A
     media: Reel
-    moq: 4000
+    moq: 3300
     status: Under NDA
```

## tpds/helper/__init__.py

```diff
@@ -1,7 +1,20 @@
 """
     Trust Platform Design Suite Helper module
 """
 
-from .logger import *
-from .processing import *
-from .utils import *
+from .logger import LogFacility, log
+from .processing import ErrorHandling, ProcessingUtils
+from .singleton import make_singleton
+from .utils import TableIterator, checkIfProcessRunning, make_dir, merge_dicts
+
+__all__ = [
+    "LogFacility",
+    "log",
+    "ProcessingUtils",
+    "ErrorHandling",
+    "make_singleton",
+    "checkIfProcessRunning",
+    "make_dir",
+    "merge_dicts",
+    "TableIterator",
+]
```

## tpds/helper/logger.py

```diff
@@ -22,15 +22,14 @@
     def __init__(
         self,
         logfile: Union[str, os.PathLike[str], None] = None,
         level: int = logging.DEBUG,
         logstream: bool = True,
         logformat: str = _default_log_format,
     ) -> None:
-
         if not hasattr(self, "_callback"):
             self._callback: Union[Callable[[str], None], None] = None
         if not hasattr(self, "_log"):
             self._log = logging.getLogger("tpds")
             self._log.setLevel(level)
 
         if not hasattr(self, "_formatter"):
```

## tpds/helper/utils.py

```diff
@@ -30,18 +30,18 @@
     curr_dir = os.getcwd()
     try:
         temp_file = "temp.txt"
         if not os.path.exists(path):
             os.makedirs(path)
         os.chdir(path)
         with open(temp_file, "w") as temp:
-            pass
+            temp.close()
     except PermissionError:
         raise PermissionError(f"Please check permission for {path} folder")
-    except:
+    except:  # noqa E722
         raise RuntimeError(f"Unknown error occurred when accessing {path} folder")
     finally:
         os.remove(temp_file) if os.path.exists(temp_file) else None
         os.chdir(curr_dir)
 
 
 def merge_dicts(
```

## tpds/launcher/__init__.py

```diff
@@ -1 +1,3 @@
-from .start import *
+from .start import TpdsBackend, launch_tpds_core
+
+__all__ = ["launch_tpds_core", "TpdsBackend"]
```

## tpds/package_manager/__init__.py

```diff
@@ -1,6 +1,8 @@
 """
 Package manager
 """
 
 from .data_models import PackageDetails
 from .manager import PackageManager, prettify_channel
+
+__all__ = ["PackageDetails", "PackageManager", "prettify_channel"]
```

## tpds/package_manager/data_models.py

```diff
@@ -1,18 +1,14 @@
 from __future__ import annotations
 
-from typing import Mapping, Optional, Sequence, Union, Dict
+from typing import Dict, Mapping, Optional, Sequence, Union
 
 from packaging.version import VERSION_PATTERN, Version
 from pydantic import BaseModel
 
-try:
-    from packaging.version import LegacyVersion
-except ImportError:
-    LegacyVersion = Version
 
 class SemVer(Version):
     """
     Wrap python packaging version with a pydantic validator class
     """
 
     @classmethod
@@ -64,70 +60,12 @@
     license_text: Optional[str]
     # Dependencies
     dependencies: Sequence[PackageDependencies] = []
     # Optional Dependencies
     extras: Union[Mapping[str, PackageDependencies], Dict] = {}
 
 
-class CondaInfoModel(BaseModel):
-    # Configured channels of the conda system
-    channels: Sequence[str]
-    # Configured environments
-    envs: Sequence[str]
-
-
 class TpdsPackagingModel(BaseModel):
     # Required Packages
     required: PackageDependencies = PackageDependencies()
     # Conditional Packages depending on the feature
     optional: Optional[Mapping[str, Sequence[str]]] = {}
-
-
-class CondaAboutExtraModel(BaseModel):
-    # Trust Platform specific metadata
-    tpds: Optional[TpdsPackagingModel] = TpdsPackagingModel()
-
-
-class CondaAboutModel(BaseModel):
-    channels: Sequence[str]
-    conda_build_version: Optional[str] = None
-    conda_private: bool
-    conda_version: Optional[str] = None
-    env_vars: Mapping[str, str] = {}
-    extra: Optional[CondaAboutExtraModel]
-    home: Optional[str] = None
-    identifiers: Optional[Sequence[str]] = []
-    keywords: Optional[Sequence[str]] = []
-    license: Optional[str] = None
-    license_file: Union[str, Sequence[str], None] = None
-    summary: Optional[str] = None
-    tags: Optional[Sequence[str]] = None
-
-
-class CondaPackageDetails(BaseModel):
-    # Package Name
-    name: str
-    # Source Channel
-    channel: str
-    # Version
-    version: SemVer
-    # Conda build
-    build_number: int
-    # Conda build identifier
-    build_string: Optional[str]
-    # Is the package a conda updatable package
-    updateable: Optional[bool] = False
-    # Conda Package Dependencies - conda installer will manage these
-    depends: Optional[Sequence[str]]
-    # License Type Summary
-    license: Optional[str]
-    # Additional Package Information
-    about: Optional[CondaAboutModel] = None
-
-    class Config:
-        allow_population_by_field_name = True
-        fields = {"build_string": "build"}
-
-
-class CondaSearchModel(BaseModel):
-    # List of Packages
-    packages: Mapping[str, Sequence[CondaPackageDetails]]
```

## tpds/package_manager/manager.py

```diff
@@ -11,22 +11,23 @@
     from tabulate import tabulate
 except ImportError:
     pass
 
 from importlib.metadata import metadata
 from typing import Any, Iterator, MutableMapping, Sequence, Union
 from zipfile import ZipFile
+
 from packaging.utils import parse_wheel_filename
+from tpds.tp_utils.tp_settings import TPSettings
 
 # Trust Platform Modules
 from tpds.helper import ProcessingUtils, TableIterator
 from tpds.helper.logger import LogFacility
 from tpds.settings.tpds_settings import TrustPlatformSettings
 from tpds.settings.validator import SettingsValidator
-from tpds.tp_utils.tp_settings import TPSettings
 
 # Package Manager Modules
 from .data_models import PackageDetails
 from .pip_client import PipPackageClient
 
 # List of exposed objects
 __all__ = ["PackageManager", "prettify_channel"]
@@ -208,18 +209,18 @@
                 installed.latest = avail.latest
                 if installed.license is None:
                     installed.license = avail.license
                 if installed.license_text is None:
                     installed.license_text = avail.license_text
             else:
                 self._packages[avail.name] = avail
-    
+
     def get_proc(self):
         return self._proc
-    
+
     def get_default_license(self):
         return self.__licenses.get("Proprietary")
 
     def refresh_package_list(self, local: bool = True, remote: bool = True, **kwargs: Any) -> None:
         self._logger.log(f"Refreshing package lists - local: {local}, remote: {remote}")
         for name, c in self._clients.items():
             self._logger.log(f"Refreshing {name} package lists - local: {local}, remote: {remote}")
@@ -281,21 +282,25 @@
         """
         return self._clients["pypi"].install(packages, **kwargs)
 
     def install_tpds_extn(self, zipPath: Union[str, os.PathLike]) -> int:
         """
         Install TPDS Extension From zip file
         """
-        workingDir = os.path.join(TPSettings().get_base_folder(), 'tpds_extn_install')
+        workingDir = os.path.join(TPSettings().get_base_folder(), "tpds_extn_install")
         os.makedirs(workingDir, exist_ok=True)
         if not zipPath:
             return None
         returncode = 0
-        with ZipFile(os.path.normpath(zipPath), 'r') as zipObject:
-            whlFiles = [zipObject.extract(fileName, workingDir) for fileName in zipObject.namelist() if fileName.endswith('.whl')]
+        with ZipFile(os.path.normpath(zipPath), "r") as zipObject:
+            whlFiles = [
+                zipObject.extract(fileName, workingDir)
+                for fileName in zipObject.namelist()
+                if fileName.endswith(".whl")
+            ]
             if len(whlFiles):
                 returncode += self.install(whlFiles, refresh=False)
         return returncode
 
     def get_packages_formatted(self) -> str:
         return tabulate(
             TableIterator(
@@ -303,18 +308,22 @@
                 ["name", ("channel", prettify_channel), "installed", "latest"],
             ),
             headers=self.__headers,
         )
 
     def getWheelDetails(self, zipPath: Union[str, os.PathLike]):
         packages_info = []
-        workingDir = os.path.join(TPSettings().get_base_folder(), 'tpds_extn_install')
+        workingDir = os.path.join(TPSettings().get_base_folder(), "tpds_extn_install")
         os.makedirs(workingDir, exist_ok=True)
-        with ZipFile(os.path.normpath(zipPath), 'r') as zipObject:
-            whlFiles = [zipObject.extract(fileName, workingDir) for fileName in zipObject.namelist() if fileName.endswith('.whl')]
+        with ZipFile(os.path.normpath(zipPath), "r") as zipObject:
+            whlFiles = [
+                zipObject.extract(fileName, workingDir)
+                for fileName in zipObject.namelist()
+                if fileName.endswith(".whl")
+            ]
             if len(whlFiles):
                 for whlFile in whlFiles:
                     name, version, _, _ = parse_wheel_filename(os.path.basename(whlFile))
                     packages_info.append({"name": name, "latest": str(version)})
         return packages_info
```

## tpds/package_manager/pip_client.py

```diff
@@ -122,46 +122,49 @@
             self._log.log(f"{package_name}: No info found")
         return details
 
     def update_remote(self, **kwargs: Any) -> None:
         """
         Retrieve the list of available packages and their versions
         """
-        if 'microchip.com' in self._index:
+        if "microchip.com" in self._index:
             search_list = list(filter(lambda x: x.startswith("tpds"), self._installed.keys()))
             search_list += list(self._search_list.keys())
             search_list = list(set(search_list))
         else:
             search_list = list(self._search_list.keys())
 
         with ThreadPoolExecutor() as exec:
             for p in exec.map(self._pip_get_package_data, search_list):
                 if p:
                     self._available[p.name] = p
 
-    def install(self, packages: Sequence[str], **kwargs: Any) -> None:
+    def install(self, packages: Sequence[str], upgrade: bool = False, **kwargs: Any) -> None:
         """
         Install the selected packages and their dependencies
         """
-        cmd = self.__cmdBase + ["install", "--upgrade"]
-        if TrustPlatformSettings().settings.develop:
-            cmd += ["--pre"]
+        cmd = self.__cmdBase + ["install"]
         if self._index:
             cmd += ["-i", self._index]
-        cmd += packages
+        if TrustPlatformSettings().settings.develop:
+            cmd += [f"{p}=={self._available[p].latest}" for p in packages]
+        else:
+            if upgrade:
+                cmd += ["--upgrade"]
+            cmd += packages
         outs, returncode = self._proc.run_cmd(cmd, err_handling=self._proc.LOG, **kwargs)
         self._log.log(outs)
         self.update_local()
         return returncode
 
     def upgrade(self, packages: Sequence[str], **kwargs: Any) -> None:
         """
         Upgrade the selected packages to the latest versions
         """
-        self.install(packages, **kwargs)
+        self.install(packages, upgrade=True, **kwargs)
 
     def update_dependency_list(
         self, packages: Union[str, Sequence[str]], channel: Optional[str] = None, **kwargs: Any
     ) -> PackageDependencies:
         """
         Dependencies are listed as part of additional metadata so we need to retrieve
         that information first before we execute additional steps
```

## tpds/servers/__init__.py

```diff
@@ -1,8 +1,10 @@
 """
 Trust Platform Design Suite servers modules
 """
 
 from .jupyter_server import JupyterServer
-from .msg_handler import *
+from .msg_handler import Messages, TpdsMessage, op_codes
 from .uno_server import UnoServer
 from .websocket_server import WebSocketServer
+
+__all__ = ["JupyterServer", "Messages", "TpdsMessage", "op_codes", "UnoServer", "WebSocketServer"]
```

## tpds/servers/msg_handler.py

```diff
@@ -28,17 +28,17 @@
     ta_provisioningXML_handle,
     ta_uno_appJSON,
     ta_uno_config_handle,
 )
 from .msg_handler_tcustom import trust_custom_read_config, trust_custom_write_config
 from .msg_handler_tflx import tflx_proto_provisioning_handle, tflx_provisioningXML_handle
 from .msg_handler_tflx_ecc204 import tflex_ecc204_json_handle, tflxecc204_proto_prov_handle
-from .symm_auth_user_inputs import SymmAuthUserInputs
-from .wpc_user_inputs import WPCUserInputs
 from .provision_user_inputs import ProvisionUserInputs
+from .symm_auth_user_inputs import SymmAuthUserInputs, Sha10xSymmAuthUserInputs
+from .wpc_user_inputs import WPCUserInputs
 
 
 def default(args):
     return {"response": "unrecognized command", "status": "error"}
 
 
 class Messages:
@@ -156,15 +156,15 @@
         file_filter = "("
         for arg in args[1]:
             file_filter += f"{arg} "
         file_filter += ")"
         log(f"File filter: {file_filter}")
         log(args[2])
         dlg = QFileDialog(None, caption=args[0], filter=file_filter, directory=args[2])
-        result = dlg.exec_()
+        result = dlg.exec()
         if result == QDialog.Accepted:
             filepath = dlg.selectedFiles()[0]
         log(filepath)
         return "OK", filepath
 
     return "error", "insufficient args"
 
@@ -191,15 +191,15 @@
 @TpdsMessage(str, str)
 def user_message_box(ctx, title, text):
     msg_box = QMessageBox()
     msg_box.setIcon(QMessageBox.Information)
     msg_box.setWindowTitle(title)
     msg_box.setText(text)
     msg_box.setStandardButtons(QMessageBox.Ok | QMessageBox.Cancel)
-    reply = msg_box.exec_()
+    reply = msg_box.exec()
     response = "OK" if reply == QMessageBox.Ok else "Cancel"
     return "OK", response
 
 
 @TpdsMessage(str, str)
 def tflex_provisioningXML(ctx, data):
     tflx_provisioningXML_handle(json.dumps(json.loads(data)))
@@ -247,29 +247,36 @@
     tflxecc204_proto_prov_handle(config)
     return "OK", ""
 
 
 @TpdsMessage(list)
 def symm_auth_user_inputs(ctx, args):
     obj = SymmAuthUserInputs()
-    obj.exec_()
+    obj.exec()
+    return "OK", f"{obj.user_data}"
+
+
+@TpdsMessage(list)
+def sha10x_symm_auth_user_inputs(ctx, args):
+    obj = Sha10xSymmAuthUserInputs()
+    obj.exec()
     return "OK", f"{obj.user_data}"
 
 
 @TpdsMessage(list)
 def wpc_user_inputs(ctx, args):
     obj = WPCUserInputs()
-    obj.exec_()
+    obj.exec()
     return "OK", f"{obj.user_data}"
 
 
 @TpdsMessage(list)
 def provision_inputs(ctx, args):
     obj = ProvisionUserInputs(xml_type=args[0], cert_type=args[1])
-    obj.exec_()
+    obj.exec()
     return "OK", f"{obj.user_data}"
 
 
 @TpdsMessage(str)
 def open_explorer_folder(ctx, path):
     try:
         if sys.platform == "darwin":
@@ -320,15 +327,15 @@
         display_msg = (
             f"<font color=#0000ff><b>{configurator_title} Configurator"
             f"</b></font><br><br>"
             f"Package is not found locally.  If package access is already granted, Click Cancel and Update from Package Manager. \
             If package access is required, Click OK to request from Microchip. <br>"
         )
         msg_box.setText(display_msg)
-        reply = msg_box.exec_()
+        reply = msg_box.exec()
 
         pdir = directory
         if reply == QMessageBox.Cancel:
             pdir = ""
     return "OK", pdir
 
 
@@ -385,12 +392,15 @@
     16: tcustom_608_config_rw,
     17: open_default_browser,
     18: user_message_box,
     20: tflex_ecc204_json,
     21: tflex_ecc204_proto_prov,
     40: symm_auth_user_inputs,
     41: wpc_user_inputs,
+    42: sha10x_symm_auth_user_inputs,
     50: provision_inputs,
     80: ta_appJSON,
     81: ta_uno_provisioningXML,
     82: ta_uno_get_config,
 }
+
+__all__ = ["Messages", "TpdsMessage", "op_codes"]
```

## tpds/servers/msg_handler_ta.py

```diff
@@ -8,15 +8,15 @@
 from pathlib import Path
 from zipfile import ZipFile
 
 from PySide6.QtCore import QDir, Slot
 from PySide6.QtWidgets import QDialog, QFileDialog, QMessageBox
 from tpds.output_grabber.library_output_grabber import LibraryOutputGrabber
 
-from tpds.helper import *
+from tpds.helper import checkIfProcessRunning, log, make_dir
 from tpds.settings import TrustPlatformSettings
 
 try:
     import cryptoauthlib_ta as cal
 except (ModuleNotFoundError, ImportError):
     import cryptoauthlib as cal
 
@@ -102,15 +102,15 @@
 @Slot(str)
 def ta_open_app_handle(args):
     msg_box = QMessageBox()
     msg_box.setIcon(QMessageBox.Information)
     msg_box.setStandardButtons(QMessageBox.Ok)
     msg_box.setWindowTitle("TA Configurator")
 
-    conf = settings.TrustPlatformSettings()
+    conf = TrustPlatformSettings()
     ta_config_dir = os.path.join(conf.settings.conda_path, "TA_Configurator")
     if os.path.exists(ta_config_dir):
         cmd = [
             os.path.join(ta_config_dir, "TaConfigurator.UI.exe"),
             "-config",
             os.path.join(ta_config_dir, "sample.taconfig"),
         ]
@@ -342,17 +342,16 @@
 
 
 ta_config_file_json_str = ""
 
 
 @Slot(str)
 def ta_uno_config_handle(config_file):
-
     global ta_config_file_json_str
-    conf = settings.TrustPlatformSettings()
+    conf = TrustPlatformSettings()
     config_file = os.path.join(conf.settings.conda_path, "TA_Configurator", "SampleConfig.taconfig")
 
     config_info = {}
     if os.path.exists(config_file):
         config_info.update({"title": Path(config_file).name})
         config_info.update({"content": Path(config_file).read_text("'utf-8-sig'")})
     ta_config_file_json_str = json.dumps(config_info)
```

## tpds/servers/msg_handler_tflx.py

```diff
@@ -66,17 +66,15 @@
             if reply == QMessageBox.Yes:
                 log("Getting Root Key")
                 cert_dlg = QFileDialog(None, caption="Select your Root Key", filter="*.key")
                 cert_file = cert_dlg.exec()
                 if cert_file == QDialog.Accepted:
                     signer_ca_key = cert_dlg.selectedFiles()[0]
                     log("Getting signer Key")
-                    cert_dlg = QFileDialog(
-                        None, caption="Select your Signer Key", filter="*.key"
-                    )
+                    cert_dlg = QFileDialog(None, caption="Select your Signer Key", filter="*.key")
                     cert_file = cert_dlg.exec()
                     if cert_file == QDialog.Accepted:
                         device_ca_key = cert_dlg.selectedFiles()[0]
 
             log("Provisioning the prototype board")
             provision = ProtoProvisioning(id, xml_file_in)
             log(f"Device details: {provision.element.get_device_details()}")
```

## tpds/servers/msg_handler_tflx_ecc204.py

```diff
@@ -1,20 +1,18 @@
 import glob
 import json
 import os
-from ctypes import byref, c_char_p, c_uint8, c_void_p, cast
 from datetime import datetime
 from pathlib import Path
 
 import cryptoauthlib as cal
 from PySide6.QtCore import QDir, Qt, Slot
 from PySide6.QtWidgets import QDialog, QFileDialog, QMessageBox
 from tpds.certs.tflex_certs import TFLEXCerts
 from tpds.proto_provision.ecc204_provision import ECC204Provision
-from tpds.secure_element import Constants
 from tpds.tp_utils.tp_keys import TPAsymmetricKey
 from tpds.tp_utils.tp_utils import add_to_zip_archive
 
 from tpds.helper import log, utils
 
 
 def ecc204_tflxauth_certs(
@@ -77,19 +75,19 @@
             time_stamp = datetime.now().strftime("%m%d%H%M%S")
             certs_zip_f = f"{device_name}_{time_stamp}.zip"
             os.chdir(certs_zip_dir)
 
             certs = ecc204_tflxauth_certs(cert_data, device_sn=cert_data.get("d_cert_cn"))
             certs.save_tflex_c_definitions()
             certs_txt = (
-                certs.root.get_certificate_in_text() +
-                "\n\n" +
-                certs.signer.get_certificate_in_text() +
-                "\n\n" +
-                certs.device.get_certificate_in_text()
+                certs.root.get_certificate_in_text()
+                + "\n\n"
+                + certs.signer.get_certificate_in_text()
+                + "\n\n"
+                + certs.device.get_certificate_in_text()
             )
             Path("custom_certs.txt").write_text(certs_txt)
             Path("root.crt").write_bytes(certs.root.get_certificate_in_pem())
             Path("signer.crt").write_bytes(certs.signer.get_certificate_in_pem())
             Path("device.crt").write_bytes(certs.device.get_certificate_in_pem())
 
             for extn in ["*.c", "*.h", "*.crt", "*.txt"]:
@@ -133,19 +131,21 @@
         cfg.cfg.atcahid.dev_identity = 0x66
         cfg.devtype = cal.get_device_type_id("ECC204")
         if data.get("interface") == "i2c":
             cfg.cfg.atcahid.dev_interface = int(cal.ATCAKitType.ATCA_KIT_I2C_IFACE)
         else:
             cfg.cfg.atcahid.dev_interface = int(cal.ATCAKitType.ATCA_KIT_SWI_IFACE)
 
-        ecc204_test_config = bytes.fromhex("""
+        ecc204_test_config = bytes.fromhex(
+            """
             8F F3 19 8B A3 3A E2 B2  58 00 01 00 00 00 00 00
             0F 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00
             00 00 00 00 FF FF FF FF  FF FF FF FF FF FF FF FF
-            33 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00""")
+            33 00 00 00 00 00 00 00  00 00 00 00 00 00 00 00"""
+        )
         ecc204_proto_provision = ECC204Provision(cfg)
         ecc204_proto_provision.element.load_tflx_test_config(ecc204_test_config)
 
         device_public_key = bytearray()
         assert (
             cal.atcab_get_pubkey(0, device_public_key) == cal.Status.ATCA_SUCCESS
         ), "Reading Public Key failed"
@@ -176,17 +176,15 @@
             if reply == QMessageBox.Yes:
                 log("Getting root Key")
                 cert_dlg = QFileDialog(None, caption="Select your Root Key", filter="*.key")
                 cert_file = cert_dlg.exec()
                 if cert_file == QDialog.Accepted:
                     signer_ca_key = cert_dlg.selectedFiles()[0]
                     log("Getting signer Key")
-                    cert_dlg = QFileDialog(
-                        None, caption="Select your Signer Key", filter="*.key"
-                    )
+                    cert_dlg = QFileDialog(None, caption="Select your Signer Key", filter="*.key")
                     cert_file = cert_dlg.exec()
                     if cert_file == QDialog.Accepted:
                         device_ca_key = cert_dlg.selectedFiles()[0]
 
             if signer_ca_key is None:
                 signer_ca_key = os.path.join(
                     str(QDir.homePath()), "Downloads", "TPDS_Downloads", "proto_root.key"
```

## tpds/servers/provision_user_inputs.py

```diff
@@ -1,22 +1,22 @@
 import sys
 
 from PySide6.QtCore import Slot
 from PySide6.QtWidgets import (
     QApplication,
+    QDialog,
+    QFileDialog,
     QHBoxLayout,
     QLabel,
     QLineEdit,
     QMessageBox,
     QPushButton,
     QSizePolicy,
     QSpacerItem,
     QVBoxLayout,
-    QDialog,
-    QFileDialog,
 )
 
 
 class ProvisionUserInputs(QDialog):
     """
     TrustFlex provisional XML Dialog to get all the user input for processing
     """
@@ -51,16 +51,15 @@
                     self.csr_zip_button.setEnabled(False)
                     self.ca_key_lineedit.setEnabled(False)
                     self.ca_key_button.setEnabled(False)
                 self.show()
             else:
                 self.close()
         except BaseException:
-            QMessageBox.warning(
-                self, "Error", "Invalid config : xml_type not found")
+            QMessageBox.warning(self, "Error", "Invalid config : xml_type not found")
             self.close()
 
     def setup_UI(self):
         """
         Function to setup UI
         """
         # Set Window title
@@ -71,16 +70,15 @@
         # Label for encryption key choosing
         self.encryption_key_label = QLabel()
         self.encryption_key_label.setText(
             """Encryption Key - Load encryption key .pem file provided by Microchip"""
         )
         # Label for csr_zip choosing
         self.csr_zip_label = QLabel()
-        self.csr_zip_label.setText(
-            """\nCSR ZIP - Load CSRs zip file provided by Microchip""")
+        self.csr_zip_label.setText("""\nCSR ZIP - Load CSRs zip file provided by Microchip""")
         # Label for CA_Key choosing
         self.ca_key_label = QLabel()
         self.ca_key_label.setText(
             """\nCA Key (optional) - Load CA Key to sign CSRs.
             If Key is provided, tool signs the CSRs and generates final package.
             If Key is not provided, tool generates Sign CSR package to sign CSRs offline.
                     Refer to readme.md in the .zip file for signing instructions."""
@@ -109,16 +107,15 @@
         # Window OK button
         self.ok_button = QPushButton()
         self.ok_button.setText("OK")
         # Window Cancel button
         self.cancel_button = QPushButton()
         self.cancel_button.setText("Cancel")
         # Define Layout
-        ok_close_spacer = QSpacerItem(
-            200, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        ok_close_spacer = QSpacerItem(200, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
         # Setup Hlayouts for individual horizontal items
         enc_H = QHBoxLayout()
         enc_H.addWidget(self.encryption_key_lineedit)
         enc_H.addWidget(self.encryption_key_button)
         csr_H = QHBoxLayout()
         csr_H.addWidget(self.csr_zip_lineedit)
         csr_H.addWidget(self.csr_zip_button)
@@ -141,16 +138,15 @@
         vlay.addLayout(ok_close_H)
         # Set Layout
         self.setLayout(vlay)
 
     @Slot()
     def setup_singals_slots(self):
         # Setup slots for file select buttons
-        self.encryption_key_button.clicked.connect(
-            self.encryption_file_callback)
+        self.encryption_key_button.clicked.connect(self.encryption_file_callback)
         self.csr_zip_button.clicked.connect(self.csr_zip_file_callback)
         self.ca_key_button.clicked.connect(self.ca_key_file_callback)
         # Setup slot for close button
         self.cancel_button.clicked.connect(self.close_app)
         # Setup slot for OK button
         self.ok_button.clicked.connect(self.process_ok)
 
@@ -191,17 +187,17 @@
     @Slot()
     def process_ok(self):
         enc_key_file = self.encryption_key_lineedit.text()
         csr_zip_file = self.csr_zip_lineedit.text()
         ca_key_file = self.ca_key_lineedit.text()
 
         # user data
-        self.user_data.update({'enc_key_file': enc_key_file})
-        self.user_data.update({'csr_zip_file': csr_zip_file})
-        self.user_data.update({'ca_key_file': ca_key_file})
+        self.user_data.update({"enc_key_file": enc_key_file})
+        self.user_data.update({"csr_zip_file": csr_zip_file})
+        self.user_data.update({"ca_key_file": ca_key_file})
 
         self.close()
 
     @Slot()
     def process_cancel(self):
         self.user_data.clear()
         self.close()
```

## tpds/servers/symm_auth_user_inputs.py

```diff
@@ -1,12 +1,12 @@
 import os
 import sys
 
-from PySide6.QtCore import QRegularExpression #QRegExp
-from PySide6.QtGui import QRegularExpressionValidator #QRegExpValidator
+from PySide6.QtCore import QRegularExpression  # QRegExp
+from PySide6.QtGui import QRegularExpressionValidator  # QRegExpValidator
 from PySide6.QtWidgets import (
     QApplication,
     QButtonGroup,
     QDialog,
     QFileDialog,
     QGridLayout,
     QLabel,
@@ -68,15 +68,17 @@
 
     def add_auth_key_input(self):
         self.add_rb_group(
             ["Generate", "Upload", "Type Hex"], "Select Key Input", self.rb_auth_key_handler
         )
         self.auth_key_line = QLineEdit()
         self.auth_key_line.setVisible(False)
-        self.auth_key_line.setValidator(QRegularExpressionValidator(QRegularExpression("[0-9A-Fa-f]{64}")))
+        self.auth_key_line.setValidator(
+            QRegularExpressionValidator(QRegularExpression("[0-9A-Fa-f]{64}"))
+        )
         self.auth_key_line.textChanged.connect(self.cb_auth_key_type_hex)
         self.layout.addWidget(self.auth_key_line, self.row, 0, 1, 2)
 
         self.auth_key_button = QPushButton("Upload File")
         self.auth_key_button.setVisible(False)
         self.auth_key_button.clicked.connect(self.cb_auth_key_upload)
         self.layout.addWidget(self.auth_key_button, self.row, 0, 1, 2)
@@ -147,12 +149,20 @@
         self.close()
 
     def process_cancel(self):
         self.user_data.clear()
         self.close()
 
 
+class Sha10xSymmAuthUserInputs(SymmAuthUserInputs):
+    def __init__(self, parent=None, config_string=None):
+        super().__init__(parent, config_string)
+
+    def add_device_interface(self):
+        self.add_rb_group(["I2C", "SWI"], "Select SHA104 device interface", self.rb_interface_handler)
+
+
 if __name__ == "__main__":
     app = QApplication(sys.argv)
-    obj = SymmAuthUserInputs()
-    app.exec_()
+    obj = Sha10xSymmAuthUserInputs()
+    app.exec()
     print(obj.user_data)
```

## tpds/servers/tflx_provisioning_xml_ui.py

```diff
@@ -19,19 +19,20 @@
     QLineEdit,
     QMessageBox,
     QPushButton,
     QSizePolicy,
     QSpacerItem,
     QVBoxLayout,
 )
-from tpds.cert_tools.cert_utils import is_key_file_password_protected, get_CSR_CN
+from tpds.cert_tools.cert_utils import get_CSR_CN, is_key_file_password_protected
 from tpds.cert_tools.sign_csr import SignCSR
 from tpds.tp_utils.tp_utils import add_to_zip_archive
 from tpds.xml_handler.ecc_xml_encryption import ECCXMLEncryption
 from tpds.xml_handler.xml_processing import XMLProcessing
+
 from tpds.helper import LogFacility, make_dir
 
 
 class TflxProvisioningXml(QDialog):
     """
     TrustFlex provisional XML Dialog to get all the user input for processing
     """
@@ -55,29 +56,27 @@
         self.csr_zip_lineedit.setText("")
         self.ca_key_lineedit.setText("")
 
         # Show UI for production XML only,
         # for proto XML just process the data directly
         try:
             xml_type = json.loads(config_string).get("xml_type")
-            cert_type = json.loads(config_string).get(
-                "slot_info")[12].get("cert_type")
+            cert_type = json.loads(config_string).get("slot_info")[12].get("cert_type")
             if xml_type == "prod_xml":
                 if cert_type != "custCert":
                     # Disable all csr and ca key data
                     self.csr_zip_lineedit.setEnabled(False)
                     self.csr_zip_button.setEnabled(False)
                     self.ca_key_lineedit.setEnabled(False)
                     self.ca_key_button.setEnabled(False)
                 self.show()
             else:
                 self.process_data()
         except BaseException:
-            QMessageBox.warning(
-                self, "Error", "Invalid config : xml_type not found")
+            QMessageBox.warning(self, "Error", "Invalid config : xml_type not found")
             self.close()
 
     def setup_UI(self):
         """
         Function to setup UI
         """
         # Set Window title
@@ -87,16 +86,15 @@
         # Label for encryption key choosing
         self.encryption_key_label = QLabel()
         self.encryption_key_label.setText(
             """Encryption Key - Load encryption keys .zip file provided by Microchip"""
         )
         # Label for csr_zip choosing
         self.csr_zip_label = QLabel()
-        self.csr_zip_label.setText(
-            """\nCSR ZIP - Load CSRs zip file provided by Microchip""")
+        self.csr_zip_label.setText("""\nCSR ZIP - Load CSRs zip file provided by Microchip""")
         # Label for CA_Key choosing
         self.ca_key_label = QLabel()
         self.ca_key_label.setText(
             """\nCA Key (optional) - Load CA Key to sign CSRs.
             If Key is provided, tool signs the CSRs and generates final package.
             If Key is not provided, tool generates Sign CSR package to sign CSRs offline.
                     Refer to readme.md in the .zip file for signing instructions."""
@@ -125,16 +123,15 @@
         # Window OK button
         self.ok_button = QPushButton()
         self.ok_button.setText("OK")
         # Window Cancel button
         self.cancel_button = QPushButton()
         self.cancel_button.setText("Cancel")
         # Define Layout
-        ok_close_spacer = QSpacerItem(
-            200, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+        ok_close_spacer = QSpacerItem(200, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
         # Setup Hlayouts for individual horizontal items
         enc_H = QHBoxLayout()
         enc_H.addWidget(self.encryption_key_lineedit)
         enc_H.addWidget(self.encryption_key_button)
         csr_H = QHBoxLayout()
         csr_H.addWidget(self.csr_zip_lineedit)
         csr_H.addWidget(self.csr_zip_button)
@@ -156,16 +153,15 @@
         vlay.addWidget(self.ok_close_label)
         vlay.addLayout(ok_close_H)
         # Set Layout
         self.setLayout(vlay)
 
     def setup_singals_slots(self):
         # Setup slots for file select buttons
-        self.encryption_key_button.clicked.connect(
-            self.encryption_file_callback)
+        self.encryption_key_button.clicked.connect(self.encryption_file_callback)
         self.csr_zip_button.clicked.connect(self.csr_zip_file_callback)
         self.ca_key_button.clicked.connect(self.ca_key_file_callback)
         # Setup slot for close button
         self.cancel_button.clicked.connect(self.close_app)
         # Setup slot for OK button
         self.ok_button.clicked.connect(self.process_data)
 
@@ -229,68 +225,64 @@
         try:
             self._log.log("Loading json str")
             part_number = json.loads(config_string).get("part_number")
             time_stamp = datetime.now().strftime("%m%d%H%M%S")
             provisioning_zip_file = f"{part_number}_{time_stamp}"
             xml_file = f"{part_number}_{time_stamp}.xml"
             xml_type = json.loads(config_string).get("xml_type")
-            cert_type = json.loads(config_string).get(
-                "slot_info")[12].get("cert_type")
+            cert_type = json.loads(config_string).get("slot_info")[12].get("cert_type")
 
             encryption_rsa_keys = ""
             if xml_type == "prod_xml":
                 encryption_rsa_keys = enc_key_file
-                assert os.path.exists(
-                    encryption_rsa_keys), "Enc Key is must for Production package"
+                assert os.path.exists(encryption_rsa_keys), "Enc Key is must for Production package"
                 provisioning_zip_file = f"{part_number}_{time_stamp}_Prod.zip"
             else:
                 self._log.log("No encryption for Proto XML")
                 provisioning_zip_file = f"{part_number}_{time_stamp}_Proto.zip"
 
             common_name = "AB-CD_Single_Signer"
             if xml_type == "prod_xml" and cert_type == "custCert":
                 csr_zip = csr_zip_file
-                assert csr_zip and os.path.exists(csr_zip), \
-                    "CSR zip is missing for production package"
+                assert csr_zip and os.path.exists(
+                    csr_zip
+                ), "CSR zip is missing for production package"
 
-                with ZipFile(csr_zip_file, 'r') as zip_file:
+                with ZipFile(csr_zip_file, "r") as zip_file:
                     file_name = zip_file.namelist()[0]
                     with open(file_name, "wb") as tempFile:
                         tempFile.write(zip_file.read(file_name))
                     common_name = get_CSR_CN(file_name)
                     os.remove(file_name)
 
                 common_name = common_name.split()[-1]
-                common_name = common_name[:2] + "-" + \
-                    common_name[2:] + "_Single_Signer"
+                common_name = common_name[:2] + "-" + common_name[2:] + "_Single_Signer"
 
             # Removed single_signer: Provisioning team have requested not to add this tag now....
             # if cert_type == "custCert":
             #     config_string = json.loads(config_string)
             #     config_string['single_signer'] = common_name
             #     config_string = json.dumps(config_string)
 
             self._log.log("Setting output directory")
-            provisioning_zip_dir = os.path.join(
-                str(QDir.homePath()), "Downloads", "TPDS_Downloads")
+            provisioning_zip_dir = os.path.join(str(QDir.homePath()), "Downloads", "TPDS_Downloads")
             make_dir(provisioning_zip_dir)
             os.chdir(provisioning_zip_dir)
 
             self._log.log("Processing configurator string")
             xml = XMLProcessing(json.loads(config_string).get("base_xml"))
             xml.update_with_user_data(config_string)
             xml.save_root(xml_file)
             for extn in ["*.c", "*.h", "*.crt", "*.txt"]:
                 zip_file_list.extend(glob.glob(extn))
 
             self._log.log("Processing CSRs")
             ca_key = csr_zip = sign_csr_zip = signed_crt_zip = None
             if xml_type == "prod_xml" and cert_type == "custCert":
-                self._log.log(
-                    "CustomPKI and Production XML is selected by user")
+                self._log.log("CustomPKI and Production XML is selected by user")
                 csr_zip = csr_zip_file
                 ca_key = ca_key_file
                 if ca_key and os.path.exists(ca_key) and csr_zip and os.path.exists(csr_zip):
                     self._log.log("Processing CSR signing request")
                     ca_key_password = None
                     if is_key_file_password_protected(ca_key):
                         self._log.log("Processing ca_key password")
@@ -305,32 +297,28 @@
                     with ZipFile(csr_zip) as zf:
                         for file_name in zf.namelist():
                             with open(file_name, "wb") as kf:
                                 kf.write(zf.read(file_name))
                             obj = SignCSR(file_name)
                             obj.sign_csr("signer.crt", ca_key, ca_key_password)
                             os.remove(file_name)
-                            file_name = Path(file_name).stem.replace(
-                                "_CSR", "") + ".cer"
+                            file_name = Path(file_name).stem.replace("_CSR", "") + ".cer"
                             Path(file_name).write_bytes(
-                                obj.signer_crt.public_bytes(
-                                    encoding=serialization.Encoding.DER)
+                                obj.signer_crt.public_bytes(encoding=serialization.Encoding.DER)
                             )
                         ca_cert_zip_list = glob.glob("*.cer")
                         signed_crt_zip = f"{part_number}_{time_stamp}_ca_cert.zip"
                         add_to_zip_archive(signed_crt_zip, ca_cert_zip_list)
                         for file in ca_cert_zip_list:
                             os.remove(file)
                 else:
-                    self._log.log(
-                        "Generating sign_CSR zip for offline processing")
+                    self._log.log("Generating sign_CSR zip for offline processing")
                     sign_csr_zip = f"{part_number}_{time_stamp}_sign_csr.zip"
                     shutil.copy(
-                        os.path.join(os.path.dirname(__file__),
-                                     "..", "certs", "sign_csr.zip"),
+                        os.path.join(os.path.dirname(__file__), "..", "certs", "sign_csr.zip"),
                         sign_csr_zip,
                     )
                     z = ZipFile(sign_csr_zip, "a")
                     z.write("signer.crt")
                     z.close()
             else:
                 self._log.log("No CSR processing for non CustomPKI-ProdXML")
@@ -346,16 +334,15 @@
                             "COSP",
                             "COSD",
                             "MTAI",
                             "UTAC",
                             "AIC",
                             "MPHL",
                         ]
-                        xml_matches = [
-                            match for match in site_codes if match in file_name]
+                        xml_matches = [match for match in site_codes if match in file_name]
                         if len(xml_matches):
                             xml_out = f"{part_number}_{xml_matches[0]}.ENC.xml"
                         else:
                             raise ValueError(f"Unknown key file:{file_name}")
 
                         with open(working_file, "wb") as kf:
                             kf.write(zf.read(file_name))
@@ -366,36 +353,33 @@
 
             self._log.log("Archive Provisioning files to Zip")
             zip_file_list.extend(
                 glob.glob("*.ENC.xml")
             ) if xml_type == "prod_xml" else zip_file_list.extend(glob.glob("*.xml"))
             add_to_zip_archive(provisioning_zip_file, zip_file_list)
 
-            path_link = os.path.join(
-                provisioning_zip_dir, provisioning_zip_file).replace("\\", "/")
+            path_link = os.path.join(provisioning_zip_dir, provisioning_zip_file).replace("\\", "/")
             display_msg = (
                 f"<font color=#0000ff>"
                 f"<b>Provisioning Package is saved.</b></font><br><br>"
                 f"""Package: <a href='{path_link}'>"""
                 f"""{path_link}</a><br>"""
             )
 
             if sign_csr_zip:
-                path_link = os.path.join(
-                    provisioning_zip_dir, sign_csr_zip).replace("\\", "/")
+                path_link = os.path.join(provisioning_zip_dir, sign_csr_zip).replace("\\", "/")
                 display_msg += (
                     f"""Scripts to Sign CSRs: <a href='{path_link}'>""" f"""{path_link}</a>"""
                 )
             elif signed_crt_zip:
-                path_link = os.path.join(
-                    provisioning_zip_dir, signed_crt_zip).replace("\\", "/")
+                path_link = os.path.join(provisioning_zip_dir, signed_crt_zip).replace("\\", "/")
                 display_msg += f"""Signed Certs: <a href='{path_link}'>""" f"""{path_link}</a>"""
 
         except BaseException as e:
-            if ("EC key" in str(e)):
+            if "EC key" in str(e):
                 e = str(e).replace("EC key", "ECC key")
             display_msg = f"Provisioning Package process failed with:\n{e}"
             msg_box.setIcon(QMessageBox.Critical)
 
         finally:
             os.remove(working_file) if os.path.exists(working_file) else None
             os.remove(xml_file) if os.path.exists(xml_file) else None
```

## tpds/servers/websocket_server.py

```diff
@@ -61,15 +61,15 @@
         self.close()
         if self._parent:
             self._parent.closeConnection(self)
 
     def close(self):
         try:
             self._socket.deleteLater()
-        except:
+        except:  # noqa E722
             pass
 
 
 class WebSocketServer(QtWebSockets.QWebSocketServer):
     """
     A websocket server which connects the tpds application with the usecases
     """
```

## tpds/servers/wpc_user_inputs.py

```diff
@@ -1,24 +1,33 @@
 import os
 import sys
 
-from PySide6.QtCore import QRegularExpression #RegExp
-from PySide6.QtGui import QRegularExpressionValidator #QRegExpValidator
+from PySide6.QtCore import QRegularExpression  # RegExp
+from PySide6.QtGui import QRegularExpressionValidator  # QRegExpValidator
 from PySide6.QtWidgets import (
-    QApplication, QButtonGroup, QDialog,
-    QFileDialog, QGridLayout, QLabel,
-    QLineEdit, QPushButton, QRadioButton)
+    QApplication,
+    QButtonGroup,
+    QDialog,
+    QFileDialog,
+    QGridLayout,
+    QLabel,
+    QLineEdit,
+    QPushButton,
+    QRadioButton,
+)
 from tpds.tp_utils.tp_keys import TPAsymmetricKey
+
 from tpds.helper import log
 
 
 class WPCUserInputs(QDialog):
     """
     WPC provisional XML Dialog to get all the user input for processing
     """
+
     def __init__(self, parent=None, config_string=None):
         """
         Init class
         """
         super(WPCUserInputs, self).__init__(parent)
         self.setup_UI()
         self.show()
@@ -55,27 +64,27 @@
         self.layout.addWidget(ok_button, self.row, 0)
         cancel_button = QPushButton("Cancel", self)
         cancel_button.clicked.connect(self.process_cancel)
         self.layout.addWidget(cancel_button, self.row, 1)
 
         # add status label at bottom of widget
         self.row += 1
-        self.status_label = QLabel(
-            "Select Inputs for WPC Authentication Usecase")
+        self.status_label = QLabel("Select Inputs for WPC Authentication Usecase")
         self.layout.addWidget(self.status_label, self.row, 0, 1, 5)
         self.setLayout(self.layout)
 
     # add PTMC CODE (4-digit Hex value)
     def add_ptmc_code_input(self):
         self.ptmc_label = QLabel("PTMC Code:")
         self.layout.addWidget(self.ptmc_label, self.row, 0, 1, 5)
         self.ptmc_code = QLineEdit()
         self.ptmc_code.setPlaceholderText("PTMC Code, default: 004E")
         self.ptmc_code.setValidator(
-            QRegularExpressionValidator(QRegularExpression("[0-9A-Fa-f]{4}")))
+            QRegularExpressionValidator(QRegularExpression("[0-9A-Fa-f]{4}"))
+        )
         self.ptmc_code.textChanged.connect(self.cb_set_ptmc_code)
         self.layout.addWidget(self.ptmc_code, self.row, 1, 1, 5)
 
     def cb_set_ptmc_code(self, text):
         self.ptmc_code.setText(text.upper())
         self.user_data.update({"ptmc_code": text.upper()})
 
@@ -95,27 +104,28 @@
 
     # add Mfg CA Sequence ID (2-digit Hex value)
     def add_ca_seqid_input(self):
         self.label = QLabel("CA Sequence ID:")
         self.layout.addWidget(self.label, self.row, 0, 1, 5)
         self.ca_seqid = QLineEdit()
         self.ca_seqid.setPlaceholderText("CA Sequence ID, default: 01")
-        self.ca_seqid.setValidator(QRegularExpressionValidator(QRegularExpression("[0-9A-Fa-f]{2}")))
+        self.ca_seqid.setValidator(
+            QRegularExpressionValidator(QRegularExpression("[0-9A-Fa-f]{2}"))
+        )
         self.ca_seqid.textChanged.connect(self.cb_set_ca_seqid)
         self.layout.addWidget(self.ca_seqid, self.row, 1, 1, 5)
 
     def cb_set_ca_seqid(self, text):
         self.ca_seqid.setText(text.upper())
         self.user_data.update({"ca_seqid": text.upper()})
 
     # add Generate / Upload Root and Mfg Private Key
     def add_key_input(self):
         # add radio button
-        self.add_rb_group(
-            ["Generate", "Upload"], "Root and Mfg. keys:", self.rb_key_handler)
+        self.add_rb_group(["Generate", "Upload"], "Root and Mfg. keys:", self.rb_key_handler)
 
         # add root key input
         self.row += 1
         self.root_key_label = QLabel("Root Key")
         self.layout.addWidget(self.root_key_label, self.row, 1)
         # add root key input text
         self.root_key_text = QLineEdit()
@@ -151,69 +161,63 @@
             self.layout.addWidget(rb, self.row, self.column)
 
         self.row += 1
         self.column = 0
 
     def cb_root_key_upload(self):
         file_name = QFileDialog.getOpenFileName(
-            None, caption="Select Root Key File", filter="*.pem, *.key")
+            None, caption="Select Root Key File", filter="*.pem, *.key"
+        )
         if file_name[0] != "":
             try:
                 self.root_key_text.setText(file_name[0])
                 self.status_label.setText(f"Root key file: {os.path.basename(file_name[0])}")
                 root_key = TPAsymmetricKey(key=file_name[0])
-                self.user_data.update(
-                    {"root_key": root_key.get_private_pem()})
+                self.user_data.update({"root_key": root_key.get_private_pem()})
             except BaseException as e:
                 log(f'File upload failed with: "{e}"')
-                self.status_label.setText(
-                    "Upload is failed. Try again or check log for details...")
+                self.status_label.setText("Upload is failed. Try again or check log for details...")
 
     def cb_mfg_key_upload(self):
         file_name = QFileDialog.getOpenFileName(
-            None, caption="Select Mfg. Key File", filter="*.pem, *.key")
+            None, caption="Select Mfg. Key File", filter="*.pem, *.key"
+        )
         if file_name[0] != "":
             try:
                 self.mfg_key_text.setText(file_name[0])
                 self.status_label.setText(f"Mfg key file: {os.path.basename(file_name[0])}")
                 mfg_key = TPAsymmetricKey(key=file_name[0])
-                self.user_data.update(
-                    {"mfg_key": mfg_key.get_private_pem()})
+                self.user_data.update({"mfg_key": mfg_key.get_private_pem()})
             except BaseException as e:
                 log(f'''File upload failed with "{e}"''')
-                self.status_label.setText(
-                    "Upload is failed. Try again or check log for details...")
+                self.status_label.setText("Upload is failed. Try again or check log for details...")
 
     def rb_key_handler(self):
         if self.sender().isChecked():
             selected = self.sender().text()
             if selected == "Generate":
                 self.setDisable(True)
-                self.user_data.update(
-                    {"root_key": TPAsymmetricKey().get_private_pem()})
-                self.user_data.update(
-                    {"mfg_key": TPAsymmetricKey().get_private_pem()})
-                self.status_label.setText(
-                    "ECC P256 random keys will be generated...")
+                self.user_data.update({"root_key": TPAsymmetricKey().get_private_pem()})
+                self.user_data.update({"mfg_key": TPAsymmetricKey().get_private_pem()})
+                self.status_label.setText("ECC P256 random keys will be generated...")
             elif selected == "Upload":
                 self.setDisable(False)
-                self.user_data.update({"root_key": '', "mfg_key": ''})
-                self.status_label.setText(
-                    "Upload ECC P256 development Key files in PEM format...")
+                self.user_data.update({"root_key": "", "mfg_key": ""})
+                self.status_label.setText("Upload ECC P256 development Key files in PEM format...")
 
     def process_ok(self):
-        if (not self.user_data.get("root_key")):
+        if not self.user_data.get("root_key"):
             self.user_data.update({"root_key": TPAsymmetricKey().get_private_pem()})
-        if (not self.user_data.get("mfg_key")):
+        if not self.user_data.get("mfg_key"):
             self.user_data.update({"mfg_key": TPAsymmetricKey().get_private_pem()})
-        if (not self.user_data.get("ptmc_code")):
+        if not self.user_data.get("ptmc_code"):
             self.user_data.update({"ptmc_code": "004E"})
-        if (not self.user_data.get("qi_id")):
+        if not self.user_data.get("qi_id"):
             self.user_data.update({"qi_id": "11430"})
-        if (not self.user_data.get("ca_seqid")):
+        if not self.user_data.get("ca_seqid"):
             self.user_data.update({"ca_seqid": "01"})
 
         self.close()
 
     def process_cancel(self):
         self.user_data.clear()
         self.close()
```

## tpds/settings/__init__.py

```diff
@@ -1,4 +1,6 @@
 """
 Settings package
 """
 from .tpds_settings import TrustPlatformSettings
+
+__all__ = ["TrustPlatformSettings"]
```

## tpds/settings/tpds_settings.py

```diff
@@ -4,14 +4,15 @@
 This module implements the Trust Platform Settings
 """
 from __future__ import annotations
 
 import json
 import logging
 import os
+from functools import singledispatchmethod
 from itertools import filterfalse
 from typing import (
     KT,
     VT,
     Any,
     Callable,
     Iterable,
@@ -71,19 +72,21 @@
 
 class TpdsSettingsList(MutableSequence[T]):
     def __init__(self, __v: Sequence[T], observer: Callable[[Any], Any]) -> None:
         super().__init__()
         self.data = __v
         self.observer = observer
 
+    @singledispatchmethod
     def __setitem__(self, __i: int, __v: T) -> None:
         self.observer(True)
         self.data.__setitem__(__i, _setting_type_check(__v, self.observer))
 
-    def __setitem__(self, __s: slice, __o: Iterable[T]) -> None:
+    @__setitem__.register
+    def _(self, __s: slice, __o: Iterable[T]) -> None:
         self.observer(True)
         self.data.__setitem__(__s, [_setting_type_check(x, self.observer) for x in __o])
 
     def __getitem__(self, __is: Union[int, slice]) -> T:
         return self.data[__is]
 
     def __delitem__(self, __i) -> None:
```

## tpds/usecase_collector/__init__.py

```diff
@@ -1,2 +1,4 @@
-from .collector import *
-from .usecase import *
+from .collector import Collector
+from .usecase import Usecase, UsecaseEntrypoint
+
+__all__ = ["Collector", "Usecase", "UsecaseEntrypoint"]
```

## tpds/usecase_collector/collector.py

```diff
@@ -58,15 +58,15 @@
             if search_paths is None or len(search_paths) == 0:
                 search_paths = cfg.get("paths", [])
 
             self.__search_paths = []
             for x in search_paths:
                 try:
                     self.__search_paths += [{"path": Collector._get_workspace_path(x)}]
-                except:
+                except FileNotFoundError:
                     continue
 
             self.update(False)
 
     def __iter__(self):
         return iter(self.__usecases.values())
```

## tpds/usecase_collector/usecase.py

```diff
@@ -16,14 +16,15 @@
 # FULLEST EXTENT ALLOWED BY LAW, MICROCHIP'S TOTAL LIABILITY ON ALL CLAIMS IN
 # ANY WAY RELATED TO THIS SOFTWARE WILL NOT EXCEED THE AMOUNT OF FEES, IF ANY,
 # THAT YOU HAVE PAID DIRECTLY TO MICROCHIP FOR THIS SOFTWARE.
 from __future__ import annotations
 
 import os
 from abc import ABCMeta, abstractmethod
+from functools import singledispatchmethod
 from typing import Any, Iterable, Mapping, MutableSequence, Optional, Sequence, Union
 from urllib.parse import quote as urlquote
 
 from tpds.settings.validator import SettingsValidator
 
 
 class UsecaseValidator(SettingsValidator):
@@ -142,18 +143,20 @@
         self.data = [UsecaseEntrypoint(**self._extras, **v) for v in __v]
 
     def _check(self, __v):
         return (
             __v if isinstance(__v, UsecaseEntrypoint) else UsecaseEntrypoint(**self._extras, **__v)
         )
 
+    @singledispatchmethod
     def __setitem__(self, __i: int, __v: Any) -> None:
         self.data.__setitem__(__i, self._check(__v))
 
-    def __setitem__(self, __s: slice, __o: Iterable[Any]) -> None:
+    @__setitem__.register
+    def _(self, __s: slice, __o: Iterable[Any]) -> None:
         self.data.__setitem__(__s, [self._check(x) for x in __o])
 
     def __getitem__(self, __is: Union[int, slice]) -> Union[UsecaseEntrypoint, UsecaseEntrypoints]:
         return (
             UsecaseEntrypoints(self.data[__is], **self._extras)
             if isinstance(__is, slice)
             else self.data[__is]
@@ -170,15 +173,19 @@
 
     def __repr__(self) -> str:
         return str(self.data)
 
 
 class UsecaseBackend:
     def __init__(
-        self, path: Optional["os.PathLike[str]"] = None, routers: Sequence[str] = [], requires: Sequence[str] = [], **kwargs: Any
+        self,
+        path: Optional["os.PathLike[str]"] = None,
+        routers: Sequence[str] = [],
+        requires: Sequence[str] = [],
+        **kwargs: Any,
     ) -> None:
         self.path = path
         self.routers = routers
         self.requires = requires
         self.__dict__.update(kwargs)
 
     def __set__(self, instance, value):
```

## Comparing `tpds_core-2.3.4.dist-info/LICENSE` & `tpds_core-2.3.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tpds_core-2.3.4.dist-info/METADATA` & `tpds_core-2.3.5.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpds-core
-Version: 2.3.4
+Version: 2.3.5
 Summary: Microchip(SPG) Trust Platform Core 
 Maintainer-email: Microchip Technology <SPG.Tools@microchip.com>
 License: (c) 2015-2023 Microchip Technology Inc. and its subsidiaries.
         
         Subject to your compliance with these terms, you may use the Microchip Software
         and any derivatives exclusively with Microchip products. It is your
         responsibility to comply with third party license terms applicable to your
@@ -31,14 +31,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: asn1crypto
 Requires-Dist: bs4
+Requires-Dist: deepdiff
 Requires-Dist: cryptography (~=35.0.0)
 Requires-Dist: python-multipart
 Requires-Dist: fastapi
 Requires-Dist: jsonschema
 Requires-Dist: Markdown
 Requires-Dist: packaging
 Requires-Dist: psutil
@@ -48,19 +49,29 @@
 Requires-Dist: pyusb
 Requires-Dist: PyYAML
 Requires-Dist: starlette
 Requires-Dist: tabulate
 Requires-Dist: uvicorn
 Requires-Dist: notebook (<7,>=6.4.12)
 Requires-Dist: voila (==0.4.0)
-Requires-Dist: cryptoauthlib
+Requires-Dist: cryptoauthlib (>=20230326)
 Requires-Dist: tpds-application-root
 Requires-Dist: tpds-boards
 Requires-Dist: tpds-manifest
 Requires-Dist: tpds-helper (>2.3.2)
 Requires-Dist: tpds-voila-template
+Provides-Extra: dev
+Requires-Dist: flake8 ; extra == 'dev'
+Requires-Dist: black ; extra == 'dev'
+Requires-Dist: isort ; extra == 'dev'
+Requires-Dist: mypy ; extra == 'dev'
+Provides-Extra: test
+Requires-Dist: httpx ; extra == 'test'
+Requires-Dist: pytest-cov ; extra == 'test'
+Requires-Dist: pytest-mock ; extra == 'test'
+Requires-Dist: pytest-integration ; extra == 'test'
 
 Trust Platform Design Suite - Core
 ===============================================================================
 
 This module contains the backend services and resources required by the TPDS
 application and utilities.
```

## Comparing `tpds_core-2.3.4.dist-info/RECORD` & `tpds_core-2.3.5.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,86 @@
 tpds/__init__.py,sha256=ED6jHcYiuYpr_0vjGz0zx2lrrmJT9sDJCzIljoDfmlM,65
-tpds/api/__init__.py,sha256=5hyUIcbhLrM51ZBdRQ8q-o1EbAsI0_dxiT3Kf1tPtA0,32
-tpds/api/core.py,sha256=pEMe04SqLVaEPPRtgqMy4iHnM5O5DXo2RcULdFvsPSQ,6250
-tpds/api/loader.py,sha256=sLsYtliOuXrT75q-iaiW6VFHhzV-egBrH39T6PLyOgs,4301
+tpds/api/__init__.py,sha256=v1m0_mbyCguf-7PKrQ1HiNj0Eo2QXeg8HX-Y7f5lrnc,61
+tpds/api/core.py,sha256=X8_qEq7FnnYINMYMJYWhmjND2NtivFxiNlKxraA1zTM,6434
+tpds/api/loader.py,sha256=xYGvDrAp5KgiDEG0SFU7zE_qb6wrXl2QeM7sxyAD3gU,4303
 tpds/api/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tpds/api/api/router.py,sha256=gWQC0iVkBj1q6jPwu3QG_BPcDy21B5bCuiyi1ii_Co4,528
 tpds/api/api/usecases.py,sha256=J-SOGCliuMoqmq1xa9z-Rhi-S8iIfrYg8bo6Urc1-4M,4745
 tpds/api/api/hw/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tpds/api/api/hw/api_board.py,sha256=xfeXvE7H1DPRgb32xCsxQvl3PpTmV1RQF_oE9nG-Sa0,3904
+tpds/api/api/hw/api_board.py,sha256=pzIx5TwrbYqncp8-fita6Y9Fl8nq5aWTgoWbGKcCakM,3803
 tpds/api/api/hw/api_device.py,sha256=ZQBAwiV17giZtvBFpEZbv7EYVqeVWuDYaHPYaXXmudE,6741
-tpds/api/api/manifest_file/api_manifest.py,sha256=Cwwomgu9OLE9G7xMoS-IeRHjU68nWbcnhpGH5_wyn5M,3718
+tpds/api/api/manifest_file/api_manifest.py,sha256=up74zJAT9EvWBpdxwIWQZCh7FAYSzxMND4Gy7-DlJzI,3711
 tpds/api/api/manifest_file/MCHP_manifest_signer/MCHP_manifest_signer_1_Jan2019_July2019.crt,sha256=xJQEUuX6QT2LotnUER7A5LMguHer_JBITL2tz6u_fls,675
 tpds/api/api/manifest_file/MCHP_manifest_signer/MCHP_manifest_signer_2_Aug2019_Aug2020.crt,sha256=JCuDe5ODt9W8ztN6Wd35VMGd3SF3lMXKaKBzl3cWuuo,676
 tpds/api/api/manifest_file/MCHP_manifest_signer/MCHP_manifest_signer_3_Aug-13-2020-Aug-13-2023.crt,sha256=cB4dAXlWeRQf1uP9jJaNkF3vZH5HwTHpO6gxsGxvB5k,676
-tpds/api/api/package_manager/api_package_manager.py,sha256=LyR2EuR-wpP-Ukouwhk0eyzdNM21HcYsDL5Or9LYfIA,3134
+tpds/api/api/package_manager/api_package_manager.py,sha256=jJUmg6IRkjid2OWlCha0Q-whulhJmSCVwCargCxX6ns,3127
 tpds/api/api/schemas/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tpds/api/api/schemas/hw.py,sha256=UFtzVFwMieohY4Jgu9awLXZbM_Ey7iHnPta_dMwaZZk,1672
 tpds/api/assets/favicon.ico,sha256=0tGdaFYSuwmFPuwO7mvBviV_g07wnuqU2AAjD0yMg-E,221974
-tpds/api/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tpds/api/tests/conftest.py,sha256=KXHdPaMbYrhFCPdi2xfLWs0boP_2127BJiDetRzhkAg,212
-tpds/api/tests/pytest.ini,sha256=bVZArHjqufq0QPHWJk0PkmNCYDuUfkJWbgi6K_Fycw4,196
-tpds/api/tests/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tpds/api/tests/api/hw/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tpds/api/tests/api/hw/test_api_board.py,sha256=vYzm_UZH69gNaOh1KiUUVgeeEpCdSWNkEhEfn4C3bE0,1284
-tpds/api/tests/api/hw/test_api_device.py,sha256=Ei-qCKJEQzVUWdEhN6FFHw03DK4-SFA8o0_1fJ8s22c,2272
+tpds/configurator/__init__.py,sha256=Kt1W6wUBmct-qmpM5ikq5kXkz4I8WxNQqikFN0P9Fyg,114
+tpds/configurator/algorithms.py,sha256=nTvsR3ZbqbDRroVHNhaZq5dffOS8zLDB8EcGvALEYhc,354
+tpds/configurator/api.py,sha256=twU_32npb3Y9rV28kcTrTElKf5jj4jg6pgf9vigDunQ,2100
+tpds/configurator/configurator.py,sha256=SxRvQ-fnoh7I_MTwVe4ucYFUwFUiJAHqfkkCvb4PvKY,1245
+tpds/configurator/models.py,sha256=rOL-lk7r6gKMNft2PD0GijQUZ06PKbAzgUIyMTIcE5E,5395
+tpds/configurator/store.py,sha256=GB_W5q_zX-LMO2CpDwbu26eBYEcERczoNrCJg_wKQsc,2377
+tpds/configurator/engine/__init__.py,sha256=OricXRycw5SnkirBiCk00ac37GZh_vhT1BPAjuWKeSs,116
+tpds/configurator/engine/engine.py,sha256=O30FWc6SjpgHK0akD0QH3Ba-4g4hlEH5RiyXyuFAtkU,6074
+tpds/configurator/engine/exceptions.py,sha256=kFI3LMAuB_7wKCACNcnRrX95WryoZwBfTeiuhCjTJlI,708
+tpds/configurator/engine/rule.py,sha256=hs_dec4FrRELFRQLrqlLP2twhGWc6ph986IOHigvSs0,1332
+tpds/configurator/engine/state.py,sha256=tcTykWhawr5Yu7VpJsW5yXpbn3wdQfY1VYVRaw7cD_8,6867
+tpds/configurator/engine/types.py,sha256=28DOoRNijkVus59-jFpdIFr4Vl7oisQ31M5CJfEC89U,187
 tpds/devices/__init__.py,sha256=ycw9n1KXlaWg0b1mhMf1BfZjImvgdR3RumsTM-BsTvY,289
 tpds/devices/boards_schema.yaml,sha256=4YgirOAW4XpFYEBHqvqTqNmNLio5KIb_J7Fdbp7wBJs,773
-tpds/devices/devices_schema.yaml,sha256=oFEtdSaNVs_1naRLmgX9y_ot4nSlPOLiACJZg4eW6NA,2246
-tpds/devices/tpds_boards.py,sha256=F3UP3Hx57ubQKSscS1ZgY6rUvKLgIxShOtIz_ZS2r2I,3371
-tpds/devices/tpds_devices.py,sha256=8kag_-hkJaCHwW5-P048Oe2ZC7XTUWkXSKZbDOgMSrE,3906
-tpds/devices/tpds_models.py,sha256=i4KGpwyK3q_9WQ0ahCzZBFzd8A4scNaf5KqoBmvu6IQ,5121
+tpds/devices/devices_schema.yaml,sha256=msbBC-Rxp64_31wG5a10XL6CAc_mKvP1EbcTcqvPYv8,2300
+tpds/devices/tpds_boards.py,sha256=6fYVsuJQX8vo_wuWkAp-149sGtnb3PvklXlFi7UWTkE,3292
+tpds/devices/tpds_devices.py,sha256=a-d9ST5VrhixazTDrthfStbVZtOdJrhqhbH1P9LFJ00,3849
+tpds/devices/tpds_models.py,sha256=QuSBIXYafNaN7rCgpeVYyHsakiU4liKyhkEZEfHkoIE,5099
 tpds/devices/data/ecc608-tcsm.yaml,sha256=ix_rWwsbnszhbT3IZVtH67nBJulY16OKz08K5VoUOwI,1106
-tpds/devices/data/ecc608-tflx.yaml,sha256=0N-ACdFR8v-DGLmYfRT7oxefP7vRuXs9W9gJs61j6UQ,1926
+tpds/devices/data/ecc608-tflx.yaml,sha256=cdUDHUJabMz-n0-alYU8dAm4NhPXX626VgSIM5Zp5wI,998
 tpds/devices/data/ecc608-tng.yaml,sha256=KPyORLBNSNsz-ipVKrnlXwftTDzDwcdisIiDxlcQLqY,3962
 tpds/devices/data/modules.yaml,sha256=CnXmy7WJO_rp3kpiIPJnoqRJdvGgJjUu_PR6eW3E9Tc,1312
-tpds/devices/data/sha204.yaml,sha256=nafEHdhhsgZiDEnWnREeO0rsF5xfPqrtj1uWNEqjI-I,1019
-tpds/devices/data/ta100.yaml,sha256=nd-Eh6M72rJ-dUtye4Aeco0vh7Nfexv6BgSP0t1AR9A,881
-tpds/helper/__init__.py,sha256=7ycIKy8pcshQx9G-j9Sqf-X0dQzk2iCuQ_AL8-Q1AqY,124
-tpds/helper/logger.py,sha256=eChDJLdU9RTrhx50zS2s038vzIuD8PUyomyq40cICm0,2544
+tpds/devices/data/sha204.yaml,sha256=FMsexuIcSRgO9ELa8MDqIg6LfZWiCqYrjMsL_C9JtiE,1056
+tpds/devices/data/ta100.yaml,sha256=Co4K7h9hAChJsTgPzTGqY_dihvZZ9cdemzoE59vsefA,880
+tpds/helper/__init__.py,sha256=6FjjNRA5Hnd6S-9TuJwF071oh5p3KrZ9RBtU5MQ1YZY,460
+tpds/helper/logger.py,sha256=m8Sys3nSrucophQu6wYUNczp3q1a8jEJ9E0AD3LGpiA,2543
 tpds/helper/processing.py,sha256=AUIq_qzSPouim24bjgrMG3zVgd0WGXyY8akvllaHvQU,4113
-tpds/helper/utils.py,sha256=AVCDQk-ywItoXPLjQKify6YK7UJhOU6cCZIQm-dmgIw,2498
-tpds/launcher/__init__.py,sha256=OzWO-jzBxgyWtAq3BS9XANcZgCIA_Wi8r_DhSrmllLU,21
+tpds/helper/singleton.py,sha256=6q9wDjJJPEiycXSGHHbbpx8TFBg0v2Ql6BU5eubbN4Q,956
+tpds/helper/utils.py,sha256=UygncRCecYwmX-yWjngQSV48RjbhCo3OIR5VjanX0yI,2519
+tpds/launcher/__init__.py,sha256=qKjt0F1xUQqKhRdIc_oKCD3sJmcYE2cqKwUl-f8DLw8,96
 tpds/launcher/start.py,sha256=tQ4YFxzz_TeKS7dEvtHNZXOVPNy-ux2BmnOi_kwg5Po,3819
-tpds/package_manager/__init__.py,sha256=ImWPo3UsVw8UUO3q4GDtsvLf9N00aE1EIBGQIuHqKs0,119
+tpds/package_manager/__init__.py,sha256=LoiJsERi-YJ_0ymt_ocOa4U2SXNLfkLuVHdR1aflSz8,187
 tpds/package_manager/client_model.py,sha256=UCECzDrV5i0bEoZxU1JJlZZpUbyoedixaJKjAYUFdTc,2567
-tpds/package_manager/conda_client.py,sha256=CIypiMYMqZRtwdBUn0IOyGS0Jn27RMd1FeGuOGr0qr8,13594
-tpds/package_manager/data_models.py,sha256=MMQDXsK3tp-7qDZkzgk7E-Kx7ey2AqIpLHlyLa8FkME,3888
-tpds/package_manager/manager.py,sha256=YbmC5LSMn1yTLst13cOHd8KkgqVA8QBXKJDdKGfwdXM,11844
+tpds/package_manager/data_models.py,sha256=SsD7ea4XnxZVq_L1CotBmjW9zm49a2W8XXG_v-5oqbY,2144
+tpds/package_manager/manager.py,sha256=OQ5bKDrSzq5bZ-O1ziJOLxY5OA_UhBVXkri1i5V6B1A,11961
 tpds/package_manager/packages_schema.yaml,sha256=DYk3xWQ_V0MsVzOBw2_w_qbleGg_aQ1WrHCaRByfj3E,1299
-tpds/package_manager/pip_client.py,sha256=OfP6W1f3eOP6pph7pZ4lj1QJgsYGZ3fbKywRoQmZyhw,6995
+tpds/package_manager/pip_client.py,sha256=aFuVTFgIxs-xdm6k16USw_CI46G50sAROyGQ_DIjVtk,7144
 tpds/package_manager/licenses/mchp.txt,sha256=MH079cSoEdwEsWmWCWSqhlA6sn8px7UxWB2Qdo7lH9g,1239
 tpds/servers/TPDS_notebook_config.py,sha256=Lexztf6-Mno7NoMDbZq_juPkHMg-mU1_o2LtvKcUPkk,21064
-tpds/servers/__init__.py,sha256=_-Cv8fiQ55ULK0B_r7-WolMF5lsBOM6-wSz5PfwdWR0,202
+tpds/servers/__init__.py,sha256=dCulWEjZoveaMUYRLARXA78q9q0t9v6jtblBbk6rTWQ,332
 tpds/servers/jupyter_server.py,sha256=qJQenD3ZK1_ztHpyKpQwMhW_tocxnDckYis2lr8Swwk,4410
-tpds/servers/msg_handler.py,sha256=2bDPzdFUYEKpyCJdZ1hEpLrD4HrFnT92q4hR7ilsm84,11491
-tpds/servers/msg_handler_ta.py,sha256=-wHfk70zcSFYJYdNcYKmD6zJ0pDTML9fa70okjVsIU0,13114
+tpds/servers/msg_handler.py,sha256=98Cv3N49xB0ZOCT0y782vVFXZLDj4THnrcbMUcywSfI,11754
+tpds/servers/msg_handler_ta.py,sha256=vG_aLSdd6v-1GHzClCRug3zH55LXJfy0SzS31wDhjGQ,13130
 tpds/servers/msg_handler_tcustom.py,sha256=4nby9LcyDlsDT6SPk9Zzd_i9i97aMbGQMnxTQ3vKceQ,2565
-tpds/servers/msg_handler_tflx.py,sha256=v1-hKSdVth3_ctxUcjP1mnm7Ra-kOLctfZwRAXG-48Y,4540
-tpds/servers/msg_handler_tflx_ecc204.py,sha256=8526Vsf-EBIidzQNlqbG8l0yyNUen7b5MOwprJsa0BQ,9708
-tpds/servers/provision_user_inputs.py,sha256=RfaqWO4zHgEU3E6EFJ6FS-tOgQQsCYLBXXTFTRFGxag,7306
-tpds/servers/symm_auth_user_inputs.py,sha256=dzJ-elX1GDL5eYgGS3_JYqeRlZI1m9Q508Q3xSE-gkU,5761
-tpds/servers/tflx_provisioning_xml_ui.py,sha256=sAgRgASfnWjEz4_P8z-qqrDi8uIPg-ABGqLi67vKlc8,16910
+tpds/servers/msg_handler_tflx.py,sha256=B4tNuqetLUdkzeCt6ZBNQGA60CfYLxx9gX9jb3ygtEI,4494
+tpds/servers/msg_handler_tflx_ecc204.py,sha256=dxkWhI1vTR3Zyt71kolhnV87_X33s_9oREbK4ZNb3_0,9582
+tpds/servers/provision_user_inputs.py,sha256=0T1vW9SORg3nOPh2P2Dj8mmsmAtMR5bOfwZxJHPchL8,7250
+tpds/servers/symm_auth_user_inputs.py,sha256=frJ6HgPEajPfm9yY6zPwpapdg3pxftOMlRTYJie3CYQ,6091
+tpds/servers/tflx_provisioning_xml_ui.py,sha256=2DAn3dpHboCOPdElBtOJimXS18KRSj6RDc3D6KfvmYI,16534
 tpds/servers/uno_server.py,sha256=fi8NKyrxWZTpj6Cn-154pkirtP6GONS74hf6VQH8enk,1093
-tpds/servers/websocket_server.py,sha256=CChd_9V83xgEl8KN3wNd6u8f33VuGyi66PunSJxLUY8,3813
-tpds/servers/wpc_user_inputs.py,sha256=3LQJ2SqM4yCob8eDkx_Y-B1relXD60cZClu0y7pjY8w,9210
-tpds/settings/__init__.py,sha256=Az_aod5gd1_BLZ6UKnArrySxRRYJsnGwi2DfgEXWscw,74
+tpds/servers/websocket_server.py,sha256=hyMak_BMmbKn7CZoheKoShktQp7ABK7a94Jl4_Vbg40,3826
+tpds/servers/wpc_user_inputs.py,sha256=J3puzvuz1Kb0kFgLsoG7z_jpiZst7b1BRXIyz8R_jGI,9087
+tpds/settings/__init__.py,sha256=-Z0f9OYt9FeWfekImbmuC-Arxxu9-i2sLWNzoZeK8M4,111
 tpds/settings/tpds_config.yaml,sha256=SNzYfN43a3EcZp2DsUjtibAgUlYqcm0Vq2Kv8dlK4SA,2583
 tpds/settings/tpds_default.yaml,sha256=Qgr4iSLalndJWL9NM9AWeZH2WJnyEp0JxP7f_wjSuKE,1048
-tpds/settings/tpds_settings.py,sha256=14BNGBYjX5txvmAPPQ6vEE-I_xe-t73j29bWCU56g2g,11471
+tpds/settings/tpds_settings.py,sha256=HxgFl8kgrc_Uyc79X-fVh7IXhsZjLVxnaTdNQI4a7-M,11556
 tpds/settings/validator.py,sha256=RGXv4NSNo0IOvOCvPOaw9QleQMGj5kp0iDU7Zm-s4hA,3444
-tpds/usecase_collector/__init__.py,sha256=WTBwv28CBa9teIJ9omhFLEvgNCJqVYhligrZMyIHyCk,48
-tpds/usecase_collector/collector.py,sha256=gS8Jw7qNk8JThAb38UDH4EXnxpnVqTucIAaN2ZttN1M,7085
-tpds/usecase_collector/usecase.py,sha256=lHW91xyxX1XHc6WAWJThWvyb-BJkl8LnksfsOe3BF3k,8889
+tpds/usecase_collector/__init__.py,sha256=rl_9KmGYtA_oYHttS_Eo8vDYthKQTgpIjDRb7KwHus0,138
+tpds/usecase_collector/collector.py,sha256=EiBlSGotzHEiVVPl0DrlHqRpwOR4ekVuzWARYWBdlFI,7103
+tpds/usecase_collector/usecase.py,sha256=x4vlHKAJXN9JI1fJHwh1FkLQT9W1tK7x44nbjLftEvQ,9007
 tpds/usecase_collector/usecase.yaml,sha256=ioSrxH0T10RqZT47DoiPpKWOUHeo2fUEiFMJ2a8Ckkw,2126
 tpds/version/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tpds_core-2.3.4.dist-info/LICENSE,sha256=F_itoJVw8BueLDyZXyIPzgH_thxrjAGZ9vasLzVc19I,1322
-tpds_core-2.3.4.dist-info/METADATA,sha256=0fVUWaYtDuGgbAOwbsNi21RtPGwC9xejD0DL_5duLSg,2846
-tpds_core-2.3.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-tpds_core-2.3.4.dist-info/entry_points.txt,sha256=r_VAMfzGMczHY7MeCGf_Q1HFmw0iRrqFpsbHJBeObfM,102
-tpds_core-2.3.4.dist-info/top_level.txt,sha256=Tl4GsItOlkTwS5kMrk7oOjlZsRztkeFRTneAJ5ZBOjQ,5
-tpds_core-2.3.4.dist-info/RECORD,,
+tpds_core-2.3.5.dist-info/LICENSE,sha256=F_itoJVw8BueLDyZXyIPzgH_thxrjAGZ9vasLzVc19I,1322
+tpds_core-2.3.5.dist-info/METADATA,sha256=yu9FQ_Sh16yc1dR0A6-yW7qYXxVqTRFT9JB3kw3LNas,3256
+tpds_core-2.3.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+tpds_core-2.3.5.dist-info/entry_points.txt,sha256=r_VAMfzGMczHY7MeCGf_Q1HFmw0iRrqFpsbHJBeObfM,102
+tpds_core-2.3.5.dist-info/top_level.txt,sha256=Tl4GsItOlkTwS5kMrk7oOjlZsRztkeFRTneAJ5ZBOjQ,5
+tpds_core-2.3.5.dist-info/RECORD,,
```


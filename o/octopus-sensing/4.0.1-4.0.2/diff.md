# Comparing `tmp/octopus-sensing-4.0.1.tar.gz` & `tmp/octopus-sensing-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octopus-sensing-4.0.1.tar", max compression
+gzip compressed data, was "octopus-sensing-4.0.2.tar", max compression
```

## Comparing `octopus-sensing-4.0.1.tar` & `octopus-sensing-4.0.2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0    35149 2020-08-21 08:41:09.800625 octopus-sensing-4.0.1/LICENSE
--rw-r--r--   0        0        0     2863 2022-05-20 05:30:08.246089 octopus-sensing-4.0.1/README.md
--rw-r--r--   0        0        0    11168 2020-08-17 23:48:22.186902 octopus-sensing-4.0.1/octopus_sensing/OpenVibe/csv2edf.xml
--rw-r--r--   0        0        0    18650 2020-08-17 23:48:22.186902 octopus-sensing-4.0.1/octopus_sensing/OpenVibe/display-save-eeg-exp2.xml
--rw-r--r--   0        0        0    18648 2020-08-17 23:48:22.186902 octopus-sensing-4.0.1/octopus_sensing/OpenVibe/display-save-eeg.xml
--rw-r--r--   0        0        0      790 2023-03-15 03:01:54.998185 octopus-sensing-4.0.1/octopus_sensing/__init__.py
--rw-r--r--   0        0        0      768 2020-12-08 03:09:47.654520 octopus-sensing-4.0.1/octopus_sensing/common/__init__.py
--rw-r--r--   0        0        0     7612 2022-05-24 06:03:24.413484 octopus-sensing-4.0.1/octopus_sensing/common/endpoint_base.py
--rw-r--r--   0        0        0     2261 2021-11-16 00:47:29.106136 octopus-sensing-4.0.1/octopus_sensing/common/message.py
--rw-r--r--   0        0        0     3645 2021-11-16 00:47:29.110136 octopus-sensing-4.0.1/octopus_sensing/common/message_creators.py
--rw-r--r--   0        0        0     7923 2023-03-13 03:09:12.050065 octopus-sensing-4.0.1/octopus_sensing/device_coordinator.py
--rw-r--r--   0        0        0     4551 2021-11-28 21:09:44.826763 octopus-sensing-4.0.1/octopus_sensing/device_message_endpoint.py
--rw-r--r--   0        0        0     1301 2021-11-18 05:55:31.419363 octopus-sensing-4.0.1/octopus_sensing/devices/__init__.py
--rw-r--r--   0        0        0     8887 2023-03-15 02:47:16.173420 octopus-sensing-4.0.1/octopus_sensing/devices/audio_streaming.py
--rw-r--r--   0        0        0     7303 2023-03-29 00:01:35.111275 octopus-sensing-4.0.1/octopus_sensing/devices/brainflow_openbci_streaming.py
--rw-r--r--   0        0        0     9113 2023-03-24 06:35:43.977593 octopus-sensing-4.0.1/octopus_sensing/devices/brainflow_streaming.py
--rw-r--r--   0        0        0    10408 2023-03-15 02:50:32.664706 octopus-sensing-4.0.1/octopus_sensing/devices/camera_streaming.py
--rw-r--r--   0        0        0     1492 2021-11-16 00:47:29.126136 octopus-sensing-4.0.1/octopus_sensing/devices/common.py
--rw-r--r--   0        0        0     2474 2021-11-16 00:47:29.126136 octopus-sensing-4.0.1/octopus_sensing/devices/device.py
--rw-r--r--   0        0        0     6140 2021-12-15 06:55:13.533285 octopus-sensing-4.0.1/octopus_sensing/devices/network_devices/http_device.py
--rw-r--r--   0        0        0     5333 2021-12-15 06:55:13.537285 octopus-sensing-4.0.1/octopus_sensing/devices/network_devices/socket_device.py
--rw-r--r--   0        0        0     2970 2021-11-16 00:47:29.126136 octopus-sensing-4.0.1/octopus_sensing/devices/open_vibe_streaming.py
--rw-r--r--   0        0        0    10264 2022-06-12 22:45:14.581331 octopus-sensing-4.0.1/octopus_sensing/devices/openbci_streaming.py
--rw-r--r--   0        0        0     3798 2023-03-15 02:49:37.500908 octopus-sensing-4.0.1/octopus_sensing/devices/realtime_data_device.py
--rw-r--r--   0        0        0    16069 2023-03-15 02:47:24.973388 octopus-sensing-4.0.1/octopus_sensing/devices/shimmer3_streaming.py
--rw-r--r--   0        0        0      908 2021-06-15 00:46:08.788642 octopus-sensing-4.0.1/octopus_sensing/preprocessing/__init__.py
--rw-r--r--   0        0        0     9318 2021-12-15 06:55:04.229264 octopus-sensing-4.0.1/octopus_sensing/preprocessing/openbci.py
--rw-r--r--   0        0        0     5569 2021-12-15 06:55:04.229264 octopus-sensing-4.0.1/octopus_sensing/preprocessing/openbci_brainflow.py
--rw-r--r--   0        0        0     9782 2023-03-15 02:13:19.401919 octopus-sensing-4.0.1/octopus_sensing/preprocessing/preprocess_devices.py
--rw-r--r--   0        0        0     8107 2021-11-19 01:23:57.615641 octopus-sensing-4.0.1/octopus_sensing/preprocessing/shimmer3.py
--rw-r--r--   0        0        0     9498 2021-12-15 06:55:04.245264 octopus-sensing-4.0.1/octopus_sensing/preprocessing/utils.py
--rw-r--r--   0        0        0      838 2021-11-16 00:47:29.130136 octopus-sensing-4.0.1/octopus_sensing/questionnaire/__init__.py
--rw-r--r--   0        0        0     6179 2021-11-19 01:15:41.861895 octopus-sensing-4.0.1/octopus_sensing/questionnaire/opinion_question.py
--rw-r--r--   0        0        0     1354 2021-11-16 00:47:29.138136 octopus-sensing-4.0.1/octopus_sensing/questionnaire/question.py
--rw-r--r--   0        0        0     6003 2021-11-16 00:47:29.150137 octopus-sensing-4.0.1/octopus_sensing/questionnaire/questionnaire.py
--rw-r--r--   0        0        0     3618 2021-11-16 00:47:29.150137 octopus-sensing-4.0.1/octopus_sensing/questionnaire/text_question.py
--rw-r--r--   0        0        0     1599 2022-06-10 02:05:46.879054 octopus-sensing-4.0.1/octopus_sensing/realtime_data_endpoint.py
--rw-r--r--   0        0        0      899 2021-11-18 05:55:31.419363 octopus-sensing-4.0.1/octopus_sensing/stimuli/__init__.py
--rw-r--r--   0        0        0     2382 2022-02-10 21:29:39.565850 octopus-sensing-4.0.1/octopus_sensing/stimuli/image_stimulus.py
--rw-r--r--   0        0        0     1088 2021-11-18 05:55:31.423363 octopus-sensing-4.0.1/octopus_sensing/stimuli/stimulus.py
--rw-r--r--   0        0        0     1283 2022-02-16 02:37:26.325088 octopus-sensing-4.0.1/octopus_sensing/stimuli/video_stimulus.py
--rw-r--r--   0        0        0      768 2020-12-08 03:09:47.838518 octopus-sensing-4.0.1/octopus_sensing/tests/__init__.py
--rw-r--r--   0        0        0     1992 2021-08-18 05:02:38.831410 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-00.csv
--rw-r--r--   0        0        0     1989 2021-08-18 05:02:44.559379 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-01.csv
--rw-r--r--   0        0        0     1511 2021-08-18 05:02:49.691350 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-02.csv
--rw-r--r--   0        0        0     1993 2021-08-18 05:02:53.691328 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep01.csv
--rw-r--r--   0        0        0     1994 2021-08-18 05:02:57.979304 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep02.csv
--rw-r--r--   0        0        0     1021 2021-08-18 05:03:07.883250 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep03.csv
--rw-r--r--   0        0        0      998 2021-08-18 05:03:10.955233 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-00.csv
--rw-r--r--   0        0        0      997 2021-08-18 05:03:14.483213 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-01.csv
--rw-r--r--   0        0        0      758 2021-08-18 05:03:33.447109 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-02.csv
--rw-r--r--   0        0        0     1001 2021-08-18 05:03:33.447109 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-01.csv
--rw-r--r--   0        0        0      999 2021-08-18 05:03:33.447109 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-02.csv
--rw-r--r--   0        0        0      511 2021-08-18 05:03:33.451109 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-03.csv
--rw-r--r--   0        0        0      300 2021-08-30 23:56:27.283000 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/gsr/gsr-20-cont-00.csv
--rw-r--r--   0        0        0      300 2021-08-30 23:56:27.385000 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/gsr/gsr-20-cont-01.csv
--rw-r--r--   0        0        0      300 2021-08-30 23:56:27.454000 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/gsr/gsr-20-cont-02.csv
--rw-r--r--   0        0        0      300 2021-08-30 23:56:37.798000 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/ppg/ppg-20-cont-00.csv
--rw-r--r--   0        0        0      300 2021-08-30 23:56:37.907000 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/ppg/ppg-20-cont-01.csv
--rw-r--r--   0        0        0      300 2021-08-30 23:56:37.960000 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/ppg/ppg-20-cont-02.csv
--rw-r--r--   0        0        0      300 2021-08-31 00:09:15.466000 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/gsr/gsr-20-sep01.csv
--rw-r--r--   0        0        0      300 2021-08-31 00:09:19.915000 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/gsr/gsr-20-sep02.csv
--rw-r--r--   0        0        0      300 2021-08-31 00:09:25.104000 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/gsr/gsr-20-sep03.csv
--rw-r--r--   0        0        0      300 2021-08-31 00:09:32.339000 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/ppg/ppg-20-sep01.csv
--rw-r--r--   0        0        0      300 2021-08-31 00:09:36.544000 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/ppg/ppg-20-sep02.csv
--rw-r--r--   0        0        0      300 2021-08-31 00:09:41.331000 octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/ppg/ppg-20-sep03.csv
--rw-r--r--   0        0        0    11792 2021-08-16 23:55:07.629704 octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/OpenBCI_16_continuous/OpenBCI-20-cont16.csv
--rw-r--r--   0        0        0     3462 2021-06-16 01:05:46.778365 octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep01.csv
--rw-r--r--   0        0        0     3813 2021-06-16 01:06:29.534207 octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep02.csv
--rw-r--r--   0        0        0     3171 2021-06-16 01:07:09.338061 octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep03.csv
--rw-r--r--   0        0        0     6488 2021-06-15 23:59:28.010010 octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/OpenBCI_8_continuous/OpenBCI-20-cont8.csv
--rw-r--r--   0        0        0     1899 2021-06-16 00:59:03.303862 octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-01.csv
--rw-r--r--   0        0        0     2086 2021-06-16 01:02:50.443017 octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-02.csv
--rw-r--r--   0        0        0     1748 2021-06-16 01:02:34.947075 octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-03.csv
--rw-r--r--   0        0        0     3445 2021-08-16 23:55:10.557787 octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/Shimmer_continuous/Shimmer-20-cont.csv
--rw-r--r--   0        0        0     1019 2021-06-16 01:10:56.233228 octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep01.csv
--rw-r--r--   0        0        0     1104 2021-06-16 01:11:42.117060 octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep02.csv
--rw-r--r--   0        0        0      932 2021-06-16 01:12:15.200939 octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep03.csv
--rw-r--r--   0        0        0     6170 2023-03-15 02:08:36.075229 octopus-sensing-4.0.1/octopus_sensing/tests/integration.py
--rw-r--r--   0        0        0     4198 2022-05-24 06:50:46.622856 octopus-sensing-4.0.1/octopus_sensing/tests/test_audio_streaming.py
--rw-r--r--   0        0        0     3758 2022-05-20 05:30:08.250089 octopus-sensing-4.0.1/octopus_sensing/tests/test_brainflow_streaming.py
--rw-r--r--   0        0        0     3274 2022-05-24 06:49:26.962799 octopus-sensing-4.0.1/octopus_sensing/tests/test_camera_streaming.py
--rw-r--r--   0        0        0     1717 2022-05-20 05:30:08.250089 octopus-sensing-4.0.1/octopus_sensing/tests/test_device_coordinator.py
--rw-r--r--   0        0        0     5286 2021-12-15 06:55:04.273264 octopus-sensing-4.0.1/octopus_sensing/tests/test_device_message_endpoint.py
--rw-r--r--   0        0        0     3481 2021-12-15 06:55:04.273264 octopus-sensing-4.0.1/octopus_sensing/tests/test_http_network_device.py
--rw-r--r--   0        0        0     8005 2021-08-30 23:59:50.554899 octopus-sensing-4.0.1/octopus_sensing/tests/test_preprocess.py
--rw-r--r--   0        0        0     2958 2021-12-15 06:55:04.273264 octopus-sensing-4.0.1/octopus_sensing/tests/test_socket_network_device.py
--rw-r--r--   0        0        0      955 2021-11-18 05:55:31.423363 octopus-sensing-4.0.1/octopus_sensing/windows/__init__.py
--rw-r--r--   0        0        0     2259 2021-11-25 20:15:14.808514 octopus-sensing-4.0.1/octopus_sensing/windows/image_window.py
--rw-r--r--   0        0        0     3076 2021-11-25 20:18:03.811225 octopus-sensing-4.0.1/octopus_sensing/windows/message_window.py
--rw-r--r--   0        0        0     3681 2021-12-07 20:15:43.372977 octopus-sensing-4.0.1/octopus_sensing/windows/timer_window.py
--rw-r--r--   0        0        0     1519 2023-03-24 09:06:51.563972 octopus-sensing-4.0.1/pyproject.toml
--rw-r--r--   0        0        0     5445 2023-03-29 00:57:12.883799 octopus-sensing-4.0.1/setup.py
--rw-r--r--   0        0        0     4303 2023-03-29 00:57:12.884125 octopus-sensing-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-08-21 08:41:09.800625 octopus-sensing-4.0.2/LICENSE
+-rw-r--r--   0        0        0     2863 2022-05-20 05:30:08.246089 octopus-sensing-4.0.2/README.md
+-rw-r--r--   0        0        0    11168 2020-08-17 23:48:22.186902 octopus-sensing-4.0.2/octopus_sensing/OpenVibe/csv2edf.xml
+-rw-r--r--   0        0        0    18650 2020-08-17 23:48:22.186902 octopus-sensing-4.0.2/octopus_sensing/OpenVibe/display-save-eeg-exp2.xml
+-rw-r--r--   0        0        0    18648 2020-08-17 23:48:22.186902 octopus-sensing-4.0.2/octopus_sensing/OpenVibe/display-save-eeg.xml
+-rw-r--r--   0        0        0      790 2023-06-01 11:27:56.875095 octopus-sensing-4.0.2/octopus_sensing/__init__.py
+-rw-r--r--   0        0        0      768 2020-12-08 03:09:47.654520 octopus-sensing-4.0.2/octopus_sensing/common/__init__.py
+-rw-r--r--   0        0        0     7612 2022-05-24 06:03:24.413484 octopus-sensing-4.0.2/octopus_sensing/common/endpoint_base.py
+-rw-r--r--   0        0        0     2261 2021-11-16 00:47:29.106136 octopus-sensing-4.0.2/octopus_sensing/common/message.py
+-rw-r--r--   0        0        0     3645 2021-11-16 00:47:29.110136 octopus-sensing-4.0.2/octopus_sensing/common/message_creators.py
+-rw-r--r--   0        0        0     7923 2023-06-01 10:51:19.874106 octopus-sensing-4.0.2/octopus_sensing/device_coordinator.py
+-rw-r--r--   0        0        0     4551 2021-11-28 21:09:44.826763 octopus-sensing-4.0.2/octopus_sensing/device_message_endpoint.py
+-rw-r--r--   0        0        0     1301 2021-11-18 05:55:31.419363 octopus-sensing-4.0.2/octopus_sensing/devices/__init__.py
+-rw-r--r--   0        0        0     8887 2023-03-15 02:47:16.173420 octopus-sensing-4.0.2/octopus_sensing/devices/audio_streaming.py
+-rw-r--r--   0        0        0     7303 2023-03-29 00:01:35.111275 octopus-sensing-4.0.2/octopus_sensing/devices/brainflow_openbci_streaming.py
+-rw-r--r--   0        0        0     9113 2023-03-24 06:35:43.977593 octopus-sensing-4.0.2/octopus_sensing/devices/brainflow_streaming.py
+-rw-r--r--   0        0        0    10893 2023-06-01 10:51:11.242158 octopus-sensing-4.0.2/octopus_sensing/devices/camera_streaming.py
+-rw-r--r--   0        0        0     1492 2021-11-16 00:47:29.126136 octopus-sensing-4.0.2/octopus_sensing/devices/common.py
+-rw-r--r--   0        0        0     2474 2021-11-16 00:47:29.126136 octopus-sensing-4.0.2/octopus_sensing/devices/device.py
+-rw-r--r--   0        0        0     6140 2021-12-15 06:55:13.533285 octopus-sensing-4.0.2/octopus_sensing/devices/network_devices/http_device.py
+-rw-r--r--   0        0        0     5333 2021-12-15 06:55:13.537285 octopus-sensing-4.0.2/octopus_sensing/devices/network_devices/socket_device.py
+-rw-r--r--   0        0        0     2970 2021-11-16 00:47:29.126136 octopus-sensing-4.0.2/octopus_sensing/devices/open_vibe_streaming.py
+-rw-r--r--   0        0        0    10264 2022-06-12 22:45:14.581331 octopus-sensing-4.0.2/octopus_sensing/devices/openbci_streaming.py
+-rw-r--r--   0        0        0     3798 2023-03-15 02:49:37.500908 octopus-sensing-4.0.2/octopus_sensing/devices/realtime_data_device.py
+-rw-r--r--   0        0        0    16069 2023-03-15 02:47:24.973388 octopus-sensing-4.0.2/octopus_sensing/devices/shimmer3_streaming.py
+-rw-r--r--   0        0        0      908 2021-06-15 00:46:08.788642 octopus-sensing-4.0.2/octopus_sensing/preprocessing/__init__.py
+-rw-r--r--   0        0        0     9318 2021-12-15 06:55:04.229264 octopus-sensing-4.0.2/octopus_sensing/preprocessing/openbci.py
+-rw-r--r--   0        0        0     5569 2021-12-15 06:55:04.229264 octopus-sensing-4.0.2/octopus_sensing/preprocessing/openbci_brainflow.py
+-rw-r--r--   0        0        0     9782 2023-03-15 02:13:19.401919 octopus-sensing-4.0.2/octopus_sensing/preprocessing/preprocess_devices.py
+-rw-r--r--   0        0        0     8107 2021-11-19 01:23:57.615641 octopus-sensing-4.0.2/octopus_sensing/preprocessing/shimmer3.py
+-rw-r--r--   0        0        0     9498 2021-12-15 06:55:04.245264 octopus-sensing-4.0.2/octopus_sensing/preprocessing/utils.py
+-rw-r--r--   0        0        0      838 2021-11-16 00:47:29.130136 octopus-sensing-4.0.2/octopus_sensing/questionnaire/__init__.py
+-rw-r--r--   0        0        0     6179 2021-11-19 01:15:41.861895 octopus-sensing-4.0.2/octopus_sensing/questionnaire/opinion_question.py
+-rw-r--r--   0        0        0     1354 2021-11-16 00:47:29.138136 octopus-sensing-4.0.2/octopus_sensing/questionnaire/question.py
+-rw-r--r--   0        0        0     6003 2021-11-16 00:47:29.150137 octopus-sensing-4.0.2/octopus_sensing/questionnaire/questionnaire.py
+-rw-r--r--   0        0        0     3618 2021-11-16 00:47:29.150137 octopus-sensing-4.0.2/octopus_sensing/questionnaire/text_question.py
+-rw-r--r--   0        0        0     1599 2023-06-01 10:51:16.854124 octopus-sensing-4.0.2/octopus_sensing/realtime_data_endpoint.py
+-rw-r--r--   0        0        0      899 2021-11-18 05:55:31.419363 octopus-sensing-4.0.2/octopus_sensing/stimuli/__init__.py
+-rw-r--r--   0        0        0     2382 2022-02-10 21:29:39.565850 octopus-sensing-4.0.2/octopus_sensing/stimuli/image_stimulus.py
+-rw-r--r--   0        0        0     1088 2021-11-18 05:55:31.423363 octopus-sensing-4.0.2/octopus_sensing/stimuli/stimulus.py
+-rw-r--r--   0        0        0     1283 2022-02-16 02:37:26.325088 octopus-sensing-4.0.2/octopus_sensing/stimuli/video_stimulus.py
+-rw-r--r--   0        0        0      768 2020-12-08 03:09:47.838518 octopus-sensing-4.0.2/octopus_sensing/tests/__init__.py
+-rw-r--r--   0        0        0     1992 2021-08-18 05:02:38.831410 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-00.csv
+-rw-r--r--   0        0        0     1989 2021-08-18 05:02:44.559379 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-01.csv
+-rw-r--r--   0        0        0     1511 2021-08-18 05:02:49.691350 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-02.csv
+-rw-r--r--   0        0        0     1993 2021-08-18 05:02:53.691328 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep01.csv
+-rw-r--r--   0        0        0     1994 2021-08-18 05:02:57.979304 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep02.csv
+-rw-r--r--   0        0        0     1021 2021-08-18 05:03:07.883250 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep03.csv
+-rw-r--r--   0        0        0      998 2021-08-18 05:03:10.955233 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-00.csv
+-rw-r--r--   0        0        0      997 2021-08-18 05:03:14.483213 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-01.csv
+-rw-r--r--   0        0        0      758 2021-08-18 05:03:33.447109 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-02.csv
+-rw-r--r--   0        0        0     1001 2021-08-18 05:03:33.447109 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-01.csv
+-rw-r--r--   0        0        0      999 2021-08-18 05:03:33.447109 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-02.csv
+-rw-r--r--   0        0        0      511 2021-08-18 05:03:33.451109 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-03.csv
+-rw-r--r--   0        0        0      300 2021-08-30 23:56:27.283000 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/gsr/gsr-20-cont-00.csv
+-rw-r--r--   0        0        0      300 2021-08-30 23:56:27.385000 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/gsr/gsr-20-cont-01.csv
+-rw-r--r--   0        0        0      300 2021-08-30 23:56:27.454000 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/gsr/gsr-20-cont-02.csv
+-rw-r--r--   0        0        0      300 2021-08-30 23:56:37.798000 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/ppg/ppg-20-cont-00.csv
+-rw-r--r--   0        0        0      300 2021-08-30 23:56:37.907000 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/ppg/ppg-20-cont-01.csv
+-rw-r--r--   0        0        0      300 2021-08-30 23:56:37.960000 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/ppg/ppg-20-cont-02.csv
+-rw-r--r--   0        0        0      300 2021-08-31 00:09:15.466000 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/gsr/gsr-20-sep01.csv
+-rw-r--r--   0        0        0      300 2021-08-31 00:09:19.915000 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/gsr/gsr-20-sep02.csv
+-rw-r--r--   0        0        0      300 2021-08-31 00:09:25.104000 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/gsr/gsr-20-sep03.csv
+-rw-r--r--   0        0        0      300 2021-08-31 00:09:32.339000 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/ppg/ppg-20-sep01.csv
+-rw-r--r--   0        0        0      300 2021-08-31 00:09:36.544000 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/ppg/ppg-20-sep02.csv
+-rw-r--r--   0        0        0      300 2021-08-31 00:09:41.331000 octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/ppg/ppg-20-sep03.csv
+-rw-r--r--   0        0        0    11792 2021-08-16 23:55:07.629704 octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/OpenBCI_16_continuous/OpenBCI-20-cont16.csv
+-rw-r--r--   0        0        0     3462 2021-06-16 01:05:46.778365 octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep01.csv
+-rw-r--r--   0        0        0     3813 2021-06-16 01:06:29.534207 octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep02.csv
+-rw-r--r--   0        0        0     3171 2021-06-16 01:07:09.338061 octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep03.csv
+-rw-r--r--   0        0        0     6488 2021-06-15 23:59:28.010010 octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/OpenBCI_8_continuous/OpenBCI-20-cont8.csv
+-rw-r--r--   0        0        0     1899 2021-06-16 00:59:03.303862 octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-01.csv
+-rw-r--r--   0        0        0     2086 2021-06-16 01:02:50.443017 octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-02.csv
+-rw-r--r--   0        0        0     1748 2021-06-16 01:02:34.947075 octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-03.csv
+-rw-r--r--   0        0        0     3445 2021-08-16 23:55:10.557787 octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/Shimmer_continuous/Shimmer-20-cont.csv
+-rw-r--r--   0        0        0     1019 2021-06-16 01:10:56.233228 octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep01.csv
+-rw-r--r--   0        0        0     1104 2021-06-16 01:11:42.117060 octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep02.csv
+-rw-r--r--   0        0        0      932 2021-06-16 01:12:15.200939 octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep03.csv
+-rw-r--r--   0        0        0     6170 2023-03-15 02:08:36.075229 octopus-sensing-4.0.2/octopus_sensing/tests/integration.py
+-rw-r--r--   0        0        0     4198 2022-05-24 06:50:46.622856 octopus-sensing-4.0.2/octopus_sensing/tests/test_audio_streaming.py
+-rw-r--r--   0        0        0     3758 2022-05-20 05:30:08.250089 octopus-sensing-4.0.2/octopus_sensing/tests/test_brainflow_streaming.py
+-rw-r--r--   0        0        0     3274 2022-05-24 06:49:26.962799 octopus-sensing-4.0.2/octopus_sensing/tests/test_camera_streaming.py
+-rw-r--r--   0        0        0     1717 2022-05-20 05:30:08.250089 octopus-sensing-4.0.2/octopus_sensing/tests/test_device_coordinator.py
+-rw-r--r--   0        0        0     5286 2021-12-15 06:55:04.273264 octopus-sensing-4.0.2/octopus_sensing/tests/test_device_message_endpoint.py
+-rw-r--r--   0        0        0     3481 2021-12-15 06:55:04.273264 octopus-sensing-4.0.2/octopus_sensing/tests/test_http_network_device.py
+-rw-r--r--   0        0        0     8005 2021-08-30 23:59:50.554899 octopus-sensing-4.0.2/octopus_sensing/tests/test_preprocess.py
+-rw-r--r--   0        0        0     2958 2021-12-15 06:55:04.273264 octopus-sensing-4.0.2/octopus_sensing/tests/test_socket_network_device.py
+-rw-r--r--   0        0        0      955 2021-11-18 05:55:31.423363 octopus-sensing-4.0.2/octopus_sensing/windows/__init__.py
+-rw-r--r--   0        0        0     2259 2021-11-25 20:15:14.808514 octopus-sensing-4.0.2/octopus_sensing/windows/image_window.py
+-rw-r--r--   0        0        0     3076 2021-11-25 20:18:03.811225 octopus-sensing-4.0.2/octopus_sensing/windows/message_window.py
+-rw-r--r--   0        0        0     3681 2021-12-07 20:15:43.372977 octopus-sensing-4.0.2/octopus_sensing/windows/timer_window.py
+-rw-r--r--   0        0        0     1519 2023-06-01 11:25:35.651792 octopus-sensing-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5445 2023-06-01 11:33:44.348008 octopus-sensing-4.0.2/setup.py
+-rw-r--r--   0        0        0     4303 2023-06-01 11:33:44.348313 octopus-sensing-4.0.2/PKG-INFO
```

### Comparing `octopus-sensing-4.0.1/LICENSE` & `octopus-sensing-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/README.md` & `octopus-sensing-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/OpenVibe/csv2edf.xml` & `octopus-sensing-4.0.2/octopus_sensing/OpenVibe/csv2edf.xml`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/OpenVibe/display-save-eeg-exp2.xml` & `octopus-sensing-4.0.2/octopus_sensing/OpenVibe/display-save-eeg-exp2.xml`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/OpenVibe/display-save-eeg.xml` & `octopus-sensing-4.0.2/octopus_sensing/OpenVibe/display-save-eeg.xml`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/__init__.py` & `octopus-sensing-4.0.2/octopus_sensing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 # Octopus Sensing is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with Octopus Sensing.
 # If not, see <https://www.gnu.org/licenses/>.
 
-__version__ = '4.0.0'
+__version__ = '4.0.2'
```

### Comparing `octopus-sensing-4.0.1/octopus_sensing/common/__init__.py` & `octopus-sensing-4.0.2/octopus_sensing/common/__init__.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/common/endpoint_base.py` & `octopus-sensing-4.0.2/octopus_sensing/common/endpoint_base.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/common/message.py` & `octopus-sensing-4.0.2/octopus_sensing/common/message.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/common/message_creators.py` & `octopus-sensing-4.0.2/octopus_sensing/common/message_creators.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/device_coordinator.py` & `octopus-sensing-4.0.2/octopus_sensing/device_coordinator.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/device_message_endpoint.py` & `octopus-sensing-4.0.2/octopus_sensing/device_message_endpoint.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/devices/__init__.py` & `octopus-sensing-4.0.2/octopus_sensing/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/devices/audio_streaming.py` & `octopus-sensing-4.0.2/octopus_sensing/devices/audio_streaming.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/devices/brainflow_openbci_streaming.py` & `octopus-sensing-4.0.2/octopus_sensing/devices/brainflow_openbci_streaming.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/devices/brainflow_streaming.py` & `octopus-sensing-4.0.2/octopus_sensing/devices/brainflow_streaming.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/devices/camera_streaming.py` & `octopus-sensing-4.0.2/octopus_sensing/devices/camera_streaming.py`

 * *Files 7% similar despite different names*

```diff
@@ -129,14 +129,15 @@
         print(f"Initialized video device [{self.name}]: {self._video_size}")
 
         while True:
             message = self.message_queue.get()
             if message is None:
                 continue
             if message.type == MessageType.START:
+                print("start camera")
                 if self._state == "START":
                     print("Video streaming has already started")
                 else:
                     self._frames = []
                     self._capture_times = []
                     if recording_thread is not None:
                         raise RuntimeError(
@@ -144,16 +145,18 @@
                             "A STOP message should be send before trying "
                             "to start a new video recording.".format(self.name)))
 
                     file_name = "{0}/{1}-{2}-{3}.avi".format(self.output_path,
                                                             self.name,
                                                             message.experiment_id,
                                                             str(message.stimulus_id).zfill(2))
+                    print("Starting the thread")
                     recording_event = threading.Event()
                     recording_event.set()
+                    print("recording_event", recording_event)
                     recording_thread = threading.Thread(
                         target=self._stream_loop, args=(file_name, recording_event), daemon=True)
                     recording_thread.start()
                     self._state = "START"
 
             elif message.type == MessageType.STOP:
                 if self._state == "STOP":
@@ -172,31 +175,30 @@
                 recording_event = None
                 break
 
         print("video terminated")
         self._video_capture.release()
 
     def _stream_loop(self, file_name: str, event: threading.Event):
+        print("Start stream camera")
         codec = cv2.VideoWriter_fourcc(*'XVID')
         try:
             while self._video_capture.isOpened:
                 if event.is_set():
                     ret, frame = self._video_capture.read()
                     if ret:
                         self._counter += 1
                         self._capture_times.append(time.time())
                         self._frames.append(frame)
                 else:
-                    time_diff = self._capture_times[-1]-self._capture_times[0]
-                    self._fps = \
-                        int(len(self._frames)/(time_diff))
-                    print("Recording frame per second", self._fps)
+                    fps = self._get_frame_rate()
+                    print("Recording frame per second", fps)
                     writer = cv2.VideoWriter(file_name,
                             codec,
-                            self._fps,
+                            fps,
                             self._video_size)
                     for frame in self._frames:
                         writer.write(frame)
                     writer.release()
                     break
 
         except Exception as error:
@@ -234,24 +236,37 @@
         Returns
         -------
         data: Dict[str, Any]
             The keys are `data` and `metadata`.  
             `data` is a list of records, or empty list if there's nothing.
             `metadata` is a dictionary of device metadata including `frame_rate` and `type` 
         '''
-
-        data = self._frames[-1 * duration * self._fps:]
-        metadata = {"frame_rate": self._fps,
+        fps = self._get_frame_rate()
+        print("len(self._frames)", len(self._frames))
+        data = self._frames[-1 * duration * fps:]
+        metadata = {"frame_rate": fps,
                     "type": self.__class__.__name__}
+        print("len(data)", len(data), fps, duration)
         if len(data) == 0:
             realtime_data = {"data": [],
                              "metadata": metadata}
         else:
             one_frame_per_seconds = []
             for i in range(duration):
-                if (i * self._fps) + 1 > len(data):
+                if (i * fps) + 1 > len(data):
                     break
-                one_frame_per_seconds.append(data[i * self._fps])
+                one_frame_per_seconds.append(data[i * fps])
         
             realtime_data = {"data": one_frame_per_seconds,
                              "metadata": metadata}
         return realtime_data
+
+    def _get_frame_rate(self):
+        time_diff = 1
+        i = 1
+        while time_diff < 5 and len(self._capture_times) > i:
+            time_diff = self._capture_times[-1] - self._capture_times[-(i+1)]
+            i += 1
+        fps = int(i/time_diff)
+        print("measured fps: ", fps)
+        return fps
+
```

### Comparing `octopus-sensing-4.0.1/octopus_sensing/devices/common.py` & `octopus-sensing-4.0.2/octopus_sensing/devices/common.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/devices/device.py` & `octopus-sensing-4.0.2/octopus_sensing/devices/device.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/devices/network_devices/http_device.py` & `octopus-sensing-4.0.2/octopus_sensing/devices/network_devices/http_device.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/devices/network_devices/socket_device.py` & `octopus-sensing-4.0.2/octopus_sensing/devices/network_devices/socket_device.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/devices/open_vibe_streaming.py` & `octopus-sensing-4.0.2/octopus_sensing/devices/open_vibe_streaming.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/devices/openbci_streaming.py` & `octopus-sensing-4.0.2/octopus_sensing/devices/openbci_streaming.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/devices/realtime_data_device.py` & `octopus-sensing-4.0.2/octopus_sensing/devices/realtime_data_device.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/devices/shimmer3_streaming.py` & `octopus-sensing-4.0.2/octopus_sensing/devices/shimmer3_streaming.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/preprocessing/__init__.py` & `octopus-sensing-4.0.2/octopus_sensing/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/preprocessing/openbci.py` & `octopus-sensing-4.0.2/octopus_sensing/preprocessing/openbci.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/preprocessing/openbci_brainflow.py` & `octopus-sensing-4.0.2/octopus_sensing/preprocessing/openbci_brainflow.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/preprocessing/preprocess_devices.py` & `octopus-sensing-4.0.2/octopus_sensing/preprocessing/preprocess_devices.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/preprocessing/shimmer3.py` & `octopus-sensing-4.0.2/octopus_sensing/preprocessing/shimmer3.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/preprocessing/utils.py` & `octopus-sensing-4.0.2/octopus_sensing/preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/questionnaire/__init__.py` & `octopus-sensing-4.0.2/octopus_sensing/questionnaire/__init__.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/questionnaire/opinion_question.py` & `octopus-sensing-4.0.2/octopus_sensing/questionnaire/opinion_question.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/questionnaire/question.py` & `octopus-sensing-4.0.2/octopus_sensing/questionnaire/question.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/questionnaire/questionnaire.py` & `octopus-sensing-4.0.2/octopus_sensing/questionnaire/questionnaire.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/questionnaire/text_question.py` & `octopus-sensing-4.0.2/octopus_sensing/questionnaire/text_question.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/realtime_data_endpoint.py` & `octopus-sensing-4.0.2/octopus_sensing/realtime_data_endpoint.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/stimuli/__init__.py` & `octopus-sensing-4.0.2/octopus_sensing/stimuli/__init__.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/stimuli/image_stimulus.py` & `octopus-sensing-4.0.2/octopus_sensing/stimuli/image_stimulus.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/stimuli/stimulus.py` & `octopus-sensing-4.0.2/octopus_sensing/stimuli/stimulus.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/stimuli/video_stimulus.py` & `octopus-sensing-4.0.2/octopus_sensing/stimuli/video_stimulus.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/__init__.py` & `octopus-sensing-4.0.2/octopus_sensing/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-00.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-00.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-01.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-01.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-02.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-02.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep01.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep01.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep02.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep02.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep03.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep03.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-00.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-00.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-01.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-01.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-02.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-02.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-01.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-01.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-02.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-02.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/OpenBCI_16_continuous/OpenBCI-20-cont16.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/OpenBCI_16_continuous/OpenBCI-20-cont16.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep01.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep01.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep02.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep02.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep03.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep03.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/OpenBCI_8_continuous/OpenBCI-20-cont8.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/OpenBCI_8_continuous/OpenBCI-20-cont8.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-01.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-01.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-02.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-02.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-03.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-03.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/Shimmer_continuous/Shimmer-20-cont.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/Shimmer_continuous/Shimmer-20-cont.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep01.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep01.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep02.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep02.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep03.csv` & `octopus-sensing-4.0.2/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep03.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/integration.py` & `octopus-sensing-4.0.2/octopus_sensing/tests/integration.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/test_audio_streaming.py` & `octopus-sensing-4.0.2/octopus_sensing/tests/test_audio_streaming.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/test_brainflow_streaming.py` & `octopus-sensing-4.0.2/octopus_sensing/tests/test_brainflow_streaming.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/test_camera_streaming.py` & `octopus-sensing-4.0.2/octopus_sensing/tests/test_camera_streaming.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/test_device_coordinator.py` & `octopus-sensing-4.0.2/octopus_sensing/tests/test_device_coordinator.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/test_device_message_endpoint.py` & `octopus-sensing-4.0.2/octopus_sensing/tests/test_device_message_endpoint.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/test_http_network_device.py` & `octopus-sensing-4.0.2/octopus_sensing/tests/test_http_network_device.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/test_preprocess.py` & `octopus-sensing-4.0.2/octopus_sensing/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/tests/test_socket_network_device.py` & `octopus-sensing-4.0.2/octopus_sensing/tests/test_socket_network_device.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/windows/__init__.py` & `octopus-sensing-4.0.2/octopus_sensing/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/windows/image_window.py` & `octopus-sensing-4.0.2/octopus_sensing/windows/image_window.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/windows/message_window.py` & `octopus-sensing-4.0.2/octopus_sensing/windows/message_window.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/octopus_sensing/windows/timer_window.py` & `octopus-sensing-4.0.2/octopus_sensing/windows/timer_window.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.1/pyproject.toml` & `octopus-sensing-4.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "octopus-sensing"
-version = "4.0.1"
+version = "4.0.2"
 description = "Library for recording data synchronously from different physiological sensors"
 authors = ["Nastaran Saffaryazdi <nsaffar@gmail.com>", "Aidin Gharibnavaz <aidin@aidinhut.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://octopus-sensing.nastaran-saffar.me"
 repository = "https://github.com/octopus-sensing/octopus-sensing"
 keywords = ["sensors", "eeg", "gsr", "recorder"]
```

### Comparing `octopus-sensing-4.0.1/setup.py` & `octopus-sensing-4.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 extras_require = \
 {':sys_platform != "win32"': ['PyGObject==3.40.1'],
  ':sys_platform == "linux"': ['bluepy>=1.3.0,<2.0.0']}
 
 setup_kwargs = {
     'name': 'octopus-sensing',
-    'version': '4.0.1',
+    'version': '4.0.2',
     'description': 'Library for recording data synchronously from different physiological sensors',
     'long_description': '<h2 align="center">Octopus Sensing</h2>\n<p align="center">\n  <img src="https://octopus-sensing.nastaran-saffar.me/_static/octopus-sensing-logo-small.png" alt="Octopus Sensing Logo">\n</p>\n<p align="center">\n  <img src="https://img.shields.io/github/workflow/status/octopus-sensing/octopus-sensing/Python%20Check?label=checks" alt="GitHub Workflow Status">\n  <img src="https://img.shields.io/codecov/c/gh/octopus-sensing/octopus-sensing" alt="Codecov">\n  <img src="https://img.shields.io/pypi/v/octopus-sensing" alt="PyPI">\n  <img src="https://img.shields.io/pypi/l/octopus-sensing" alt="PyPI - License">\n</p>\n\nOctopus Sensing is a tool to help you run scientific experiments that involve recording data synchronously from\nmultiple sources in human-computer interaction studies. You write steps of an experiment scenario, for example showing a stimulus and then a questionnaire. The tool takes care of the rest.\n\nIt can collect data from multiple devices such as OpenBCI EEG headset, Shimmer sensor (GSR and PPG),\nVideo and Audio and so forth simultaneously. Data collection can be started and stopped synchronously across all devices.\nCollected data will be tagged with the timestamp of the start and stop of the experiment, the ID of\nthe experiment, etc.\n\nThe aim is to make the scripting interface so simple that people with minimum or no software\ndevelopment skills can define experiment scenarios with no effort.\nAlso, this tool can be used as the base structure for creating real-time data processing systems like systems with capabilities of recognizing emotions, stress, cognitive load, or analyzing human behaviors.\n\n\n**To see the full documentation visit the [Octopus Sensing website](https://octopus-sensing.nastaran-saffar.me/).**\n\nWhen using the package in your research, please cite:\n-----------------------------------------------------\n\nSaffaryazdi, N., Gharibnavaz, A., & Billinghurst, M. (2022). Octopus Sensing: A Python library for human behavior studies. Journal of Open Source Software, 7(71), 4045.\n\nMain features\n--------------\n\n* Controls data recording from multiple sources using a simple unified interface\n* Tags an event on collected data, such as the start of an experiment, and events during the experiment, etc.\n* Can show stimuli (images and videos) and questionnaires\n* Monitoring interface that visualizes collected data in real-time\n* Offline visualization of data from multiple sources simultanously\n\nCopyright\n---------\nCopyright © 2020-2022 Nastaran Saffaryazdi, Aidin Gharibnavaz\n\nThis program is free software: you can redistribute it and/or modify it under the terms of the GNU\nGeneral Public License as published by the Free Software Foundation, either version 3 of the\nLicense, or (at your option) any later version.\n\nSee [License file](https://github.com/nastaran62/octopus-sensing/blob/master/LICENSE) for full terms.\n',
     'author': 'Nastaran Saffaryazdi',
     'author_email': 'nsaffar@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://octopus-sensing.nastaran-saffar.me',
```

### Comparing `octopus-sensing-4.0.1/PKG-INFO` & `octopus-sensing-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octopus-sensing
-Version: 4.0.1
+Version: 4.0.2
 Summary: Library for recording data synchronously from different physiological sensors
 Home-page: https://octopus-sensing.nastaran-saffar.me
 License: GPL-3.0-or-later
 Keywords: sensors,eeg,gsr,recorder
 Author: Nastaran Saffaryazdi
 Author-email: nsaffar@gmail.com
 Requires-Python: >=3.7.1,<4.0
```

